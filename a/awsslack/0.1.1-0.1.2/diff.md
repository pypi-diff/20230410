# Comparing `tmp/awsslack-0.1.1.tar.gz` & `tmp/awsslack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsslack-0.1.1.tar", max compression
+gzip compressed data, was "awsslack-0.1.2.tar", max compression
```

## Comparing `awsslack-0.1.1.tar` & `awsslack-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1032 2023-03-24 19:56:28.581324 awsslack-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/__init__.py
--rw-r--r--   0        0        0       88 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/__main__.py
--rw-r--r--   0        0        0     5859 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/code_build.py
--rw-r--r--   0        0        0    12550 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/code_deploy.py
--rw-r--r--   0        0        0        0 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/commands/__init__.py
--rw-r--r--   0        0        0     6561 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/commands/config.py
--rw-r--r--   0        0        0     1243 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/main.py
--rw-r--r--   0        0        0        0 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/utils/__init__.py
--rw-r--r--   0        0        0     5859 2023-03-24 19:56:28.581324 awsslack-0.1.1/awsslack/utils/code_build.py
--rw-r--r--   0        0        0    12550 2023-03-24 19:56:28.581324 awsslack-0.1.1/awsslack/utils/code_deploy.py
--rw-r--r--   0        0        0      848 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/utils/yaml.py
--rw-r--r--   0        0        0      709 2023-04-09 18:44:27.094832 awsslack-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 awsslack-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1691 2023-04-10 19:48:19.044052 awsslack-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 18:51:06.063459 awsslack-0.1.2/awsslack/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:51:06.083459 awsslack-0.1.2/awsslack/commands/__init__.py
+-rw-r--r--   0        0        0      778 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/commands/codebuild.py
+-rw-r--r--   0        0        0     1208 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/commands/codedeploy.py
+-rw-r--r--   0        0        0     8812 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/commands/config.py
+-rw-r--r--   0        0        0     2819 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/main.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:51:06.067458 awsslack-0.1.2/awsslack/utils/__init__.py
+-rw-r--r--   0        0        0     5496 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/utils/code_build.py
+-rw-r--r--   0        0        0    10841 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/utils/code_deploy.py
+-rw-r--r--   0        0        0      884 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/utils/yaml.py
+-rw-r--r--   0        0        0      709 2023-04-10 19:56:40.872798 awsslack-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 awsslack-0.1.2/PKG-INFO
```

### Comparing `awsslack-0.1.1/awsslack/code_build.py` & `awsslack-0.1.2/awsslack/utils/code_build.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,80 @@
-import argparse
-import json
+from __future__ import annotations
+
 import time
 import urllib.parse
 from collections import OrderedDict
-from datetime import datetime
 
 import boto3
 
+from awsslack.commands.config import AWSConfig, SlackConfig
 from progress_bar import SlackProgress
 
 
-def main(args: argparse.Namespace) -> None:
-    slack_token = args.slack_token
-    channel_name = args.channel_name
-    project_name = args.project_name
-    iam_slack_usernames_mapping = args.iam_slack_usernames_mapping
-    aws_region = args.aws_region
-
-    codebuild_client = boto3.client("codebuild")
+def execute_cb(
+    cb_conf: dict[str, str],
+    slack_conf: SlackConfig,
+    aws_conf: AWSConfig,
+) -> int:
+    project_name = cb_conf["name"]
+
+    # Not Live Yet!
+    # breakpoint()
+    return 1
 
-    iam_slack_usernames_mapping = json.loads(iam_slack_usernames_mapping)
+    # get IAM User
+    print("fetching IAM User...")
     sts_client = boto3.client("sts")
     response = sts_client.get_caller_identity()
     iam_username = response["Arn"].partition("/")[-1]
     iam_account_id = response["Account"]
-    if iam_slack_usernames_mapping.get(iam_username):
-        iam_username_log_message = f"<@{iam_slack_usernames_mapping[iam_username]}>"
+
+    # get Slack User
+    print("fetching Slack User...")
+    if slack_conf.iam_slack_users.get(iam_username):
+        iam_username_log_message = f"<@{slack_conf.iam_slack_users[iam_username]}>"
     else:
         iam_username_log_message = f"'AWS User {iam_username}'"
 
