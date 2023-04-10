# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.868.tar", last modified: Fri Apr  7 01:03:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.869.tar", last modified: Mon Apr 10 03:16:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.868.tar` & `tencentcloud-sdk-python-tke-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   638945 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19267 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   176385 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 01:03:20.000000 tencentcloud-sdk-python-tke-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)   638897 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19267 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   176385 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:16:38.000000 tencentcloud-sdk-python-tke-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tke-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.869/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         :type NodePool: :class:`tencentcloud.tke.v20180525.models.NodePoolOption`
         :param SkipValidateOptions: 校验规则相关选项，可配置跳过某些校验规则。目前支持GlobalRouteCIDRCheck（跳过GlobalRouter的相关校验），VpcCniCIDRCheck（跳过VpcCni相关校验）
         :type SkipValidateOptions: list of str
         :param InstanceAdvancedSettingsOverrides: 参数InstanceAdvancedSettingsOverride数组用于定制化地配置各台instance，与InstanceIds顺序对应。当传入InstanceAdvancedSettingsOverrides数组时，将覆盖默认参数InstanceAdvancedSettings；当没有传入参数InstanceAdvancedSettingsOverrides时，InstanceAdvancedSettings参数对每台instance生效。
 
 参数InstanceAdvancedSettingsOverride数组的长度应与InstanceIds数组一致；当长度大于InstanceIds数组长度时将报错；当长度小于InstanceIds数组时，没有对应配置的instace将使用默认配置。
         :type InstanceAdvancedSettingsOverrides: list of InstanceAdvancedSettings
-        :param ImageId: 节点镜像（节点选项时，该参数是必传参数）
+        :param ImageId: 节点镜像
         :type ImageId: str
         """
         self.ClusterId = None
         self.InstanceIds = None
         self.InstanceAdvancedSettings = None
         self.EnhancedService = None
         self.LoginSettings = None
```

### Comparing `tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.868/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.869/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.868/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.869/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.868/README.rst` & `tencentcloud-sdk-python-tke-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.868/setup.py` & `tencentcloud-sdk-python-tke-3.0.869/setup.py`

 * *Files identical despite different names*

