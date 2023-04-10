# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.868.tar", last modified: Fri Apr  7 00:25:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.869.tar", last modified: Mon Apr 10 02:59:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.868.tar` & `tencentcloud-sdk-python-cwp-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)   891318 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   249576 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)     3900 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:25:57.000000 tencentcloud-sdk-python-cwp-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)   900650 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250495 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.869/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12479,14 +12479,94 @@
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeFileTamperEventsRequest(AbstractModel):
+    """DescribeFileTamperEvents请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filters: 过滤条件。
+<li>Status - String - 是否必填：否 - 处理状态  0 -- 待处理 1 -- 已加白 2 -- 已删除 3 - 已忽略</li>
+<li>ModifyTime - String - 是否必填：否 - 最近发生时间</li>
+<li>Uuid- String - 是否必填：否 - 主机uuid查询</li>
+<li>RuleCategory- string - 是否必填：否 - 规则类别 0 系统规则 1 自定义规则</li>
+        :type Filters: list of Filters
+        :param Offset: 偏移量，默认为0。
+        :type Offset: int
+        :param Limit: 需要返回的数量，默认为10，最大值为100
+        :type Limit: int
+        :param Order: 排序方式 ASC,DESC
+        :type Order: str
+        :param By: 排序字段 CreateTime、ModifyTime
+        :type By: str
+        """
+        self.Filters = None
+        self.Offset = None
+        self.Limit = None
+        self.Order = None
+        self.By = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filters()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.Order = params.get("Order")
+        self.By = params.get("By")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeFileTamperEventsResponse(AbstractModel):
+    """DescribeFileTamperEvents返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param List: 核心文件事件列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type List: list of FileTamperEvent
+        :param TotalCount: 数据总条数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.List = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("List") is not None:
+            self.List = []
+            for item in params.get("List"):
+                obj = FileTamperEvent()
+                obj._deserialize(item)
+                self.List.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeGeneralStatRequest(AbstractModel):
     """DescribeGeneralStat请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -20278,14 +20358,188 @@
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.RequestId = params.get("RequestId")
 
 
+class FileTamperEvent(AbstractModel):
+    """核心文件监控事件
+
+    """
+
+    def __init__(self):
+        r"""
+        :param HostName: 机器名称
+        :type HostName: str
+        :param HostIp: 机器IP
+        :type HostIp: str
+        :param CreateTime: 发生时间
+        :type CreateTime: str
+        :param ModifyTime: 最近发生时间
+        :type ModifyTime: str
+        :param Id: 事件id
+        :type Id: int
+        :param Uuid: 主机uuid
+        :type Uuid: str
+        :param Quuid: cvm id
+        :type Quuid: str
+        :param Type: 事件类型/动作  0 -- 告警
+        :type Type: int
+        :param ProcessExe: 进程路径
+        :type ProcessExe: str
+        :param ProcessArgv: 进程参数
+        :type ProcessArgv: str
+        :param Target: 目标文件路径
+        :type Target: str
+        :param Status: 处理状态  0 -- 待处理 1 -- 已加白 2 -- 已删除 3 - 已忽略 4-已手动处理
+        :type Status: int
+        :param EventCount: 事件产生次数
+        :type EventCount: int
+        :param RuleId: 规则id
+        :type RuleId: int
+        :param RuleName: 规则名称
+        :type RuleName: str
+        :param Pstree: 事件详情: json格式
+        :type Pstree: str
+        :param RuleCategory: 规则类型 0系统规则 1自定义规则
+        :type RuleCategory: int
+        :param MachineStatus: 主机在线信息 ONLINE、OFFLINE
+        :type MachineStatus: str
+        :param Description: 危害描述
+        :type Description: str
+        :param Suggestion: 修护建议
+        :type Suggestion: str
+        :param PrivateIp: 内网ip
+        :type PrivateIp: str
+        :param ExePermission: 进程权限
+        :type ExePermission: str
+        :param UserName: 用户名
+        :type UserName: str
+        :param UserGroup: 用户组
+        :type UserGroup: str
+        :param ExeMd5: 进程名
+        :type ExeMd5: str
+        :param ExeSize: 进程文件大小
+        :type ExeSize: int
+        :param ExeTime: 进程执行时长
+        :type ExeTime: int
+        :param TargetSize: 目标文件大小
+        :type TargetSize: int
+        :param TargetPermission: 目标文件权限
+        :type TargetPermission: str
+        :param TargetModifyTime: 目标文件更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TargetModifyTime: str
+        :param TargetCreatTime: 目标文件创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TargetCreatTime: str
+        :param ExePid: 进程pid
+        :type ExePid: int
+        :param TargetName: 文件名称
+        :type TargetName: str
+        :param Reference: 参考链接
+        :type Reference: str
+        :param Level: 风险等级 0：无， 1: 高危， 2:中危， 3: 低危
+        :type Level: int
+        :param ExeName: 进程名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExeName: str
+        :param MachineExtraInfo:  主机额外信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MachineExtraInfo: :class:`tencentcloud.cwp.v20180228.models.MachineExtraInfo`
+        """
+        self.HostName = None
+        self.HostIp = None
+        self.CreateTime = None
+        self.ModifyTime = None
+        self.Id = None
+        self.Uuid = None
+        self.Quuid = None
+        self.Type = None
+        self.ProcessExe = None
+        self.ProcessArgv = None
+        self.Target = None
+        self.Status = None
+        self.EventCount = None
+        self.RuleId = None
+        self.RuleName = None
+        self.Pstree = None
+        self.RuleCategory = None
+        self.MachineStatus = None
+        self.Description = None
+        self.Suggestion = None
+        self.PrivateIp = None
+        self.ExePermission = None
+        self.UserName = None
+        self.UserGroup = None
+        self.ExeMd5 = None
+        self.ExeSize = None
+        self.ExeTime = None
+        self.TargetSize = None
+        self.TargetPermission = None
+        self.TargetModifyTime = None
+        self.TargetCreatTime = None
+        self.ExePid = None
+        self.TargetName = None
+        self.Reference = None
+        self.Level = None
+        self.ExeName = None
+        self.MachineExtraInfo = None
+
+
+    def _deserialize(self, params):
+        self.HostName = params.get("HostName")
+        self.HostIp = params.get("HostIp")
+        self.CreateTime = params.get("CreateTime")
+        self.ModifyTime = params.get("ModifyTime")
+        self.Id = params.get("Id")
+        self.Uuid = params.get("Uuid")
+        self.Quuid = params.get("Quuid")
+        self.Type = params.get("Type")
+        self.ProcessExe = params.get("ProcessExe")
+        self.ProcessArgv = params.get("ProcessArgv")
+        self.Target = params.get("Target")
+        self.Status = params.get("Status")
+        self.EventCount = params.get("EventCount")
+        self.RuleId = params.get("RuleId")
+        self.RuleName = params.get("RuleName")
+        self.Pstree = params.get("Pstree")
+        self.RuleCategory = params.get("RuleCategory")
+        self.MachineStatus = params.get("MachineStatus")
+        self.Description = params.get("Description")
+        self.Suggestion = params.get("Suggestion")
+        self.PrivateIp = params.get("PrivateIp")
+        self.ExePermission = params.get("ExePermission")
+        self.UserName = params.get("UserName")
+        self.UserGroup = params.get("UserGroup")
+        self.ExeMd5 = params.get("ExeMd5")
+        self.ExeSize = params.get("ExeSize")
+        self.ExeTime = params.get("ExeTime")
+        self.TargetSize = params.get("TargetSize")
+        self.TargetPermission = params.get("TargetPermission")
+        self.TargetModifyTime = params.get("TargetModifyTime")
+        self.TargetCreatTime = params.get("TargetCreatTime")
+        self.ExePid = params.get("ExePid")
+        self.TargetName = params.get("TargetName")
+        self.Reference = params.get("Reference")
+        self.Level = params.get("Level")
+        self.ExeName = params.get("ExeName")
+        if params.get("MachineExtraInfo") is not None:
+            self.MachineExtraInfo = MachineExtraInfo()
+            self.MachineExtraInfo._deserialize(params.get("MachineExtraInfo"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Filter(AbstractModel):
     """描述键值对过滤器，用于条件过滤查询。例如过滤ID、名称、状态等
 
     若存在多个Filter时，Filter间的关系为逻辑与（AND）关系。
     若同一个Filter存在多个Values，同一Filter下Values间的关系为逻辑或（OR）关系。
 
     * 最多只能有5个Filter
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2762,14 +2762,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeFileTamperEvents(self, request):
+        """核心文件监控事件列表
+
+        :param request: Request instance for DescribeFileTamperEvents.
+        :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeFileTamperEventsRequest`
+        :rtype: :class:`tencentcloud.cwp.v20180228.models.DescribeFileTamperEventsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeFileTamperEvents", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeFileTamperEventsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeGeneralStat(self, request):
         """获取主机相关统计
 
         :param request: Request instance for DescribeGeneralStat.
         :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeGeneralStatRequest`
         :rtype: :class:`tencentcloud.cwp.v20180228.models.DescribeGeneralStatResponse`
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cwp-3.0.868/README.rst` & `tencentcloud-sdk-python-cwp-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.868/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.868/setup.py` & `tencentcloud-sdk-python-cwp-3.0.869/setup.py`

 * *Files identical despite different names*

