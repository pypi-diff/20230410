# Comparing `tmp/nvosscript-1.1.3.tar.gz` & `tmp/nvosscript-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.1.3.tar", last modified: Thu Apr  6 11:34:07 2023, max compression
+gzip compressed data, was "nvosscript-1.1.4.tar", last modified: Mon Apr 10 08:07:22 2023, max compression
```

## Comparing `nvosscript-1.1.3.tar` & `nvosscript-1.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-06 11:34:07.523738 nvosscript-1.1.3/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.1.3/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-06 11:34:07.523524 nvosscript-1.1.3/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.1.3/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-06 11:34:07.521432 nvosscript-1.1.3/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.1.3/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    12412 2023-04-03 03:55:32.000000 nvosscript-1.1.3/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.1.3/nvos/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     6338 2023-04-06 11:31:52.000000 nvosscript-1.1.3/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3885 2023-04-06 08:59:52.000000 nvosscript-1.1.3/nvos/run.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      812 2023-03-30 03:32:22.000000 nvosscript-1.1.3/nvos/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-06 11:34:07.522725 nvosscript-1.1.3/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-06 11:34:07.000000 nvosscript-1.1.3/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-06 11:34:07.000000 nvosscript-1.1.3/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-06 11:34:07.000000 nvosscript-1.1.3/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-06 11:34:07.000000 nvosscript-1.1.3/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-06 11:34:07.000000 nvosscript-1.1.3/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-06 11:34:07.000000 nvosscript-1.1.3/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-06 11:34:07.523799 nvosscript-1.1.3/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-06 11:33:54.000000 nvosscript-1.1.3/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-06 11:34:07.522970 nvosscript-1.1.3/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.1.3/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3504 2023-04-06 11:33:59.000000 nvosscript-1.1.3/start/main.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-06 11:34:07.523104 nvosscript-1.1.3/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-06 07:02:53.000000 nvosscript-1.1.3/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.738506 nvosscript-1.1.4/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.1.4/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-10 08:07:22.738351 nvosscript-1.1.4/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.1.4/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.736632 nvosscript-1.1.4/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.1.4/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    12391 2023-04-10 07:03:10.000000 nvosscript-1.1.4/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.1.4/nvos/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     6390 2023-04-07 10:00:33.000000 nvosscript-1.1.4/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3627 2023-04-10 07:04:18.000000 nvosscript-1.1.4/nvos/run.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      812 2023-03-30 03:32:22.000000 nvosscript-1.1.4/nvos/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.737603 nvosscript-1.1.4/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-10 08:07:22.000000 nvosscript-1.1.4/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-10 08:07:22.738547 nvosscript-1.1.4/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-10 08:06:44.000000 nvosscript-1.1.4/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.737838 nvosscript-1.1.4/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.1.4/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3580 2023-04-10 08:06:51.000000 nvosscript-1.1.4/start/main.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 08:07:22.738054 nvosscript-1.1.4/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-06 07:02:53.000000 nvosscript-1.1.4/win/win_auto_script.py
```

### Comparing `nvosscript-1.1.3/LICENSE` & `nvosscript-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.3/nvos/file.py` & `nvosscript-1.1.4/nvos/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,15 @@
     file_list = []
     find_json_config(workspace_path, file_list, project_space_list)
     # 将来可以优化上传文件信息，针对于已经上传过的就不在上传
     with open(os.path.join(nvos_dir, "config"), 'w') as file:
         for item in file_list:
             file.write(json.dumps(item) + "\n")
 
-    if success:
-        # 上传文件
-        remote.upload_file(file_list, project_space_list)
+    remote.upload_file(file_list, project_space_list)
     return True
 
 
 def pull_data_from_cloud(workspace_path):
     sync_project_data(workspace_path)
 
     overwrite_file(workspace_path)
@@ -62,15 +60,14 @@
         logger.info(f"start save all file config ")
         origin_file_list.append(add_file_list)
         with open(os.path.join(nvos_path, "config"), 'w') as f:
             for item in origin_file_list:
                 f.write(json.dumps(item) + "\n")
 
 
-
 # 同步项目数据到远程
 def sync_project_data(workspace_path):
     logger.info(f"start execute sync_project_data {workspace_path}")
     project_space_path = os.path.join(workspace_path, ".ndtc", "project_space")
     origin_project_space_list = []
     if os.path.exists(project_space_path):
         with open(project_space_path, 'r') as f:
@@ -147,15 +144,16 @@
         return project_space_list
     if len(exit_git_data) == 0:
         result_list = []
         for file_path in os.listdir(workspace_path):
             if file_path == ".idea" or file_path == ".repo" or file_path == ".ndtc" or file_path == ".DS_Store":
                 continue
             if os.path.isdir(os.path.join(workspace_path, file_path)):
