# Comparing `tmp/tencentcloud-sdk-python-yinsuda-3.0.867.tar.gz` & `tmp/tencentcloud-sdk-python-yinsuda-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.867.tar", last modified: Wed Apr  5 17:01:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.869.tar", last modified: Mon Apr 10 03:18:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yinsuda-3.0.867.tar` & `tencentcloud-sdk-python-yinsuda-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud_sdk_python_yinsuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/v20220527/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/v20220527/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/v20220527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    15889 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/v20220527/yinsuda_client.py
--rw-r--r--   0 root         (0) root         (0)    71047 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/v20220527/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-05 17:01:01.000000 tencentcloud-sdk-python-yinsuda-3.0.867/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/v20220527/
+-rw-r--r--   0 root         (0) root         (0)    71047 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/v20220527/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/v20220527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/v20220527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    15889 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/v20220527/yinsuda_client.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud_sdk_python_yinsuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:18:59.000000 tencentcloud-sdk-python-yinsuda-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.869/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.867
+Version: 3.0.869
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.867/setup.py` & `tencentcloud-sdk-python-yinsuda-3.0.869/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/v20220527/errorcodes.py` & `tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/v20220527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/v20220527/yinsuda_client.py` & `tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/v20220527/yinsuda_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/yinsuda/v20220527/models.py` & `tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/yinsuda/v20220527/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.867/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.867'
+__version__ = '3.0.869'
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.867/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.869/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.867
+Version: 3.0.869
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.867/README.rst` & `tencentcloud-sdk-python-yinsuda-3.0.869/README.rst`

 * *Files identical despite different names*

