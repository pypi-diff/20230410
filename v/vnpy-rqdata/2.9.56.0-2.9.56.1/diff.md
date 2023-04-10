# Comparing `tmp/vnpy_rqdata-2.9.56.0.tar.gz` & `tmp/vnpy_rqdata-2.9.56.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_rqdata-2.9.56.0.tar", last modified: Fri Aug  5 01:27:57 2022, max compression
+gzip compressed data, was "vnpy_rqdata-2.9.56.1.tar", last modified: Tue Dec 13 07:57:10 2022, max compression
```

## Comparing `vnpy_rqdata-2.9.56.0.tar` & `vnpy_rqdata-2.9.56.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-08-05 01:27:57.312760 vnpy_rqdata-2.9.56.0/
--rw-rw-rw-   0        0        0     1109 2021-09-14 13:23:39.000000 vnpy_rqdata-2.9.56.0/LICENSE
--rw-rw-rw-   0        0        0     2635 2022-08-05 01:27:57.313782 vnpy_rqdata-2.9.56.0/PKG-INFO
--rw-rw-rw-   0        0        0     1747 2022-08-05 01:26:09.000000 vnpy_rqdata-2.9.56.0/README.md
--rw-rw-rw-   0        0        0      987 2022-08-05 01:27:57.322427 vnpy_rqdata-2.9.56.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2021-09-14 13:23:39.000000 vnpy_rqdata-2.9.56.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-05 01:27:57.287354 vnpy_rqdata-2.9.56.0/vnpy_rqdata/
--rw-rw-rw-   0        0        0     1382 2021-09-14 13:23:39.000000 vnpy_rqdata-2.9.56.0/vnpy_rqdata/__init__.py
--rw-rw-rw-   0        0        0     9809 2022-08-05 01:24:51.000000 vnpy_rqdata-2.9.56.0/vnpy_rqdata/rqdata_datafeed.py
-drwxrwxrwx   0        0        0        0 2022-08-05 01:27:57.311740 vnpy_rqdata-2.9.56.0/vnpy_rqdata.egg-info/
--rw-rw-rw-   0        0        0     2635 2022-08-05 01:27:56.000000 vnpy_rqdata-2.9.56.0/vnpy_rqdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2022-08-05 01:27:56.000000 vnpy_rqdata-2.9.56.0/vnpy_rqdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-05 01:27:56.000000 vnpy_rqdata-2.9.56.0/vnpy_rqdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-05 01:27:56.000000 vnpy_rqdata-2.9.56.0/vnpy_rqdata.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2022-08-05 01:27:56.000000 vnpy_rqdata-2.9.56.0/vnpy_rqdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-08-05 01:27:56.000000 vnpy_rqdata-2.9.56.0/vnpy_rqdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-13 07:57:10.196242 vnpy_rqdata-2.9.56.1/
+-rw-rw-rw-   0        0        0     1109 2022-11-13 00:49:24.000000 vnpy_rqdata-2.9.56.1/LICENSE
+-rw-rw-rw-   0        0        0     2612 2022-12-13 07:57:10.197263 vnpy_rqdata-2.9.56.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1747 2022-12-13 07:55:43.000000 vnpy_rqdata-2.9.56.1/README.md
+-rw-rw-rw-   0        0        0      987 2022-12-13 07:57:10.199347 vnpy_rqdata-2.9.56.1/setup.cfg
+-rw-rw-rw-   0        0        0       43 2022-11-13 00:49:24.000000 vnpy_rqdata-2.9.56.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-13 07:57:10.170272 vnpy_rqdata-2.9.56.1/vnpy_rqdata/
+-rw-rw-rw-   0        0        0     1425 2022-12-06 01:29:27.000000 vnpy_rqdata-2.9.56.1/vnpy_rqdata/__init__.py
+-rw-rw-rw-   0        0        0     9809 2022-11-13 00:49:24.000000 vnpy_rqdata-2.9.56.1/vnpy_rqdata/rqdata_datafeed.py
+-rw-rw-rw-   0        0        0     8209 2022-12-06 02:13:49.000000 vnpy_rqdata-2.9.56.1/vnpy_rqdata/rqdata_gateway.py
+drwxrwxrwx   0        0        0        0 2022-12-13 07:57:10.195202 vnpy_rqdata-2.9.56.1/vnpy_rqdata.egg-info/
+-rw-rw-rw-   0        0        0     2612 2022-12-13 07:57:09.000000 vnpy_rqdata-2.9.56.1/vnpy_rqdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2022-12-13 07:57:10.000000 vnpy_rqdata-2.9.56.1/vnpy_rqdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-13 07:57:09.000000 vnpy_rqdata-2.9.56.1/vnpy_rqdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-13 07:57:09.000000 vnpy_rqdata-2.9.56.1/vnpy_rqdata.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2022-12-13 07:57:09.000000 vnpy_rqdata-2.9.56.1/vnpy_rqdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-12-13 07:57:09.000000 vnpy_rqdata-2.9.56.1/vnpy_rqdata.egg-info/top_level.txt
```

### Comparing `vnpy_rqdata-2.9.56.0/LICENSE` & `vnpy_rqdata-2.9.56.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_rqdata-2.9.56.0/PKG-INFO` & `vnpy_rqdata-2.9.56.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vnpy_rqdata
-Version: 2.9.56.0
+Version: 2.9.56.1
 Summary: RQData datafeed for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -23,15 +22,15 @@
 # VeighNa框架的RQData数据服务接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-2.9.56.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-2.9.56.1-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
