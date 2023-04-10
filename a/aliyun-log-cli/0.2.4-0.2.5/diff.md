# Comparing `tmp/aliyun-log-cli-0.2.4.tar.gz` & `tmp/aliyun-log-cli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-log-cli-0.2.4.tar", last modified: Mon Jan 10 11:41:11 2022, max compression
+gzip compressed data, was "aliyun-log-cli-0.2.5.tar", last modified: Mon Apr 10 03:14:56 2023, max compression
```

## Comparing `aliyun-log-cli-0.2.4.tar` & `aliyun-log-cli-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 licheng    (502) staff       (20)        0 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/
--rw-r--r--   0 licheng    (502) staff       (20)      897 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/PKG-INFO
--rw-r--r--   0 licheng    (502) staff       (20)    19859 2022-01-10 11:40:25.000000 aliyun-log-cli-0.2.4/README.md
-drwxr-xr-x   0 licheng    (502) staff       (20)        0 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/aliyun_log_cli.egg-info/
--rw-r--r--   0 licheng    (502) staff       (20)      897 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/aliyun_log_cli.egg-info/PKG-INFO
--rw-r--r--   0 licheng    (502) staff       (20)      415 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/aliyun_log_cli.egg-info/SOURCES.txt
--rw-r--r--   0 licheng    (502) staff       (20)        1 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/aliyun_log_cli.egg-info/dependency_links.txt
--rw-r--r--   0 licheng    (502) staff       (20)       53 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/aliyun_log_cli.egg-info/entry_points.txt
--rw-r--r--   0 licheng    (502) staff       (20)      100 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/aliyun_log_cli.egg-info/requires.txt
--rw-r--r--   0 licheng    (502) staff       (20)       13 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/aliyun_log_cli.egg-info/top_level.txt
-drwxr-xr-x   0 licheng    (502) staff       (20)        0 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/aliyunlogcli/
--rw-r--r--   0 licheng    (502) staff       (20)       33 2022-01-10 11:40:25.000000 aliyun-log-cli-0.2.4/aliyunlogcli/__init__.py
--rwxr-xr-x   0 licheng    (502) staff       (20)      266 2022-01-10 11:40:25.000000 aliyun-log-cli-0.2.4/aliyunlogcli/cli.py
--rw-r--r--   0 licheng    (502) staff       (20)    11639 2022-01-10 11:40:25.000000 aliyun-log-cli-0.2.4/aliyunlogcli/cli_core.py
--rw-r--r--   0 licheng    (502) staff       (20)    17897 2022-01-10 11:40:25.000000 aliyun-log-cli-0.2.4/aliyunlogcli/config.py
--rw-r--r--   0 licheng    (502) staff       (20)      152 2022-01-10 11:40:25.000000 aliyun-log-cli-0.2.4/aliyunlogcli/exceptions.py
--rw-r--r--   0 licheng    (502) staff       (20)    14194 2022-01-10 11:40:25.000000 aliyun-log-cli-0.2.4/aliyunlogcli/parser.py
--rw-r--r--   0 licheng    (502) staff       (20)      147 2022-01-10 11:40:25.000000 aliyun-log-cli-0.2.4/aliyunlogcli/version.py
--rw-r--r--   0 licheng    (502) staff       (20)       38 2022-01-10 11:41:11.000000 aliyun-log-cli-0.2.4/setup.cfg
--rwxr-xr-x   0 licheng    (502) staff       (20)     1719 2022-01-10 11:40:25.000000 aliyun-log-cli-0.2.4/setup.py
+drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:14:56.593860 aliyun-log-cli-0.2.5/
+-rw-r--r--   0 zhhfan     (502) staff       (20)     1070 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/LICENSE
+-rw-r--r--   0 zhhfan     (502) staff       (20)      825 2023-04-10 03:14:56.593428 aliyun-log-cli-0.2.5/PKG-INFO
+-rw-r--r--   0 zhhfan     (502) staff       (20)    19823 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/README.md
+drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:14:56.587760 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/
+-rw-r--r--   0 zhhfan     (502) staff       (20)      825 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/PKG-INFO
+-rw-r--r--   0 zhhfan     (502) staff       (20)      423 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 zhhfan     (502) staff       (20)        1 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 zhhfan     (502) staff       (20)       52 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/entry_points.txt
+-rw-r--r--   0 zhhfan     (502) staff       (20)      100 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/requires.txt
+-rw-r--r--   0 zhhfan     (502) staff       (20)       13 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/top_level.txt
+drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:14:56.592880 aliyun-log-cli-0.2.5/aliyunlogcli/
+-rw-r--r--   0 zhhfan     (502) staff       (20)       33 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/aliyunlogcli/__init__.py
+-rwxr-xr-x   0 zhhfan     (502) staff       (20)      266 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/aliyunlogcli/cli.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)    11518 2023-04-10 03:12:40.000000 aliyun-log-cli-0.2.5/aliyunlogcli/cli_core.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)    20923 2023-04-10 03:12:40.000000 aliyun-log-cli-0.2.5/aliyunlogcli/config.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)      152 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/aliyunlogcli/exceptions.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)    13462 2023-04-10 03:12:40.000000 aliyun-log-cli-0.2.5/aliyunlogcli/parser.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)      147 2023-04-10 03:14:34.000000 aliyun-log-cli-0.2.5/aliyunlogcli/version.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)       38 2023-04-10 03:14:56.593966 aliyun-log-cli-0.2.5/setup.cfg
+-rwxr-xr-x   0 zhhfan     (502) staff       (20)     1719 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aliyun-log-cli-0.2.4/PKG-INFO` & `aliyun-log-cli-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: aliyun-log-cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: Aliyun log service CLI
 Home-page: https://github.com/aliyun/aliyun-log-cli
 Author: Aliyun
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: 
-        Command Line Interface for Aliyun Log Service 
-        http://aliyun-log-cli.readthedocs.io
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
+
+
+Command Line Interface for Aliyun Log Service 
+http://aliyun-log-cli.readthedocs.io
```

### Comparing `aliyun-log-cli-0.2.4/README.md` & `aliyun-log-cli-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -445,17 +445,16 @@
 {
  "machine_list": [
    "machine1",
    "machine2"
  ],
  "machine_type": "userdefined",
  "group_name": "group_name2",
- "group_type": "Armory",
+ "group_type": "",
  "group_attribute": {
-   "externalName": "ex name",
    "groupTopic": "topic x"
  }
 }
 ```
 
 - delete_machine_group
 - update_machine_group
```

