# Comparing `tmp/tencentcloud-sdk-python-cdc-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-cdc-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdc-3.0.868.tar", last modified: Fri Apr  7 00:22:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdc-3.0.869.tar", last modified: Mon Apr 10 02:57:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdc-3.0.868.tar` & `tencentcloud-sdk-python-cdc-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/v20201214/
--rw-r--r--   0 root         (0) root         (0)    84528 2023-04-07 00:22:57.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/v20201214/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:22:57.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/v20201214/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19359 2023-04-07 00:22:57.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/v20201214/cdc_client.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-04-07 00:22:57.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/v20201214/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:22:57.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:22:57.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 00:22:57.000000 tencentcloud-sdk-python-cdc-3.0.868/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud_sdk_python_cdc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud_sdk_python_cdc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud_sdk_python_cdc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud_sdk_python_cdc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/tencentcloud_sdk_python_cdc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-07 00:22:57.000000 tencentcloud-sdk-python-cdc-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:22:58.000000 tencentcloud-sdk-python-cdc-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/v20201214/
+-rw-r--r--   0 root         (0) root         (0)    84528 2023-04-10 02:57:12.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/v20201214/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:57:12.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/v20201214/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19359 2023-04-10 02:57:12.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/v20201214/cdc_client.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-04-10 02:57:12.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/v20201214/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:57:12.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:57:12.000000 tencentcloud-sdk-python-cdc-3.0.869/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud_sdk_python_cdc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud_sdk_python_cdc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud_sdk_python_cdc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud_sdk_python_cdc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/tencentcloud_sdk_python_cdc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:57:12.000000 tencentcloud-sdk-python-cdc-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:57:13.000000 tencentcloud-sdk-python-cdc-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdc-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-cdc-3.0.869/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdc
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cdc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/v20201214/models.py` & `tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/v20201214/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/v20201214/cdc_client.py` & `tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/v20201214/cdc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/cdc/v20201214/errorcodes.py` & `tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/cdc/v20201214/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdc-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdc-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdc-3.0.868/README.rst` & `tencentcloud-sdk-python-cdc-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdc-3.0.868/tencentcloud_sdk_python_cdc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdc-3.0.869/tencentcloud_sdk_python_cdc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdc
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cdc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdc-3.0.868/setup.py` & `tencentcloud-sdk-python-cdc-3.0.869/setup.py`

 * *Files identical despite different names*

