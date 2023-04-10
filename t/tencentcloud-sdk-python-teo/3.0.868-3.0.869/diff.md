# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.869.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.868.tar", last modified: Fri Apr  7 01:01:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.869.tar", last modified: Mon Apr 10 03:15:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.868.tar` & `tencentcloud-sdk-python-teo-3.0.869.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)   468214 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7631 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    87643 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)   504485 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20753 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    81864 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 01:01:25.000000 tencentcloud-sdk-python-teo-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)   468214 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    87643 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)   504971 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20753 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    81864 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.869/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4508,18 +4508,22 @@
     def __init__(self):
         r"""
         :param StartTime: 开始时间。
         :type StartTime: str
         :param EndTime: 结束时间。
         :type EndTime: str
         :param MetricNames: 查询的指标，取值有：
-<li>l7Flow_outFlux: 访问流量；</li>
+<li>l7Flow_outFlux: Edegone响应流量；</li>
+<li>l7Flow_inFlux: Edgeone请求流量；</li>
+<li>l7Flow_outBandwidth: Edegone响应带宽；</li>
+<li>l7Flow_inBandwidth: Edegone请求带宽；</li>
+<li>l7Flow_hit_outFlux: 缓存命中流量；</li>
 <li>l7Flow_request: 访问请求数；</li>
-<li>l7Flow_outBandwidth: 访问带宽；</li>
-<li>l7Flow_hit_outFlux: 缓存命中流量。</li>
+<li>l7Flow_flux: 访问请求上行+下行流量；</li>
+<li>l7Flow_bandwidth：访问请求上行+下行带宽。</li>
         :type MetricNames: list of str
         :param ZoneIds: 站点集合。
 若不填写，默认选择全部站点，且最多只能查询近30天的数据；若填写，则可查询站点绑定套餐支持的<a href="https://cloud.tencent.com/document/product/1552/77380#edgeone-.E5.A5.97.E9.A4.90">数据分析最大查询范围</a>。
         :type ZoneIds: list of str
         :param Domains: 查询的域名集合，不填默认查询所有子域名。
         :type Domains: list of str
         :param Protocol: 查询的协议类型，取值有：
@@ -5215,17 +5219,21 @@
     def __init__(self):
         r"""
         :param StartTime: 开始时间。
         :type StartTime: str
         :param EndTime: 结束时间。
         :type EndTime: str
         :param MetricNames: 指标列表，取值有:
-<li>l7Flow_outFlux: 访问流量；</li>
+<li>l7Flow_outFlux: Edgeone响应流量；</li>
+<li>l7Flow_inFlux: Edgeone请求流量；</li>
+<li>l7Flow_outBandwidth: Edgeone响应带宽；</li>
+<li>l7Flow_inBandwidth：Edgeone请求带宽；</li>
 <li>l7Flow_request: 访问请求数；</li>
-<li>l7Flow_outBandwidth: 访问带宽。</li>
+<li>l7Flow_flux: 访问请求上行+下行流量；</li>
+<li>l7Flow_bandwidth：访问请求上行+下行带宽。</li>
         :type MetricNames: list of str
         :param ZoneIds: 站点集合。
 若不填写，默认选择全部站点，且最多只能查询近30天的数据；若填写，则可查询站点绑定套餐支持的<a href="https://cloud.tencent.com/document/product/1552/77380#edgeone-.E5.A5.97.E9.A4.90">数据分析最大查询范围</a>。
         :type ZoneIds: list of str
         :param Interval: 查询时间粒度，取值有：
 <li>min: 1分钟；</li>
 <li>5min: 5分钟；</li>
@@ -5668,15 +5676,15 @@
 <li> l7Cache_outFlux_domain：host/域名；</li>
 <li> l7Cache_outFlux_url：url地址；</li>
 <li> l7Cache_outFlux_resourceType：资源类型；</li>
 <li> l7Cache_outFlux_statusCode：状态码。</li>
         :type MetricName: str
         :param ZoneIds: 站点id集合，不填默认选择全部站点。
         :type ZoneIds: list of str
-        :param Limit: 查询前多少个数据，不填默认默认为10， 表示查询前top 10的数据。
+        :param Limit: 查询前多少个数据，最大值为1000，不填默认默认为10， 表示查询前top 10的数据。
         :type Limit: int
         :param Filters: 过滤条件，详细的过滤条件如下：
 <li>domain<br>   按照【<strong>子域名</strong>】进行过滤，子域名形如： test.example.com。<br>   类型：String<br>   必选：否</li>
 <li>url<br>   按照【<strong>URL</strong>】进行过滤，此参数只支持30天的时间范围，URL形如：/content。<br>   类型：String<br>   必选：否</li>
 <li>resourceType<br>   按照【<strong>资源类型</strong>】进行过滤，此参数只支持30天的时间范围，资源类型形如：jpg，png。<br>   类型：String<br>   必选：否</li>
 <li>cacheType<br>   按照【<strong>缓存类型</strong>】进行过滤。<br>   类型：String<br>   必选：否<br>   可选项：<br>   hit：命中缓存；<br>   dynamic：资源不可缓存；<br>   miss：未命中缓存。</li>
 <li>statusCode<br>   按照【<strong>状态码</strong>】进行过滤，此参数只支持30天的时间范围。<br>   类型：String<br>   必选：否<br>   可选项：<br>   1XX：1xx类型的状态码；<br>   100：100状态码；<br>   101：101状态码；<br>   102：102状态码；<br>   2XX：2xx类型的状态码；<br>   200：200状态码；<br>   201：201状态码；<br>   202：202状态码；<br>   203：203状态码；<br>   204：204状态码；<br>   100：100状态码；<br>   206：206状态码；<br>   207：207状态码；<br>   3XX：3xx类型的状态码；<br>   300：300状态码；<br>   301：301状态码；<br>   302：302状态码；<br>   303：303状态码；<br>   304：304状态码；<br>   305：305状态码；<br>   307：307状态码；<br>   4XX：4xx类型的状态码；<br>   400：400状态码；<br>   401：401状态码；<br>   402：402状态码；<br>   403：403状态码；<br>   404：404状态码；<br>   405：405状态码；<br>   406：406状态码；<br>   407：407状态码；<br>   408：408状态码；<br>   409：409状态码；<br>   410：410状态码；<br>   411：411状态码；<br>   412：412状态码；<br>   412：413状态码；<br>   414：414状态码；<br>   415：415状态码；<br>   416：416状态码；<br>   417：417状态码；<br>   422：422状态码；<br>   423：423状态码；<br>   424：424状态码；<br>   426：426状态码；<br>   451：451状态码；<br>   5XX：5xx类型的状态码；<br>   500：500状态码；<br>   501：501状态码；<br>   502：502状态码；<br>   503：503状态码；<br>   504：504状态码；<br>   505：505状态码；<br>   506：506状态码；<br>   507：507状态码；<br>   510：510状态码；<br>   514：514状态码；<br>   544：544状态码。</li>
```

### Comparing `tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.868/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.868/README.rst` & `tencentcloud-sdk-python-teo-3.0.869/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.868/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.868
+Version: 3.0.869
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.868/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.868/setup.py` & `tencentcloud-sdk-python-teo-3.0.869/setup.py`

 * *Files identical despite different names*