### Comparing `aliyun-log-cli-0.2.4/aliyun_log_cli.egg-info/PKG-INFO` & `aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: aliyun-log-cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: Aliyun log service CLI
 Home-page: https://github.com/aliyun/aliyun-log-cli
 Author: Aliyun
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: 
-        Command Line Interface for Aliyun Log Service 
-        http://aliyun-log-cli.readthedocs.io
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
+
+
+Command Line Interface for Aliyun Log Service 
+http://aliyun-log-cli.readthedocs.io
```

### Comparing `aliyun-log-cli-0.2.4/aliyunlogcli/cli_core.py` & `aliyun-log-cli-0.2.5/aliyunlogcli/cli_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,16 +211,15 @@
         for x in ret:
             _process_response(x, jmes_filter, format_output, decode_output)
     else:
         logger.warning("unknown response data: %s", ret)
 
 
 def main():
-    method_types, method_param_usage, optdoc, usage = parse_method_types_optdoc_from_class(LogClient,
-                                                                                           LOG_CLIENT_METHOD_BLACK_LIST)
+    method_types, method_param_usage, optdoc, usage = parse_method_types_optdoc_from_class(LogClient)
 
     arguments = docopt_ex(optdoc, usage, method_param_usage, hlp=False, ver=USER_AGENT)
     if arguments is None:
         exit(1)
 
     system_options = normalize_system_options(arguments)
```

### Comparing `aliyun-log-cli-0.2.4/aliyunlogcli/config.py` & `aliyun-log-cli-0.2.5/aliyunlogcli/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,43 +8,35 @@
 import logging
 from logging.handlers import RotatingFileHandler
 from .exceptions import IncompleteAccountInfoError
 import requests
 from aliyunsdkcore import client
 from aliyunsdksts.request.v20150401 import AssumeRoleRequest
 
-LOG_CLIENT_METHOD_BLACK_LIST = (r'_.+', r'\w+acl', 'set_source', 'delete_shard', 'heart_beat',
-                                'set_user_agent', 'get_unicode', 'list_logstores', 'put_log_raw'
-                                )
-
-LOG_CREDS_FILENAME = "%s/.aliyunlogcli" % os.path.expanduser('~')
-ALIYUN_CLI_CONF_FILENAME = "%s/.aliyun/config.json" % os.path.expanduser('~')
-DEFAULT_DEBUG_LOG_FILE_PATH = "%s/aliyunlogcli.log" % os.path.expanduser('~')
+
+LOG_CREDS_FILENAME = "%s/.aliyunlogcli" % os.path.expanduser("~")
+ALIYUN_CLI_CONF_FILENAME = "%s/.aliyun/config.json" % os.path.expanduser("~")
+DEFAULT_DEBUG_LOG_FILE_PATH = "%s/aliyunlogcli.log" % os.path.expanduser("~")
 DEFAULT_DEBUG_LOG_FORMAT = "%(asctime)s %(levelname)s %(process)s:%(threadName)s:%(filename)s:%(lineno)d %(funcName)s %(message)s"
 ECS_RAM_ROLE_URL = "http://100.100.100.200/latest/meta-data/Ram/security-credentials/"
 
 LOG_CONFIG_SECTION = "main"
 GLOBAL_OPTION_SECTION = "__option__"
 GLOBAL_OPTION_KEY_FORMAT_OUTPUT = "format-output"
 GLOBAL_OPTION_KEY_DEFAULT_CLIENT = "default-client"
 GLOBAL_OPTION_KEY_DECODE_OUTPUT = "decode-output"
 
 STS_TOKEN_SEP = "::"
 
 SYSTEM_OPTIONS = ['access-id', 'access-key', 'sts-token', 'region-endpoint', 'client-name', 'jmes-filter', 'format-output',
                   'decode-output', 'profile']
