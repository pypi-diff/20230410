# Comparing `tmp/pyllms-0.1.1.tar.gz` & `tmp/pyllms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.1.1.tar", last modified: Mon Apr 10 19:35:57 2023, max compression
+gzip compressed data, was "pyllms-0.1.2.tar", last modified: Mon Apr 10 19:41:55 2023, max compression
```

## Comparing `pyllms-0.1.1.tar` & `pyllms-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:35:57.319219 pyllms-0.1.1/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.1/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    11441 2023-04-10 19:35:57.318889 pyllms-0.1.1/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    10284 2023-04-10 19:32:25.000000 pyllms-0.1.1/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:35:57.316573 pyllms-0.1.1/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)       83 2023-04-09 22:07:03.000000 pyllms-0.1.1/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    14766 2023-04-10 19:11:55.000000 pyllms-0.1.1/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:35:57.317434 pyllms-0.1.1/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.1/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1631 2023-04-10 19:09:27.000000 pyllms-0.1.1/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2003 2023-04-10 19:08:51.000000 pyllms-0.1.1/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1803 2023-04-10 19:09:11.000000 pyllms-0.1.1/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:35:57.318556 pyllms-0.1.1/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    11441 2023-04-10 19:35:57.000000 pyllms-0.1.1/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-10 19:35:57.000000 pyllms-0.1.1/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-10 19:35:57.000000 pyllms-0.1.1/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       60 2023-04-10 19:35:57.000000 pyllms-0.1.1/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-10 19:35:57.000000 pyllms-0.1.1/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-10 19:35:57.319305 pyllms-0.1.1/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1680 2023-04-10 19:35:52.000000 pyllms-0.1.1/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:41:55.712215 pyllms-0.1.2/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.2/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    11447 2023-04-10 19:41:55.711900 pyllms-0.1.2/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    10284 2023-04-10 19:32:25.000000 pyllms-0.1.2/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:41:55.709494 pyllms-0.1.2/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)       83 2023-04-09 22:07:03.000000 pyllms-0.1.2/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    14766 2023-04-10 19:11:55.000000 pyllms-0.1.2/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:41:55.710433 pyllms-0.1.2/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.2/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1631 2023-04-10 19:09:27.000000 pyllms-0.1.2/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2003 2023-04-10 19:08:51.000000 pyllms-0.1.2/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1803 2023-04-10 19:09:11.000000 pyllms-0.1.2/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:41:55.711571 pyllms-0.1.2/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    11447 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       60 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-10 19:41:55.712294 pyllms-0.1.2/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1682 2023-04-10 19:41:51.000000 pyllms-0.1.2/setup.py
```

### Comparing `pyllms-0.1.1/LICENSE` & `pyllms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.1/PKG-INFO` & `pyllms-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A brief description of your package
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
-Project-URL: Documentation, https://github.com/kagisearch/llms
-Project-URL: Source Code, https://github.com/kagisearch/llms
-Project-URL: Issue Tracker, https://github.com/kagisearch/llms/issues
+Project-URL: Documentation, https://github.com/kagisearch/pyllms
+Project-URL: Source Code, https://github.com/kagisearch/pyllms
+Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyllms-0.1.1/README.md` & `pyllms-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.1/llms/llms.py` & `pyllms-0.1.2/llms/llms.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.1/llms/providers/ai21.py` & `pyllms-0.1.2/llms/providers/ai21.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.1/llms/providers/anthropic.py` & `pyllms-0.1.2/llms/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.1/llms/providers/openai.py` & `pyllms-0.1.2/llms/providers/openai.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.1/pyllms.egg-info/PKG-INFO` & `pyllms-0.1.2/pyllms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A brief description of your package
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
-Project-URL: Documentation, https://github.com/kagisearch/llms
-Project-URL: Source Code, https://github.com/kagisearch/llms
-Project-URL: Issue Tracker, https://github.com/kagisearch/llms/issues
+Project-URL: Documentation, https://github.com/kagisearch/pyllms
+Project-URL: Source Code, https://github.com/kagisearch/pyllms
+Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyllms-0.1.1/setup.py` & `pyllms-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 import pathlib
 
 # Get the long description from the README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
-_project_homepage = "https://github.com/kagisearch/llms"
+_project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.1.1",
+    version="0.1.2",
     description="A brief description of your package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
```

