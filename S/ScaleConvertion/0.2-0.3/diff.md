# Comparing `tmp/ScaleConvertion-0.2.tar.gz` & `tmp/ScaleConvertion-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ScaleConvertion-0.2.tar", last modified: Sun Apr  9 16:14:38 2023, max compression
+gzip compressed data, was "dist\ScaleConvertion-0.3.tar", last modified: Mon Apr 10 01:49:31 2023, max compression
```

## Comparing `ScaleConvertion-0.2.tar` & `ScaleConvertion-0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/
--rw-rw-rw-   0        0        0     1189 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-09 16:11:33.000000 ScaleConvertion-0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion/
-drwxrwxrwx   0        0        0        0 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion/Model/
--rw-rw-rw-   0        0        0     7201 2023-04-09 06:38:21.000000 ScaleConvertion-0.2/ScaleConvertion/Model/Efficientnet.py
--rw-rw-rw-   0        0        0    12126 2023-03-05 09:30:27.000000 ScaleConvertion-0.2/ScaleConvertion/Model/Restnet.py
--rw-rw-rw-   0        0        0     9277 2023-04-09 06:38:21.000000 ScaleConvertion-0.2/ScaleConvertion/Model/SwimModel.py
--rw-rw-rw-   0        0        0     9351 2023-04-09 06:38:21.000000 ScaleConvertion-0.2/ScaleConvertion/Model/SwimModel_2.py
--rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.2/ScaleConvertion/Model/__init__.py
--rw-rw-rw-   0        0        0    26665 2023-04-09 06:38:21.000000 ScaleConvertion-0.2/ScaleConvertion/Model/restnet_transformer.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion/PicProcess/
--rw-rw-rw-   0        0        0      556 2023-04-09 11:16:51.000000 ScaleConvertion-0.2/ScaleConvertion/PicProcess/ConcatAnswer.py
--rw-rw-rw-   0        0        0     2962 2023-04-09 15:57:59.000000 ScaleConvertion-0.2/ScaleConvertion/PicProcess/DataPredict.py
--rw-rw-rw-   0        0        0     9504 2023-04-09 14:53:26.000000 ScaleConvertion-0.2/ScaleConvertion/PicProcess/Draw_Window.py
--rw-rw-rw-   0        0        0     2232 2023-04-09 12:04:26.000000 ScaleConvertion-0.2/ScaleConvertion/PicProcess/MakeData.py
--rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.2/ScaleConvertion/PicProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion/Utiles/
--rw-rw-rw-   0        0        0      853 2023-04-09 15:59:04.000000 ScaleConvertion-0.2/ScaleConvertion/Utiles/Info.py
--rw-rw-rw-   0        0        0     1172 2023-04-09 14:00:58.000000 ScaleConvertion-0.2/ScaleConvertion/Utiles/PictureInfo.py
--rw-rw-rw-   0        0        0     7930 2023-01-04 15:45:26.000000 ScaleConvertion-0.2/ScaleConvertion/Utiles/SED.py
--rw-rw-rw-   0        0        0      878 2023-04-09 12:12:21.000000 ScaleConvertion-0.2/ScaleConvertion/Utiles/SaveFile.py
--rw-rw-rw-   0        0        0     1308 2023-04-09 08:10:19.000000 ScaleConvertion-0.2/ScaleConvertion/Utiles/ScaleCompute.py
--rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.2/ScaleConvertion/Utiles/__init__.py
--rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.2/ScaleConvertion/__init__.py
--rw-rw-rw-   0        0        0      993 2023-04-09 15:01:28.000000 ScaleConvertion-0.2/ScaleConvertion/main.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion.egg-info/
--rw-rw-rw-   0        0        0     1189 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      900 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/ScaleConvertion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 16:14:38.000000 ScaleConvertion-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1565 2023-04-09 16:14:31.000000 ScaleConvertion-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/
+-rw-rw-rw-   0        0        0     1189 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-04-09 16:11:33.000000 ScaleConvertion-0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion/
+drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion/Model/
+-rw-rw-rw-   0        0        0     7201 2023-04-09 06:38:21.000000 ScaleConvertion-0.3/ScaleConvertion/Model/Efficientnet.py
+-rw-rw-rw-   0        0        0    12126 2023-03-05 09:30:27.000000 ScaleConvertion-0.3/ScaleConvertion/Model/Restnet.py
+-rw-rw-rw-   0        0        0     9277 2023-04-09 06:38:21.000000 ScaleConvertion-0.3/ScaleConvertion/Model/SwimModel.py
+-rw-rw-rw-   0        0        0     9351 2023-04-09 06:38:21.000000 ScaleConvertion-0.3/ScaleConvertion/Model/SwimModel_2.py
+-rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.3/ScaleConvertion/Model/__init__.py
+-rw-rw-rw-   0        0        0    26665 2023-04-09 06:38:21.000000 ScaleConvertion-0.3/ScaleConvertion/Model/restnet_transformer.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/
+-rw-rw-rw-   0        0        0      556 2023-04-09 11:16:51.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/ConcatAnswer.py
+-rw-rw-rw-   0        0        0     2962 2023-04-09 15:57:59.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/DataPredict.py
+-rw-rw-rw-   0        0        0     9504 2023-04-09 14:53:26.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/Draw_Window.py
+-rw-rw-rw-   0        0        0     2232 2023-04-09 12:04:26.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/MakeData.py
+-rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/
+-rw-rw-rw-   0        0        0      853 2023-04-09 15:59:04.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/Info.py
+-rw-rw-rw-   0        0        0     1172 2023-04-09 14:00:58.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/PictureInfo.py
+-rw-rw-rw-   0        0        0     7930 2023-01-04 15:45:26.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/SED.py
+-rw-rw-rw-   0        0        0      878 2023-04-09 12:12:21.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/SaveFile.py
+-rw-rw-rw-   0        0        0     1308 2023-04-09 08:10:19.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/ScaleCompute.py
+-rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/__init__.py
+-rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.3/ScaleConvertion/__init__.py
+-rw-rw-rw-   0        0        0      993 2023-04-09 15:01:28.000000 ScaleConvertion-0.3/ScaleConvertion/main.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/
+-rw-rw-rw-   0        0        0     1189 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      900 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1936 2023-04-10 01:47:32.000000 ScaleConvertion-0.3/setup.py
```

### Comparing `ScaleConvertion-0.2/PKG-INFO` & `ScaleConvertion-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ScaleConvertion
-Version: 0.2
+Version: 0.3
 Summary: Helps achieve surface reflectance scale conversion
 Home-page: https://github.com/qxcnwu
 Author: qxcnwu
 Author-email: qxcnwu@gmail.com
 Maintainer: qxcnwu
 Maintainer-email: qxcnwu@gmail.com
 License: MIT License