-SYSTEM_OPTIONS_STR = ' '.join('[--' + x + '=<value>]' for x in SYSTEM_OPTIONS)
+SYSTEM_OPTIONS_STR = " ".join("[--" + x + "=<value>]" for x in SYSTEM_OPTIONS)
 
 SystemConfig = namedtuple('SystemConfig', "access_id access_key endpoint sts_token, jmes_filter format_output decode_output")
 
-API_GROUP = [('project$', 'Project'), 'logstore', ('index|topics', "Index"),
-             ('logtail_config', "Logtail Config"), ('machine', "Machine Group"), 'shard',
-             'cursor', ('log|histogram', "Logs"), ('consumer|check_point', "Consumer Group"), 'shipper',
-             'dashboard', 'savedsearch', 'alert', ('external_store', "External Store")]
-
 GLOBAL_OPTIONS_STR = """
 Global Options:
 [--access-id=<value>]		        : use this access id in this command
 [--access-key=<value>]		        : use this access key in this command
 [--sts-token=<value>]		        : use this sts token in this command
 [--region-endpoint=<value>]	        : use this endpoint in this command
 [--client-name=<value>]		        : use this client name in configured accounts
@@ -72,20 +64,141 @@
 3. aliyunlog log create_project --project_name="test"
 4. aliyunlog configure AKID124 AKKey123 cn-hangzhou.log.aliyuncs.com main StsTokenValue1234
 
 Subcommand:
 {grouped_api}
 """ + GLOBAL_OPTIONS_STR
 
+
 MORE_DOCOPT_CMD = """aliyunlog configure <secure_id> <secure_key> <endpoint> [<client_name>] [<sts_token>]
 aliyunlog configure [--format-output=json,no_escape] [--default-client=<client_name>] [--decode-output=utf8,latin1]
 """
 
 DEBUG_SECTION_NAME = "__logging__"
 
+SUPPORT_LIST = {
+    "Project": [
+        "copy_project",
+        "create_project",
+        "delete_project",
+        "get_project",
+        "list_project",
+        "tag_project",
+        "untag_project",
+    ],
+    "Logstore": [
+        "copy_logstore",
+        "create_logstore",
+        "delete_logstore",
+        "execute_logstore_sql",
+        "get_logstore",
+        "list_logstore",
+        "update_logstore",
+    ],
+    "Index": [
+        "create_index",
+        "delete_index",
+        "get_index_config",
+        "list_topics",
+        "update_index",
+    ],
+    "Logtail Config": [
+        "create_logtail_config",
+        "delete_logtail_config",
+        "get_logtail_config",
+        "list_logtail_config",
+        "update_logtail_config",
+    ],
+    "Machine Group": [
+        "apply_config_to_machine_group",
+        "create_machine_group",
+        "delete_machine_group",
+        "get_config_applied_machine_groups",
+        "get_machine_group",
+        "get_machine_group_applied_configs",
+        "list_machine_group",
+        "list_machines",
+        "remove_config_to_machine_group",
+        "update_machine_group",
+    ],
+    "Shard": ["arrange_shard", "list_shards", "merge_shard", "split_shard"],
+    "Cursor": [
+        "get_begin_cursor",
+        "get_cursor",
+        "get_cursor_time",
+        "get_end_cursor",
+        "get_previous_cursor_time",
+    ],
+    "Logs": [
+        "get_context_logs",
+        "get_histograms",
+        "get_log",
+        "get_log_all",
+        "get_logs",
+        "get_project_logs",
+        "pull_log",
+        "pull_log_dump",
+        "pull_logs",
+    ],
+    "Consumer Group": [
+        "create_consumer_group",
+        "delete_consumer_group",
+        "get_check_point",
+        "get_check_point_fixed",
+        "list_consumer_group",
+        "update_check_point",
+        "update_consumer_group",
+    ],
+    "Dashboard": [
+        "create_dashboard",
+        "delete_dashboard",
+        "get_dashboard",
+        "list_dashboard",
+        "update_dashboard",
+    ],
+    "Savedsearch": [
+        "create_savedsearch",
+        "delete_savedsearch",
+        "get_savedsearch",
+        "list_savedsearch",
+        "update_savedsearch",
+    ],
+    "Alert": [
+        "create_alert",
+        "delete_alert",
+        "disable_alert",
+        "enable_alert",
+        "get_alert",
+        "list_alert",
+        "update_alert",
+    ],
+    "External Store": [
+        "create_external_store",
+        "delete_external_store",
+        "get_external_store",
+        "list_external_store",
+        "update_external_store",
+    ],
+    "Others": [
+        "create_metric_store",
+        "create_substore",
+        "delete_metric_store",
+        "delete_substore",
+        "es_migration",
+        "execute_project_sql",
+        "get_metric_store",
+        "get_project_tags",
+        "get_substore",
+        "get_substore_ttl",
+        "list_substore",
+        "update_substore",
+        "update_substore_ttl",
+    ]
+}
+
 
 def _get_section_option(config, section_name, option_name, default=None):
     if six.PY3:
         return config.get(section_name, option_name, fallback=default)
     else:
         return config.get(section_name, option_name) if config.has_option(section_name, option_name) else default
 
