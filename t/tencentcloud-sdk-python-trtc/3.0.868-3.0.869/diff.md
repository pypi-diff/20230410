# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.868.tar", last modified: Fri Apr  7 01:04:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.869.tar", last modified: Mon Apr 10 03:17:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.868.tar` & `tencentcloud-sdk-python-trtc-3.0.869.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)   198636 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58128 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9679 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 01:04:03.000000 tencentcloud-sdk-python-trtc-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)   198735 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58128 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.869/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4043,27 +4043,27 @@
         :type SdkAppId: int
         :param RoomId: 主房间信息RoomId，转推的TRTC房间所对应的RoomId。
         :type RoomId: str
         :param RoomIdType: 主房间信息RoomType，必须和转推的房间所对应的RoomId类型相同，0为整形房间号，1为字符串房间号。
         :type RoomIdType: int
         :param AgentParams: 转推服务加入TRTC房间的机器人参数。
         :type AgentParams: :class:`tencentcloud.trtc.v20190722.models.AgentParams`
-        :param WithTranscoding: 是否转码，0表示无需转码，1表示需要转码。是否收取转码费是由WithTranscoding参数决定的，WithTranscoding为0，表示旁路转推，不会收取转码费用，WithTranscoding为1，表示混流转推，会收取转吗费用。
+        :param WithTranscoding: 是否转码，0表示无需转码，1表示需要转码。是否收取转码费是由WithTranscoding参数决定的，WithTranscoding为0，表示旁路转推，不会收取转码费用，WithTranscoding为1，表示混流转推，会收取转码费用。
         :type WithTranscoding: int
         :param AudioParams: 转推流的音频编码参数。由于音频是必转码的（不会收取转码费用），所以启动任务的时候，必须填写。
         :type AudioParams: :class:`tencentcloud.trtc.v20190722.models.McuAudioParams`
         :param VideoParams: 转推流的视频编码参数，不填表示纯音频转推。
         :type VideoParams: :class:`tencentcloud.trtc.v20190722.models.McuVideoParams`
         :param SingleSubscribeParams: 需要单流旁路转推的用户上行参数，单流旁路转推时，WithTranscoding需要设置为0。
         :type SingleSubscribeParams: :class:`tencentcloud.trtc.v20190722.models.SingleSubscribeParams`
         :param PublishCdnParams: 转推的CDN参数。和回推房间参数必须要有一个。
         :type PublishCdnParams: list of McuPublishCdnParam
         :param SeiParams: 混流SEI参数
         :type SeiParams: :class:`tencentcloud.trtc.v20190722.models.McuSeiParams`
-        :param FeedBackRoomParams: 回推房间信息，和转推CDN参数必须要有一个。
+        :param FeedBackRoomParams: 回推房间信息，和转推CDN参数必须要有一个。注：回推房间需使用特殊的SDK版本，如您有需求，请联系腾讯云技术支持。
         :type FeedBackRoomParams: list of McuFeedBackRoomParams
         """
         self.SdkAppId = None
         self.RoomId = None
         self.RoomIdType = None
         self.AgentParams = None
         self.WithTranscoding = None
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.868/README.rst` & `tencentcloud-sdk-python-trtc-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.868/setup.py` & `tencentcloud-sdk-python-trtc-3.0.869/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.868/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

