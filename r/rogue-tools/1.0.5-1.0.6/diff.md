# Comparing `tmp/rogue_tools-1.0.5.tar.gz` & `tmp/rogue_tools-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rogue_tools-1.0.5.tar", last modified: Tue Mar 28 11:06:23 2023, max compression
+gzip compressed data, was "rogue_tools-1.0.6.tar", last modified: Mon Apr 10 04:00:16 2023, max compression
```

## Comparing `rogue_tools-1.0.5.tar` & `rogue_tools-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 11:06:23.175510 rogue_tools-1.0.5/
--rw-rw-rw-   0        0        0      517 2023-03-28 11:06:23.174512 rogue_tools-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-28 11:06:23.158564 rogue_tools-1.0.5/rogue_tools/
--rw-rw-rw-   0        0        0        0 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/__init__.py
--rw-rw-rw-   0        0        0     6206 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/android_tool.py
--rw-rw-rw-   0        0        0     6255 2023-03-07 02:54:55.000000 rogue_tools-1.0.5/rogue_tools/excel_tool.py
--rw-rw-rw-   0        0        0     4056 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/file_tool.py
--rw-rw-rw-   0        0        0     1157 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/filter_tool.py
--rw-rw-rw-   0        0        0     2353 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/ini_tool.py
--rw-rw-rw-   0        0        0    13116 2023-03-28 10:00:02.000000 rogue_tools-1.0.5/rogue_tools/path_tool.py
--rw-rw-rw-   0        0        0     2416 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/robot_tool.py
--rw-rw-rw-   0        0        0     4064 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/show_tool.py
--rw-rw-rw-   0        0        0      147 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/string_tool.py
--rw-rw-rw-   0        0        0     1610 2023-03-28 10:13:23.000000 rogue_tools-1.0.5/rogue_tools/time_tool.py
--rw-rw-rw-   0        0        0     2922 2023-03-28 09:52:02.000000 rogue_tools-1.0.5/rogue_tools/ui_tool.py
--rw-rw-rw-   0        0        0     1967 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/web_tool.py
--rw-rw-rw-   0        0        0    17995 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/win_tool.py
--rw-rw-rw-   0        0        0     3914 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/yaml_tool.py
--rw-rw-rw-   0        0        0     1260 2023-03-03 12:10:10.000000 rogue_tools-1.0.5/rogue_tools/zip_tool.py
-drwxrwxrwx   0        0        0        0 2023-03-28 11:06:23.171521 rogue_tools-1.0.5/rogue_tools.egg-info/
--rw-rw-rw-   0        0        0      517 2023-03-28 11:06:22.000000 rogue_tools-1.0.5/rogue_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-03-28 11:06:23.000000 rogue_tools-1.0.5/rogue_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 11:06:22.000000 rogue_tools-1.0.5/rogue_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-03-28 11:06:22.000000 rogue_tools-1.0.5/rogue_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-28 11:06:22.000000 rogue_tools-1.0.5/rogue_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-28 11:06:22.000000 rogue_tools-1.0.5/rogue_tools.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-03-28 11:06:23.175510 rogue_tools-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-03-28 11:06:05.000000 rogue_tools-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:00:16.676977 rogue_tools-1.0.6/
+-rw-rw-rw-   0        0        0      517 2023-04-10 04:00:16.676006 rogue_tools-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 04:00:16.656490 rogue_tools-1.0.6/rogue_tools/
+-rw-rw-rw-   0        0        0        0 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/__init__.py
+-rw-rw-rw-   0        0        0     6206 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/android_tool.py
+-rw-rw-rw-   0        0        0     6255 2023-03-07 02:54:55.000000 rogue_tools-1.0.6/rogue_tools/excel_tool.py
+-rw-rw-rw-   0        0        0     4056 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/file_tool.py
+-rw-rw-rw-   0        0        0     1157 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/filter_tool.py
+-rw-rw-rw-   0        0        0     2353 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/ini_tool.py
+-rw-rw-rw-   0        0        0    13253 2023-04-10 03:02:30.000000 rogue_tools-1.0.6/rogue_tools/path_tool.py
+-rw-rw-rw-   0        0        0     2416 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/robot_tool.py
+-rw-rw-rw-   0        0        0     4064 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/show_tool.py
+-rw-rw-rw-   0        0        0      147 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/string_tool.py
+-rw-rw-rw-   0        0        0     1862 2023-04-10 03:55:21.000000 rogue_tools-1.0.6/rogue_tools/time_tool.py
+-rw-rw-rw-   0        0        0     2922 2023-03-28 09:52:02.000000 rogue_tools-1.0.6/rogue_tools/ui_tool.py
+-rw-rw-rw-   0        0        0     1967 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/web_tool.py
+-rw-rw-rw-   0        0        0    17995 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/win_tool.py
+-rw-rw-rw-   0        0        0     3914 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/yaml_tool.py
+-rw-rw-rw-   0        0        0     1260 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/zip_tool.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:00:16.674010 rogue_tools-1.0.6/rogue_tools.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-10 04:00:16.676977 rogue_tools-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-04-10 03:56:58.000000 rogue_tools-1.0.6/setup.py
```

### Comparing `rogue_tools-1.0.5/PKG-INFO` & `rogue_tools-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue_tools
-Version: 1.0.5
+Version: 1.0.6
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.5/rogue_tools/android_tool.py` & `rogue_tools-1.0.6/rogue_tools/android_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/excel_tool.py` & `rogue_tools-1.0.6/rogue_tools/excel_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/file_tool.py` & `rogue_tools-1.0.6/rogue_tools/file_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/filter_tool.py` & `rogue_tools-1.0.6/rogue_tools/filter_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/ini_tool.py` & `rogue_tools-1.0.6/rogue_tools/ini_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/path_tool.py` & `rogue_tools-1.0.6/rogue_tools/path_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,27 +60,31 @@
 def copy(src, tar,is_cover=False):
     '''
     通用的复制文件或者文件夹
     is_cover = True 可以不用删除旧文件夹,直接覆盖过去
     仅支持本地copy
     '''
     print(f'copy:{src} -->> {tar}')
