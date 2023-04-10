# Comparing `tmp/django-ipghrms-notification-1.0.tar.gz` & `tmp/django-ipghrms-notification-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-notification-1.0.tar", last modified: Mon Mar 27 14:58:58 2023, max compression
+gzip compressed data, was "django-ipghrms-notification-1.1.tar", last modified: Mon Apr 10 06:03:45 2023, max compression
```

## Comparing `django-ipghrms-notification-1.0.tar` & `django-ipghrms-notification-1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.282540 django-ipghrms-notification-1.0/
--rw-rw-rw-   0        0        0     1072 2023-03-27 14:58:28.000000 django-ipghrms-notification-1.0/LICENSE
--rw-rw-rw-   0        0        0      164 2023-03-27 14:27:27.000000 django-ipghrms-notification-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      987 2023-03-27 14:58:58.282540 django-ipghrms-notification-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-03-27 14:28:14.000000 django-ipghrms-notification-1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.199916 django-ipghrms-notification-1.0/django_ipghrms_notification.egg-info/
--rw-rw-rw-   0        0        0      987 2023-03-27 14:58:58.000000 django-ipghrms-notification-1.0/django_ipghrms_notification.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1361 2023-03-27 14:58:58.000000 django-ipghrms-notification-1.0/django_ipghrms_notification.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 14:58:58.000000 django-ipghrms-notification-1.0/django_ipghrms_notification.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-27 14:58:58.000000 django-ipghrms-notification-1.0/django_ipghrms_notification.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.226803 django-ipghrms-notification-1.0/notification/
--rw-rw-rw-   0        0        0        0 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.0/notification/__init__.py
--rw-rw-rw-   0        0        0       66 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.0/notification/admin.py
--rw-rw-rw-   0        0        0       56 2023-01-09 23:46:45.000000 django-ipghrms-notification-1.0/notification/api_urls.py
--rw-rw-rw-   0        0        0      162 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.0/notification/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.228001 django-ipghrms-notification-1.0/notification/migrations/
--rw-rw-rw-   0        0        0        0 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.0/notification/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.229747 django-ipghrms-notification-1.0/notification/migrations/__pycache__/
--rw-rw-rw-   0        0        0      150 2023-01-09 13:24:16.000000 django-ipghrms-notification-1.0/notification/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0       60 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.0/notification/models.py
--rw-rw-rw-   0        0        0     1869 2023-01-22 08:17:24.000000 django-ipghrms-notification-1.0/notification/notif_urls.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.165848 django-ipghrms-notification-1.0/notification/templates/
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.168352 django-ipghrms-notification-1.0/notification/templates/notification/
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.231298 django-ipghrms-notification-1.0/notification/templates/notification/dep/
--rw-rw-rw-   0        0        0     2428 2023-03-15 09:59:30.000000 django-ipghrms-notification-1.0/notification/templates/notification/dep/leave.html
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.233009 django-ipghrms-notification-1.0/notification/templates/notification/div/
--rw-rw-rw-   0        0        0     2797 2023-03-15 10:00:15.000000 django-ipghrms-notification-1.0/notification/templates/notification/div/leave.html
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.254727 django-ipghrms-notification-1.0/notification/templates/notification/hr/
--rw-rw-rw-   0        0        0     3195 2023-01-23 17:40:48.000000 django-ipghrms-notification-1.0/notification/templates/notification/hr/birthday.html
--rw-rw-rw-   0        0        0     2742 2023-01-23 17:23:04.000000 django-ipghrms-notification-1.0/notification/templates/notification/hr/contract.html
--rw-rw-rw-   0        0        0     2083 2023-01-23 17:41:08.000000 django-ipghrms-notification-1.0/notification/templates/notification/hr/evaluation.html
--rw-rw-rw-   0        0        0     2525 2023-03-14 14:33:51.000000 django-ipghrms-notification-1.0/notification/templates/notification/hr/leave.html
--rw-rw-rw-   0        0        0     2163 2023-01-20 02:29:45.000000 django-ipghrms-notification-1.0/notification/templates/notification/hr/leave_end.html
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.258723 django-ipghrms-notification-1.0/notification/templates/notification/pr/
--rw-rw-rw-   0        0        0     2266 2023-03-13 18:21:55.000000 django-ipghrms-notification-1.0/notification/templates/notification/pr/leave.html
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.259824 django-ipghrms-notification-1.0/notification/templates/notification/staff/
--rw-rw-rw-   0        0        0     2862 2023-01-22 09:02:07.000000 django-ipghrms-notification-1.0/notification/templates/notification/staff/leave.html
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.262782 django-ipghrms-notification-1.0/notification/templates/notification/vice/
--rw-rw-rw-   0        0        0     2786 2023-01-22 08:18:47.000000 django-ipghrms-notification-1.0/notification/templates/notification/vice/leave.html
--rw-rw-rw-   0        0        0       63 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.0/notification/tests.py
--rw-rw-rw-   0        0        0      167 2023-01-10 00:02:52.000000 django-ipghrms-notification-1.0/notification/urls.py
--rw-rw-rw-   0        0        0      301 2023-01-20 04:06:09.000000 django-ipghrms-notification-1.0/notification/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.271504 django-ipghrms-notification-1.0/notification/views/
--rw-rw-rw-   0        0        0       47 2023-01-09 15:20:35.000000 django-ipghrms-notification-1.0/notification/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:58:58.277482 django-ipghrms-notification-1.0/notification/views/__pycache__/
--rw-rw-rw-   0        0        0      189 2023-01-09 23:59:39.000000 django-ipghrms-notification-1.0/notification/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      140 2023-01-09 23:59:39.000000 django-ipghrms-notification-1.0/notification/views/__pycache__/api.cpython-310.pyc
--rw-rw-rw-   0        0        0    11193 2023-03-13 18:44:26.000000 django-ipghrms-notification-1.0/notification/views/__pycache__/notification.cpython-310.pyc
--rw-rw-rw-   0        0        0        0 2023-01-09 15:19:55.000000 django-ipghrms-notification-1.0/notification/views/api.py
--rw-rw-rw-   0        0        0    17195 2023-03-13 18:44:23.000000 django-ipghrms-notification-1.0/notification/views/notification.py
--rw-rw-rw-   0        0        0       66 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.0/notification/views.py
--rw-rw-rw-   0        0        0      519 2023-03-27 14:58:58.284851 django-ipghrms-notification-1.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-notification-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.701527 django-ipghrms-notification-1.1/
+-rw-rw-rw-   0        0        0     1072 2023-03-27 14:58:28.000000 django-ipghrms-notification-1.1/LICENSE
+-rw-rw-rw-   0        0        0      164 2023-03-27 14:27:27.000000 django-ipghrms-notification-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      987 2023-04-10 06:03:45.701527 django-ipghrms-notification-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2023-03-27 14:28:14.000000 django-ipghrms-notification-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.467804 django-ipghrms-notification-1.1/django_ipghrms_notification.egg-info/
+-rw-rw-rw-   0        0        0      987 2023-04-10 06:03:45.000000 django-ipghrms-notification-1.1/django_ipghrms_notification.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1361 2023-04-10 06:03:45.000000 django-ipghrms-notification-1.1/django_ipghrms_notification.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 06:03:45.000000 django-ipghrms-notification-1.1/django_ipghrms_notification.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 06:03:45.000000 django-ipghrms-notification-1.1/django_ipghrms_notification.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.526380 django-ipghrms-notification-1.1/notification/
+-rw-rw-rw-   0        0        0        0 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.1/notification/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.1/notification/admin.py
+-rw-rw-rw-   0        0        0       56 2023-01-09 23:46:45.000000 django-ipghrms-notification-1.1/notification/api_urls.py
+-rw-rw-rw-   0        0        0      162 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.1/notification/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.526380 django-ipghrms-notification-1.1/notification/migrations/
+-rw-rw-rw-   0        0        0        0 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.1/notification/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.526380 django-ipghrms-notification-1.1/notification/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      150 2023-01-09 13:24:16.000000 django-ipghrms-notification-1.1/notification/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0       60 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.1/notification/models.py
+-rw-rw-rw-   0        0        0     1869 2023-01-22 08:17:24.000000 django-ipghrms-notification-1.1/notification/notif_urls.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.378384 django-ipghrms-notification-1.1/notification/templates/
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.385584 django-ipghrms-notification-1.1/notification/templates/notification/
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.552521 django-ipghrms-notification-1.1/notification/templates/notification/dep/
+-rw-rw-rw-   0        0        0     2428 2023-03-15 09:59:30.000000 django-ipghrms-notification-1.1/notification/templates/notification/dep/leave.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.561794 django-ipghrms-notification-1.1/notification/templates/notification/div/
+-rw-rw-rw-   0        0        0     2797 2023-03-15 10:00:15.000000 django-ipghrms-notification-1.1/notification/templates/notification/div/leave.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.615378 django-ipghrms-notification-1.1/notification/templates/notification/hr/
+-rw-rw-rw-   0        0        0     2641 2023-04-10 02:58:02.000000 django-ipghrms-notification-1.1/notification/templates/notification/hr/birthday.html
+-rw-rw-rw-   0        0        0     3104 2023-04-10 02:58:09.000000 django-ipghrms-notification-1.1/notification/templates/notification/hr/contract.html
+-rw-rw-rw-   0        0        0     6223 2023-04-10 05:02:25.000000 django-ipghrms-notification-1.1/notification/templates/notification/hr/evaluation.html
+-rw-rw-rw-   0        0        0     2758 2023-04-10 02:58:35.000000 django-ipghrms-notification-1.1/notification/templates/notification/hr/leave.html
+-rw-rw-rw-   0        0        0     2421 2023-04-10 02:58:25.000000 django-ipghrms-notification-1.1/notification/templates/notification/hr/leave_end.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.628437 django-ipghrms-notification-1.1/notification/templates/notification/pr/
+-rw-rw-rw-   0        0        0     2266 2023-03-13 18:21:55.000000 django-ipghrms-notification-1.1/notification/templates/notification/pr/leave.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.638528 django-ipghrms-notification-1.1/notification/templates/notification/staff/
+-rw-rw-rw-   0        0        0     2862 2023-01-22 09:02:07.000000 django-ipghrms-notification-1.1/notification/templates/notification/staff/leave.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.646763 django-ipghrms-notification-1.1/notification/templates/notification/vice/
+-rw-rw-rw-   0        0        0     2786 2023-01-22 08:18:47.000000 django-ipghrms-notification-1.1/notification/templates/notification/vice/leave.html
+-rw-rw-rw-   0        0        0       63 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.1/notification/tests.py
+-rw-rw-rw-   0        0        0      167 2023-01-10 00:02:52.000000 django-ipghrms-notification-1.1/notification/urls.py
+-rw-rw-rw-   0        0        0      301 2023-01-20 04:06:09.000000 django-ipghrms-notification-1.1/notification/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.663318 django-ipghrms-notification-1.1/notification/views/
+-rw-rw-rw-   0        0        0       47 2023-01-09 15:20:35.000000 django-ipghrms-notification-1.1/notification/views/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:03:45.692934 django-ipghrms-notification-1.1/notification/views/__pycache__/
+-rw-rw-rw-   0        0        0      189 2023-01-09 23:59:39.000000 django-ipghrms-notification-1.1/notification/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      140 2023-01-09 23:59:39.000000 django-ipghrms-notification-1.1/notification/views/__pycache__/api.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11193 2023-03-13 18:44:26.000000 django-ipghrms-notification-1.1/notification/views/__pycache__/notification.cpython-310.pyc
+-rw-rw-rw-   0        0        0        0 2023-01-09 15:19:55.000000 django-ipghrms-notification-1.1/notification/views/api.py
+-rw-rw-rw-   0        0        0    17391 2023-04-10 02:57:47.000000 django-ipghrms-notification-1.1/notification/views/notification.py
+-rw-rw-rw-   0        0        0       66 2023-01-09 13:23:49.000000 django-ipghrms-notification-1.1/notification/views.py
+-rw-rw-rw-   0        0        0      519 2023-04-10 06:03:45.707639 django-ipghrms-notification-1.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-notification-1.1/setup.py
```

### Comparing `django-ipghrms-notification-1.0/LICENSE` & `django-ipghrms-notification-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-notification-1.0/PKG-INFO` & `django-ipghrms-notification-1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-notification
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP NOTIFICATION
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-notification-1.0/README.rst` & `django-ipghrms-notification-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-ipghrms-notification-1.0/django_ipghrms_notification.egg-info/PKG-INFO` & `django-ipghrms-notification-1.1/django_ipghrms_notification.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-notification
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP NOTIFICATION
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-notification-1.0/django_ipghrms_notification.egg-info/SOURCES.txt` & `django-ipghrms-notification-1.1/django_ipghrms_notification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-notification-1.0/notification/notif_urls.py` & `django-ipghrms-notification-1.1/notification/notif_urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-notification-1.0/notification/templates/notification/dep/leave.html` & `django-ipghrms-notification-1.1/notification/templates/notification/dep/leave.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-notification-1.0/notification/templates/notification/div/leave.html` & `django-ipghrms-notification-1.1/notification/templates/notification/div/leave.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-notification-1.0/notification/templates/notification/hr/birthday.html` & `django-ipghrms-notification-1.1/notification/templates/notification/hr/leave.html`

 * *Files 14% similar despite different names*

```diff
@@ -7,57 +7,56 @@
 			<li class="breadcrumb-item active">{{ legend|upper }}</li>
 		</ul>
 	</div>
 </div>
 <div class="container-fluid"><br/>
     <div class="row">
         <div class="col-sm-12">
