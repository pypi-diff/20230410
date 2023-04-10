# Comparing `tmp/text_excuse_generator-1.1.3.tar.gz` & `tmp/text_excuse_generator-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_excuse_generator-1.1.3.tar", last modified: Mon Apr 10 07:40:23 2023, max compression
+gzip compressed data, was "text_excuse_generator-1.1.4.tar", last modified: Mon Apr 10 07:44:12 2023, max compression
```

## Comparing `text_excuse_generator-1.1.3.tar` & `text_excuse_generator-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:40:23.865104 text_excuse_generator-1.1.3/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.3/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 07:40:23.864934 text_excuse_generator-1.1.3/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 07:40:23.865154 text_excuse_generator-1.1.3/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)      986 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/setup.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:40:23.864050 text_excuse_generator-1.1.3/text_excuse_generator/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.3/text_excuse_generator/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)    10312 2023-04-10 07:37:07.000000 text_excuse_generator-1.1.3/text_excuse_generator/excuse_generator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:40:23.864714 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/top_level.txt
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:44:12.777505 text_excuse_generator-1.1.4/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.4/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 07:44:12.777267 text_excuse_generator-1.1.4/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 07:44:12.777576 text_excuse_generator-1.1.4/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)      986 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:44:12.776367 text_excuse_generator-1.1.4/text_excuse_generator/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.4/text_excuse_generator/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)    10312 2023-04-10 07:37:07.000000 text_excuse_generator-1.1.4/text_excuse_generator/excuse_generator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:44:12.776984 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/top_level.txt
```

### Comparing `text_excuse_generator-1.1.3/LICENSE` & `text_excuse_generator-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `text_excuse_generator-1.1.3/PKG-INFO` & `text_excuse_generator-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_excuse_generator
-Version: 1.1.3
+Version: 1.1.4
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `text_excuse_generator-1.1.3/setup.py` & `text_excuse_generator-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 README_PATH = join(dirname(__file__), "docs/README.md")
 
 with open(README_PATH, "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name = "text_excuse_generator",
-	version = '1.1.3',
+	version = '1.1.4',
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
     description = "Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it",
     long_description = LONG_DESCRIPTION,
     long_description_content_type = "text/markdown",
     packages = find_packages(),
     install_requires = ["python-dotenv", "twilio", "openai", "phonenumbers"],
```

### Comparing `text_excuse_generator-1.1.3/text_excuse_generator/excuse_generator.py` & `text_excuse_generator-1.1.4/text_excuse_generator/excuse_generator.py`

 * *Files identical despite different names*

### Comparing `text_excuse_generator-1.1.3/text_excuse_generator.egg-info/PKG-INFO` & `text_excuse_generator-1.1.4/text_excuse_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-excuse-generator
-Version: 1.1.3
+Version: 1.1.4
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

