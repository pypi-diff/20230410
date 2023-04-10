# Comparing `tmp/tencentcloud-sdk-python-monitor-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-monitor-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.868.tar", last modified: Fri Apr  7 00:45:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.869.tar", last modified: Mon Apr 10 03:09:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-monitor-3.0.868.tar` & `tencentcloud-sdk-python-monitor-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/v20180724/
--rw-r--r--   0 root         (0) root         (0)   549203 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143620 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/v20180724/monitor_client.py
--rw-r--r--   0 root         (0) root         (0)    10246 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud_sdk_python_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:45:46.000000 tencentcloud-sdk-python-monitor-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/
+-rw-r--r--   0 root         (0) root         (0)   551746 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143620 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/monitor_client.py
+-rw-r--r--   0 root         (0) root         (0)    10246 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.869/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/v20180724/models.py` & `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8125,21 +8125,25 @@
         :type ServiceMonitors: list of PrometheusConfigItem
         :param PodMonitors: PodMonitors列表以及对应targets信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type PodMonitors: list of PrometheusConfigItem
         :param RawJobs: RawJobs列表以及对应targets信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type RawJobs: list of PrometheusConfigItem
+        :param Probes: Probes列表以及对应targets信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Probes: list of PrometheusConfigItem
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Config = None
         self.ServiceMonitors = None
         self.PodMonitors = None
         self.RawJobs = None
+        self.Probes = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Config = params.get("Config")
         if params.get("ServiceMonitors") is not None:
             self.ServiceMonitors = []
@@ -8155,14 +8159,20 @@
                 self.PodMonitors.append(obj)
         if params.get("RawJobs") is not None:
             self.RawJobs = []
             for item in params.get("RawJobs"):
                 obj = PrometheusConfigItem()
                 obj._deserialize(item)
                 self.RawJobs.append(obj)
+        if params.get("Probes") is not None:
+            self.Probes = []
+            for item in params.get("Probes"):
+                obj = PrometheusConfigItem()
+                obj._deserialize(item)
+                self.Probes.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class DescribePrometheusGlobalNotificationRequest(AbstractModel):
     """DescribePrometheusGlobalNotification请求参数结构体
 
     """
@@ -12803,24 +12813,31 @@
         :param Name: 名称
         :type Name: str
         :param Config: 配置内容
         :type Config: str
         :param TemplateId: 用于出参，如果该配置来至模板，则为模板id
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateId: str
+        :param Targets: 目标数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Targets: :class:`tencentcloud.monitor.v20180724.models.Targets`
         """
         self.Name = None
         self.Config = None
         self.TemplateId = None
+        self.Targets = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Config = params.get("Config")
         self.TemplateId = params.get("TemplateId")
+        if params.get("Targets") is not None:
+            self.Targets = Targets()
+            self.Targets._deserialize(params.get("Targets"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -13336,28 +13353,43 @@
         :type TemplateId: str
         :param Content: 如果该聚合规则来至模板，则TemplateId为模板id
 注意：此字段可能返回 null，表示取不到有效值。
         :type Content: str
         :param ClusterId: 该聚合规则如果来源于用户集群crd资源定义，则ClusterId为所属集群ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type ClusterId: str
+        :param Status: 状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: int
+        :param Id: id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param Count: 规则数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Count: int
         """
         self.Name = None
         self.UpdateTime = None
         self.TemplateId = None
         self.Content = None
         self.ClusterId = None
+        self.Status = None
+        self.Id = None
+        self.Count = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.UpdateTime = params.get("UpdateTime")
         self.TemplateId = params.get("TemplateId")
         self.Content = params.get("Content")
         self.ClusterId = params.get("ClusterId")
+        self.Status = params.get("Status")
+        self.Id = params.get("Id")
+        self.Count = params.get("Count")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -14393,14 +14425,54 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class Targets(AbstractModel):
+    """抓取目标数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Total: int
+        :param Up: 在线数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Up: int
+        :param Down: 不在线数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Down: int
+        :param Unknown: 未知状态数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Unknown: int
+        """
+        self.Total = None
+        self.Up = None
+        self.Down = None
+        self.Unknown = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        self.Up = params.get("Up")
+        self.Down = params.get("Down")
+        self.Unknown = params.get("Unknown")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class TaskStepInfo(AbstractModel):
     """任务步骤信息
 
     """
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/v20180724/monitor_client.py` & `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/monitor_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/monitor/v20180724/errorcodes.py` & `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-monitor-3.0.868/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.868/README.rst` & `tencentcloud-sdk-python-monitor-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.868/setup.py` & `tencentcloud-sdk-python-monitor-3.0.869/setup.py`

 * *Files identical despite different names*

