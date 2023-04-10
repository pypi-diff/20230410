# Comparing `tmp/w32py-0.3.5.tar.gz` & `tmp/w32py-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w32py-0.3.5.tar", last modified: Thu Apr  6 11:40:23 2023, max compression
+gzip compressed data, was "w32py-0.3.6.tar", last modified: Mon Apr 10 13:03:12 2023, max compression
```

## Comparing `w32py-0.3.5.tar` & `w32py-0.3.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1928 2023-02-27 00:06:25.404193 w32py-0.3.5/.gitignore
--rw-r--r--   0        0        0     1081 2023-02-27 00:06:25.406271 w32py-0.3.5/LICENSE
--rw-r--r--   0        0        0      261 2023-02-27 00:06:25.407194 w32py-0.3.5/README.md
--rwxr-xr-x   0        0        0      156 2023-02-27 00:06:25.408194 w32py-0.3.5/lint.cmd
--rw-r--r--   0        0        0     1437 2023-04-04 22:58:25.435106 w32py-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       49 2023-04-06 11:39:08.414252 w32py-0.3.5/w32py/__init__.py
--rw-r--r--   0        0        0    13270 2023-04-04 22:58:25.440103 w32py-0.3.5/w32py/ebest.py
--rw-r--r--   0        0        0    11514 2023-04-06 11:39:08.415251 w32py-0.3.5/w32py/korea.py
--rw-r--r--   0        0        0      188 2023-02-27 00:06:25.415582 w32py-0.3.5/w32py/psutil.py
--rw-r--r--   0        0        0        0 2023-02-27 00:06:25.415582 w32py-0.3.5/w32py/py.typed
--rw-r--r--   0        0        0      921 2023-02-27 00:06:25.416774 w32py-0.3.5/w32py/win.py
--rw-r--r--   0        0        0      163 2023-02-27 00:06:25.416774 w32py-0.3.5/w32py/winauto.py
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 w32py-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1928 2023-02-27 00:06:25.404193 w32py-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1081 2023-02-27 00:06:25.406271 w32py-0.3.6/LICENSE
+-rw-r--r--   0        0        0      261 2023-02-27 00:06:25.407194 w32py-0.3.6/README.md
+-rwxr-xr-x   0        0        0      156 2023-02-27 00:06:25.408194 w32py-0.3.6/lint.cmd
+-rw-r--r--   0        0        0     1437 2023-04-04 22:58:25.435106 w32py-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-04-10 00:51:43.653238 w32py-0.3.6/w32py/__init__.py
+-rw-r--r--   0        0        0    13270 2023-04-04 22:58:25.440103 w32py-0.3.6/w32py/ebest.py
+-rw-r--r--   0        0        0    11514 2023-04-10 12:54:57.481179 w32py-0.3.6/w32py/korea.py
+-rw-r--r--   0        0        0      188 2023-02-27 00:06:25.415582 w32py-0.3.6/w32py/psutil.py
+-rw-r--r--   0        0        0        0 2023-02-27 00:06:25.415582 w32py-0.3.6/w32py/py.typed
+-rw-r--r--   0        0        0      921 2023-02-27 00:06:25.416774 w32py-0.3.6/w32py/win.py
+-rw-r--r--   0        0        0      163 2023-02-27 00:06:25.416774 w32py-0.3.6/w32py/winauto.py
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 w32py-0.3.6/PKG-INFO
```

### Comparing `w32py-0.3.5/.gitignore` & `w32py-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `w32py-0.3.5/LICENSE` & `w32py-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `w32py-0.3.5/pyproject.toml` & `w32py-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `w32py-0.3.5/w32py/ebest.py` & `w32py-0.3.6/w32py/ebest.py`

 * *Files identical despite different names*

### Comparing `w32py-0.3.5/w32py/korea.py` & `w32py-0.3.6/w32py/korea.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         ):
             fields = v["fields"]
             if v["occurs"]:
                 block[szBlockName] = [
                     self.getBlock(nBlockIdx, nRecIdx, fields)
                     for nRecIdx in range(
                         self.com.dynamicCall(
-                            "GetMultiRecrodCount(int)", nBlockIdx
+                            "GetMultiRecordCount(int)", nBlockIdx
                         )
                     )
                 ]
             else:
                 nRecIdx = 0
                 block[szBlockName] = self.getBlock(nBlockIdx, nRecIdx, fields)
         responseQuery = {
```

### Comparing `w32py-0.3.5/w32py/win.py` & `w32py-0.3.6/w32py/win.py`

 * *Files identical despite different names*

### Comparing `w32py-0.3.5/PKG-INFO` & `w32py-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w32py
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python Win32 API
 Author-email: Tom <nanticj@users.noreply.github.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: PyQt5 >=5.15,<5.16
 Requires-Dist: loguru >=0.6,<0.7
```

