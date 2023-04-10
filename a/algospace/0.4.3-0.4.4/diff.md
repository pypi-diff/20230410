# Comparing `tmp/algospace-0.4.3.tar.gz` & `tmp/algospace-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algospace-0.4.3.tar", last modified: Wed Mar 29 09:51:22 2023, max compression
+gzip compressed data, was "algospace-0.4.4.tar", last modified: Mon Apr 10 08:41:11 2023, max compression
```

## Comparing `algospace-0.4.3.tar` & `algospace-0.4.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:51:22.872854 algospace-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-29 09:51:12.000000 algospace-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-29 09:51:12.000000 algospace-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-03-29 09:51:22.872854 algospace-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-29 09:51:12.000000 algospace-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:51:22.868854 algospace-0.4.3/algospace/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:51:22.868854 algospace-0.4.3/algospace/customer/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/customer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/customer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/customer/fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/customer/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:51:22.868854 algospace-0.4.3/algospace/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:51:22.868854 algospace-0.4.3/algospace/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/docker_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/enroll.py
--rw-r--r--   0 runner    (1001) docker     (123)    41123 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/stdio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:51:22.868854 algospace-0.4.3/algospace/provider/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/templates/algospace-config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:51:22.872854 algospace-0.4.3/algospace/provider/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/templates/docker/algospace-docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/templates/docker/algospace-docker-logs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/templates/docker/algospace-docker-start.sh
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/templates/docker/algospace-docker-stop.sh
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/provider/templates/docker/algospace-dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-29 09:51:12.000000 algospace-0.4.3/algospace/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:51:22.868854 algospace-0.4.3/algospace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-03-29 09:51:22.000000 algospace-0.4.3/algospace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-29 09:51:22.000000 algospace-0.4.3/algospace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:51:22.000000 algospace-0.4.3/algospace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-29 09:51:22.000000 algospace-0.4.3/algospace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-29 09:51:22.000000 algospace-0.4.3/algospace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-29 09:51:22.000000 algospace-0.4.3/algospace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 09:51:22.872854 algospace-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-29 09:51:12.000000 algospace-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 08:41:00.000000 algospace-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-10 08:41:00.000000 algospace-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-10 08:41:11.246638 algospace-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-10 08:41:00.000000 algospace-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.242638 algospace-0.4.4/algospace/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/customer/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/customer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/customer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/customer/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/customer/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/docker_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/enroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41153 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/stdio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/provider/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/algospace-config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/provider/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-docker-logs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-docker-start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-docker-stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:41:11.246638 algospace-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-10 08:41:00.000000 algospace-0.4.4/setup.py
```

### Comparing `algospace-0.4.3/PKG-INFO` & `algospace-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.3
-Summary: AlgoSpace: A platform for displaying algorithm achievements
+Version: 0.4.4
+Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
 Project-URL: Documentation, https://algospace.top/publish
```

### Comparing `algospace-0.4.3/README.md` & `algospace-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/__init__.py` & `algospace-0.4.4/algospace/__init__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/__main__.py` & `algospace-0.4.4/algospace/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: AlgoSpace 脚本入口
 @Author: Kermit
 @Date: 2022-11-05 16:46:46
 @LastEditors: Kermit