-    build_response_data: dict = codebuild_client.start_build(
+    # start Build
+    print("Starting CodeBuild...")
+    codebuild_client = boto3.client("codebuild")
+    build_response_data_init: dict = codebuild_client.start_build(
         projectName=project_name,
     )
-    build_id = build_response_data["build"]["id"]
-    build_status = build_response_data["build"]["buildStatus"]
-    build_phases = build_response_data["build"]["phases"]
+    build_id = build_response_data_init["build"]["id"]
+    build_status = build_response_data_init["build"]["buildStatus"]
+    build_phases = build_response_data_init["build"]["phases"]
+    build_phases_updated_in_slack_mapping = OrderedDict()
+    for _start_build_phase in build_phases:
+        build_phases_updated_in_slack_mapping[_start_build_phase["phaseType"]] = False
 
-    # Create AWS CodeBuild Console URL
+    # generate AWS CodeBuild Console URL
     build_id_url_encoded = urllib.parse.quote_plus(build_id)
-    code_build_console_link = f"https://{aws_region}.console.aws.amazon.com/codesuite/codebuild/{iam_account_id}/projects/{project_name}/build/{build_id_url_encoded}/phase?region={aws_region}"
+    code_build_console_link = f"https://{aws_conf.region}.console.aws.amazon.com/codesuite/codebuild/{iam_account_id}/projects/{project_name}/build/{build_id_url_encoded}/phase?region={aws_conf.region}"
 
     # Initialize Slack here
     prefix = f"<{code_build_console_link}|*CodeBuild: {project_name}*>"
-    sp = SlackProgress(token=slack_token, channel=channel_name, prefix=prefix)
-    current_percentage_int = 0
-
-    build_phases_updated_in_slack_mapping = OrderedDict()
-    for _start_build_phase in build_phases:
-        build_phases_updated_in_slack_mapping[_start_build_phase["phaseType"]] = False
+    sp = SlackProgress(
+        token=slack_conf.token,
+        channel=slack_conf.channel_name,
+        prefix=prefix,
+    )
+    current_percentage = 0.0
 
     # Initialize Slack ProgressBar here
     pbar = sp.new()
     log_message = f"Build: *{project_name}*, BuildStatus=`{build_status}`, Initiated by: {iam_username_log_message}"
-    pbar.pos = current_percentage_int
+    pbar.pos = current_percentage
     pbar.log(log_message)
 
+    # send updates to Slack
     is_build_running = True
     while is_build_running:
-        print(f"Sleeping for 5 sec... {datetime.now()}")
+        # Sleeping for 5 sec
         time.sleep(5)
 
         build_response_data: dict = codebuild_client.batch_get_builds(ids=[build_id])
 
         build_status = build_response_data["builds"][0]["buildStatus"]
         if build_status != "IN_PROGRESS":
             # break here and update slack finally.
@@ -84,69 +97,56 @@
         for _, (_build_phase, _is_build_phase_updated_in_slack) in enumerate(
             list(build_phases_updated_in_slack_mapping.items()),
             start=1,
         ):
             if _is_build_phase_updated_in_slack:
                 continue
 
-            print(f"updating {_build_phase} in slack...")
+            print(f"updating slack, Build Phase: {_build_phase}")
             build_phase_found = False
             phases_found = []
             for current_build_phase in current_build_phases:
                 phaseType = current_build_phase["phaseType"]
                 phases_found.append(phaseType)
 
                 if _build_phase != phaseType:
                     continue
 
                 build_phase_found = True
                 break
 
             if not build_phase_found:
-                print(
-                    f"ughh, Build Phase {_build_phase} not found, found {phases_found} instead",
-                )
+                # Build Phase not found, try again
                 break
 
             if not current_build_phase.get("phaseStatus"):
-                print(f"ughh, Build Phase {_build_phase} has no status yet.")
+                # Build Phase has no status yet, try again
                 break
 
             phase_type, phase_status = (
                 current_build_phase["phaseType"],
                 current_build_phase["phaseStatus"],
             )
             log_message = f"Build's Phase: {phase_type}, PhaseStatus=*{phase_status}*"
-            current_percentage_int += 100 / 11
-            current_percentage_int = round(current_percentage_int, 1)
-            pbar.pos = current_percentage_int
+            current_percentage += 100 / 11
+            current_percentage = round(current_percentage, 1)
+            pbar.pos = current_percentage
             pbar.log(log_message)
             build_phases_updated_in_slack_mapping[_build_phase] = True
 
+    # send final update to Slack - reply in the thread
     build_phases_contexts = ""
     for current_build_phase in current_build_phases:
         if not current_build_phase.get("contexts"):
             continue
-
         for context in current_build_phase.get("contexts"):
             if context.get("message"):
                 build_phases_contexts += f"\n\nBuild's Phase: *{current_build_phase['phaseType']}* Context: `{context.get('message')}`."
-
-    log_message = (
-        f"{prefix} *{build_status}!* {iam_username_log_message} {build_phases_contexts}"
+    pbar.log_thread(
+        f"{prefix} *{build_status}!* {iam_username_log_message} {build_phases_contexts}",
     )
-    pbar.log_thread(log_message)
 
+    return 0
 
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        prog="aws-deployments-test",
-        description="Pushes updates to slack about a CodeBuild",
-    )
-    parser.add_argument("--slack_token", type=str)
-    parser.add_argument("--channel_name", type=str)
-    parser.add_argument("--project_name", type=str)
-    parser.add_argument("--iam_slack_usernames_mapping", default="{}", type=str)
-    parser.add_argument("--aws_region", type=str)
-    args = parser.parse_args()
 
-    main(args=args)
+def update_sources_i(cb_conf: dict[str, str]) -> None:
+    raise NotImplementedError
```

### Comparing `awsslack-0.1.1/awsslack/code_deploy.py` & `awsslack-0.1.2/awsslack/utils/code_deploy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,86 @@
-import argparse
-import json
+from __future__ import annotations
+
 import subprocess
 import time
 from collections import OrderedDict
-from datetime import datetime
+from typing import Any
 
 import boto3
 
+from awsslack.commands.config import AWSConfig, CodeDeployConfigApp, SlackConfig
 from progress_bar import SlackProgress
 
 
-def main(args: argparse.Namespace) -> None:
-    slack_token = args.slack_token
-    channel_name = args.channel_name
-    project_name = args.project_name
-    iam_slack_usernames_mapping = args.iam_slack_usernames_mapping
-    aws_region = args.aws_region
-    slack_link = args.slack_link
-    commit_id = args.commit_id
-    ssh_git_repo_url = args.ssh_git_repo_url
-    git_repo_branch = args.git_repo_branch
-    deployment_group_name = args.deployment_group_name
-    repository_name = args.repository_name
-
-    if not commit_id:
-        commit_id = subprocess.Popen(
-            f'echo "$(git ls-remote {ssh_git_repo_url} | grep refs/heads/{git_repo_branch} | cut -f 1)"',
-            shell=True,
-            stdout=subprocess.PIPE,
-        ).stdout.read()
-        commit_id = commit_id.decode("utf-8")
-        commit_id = commit_id.strip("\n")
-
-    codedeploy_client = boto3.client("codedeploy")
+def execute_cd(
+    cd_conf: CodeDeployConfigApp,
+    slack_conf: SlackConfig,
+    aws_conf: AWSConfig,
+    commit: str,
+) -> int:
+    project_name = cd_conf.app
+    deployment_group = cd_conf.group
+    github_repository = cd_conf.repo
+
+    # Not Live Yet!
+    # breakpoint()
+    return 1
 
-    iam_slack_usernames_mapping = json.loads(iam_slack_usernames_mapping)
+    # get IAM User
+    print("fetching IAM User...")
     sts_client = boto3.client("sts")
     response = sts_client.get_caller_identity()
     iam_username = response["Arn"].partition("/")[-1]
-    if iam_slack_usernames_mapping.get(iam_username):
-        iam_username_log_message = f"<@{iam_slack_usernames_mapping[iam_username]}>"
+    iam_account_id = response["Account"]
+
+    # get Slack User
+    print("fetching Slack User...")
+    if slack_conf.iam_slack_users.get(iam_username):
+        iam_username_log_message = f"<@{slack_conf.iam_slack_users[iam_username]}>"
     else:
         iam_username_log_message = f"'AWS User {iam_username}'"
 
-    deployment_id = args.deployment_id
-    if not deployment_id:
-        print(f"creating deployment for commit_id: {commit_id}...")
-        deploy_response_data: dict = codedeploy_client.create_deployment(
-            applicationName=project_name,
-            deploymentGroupName=deployment_group_name,
-            deploymentConfigName="CodeDeployDefault.AllAtOnce",
-            description=f"Initiated by code_deploy.py script - by {iam_username}",
-            revision={
-                "revisionType": "GitHub",
-                "gitHubLocation": {
-                    "repository": f"{repository_name}/{project_name}",
-                    "commitId": commit_id,
-                },
+    # create Deployment
+    print(f"Creating deployment for commit: {commit}")
+    codedeploy_client = boto3.client("codedeploy")
+    deploy_response_data: dict = codedeploy_client.create_deployment(
+        applicationName=project_name,
+        deploymentGroupName=deployment_group,
+        deploymentConfigName="CodeDeployDefault.AllAtOnce",
+        description=f"Initiated using `awsslack` package - by {iam_username}",
+        revision={
+            "revisionType": "GitHub",
+            "gitHubLocation": {
+                "repository": github_repository,
+                "commitId": commit,
             },
-            fileExistsBehavior="OVERWRITE",
-        )
-        deployment_id = deploy_response_data["deploymentId"]
-    print(f"deployment_id: {deployment_id}...")
+        },
+        fileExistsBehavior="OVERWRITE",
+    )
+    deployment_id = deploy_response_data["deploymentId"]
 
-    # Get Deployment
+    # get Deployment
     deploy_response_data = codedeploy_client.get_deployment(deploymentId=deployment_id)
     deployment_info = deploy_response_data["deploymentInfo"]
     deployment_status = deployment_info["status"]
 
-    # List Deployment Instances
+    # list Deployment Instances
     is_deployment_ready = False
     while not is_deployment_ready:
         try:
             response = codedeploy_client.list_deployment_instances(
                 deploymentId=deployment_id,
             )
             instances_list = response["instancesList"]
             is_deployment_ready = True
-        except Exception as err:
-            print(err)
-            print(f"deployment not ready, sleeping for 5 sec")
+        except Exception:
+            # sleeping for 5 sec
             time.sleep(5)
 
-    deploy_phases_updated_in_slack_mapping = {}
+    deploy_phases_updated_in_slack_mapping: dict[str, Any] = {}
     for instance in instances_list:
         deploy_phases_updated_in_slack_mapping[instance] = OrderedDict()
 
     # Batch Get Deployment Targets
     response = codedeploy_client.batch_get_deployment_instances(
         deploymentId=deployment_id,
         instanceIds=instances_list,
@@ -101,43 +95,37 @@
             lifecycle_event_name = deployment_instance_lifecycle_event[
                 "lifecycleEventName"
             ]
             deploy_phases_updated_in_slack_mapping[_instance_id][
                 lifecycle_event_name
             ] = False
 
-    # Create AWS CodeDeploy Console URL
-    code_deploy_console_link = f"https://{aws_region}.console.aws.amazon.com/codesuite/codedeploy/deployments/{deployment_id}?region={aws_region}"
+    # generate AWS CodeDeploy Console URL
+    code_deploy_console_link = f"https://{aws_conf.region}.console.aws.amazon.com/codesuite/codedeploy/deployments/{deployment_id}?region={aws_conf.region}"
 
     # Initialize Slack here
-    prefix = f"<{code_deploy_console_link}|*CodeDeploy: {project_name} - {deployment_group_name}*>"
-    if slack_link:
-        slack_link_pts = slack_link.rpartition("/")[-1]
-        msg_ts = f"{(slack_link_pts.split('p')[-1])[:-6]}.{(slack_link_pts.split('p')[-1])[-6:]}"
-        sp = SlackProgress(
-            token=slack_token,
-            channel=channel_name,
-            prefix=prefix,
-            msg_ts=msg_ts,
-        )
-    else:
-        sp = SlackProgress(token=slack_token, channel=channel_name, prefix=prefix)
-    current_percentage_int = 0
+    prefix = f"<{code_deploy_console_link}|*CodeDeploy: {project_name} - {deployment_group}*>"
+    sp = SlackProgress(
+        token=slack_conf.token,
+        channel=slack_conf.channel_name,
+        prefix=prefix,
+    )
+    current_percentage_int = 0.0
 
     # Initialize Slack ProgressBar here
     pbar = sp.new()
     log_message = f"Build: *{project_name}*, DeploymentStatus=`{deployment_status}`, Initiated by: {iam_username_log_message}"
     pbar.pos = current_percentage_int
     pbar.log(log_message)
 
     is_deployment_in_progress = (
         True if deployment_status not in ["Succeeded", "Failed", "Stopped"] else False
     )
     while is_deployment_in_progress:
-        print(f"Sleeping for 5 sec... {datetime.now()}")
+        # Sleeping for 5 sec
         time.sleep(5)
 
         ## Update new phases
         # Get Deployment
         deploy_response_data = codedeploy_client.get_deployment(
             deploymentId=deployment_id,
         )
@@ -206,15 +194,15 @@
             for (
                 _deploy_phase,
                 _is_deploy_phase_updated_in_slack,
             ) in instance_phases.items():
                 if _is_deploy_phase_updated_in_slack:
                     continue
 
-                print(f"updating {_deploy_phase} in slack...")
+                print(f"updating slack, Deploy Phase: {_deploy_phase}")
                 phases_found = []
                 break_main = False
                 for deployment_instance in response["instancesSummary"]:
                     if break_main:
                         break
 
                     deployment_instance_id = deployment_instance["instanceId"]
@@ -232,73 +220,54 @@
                             "lifecycleEventName"
                         ]
                         # lifecycle_event_status = deployment_instance_lifecycle_event["status"]
                         phases_found.append(lifecycle_event_name)
                         if _deploy_phase != lifecycle_event_name:
                             continue
 
-                        deploy_phase_found = True
                         break_main = True
                         phase_type, phase_status, instance_label = (
                             lifecycle_event_name,
                             deployment_instance_lifecycle_event.get("status"),
                             deployment_instance.get("instanceType"),
                         )
 
                         if not phase_status:
-                            print(
-                                f"ughh, Deploy Phase {_deploy_phase} has no status yet.",
-                            )
+                            # Deploy Phase has no status yet
                             break
 
                         if phase_status in ["Pending", "InProgress"]:
-                            print(
-                                f"skipping, phase {phase_type} has status {phase_status}",
-                            )
+                            # skipping, phase is either Pending or InProgress
                             continue
 
                         log_message = f"Deploy: *{project_name}*, DeployentStatus=`{deployment_status}`"
-                        print(f"instance_label: {instance_label}")
 
                         if instance_label == "Blue":
                             log_message_emoji = ":blue_book:"
                         else:
                             log_message_emoji = ":green_book:"
 
-                        instance_link = f"https://{aws_region}.console.aws.amazon.com/ec2/v2/home?region={aws_region}#Instances:instanceId={_instance_id}"
+                        instance_link = f"https://{aws_conf.region}.console.aws.amazon.com/ec2/v2/home?region={aws_conf.region}#Instances:instanceId={_instance_id}"
                         log_message = f"Deployment's Phase: {phase_type}, [{log_message_emoji} <{instance_link}|*{_instance_id}*>] PhaseStatus=*{phase_status}*"
                         current_percentage_int += 100 / 13
                         current_percentage_int = round(current_percentage_int, 1)
                         pbar.pos = current_percentage_int
                         pbar.log(log_message)
                         deploy_phases_updated_in_slack_mapping[_instance_id][
                             _deploy_phase
                         ] = True
                         break
 
     log_message = f"{prefix} *{deployment_status}!* {iam_username_log_message}"
     pbar.log_thread(log_message)
 
+    return 0
 
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        prog="aws-deployments-test",
-        description="Pushes updates to slack about a CodeDeploy",
-    )
-    parser.add_argument("--slack_token", type=str)
-    parser.add_argument("--channel_name", type=str)
-    parser.add_argument("--iam_slack_usernames_mapping", type=str)
-    parser.add_argument("--aws_region", default="eu-west-1", type=str)
-    parser.add_argument("--slack_link", type=str)
-
-    parser.add_argument("--project_name", type=str)
-    parser.add_argument("--deployment_group_name", type=str)
-    parser.add_argument("--deployment_id", default="", type=str)
-
-    parser.add_argument("--commit_id", default="", type=str)
-    parser.add_argument("--ssh_git_repo_url", type=str)
-    parser.add_argument("--git_repo_branch", type=str)
-    parser.add_argument("--repository_name", type=str)
 
-    args = parser.parse_args()
+def get_commit_remote(repo: str, branch: str) -> str:
+    ssh_git_repo_url = f"git@github.com:{repo}.git"
+
+    cmd = f'echo "$(git ls-remote {ssh_git_repo_url} | grep refs/heads/{branch} | cut -f 1)"'
+    p_stdout = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE).stdout
+    assert p_stdout, "can't fetch commit, please consider providing'--commit'"
 
-    main(args=args)
+    return p_stdout.read().decode("utf-8").strip("\n")
```

### Comparing `awsslack-0.1.1/awsslack/utils/yaml.py` & `awsslack-0.1.2/awsslack/utils/yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from typing import Any
 
 import yaml
 
 CONFIG_FILE_PATH = Path(f"{Path.home()}/.aws/.awsslack-config.yaml")
```

### Comparing `awsslack-0.1.1/pyproject.toml` & `awsslack-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsslack"
-version = "0.1.1"
+version = "0.1.2"
 description = "AWS CodeBuild/CodeDeploy triggers & updates to Slack with a cool Progress Bar!"
 authors = ["Saurabh Chopra <Saurabh.Chopra.2021@live.rhul.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 exclude = ["./scripts", "./tests"]
 
 [tool.poetry.scripts]
```

