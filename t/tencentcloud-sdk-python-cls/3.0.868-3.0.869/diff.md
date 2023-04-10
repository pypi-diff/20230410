# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.868.tar", last modified: Fri Apr  7 00:24:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.869.tar", last modified: Mon Apr 10 02:58:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.868.tar` & `tencentcloud-sdk-python-cls-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)   237759 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    66970 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:24:57.000000 tencentcloud-sdk-python-cls-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)   238657 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    66970 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.869/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2023,23 +2023,30 @@
         :type AutoSplit: bool
         :param MaxSplitPartitions: 开启自动分裂后，每个主题能够允许的最大分区数，默认值为50
         :type MaxSplitPartitions: int
         :param StorageType: 日志主题的存储类型，可选值 hot（标准存储），cold（低频存储）；默认为hot。
         :type StorageType: str
         :param Period: 生命周期，单位天，标准存储取值范围1\~3600，低频存储取值范围7\~3600天。取值为3640时代表永久保存
         :type Period: int
+        :param Describes: 日志主题描述
+        :type Describes: str
+        :param HotPeriod: 0：关闭日志沉降。
+非0：开启日志沉降后标准存储的天数。HotPeriod需要大于等于7，且小于Period。仅在StorageType为 hot 时生效
+        :type HotPeriod: int
         """
         self.LogsetId = None
         self.TopicName = None
         self.PartitionCount = None
         self.Tags = None
         self.AutoSplit = None
         self.MaxSplitPartitions = None
         self.StorageType = None
         self.Period = None
+        self.Describes = None
+        self.HotPeriod = None
 
 
     def _deserialize(self, params):
         self.LogsetId = params.get("LogsetId")
         self.TopicName = params.get("TopicName")
         self.PartitionCount = params.get("PartitionCount")
         if params.get("Tags") is not None:
@@ -2048,14 +2055,16 @@
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.AutoSplit = params.get("AutoSplit")
         self.MaxSplitPartitions = params.get("MaxSplitPartitions")
         self.StorageType = params.get("StorageType")
         self.Period = params.get("Period")
+        self.Describes = params.get("Describes")
+        self.HotPeriod = params.get("HotPeriod")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5855,22 +5864,29 @@
         :type Status: bool
         :param AutoSplit: 是否开启自动分裂
         :type AutoSplit: bool
         :param MaxSplitPartitions: 若开启最大分裂，该主题能够能够允许的最大分区数
         :type MaxSplitPartitions: int
         :param Period: 生命周期，单位天，标准存储取值范围1\~3600，低频存储取值范围7\~3600。取值为3640时代表永久保存
         :type Period: int
+        :param Describes: 日志主题描述
+        :type Describes: str
+        :param HotPeriod: 0：关闭日志沉降。
+非0：开启日志沉降后标准存储的天数。HotPeriod需要大于等于7，且小于Period。仅在StorageType为 hot 时生效
+        :type HotPeriod: int
         """
         self.TopicId = None
         self.TopicName = None
         self.Tags = None
         self.Status = None
         self.AutoSplit = None
         self.MaxSplitPartitions = None
         self.Period = None
+        self.Describes = None
+        self.HotPeriod = None
 
 
     def _deserialize(self, params):
         self.TopicId = params.get("TopicId")
         self.TopicName = params.get("TopicName")
         if params.get("Tags") is not None:
             self.Tags = []
@@ -5878,14 +5894,16 @@
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.Status = params.get("Status")
         self.AutoSplit = params.get("AutoSplit")
         self.MaxSplitPartitions = params.get("MaxSplitPartitions")
         self.Period = params.get("Period")
+        self.Describes = params.get("Describes")
+        self.HotPeriod = params.get("HotPeriod")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.868/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.868/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.868/README.rst` & `tencentcloud-sdk-python-cls-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.868/setup.py` & `tencentcloud-sdk-python-cls-3.0.869/setup.py`

 * *Files identical despite different names*

