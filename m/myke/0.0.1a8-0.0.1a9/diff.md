# Comparing `tmp/myke-0.0.1a8.tar.gz` & `tmp/myke-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myke-0.0.1a8.tar", last modified: Tue Dec  6 19:09:33 2022, max compression
+gzip compressed data, was "myke-0.0.1a9.tar", last modified: Wed Dec  7 09:03:14 2022, max compression
```

## Comparing `myke-0.0.1a8.tar` & `myke-0.0.1a9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 donald    (1000) donald    (1000)        0 2022-12-06 19:09:33.570773 myke-0.0.1a8/
--rw-rw-r--   0 donald    (1000) donald    (1000)     1080 2022-12-02 04:37:37.000000 myke-0.0.1a8/LICENSE
--rw-rw-r--   0 donald    (1000) donald    (1000)       16 2022-11-03 05:53:17.000000 myke-0.0.1a8/MANIFEST.in
--rw-rw-r--   0 donald    (1000) donald    (1000)     1324 2022-12-06 19:09:33.570773 myke-0.0.1a8/PKG-INFO
--rw-rw-r--   0 donald    (1000) donald    (1000)      598 2022-12-06 19:03:56.000000 myke-0.0.1a8/README.md
--rw-rw-r--   0 donald    (1000) donald    (1000)        8 2022-11-28 05:07:59.000000 myke-0.0.1a8/VERSION
--rw-rw-r--   0 donald    (1000) donald    (1000)     2762 2022-12-06 19:09:33.570773 myke-0.0.1a8/setup.cfg
--rw-rw-r--   0 donald    (1000) donald    (1000)       38 2022-12-02 04:37:37.000000 myke-0.0.1a8/setup.py
-drwxrwxr-x   0 donald    (1000) donald    (1000)        0 2022-12-06 19:09:33.566773 myke-0.0.1a8/src/
-drwxrwxr-x   0 donald    (1000) donald    (1000)        0 2022-12-06 19:09:33.566773 myke-0.0.1a8/src/myke/
--rw-rw-r--   0 donald    (1000) donald    (1000)      818 2022-12-02 04:37:37.000000 myke-0.0.1a8/src/myke/__init__.py
--rw-rw-r--   0 donald    (1000) donald    (1000)       62 2022-12-02 04:37:37.000000 myke-0.0.1a8/src/myke/__main__.py
--rw-rw-r--   0 donald    (1000) donald    (1000)       24 2022-12-02 04:37:37.000000 myke-0.0.1a8/src/myke/__version__.py
--rw-rw-r--   0 donald    (1000) donald    (1000)      859 2022-12-02 04:37:37.000000 myke-0.0.1a8/src/myke/exceptions.py
--rw-rw-r--   0 donald    (1000) donald    (1000)      206 2022-11-16 13:23:00.000000 myke-0.0.1a8/src/myke/globals.py
-drwxrwxr-x   0 donald    (1000) donald    (1000)        0 2022-12-06 19:09:33.570773 myke-0.0.1a8/src/myke/io/
--rw-rw-r--   0 donald    (1000) donald    (1000)        0 2022-11-03 05:53:17.000000 myke-0.0.1a8/src/myke/io/__init__.py
--rw-rw-r--   0 donald    (1000) donald    (1000)     2738 2022-11-28 04:47:38.000000 myke-0.0.1a8/src/myke/io/echo.py
--rw-rw-r--   0 donald    (1000) donald    (1000)     4150 2022-11-16 13:23:00.000000 myke-0.0.1a8/src/myke/io/read.py
--rw-rw-r--   0 donald    (1000) donald    (1000)     2953 2022-12-06 19:04:03.000000 myke-0.0.1a8/src/myke/io/write.py
--rw-rw-r--   0 donald    (1000) donald    (1000)     5159 2022-12-06 19:04:03.000000 myke-0.0.1a8/src/myke/main.py
--rw-rw-r--   0 donald    (1000) donald    (1000)        0 2022-12-02 04:37:37.000000 myke-0.0.1a8/src/myke/py.typed
--rw-rw-r--   0 donald    (1000) donald    (1000)     2158 2022-11-16 13:23:00.000000 myke-0.0.1a8/src/myke/sh.py
--rw-rw-r--   0 donald    (1000) donald    (1000)     6766 2022-11-28 04:47:38.000000 myke-0.0.1a8/src/myke/tasks.py
--rw-rw-r--   0 donald    (1000) donald    (1000)      235 2022-11-16 13:23:00.000000 myke-0.0.1a8/src/myke/types.py
--rw-rw-r--   0 donald    (1000) donald    (1000)     2120 2022-11-16 13:23:00.000000 myke-0.0.1a8/src/myke/utils.py
-drwxrwxr-x   0 donald    (1000) donald    (1000)        0 2022-12-06 19:09:33.570773 myke-0.0.1a8/src/myke.egg-info/
--rw-rw-r--   0 donald    (1000) donald    (1000)     1324 2022-12-06 19:09:33.000000 myke-0.0.1a8/src/myke.egg-info/PKG-INFO
--rw-rw-r--   0 donald    (1000) donald    (1000)      548 2022-12-06 19:09:33.000000 myke-0.0.1a8/src/myke.egg-info/SOURCES.txt
--rw-rw-r--   0 donald    (1000) donald    (1000)        1 2022-12-06 19:09:33.000000 myke-0.0.1a8/src/myke.egg-info/dependency_links.txt
--rw-rw-r--   0 donald    (1000) donald    (1000)       44 2022-12-06 19:09:33.000000 myke-0.0.1a8/src/myke.egg-info/entry_points.txt
--rw-rw-r--   0 donald    (1000) donald    (1000)      613 2022-12-06 19:09:33.000000 myke-0.0.1a8/src/myke.egg-info/requires.txt
--rw-rw-r--   0 donald    (1000) donald    (1000)        5 2022-12-06 19:09:33.000000 myke-0.0.1a8/src/myke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.264223 myke-0.0.1a9/
+-rw-r--r--   0 root         (0) root         (0)     1080 2022-12-07 08:59:42.000000 myke-0.0.1a9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2022-12-07 08:59:42.000000 myke-0.0.1a9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1324 2022-12-07 09:03:14.264223 myke-0.0.1a9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      598 2022-12-07 08:59:42.000000 myke-0.0.1a9/README.md
+-rw-r--r--   0 root         (0) root         (0)        8 2022-12-07 08:59:42.000000 myke-0.0.1a9/VERSION
+-rw-r--r--   0 root         (0) root         (0)     2762 2022-12-07 09:03:14.264223 myke-0.0.1a9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-07 08:59:42.000000 myke-0.0.1a9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.260223 myke-0.0.1a9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.264223 myke-0.0.1a9/src/myke/
+-rw-r--r--   0 root         (0) root         (0)      818 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       62 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2022-12-07 09:03:07.000000 myke-0.0.1a9/src/myke/__version__.py
+-rw-r--r--   0 root         (0) root         (0)      859 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      206 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/globals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.264223 myke-0.0.1a9/src/myke/io/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/io/echo.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/io/read.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/io/write.py
+-rw-r--r--   0 root         (0) root         (0)     5159 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/main.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2126 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/sh.py
+-rw-r--r--   0 root         (0) root         (0)     6766 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/tasks.py
+-rw-r--r--   0 root         (0) root         (0)      235 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/types.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.264223 myke-0.0.1a9/src/myke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1324 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      613 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/top_level.txt
```

### Comparing `myke-0.0.1a8/LICENSE` & `myke-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/PKG-INFO` & `myke-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myke
-Version: 0.0.1a8
+Version: 0.0.1a9
 Home-page: https://codeberg.org/Fresh2dev/myke
 Author: donald
 Author-email: hello@Fresh2.dev
 Project-URL: Repository, https://codeberg.org/Fresh2dev/myke
 Project-URL: Issues, https://codeberg.org/Fresh2dev/myke/issues
 Project-URL: Documentation, https://www.Fresh2.dev/code/r/myke/i/docs
 Project-URL: Changelog, https://www.Fresh2.dev/code/r/myke/i/docs/changelog
