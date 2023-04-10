# Comparing `tmp/nvosscript-1.1.4.tar.gz` & `tmp/nvosscript-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.1.4.tar", last modified: Mon Apr 10 08:07:22 2023, max compression
+gzip compressed data, was "nvosscript-1.1.5.tar", last modified: Mon Apr 10 11:42:00 2023, max compression
```

## Comparing `nvosscript-1.1.4.tar` & `nvosscript-1.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.738506 nvosscript-1.1.4/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.1.4/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-10 08:07:22.738351 nvosscript-1.1.4/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.1.4/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.736632 nvosscript-1.1.4/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.1.4/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    12391 2023-04-10 07:03:10.000000 nvosscript-1.1.4/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.1.4/nvos/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     6390 2023-04-07 10:00:33.000000 nvosscript-1.1.4/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3627 2023-04-10 07:04:18.000000 nvosscript-1.1.4/nvos/run.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      812 2023-03-30 03:32:22.000000 nvosscript-1.1.4/nvos/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.737603 nvosscript-1.1.4/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-10 08:07:22.738547 nvosscript-1.1.4/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-10 08:06:44.000000 nvosscript-1.1.4/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.737838 nvosscript-1.1.4/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.1.4/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3580 2023-04-10 08:06:51.000000 nvosscript-1.1.4/start/main.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.738054 nvosscript-1.1.4/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-06 07:02:53.000000 nvosscript-1.1.4/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.835532 nvosscript-1.1.5/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.1.5/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-10 11:42:00.835392 nvosscript-1.1.5/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.1.5/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.833397 nvosscript-1.1.5/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.1.5/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    12391 2023-04-10 07:03:10.000000 nvosscript-1.1.5/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.1.5/nvos/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     7331 2023-04-10 10:09:11.000000 nvosscript-1.1.5/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3524 2023-04-10 09:34:12.000000 nvosscript-1.1.5/nvos/run.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      812 2023-03-30 03:32:22.000000 nvosscript-1.1.5/nvos/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.834502 nvosscript-1.1.5/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-10 11:42:00.835584 nvosscript-1.1.5/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-10 10:14:52.000000 nvosscript-1.1.5/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.834745 nvosscript-1.1.5/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.1.5/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3480 2023-04-10 10:15:03.000000 nvosscript-1.1.5/start/main.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.835058 nvosscript-1.1.5/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-06 07:02:53.000000 nvosscript-1.1.5/win/win_auto_script.py
```

### Comparing `nvosscript-1.1.4/LICENSE` & `nvosscript-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.4/nvos/file.py` & `nvosscript-1.1.5/nvos/file.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.4/nvos/login.py` & `nvosscript-1.1.5/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.4/nvos/remote.py` & `nvosscript-1.1.5/nvos/remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,20 +15,39 @@
 # 导入全局日志记录器
 logger = logging.getLogger(__name__)
 daemon_network = "https://nvos-toolchain.nioint.com"
 
 daemon_network_mapping = {
     "prod": "https://nvos-toolchain.nioint.com",
     "stg": "https://nvos-toolchain-stg.nioint.com",
-    "test": "https://nvos-toolchain-test.nioint.com",
     "dev": "https://nvos-toolchain-dev.nioint.com"
 }
+
+daemon_network_front_mapping = {
+    "prod": "https://ndtc.nioint.com/#/nvosTool/spaceList",
+    "stg": "https://ndtc-stg.nioint.com/#/nvosTool/spaceList",
+    "dev": " https://soa-tools-dev.nioint.com/#/nvosTool/spaceList"
+}
 global_var = 0
 
 