-            <div class="card shadow-lg border-info rounded">
+            <div class="card shadow-lg border-default rounded">
+                <div class="card-header border-primary">
+                    <h2>  {{legend|upper}}</h4>
+                </div>
                 <div class="card-body">
-                    <div class="row">
-                        <div class="col-sm-12">
-                            <div class="card shadow-md border-default rounded">
-                                <div class="card-body">
-                                    <h4 align="center"> <i class="fa fa-cake-candles"></i> {{legend|upper}}</h4>
-                                    <hr/>
+                    <div class="alert alert-info">
+                        <i class="fa fa-info-circle"></i>
+                        Tabela refere fo sai lista <strong>Pedidu Husu Licensa</strong>
+                    </div>
+                    <table class="table table-sm table-bordered" id="example">
+                        <thead>
+                            <tr>
+                                <th>Nu.</th>
+                                <th>Naran</th>
+                                <th>Asuntu</th>
+                                <th>Data Kria Aplikasaun</th>
+                                <th>Data Hahu</th>
+                                <th>Data Remata</th>
+                                <th>Loron</th>
+                                <th>#</th>
+                            </tr>
+                        </thead>
+                        <tbody>
+                            {% for obj in objects  %}
+                                <tr>
+                                    <td>{{forloop.counter}}</td>
+                                    <td>{{obj.employee}}</td>
+                                    <td>{{obj.description}}</td>
+                                    <td>{{obj.datetime|date:'d-M-Y, H:m A'}}</td>
+                                    <td>{{obj.start_date|date:'d-M-Y'}}</td>
+                                    <td>{{obj.end_date|date:'d-M-Y'}}</td>
+                                    <td>{{obj.days}}</td>
+                                    <td>
+                                        <a href="{% url 'leave-hr-app-detail' obj.hashed %}" class="btn btn-sm btn-info">Detalha <i class="fa fa-eye"></i></a>
+                                    </td>
+                                </tr>
+                            {% endfor %}
+                        </tbody>
+                    </table>
+                </div><!--end card-body-->
+            </div><!--end card-->
 
