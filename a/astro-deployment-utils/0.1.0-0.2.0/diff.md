# Comparing `tmp/astro_deployment_utils-0.1.0.tar.gz` & `tmp/astro_deployment_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_deployment_utils-0.1.0.tar", max compression
+gzip compressed data, was "astro_deployment_utils-0.2.0.tar", max compression
```

## Comparing `astro_deployment_utils-0.1.0.tar` & `astro_deployment_utils-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0        0 2023-04-10 10:01:41.152578 astro_deployment_utils-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-10 11:37:57.519380 astro_deployment_utils-0.1.0/deployment_utils/__init__.py
--rw-r--r--   0        0        0     4702 2023-04-10 11:00:59.470692 astro_deployment_utils-0.1.0/deployment_utils/api_handler.py
--rw-r--r--   0        0        0     1490 2023-03-20 07:49:45.608000 astro_deployment_utils-0.1.0/deployment_utils/cloud_config.py
--rw-r--r--   0        0        0     6462 2023-03-30 05:21:25.276000 astro_deployment_utils-0.1.0/deployment_utils/cloud_constants.py
--rw-r--r--   0        0        0    15853 2023-04-10 11:37:57.522961 astro_deployment_utils-0.1.0/deployment_utils/cloud_utils.py
--rw-r--r--   0        0        0      691 2022-12-28 12:06:09.234000 astro_deployment_utils-0.1.0/deployment_utils/log.py
--rw-r--r--   0        0        0    22444 2023-04-10 10:10:08.016322 astro_deployment_utils-0.1.0/deployment_utils/logs/execution_logfile.log
--rw-r--r--   0        0        0     4038 2022-12-27 18:51:32.682000 astro_deployment_utils-0.1.0/deployment_utils/models.py
--rw-r--r--   0        0        0      399 2023-04-10 12:01:45.538302 astro_deployment_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 astro_deployment_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      833 2023-04-10 15:23:00.667889 astro_deployment_utils-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 11:37:57.519380 astro_deployment_utils-0.2.0/deployment_utils/__init__.py
+-rw-r--r--   0        0        0     4702 2023-04-10 11:00:59.470692 astro_deployment_utils-0.2.0/deployment_utils/api_handler.py
+-rw-r--r--   0        0        0     2959 2023-04-10 14:40:49.067363 astro_deployment_utils-0.2.0/deployment_utils/astro_cli_utils.py
+-rw-r--r--   0        0        0     1490 2023-03-20 07:49:45.608000 astro_deployment_utils-0.2.0/deployment_utils/cloud_config.py
+-rw-r--r--   0        0        0     6462 2023-03-30 05:21:25.276000 astro_deployment_utils-0.2.0/deployment_utils/cloud_constants.py
+-rw-r--r--   0        0        0    16636 2023-04-10 15:24:25.982985 astro_deployment_utils-0.2.0/deployment_utils/cloud_utils.py
+-rw-r--r--   0        0        0     1371 2023-04-10 13:04:35.177365 astro_deployment_utils-0.2.0/deployment_utils/helpers.py
+-rw-r--r--   0        0        0    10664 2023-04-10 12:55:44.302453 astro_deployment_utils-0.2.0/deployment_utils/io.py
+-rw-r--r--   0        0        0      691 2022-12-28 12:06:09.234000 astro_deployment_utils-0.2.0/deployment_utils/log.py
+-rw-r--r--   0        0        0    22444 2023-04-10 10:10:08.016322 astro_deployment_utils-0.2.0/deployment_utils/logs/execution_logfile.log
+-rw-r--r--   0        0        0     4038 2022-12-27 18:51:32.682000 astro_deployment_utils-0.2.0/deployment_utils/models.py
+-rw-r--r--   0        0        0      479 2023-04-10 15:41:44.219084 astro_deployment_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 astro_deployment_utils-0.2.0/PKG-INFO
```

### Comparing `astro_deployment_utils-0.1.0/deployment_utils/api_handler.py` & `astro_deployment_utils-0.2.0/deployment_utils/api_handler.py`

 * *Files identical despite different names*

### Comparing `astro_deployment_utils-0.1.0/deployment_utils/cloud_config.py` & `astro_deployment_utils-0.2.0/deployment_utils/cloud_config.py`

 * *Files identical despite different names*

### Comparing `astro_deployment_utils-0.1.0/deployment_utils/cloud_constants.py` & `astro_deployment_utils-0.2.0/deployment_utils/cloud_constants.py`

 * *Files identical despite different names*

### Comparing `astro_deployment_utils-0.1.0/deployment_utils/cloud_utils.py` & `astro_deployment_utils-0.2.0/deployment_utils/cloud_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ImageDeploy,
     DeleteDeployment,
     WorkerQueues,
     EnvVar,
 )
 from . import cloud_constants
 from .log import get_logger
