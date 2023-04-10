# Comparing `tmp/yunxiao-0.1.2.tar.gz` & `tmp/yunxiao-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.1.2.tar", last modified: Sun Apr  9 22:33:56 2023, max compression
+gzip compressed data, was "yunxiao-0.1.3.tar", last modified: Mon Apr 10 14:57:27 2023, max compression
```

## Comparing `yunxiao-0.1.2.tar` & `yunxiao-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 22:33:56.228223 yunxiao-0.1.2/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      940 2023-04-09 22:33:56.227223 yunxiao-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-04-09 14:22:29.000000 yunxiao-0.1.2/README.md
--rw-rw-rw-   0        0        0      587 2023-04-09 22:28:55.000000 yunxiao-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 22:33:56.228223 yunxiao-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-09 22:33:56.220691 yunxiao-0.1.2/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.2/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    18051 2023-04-09 22:32:12.000000 yunxiao-0.1.2/yunxiao/app.py
--rw-rw-rw-   0        0        0     5790 2023-04-09 22:33:00.000000 yunxiao-0.1.2/yunxiao/web.py
--rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.2/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:33:56.226220 yunxiao-0.1.2/yunxiao.egg-info/
--rw-rw-rw-   0        0        0      940 2023-04-09 22:33:56.000000 yunxiao-0.1.2/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-09 22:33:56.000000 yunxiao-0.1.2/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 22:33:56.000000 yunxiao-0.1.2/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-09 22:33:56.000000 yunxiao-0.1.2/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 22:33:56.000000 yunxiao-0.1.2/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 14:57:27.007994 yunxiao-0.1.3/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     7017 2023-04-10 14:57:27.007307 yunxiao-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6530 2023-04-10 01:07:24.000000 yunxiao-0.1.3/README.md
+-rw-rw-rw-   0        0        0      587 2023-04-10 14:57:10.000000 yunxiao-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:57:27.007994 yunxiao-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 14:57:26.982764 yunxiao-0.1.3/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.3/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    18394 2023-04-10 14:56:31.000000 yunxiao-0.1.3/yunxiao/app.py
+-rw-rw-rw-   0        0        0     8911 2023-04-10 01:47:54.000000 yunxiao-0.1.3/yunxiao/web.py
+-rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.3/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:57:27.005746 yunxiao-0.1.3/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     7017 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.1.2/LICENSE` & `yunxiao-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.2/pyproject.toml` & `yunxiao-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.1.2"
+version = "0.1.3"
 description = "An API tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
```

### Comparing `yunxiao-0.1.2/yunxiao/app.py` & `yunxiao-0.1.3/yunxiao/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from .yunxiao import AppOAuth, UsedTime
 
 
 class App(AppOAuth):
-    def __init__(self, userphone: str, password: str, campus: list):
+    def __init__(self, userphone: str, password: str, campus: list = None):
+        """
+        初始化，输入用户账号密码，以及要操作的校区。
+        :param userphone: 账号
+        :param password: 密码
+        :param campus: 校区
+        """
         super().__init__(userphone, password)
         if campus is None:
             self.campus = []
         else:
             self.campus = campus
 
         self.reportpath = "https://yunxiao.xiaogj.com/api/cs-report/report/"
@@ -336,29 +342,33 @@
             url=self.edupath + "courseStudent/findStudentAttendCourse",
             json=data
         ).json()
 
     # [工作台][学员][就读课程][出入班记录]
     def operation_record_list(
             self,
-            studentid: str = None,
+            studentid: int = None,
             curriculum_id: int = None,
-            campus_ids_index: int = 0
+            campus_ids_index: int = None,
+            campus_id: int = None
     ):
         """
         [工作台][学员][就读课程][出入班记录]
+        :param campus_id:
         :param campus_ids_index: 实例中选择的校区列表索引，必须从中列表中选择一个。
         :param studentid:
         :param curriculum_id:
         :return:
         """
+        if campus_ids_index:
+            campus_id = self.campus[campus_ids_index]
         data = {
             "_t_": UsedTime.stamp,
-            "campusId": self.campus[campus_ids_index],
-            "studentId": studentid,
+            "campusId": campus_id,
+            "studentId": str(studentid),
             "curriculumId": curriculum_id
         }
         return self.session.post(
             url=self.edupath + "student/findOperationRecordList",
             json=data
         ).json()