@@ -94,21 +207,21 @@
     # load key value from file
     config = configparser.SafeConfigParser()
     config.read(LOG_CREDS_FILENAME)
 
     return _get_section_option(config, section, key, default)
 
 
-def load_config_from_cloudshell(default_ak_id='', default_ak_key='', default_endpoint=''):
+def load_config_from_cloudshell(default_ak_id="", default_ak_key="", default_endpoint=""):
     # Cloudshell envs
-    access_id = os.environ.get('ALIBABA_CLOUD_ACCESS_KEY_ID', default_ak_id)
-    access_key = os.environ.get('ALIBABA_CLOUD_ACCESS_KEY_SECRET', default_ak_key)
-    endpoint = os.environ.get('ALIBABA_CLOUD_DEFAULT_REGION', default_endpoint)
-    if endpoint and not endpoint.endswith('.com'):
-        endpoint = endpoint + '.log.aliyuncs.com'
+    access_id = os.environ.get("ALIBABA_CLOUD_ACCESS_KEY_ID", default_ak_id)
+    access_key = os.environ.get("ALIBABA_CLOUD_ACCESS_KEY_SECRET", default_ak_key)
+    endpoint = os.environ.get("ALIBABA_CLOUD_DEFAULT_REGION", default_endpoint)
+    if endpoint and not endpoint.endswith(".com"):
+        endpoint = endpoint + ".log.aliyuncs.com"
 
     return access_id, access_key, endpoint
 
 
 def verify_sts_token(ac_id, sts_token, use=False):
     sts_token = sts_token or ""
 
@@ -138,189 +251,264 @@
     # load config from file
     config = configparser.ConfigParser()
     config.read(LOG_CREDS_FILENAME)
 
     # access_id, access_key, endpoint = load_config_from_cloudshell()
     # sts_token = ""
 
-    access_id = _get_section_option(config, client_name, 'access-id', "")
-    access_key = _get_section_option(config, client_name, 'access-key', "")
-    endpoint = _get_section_option(config, client_name, 'region-endpoint', "")
-    sts_token = _get_section_option(config, client_name, 'sts-token', "")
+    access_id = _get_section_option(config, client_name, "access-id", "")
+    access_key = _get_section_option(config, client_name, "access-key", "")
+    endpoint = _get_section_option(config, client_name, "region-endpoint", "")
+    sts_token = _get_section_option(config, client_name, "sts-token", "")
     sts_token = verify_sts_token(access_id, sts_token)
 
     return access_id, access_key, endpoint, sts_token
 
 
 def load_default_config_from_file_env():
     access_id, access_key, endpoint, sts_token = load_confidential_from_file(LOG_CONFIG_SECTION)
 
     # load config from envs
-    access_id = os.environ.get('ALIYUN_LOG_CLI_ACCESSID', access_id)
-    access_key = os.environ.get('ALIYUN_LOG_CLI_ACCESSKEY', access_key)
-    endpoint = os.environ.get('ALIYUN_LOG_CLI_ENDPOINT', endpoint)
-    sts_token = os.environ.get('ALIYUN_LOG_CLI_STS_TOKEN', sts_token)
+    access_id = os.environ.get("ALIYUN_LOG_CLI_ACCESSID", access_id)
+    access_key = os.environ.get("ALIYUN_LOG_CLI_ACCESSKEY", access_key)
+    endpoint = os.environ.get("ALIYUN_LOG_CLI_ENDPOINT", endpoint)
+    sts_token = os.environ.get("ALIYUN_LOG_CLI_STS_TOKEN", sts_token)
 
     return access_id, access_key, endpoint, sts_token
 
+
 def parse_authenticity_from_response(response):
     if isinstance(response, bytes):
         response = response.decode()
     response = json.loads(response)
     credentials = response.get("Credentials")
     sts_token = credentials.get("SecurityToken", "")
     ak_id = credentials.get("AccessKeyId", "")
     ak_key = credentials.get("AccessKeySecret", "")
     return ak_id, ak_key, sts_token
 
+
 def parse_xml_info_from_assumerole(access_id, access_key, endpoint, ram_role_arn):