+def upload_client_script():
+    get_current_env()
+    s3_secret = get_s3_secret()
+    bucket_name = s3_secret["bucket"]
+    aws_ak = s3_secret["ak"]
+    aws_sk = s3_secret["sk"]
+    aws_region = s3_secret["regionId"]
+    s3 = boto3.resource('s3', region_name=aws_region, aws_access_key_id=aws_ak,
+                        aws_secret_access_key=aws_sk)
+    bucket = s3.Bucket(bucket_name)
+    file_path = "/Users/andre.zhao/PycharmProjects/nvos-script/dist/nvosscript.zip"
+    file_name = "/nvos-script/nvosscript.zip"
+    bucket.upload_file(file_path, file_name)
+
 def upload_file(file_path_list, project_space_list):
     s3_secret = get_s3_secret()
     bucket_name = s3_secret["bucket"]
     aws_ak = s3_secret["ak"]
     aws_sk = s3_secret["sk"]
     aws_region = s3_secret["regionId"]
     s3 = boto3.resource('s3', region_name=aws_region, aws_access_key_id=aws_ak,
@@ -126,16 +145,20 @@
 
 def post_data(url, params):
     headers = {"content-type": "application/json"}
     logger.info(f'request url:{url} params:{params}')
     response = requests.post(url, headers=headers, data=json.dumps(params))
     logger.info(f"response status_code: {response.status_code} text: {response.text} \n content:{response.content}")
     if response.status_code == 200:
-        response_data = json.loads(response.text)["data"]
-        return response_data
+        result = json.loads(response.text)
+        if result["code"] == "200":
+            return result["data"]
+        else:
+            message = result["message"]
+            raise Exception('please error message is :{}'.format(message))
     return {}
 
 
 def md5(git_branch, project_space):
     string = "%s%s" % (git_branch, project_space)
     hash_object = hashlib.md5(string.encode())
     md5_hash = hash_object.hexdigest()
@@ -159,17 +182,18 @@
     return {}
 
 
 def switch_env(env):
     val = daemon_network_mapping.get(env)
     if len(val) == 0:
         return
-    with open(os.path.expanduser(os.path.join('~','nvos_env')),'w') as f:
+    with open(os.path.expanduser(os.path.join('~', 'nvos_env')), 'w') as f:
         f.writelines(val)
-    print(f"this script current env:{env} and cloud linked:{val}")
+    tip = daemon_network_front_mapping.get(env)
+    print(f"this script current env:{env} and cloud linked:{tip}")
 
 
 def get_current_env():
     global daemon_network
     if os.path.exists(os.path.expanduser(os.path.join('~', 'nvos_env'))):
         with open(os.path.expanduser(os.path.join('~', 'nvos_env')), 'r')as f:
             daemon_network = f.readline()
```

### Comparing `nvosscript-1.1.4/nvos/run.py` & `nvosscript-1.1.5/nvos/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,14 +97,9 @@
     status = login.check_login_status()
     if not status:
         print("Please login first. you could use login command to login this script")
         return workspace_path, False
     return workspace_path, True
 
 
-# 登录以后初始化一些必要信息
-def login_init_data():
-    result = remote.get_s3_secret()
-
-
 def command_env(env):
     remote.switch_env(env)
```

### Comparing `nvosscript-1.1.4/nvos/utils.py` & `nvosscript-1.1.5/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.4/setup.py` & `nvosscript-1.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.1.4',
+    version='1.1.5',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.1.4/start/main.py` & `nvosscript-1.1.5/start/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Press ⌃R to execute it or replace it with your code.
 # Press Double ⇧ to search everywhere for classes, files, tool windows, actions, and settings.
 import sys
 import logging
 import getpass
 import argparse
 import multiprocessing
-from nvos import login, run
+from nvos import login, run,remote
 
 # 创建全局记录器
 # 配置日志格式化信息
 logging.basicConfig(filename=os.path.expanduser(os.path.join("~", "logger.log")), level=logging.INFO,
                     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 logger = logging.getLogger()
 
@@ -27,34 +27,33 @@
     subparsers.add_parser('pull', help='The pull command pulls the data you modify from the cloud')
     subparsers.add_parser('push', help='The push command is used upload local new files or folders to the cloud')
     subparsers.add_parser('version', help='The version command will tell you this script really version')
     subparsers.add_parser('path', help='The path command will return windows service register script path, so you can '
                                        'install this script for windows like async command.You need execute "pythonw '
                                        'win_auto_script.py" and script is this command return path content')
     env = subparsers.add_parser('env', help='The env command will switch you need to network cloud, this args have dev,'
-                                      'test,stg and prod.')
+                                      'stg and prod.')
     env.add_argument('-s', '--switch', help='switch you want linked cloud environment')
     args = parser.parse_args()
 
     if args.subcommand == "login":
         username = input("email：")
         password = getpass.getpass("password：")
         status = login.login_user_check(username, password)
         print(status)
-        run.login_init_data()
     elif args.subcommand == "init":
         run.command_init()
     elif args.subcommand == "async":
         run.command_async()
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.1.4")
+        print("1.1.5")
     elif args.subcommand == 'env':
         run.command_env(args.switch)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
         current_file_dir = os.path.dirname(current_file_dir)
         win_path = os.path.join(current_file_dir, 'win', 'win_auto_script.py')
@@ -64,11 +63,10 @@
         print(
             "\n\t if you still have many things you don't understand,you can take a look as https://nio.feishu.cn/wiki/wikcn9L7Di4ILQKaNmDDTrmpLqg ")
 
 
 if __name__ == '__main__':
     multiprocessing.freeze_support()
     main()
-    # flag = utils.check_subdirectory_workspace_exist("/Users/andre.zhao/Documents/test")
-    # print(flag)
+    # remote.upload_client_script()
 
 # See PyCharm help at https://www.jetbrains.com/help/pycharm/
```

### Comparing `nvosscript-1.1.4/win/win_auto_script.py` & `nvosscript-1.1.5/win/win_auto_script.py`

 * *Files identical despite different names*