```

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Model/Efficientnet.py` & `ScaleConvertion-0.3/ScaleConvertion/Model/Efficientnet.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Model/Restnet.py` & `ScaleConvertion-0.3/ScaleConvertion/Model/Restnet.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Model/SwimModel.py` & `ScaleConvertion-0.3/ScaleConvertion/Model/SwimModel.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Model/SwimModel_2.py` & `ScaleConvertion-0.3/ScaleConvertion/Model/SwimModel_2.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Model/restnet_transformer.py` & `ScaleConvertion-0.3/ScaleConvertion/Model/restnet_transformer.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/PicProcess/ConcatAnswer.py` & `ScaleConvertion-0.3/ScaleConvertion/PicProcess/ConcatAnswer.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/PicProcess/DataPredict.py` & `ScaleConvertion-0.3/ScaleConvertion/PicProcess/DataPredict.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/PicProcess/Draw_Window.py` & `ScaleConvertion-0.3/ScaleConvertion/PicProcess/Draw_Window.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/PicProcess/MakeData.py` & `ScaleConvertion-0.3/ScaleConvertion/PicProcess/MakeData.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Utiles/Info.py` & `ScaleConvertion-0.3/ScaleConvertion/Utiles/Info.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Utiles/PictureInfo.py` & `ScaleConvertion-0.3/ScaleConvertion/Utiles/PictureInfo.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Utiles/SED.py` & `ScaleConvertion-0.3/ScaleConvertion/Utiles/SED.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Utiles/SaveFile.py` & `ScaleConvertion-0.3/ScaleConvertion/Utiles/SaveFile.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/Utiles/ScaleCompute.py` & `ScaleConvertion-0.3/ScaleConvertion/Utiles/ScaleCompute.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion/main.py` & `ScaleConvertion-0.3/ScaleConvertion/main.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/ScaleConvertion.egg-info/PKG-INFO` & `ScaleConvertion-0.3/ScaleConvertion.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ScaleConvertion
-Version: 0.2
+Version: 0.3
 Summary: Helps achieve surface reflectance scale conversion
 Home-page: https://github.com/qxcnwu
 Author: qxcnwu
 Author-email: qxcnwu@gmail.com
 Maintainer: qxcnwu
 Maintainer-email: qxcnwu@gmail.com
 License: MIT License
```

### Comparing `ScaleConvertion-0.2/ScaleConvertion.egg-info/SOURCES.txt` & `ScaleConvertion-0.3/ScaleConvertion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.2/setup.py` & `ScaleConvertion-0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+'''
+Author: qxcnwu 2081896628@qq.com
+Date: 2023-04-09 21:34:20
+LastEditors: qxcnwu 2081896628@qq.com
+LastEditTime: 2023-04-10 00:18:40
+FilePath: \package\setup.py
+Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
+'''
 # -*- coding: utf-8 -*-
 # @Time    : 2023/4/9 21:34
 # @Author  : qxcnwu
 # @FileName: setup.py
 # @Software: PyCharm
 from setuptools import setup, find_packages
 
 setup(
     name='ScaleConvertion',  # 包名
-    version='0.2',  # 版本
+    version='0.3',  # 版本
     description="Helps achieve surface reflectance scale conversion",  # 包简介
     long_description=open('README.rst').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='qxcnwu',  # 作者
     author_email='qxcnwu@gmail.com',  # 作者邮件
     maintainer='qxcnwu',  # 维护者
     maintainer_email='qxcnwu@gmail.com',  # 维护者邮件
@@ -24,14 +32,14 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',  # 设置编写时的python版本
     ],
     python_requires='>=3.4',  # 设置python版本要求
     install_requires=['tqdm', 'numpy', 'pandas', 'torch', 'timm', 'exifread', 'qt5_applications', 'matplotlib',
-                      'torchvision', 'requests'],  # 安装所需要的库
+                      'torchvision', 'requests', 'colour', 'opencv-python'],  # 安装所需要的库
     # entry_points={
     #     'console_scripts': [
     #         ''],
     # },  # 设置命令行工具(可不使用就可以注释掉)
 
 )
```

