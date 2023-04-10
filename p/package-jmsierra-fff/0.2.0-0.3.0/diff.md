# Comparing `tmp/package_jmsierra_fff-0.2.0.tar.gz` & `tmp/package_jmsierra_fff-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package_jmsierra_fff-0.2.0.tar", max compression
+gzip compressed data, was "package_jmsierra_fff-0.3.0.tar", max compression
```

## Comparing `package_jmsierra_fff-0.2.0.tar` & `package_jmsierra_fff-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-04-10 16:30:29.551334 package_jmsierra_fff-0.2.0/LICENSE
--rw-r--r--   0        0        0     1787 2023-04-10 16:20:45.319526 package_jmsierra_fff-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-10 16:19:02.267005 package_jmsierra_fff-0.2.0/package_jmsierra_fff/__init__.py
--rw-r--r--   0        0        0       29 2023-04-10 16:33:29.310919 package_jmsierra_fff-0.2.0/package_jmsierra_fff/dividir.py
--rw-r--r--   0        0        0       29 2023-04-10 16:33:29.306661 package_jmsierra_fff-0.2.0/package_jmsierra_fff/multiplicar.py
--rw-r--r--   0        0        0       29 2023-04-10 16:32:55.367219 package_jmsierra_fff-0.2.0/package_jmsierra_fff/restar.py
--rw-r--r--   0        0        0       29 2023-04-10 16:32:55.360174 package_jmsierra_fff-0.2.0/package_jmsierra_fff/sumar.py
--rw-r--r--   0        0        0      915 2023-04-10 17:04:02.555496 package_jmsierra_fff-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 package_jmsierra_fff-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-10 16:30:29.551334 package_jmsierra_fff-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1787 2023-04-10 16:20:45.319526 package_jmsierra_fff-0.3.0/README.md
+-rw-r--r--   0        0        0      171 2023-04-10 17:13:19.926450 package_jmsierra_fff-0.3.0/package_jmsierra_fff/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-10 17:13:19.922376 package_jmsierra_fff-0.3.0/package_jmsierra_fff/_dividir.py
+-rw-r--r--   0        0        0       30 2023-04-10 17:13:19.929953 package_jmsierra_fff-0.3.0/package_jmsierra_fff/_multiplicar.py
+-rw-r--r--   0        0        0       30 2023-04-10 17:13:19.933591 package_jmsierra_fff-0.3.0/package_jmsierra_fff/_restar.py
+-rw-r--r--   0        0        0       30 2023-04-10 17:13:19.937963 package_jmsierra_fff-0.3.0/package_jmsierra_fff/_sumar.py
+-rw-r--r--   0        0        0      914 2023-04-10 17:14:48.550386 package_jmsierra_fff-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 package_jmsierra_fff-0.3.0/PKG-INFO
```

### Comparing `package_jmsierra_fff-0.2.0/LICENSE` & `package_jmsierra_fff-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `package_jmsierra_fff-0.2.0/README.md` & `package_jmsierra_fff-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `package_jmsierra_fff-0.2.0/pyproject.toml` & `package_jmsierra_fff-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 [tool.poetry]
 name = "package-jmsierra-fff"
 license = "MIT License"
-version = "0.2.0"
+version = "0.3.0"
 description = "Es un proyecto de prueba"
 authors = ["Mauricio Sierra"]
 maintainers = ["Developers <mauricio@gmail.com>"]
 readme = "README.md"
 packages = [{include = "package_jmsierra_fff"}]
+classifiers = [
+    'Development Status :: 5 - Production/Stable',
+    'Intended Audience :: Science/Research',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: BSD License',
+    'Programming Language :: C',
+    'Programming Language :: Python', ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.24.2"
 pandas = "^2.0.0"
 requests = "^2.28.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
-classifiers = [
-    'Development Status :: 5 - Production/Stable',
-    'Intended Audience :: Science/Research',
-    'Intended Audience :: Developers',
-    'License :: OSI Approved :: BSD License',
-    'Programming Language :: C',
-    'Programming Language :: Python',
-]
-
 [project.urls]
 homepage = "https://numpy.org"
 documentation = "https://numpy.org/doc/"
 source = "https://github.com/mauriciosierrav/ETL_API_smn_mexico"
 download = ""
 tracker = ""
```

### Comparing `package_jmsierra_fff-0.2.0/PKG-INFO` & `package_jmsierra_fff-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: package-jmsierra-fff
-Version: 0.2.0
+Version: 0.3.0
 Summary: Es un proyecto de prueba
 License: MIT
 Author: Mauricio Sierra
 Maintainer: Developers
 Maintainer-email: mauricio@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
```

