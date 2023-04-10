# Comparing `tmp/goby_sdk-1.0.1.tar.gz` & `tmp/goby_sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goby_sdk-1.0.1.tar", last modified: Tue Apr  4 07:10:39 2023, max compression
+gzip compressed data, was "goby_sdk-1.0.3.tar", last modified: Mon Apr 10 10:32:58 2023, max compression
```

## Comparing `goby_sdk-1.0.1.tar` & `goby_sdk-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 07:10:39.541163 goby_sdk-1.0.1/
--rw-rw-rw-   0        0        0      144 2023-04-04 07:10:39.540163 goby_sdk-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-04 07:10:39.510605 goby_sdk-1.0.1/goby_sdk/
-drwxrwxrwx   0        0        0        0 2023-04-04 07:10:39.524588 goby_sdk-1.0.1/goby_sdk/V1/
--rw-rw-rw-   0        0        0        0 2023-04-03 07:20:55.000000 goby_sdk-1.0.1/goby_sdk/V1/__init__.py
--rw-rw-rw-   0        0        0     4963 2023-04-04 06:42:30.000000 goby_sdk-1.0.1/goby_sdk/V1/api.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:10:39.538164 goby_sdk-1.0.1/goby_sdk/V1/lib/
--rw-rw-rw-   0        0        0        0 2023-04-03 08:10:31.000000 goby_sdk-1.0.1/goby_sdk/V1/lib/__init__.py
--rw-rw-rw-   0        0        0     3805 2023-04-04 07:08:58.000000 goby_sdk-1.0.1/goby_sdk/V1/lib/asset_page.py
--rw-rw-rw-   0        0        0     1095 2023-04-04 07:07:49.000000 goby_sdk-1.0.1/goby_sdk/V1/lib/base_page.py
--rw-rw-rw-   0        0        0     1610 2023-04-04 07:09:05.000000 goby_sdk-1.0.1/goby_sdk/V1/lib/config_page.py
--rw-rw-rw-   0        0        0     5578 2023-04-04 07:09:21.000000 goby_sdk-1.0.1/goby_sdk/V1/lib/home_page.py
--rw-rw-rw-   0        0        0     1515 2023-04-04 07:09:53.000000 goby_sdk-1.0.1/goby_sdk/V1/lib/report_page.py
--rw-rw-rw-   0        0        0     3391 2023-04-04 07:10:18.000000 goby_sdk-1.0.1/goby_sdk/V1/lib/vulnerability_management_page.py
--rw-rw-rw-   0        0        0        0 2023-04-03 07:20:26.000000 goby_sdk-1.0.1/goby_sdk/__init__.py
--rw-rw-rw-   0        0        0      121 2023-04-04 06:47:49.000000 goby_sdk-1.0.1/goby_sdk/version.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:10:39.521589 goby_sdk-1.0.1/goby_sdk.egg-info/
--rw-rw-rw-   0        0        0      144 2023-04-04 07:10:39.000000 goby_sdk-1.0.1/goby_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-04-04 07:10:39.000000 goby_sdk-1.0.1/goby_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 07:10:39.000000 goby_sdk-1.0.1/goby_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-04 07:10:39.000000 goby_sdk-1.0.1/goby_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-04 07:10:39.000000 goby_sdk-1.0.1/goby_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 07:10:39.541163 goby_sdk-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      302 2023-04-04 07:10:33.000000 goby_sdk-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:32:58.951354 goby_sdk-1.0.3/
+-rw-rw-rw-   0        0        0      187 2023-04-10 10:32:58.950353 goby_sdk-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-04-10 10:29:52.000000 goby_sdk-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 10:32:58.913356 goby_sdk-1.0.3/goby_sdk/
+drwxrwxrwx   0        0        0        0 2023-04-10 10:32:58.929360 goby_sdk-1.0.3/goby_sdk/V1/
+-rw-rw-rw-   0        0        0        0 2023-04-03 07:20:55.000000 goby_sdk-1.0.3/goby_sdk/V1/__init__.py
+-rw-rw-rw-   0        0        0     4976 2023-04-10 03:43:42.000000 goby_sdk-1.0.3/goby_sdk/V1/api.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:32:58.946354 goby_sdk-1.0.3/goby_sdk/V1/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-03 08:10:31.000000 goby_sdk-1.0.3/goby_sdk/V1/lib/__init__.py
+-rw-rw-rw-   0        0        0     3805 2023-04-04 07:08:58.000000 goby_sdk-1.0.3/goby_sdk/V1/lib/asset_page.py
+-rw-rw-rw-   0        0        0     1095 2023-04-04 07:07:49.000000 goby_sdk-1.0.3/goby_sdk/V1/lib/base_page.py
+-rw-rw-rw-   0        0        0     1610 2023-04-04 07:09:05.000000 goby_sdk-1.0.3/goby_sdk/V1/lib/config_page.py
+-rw-rw-rw-   0        0        0     4911 2023-04-10 03:26:09.000000 goby_sdk-1.0.3/goby_sdk/V1/lib/home_page.py
+-rw-rw-rw-   0        0        0     1515 2023-04-04 07:09:53.000000 goby_sdk-1.0.3/goby_sdk/V1/lib/report_page.py
+-rw-rw-rw-   0        0        0     3391 2023-04-04 07:10:18.000000 goby_sdk-1.0.3/goby_sdk/V1/lib/vulnerability_management_page.py
+-rw-rw-rw-   0        0        0        0 2023-04-03 07:20:26.000000 goby_sdk-1.0.3/goby_sdk/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-04-10 10:30:28.000000 goby_sdk-1.0.3/goby_sdk/version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:32:58.926361 goby_sdk-1.0.3/goby_sdk.egg-info/
+-rw-rw-rw-   0        0        0      187 2023-04-10 10:32:58.000000 goby_sdk-1.0.3/goby_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-04-10 10:32:58.000000 goby_sdk-1.0.3/goby_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:32:58.000000 goby_sdk-1.0.3/goby_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-10 10:32:58.000000 goby_sdk-1.0.3/goby_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 10:32:58.000000 goby_sdk-1.0.3/goby_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 10:32:58.951354 goby_sdk-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      345 2023-04-10 10:24:50.000000 goby_sdk-1.0.3/setup.py
```

### Comparing `goby_sdk-1.0.1/goby_sdk/V1/api.py` & `goby_sdk-1.0.3/goby_sdk/V1/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,53 +59,53 @@
 
     # 获取IP详情
     def get_ip_info(self, task_id, ip):
         return self.AssetPage.get_ip_info(task_id=task_id, ip=ip)
 
     # 获取任务的Web漏洞列表
     def get_web_list(self, task_id, page=1, size=20):
