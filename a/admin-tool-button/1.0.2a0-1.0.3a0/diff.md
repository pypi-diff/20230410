# Comparing `tmp/admin_tool_button-1.0.2a0.tar.gz` & `tmp/admin_tool_button-1.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admin_tool_button-1.0.2a0.tar", last modified: Mon Apr 10 11:09:44 2023, max compression
+gzip compressed data, was "admin_tool_button-1.0.3a0.tar", last modified: Mon Apr 10 11:26:42 2023, max compression
```

## Comparing `admin_tool_button-1.0.2a0.tar` & `admin_tool_button-1.0.3a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/
--rw-rw-r--   0 bram      (1000) bram      (1000)      935 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/PKG-INFO
--rw-rw-r--   0 bram      (1000) bram      (1000)      585 2023-04-10 11:05:04.000000 admin_tool_button-1.0.2a0/README.md
-drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:09:44.235140 admin_tool_button-1.0.2a0/admin_tool_button/
--rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-08 20:06:04.000000 admin_tool_button-1.0.2a0/admin_tool_button/__init__.py
-drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/admin_tool_button/contrib/
--rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-08 20:06:04.000000 admin_tool_button-1.0.2a0/admin_tool_button/contrib/__init__.py
--rw-rw-r--   0 bram      (1000) bram      (1000)     1488 2023-04-09 16:46:09.000000 admin_tool_button-1.0.2a0/admin_tool_button/contrib/admin.py
--rw-rw-r--   0 bram      (1000) bram      (1000)      266 2023-04-08 20:06:04.000000 admin_tool_button-1.0.2a0/admin_tool_button/version.py
-drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/
--rw-rw-r--   0 bram      (1000) bram      (1000)      935 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/PKG-INFO
--rw-rw-r--   0 bram      (1000) bram      (1000)      394 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/SOURCES.txt
--rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/dependency_links.txt
--rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-09 17:15:25.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/not-zip-safe
--rw-rw-r--   0 bram      (1000) bram      (1000)       51 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/requires.txt
--rw-rw-r--   0 bram      (1000) bram      (1000)       18 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/top_level.txt
--rw-rw-r--   0 bram      (1000) bram      (1000)       38 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/setup.cfg
--rw-rw-r--   0 bram      (1000) bram      (1000)      811 2023-04-10 11:09:02.000000 admin_tool_button-1.0.2a0/setup.py
+drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:26:42.124137 admin_tool_button-1.0.3a0/
+-rw-rw-r--   0 bram      (1000) bram      (1000)      935 2023-04-10 11:26:42.124137 admin_tool_button-1.0.3a0/PKG-INFO
+-rw-rw-r--   0 bram      (1000) bram      (1000)      585 2023-04-10 11:05:04.000000 admin_tool_button-1.0.3a0/README.md
+drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:26:42.124137 admin_tool_button-1.0.3a0/admin_tool_button/
+-rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-08 20:06:04.000000 admin_tool_button-1.0.3a0/admin_tool_button/__init__.py
+drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:26:42.124137 admin_tool_button-1.0.3a0/admin_tool_button/contrib/
+-rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-08 20:06:04.000000 admin_tool_button-1.0.3a0/admin_tool_button/contrib/__init__.py
+-rw-rw-r--   0 bram      (1000) bram      (1000)     1488 2023-04-09 16:46:09.000000 admin_tool_button-1.0.3a0/admin_tool_button/contrib/admin.py
+-rw-rw-r--   0 bram      (1000) bram      (1000)      266 2023-04-08 20:06:04.000000 admin_tool_button-1.0.3a0/admin_tool_button/version.py
+drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:26:42.124137 admin_tool_button-1.0.3a0/admin_tool_button.egg-info/
+-rw-rw-r--   0 bram      (1000) bram      (1000)      935 2023-04-10 11:26:42.000000 admin_tool_button-1.0.3a0/admin_tool_button.egg-info/PKG-INFO
+-rw-rw-r--   0 bram      (1000) bram      (1000)      394 2023-04-10 11:26:42.000000 admin_tool_button-1.0.3a0/admin_tool_button.egg-info/SOURCES.txt
+-rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-10 11:26:42.000000 admin_tool_button-1.0.3a0/admin_tool_button.egg-info/dependency_links.txt
+-rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-09 17:15:25.000000 admin_tool_button-1.0.3a0/admin_tool_button.egg-info/not-zip-safe
+-rw-rw-r--   0 bram      (1000) bram      (1000)       51 2023-04-10 11:26:42.000000 admin_tool_button-1.0.3a0/admin_tool_button.egg-info/requires.txt
+-rw-rw-r--   0 bram      (1000) bram      (1000)       18 2023-04-10 11:26:42.000000 admin_tool_button-1.0.3a0/admin_tool_button.egg-info/top_level.txt
+-rw-rw-r--   0 bram      (1000) bram      (1000)       38 2023-04-10 11:26:42.124137 admin_tool_button-1.0.3a0/setup.cfg
+-rw-rw-r--   0 bram      (1000) bram      (1000)      842 2023-04-10 11:25:42.000000 admin_tool_button-1.0.3a0/setup.py
```

### Comparing `admin_tool_button-1.0.2a0/PKG-INFO` & `admin_tool_button-1.0.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admin_tool_button
-Version: 1.0.2a0
+Version: 1.0.3a0
 Summary: Extra tool buttons for Django admin
 Home-page: https://github.com/bboogaard/admin_tool_button
 Author: Bram Boogaard
 Author-email: padawan@hetnet.nl
 License: MIT License
 Keywords: Django Admin
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `admin_tool_button-1.0.2a0/README.md` & `admin_tool_button-1.0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `admin_tool_button-1.0.2a0/admin_tool_button/contrib/admin.py` & `admin_tool_button-1.0.3a0/admin_tool_button/contrib/admin.py`

 * *Files identical despite different names*

### Comparing `admin_tool_button-1.0.2a0/admin_tool_button.egg-info/PKG-INFO` & `admin_tool_button-1.0.3a0/admin_tool_button.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admin-tool-button
-Version: 1.0.2a0
+Version: 1.0.3a0
 Summary: Extra tool buttons for Django admin
 Home-page: https://github.com/bboogaard/admin_tool_button
 Author: Bram Boogaard
 Author-email: padawan@hetnet.nl
 License: MIT License
 Keywords: Django Admin
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `admin_tool_button-1.0.2a0/setup.py` & `admin_tool_button-1.0.3a0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 from admin_tool_button.version import Version
 
 
 setup(name='admin_tool_button',
-     version=Version('1.0.2-alpha').number,
+     version=Version('1.0.3-alpha').number,
      description='Extra tool buttons for Django admin',
      long_description=open('README.md').read().strip(),
      long_description_content_type="text/markdown",
      author='Bram Boogaard',
      author_email='padawan@hetnet.nl',
      url='https://github.com/bboogaard/admin_tool_button',
-     packages=find_packages(include=['admin_tool_button', 'admin_tool_button.contrib']),
+     packages=find_packages(include=['admin_tool_button', 'admin_tool_button.contrib', 'admin_tool_button.templates']),
      install_requires=[
          'pytest',
          'pytest-cov',
          'pytest-django==4.5.2',
          'django==3.2'
      ],
      license='MIT License',
```

