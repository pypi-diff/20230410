# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.868.tar", last modified: Fri Apr  7 00:24:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.869.tar", last modified: Mon Apr 10 02:58:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.868.tar` & `tencentcloud-sdk-python-ckafka-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)   457098 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67457 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)     3206 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)   457296 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67457 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:58:24.000000 tencentcloud-sdk-python-ckafka-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.869/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3304,20 +3304,25 @@
 
     """
 
     def __init__(self):
         r"""
         :param TopicName: Topic名称
         :type TopicName: str
+        :param TopicId: TopicId
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TopicId: str
         """
         self.TopicName = None
+        self.TopicId = None
 
 
     def _deserialize(self, params):
         self.TopicName = params.get("TopicName")
+        self.TopicId = params.get("TopicId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.868/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.869/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.868/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.868/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.869/setup.py`

 * *Files identical despite different names*