```

### Comparing `yunxiao-0.1.2/yunxiao/web.py` & `yunxiao-0.1.3/yunxiao/web.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .yunxiao import WebOAuth, UsedTime
+from yunxiao import WebOAuth, UsedTime
 
 
 class Web(WebOAuth):
-    def __init__(self, userphone: str, password: str, campus: list):
+    def __init__(self, userphone: str, password: str, campus: list =None):
         super().__init__(userphone, password)
         if campus is None:
             self.campus = []
         else:
             self.campus = campus
         self.reportpath = "https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/"
         self.edupath = "https://yunxiao.xiaogj.com/api/cs-pc-edu/"
@@ -160,7 +160,109 @@
                 "studentIds": [],
                 "reserve": 0,
                 "displayCompletedClass": False,
                 "courseStatusList": [],
                 "page": {"pageNum": page_num, "pageSize": page_size}
             }
         ).json()
+
+    def find_payment_list(
+            self,
+            pay_start_date: str = UsedTime.weekstrat,
+            pay_end_date: str = UsedTime.weekend,
+            order_status: int = 1,
+            page_num: int = 1,
+            page_size: int = 9999
+    ):
+        """
+        收入明细报表。
+        :param pay_start_date: 支付起始时间
+        :param pay_end_date: 支付结束时间
+        :param order_status: 订单状态 1>已付款
+        :param page_num: 页数
+        :param page_size: 每页项目数
+        :return:
+        """
+        return self.session.post(
+            url=self.reportpath + "findPaymentList",
+            json={
+                "_t_": UsedTime.stamp,
+                "campusIds": self.campus,
+                "payType": "",
+                "payStartTime": pay_start_date,
+                "payEndTime": pay_end_date,
+                "orderStatus": order_status,
+                "orderStartTime": "",
+                "orderEndTime": "",
+                "btransactionId": "",
+                "aymentAccountCustomIds": [],
+                "confirmStatusList": [],
+                "revenueType": "",
+                "page": {"pageNum": page_num, "pageSize": page_size}
+            }
+        ).json()
+
+    def find_receipt(
+            self,
+            order_id: int,
+            payment_group_id: int
+    ):
+        """
+        收据。
+        :param order_id: 订单 ID
+        :param payment_group_id: 支付 ID
+        :return:
+        """
+        return self.session.get(
+            url="https://yunxiao.xiaogj.com/api/cs-pc-edu/public/receipt/findReceipt",
+            params={
+                "orderId": order_id,
+                "paymentGroupId": payment_group_id,
+                "_t_": UsedTime.stamp
+            }
+        ).json()
+
+    def snap_info_by_payment_group_id(
+            self,
+            order_id: int,
+            payment_group_id: int
+    ):
+        """
+        收据。
+        :param order_id: 订单 ID
+        :param payment_group_id: 支付 ID
+        :return:
+        """
+        return self.session.get(
+            url="https://yunxiao.xiaogj.com/api/cs-pc-edu/public/receipt/snapInfoByPaymentGroupId",
+            params={
+                "orderId": order_id,
+                "paymentGroupId": payment_group_id,
+                "_t_": UsedTime.stamp
+            }
+        ).json()
+
+    def receipt(
+            self,
+            order_id: int,
+            payment_group_id: int
+    ):
+        """
+        收据。
+        :param order_id: 订单 ID
+        :param payment_group_id: 支付 ID
+        :return: Respose 数据
+        """
+        return self.session.get(
+            url="https://yunxiao.xiaogj.com/web/teacher/#/receipt",
+            params={
+                "orderId": order_id,
+                "paymentGroupId": payment_group_id
+            }
+        )
+
+
+if __name__ == "__main__":
+    import sys
+    web = Web(sys.argv[1], sys.argv[2])
+    res = web.receipt(5744750, 5744752)
+    print(res.content.decode("utf-8"))
```

### Comparing `yunxiao-0.1.2/yunxiao/yunxiao.py` & `yunxiao-0.1.3/yunxiao/yunxiao.py`

 * *Files identical despite different names*

