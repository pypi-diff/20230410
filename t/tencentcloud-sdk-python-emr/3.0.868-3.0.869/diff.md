# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.868.tar", last modified: Fri Apr  7 00:37:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.869.tar", last modified: Mon Apr 10 03:05:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.868.tar` & `tencentcloud-sdk-python-emr-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:37:49.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    25510 2023-04-07 00:37:49.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)   251822 2023-04-07 00:37:49.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:37:49.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13479 2023-04-07 00:37:49.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 00:37:49.000000 tencentcloud-sdk-python-emr-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-07 00:37:49.000000 tencentcloud-sdk-python-emr-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:37:50.000000 tencentcloud-sdk-python-emr-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)    27330 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)   258513 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13479 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:05:05.000000 tencentcloud-sdk-python-emr-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-emr-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.869/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/v20190103/emr_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -576,14 +576,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def StartStopServiceOrMonitor(self, request):
+        """用于启动或停止监控或服务
+
+        :param request: Request instance for StartStopServiceOrMonitor.
+        :type request: :class:`tencentcloud.emr.v20190103.models.StartStopServiceOrMonitorRequest`
+        :rtype: :class:`tencentcloud.emr.v20190103.models.StartStopServiceOrMonitorResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StartStopServiceOrMonitor", params, headers=headers)
+            response = json.loads(body)
+            model = models.StartStopServiceOrMonitorResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def SyncPodState(self, request):
         """EMR同步TKE中POD状态
 
         :param request: Request instance for SyncPodState.
         :type request: :class:`tencentcloud.emr.v20190103.models.SyncPodStateRequest`
         :rtype: :class:`tencentcloud.emr.v20190103.models.SyncPodStateResponse`
 
@@ -597,14 +620,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def TerminateClusterNodes(self, request):
+        """销毁集群节点
+
+        :param request: Request instance for TerminateClusterNodes.
+        :type request: :class:`tencentcloud.emr.v20190103.models.TerminateClusterNodesRequest`
+        :rtype: :class:`tencentcloud.emr.v20190103.models.TerminateClusterNodesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("TerminateClusterNodes", params, headers=headers)
+            response = json.loads(body)
+            model = models.TerminateClusterNodesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def TerminateInstance(self, request):
         """销毁EMR实例。此接口仅支持弹性MapReduce正式计费版本。
 
         :param request: Request instance for TerminateInstance.
         :type request: :class:`tencentcloud.emr.v20190103.models.TerminateInstanceRequest`
```

### Comparing `tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/v20190103/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -760,14 +760,44 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ComponentBasicRestartInfo(AbstractModel):
+    """操作的进程范围
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ComponentName: 进程名，必填，如NameNode
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ComponentName: str
+        :param IpList: 操作的IP列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpList: list of str
+        """
+        self.ComponentName = None
+        self.IpList = None
+
+
+    def _deserialize(self, params):
+        self.ComponentName = params.get("ComponentName")
+        self.IpList = params.get("IpList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Configuration(AbstractModel):
     """自定义配置参数
 
     """
 
     def __init__(self):
         r"""
@@ -4252,14 +4282,44 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class OpScope(AbstractModel):
+    """操作范围
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ServiceInfoList: 操作范围，要操作的服务信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ServiceInfoList: list of ServiceBasicRestartInfo
+        """
+        self.ServiceInfoList = None
+
+
+    def _deserialize(self, params):
+        if params.get("ServiceInfoList") is not None:
+            self.ServiceInfoList = []
+            for item in params.get("ServiceInfoList"):
+                obj = ServiceBasicRestartInfo()
+                obj._deserialize(item)
+                self.ServiceInfoList.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class OutterResource(AbstractModel):
     """资源详情
 
     """
 
     def __init__(self):
         r"""
@@ -6015,14 +6075,47 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ServiceBasicRestartInfo(AbstractModel):
+    """操作的服务范围
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ServiceName: 服务名，必填，如HDFS
+        :type ServiceName: str
+        :param ComponentInfoList: 如果没传，则表示所有进程
+        :type ComponentInfoList: list of ComponentBasicRestartInfo
+        """
+        self.ServiceName = None
+        self.ComponentInfoList = None
+
+
+    def _deserialize(self, params):
+        self.ServiceName = params.get("ServiceName")
+        if params.get("ComponentInfoList") is not None:
+            self.ComponentInfoList = []
+            for item in params.get("ComponentInfoList"):
+                obj = ComponentBasicRestartInfo()
+                obj._deserialize(item)
+                self.ComponentInfoList.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ShortNodeInfo(AbstractModel):
     """节点信息
 
     """
 
     def __init__(self):
         r"""
@@ -6073,14 +6166,70 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class StartStopServiceOrMonitorRequest(AbstractModel):
+    """StartStopServiceOrMonitor请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 集群ID
+        :type InstanceId: str
+        :param OpType: 操作类型，当前支持
+<li>StartService：启动服务</li>
+<li>StopService：停止服务</li>
+<li>StartMonitor：退出维护</li>
+<li>StopMonitor：进入维护</li>
+
+        :type OpType: str
+        :param OpScope: 操作范围
+        :type OpScope: :class:`tencentcloud.emr.v20190103.models.OpScope`
+        """
+        self.InstanceId = None
+        self.OpType = None
+        self.OpScope = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.OpType = params.get("OpType")
+        if params.get("OpScope") is not None:
+            self.OpScope = OpScope()
+            self.OpScope._deserialize(params.get("OpScope"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class StartStopServiceOrMonitorResponse(AbstractModel):
+    """StartStopServiceOrMonitor返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class Step(AbstractModel):
     """执行步骤
 
     """
 
     def __init__(self):
         r"""
@@ -6214,14 +6363,81 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class TerminateClusterNodesRequest(AbstractModel):
+    """TerminateClusterNodes请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        :param CvmInstanceIds: 销毁资源列表
+        :type CvmInstanceIds: list of str
+        :param NodeFlag: 销毁节点类型取值范围：
+  <li>MASTER</li>
+  <li>TASK</li>
+  <li>CORE</li>
+  <li>ROUTER</li>
+        :type NodeFlag: str
+        :param GraceDownFlag: 优雅缩容开关
+  <li>true:开启</li>
+  <li>false:不开启</li>
+        :type GraceDownFlag: bool
+        :param GraceDownTime: 优雅缩容等待时间,时间范围60到1800  单位秒
+        :type GraceDownTime: int
+        """
+        self.InstanceId = None
+        self.CvmInstanceIds = None
+        self.NodeFlag = None
+        self.GraceDownFlag = None
+        self.GraceDownTime = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.CvmInstanceIds = params.get("CvmInstanceIds")
+        self.NodeFlag = params.get("NodeFlag")
+        self.GraceDownFlag = params.get("GraceDownFlag")
+        self.GraceDownTime = params.get("GraceDownTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TerminateClusterNodesResponse(AbstractModel):
+    """TerminateClusterNodes返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 缩容流程ID。
+        :type FlowId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.RequestId = params.get("RequestId")
+
+
 class TerminateInstanceRequest(AbstractModel):
     """TerminateInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-emr-3.0.868/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.869/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.868/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.869/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.868/README.rst` & `tencentcloud-sdk-python-emr-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.868/setup.py` & `tencentcloud-sdk-python-emr-3.0.869/setup.py`

 * *Files identical despite different names*