@@ -75,9 +74,7 @@
 在VeighNa中使用米筐RQData时，需要在全局配置中填写以下字段信息：
 
 |名称|含义|必填|举例|
 |---------|----|---|---|
 |datafeed.name|名称|是|rqdata|
 |datafeed.username|用户名|是|license|
 |datafeed.password|密码|是|(请填写购买或申请试用RQData后，RQData提供的token)|
-
-
```

### Comparing `vnpy_rqdata-2.9.56.0/README.md` & `vnpy_rqdata-2.9.56.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的RQData数据服务接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-2.9.56.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-2.9.56.1-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_rqdata-2.9.56.0/setup.cfg` & `vnpy_rqdata-2.9.56.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7271 6461 7461 0d0a   = vnpy_rqdata..
 00000020: 7665 7273 696f 6e20 3d20 322e 392e 3536  version = 2.9.56
-00000030: 2e30 0d0a 7572 6c20 3d20 6874 7470 733a  .0..url = https:
+00000030: 2e31 0d0a 7572 6c20 3d20 6874 7470 733a  .1..url = https:
 00000040: 2f2f 7777 772e 766e 7079 2e63 6f6d 0d0a  //www.vnpy.com..
 00000050: 6c69 6365 6e73 6520 3d20 4d49 540d 0a61  license = MIT..a
 00000060: 7574 686f 7220 3d20 5869 616f 796f 7520  uthor = Xiaoyou 
 00000070: 4368 656e 0d0a 6175 7468 6f72 5f65 6d61  Chen..author_ema
 00000080: 696c 203d 2078 6961 6f79 6f75 2e63 6865  il = xiaoyou.che
 00000090: 6e40 6d61 696c 2e76 6e70 792e 636f 6d0d  n@mail.vnpy.com.
 000000a0: 0a64 6573 6372 6970 7469 6f6e 203d 2052  .description = R
```

### Comparing `vnpy_rqdata-2.9.56.0/vnpy_rqdata/__init__.py` & `vnpy_rqdata-2.9.56.1/vnpy_rqdata/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,13 +20,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 import importlib_metadata
 
 from .rqdata_datafeed import RqdataDatafeed as Datafeed
+from .rqdata_gateway import RqdataGateway
 
 
 try:
     __version__ = importlib_metadata.version("vnpy_rqdata")
 except importlib_metadata.PackageNotFoundError:
     __version__ = "dev"
```

### Comparing `vnpy_rqdata-2.9.56.0/vnpy_rqdata/rqdata_datafeed.py` & `vnpy_rqdata-2.9.56.1/vnpy_rqdata/rqdata_datafeed.py`

 * *Files identical despite different names*

### Comparing `vnpy_rqdata-2.9.56.0/vnpy_rqdata.egg-info/PKG-INFO` & `vnpy_rqdata-2.9.56.1/vnpy_rqdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vnpy-rqdata
-Version: 2.9.56.0
+Version: 2.9.56.1
 Summary: RQData datafeed for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -23,15 +22,15 @@
 # VeighNa框架的RQData数据服务接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-2.9.56.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-2.9.56.1-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
@@ -75,9 +74,7 @@
 在VeighNa中使用米筐RQData时，需要在全局配置中填写以下字段信息：
 
 |名称|含义|必填|举例|
 |---------|----|---|---|
 |datafeed.name|名称|是|rqdata|
 |datafeed.username|用户名|是|license|
 |datafeed.password|密码|是|(请填写购买或申请试用RQData后，RQData提供的token)|
-
-
```