+    if type(src) in [tuple,list]:
+        for obj in src:
+            copy(obj,tar,is_cover)
+        return
     # copy文件
     if os.path.isfile(src):
         #  复制到目录
         if os.path.isdir(tar):
             base_name = get_file_base_name(src)
             return shutil.copyfile(src, join_path(tar,base_name))
         # 复制到文件
         if os.path.isfile(tar):
             return shutil.copyfile(src, tar)
 
         else:
             make_folder(get_file_dirname(tar))
-            shutil.copyfile(src, tar)
+            copy(src, tar)
     # copy文件夹
     else:
         # 源文件不存在
         if not os.path.exists(src):
             raise Exception(f'can not find src :\n{src}')
         if os.path.isfile(tar):
             # 尝试将一个文件夹复制为文件
@@ -233,14 +237,15 @@
         except Exception:
             traceback.print_exc()
 
 def make_folder(folder_path):
     '''
     创建一个文件夹
     '''
+    print(f'make_folder:{folder_path}')
     if os.path.exists(folder_path):
         return
     if folder_path in ('',None):
         return
     try:
         os.makedirs(folder_path,mode=0o777)
     except FileExistsError:
```

### Comparing `rogue_tools-1.0.5/rogue_tools/robot_tool.py` & `rogue_tools-1.0.6/rogue_tools/robot_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/show_tool.py` & `rogue_tools-1.0.6/rogue_tools/show_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/time_tool.py` & `rogue_tools-1.0.6/rogue_tools/time_tool.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 	'''
 	tp1 = t1.split('-')
 	tp2 = t2.split('-')
 	return (int(tp2[0])-int(tp1[0]))*3600000+(int(tp2[1])-int(tp1[1]))*60000+(int(tp2[2])-int(tp1[2]))*1000+(int(tp2[3])-int(tp1[3]))
 	
 
 
+def get_now_ms(time_stamp = None,delay_stamp_ms=0):
+	if time_stamp == None:
+		time_stamp = time.time()
+	x = str(int(time_stamp * 1000) % 1000).rjust(3,'0')
+	return time.strftime(f"%Y-%m-%d_%H-%M-%S-{x}", time.localtime(time_stamp+delay_stamp_ms/1000))
 
 def get_now_time():
 	return time.strftime("%Y-%m-%d_%H-%M-%S", time.localtime())
 def get_now_date():
 	return time.strftime("%Y-%m-%d", time.localtime())
 
 def get_next_date(days=1):
```

### Comparing `rogue_tools-1.0.5/rogue_tools/ui_tool.py` & `rogue_tools-1.0.6/rogue_tools/ui_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/web_tool.py` & `rogue_tools-1.0.6/rogue_tools/web_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/win_tool.py` & `rogue_tools-1.0.6/rogue_tools/win_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/yaml_tool.py` & `rogue_tools-1.0.6/rogue_tools/yaml_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools/zip_tool.py` & `rogue_tools-1.0.6/rogue_tools/zip_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/rogue_tools.egg-info/PKG-INFO` & `rogue_tools-1.0.6/rogue_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue-tools
-Version: 1.0.5
+Version: 1.0.6
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.5/rogue_tools.egg-info/SOURCES.txt` & `rogue_tools-1.0.6/rogue_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.5/setup.py` & `rogue_tools-1.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 except ImportError:
     from distutils.core import setup
 import setuptools
 
 setup(
     name='rogue_tools',  # 包的名字
     author='luohao',  # 作者
-    version='1.0.5',  # 版本号
+    version='1.0.6',  # 版本号
     license='MIT',
 
     description='private tools',  # 描述
     long_description='''long description''',
     author_email='luohao@aobi.com',  # 你的邮箱**
     url='',  # 可以写github上的地址，或者其他地址
     # 包内需要引用的文件夹
```

