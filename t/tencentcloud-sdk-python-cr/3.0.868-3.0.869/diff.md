# Comparing `tmp/tencentcloud-sdk-python-cr-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-cr-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cr-3.0.868.tar", last modified: Fri Apr  7 00:25:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cr-3.0.869.tar", last modified: Mon Apr 10 02:59:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cr-3.0.868.tar` & `tencentcloud-sdk-python-cr-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1654 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:25:43.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/v20180321/
--rw-r--r--   0 root         (0) root         (0)    83768 2023-04-07 00:25:43.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:25:43.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-04-07 00:25:43.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    26019 2023-04-07 00:25:43.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/v20180321/cr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:25:43.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud_sdk_python_cr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1654 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud_sdk_python_cr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud_sdk_python_cr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud_sdk_python_cr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/tencentcloud_sdk_python_cr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      734 2023-04-07 00:25:43.000000 tencentcloud-sdk-python-cr-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1004 2023-04-07 00:25:43.000000 tencentcloud-sdk-python-cr-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:25:44.000000 tencentcloud-sdk-python-cr-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/v20180321/
+-rw-r--r--   0 root         (0) root         (0)    83768 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26019 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/v20180321/cr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud_sdk_python_cr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud_sdk_python_cr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud_sdk_python_cr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud_sdk_python_cr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/tencentcloud_sdk_python_cr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      734 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:59:31.000000 tencentcloud-sdk-python-cr-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cr-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-cr-3.0.869/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cr
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cr-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cr-3.0.869/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.868'
+__version__ = '3.0.869'
```

### Comparing `tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/v20180321/models.py` & `tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/v20180321/errorcodes.py` & `tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.868/tencentcloud/cr/v20180321/cr_client.py` & `tencentcloud-sdk-python-cr-3.0.869/tencentcloud/cr/v20180321/cr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.868/tencentcloud_sdk_python_cr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cr-3.0.869/tencentcloud_sdk_python_cr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cr
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cr-3.0.868/README.rst` & `tencentcloud-sdk-python-cr-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.868/setup.py` & `tencentcloud-sdk-python-cr-3.0.869/setup.py`

 * *Files identical despite different names*