-                                    <table class="table table-sm" id="example">
-                                        <thead>
-                                            <tr align="center">
-                                                <th>Nu.</th>
-                                                <th>ID IPG</th>
-                                                <th>Naran</th>
-                                                <th>Data Moris</th>
-                                            </tr>
-                                        </thead>
-                                        <tbody>
-                                            {% for obj in objects  %}
-                                              <tr align="center">
-                                                <td>{{forloop.counter}}</td>
-                                                
-                                                <td>{{obj.emp_id}}</td>
-                                                <td>{{obj}}</td>
-                                                <td>
-                                                    {% if obj.dob.day == today.day and obj.dob.month == today.month %}
-                                                      <i class="fa fa-star text-danger"></i>
-                                                    {% else %}
-                                                      <i class="fa fa-bell text-warning"></i>
-                                                    {% endif %}
-                                                    {{obj.dob|date:"d-m-Y"}}
-                                                </td>
-                                              </tr>
-                                            {% endfor %}
-                                        </tbody>
-                                    </table>
-                                </div><!--end card-body-->
-                            </div><!--end card-->
-                        </div><!--end col-->
-                    </div><!--end row-->
-                </div> <!--end card-body-->
-            </div> <!--end card-->
         </div> <!--end col-->
     </div> <!--end row-->
 </div>
 {% endblock %}
 {% block scripts %}
 	<script type="text/javascript">
 		$(document).ready(function() {
```

### Comparing `django-ipghrms-notification-1.0/notification/templates/notification/hr/contract.html` & `django-ipghrms-notification-1.1/notification/templates/notification/hr/contract.html`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,24 @@
 		</ul>
 	</div>
 </div>
 <div class="container-fluid"><br/>
     <div class="row">
         <div class="col-sm-12">
             <div class="card shadow-lg border-default rounded">
+                <div class="card-header border-primary">
+                    <h2>{{legend|upper}}</h2>
+                </div>
                 <div class="card-body">
-                    <h4 align="center"> <i class="fa fa-handshake"></i> {{legend|upper}}</h4>
-                    <hr/>
-
-                    <table class="table table-sm" id="example">
+                    <div class="alert alert-info">
+                        <i class="fa fa-info-circle"></i>
+                        Tabela refere fo sai lista funsionario sira ne'ebe <strong>Kontrato Remata Ona</strong>
+                        <i>ou</i> <strong>Kontrato Sei Remata Iha Tempo Oin Mai</strong>
+                    </div>
+                    <table class="table table-sm table-bordered" id="example">
                         <thead>
                             <tr>
                                 <th>Nu.</th>
                                 <th>ID IPG</th>
                                 <th>Naran</th>
                                 <th>Data Hahu</th>
                                 <th>Data Remata</th>
```

### Comparing `django-ipghrms-notification-1.0/notification/templates/notification/hr/leave.html` & `django-ipghrms-notification-1.1/notification/templates/notification/vice/leave.html`

 * *Files 9% similar despite different names*

```diff
@@ -17,35 +17,39 @@
                     <hr/>
 
                     <table class="table table-sm" id="example">
                         <thead>
                             <tr>
                                 <th>Nu.</th>
                                 <th>Naran</th>
-                                <th>Asuntu</th>
-                                <th>Data Kria Aplikasaun</th>
+                                <th>Data Pedido</th>
                                 <th>Data Hahu</th>
                                 <th>Data Remata</th>
                                 <th>Loron</th>
                                 <th>#</th>
                             </tr>
                         </thead>
                         <tbody>
                             {% for obj in objects  %}
                                 <tr>
                                     <td>{{forloop.counter}}</td>
                                     <td>{{obj.employee}}</td>
-                                    <td>{{obj.description}}</td>
-                                    <td>{{obj.datetime|date:'d-M-Y, H:m A'}}</td>
+                                    <td>{{obj.date|date:'d-M-Y'}}</td>
                                     <td>{{obj.start_date|date:'d-M-Y'}}</td>
                                     <td>{{obj.end_date|date:'d-M-Y'}}</td>
                                     <td>{{obj.days}}</td>
+                                    {% if obj.pr_send %}
                                     <td>
-                                        <a href="{% url 'leave-hr-app-detail' obj.hashed %}" class="btn btn-sm btn-info">Detalha <i class="fa fa-eye"></i></a>
+                                        <a href="{% url 'leave-c-detail'  obj.hashed %}" class="btn btn-sm btn-info">Detalha <i class="fa fa-eye"></i></a>
                                     </td>
+                                    {% else %}
+                                    <td>
+                                        <a href="{% url 'leave-c-ver-detail'  obj.hashed %}" class="btn btn-sm btn-info">Detalha <i class="fa fa-eye"></i></a>
+                                    </td>
+                                    {% endif %}
                                 </tr>
                             {% endfor %}
                         </tbody>
                     </table>
                 </div><!--end card-body-->
             </div><!--end card-->
```

### Comparing `django-ipghrms-notification-1.0/notification/templates/notification/hr/leave_end.html` & `django-ipghrms-notification-1.1/notification/templates/notification/hr/leave_end.html`

 * *Files 7% similar despite different names*

```diff
@@ -8,19 +8,23 @@
 		</ul>
 	</div>
 </div>
 <div class="container-fluid"><br/>
     <div class="row">
         <div class="col-sm-12">
             <div class="card shadow-lg border-default rounded">
+                <div class="card-header border-primary">
+                    <h2> {{legend|upper}}</h2>
+                </div>
                 <div class="card-body">
-                    <h4 align="center"> <i class="fa-solid fa-person-circle-exclamation"></i> {{legend|upper}}</h4>
-                    <hr/>
-
-                    <table class="table table-sm" id="example">
+                    <div class="alert alert-info">
+                        <i class="fa fa-info-circle"></i>
+                        Tabela refere fo sai lista funsionario sira ne'ebe <strong>Periode Licensa Remata Ona</strong>
+                    </div>
+                    <table class="table table-sm table-bordered" id="example">
                         <thead>
                             <tr>
                                 <th>Nu.</th>
                                 <th>Naran</th>
                                 <th>Data Hahu</th>
                                 <th>Data Remata</th>
                                 <th>#</th>
```

### Comparing `django-ipghrms-notification-1.0/notification/templates/notification/pr/leave.html` & `django-ipghrms-notification-1.1/notification/templates/notification/pr/leave.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-notification-1.0/notification/templates/notification/staff/leave.html` & `django-ipghrms-notification-1.1/notification/templates/notification/staff/leave.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-notification-1.0/notification/views/__pycache__/notification.cpython-310.pyc` & `django-ipghrms-notification-1.1/notification/views/__pycache__/notification.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-notification-1.0/notification/views/notification.py` & `django-ipghrms-notification-1.1/notification/views/notification.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime, timedelta
 from employee.models import Employee
 from notification.utils import is_birthday_coming
 from  django.http import JsonResponse
 from leave.models import Leave, LeaveDep
 from settings_app.user_utils import c_staff,c_unit
 from django.db.models import Q
-from perform.models  import Eval, Category, EvalYear
+from perform.models  import Eval, Category, EvalYear, ParameterA, ParameterB, EvalPlanning, EvalPreAssessment, EvalPlanningA, EvalSelf
 from leave.models import LeavePeriod, LeaveCount
 
 
 # done: Notif HR
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrNotifAllBadge(request):
@@ -46,20 +46,15 @@
             Q( Q(is_approve=True)|Q(is_reject=True, is_done=False), unit_send_pr=True, hr_confirm = False)|\
             Q(pr_notify=True,hr_confirm = False)|
             Q(pr_send=True,is_approve=True, hr_confirm = False)|
             Q(is_send_to_div=True,is_approve=True, hr_confirm=False)|
             Q(is_send_to_div=True,is_done=False, is_finish=False)|
             Q(is_approve=True, hr_confirm=False)
         ).count()
-
-    for i in cats:
-        a = Contract.objects.filter(category=i, is_active=True).all().count()
-        b = Eval.objects.filter(employee__contract__category=i, year__year=todayYear.year).all().count()
-        c = a - b
-        eval = eval + c
+    eval = Eval.objects.filter(year__is_active=True, is_finish=False).all().count()
     cont = len(d)
     birth = len(birtharr)
     dt_tot =  birth + cont + leave + eval + leave_end
     return JsonResponse({'value':dt_tot})
 
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
@@ -93,19 +88,15 @@
             Q(pr_notify=True,hr_confirm = False)|
             Q(pr_send=True,is_approve=True, hr_confirm = False)|
             Q(is_send_to_div=True,is_approve=True, hr_confirm=False)|
             Q(is_send_to_div=True,is_done=False, is_finish=False)|
             Q(is_approve=True, hr_confirm=False)
             
         ).count()
