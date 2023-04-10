# Comparing `tmp/sos_ansible-1.0.2.tar.gz` & `tmp/sos_ansible-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sos_ansible-1.0.2.tar", last modified: Mon Apr  3 16:10:59 2023, max compression
+gzip compressed data, was "sos_ansible-1.0.3.tar", last modified: Mon Apr 10 07:59:41 2023, max compression
```

## Comparing `sos_ansible-1.0.2.tar` & `sos_ansible-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:59.970218 sos_ansible-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:59.962218 sos_ansible-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:59.966218 sos_ansible-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/DockerfileDebug
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-03 16:10:59.970218 sos_ansible-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:59.966218 sos_ansible-1.0.2/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/rules/rules.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 16:10:59.970218 sos_ansible-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:59.970218 sos_ansible-1.0.2/sos_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:59.970218 sos_ansible-1.0.2/sos_ansible/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/modules/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/modules/file_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:59.970218 sos_ansible-1.0.2/sos_ansible/modules/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/modules/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/modules/helpers/rule_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/modules/helpers/rule_writer_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/modules/helpers/write_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/modules/locating_sos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-03 16:10:49.000000 sos_ansible-1.0.2/sos_ansible/modules/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:10:59.970218 sos_ansible-1.0.2/sos_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-03 16:10:59.000000 sos_ansible-1.0.2/sos_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-03 16:10:59.000000 sos_ansible-1.0.2/sos_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:10:59.000000 sos_ansible-1.0.2/sos_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-03 16:10:59.000000 sos_ansible-1.0.2/sos_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-03 16:10:59.000000 sos_ansible-1.0.2/sos_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 16:10:59.000000 sos_ansible-1.0.2/sos_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.428466 sos_ansible-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.432466 sos_ansible-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/DockerfileDebug
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.432466 sos_ansible-1.0.3/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/rules/controller.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/rules/hub-rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/rules/rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/rules/tower.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.432466 sos_ansible-1.0.3/sos_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/sos_ansible/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/file_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/sos_ansible/modules/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/helpers/rule_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/helpers/rule_writer_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/helpers/write_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/locating_sos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.432466 sos_ansible-1.0.3/sos_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/top_level.txt
```

### Comparing `sos_ansible-1.0.2/.github/workflows/pylint.yml` & `sos_ansible-1.0.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/.github/workflows/python-publish.yml` & `sos_ansible-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/.gitignore` & `sos_ansible-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/.pylintrc` & `sos_ansible-1.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/LICENSE` & `sos_ansible-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/PKG-INFO` & `sos_ansible-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sos_ansible
-Version: 1.0.2
+Version: 1.0.3
 Summary: A sosreport parser for ansible
 Author-email: Lucas Benedito <lbenedit@redhat.com>
 License: GPL-3.0 license
 Project-URL: Homepage, https://github.com/lucas-benedito/sos-ansible
 Project-URL: Bug Tracker, https://github.com/lucas-benedito/sos-ansible/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -22,26 +22,31 @@
 * [Installation](#installation)
 * [Sosreport location and rules files](#sosreport-location-and-rules-files)
 * [Running the tool and checking the logs [WIP]](#running-the-tool-and-checking-the-logs-[wip])
 * [Running tool via container](#running-tool-via-container)
 * [Additional notes for troubleshooting containerized tool](#additional-notes-for-troubleshooting-containerized-tool)
 * [Setup Development Environment](#setup-development-environment)
 ---
-## Installation
+## Installation and Upgrade
 This tool can be installed from pip
 ```
-$ pip install sos_ansible
+$ pip install -U sos_ansible
 ```
 
 ---
 ## Sosreport location and rules files
 Extract all the sosreport files for evaluation on the same directory as per the example:
 ```
 $ tar xf sosreport-lbenedit-test-node-xxxx-xxx-xxx.tar.xz -C /tmp/test_sosreport/9999999
 ```
+### As an alternative to using the tar command
+
+`sos_ansible -c 999999 -t sosreport-lbenedit-test-node-xxxx-xxx-xxx.tar.xz, sosreport-lbenedit-test-node2-xxxx-xxx-xxx.tar.xz`
+
+*Note* -t or --tarball takes a comma separated list of sosreports and untars them in the /tmp/sosreport by default. Case number is mandatory for untar feature
 
 Use the rules file located in this project or create your own. Sharing your rules with your peers is the key for this tools success.
 ```
 $ head rules/rules.json                                                                       
 {
     "Filesystem": {
         "files": ["df"],
```

### Comparing `sos_ansible-1.0.2/README.md` & `sos_ansible-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,31 @@
 * [Installation](#installation)
 * [Sosreport location and rules files](#sosreport-location-and-rules-files)
 * [Running the tool and checking the logs [WIP]](#running-the-tool-and-checking-the-logs-[wip])
 * [Running tool via container](#running-tool-via-container)
 * [Additional notes for troubleshooting containerized tool](#additional-notes-for-troubleshooting-containerized-tool)
 * [Setup Development Environment](#setup-development-environment)
 ---
-## Installation
+## Installation and Upgrade
 This tool can be installed from pip
 ```
-$ pip install sos_ansible
+$ pip install -U sos_ansible
 ```
 
 ---
 ## Sosreport location and rules files
 Extract all the sosreport files for evaluation on the same directory as per the example:
 ```
 $ tar xf sosreport-lbenedit-test-node-xxxx-xxx-xxx.tar.xz -C /tmp/test_sosreport/9999999
 ```
+### As an alternative to using the tar command
+
+`sos_ansible -c 999999 -t sosreport-lbenedit-test-node-xxxx-xxx-xxx.tar.xz, sosreport-lbenedit-test-node2-xxxx-xxx-xxx.tar.xz`
+
+*Note* -t or --tarball takes a comma separated list of sosreports and untars them in the /tmp/sosreport by default. Case number is mandatory for untar feature
 
 Use the rules file located in this project or create your own. Sharing your rules with your peers is the key for this tools success.
 ```
 $ head rules/rules.json                                                                       
 {
     "Filesystem": {
         "files": ["df"],
@@ -155,8 +160,8 @@
 ---
 ## Setup Development Environment
 Create virtual environment and use `make init`.
 ```
 $ python -m venv venv
 $ source venv/bin/activate
 $ make init
-```
+```
```

### Comparing `sos_ansible-1.0.2/pyproject.toml` & `sos_ansible-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sos_ansible"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     {name = "Lucas Benedito", email = "lbenedit@redhat.com"},
 ]
 description = "A sosreport parser for ansible"
 requires-python = ">=3.9"
 license = {text = "GPL-3.0 license"}
 dependencies = [
```

### Comparing `sos_ansible-1.0.2/rules/rules.json` & `sos_ansible-1.0.3/rules/controller.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6323529411764706%*

 * *Differences: {"'Controller Info'": "OrderedDict([('files', ['awx-manage_--version', "*

 * *                      "'awx-manage_check_license_--data', 'awx-manage_run_wsbroadcast_--status', "*

 * *                      "'supervisorctl_status']), ('path', 'sos_commands/controller'), ('query', "*

 * *                      "'')])",*

 * * "'Installed Packages'": "{'query': 'ansible, automation, receptor, postgres'}",*

 * * "'Instances Capacity'": "{'path': 'sos_commands/controller', 'query': 'capacity=0, , \\\\['}",*

 * * "'PIP Conflict'": "OrderedDict([( […]*

```diff
@@ -2,34 +2,44 @@
     "Antivirus": {
         "files": [
             "installed-rpms"
         ],
         "path": "",
         "query": "falcon, crowd"
     },
+    "Controller Info": {
+        "files": [
+            "awx-manage_--version",
+            "awx-manage_check_license_--data",
+            "awx-manage_run_wsbroadcast_--status",
+            "supervisorctl_status"
+        ],
+        "path": "sos_commands/controller",
+        "query": ""
+    },
     "Filesystem": {
         "files": [
             "df"
         ],
         "path": "",
         "query": "100%"
     },
     "Installed Packages": {
         "files": [
             "installed-rpms"
         ],
         "path": "",
-        "query": "ansible, automation, receptor, hub, keycloak"
+        "query": "ansible, automation, receptor, postgres"
     },
     "Instances Capacity": {
         "files": [
             "awx-manage_list_instances"
         ],
-        "path": "sos_commands/tower",
-        "query": "capacity=0, controller="
+        "path": "sos_commands/controller",
+        "query": "capacity=0, , \\["
     },
     "LDAP": {
         "files": [
             "tower.log"
         ],
         "path": "var/log/tower",
         "query": "django_auth_ldap"
@@ -47,14 +57,21 @@
     "OOM": {
         "files": [
             "dmesg"
         ],
         "path": "sos_commands/kernel/",
         "query": "OOM"
     },
+    "PIP Conflict": {
+        "files": [
+            "pip_list"
+        ],
+        "path": "sos_commands/python",
+        "query": "ansible"
+    },
     "Receptor": {
         "files": [
             "receptor.log"
         ],
         "path": "var/log/receptor",
         "query": "error"
     },
@@ -75,55 +92,30 @@
             "supervisord.log",
             "awx-daphne.log",
             "awx-uwsgi.log"
         ],
         "path": "var/log/supervisor",
         "query": "error"
     },
-    "Tower Errors": {
-        "files": [
-            "callback_receiver.log",
-            "dispatcher.log",
-            "job_lifecycle.log",
-            "management_playbooks.log",
-            "task_system.log",
-            "tower.log",
-            "tower_rbac_migrations.log",
-            "tower_system_tracking_migrations.log",
-            "wsbroadcast.log"
-        ],
-        "path": "var/log/tower",
-        "query": "error"
-    },
-    "Tower Info": {
+    "noexec": {
         "files": [
-            "awx-manage_--version",
-            "awx-manage_check_license_--data",
-            "awx-manage_run_wsbroadcast_--status",
-            "supervisorctl_status"
+            "mount"
         ],
-        "path": "sos_commands/tower",
-        "query": ""
+        "path": "",
+        "query": "noexec"
     },
-    "Tower Traceback": {
+    "tower errors": {
         "files": [
             "callback_receiver.log",
             "dispatcher.log",
             "job_lifecycle.log",
             "management_playbooks.log",
             "task_system.log",
             "tower.log",
             "tower_rbac_migrations.log",
             "tower_system_tracking_migrations.log",
             "wsbroadcast.log"
         ],
         "path": "var/log/tower",
-        "query": "Traceback"
-    },
-    "noexec": {
-        "files": [
-            "mount"
-        ],
-        "path": "",
-        "query": "noexec"
+        "query": "error"
     }
 }
```

### Comparing `sos_ansible-1.0.2/sos_ansible/__main__.py` & `sos_ansible-1.0.3/sos_ansible/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 #!/usr/bin/env python
 """
 sos_ansible, main program
 """
 import os
 import sys
-import logging.config as loggerconf
 from logging import getLogger
 import inquirer
 from sos_ansible.modules.file_handling import (
     validate_out_dir,
     data_input,
     rules_processing,
     expand_sosreport,
 )
 from sos_ansible.modules.parsing import Parser
-from sos_ansible.modules.config_manager import ConfigParser, validator
+from sos_ansible.modules.config_manager import ConfigParser
 
 # Setting up local settings
 config = ConfigParser()
 config.setup()
-validator(config.config_handler)
 
 # Setting up Logger
-loggerconf.fileConfig(config.config_file)
 logger = getLogger("root")
 
 
 # Processing user input for directory choice
 def get_user_input(sos_directory):
     """Select work directory"""
     choice = os.listdir(sos_directory)
@@ -69,17 +66,17 @@
 
     # if case number is not provided prompt if provided just use it
     if os.path.isdir(sos_directory) and not params.case:
         user_choice = get_user_input(sos_directory)
     elif os.path.isdir(sos_directory) and params.case:
         user_choice = params.case
     else:
-        logger.error(
+        logger.critical(
             "The selected directory %s doesn't exist."
-            "Select a new directory and try again.",
+            " Select a new directory and try again.",
             sos_directory,
         )
         sys.exit(1)
 
     node_data, curr_policy = data_input(sos_directory, rules_file, user_choice)
     if not node_data:
         logger.critical(
```

### Comparing `sos_ansible-1.0.2/sos_ansible/modules/file_handling.py` & `sos_ansible-1.0.3/sos_ansible/modules/file_handling.py`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/sos_ansible/modules/helpers/rule_writer.py` & `sos_ansible-1.0.3/sos_ansible/modules/helpers/rule_writer.py`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/sos_ansible/modules/helpers/rule_writer_input.py` & `sos_ansible-1.0.3/sos_ansible/modules/helpers/rule_writer_input.py`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/sos_ansible/modules/helpers/write_json.py` & `sos_ansible-1.0.3/sos_ansible/modules/helpers/write_json.py`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/sos_ansible/modules/locating_sos.py` & `sos_ansible-1.0.3/sos_ansible/modules/locating_sos.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 Class based on the lookup plugin created by Chris Meyers.
 https://github.com/chrismeyersfsu/sosreport-elk
 """
 
 import glob
 import os
 import re
-import logging.config as loggerconf
 from logging import getLogger
 
 from sos_ansible.modules.config_manager import ConfigParser
 
 config = ConfigParser()
 config.setup()
 
-loggerconf.fileConfig(config.config_file)
 logger = getLogger("root")
 
 
 class LocateReports:
     """
     Validate the sosreport directory existance and provide the hostname and path for reference
     """
```

### Comparing `sos_ansible-1.0.2/sos_ansible/modules/parsing.py` & `sos_ansible-1.0.3/sos_ansible/modules/parsing.py`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.2/sos_ansible.egg-info/PKG-INFO` & `sos_ansible-1.0.3/sos_ansible.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sos-ansible
-Version: 1.0.2
+Version: 1.0.3
 Summary: A sosreport parser for ansible
 Author-email: Lucas Benedito <lbenedit@redhat.com>
 License: GPL-3.0 license
 Project-URL: Homepage, https://github.com/lucas-benedito/sos-ansible
 Project-URL: Bug Tracker, https://github.com/lucas-benedito/sos-ansible/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -22,26 +22,31 @@
 * [Installation](#installation)
 * [Sosreport location and rules files](#sosreport-location-and-rules-files)
 * [Running the tool and checking the logs [WIP]](#running-the-tool-and-checking-the-logs-[wip])
 * [Running tool via container](#running-tool-via-container)
 * [Additional notes for troubleshooting containerized tool](#additional-notes-for-troubleshooting-containerized-tool)
 * [Setup Development Environment](#setup-development-environment)
 ---
-## Installation
+## Installation and Upgrade
 This tool can be installed from pip
 ```
-$ pip install sos_ansible
+$ pip install -U sos_ansible
 ```
 
 ---
 ## Sosreport location and rules files
 Extract all the sosreport files for evaluation on the same directory as per the example:
 ```
 $ tar xf sosreport-lbenedit-test-node-xxxx-xxx-xxx.tar.xz -C /tmp/test_sosreport/9999999
 ```
+### As an alternative to using the tar command
+
+`sos_ansible -c 999999 -t sosreport-lbenedit-test-node-xxxx-xxx-xxx.tar.xz, sosreport-lbenedit-test-node2-xxxx-xxx-xxx.tar.xz`
+
+*Note* -t or --tarball takes a comma separated list of sosreports and untars them in the /tmp/sosreport by default. Case number is mandatory for untar feature
 
 Use the rules file located in this project or create your own. Sharing your rules with your peers is the key for this tools success.
 ```
 $ head rules/rules.json                                                                       
 {
     "Filesystem": {
         "files": ["df"],
```