-                temp = {"project_space": os.path.join(workspace_path, file_path), "fileDirectory": os.path.join(workspace_path, file_path),
+                temp = {"project_space": os.path.join(workspace_path, file_path),
+                        "fileDirectory": os.path.join(workspace_path, file_path),
                         "git_branch": "nvos_default", "gitBranch": "nvos_default"}
                 result_list.append(temp)
         return result_list
 
     filter_exit_data = []
     for project_space in not_exit_git_data:
         max_prefix = ""
@@ -264,21 +262,19 @@
 def find_json_config(file_path, config_list, project_space_list):
     for file_name in os.listdir(file_path):
         if file_name == ".idea" or file_name == ".git" or file_name == ".repo" or file_name == ".ndtc" or file_name == ".DS_Store":
             continue
         if os.path.isdir(os.path.join(file_path, file_name)):
             find_json_config(os.path.join(file_path, file_name), config_list, project_space_list)
         elif file_name.endswith(".json"):
-            file_full_path = os.path.join(file_path,file_name)
+            file_full_path = os.path.join(file_path, file_name)
             for project_space in project_space_list:
                 if file_full_path.startswith(project_space["project_space"]):
                     file_data = {"file_path": os.path.join(file_path, file_name),
                                  "file_size": os.path.getsize(os.path.join(file_path, file_name)),
                                  "git_branch": project_space["git_branch"]}
                     config_list.append(file_data)
                     break
 
 
-
-
 def create_work_space(user_name, work_space):
     return "%s_%s" % (user_name, work_space)
```

### Comparing `nvosscript-1.1.3/nvos/login.py` & `nvosscript-1.1.4/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.3/nvos/remote.py` & `nvosscript-1.1.4/nvos/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                 temp_file = {"local_file_path": local_file_path, "file_name": file_name}
                 upload_list.append(temp_file)
     upload_process(upload_list, bucket)
 
 
 def upload_process(upload_list, bucket):
     global global_var
+    multiprocessing.set_start_method('spawn', True)
     cores = multiprocessing.cpu_count()
     with concurrent.futures.ThreadPoolExecutor(max_workers=cores) as executor, tqdm(desc="uploading", total=len(upload_list)) as progress:
         for index, file in enumerate(upload_list):
             executor.submit(uploading_file, file, bucket)
         time_count = 0
         addition = 0
         while True:
```

### Comparing `nvosscript-1.1.3/nvos/run.py` & `nvosscript-1.1.4/nvos/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,15 @@
 def command_init():
     status = login.check_login_status()
     if not status:
         print("Please login first. you could use login command to login this script")
         return
     workspace_path, success = utils.check_workspace_exist(os.getcwd())
     init_path = os.path.join(workspace_path, ".ndtc", "init")
-    if os.path.exists(init_path):
-        with open(init_path, 'r') as f:
-            line = f.readlines()
-        if line == workspace_path:
-            print("Don't repeat execute init command or executor init command in a subdirectory")
-            return
+
     flag = utils.check_subdirectory_workspace_exist(os.getcwd())
     if flag:
         print("The subdirectory has already bean initialized, don't repeat execute init command")
         try:
             shutil.rmtree(os.path.join(os.getcwd(), ".ndtc"))
         except OSError as e:
             print(f"Error: {os.path.join(os.getcwd(), '.ndtc')} : {e.strerror}")
```

### Comparing `nvosscript-1.1.3/nvos/utils.py` & `nvosscript-1.1.4/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.3/setup.py` & `nvosscript-1.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.1.3',
+    version='1.1.4',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.1.3/start/main.py` & `nvosscript-1.1.4/start/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,41 @@
 import os.path
 # Press ⌃R to execute it or replace it with your code.
 # Press Double ⇧ to search everywhere for classes, files, tool windows, actions, and settings.
 import sys
 import logging
 import getpass
 import argparse
+import multiprocessing
 from nvos import login, run
 
 # 创建全局记录器
 # 配置日志格式化信息
 logging.basicConfig(filename=os.path.expanduser(os.path.join("~", "logger.log")), level=logging.INFO,
                     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 logger = logging.getLogger()
 
 
 def main():
     parser = argparse.ArgumentParser(description="Script Description")
     subparsers = parser.add_subparsers(title="NVOS Script Command", dest='subcommand')
     subparsers.add_parser('login', help='The login command is the first command that must be executed.')
 
-    subparsers.add_parser('init', help='The Init command is used to initialize the workspace. Please execute the '
+    init_command = subparsers.add_parser('init', help='The Init command is used to initialize the workspace. Please execute the '
                                       'command in your workspace directory')
     subparsers.add_parser('async', help='The async command automatically synchronizes the data you modify from the cloud and to push addtion file to cloud')
     subparsers.add_parser('pull', help='The pull command pulls the data you modify from the cloud')
     subparsers.add_parser('push', help='The push command is used upload local new files or folders to the cloud')
     subparsers.add_parser('version', help='The version command will tell you this script really version')
     subparsers.add_parser('path', help='The path command will return windows service register script path, so you can '
                                        'install this script for windows like async command.You need execute "pythonw '
                                        'win_auto_script.py" and script is this command return path content')
     env = subparsers.add_parser('env', help='The env command will switch you need to network cloud, this args have dev,'
                                       'test,stg and prod.')
-    env.add_argument('-s', '--switch', help='swich you want linked cloud environment')
+    env.add_argument('-s', '--switch', help='switch you want linked cloud environment')
     args = parser.parse_args()
 
     if args.subcommand == "login":
         username = input("email：")
         password = getpass.getpass("password：")
         status = login.login_user_check(username, password)
         print(status)
@@ -45,15 +46,15 @@
     elif args.subcommand == "async":
         run.command_async()
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.1.3")
+        print("1.1.4")
     elif args.subcommand == 'env':
         run.command_env(args.switch)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
         current_file_dir = os.path.dirname(current_file_dir)
         win_path = os.path.join(current_file_dir, 'win', 'win_auto_script.py')
@@ -61,12 +62,13 @@
     else:
         parser.print_help()
         print(
             "\n\t if you still have many things you don't understand,you can take a look as https://nio.feishu.cn/wiki/wikcn9L7Di4ILQKaNmDDTrmpLqg ")
 
 
 if __name__ == '__main__':
+    multiprocessing.freeze_support()
     main()
     # flag = utils.check_subdirectory_workspace_exist("/Users/andre.zhao/Documents/test")
     # print(flag)
 
 # See PyCharm help at https://www.jetbrains.com/help/pycharm/
```

### Comparing `nvosscript-1.1.3/win/win_auto_script.py` & `nvosscript-1.1.4/win/win_auto_script.py`

 * *Files identical despite different names*