-        for i in cats:
-            a = Contract.objects.filter(category=i, is_active=True).all().count()
-            b = Eval.objects.filter(employee__contract__category=i, year__year=todayYear.year).all().count()
-            c = a - b
-            eval = eval + c
+        eval = Eval.objects.filter(year__is_active=True, is_finish=False).all().count()
     cont = len(d)
     birth = len(birtharr)
     return JsonResponse({'data1':birth, 'data2': cont, 'data3':leave, 'data4': eval, 'data5': leave_end})
 
 
 
 
@@ -164,27 +155,37 @@
     return render(request, 'notification/hr/leave.html', context)
 
 
 @login_required
 @allowed_users(allowed_roles=['hr','de','deputy'])
 def PerformList(request):
     group = request.user.groups.all()[0].name
-    todayYear = datetime.today().date()
-    year = EvalYear.objects.filter(is_active=True).last()
-    cats = Category.objects.exclude(Q(pk=1)|Q(pk=2)).order_by('name')
+    paramas = ParameterA.objects.filter().all()
+    parambs = ParameterB.objects.filter().all()
+    years = EvalYear.objects.filter().all().order_by('year')
+    employee = Employee.objects.filter(status_id=1).exclude(curempdivision__de__pk=1)
+    ayear = EvalYear.objects.filter(is_active=True).last()
     objects = []