```

### Comparing `myke-0.0.1a8/README.md` & `myke-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/setup.cfg` & `myke-0.0.1a9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	typing-extensions; python_version<'3.10'
-	yapx==0.0.1a5
+	yapx==0.0.1a6
 
 [options.package_data]
 * = *
 
 [options.extras_require]
 build = 
 	build
```

### Comparing `myke-0.0.1a8/src/myke/__init__.py` & `myke-0.0.1a9/src/myke/__init__.py`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/src/myke/exceptions.py` & `myke-0.0.1a9/src/myke/exceptions.py`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/src/myke/io/echo.py` & `myke-0.0.1a9/src/myke/io/echo.py`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/src/myke/io/read.py` & `myke-0.0.1a9/src/myke/io/read.py`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/src/myke/io/write.py` & `myke-0.0.1a9/src/myke/io/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             content="""#!/usr/bin/env python3
 # type: ignore
 # pylint: skip-file
 # flake8: noqa
 import myke  # noqa
 
 myke.require(
-    "mykefiles==0.0.1a3.dev8",
+    "mykefiles==0.0.1a3.dev9",
     pip_args=[
         "--extra-index-url",
         "https://codeberg.org/api/packages/Fresh2dev/pypi/simple",
     ],
 )
 from mykefiles import hello_world  # noqa
```

### Comparing `myke-0.0.1a8/src/myke/main.py` & `myke-0.0.1a9/src/myke/main.py`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/src/myke/sh.py` & `myke-0.0.1a9/src/myke/sh.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     return os.linesep.join(sh_stdout_lines(*args, **kwargs))
 
 
 def require(*args: str, pip_args: list[str] | None = None, **kwargs: str) -> None:
     if not pip_args:
         pip_args = []
 
-    # 'mykefiles==0.0.1a3.dev2'
     sh_stdout(
         [
             sys.executable,
             "-m",
             "pip",
             "install",
             *pip_args,
```

### Comparing `myke-0.0.1a8/src/myke/tasks.py` & `myke-0.0.1a9/src/myke/tasks.py`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/src/myke/utils.py` & `myke-0.0.1a9/src/myke/utils.py`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/src/myke.egg-info/PKG-INFO` & `myke-0.0.1a9/src/myke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myke
-Version: 0.0.1a8
+Version: 0.0.1a9
 Home-page: https://codeberg.org/Fresh2dev/myke
 Author: donald
 Author-email: hello@Fresh2.dev
 Project-URL: Repository, https://codeberg.org/Fresh2dev/myke
 Project-URL: Issues, https://codeberg.org/Fresh2dev/myke/issues
 Project-URL: Documentation, https://www.Fresh2.dev/code/r/myke/i/docs
 Project-URL: Changelog, https://www.Fresh2.dev/code/r/myke/i/docs/changelog
```

### Comparing `myke-0.0.1a8/src/myke.egg-info/SOURCES.txt` & `myke-0.0.1a9/src/myke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myke-0.0.1a8/src/myke.egg-info/requires.txt` & `myke-0.0.1a9/src/myke.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-yapx==0.0.1a5
+yapx==0.0.1a6
 
 [:python_version < "3.10"]
 typing-extensions
 
 [build]
 build
 setuptools
```