-
+from .astro_cli_utils import  astro_setup , astro_deploy
 logger = get_logger()
 
 """
 Generate bearer token for cloud deployment which will be used for all graphql calls as auth
 """
 
 
@@ -36,15 +36,15 @@
     auth_request_dict = BearerToken(
         env_config[cloud_env]["CLIENT_ID"],
         env_config[cloud_env]["PLATFORM_USER_EMAIL"],
         env_config[cloud_env]["PLATFORM_USER_PASSWORD"],
     )
 
     api_test = RequestAPI(
-        cloud_constants.token_base_uri + os.environ[cloud_constants.cloud_env],
+        cloud_constants.token_base_uri + cloud_env,
         cloud_constants.token_endpoint,
         post_data=asdict(auth_request_dict),
     )
     status_code, response_body = api_test.post_call()
     bearer_token = response_body["access_token"]
     os.environ['AUTH_BEARER_TOKEN'] = bearer_token
     return bearer_token
@@ -192,17 +192,17 @@
 
 
 """
 deletes provided deployment_id and return the same id from response 
 """
 
 
-def delete_deployment(deployment_id) -> str:
-    cloud_env = os.environ[cloud_constants.cloud_env]
+def delete_deployment(deployment_id,cloud_env='dev') -> str:
     delete_deployment = DeleteDeployment(deployment_id)
+    generate_bearer_token()
     data = {"input": asdict(delete_deployment)}
     variables_json = json.dumps(data, indent=2)
     logger.info(variables_json)
     headers = {"Authorization": f"Bearer {os.environ['AUTH_BEARER_TOKEN']}"}
     api_test = RequestAPI(
         cloud_constants.astrohub_base_uri + cloud_env,
         cloud_constants.astrohub_endpoint,
@@ -447,8 +447,22 @@
     )
     os.environ['DEPLOYMENT_ID'] = deployment_id
     os.environ['DEPLOYMENT_NAMESPACE'] = namespace
 
 
     time.sleep(300)
 
+
     return deployment_id,namespace
+
+
+
+def create_deployment_with_basic_dags(cloud_env='dev', cluster_id='cldog74ht02b30tx3bn955ddv',
+                            runtime_version_tag='7.5.0-alpha2', executor='CeleryExecutor',quay_repo_name='astro-runtime-dev',dags_repo='qa-scenario-dags'):
+    deployment_id,namespace = create_empty_deployment(cloud_env,cluster_id,runtime_version_tag,executor)
+   # astro_setup()
+    astro_deploy(deployment_id,cloud_env,quay_repo_name,runtime_version_tag,dags_repo)
+
+def astro_deployment(deployment_id,cloud_env='dev',
+                            runtime_version_tag='7.5.0-alpha2',quay_repo_name='astro-runtime-dev',dags_repo='qa-scenario-dags'):
+    generate_bearer_token()
+    astro_deploy(deployment_id,cloud_env, quay_repo_name, runtime_version_tag, dags_repo)
```

### Comparing `astro_deployment_utils-0.1.0/deployment_utils/log.py` & `astro_deployment_utils-0.2.0/deployment_utils/log.py`

 * *Files identical despite different names*

### Comparing `astro_deployment_utils-0.1.0/deployment_utils/logs/execution_logfile.log` & `astro_deployment_utils-0.2.0/deployment_utils/logs/execution_logfile.log`

 * *Files identical despite different names*

### Comparing `astro_deployment_utils-0.1.0/deployment_utils/models.py` & `astro_deployment_utils-0.2.0/deployment_utils/models.py`

 * *Files identical despite different names*