-    for i in cats:
-        a = Contract.objects.filter(category=i, is_active=True).all().count()
-        b = Eval.objects.filter(employee__contract__category=i, year__year=todayYear.year).all().count()
-        c = a - b
-        objects.append([i,a,b,c])
+    for emp in employee:
+        evalplan = EvalPlanning.objects.filter(employee=emp, year=ayear).last()
+        evalpreass = EvalPreAssessment.objects.filter(employee=emp, year=ayear).last()
+        check_plan = EvalPlanningA.objects.filter(eval=evalplan).exists()
+        evalself = EvalSelf.objects.filter(employee=emp, year=ayear).last()
+        eval = Eval.objects.filter(employee=emp, year=ayear).last()
+        
+        if eval:
+            if eval.is_finish == False:
+                objects.append([emp,evalplan, evalpreass, check_plan, evalself, eval])
+
+
     context = {
-        'group': group, 'objects': objects,
-        'title': 'Lista Avaliasaun Seidauk Prosesa', 'legend': f'Lista Avaliasaun Seidauk Prosesa iha Tinan {todayYear.year}'
-    }
+		'group': group, 'years': years, 'paramas': paramas, 'parambs': parambs,
+		'title': 'Lista Avaliasaun', 'legend': 'Lista Avaliasaun', \
+		'objects': objects, 'ayear':ayear.year
+	}
     return render(request, 'notification/hr/evaluation.html', context)
 
 
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def LeaveEndList(request):
     objects = []
```

### Comparing `django-ipghrms-notification-1.0/setup.cfg` & `django-ipghrms-notification-1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6970 6768 726d   = django-ipghrm
 00000020: 732d 6e6f 7469 6669 6361 7469 6f6e 0d0a  s-notification..
-00000030: 7665 7273 696f 6e20 3d20 312e 300d 0a61  version = 1.0..a
+00000030: 7665 7273 696f 6e20 3d20 312e 310d 0a61  version = 1.1..a
 00000040: 7574 686f 7220 3d20 4b69 6e6f 730d 0a61  uthor = Kinos..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 696e  uthor_email = in
 00000060: 666f 406b 696e 6f73 2e74 6c0d 0a6d 6169  fo@kinos.tl..mai
 00000070: 6e74 6169 6e65 7220 3d20 6b69 6e6f 730d  ntainer = kinos.
 00000080: 0a6d 6169 6e74 6169 6e65 725f 656d 6169  .maintainer_emai
 00000090: 6c20 3d20 696e 666f 406b 696e 6f73 2e74  l = info@kinos.t
 000000a0: 6c0d 0a64 6573 6372 6970 7469 6f6e 203d  l..description =
```