-    endpoint = endpoint.replace(".log.aliyuncs.com", "") if endpoint.endswith(".log.aliyuncs.com") else endpoint
+    endpoint = (
+        endpoint.replace(".log.aliyuncs.com", "")
+        if endpoint.endswith(".log.aliyuncs.com")
+        else endpoint
+    )
     clt = client.AcsClient(access_id, access_key, endpoint)
     # 构造"AssumeRole"请求
     request = AssumeRoleRequest.AssumeRoleRequest()
     # 指定角色
     request.set_RoleArn(ram_role_arn)
     # 设置会话名称，审计服务使用此名称区分调用者
-    request.set_RoleSessionName('etl-test')
+    request.set_RoleSessionName("etl-test")
     # 发起请求，并得到response
     response = clt.do_action_with_exception(request)
     ak_id, ak_key, sts_token = parse_authenticity_from_response(response)
     return ak_id, ak_key, sts_token
 
+
 def parse_ecs_ram_role_authenticity_from_response(ram_role_name):
     url = ECS_RAM_ROLE_URL + ram_role_name
     response = requests.get(url)
     content = response.content
     if isinstance(content, bytes):
         content = content.decode()
     authenticity = json.loads(content)
     ak_id = authenticity.get("AccessKeyId", "")
     ak_key = authenticity.get("AccessKeySecret", "")
     sts_token = authenticity.get("SecurityToken", "")
     return ak_id, ak_key, sts_token
 
-def load_confidential_from_aliyun_client_file(config_file, profile_mode='', ak_id="", ak_key="", endpoint="", sts_token=""):
+
+def load_confidential_from_aliyun_client_file(config_file, profile_mode="", ak_id="", ak_key="", endpoint="", sts_token=""):
     user_define_profile = True if profile_mode else False
     try:
         with open(config_file) as cf:
             cf_content = json.load(cf)
         current_profile = cf_content.get("current")
         profiles = cf_content.get("profiles")
         profile = None
         for _profile in profiles:
             profile_name = _profile.get("name")
-            if (user_define_profile and profile_name == profile_mode) or (profile_name == current_profile and not user_define_profile):
+            if user_define_profile and profile_name == profile_mode or \
+                    (profile_name == current_profile and not user_define_profile):
                 profile = _profile
                 break
         current_mode = profile.get("mode")
         access_id = profile.get("access_key_id", ak_id)
         access_key = profile.get("access_key_secret", ak_key)
         endpoint = profile.get("region_id", endpoint)
         endpoint = endpoint + '.log.aliyuncs.com' if endpoint != "" else "cn-hangzhou.log.aliyuncs.com"
         sts_token = profile.get("sts_token", sts_token)
-        #RamRoleArn config
+        # RamRoleArn config
         if current_mode == "RamRoleArn":
             ram_role_arn = profile.get("ram_role_arn")
             ak_id, ak_secret, sts_token = parse_xml_info_from_assumerole(access_id, access_key, endpoint, ram_role_arn)
             return ak_id, ak_secret, endpoint, sts_token
-        #EcsRamRole config
+        # EcsRamRole config
         if current_mode == "EcsRamRole":
             ram_role_name = profile.get("ram_role_name")
             ak_id, ak_secret, sts_token = parse_ecs_ram_role_authenticity_from_response(ram_role_name)
             return ak_id, ak_secret, endpoint, sts_token
     except Exception as e:
         return "", "", "", ""
     return access_id, access_key, endpoint, sts_token
 
 
 def load_config(system_options):
-    access_id, access_key, endpoint, sts_token = '', '', '', ''
+    access_id, access_key, endpoint, sts_token = "", "", "", ""
     # load config from file
     config = configparser.ConfigParser()
     config.read(LOG_CREDS_FILENAME)
 
     # get section name
-    client_name = load_kv_from_file(GLOBAL_OPTION_SECTION, GLOBAL_OPTION_KEY_DEFAULT_CLIENT, LOG_CONFIG_SECTION) or LOG_CONFIG_SECTION
-    client_name = os.environ.get('ALIYUN_LOG_CLI_CLIENT_NAME', client_name)
-    client_name = system_options.get('client-name', client_name)
-    format_output = load_kv_from_file(GLOBAL_OPTION_SECTION, GLOBAL_OPTION_KEY_FORMAT_OUTPUT, '')
+    client_name = (
+        load_kv_from_file(
+            GLOBAL_OPTION_SECTION, GLOBAL_OPTION_KEY_DEFAULT_CLIENT, LOG_CONFIG_SECTION
+        )
+        or LOG_CONFIG_SECTION
+    )
+    client_name = os.environ.get("ALIYUN_LOG_CLI_CLIENT_NAME", client_name)
+    client_name = system_options.get("client-name", client_name)
+    format_output = load_kv_from_file(GLOBAL_OPTION_SECTION, GLOBAL_OPTION_KEY_FORMAT_OUTPUT, "")
     decode_output = load_kv_from_file(GLOBAL_OPTION_SECTION, GLOBAL_OPTION_KEY_DECODE_OUTPUT, ("utf8", "latin1"))
 
