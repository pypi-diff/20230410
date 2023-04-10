# Comparing `tmp/tencentcloud-sdk-python-mongodb-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-mongodb-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.868.tar", last modified: Fri Apr  7 00:45:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.869.tar", last modified: Mon Apr 10 03:09:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mongodb-3.0.868.tar` & `tencentcloud-sdk-python-mongodb-3.0.869.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20180408/
--rw-r--r--   0 root         (0) root         (0)    46677 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13571 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20180408/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20190725/
--rw-r--r--   0 root         (0) root         (0)   146939 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20190725/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20190725/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35460 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20190725/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)     7304 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20190725/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud_sdk_python_mongodb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:45:40.000000 tencentcloud-sdk-python-mongodb-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    46677 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13571 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/
+-rw-r--r--   0 root         (0) root         (0)   147320 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35476 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)     7304 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.869/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20180408/models.py` & `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20180408/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20180408/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20190725/models.py` & `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 class CreateAccountUserRequest(AbstractModel):
     """CreateAccountUser请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例 ID。
+        :param InstanceId: 实例 ID。例如：cmgo-p8vn****。请登录 [MongoDB 控制台](https://console.cloud.tencent.com/mongodb)在实例列表复制实例 ID。
         :type InstanceId: str
         :param UserName: 新账号名称。其格式要求如下：<ul><li>字符范围[1,32]。</li><li>可输入[A,Z]、[a,z]、[1,9]范围的字符以及下划线“_”与短划线“-”。</li></ul>
         :type UserName: str
         :param Password: 新账号密码。密码复杂度要求如下：<ul><li>字符长度范围[8,32]。</li><li>至少包含字母、数字和特殊字符（叹号“!”、at"@"、井号“#”、百分号“%”、插入符“^”、星号“*”、小括号“()”、下划线“_”）中的两种。</li></ul>
         :type Password: str
         :param MongoUserPassword: mongouser 账号对应的密码。mongouser 为系统默认账号，即为创建实例时，设置的密码。
         :type MongoUserPassword: str
@@ -941,15 +941,15 @@
 class DescribeAccountUsersRequest(AbstractModel):
     """DescribeAccountUsers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID。
+        :param InstanceId: 指定待获取账号的实例ID。例如：cmgo-p8vn****。请登录 [MongoDB 控制台](https://console.cloud.tencent.com/mongodb)在实例列表复制实例 ID。
         :type InstanceId: str
         """
         self.InstanceId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
@@ -1122,19 +1122,20 @@
 class DescribeClientConnectionsRequest(AbstractModel):
     """DescribeClientConnections请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID，格式如：cmgo-p8vnipr5。与云数据库控制台页面中显示的实例ID相同
+        :param InstanceId: 指定待查询的实例ID，例如：cmgo-p8vn****。请登录 [MongoDB 控制台](https://console.cloud.tencent.com/mongodb)在实例列表复制实例 ID。
+
         :type InstanceId: str
-        :param Limit: 单次请求返回的数量，最小值为1，最大值为1000，默认值为1000。
+        :param Limit: 单次请求返回的数量。最小值为1，最大值为1000，默认值为1000。
         :type Limit: int
-        :param Offset: 偏移量，默认值为0。
+        :param Offset: 偏移量，默认值为0。Offset=Limit*(页码-1)。
         :type Offset: int
         """
         self.InstanceId = None
         self.Limit = None
         self.Offset = None
 
 
@@ -1154,15 +1155,15 @@
 class DescribeClientConnectionsResponse(AbstractModel):
     """DescribeClientConnections返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Clients: 客户端连接信息，包括客户端IP和对应IP的连接数量。
+        :param Clients: 客户端连接信息，包括客户端 IP 和对应 IP 的连接数量。
         :type Clients: list of ClientConnection
         :param TotalCount: 满足条件的记录总条数，可用于分页查询。
         :type TotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Clients = None
@@ -1489,15 +1490,15 @@
 class DescribeDBInstancesRequest(AbstractModel):
     """DescribeDBInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceIds: 实例ID列表。例如：cmgo-p8vn****。请登录 [MongoDB 控制台](https://console.cloud.tencent.com/mongodb)在实例列表复制实例 ID。
+        :param InstanceIds: 实例 ID 列表。例如：cmgo-p8vn****。请登录 [MongoDB 控制台](https://console.cloud.tencent.com/mongodb)在实例列表复制实例 ID。
         :type InstanceIds: list of str
         :param InstanceType: 实例类型。取值范围如下：<ul><li>0：所有实例。</li><li>1：正式实例。</li><li>2：临时实例。</li><li>3：只读实例。</li><li>-1：正式实例、只读、灾备实例。</li></ul>
         :type InstanceType: int
         :param ClusterType: 集群类型，取值范围如下：<ul><li>0：副本集实例。</li><li>1：分片实例。</li><li>-1：所有实例。</li></ul>
         :type ClusterType: int
         :param Status: 实例状态，取值范围如下所示：<ul><li>0：待初始化。</li><li>1：流程执行中。</li><li>2：实例有效。</li><li>-2：已隔离（包年包月实例）。</li><li>-3：已隔离（按量计费实例）。</li></ul>
         :type Status: list of int
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20190725/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/mongodb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateAccountUser(self, request):
-        """本接口(CreateAccountUser)用于创建mongodb实例账号。
+        """本接口（CreateAccountUser）用于自定义实例访问账号。
 
         :param request: Request instance for CreateAccountUser.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.CreateAccountUserRequest`
         :rtype: :class:`tencentcloud.mongodb.v20190725.models.CreateAccountUserResponse`
 
         """
         try:
@@ -161,15 +161,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeAccountUsers(self, request):
-        """本接口(DescribeAccountUsers)用于获取当前实例的全部账号。
+        """本接口（DescribeAccountUsers）用于获取当前实例的全部账号。
 
         :param request: Request instance for DescribeAccountUsers.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeAccountUsersRequest`
         :rtype: :class:`tencentcloud.mongodb.v20190725.models.DescribeAccountUsersResponse`
 
         """
         try:
@@ -230,15 +230,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeClientConnections(self, request):
-        """本接口(DescribeClientConnections)用于查询实例客户端连接信息，包括连接IP和连接数量。
+        """本接口（DescribeClientConnections）用于查询实例客户端连接信息，包括连接 IP 和连接数量。
 
         :param request: Request instance for DescribeClientConnections.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeClientConnectionsRequest`
         :rtype: :class:`tencentcloud.mongodb.v20190725.models.DescribeClientConnectionsResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud/mongodb/v20190725/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/README.rst` & `tencentcloud-sdk-python-mongodb-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.868/setup.py` & `tencentcloud-sdk-python-mongodb-3.0.869/setup.py`

 * *Files identical despite different names*

