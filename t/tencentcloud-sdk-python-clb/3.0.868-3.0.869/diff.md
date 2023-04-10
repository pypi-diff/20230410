# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.868.tar", last modified: Fri Apr  7 00:24:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.869.tar", last modified: Mon Apr 10 02:58:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.868.tar` & `tencentcloud-sdk-python-clb-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)   326602 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89842 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/v20180317/clb_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud_sdk_python_clb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:24:31.000000 tencentcloud-sdk-python-clb-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)   328056 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89842 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/v20180317/clb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:58:30.000000 tencentcloud-sdk-python-clb-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-clb-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.869/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1486,14 +1486,16 @@
         :type DeregisterTargetRst: bool
         :param MultiCertInfo: 证书信息，支持同时传入不同算法类型的多本服务端证书；此参数仅适用于未开启SNI特性的HTTPS监听器。此参数和Certificate不能同时传入。
         :type MultiCertInfo: :class:`tencentcloud.clb.v20180317.models.MultiCertInfo`
         :param MaxConn: 监听器最大连接数，只有TCP/UDP/TCP_SSL/QUIC监听器支持，不传或者传-1表示监听器维度不限速。
         :type MaxConn: int
         :param MaxCps: 监听器最大新增连接数，只有TCP/UDP/TCP_SSL/QUIC监听器支持，不传或者传-1表示监听器维度不限速。
         :type MaxCps: int
+        :param IdleConnectTimeout: 空闲连接超时时间，此参数仅适用于TCP监听器，单位：秒。默认值：900，取值范围：共享型实例和独占型实例支持：300～900，性能容量型实例支持：300~2000。如需设置超过2000s，请通过 [工单申请](https://console.cloud.tencent.com/workorder/category),最大可设置到3600s。
+        :type IdleConnectTimeout: int
         """
         self.LoadBalancerId = None
         self.Ports = None
         self.Protocol = None
         self.ListenerNames = None
         self.HealthCheck = None
         self.Certificate = None
@@ -1504,14 +1506,15 @@
         self.SessionType = None
         self.KeepaliveEnable = None
         self.EndPort = None
         self.DeregisterTargetRst = None
         self.MultiCertInfo = None
         self.MaxConn = None
         self.MaxCps = None
+        self.IdleConnectTimeout = None
 
 
     def _deserialize(self, params):
         self.LoadBalancerId = params.get("LoadBalancerId")
         self.Ports = params.get("Ports")
         self.Protocol = params.get("Protocol")
         self.ListenerNames = params.get("ListenerNames")
@@ -1530,14 +1533,15 @@
         self.EndPort = params.get("EndPort")
         self.DeregisterTargetRst = params.get("DeregisterTargetRst")
         if params.get("MultiCertInfo") is not None:
             self.MultiCertInfo = MultiCertInfo()
             self.MultiCertInfo._deserialize(params.get("MultiCertInfo"))
         self.MaxConn = params.get("MaxConn")
         self.MaxCps = params.get("MaxCps")
+        self.IdleConnectTimeout = params.get("IdleConnectTimeout")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5039,14 +5043,17 @@
         :type TargetGroupList: list of BasicTargetGroupInfo
         :param MaxConn: 监听器最大连接数，-1表示监听器维度不限速。
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxConn: int
         :param MaxCps: 监听器最大新增连接数，-1表示监听器维度不限速。
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxCps: int
+        :param IdleConnectTimeout: 空闲连接超时时间，仅支持TCP监听器。默认值:900；共享型实例和独占型实例取值范围：300～900，性能容量型实例取值范围:300～1980。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IdleConnectTimeout: int
         """
         self.ListenerId = None
         self.Protocol = None
         self.Port = None
         self.Certificate = None
         self.HealthCheck = None
         self.Scheduler = None
@@ -5062,14 +5069,15 @@
         self.KeepaliveEnable = None
         self.Toa = None
         self.DeregisterTargetRst = None
         self.AttrFlags = None
         self.TargetGroupList = None
         self.MaxConn = None
         self.MaxCps = None
+        self.IdleConnectTimeout = None
 
 
     def _deserialize(self, params):
         self.ListenerId = params.get("ListenerId")
         self.Protocol = params.get("Protocol")
         self.Port = params.get("Port")
         if params.get("Certificate") is not None:
@@ -5103,14 +5111,15 @@
             self.TargetGroupList = []
             for item in params.get("TargetGroupList"):
                 obj = BasicTargetGroupInfo()
                 obj._deserialize(item)
                 self.TargetGroupList.append(obj)
         self.MaxConn = params.get("MaxConn")
         self.MaxCps = params.get("MaxCps")
+        self.IdleConnectTimeout = params.get("IdleConnectTimeout")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6310,14 +6319,16 @@
         :type SessionType: str
         :param MultiCertInfo: 证书信息，支持同时传入不同算法类型的多本服务端证书；此参数仅适用于未开启SNI特性的HTTPS监听器。此参数和Certificate不能同时传入。
         :type MultiCertInfo: :class:`tencentcloud.clb.v20180317.models.MultiCertInfo`
         :param MaxConn: 监听器粒度并发连接数上限，当前仅性能容量型实例且仅TCP/UDP/TCP_SSL/QUIC监听器支持。取值范围：1-实例规格并发连接上限，其中-1表示关闭监听器粒度并发连接数限速。
         :type MaxConn: int
         :param MaxCps: 监听器粒度新建连接数上限，当前仅性能容量型实例且仅TCP/UDP/TCP_SSL/QUIC监听器支持。取值范围：1-实例规格新建连接上限，其中-1表示关闭监听器粒度新建连接数限速。
         :type MaxCps: int
+        :param IdleConnectTimeout: 空闲连接超时时间，此参数仅适用于TCP监听器，单位：秒。默认值：900，取值范围：共享型实例和独占型实例支持：300～900，性能容量型实例支持：300~2000。如需设置超过2000s，请通过 [工单申请](https://console.cloud.tencent.com/workorder/category),最大可设置到3600s。
+        :type IdleConnectTimeout: int
         """
         self.LoadBalancerId = None
         self.ListenerId = None
         self.ListenerName = None
         self.SessionExpireTime = None
         self.HealthCheck = None
         self.Certificate = None
@@ -6326,14 +6337,15 @@
         self.TargetType = None
         self.KeepaliveEnable = None
         self.DeregisterTargetRst = None
         self.SessionType = None
         self.MultiCertInfo = None
         self.MaxConn = None
         self.MaxCps = None
+        self.IdleConnectTimeout = None
 
 
     def _deserialize(self, params):
         self.LoadBalancerId = params.get("LoadBalancerId")
         self.ListenerId = params.get("ListenerId")
         self.ListenerName = params.get("ListenerName")
         self.SessionExpireTime = params.get("SessionExpireTime")
@@ -6350,14 +6362,15 @@
         self.DeregisterTargetRst = params.get("DeregisterTargetRst")
         self.SessionType = params.get("SessionType")
         if params.get("MultiCertInfo") is not None:
             self.MultiCertInfo = MultiCertInfo()
             self.MultiCertInfo._deserialize(params.get("MultiCertInfo"))
         self.MaxConn = params.get("MaxConn")
         self.MaxCps = params.get("MaxCps")
+        self.IdleConnectTimeout = params.get("IdleConnectTimeout")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.868/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.869/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.868/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.869/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.868/README.rst` & `tencentcloud-sdk-python-clb-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.868/setup.py` & `tencentcloud-sdk-python-clb-3.0.869/setup.py`

 * *Files identical despite different names*