-    #load config from aliyun cfg file
+    # load config from aliyun cfg file
     _access_id, _access_key, _endpoint, _sts_token = load_confidential_from_aliyun_client_file(ALIYUN_CLI_CONF_FILENAME)
     endpoint = _endpoint or endpoint
     if all((_access_id, _access_key)):
         access_id, access_key, sts_token = _access_id, _access_key, _sts_token
 
-    #load config from aliyun-cli envs
-    alicloud_access_id, alicloud_access_key, alicloud_endpoint, alicloud_sts_token = os.environ.get('ALICLOUD_ACCESS_KEY_ID'), os.environ.get('ALICLOUD_ACCESS_KEY_SECRET'), \
-        os.environ.get('ALICLOUD_REGION_ID'), os.environ.get('SECURITY_TOKEN')
+    # load config from aliyun-cli envs
+    alicloud_access_id, alicloud_access_key, alicloud_endpoint, alicloud_sts_token = (
+        os.environ.get("ALICLOUD_ACCESS_KEY_ID"),
+        os.environ.get("ALICLOUD_ACCESS_KEY_SECRET"),
+        os.environ.get("ALICLOUD_REGION_ID"),
+        os.environ.get("SECURITY_TOKEN"),
+    )
     endpoint = alicloud_endpoint or endpoint
     if all((alicloud_access_id, alicloud_access_key)):
-        access_id, access_key, sts_token = alicloud_access_id, alicloud_access_key, alicloud_sts_token
-
-    alibabacloud_access_id, alibabacloud_access_key, alibabacloud_endpoint, alibabacloud_sts_token = os.environ.get('ALIBABACLOUD_ACCESS_KEY_ID'), os.environ.get('ALIBABACLOUD_ACCESS_KEY_SECRET'), \
-        os.environ.get('ALIBABACLOUD_REGION_ID'), os.environ.get('SECURITY_TOKEN')
+        access_id, access_key, sts_token = (
+            alicloud_access_id,
+            alicloud_access_key,
+            alicloud_sts_token,
+        )
+
+    (
+        alibabacloud_access_id,
+        alibabacloud_access_key,
+        alibabacloud_endpoint,
+        alibabacloud_sts_token,
+    ) = (
+        os.environ.get("ALIBABACLOUD_ACCESS_KEY_ID"),
+        os.environ.get("ALIBABACLOUD_ACCESS_KEY_SECRET"),
+        os.environ.get("ALIBABACLOUD_REGION_ID"),
+        os.environ.get("SECURITY_TOKEN"),
+    )
     endpoint = alibabacloud_endpoint or endpoint
     if all((alibabacloud_access_id, alibabacloud_access_key)):
-        access_id, access_key, sts_token = alibabacloud_access_id, alibabacloud_access_key, alibabacloud_sts_token
-
-    #load config from cloudshell envs
-    alicloud_access_id, alicloud_access_key, alicloud_endpoint, alicloud_sts_token = os.environ.get('ALICLOUD_ACCESS_KEY'), os.environ.get('ALICLOUD_SECRET_KEY'), \
-        os.environ.get('ALICLOUD_REGION'), os.environ.get('SECURITY_TOKEN')
+        access_id, access_key, sts_token = (
+            alibabacloud_access_id,
+            alibabacloud_access_key,
+            alibabacloud_sts_token,
+        )
+
+    # load config from cloudshell envs
+    alicloud_access_id, alicloud_access_key, alicloud_endpoint, alicloud_sts_token = (
+        os.environ.get("ALICLOUD_ACCESS_KEY"),
+        os.environ.get("ALICLOUD_SECRET_KEY"),
+        os.environ.get("ALICLOUD_REGION"),
+        os.environ.get("SECURITY_TOKEN"),
+    )
     endpoint = alicloud_endpoint or endpoint
     if all((alicloud_access_id, alicloud_access_key)):
-        access_id, access_key, sts_token = alicloud_access_id, alicloud_access_key, alicloud_sts_token
-
-    alibabacloud_access_id, alibabacloud_access_key, alibabacloud_endpoint, alibabacloud_sts_token = os.environ.get('ALIBABA_CLOUD_ACCESS_KEY_ID'), os.environ.get('ALIBABA_CLOUD_ACCESS_KEY_SECRET'), \
-        os.environ.get('ALIBABA_CLOUD_DEFAULT_REGION'), os.environ.get('ALIBABA_CLOUD_SECURITY_TOKEN')
+        access_id, access_key, sts_token = (
+            alicloud_access_id,
+            alicloud_access_key,
+            alicloud_sts_token,
+        )
+
+    (
+        alibabacloud_access_id,
+        alibabacloud_access_key,
+        alibabacloud_endpoint,
+        alibabacloud_sts_token,
+    ) = (
+        os.environ.get("ALIBABA_CLOUD_ACCESS_KEY_ID"),
+        os.environ.get("ALIBABA_CLOUD_ACCESS_KEY_SECRET"),
+        os.environ.get("ALIBABA_CLOUD_DEFAULT_REGION"),
+        os.environ.get("ALIBABA_CLOUD_SECURITY_TOKEN"),
+    )
     endpoint = alibabacloud_endpoint or endpoint
     if all((alibabacloud_access_id, alibabacloud_access_key)):
