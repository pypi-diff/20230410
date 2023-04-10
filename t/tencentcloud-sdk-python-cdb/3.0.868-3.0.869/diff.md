# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.868.tar", last modified: Fri Apr  7 00:22:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.869.tar", last modified: Mon Apr 10 02:57:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.868.tar` & `tencentcloud-sdk-python-cdb-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:22:50.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   485267 2023-04-07 00:22:50.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:22:50.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18041 2023-04-07 00:22:50.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   141262 2023-04-07 00:22:50.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:22:50.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 00:22:50.000000 tencentcloud-sdk-python-cdb-3.0.868/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-07 00:22:50.000000 tencentcloud-sdk-python-cdb-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:22:51.000000 tencentcloud-sdk-python-cdb-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   485265 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   141262 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.869/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13048,17 +13048,17 @@
         :type WaitSwitch: int
         :param BackupZone: 备库 2 的可用区信息，默认为空，升级主实例时可指定该参数，升级只读实例或者灾备实例时指定该参数无意义。
         :type BackupZone: str
         :param InstanceRole: 实例类型，默认为 master，支持值包括：master - 表示主实例，dr - 表示灾备实例，ro - 表示只读实例。
         :type InstanceRole: str
         :param DeviceType: 实例隔离类型。支持值包括： "UNIVERSAL" - 通用型实例， "EXCLUSIVE" - 独享型实例， "BASIC" - 基础版实例。
         :type DeviceType: str
-        :param Cpu: 升级后的实例cpu核数， 如果不传将根据 Memory 指定的内存值自动填充对应的cpu值。
+        :param Cpu: 升级后的实例cpu核数，如果不传将根据 Memory 指定的内存值自动填充对应的cpu值。
         :type Cpu: int
-        :param FastUpgrade: 是否极速变配。0-普通升级，1-极速变配,，2 极速优先。选择极速变配会根据资源状况校验是否可以进行极速变配，满足条件则进行极速变配，不满足条件会返回报错信息。
+        :param FastUpgrade: 是否极速变配。0-普通升级，1-极速变配，2 极速优先。选择极速变配会根据资源状况校验是否可以进行极速变配，满足条件则进行极速变配，不满足条件会返回报错信息。
         :type FastUpgrade: int
         :param MaxDelayTime: 延迟阈值。取值范围1~10，默认值为10。
         :type MaxDelayTime: int
         :param CrossCluster: 是否跨区迁移。0-普通迁移，1-跨区迁移，默认值为0。该值为1时支持变更实例主节点可用区。
         :type CrossCluster: int
         :param ZoneId: 主节点可用区，该值仅在跨区迁移时生效。仅支持同地域下的可用区进行迁移。
         :type ZoneId: str
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.868/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.868/README.rst` & `tencentcloud-sdk-python-cdb-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.868/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.868/setup.py` & `tencentcloud-sdk-python-cdb-3.0.869/setup.py`

 * *Files identical despite different names*

