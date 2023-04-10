# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.868.tar", last modified: Fri Apr  7 00:46:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.869.tar", last modified: Mon Apr 10 03:10:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.868.tar` & `tencentcloud-sdk-python-ocr-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   398815 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   103160 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:46:50.000000 tencentcloud-sdk-python-ocr-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   406294 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   104266 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.869/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2669,14 +2669,43 @@
 
 
     def _deserialize(self, params):
         self.TaskState = params.get("TaskState")
         self.RequestId = params.get("RequestId")
 
 
+class GroupInfo(AbstractModel):
+    """组在图中的序号
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Groups: 每一行的元素
+        :type Groups: list of LineInfo
+        """
+        self.Groups = None
+
+
+    def _deserialize(self, params):
+        if params.get("Groups") is not None:
+            self.Groups = []
+            for item in params.get("Groups"):
+                obj = LineInfo()
+                obj._deserialize(item)
+                self.Groups.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class HKIDCardOCRRequest(AbstractModel):
     """HKIDCardOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3467,14 +3496,72 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ItemInfo(AbstractModel):
+    """智能结构化元素组
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Key: key信息组
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Key: :class:`tencentcloud.ocr.v20181119.models.Key`
+        :param Value: Value信息组
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Value: :class:`tencentcloud.ocr.v20181119.models.Value`
+        """
+        self.Key = None
+        self.Value = None
+
+
+    def _deserialize(self, params):
+        if params.get("Key") is not None:
+            self.Key = Key()
+            self.Key._deserialize(params.get("Key"))
+        if params.get("Value") is not None:
+            self.Value = Value()
+            self.Value._deserialize(params.get("Value"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class Key(AbstractModel):
+    """key信息组
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AutoName: 自动识别的字段名称
+        :type AutoName: str
+        """
+        self.AutoName = None
+
+
+    def _deserialize(self, params):
+        self.AutoName = params.get("AutoName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class LicensePlateInfo(AbstractModel):
     """全部车牌信息
 
     """
 
     def __init__(self):
         r"""
@@ -3584,14 +3671,43 @@
             for item in params.get("LicensePlateInfos"):
                 obj = LicensePlateInfo()
                 obj._deserialize(item)
                 self.LicensePlateInfos.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class LineInfo(AbstractModel):
+    """按行输出，行序号
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Lines: 每行的一个元素
+        :type Lines: list of ItemInfo
+        """
+        self.Lines = None
+
+
+    def _deserialize(self, params):
+        if params.get("Lines") is not None:
+            self.Lines = []
+            for item in params.get("Lines"):
+                obj = ItemInfo()
+                obj._deserialize(item)
+                self.Lines.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class MLIDCardOCRRequest(AbstractModel):
     """MLIDCardOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6927,14 +7043,94 @@
             for item in params.get("StructuralItems"):
                 obj = StructuralItem()
                 obj._deserialize(item)
                 self.StructuralItems.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class SmartStructuralOCRV2Request(AbstractModel):
+    """SmartStructuralOCRV2请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ImageUrl: 图片的 Url 地址。
+支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
+支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。
+图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
+非腾讯云存储的 Url 速度和稳定性可能受一定影响。
+        :type ImageUrl: str
+        :param ImageBase64: 图片的 Base64 值。
+支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
+支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
+图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
+        :type ImageBase64: str
+        :param IsPdf: 是否开启PDF识别，默认值为false，开启后可同时支持图片和PDF的识别。
+        :type IsPdf: bool
+        :param PdfPageNumber: 需要识别的PDF页面的对应页码，仅支持PDF单页识别，当上传文件为PDF且IsPdf参数值为true时有效，默认值为1。
+        :type PdfPageNumber: int
+        :param ItemNames: 自定义结构化功能需返回的字段名称，例：
+若客户只想返回姓名、性别两个字段的识别结果，则输入
+ItemNames=["姓名","性别"]
+        :type ItemNames: list of str
+        """
+        self.ImageUrl = None
+        self.ImageBase64 = None
+        self.IsPdf = None
+        self.PdfPageNumber = None
+        self.ItemNames = None
+
+
+    def _deserialize(self, params):
+        self.ImageUrl = params.get("ImageUrl")
+        self.ImageBase64 = params.get("ImageBase64")
+        self.IsPdf = params.get("IsPdf")
+        self.PdfPageNumber = params.get("PdfPageNumber")
+        self.ItemNames = params.get("ItemNames")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SmartStructuralOCRV2Response(AbstractModel):
+    """SmartStructuralOCRV2返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Angle: 图片旋转角度(角度制)，文本的水平方向
+为 0；顺时针为正，逆时针为负
+        :type Angle: float
+        :param StructuralList: 配置结构化文本信息
+        :type StructuralList: list of GroupInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Angle = None
+        self.StructuralList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Angle = params.get("Angle")
+        if params.get("StructuralList") is not None:
+            self.StructuralList = []
+            for item in params.get("StructuralList"):
+                obj = GroupInfo()
+                obj._deserialize(item)
+                self.StructuralList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class StructuralItem(AbstractModel):
     """智能结构化识别
 
     """
 
     def __init__(self):
         r"""
@@ -8477,14 +8673,45 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class Value(AbstractModel):
+    """value信息组
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AutoContent: 自动识别的字段内容
+        :type AutoContent: str
+        :param Coord: 四点坐标
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Coord: :class:`tencentcloud.ocr.v20181119.models.Polygon`
+        """
+        self.AutoContent = None
+        self.Coord = None
+
+
+    def _deserialize(self, params):
+        self.AutoContent = params.get("AutoContent")
+        if params.get("Coord") is not None:
+            self.Coord = Polygon()
+            self.Coord._deserialize(params.get("Coord"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class VatInvoice(AbstractModel):
     """增值税发票信息
 
     """
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1820,14 +1820,39 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def SmartStructuralOCRV2(self, request):
+        """本接口支持识别并提取各类证照、票据、表单、合同等结构化场景的字段信息。无需任何配置，灵活高效。适用于各类结构化信息录入场景。
+
+        默认接口请求频率限制：10次/秒。
+
+        :param request: Request instance for SmartStructuralOCRV2.
+        :type request: :class:`tencentcloud.ocr.v20181119.models.SmartStructuralOCRV2Request`
+        :rtype: :class:`tencentcloud.ocr.v20181119.models.SmartStructuralOCRV2Response`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SmartStructuralOCRV2", params, headers=headers)
+            response = json.loads(body)
+            model = models.SmartStructuralOCRV2Response()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def TableOCR(self, request):
         """<b>此接口为表格识别的旧版本服务，不再进行服务升级，建议您使用识别能力更强、服务性能更优的<a href="https://cloud.tencent.com/document/product/866/49525">新版表格识别</a>。</b>
 
         本接口支持图片内表格文档的检测和识别，返回每个单元格的文字内容，支持将识别结果保存为 Excel 格式。
 
         默认接口请求频率限制：10次/秒。
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.868/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.868/README.rst` & `tencentcloud-sdk-python-ocr-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.868/setup.py` & `tencentcloud-sdk-python-ocr-3.0.869/setup.py`

 * *Files identical despite different names*