-        access_id, access_key, sts_token = alibabacloud_access_id, alibabacloud_access_key, alibabacloud_sts_token
+        access_id, access_key, sts_token = (
+            alibabacloud_access_id,
+            alibabacloud_access_key,
+            alibabacloud_sts_token,
+        )
 
-    if endpoint and not endpoint.endswith('.com'):
-        endpoint = endpoint + '.log.aliyuncs.com'
+    if endpoint and not endpoint.endswith(".com"):
+        endpoint = endpoint + ".log.aliyuncs.com"
 
-    #load config from sls cfg file
+    # load config from sls cfg file
     sls_access_id, sls_access_key, sls_endpoint, sls_sts_token = load_confidential_from_file(client_name)
     endpoint = sls_endpoint or endpoint
     if all((sls_access_id, sls_access_key)):
         access_id, access_key, sts_token = sls_access_id, sls_access_key, sls_sts_token
 
     # load config from sls envs
-    aliyun_access_id, aliyun_access_key, aliyun_endpoint, aliyun_sts_token = os.environ.get('ALIYUN_LOG_CLI_ACCESSID'), os.environ.get('ALIYUN_LOG_CLI_ACCESSKEY'), \
-        os.environ.get('ALIYUN_LOG_CLI_ENDPOINT'), os.environ.get('ALIYUN_LOG_CLI_STS_TOKEN')
+    aliyun_access_id, aliyun_access_key, aliyun_endpoint, aliyun_sts_token = (
+        os.environ.get("ALIYUN_LOG_CLI_ACCESSID"),
+        os.environ.get("ALIYUN_LOG_CLI_ACCESSKEY"),
+        os.environ.get("ALIYUN_LOG_CLI_ENDPOINT"),
+        os.environ.get("ALIYUN_LOG_CLI_STS_TOKEN"),
+    )
     endpoint = aliyun_endpoint or endpoint
     if all((aliyun_access_id, aliyun_access_key)):
-        access_id, access_key, sts_token = aliyun_access_id, aliyun_access_key, aliyun_sts_token
-    format_output = os.environ.get('ALIYUN_LOG_CLI_FORMAT_OUTPUT', format_output)
-    decode_output = os.environ.get('ALIYUN_LOG_CLI_DECODE_OUTPUT', decode_output)
+        access_id, access_key, sts_token = (
+            aliyun_access_id,
+            aliyun_access_key,
+            aliyun_sts_token,
+        )
+    format_output = os.environ.get("ALIYUN_LOG_CLI_FORMAT_OUTPUT", format_output)
+    decode_output = os.environ.get("ALIYUN_LOG_CLI_DECODE_OUTPUT", decode_output)
 
     # load config from profile mode
-    profile = system_options.get('profile', '')
+    profile = system_options.get("profile", "")
     if profile:
-        pro_access_id, pro_access_key, pro_endpoint, pro_sts_token = load_confidential_from_aliyun_client_file(ALIYUN_CLI_CONF_FILENAME, profile_mode=profile)
+        (
+            pro_access_id,
+            pro_access_key,
+            pro_endpoint,
+            pro_sts_token,
+        ) = load_confidential_from_aliyun_client_file(
+            ALIYUN_CLI_CONF_FILENAME, profile_mode=profile
+        )
         endpoint = pro_endpoint or endpoint
         if all((pro_access_id, pro_access_key)):
             access_id, access_key, sts_token = pro_access_id, pro_access_key, pro_sts_token
 
     # load config from command lines
-    _access_id, _access_key, _endpoint, _sts_token = system_options.get('access-id'), system_options.get('access-key'), \
-                                                     system_options.get('region-endpoint'), system_options.get('sts-token')
+    _access_id, _access_key, _endpoint, _sts_token = (
+        system_options.get("access-id"),
+        system_options.get("access-key"),
+        system_options.get("region-endpoint"),
+        system_options.get("sts-token"),
+    )
     endpoint = _endpoint or endpoint
     if all((_access_id, _access_key)):
         access_id, access_key, sts_token = _access_id, _access_key, _sts_token
-    format_output = system_options.get('format-output', format_output)
-    decode_output = system_options.get('decode-output', decode_output)
+    format_output = system_options.get("format-output", format_output)
+    decode_output = system_options.get("decode-output", decode_output)
 
     if not (access_id and access_key and endpoint):
         raise IncompleteAccountInfoError("Access id/key or endpoint is empty!")
 
     # load jmes filter from cmd