-        return self.AssetPage.get_web_list(task_id=task_id,page=page,size=size)
+        return self.AssetPage.get_web_list(task_id=task_id, page=page, size=size)
 
     # 获取漏洞信息
     def get_pocs(self, task_id, query, reload_pocs=False, order_by='vul_nums', order='desc', page=1, page_size=20):
         return self.VuleManagePage.get_pocs(task_id=task_id, query=query, reload_pocs=reload_pocs, order_by=order_by,
                                             order=order, page=page, page_size=page_size)
 
     # 获取失败的POC列表
     def get_failed_pocs(self):
         return self.VuleManagePage.get_failed_pocs()
 
     # 获取任务的漏洞统计数据
-    def get_vuln_statistics(self,task_id):
+    def get_vuln_statistics(self, task_id):
         return self.VuleManagePage.get_vuln_statistics(task_id=task_id)
 
     # 获取任务的漏洞搜索结果
-    def get_vulnerability_search(self,task_id, page=1, size=20):
-        return self.VuleManagePage.get_vulnerability_search(task_id=task_id,page=page,size=size)
+    def get_vulnerability_search(self, task_id, page=1, size=20):
+        return self.VuleManagePage.get_vulnerability_search(task_id=task_id, page=page, size=size)
 
     # 获取POC信息
-    def get_poc_info(self,vul_name):
+    def get_poc_info(self, vul_name):
         return self.VuleManagePage.get_poc_info(vul_name=vul_name)
 
     # 获取指定任务下的IP段信息
     def get_ip_segment(self, task_id, type):
-        return self.ReportPage.get_ip_segment(task_id=task_id,segment_type=type)
+        return self.ReportPage.get_ip_segment(task_id=task_id, segment_type=type)
 
     # 获取任务的漏洞分析数据
     def get_vul_analysis(self, task_id):
         return self.ReportPage.get_vul_analysis(task_id=task_id)
 
     # 获取指定任务的资产标签数据
-    def get_asset_tags(self,task_id):
+    def get_asset_tags(self, task_id):
         return self.ReportPage.get_asset_tags(task_id=task_id)
 
     # 配置类：获取可用的网卡列表
     def get_list_adapters(self):
         return self.ConfigPage.get_list_adapters()
 
     # 配置类：获取系统环境信息
     def get_env_info(self):
         return self.ConfigPage.get_environment_info()
 
-    #设置系统环境信息
+    # 设置系统环境信息
     def set_env_info(self, dns_server, proxy_server):
-        return self.ConfigPage.set_environment_info(dns_server=dns_server,proxy_server=proxy_server)
+        return self.ConfigPage.set_environment_info(dns_server=dns_server, proxy_server=proxy_server)
```

### Comparing `goby_sdk-1.0.1/goby_sdk/V1/lib/asset_page.py` & `goby_sdk-1.0.3/goby_sdk/V1/lib/asset_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.1/goby_sdk/V1/lib/base_page.py` & `goby_sdk-1.0.3/goby_sdk/V1/lib/base_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.1/goby_sdk/V1/lib/config_page.py` & `goby_sdk-1.0.3/goby_sdk/V1/lib/config_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.1/goby_sdk/V1/lib/home_page.py` & `goby_sdk-1.0.3/goby_sdk/V1/lib/home_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,14 @@
 from goby_sdk.V1.lib.base_page import BasePage
 
 
 class HomePage(BasePage):
 
     def get_poc_list(self, query="vultype=2", reload_pocs=False,
                      order_by={"vul_nums": "desc", "level": "desc", "host_nums": "desc"}, page=1, size=3000):
-        """
-        获取POC列表信息
-        :param query: 查询条件，默认为"vultype=2"
-        :type query: str
-        :param reload_pocs: 是否重新加载POC，默认为False
-        :type reload_pocs: bool
-        :param order_by: 排序字段，默认为{"vul_nums": "desc", "level": "desc", "host_nums": "desc"}，可选值为"vul_nums"、"level"和"host_nums"
-        :type order_by: dict
-        :param page: 当前页码，默认为1
-        :type page: int
-        :param size: 每页显示的记录数，默认为3000
-        :type size: int
-        :return: 返回POC列表信息的JSON对象
-        :rtype: dict
-        """
         data = {
             "query": query,
             "options": {
                 "reloadPocs": reload_pocs,
                 "order": order_by,
                 "page": {
                     "page": page,
```

### Comparing `goby_sdk-1.0.1/goby_sdk/V1/lib/report_page.py` & `goby_sdk-1.0.3/goby_sdk/V1/lib/report_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.1/goby_sdk/V1/lib/vulnerability_management_page.py` & `goby_sdk-1.0.3/goby_sdk/V1/lib/vulnerability_management_page.py`

 * *Files identical despite different names*