-@LastEditTime: 2023-01-10 16:36:26
+@LastEditTime: 2023-03-30 05:13:12
 '''
 
 from argparse import ArgumentParser
 
 
 class ArgNamespace:
     command = 'command'
@@ -20,15 +20,15 @@
     generate_debian_mirror = 'generate_debian_mirror'
     generate_use_buildkit_debian_cache = 'generate_use_buildkit_debian_cache'
     generate_use_buildkit_pip_cache = 'generate_use_buildkit_pip_cache'
     cloud_deploy_reset = 'cloud_deploy_reset'
 
 
 def run():
-    parser = ArgumentParser('algospace', description='AlgoSpace 远程算法调用平台')
+    parser = ArgumentParser('algospace', description='AlgoSpace 打造我的算法模型集')
     subparsers = parser.add_subparsers(dest=ArgNamespace.command)  # ArgNamespace.command
 
     init_parser = subparsers.add_parser('init', description='初始化算法服务配置', help='初始化算法服务配置')
     start_parser = subparsers.add_parser('start', description='启动算法服务', help='启动算法服务')
     generate_parser = subparsers.add_parser('generate', description='生成容器配置', help='生成容器配置')
     enroll_parser = subparsers.add_parser('enroll', description='注册算法服务', help='注册算法服务')
     cloud_deploy_parser = subparsers.add_parser('cloud:deploy', description='部署云端托管算法', help='部署云端托管算法')
```

### Comparing `algospace-0.4.3/algospace/customer/fn.py` & `algospace-0.4.4/algospace/customer/fn.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/customer/service.py` & `algospace-0.4.4/algospace/customer/service.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/exceptions/__init__.py` & `algospace-0.4.4/algospace/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/logger.py` & `algospace-0.4.4/algospace/logger.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/login.py` & `algospace-0.4.4/algospace/login.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/provider/cloud.py` & `algospace-0.4.4/algospace/provider/cloud.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/provider/config.py` & `algospace-0.4.4/algospace/provider/config.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/provider/config_generator.py` & `algospace-0.4.4/algospace/provider/config_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/provider/config_loader.py` & `algospace-0.4.4/algospace/provider/config_loader.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/provider/docker_generator.py` & `algospace-0.4.4/algospace/provider/docker_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/provider/enroll.py` & `algospace-0.4.4/algospace/provider/enroll.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace/provider/service.py` & `algospace-0.4.4/algospace/provider/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: 算法提供者核心服务
 @Author: Kermit
 @Date: 2022-11-05 16:46:46
 @LastEditors: Kermit
-@LastEditTime: 2023-03-29 17:44:22
+@LastEditTime: 2023-04-04 14:54:51
 '''
 
 from typing import Any, Callable, Optional, List, Tuple, Union
 from algospace.logger import Logger, algospace_logger
 from algospace.util import create_timestamp_filename
 from . import config
 from .config import Algoinfo
@@ -867,14 +867,15 @@
                     await asyncio.sleep(1)
                     if times % 10 == 0:
                         # 每 10 秒发送心跳
                         await asyncio.get_running_loop().run_in_executor(None, self.send_heartbeat)
                         times = 0
                     times += 1
                 except Exception as e:
+                    times = 1
                     traceback.print_exc()
                     self.algo_logger.error(f'Heartbeat error: {str(e)}')
 
         async def subprocess_stdio_task():
             queue_stdio_exec = QueueStdIOExec(stdio_queue)
             stdio_exec = queue_stdio_exec.exec
             stdio_exec_all = queue_stdio_exec.exec_all
```

### Comparing `algospace-0.4.3/algospace/provider/stdio.py` & `algospace-0.4.4/algospace/provider/stdio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: 标准输入输出处理
 @Author: Kermit
 @Date: 2022-11-07 14:56:36
 @LastEditors: Kermit
-@LastEditTime: 2023-01-06 16:30:43
+@LastEditTime: 2023-04-10 16:37:02
 '''
 
 import sys
 import os
 from typing import Callable
 import time
 from multiprocessing import Queue
@@ -87,15 +87,15 @@
     def __getattr__(self, name: str):
         attr = getattr(self.io, name)
         if hasattr(attr, '__call__'):
             def call(*args, **kwargs):
                 self.queue.put((self.io_name, name, args, kwargs))
             return call
         else:
-            return self.io
+            return self.io.__getattribute__(name)
 
 
 class QueueStdIOExec:
     ''' 接收子进程 IO 操作并在父进程执行的处理器 '''
 
     def __init__(self, queue: Queue):
         self.queue = queue
```

### Comparing `algospace-0.4.3/algospace/provider/templates/algospace-config.py` & `algospace-0.4.4/algospace/provider/templates/algospace-config.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/algospace.egg-info/PKG-INFO` & `algospace-0.4.4/algospace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.3
-Summary: AlgoSpace: A platform for displaying algorithm achievements
+Version: 0.4.4
+Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
 Project-URL: Documentation, https://algospace.top/publish
```

### Comparing `algospace-0.4.3/algospace.egg-info/SOURCES.txt` & `algospace-0.4.4/algospace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `algospace-0.4.3/setup.py` & `algospace-0.4.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: Setuptools
 @Author: Kermit
 @Date: 2022-10-06 12:30:47
 @LastEditors: Kermit
-@LastEditTime: 2023-02-22 16:17:40
+@LastEditTime: 2023-03-30 05:11:30
 '''
 
 from setuptools import setup, find_packages
 from os import path
 
 name = 'algospace'
 with open(path.join(name, 'version.txt'), 'r', encoding='utf-8') as f:
     version = f.read().strip()
 
 setup(
     name=name,
     version=version,
     description=(
-        'AlgoSpace: A platform for displaying algorithm achievements'
+        'AlgoSpace: A platform for displaying and using algorithm achievements'
     ),
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     author='DBIIR',
     author_email='ckeming@outlook.com',
     maintainer='DBIIR',
     maintainer_email='ckeming@outlook.com',
```