-    jmes_filter = system_options.get('jmes-filter', '')
+    jmes_filter = system_options.get("jmes-filter", "")
     if jmes_filter:
         try:
             jmespath.compile(jmes_filter)
         except jmespath.exceptions.ParseError as ex:
             print(ex)
             raise ValueError("Invalid JMES filter path")
 
@@ -343,28 +531,28 @@
 
 def config_logging_from_config_file():
     # load debug config from file
     config = configparser.RawConfigParser()
     config.read(LOG_CREDS_FILENAME)
 
     filename = DEFAULT_DEBUG_LOG_FILE_PATH
-    level = "warn"          # use string first
+    level = "warn"  # use string first
     fmt = DEFAULT_DEBUG_LOG_FORMAT
     datefmt = None
     filebytes = 100 * 1024 * 1024
     backupcount = 5
 
     client_name = DEBUG_SECTION_NAME
     if config.has_section(client_name):
-        filename = _get_section_option(config, client_name, 'filename', filename)
-        level = _get_section_option(config, client_name, 'level', level)
-        fmt = _get_section_option(config, client_name, 'format', fmt)
-        datefmt = _get_section_option(config, client_name, 'datefmt', datefmt)
-        filebytes = int(_get_section_option(config, client_name, 'filebytes', filebytes))
-        backupcount = int(_get_section_option(config, client_name, 'backupcount', backupcount))
+        filename = _get_section_option(config, client_name, "filename", filename)
+        level = _get_section_option(config, client_name, "level", level)
+        fmt = _get_section_option(config, client_name, "format", fmt)
+        datefmt = _get_section_option(config, client_name, "datefmt", datefmt)
+        filebytes = int(_get_section_option(config, client_name, "filebytes", filebytes))
+        backupcount = int(_get_section_option(config, client_name, "backupcount", backupcount))
 
     root = logging.getLogger()
     handler = RotatingFileHandler(filename, maxBytes=filebytes, backupCount=backupcount)
     root.setLevel(__LOGGING_LEVEL_MAP.get(level.lower().strip(), logging.WARN))
     root.addHandler(handler)
     handler.setFormatter(logging.Formatter(fmt=fmt, datefmt=datefmt))
 
@@ -382,8 +570,7 @@
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.activated:
             setattr(self.src_obj, self.src_prop, self.origin)
-
```

### Comparing `aliyun-log-cli-0.2.4/aliyunlogcli/parser.py` & `aliyun-log-cli-0.2.5/aliyunlogcli/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -383,66 +383,43 @@
     return False
 
 
 def _attach_more_cmd_docopt():
     return MORE_DOCOPT_CMD
 
 
-def _get_grouped_usage(method_list):
-    dct = OrderedDict()
-    for k in API_GROUP:
-        des = k[1] if isinstance(k, (list, tuple)) else k.title()
-        dct[des] = []
-
-    for x in method_list:
-        for k in API_GROUP:
-            key = k[0] if isinstance(k, (list, tuple)) else k
-            des = k[1] if isinstance(k, (list, tuple)) else k.title()
-            if re.search(key, x):
-                dct[des].append(x)
-                break
-        else:
-            if "Others" not in dct:
-                dct["Others"] = []
-            dct["Others"].append(x)
-
+def _get_grouped_usage():
     usage = StringIO()
-    for k, v in dct.items():
+    for k, v in SUPPORT_LIST.items():
         usage.write("\n\t")
         usage.write(k)
         usage.write("\n\t" + "-" * 35)
         for d in sorted(v):
             usage.write("\n\t")
             usage.write(d)
-
         usage.write("\n")
-
     return usage.getvalue()
 
 
-def _get_method_list(cls, black_list=None):
-    if black_list is None:
-        black_list = (r'^_.+',)
-
+def _get_method_list(cls):
     method_list = []
+    all_support_list = [i for j in SUPPORT_LIST.values() for i in j]
     for k in dir(cls):
-        m = getattr(cls, k, None)
-        if not k.startswith('_') and not _match_black_list(k, black_list) \
-                and (inspect.isfunction(m) or inspect.ismethod(m)):
+        if k in all_support_list:
             method_list.append(k)
 
     return method_list
 
 
-def parse_method_types_optdoc_from_class(cls, black_list=None):
-    method_list = _get_method_list(cls, black_list)
+def parse_method_types_optdoc_from_class(cls):
+    method_list = _get_method_list(cls)
     params_types = {}
     params_doc = {}
 
-    cli_usage_doc = USAGE_STR_TEMPLATE.format(grouped_api=_get_grouped_usage(method_list))
+    cli_usage_doc = USAGE_STR_TEMPLATE.format(grouped_api=_get_grouped_usage())
 
     opt_doc = 'Usage:\n'
     opt_doc += MORE_DOCOPT_CMD
 
     for m in method_list:
         method = getattr(cls, m, None)
         if method:
```

### Comparing `aliyun-log-cli-0.2.4/setup.py` & `aliyun-log-cli-0.2.5/setup.py`

 * *Files identical despite different names*

