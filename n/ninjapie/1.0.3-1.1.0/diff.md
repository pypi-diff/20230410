# Comparing `tmp/ninjapie-1.0.3.tar.gz` & `tmp/ninjapie-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjapie-1.0.3.tar", last modified: Sun Apr  9 18:13:50 2023, max compression
+gzip compressed data, was "ninjapie-1.1.0.tar", last modified: Mon Apr 10 06:38:42 2023, max compression
```

## Comparing `ninjapie-1.0.3.tar` & `ninjapie-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 18:13:50.010150 ninjapie-1.0.3/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.0.3/LICENSE
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 18:13:50.010150 ninjapie-1.0.3/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6139 2023-04-09 11:30:25.000000 ninjapie-1.0.3/README.md
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 18:13:50.006817 ninjapie-1.0.3/ninjapie/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      158 2023-04-09 18:13:41.000000 ninjapie-1.0.3/ninjapie/__init__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     4644 2023-04-09 15:55:05.000000 ninjapie-1.0.3/ninjapie/__main__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27728 2023-04-09 16:36:42.000000 ninjapie-1.0.3/ninjapie/env.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19340 2023-04-09 15:57:25.000000 ninjapie-1.0.3/ninjapie/generator.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.0.3/ninjapie/path.py
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 18:13:50.006817 ninjapie-1.0.3/ninjapie.egg-info/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      292 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/SOURCES.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/dependency_links.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/entry_points.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       14 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/top_level.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1339 2023-04-09 18:13:41.000000 ninjapie-1.0.3/pyproject.toml
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-09 18:13:50.010150 ninjapie-1.0.3/setup.cfg
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-10 06:38:42.496231 ninjapie-1.1.0/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.1.0/LICENSE
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-10 06:38:42.496231 ninjapie-1.1.0/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6139 2023-04-09 11:30:25.000000 ninjapie-1.1.0/README.md
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-10 06:38:42.496231 ninjapie-1.1.0/ninjapie/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      169 2023-04-10 06:20:47.000000 ninjapie-1.1.0/ninjapie/__init__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     5045 2023-04-10 06:32:28.000000 ninjapie-1.1.0/ninjapie/__main__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27728 2023-04-09 16:36:42.000000 ninjapie-1.1.0/ninjapie/env.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19340 2023-04-09 15:57:25.000000 ninjapie-1.1.0/ninjapie/generator.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.1.0/ninjapie/path.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       22 2023-04-10 06:36:28.000000 ninjapie-1.1.0/ninjapie/version.py
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-10 06:38:42.496231 ninjapie-1.1.0/ninjapie.egg-info/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      312 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/SOURCES.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/dependency_links.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/entry_points.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       20 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/top_level.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1338 2023-04-10 06:36:28.000000 ninjapie-1.1.0/pyproject.toml
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-10 06:38:42.496231 ninjapie-1.1.0/setup.cfg
```

### Comparing `ninjapie-1.0.3/LICENSE` & `ninjapie-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.3/PKG-INFO` & `ninjapie-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.0.3
+Version: 1.1.0
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `ninjapie-1.0.3/README.md` & `ninjapie-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.3/ninjapie/__main__.py` & `ninjapie-1.1.0/ninjapie/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import argparse
 from glob import glob
 import os
 import subprocess
 import sys
 
+# read __version__ from relative from file to avoid that we need the ninjapie package
+with open(os.path.dirname(__file__) + '/version.py', encoding='utf-8') as vfile:
+    exec(vfile.read())  # pylint: disable=W0122
+
 
 def all_files(build_dir):
     """Collects a string with all files found by the patters in the globs file"""
 
     files = ''
     try:
         with open(build_dir + '/.build.globs', 'r', encoding='utf-8') as file:
@@ -98,14 +102,18 @@
 
     # define command line arguments
     parser = argparse.ArgumentParser(
         description='This is the Ninjapie build system. '
         'Besides the supported command line arguments all additional arguments, '
         'preceeded by "--", will be passed to ninja. For example "ninjapie -- -v".'
     )
+    version = __version__  # pylint: disable=E0602
+    parser.add_argument('--version', action='version',
+                        version='%(prog)s {version}'.format(version=version))
+
     subparsers = parser.add_subparsers(
         title='commands',
         description='The command to execute (build by default)',
     )
 
     parser_clean = subparsers.add_parser('clean', description='Removes the build directory')
     parser_clean.set_defaults(func=clean)
```

### Comparing `ninjapie-1.0.3/ninjapie/env.py` & `ninjapie-1.1.0/ninjapie/env.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.3/ninjapie/generator.py` & `ninjapie-1.1.0/ninjapie/generator.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.3/ninjapie/path.py` & `ninjapie-1.1.0/ninjapie/path.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.3/ninjapie.egg-info/PKG-INFO` & `ninjapie-1.1.0/ninjapie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.0.3
+Version: 1.1.0
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `ninjapie-1.0.3/pyproject.toml` & `ninjapie-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ninjapie"
-version = "1.0.3"
+version = "1.1.0"
 description = "Ninja-based build system with a Python API"
 readme = "README.md"
 authors = [{ name = "Nils Asmussen", email = "nils.asmussen@barkhauseninstitut.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -30,17 +30,17 @@
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 exclude = ["coverage*", "tests*"]
 
 [tool.bumpver]
-current_version = "1.0.3"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}."
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"ninjapie/__init__.py" = ["{version}"]
+"ninjapie/version.py" = ["{version}"]
```

