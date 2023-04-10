# Comparing `tmp/botsh-0.1.0.tar.gz` & `tmp/botsh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botsh-0.1.0.tar", last modified: Mon Apr 10 14:14:39 2023, max compression
+gzip compressed data, was "botsh-0.1.1.tar", last modified: Mon Apr 10 14:30:02 2023, max compression
```

## Comparing `botsh-0.1.0.tar` & `botsh-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:14:39.104195 botsh-0.1.0/
--rw-r--r--   0 paulbutler   (501) staff       (20)     3444 2023-04-10 14:14:39.104041 botsh-0.1.0/PKG-INFO
--rw-r--r--   0 paulbutler   (501) staff       (20)     2763 2023-04-10 14:10:28.000000 botsh-0.1.0/README.md
--rw-r--r--   0 paulbutler   (501) staff       (20)       38 2023-04-10 14:14:39.104232 botsh-0.1.0/setup.cfg
--rw-r--r--   0 paulbutler   (501) staff       (20)     1540 2023-04-10 10:50:15.000000 botsh-0.1.0/setup.py
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:14:39.100194 botsh-0.1.0/src/
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:14:39.102554 botsh-0.1.0/src/botsh/
--rw-r--r--   0 paulbutler   (501) staff       (20)        0 2023-04-10 09:30:05.000000 botsh-0.1.0/src/botsh/__init__.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     3056 2023-04-10 14:09:21.000000 botsh-0.1.0/src/botsh/docker_exec.py
--rw-r--r--   0 paulbutler   (501) staff       (20)      317 2023-04-10 11:28:56.000000 botsh-0.1.0/src/botsh/history.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     1479 2023-04-10 13:40:08.000000 botsh-0.1.0/src/botsh/llm.py
--rw-r--r--   0 paulbutler   (501) staff       (20)       46 2023-04-10 12:14:03.000000 botsh-0.1.0/src/botsh/logging.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     2539 2023-04-10 14:08:25.000000 botsh-0.1.0/src/botsh/main.py
--rw-r--r--   0 paulbutler   (501) staff       (20)      972 2023-04-10 12:28:06.000000 botsh-0.1.0/src/botsh/prompt.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     2164 2023-04-10 13:51:16.000000 botsh-0.1.0/src/botsh/task_driver.py
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:14:39.103822 botsh-0.1.0/src/botsh.egg-info/
--rw-r--r--   0 paulbutler   (501) staff       (20)     3444 2023-04-10 14:14:39.000000 botsh-0.1.0/src/botsh.egg-info/PKG-INFO
--rw-r--r--   0 paulbutler   (501) staff       (20)      387 2023-04-10 14:14:39.000000 botsh-0.1.0/src/botsh.egg-info/SOURCES.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)        1 2023-04-10 14:14:39.000000 botsh-0.1.0/src/botsh.egg-info/dependency_links.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)       42 2023-04-10 14:14:39.000000 botsh-0.1.0/src/botsh.egg-info/entry_points.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)      881 2023-04-10 14:14:39.000000 botsh-0.1.0/src/botsh.egg-info/requires.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)        6 2023-04-10 14:14:39.000000 botsh-0.1.0/src/botsh.egg-info/top_level.txt
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.147375 botsh-0.1.1/
+-rw-r--r--   0 paulbutler   (501) staff       (20)       54 2023-04-10 14:28:50.000000 botsh-0.1.1/MANIFEST.in
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3527 2023-04-10 14:30:02.147196 botsh-0.1.1/PKG-INFO
+-rw-r--r--   0 paulbutler   (501) staff       (20)      234 2023-04-10 14:12:58.000000 botsh-0.1.1/Pipfile
+-rw-r--r--   0 paulbutler   (501) staff       (20)    64876 2023-04-10 14:13:02.000000 botsh-0.1.1/Pipfile.lock
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2888 2023-04-10 14:19:23.000000 botsh-0.1.1/README.md
+-rw-r--r--   0 paulbutler   (501) staff       (20)       38 2023-04-10 14:30:02.147416 botsh-0.1.1/setup.cfg
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1597 2023-04-10 14:25:01.000000 botsh-0.1.1/setup.py
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.142576 botsh-0.1.1/src/
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.145370 botsh-0.1.1/src/botsh/
+-rw-r--r--   0 paulbutler   (501) staff       (20)        0 2023-04-10 09:30:05.000000 botsh-0.1.1/src/botsh/__init__.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3056 2023-04-10 14:09:21.000000 botsh-0.1.1/src/botsh/docker_exec.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)      317 2023-04-10 11:28:56.000000 botsh-0.1.1/src/botsh/history.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1479 2023-04-10 13:40:08.000000 botsh-0.1.1/src/botsh/llm.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)       46 2023-04-10 12:14:03.000000 botsh-0.1.1/src/botsh/logging.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2539 2023-04-10 14:08:25.000000 botsh-0.1.1/src/botsh/main.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)      972 2023-04-10 12:28:06.000000 botsh-0.1.1/src/botsh/prompt.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2164 2023-04-10 13:51:16.000000 botsh-0.1.1/src/botsh/task_driver.py
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.146744 botsh-0.1.1/src/botsh/templates/
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1099 2023-04-10 13:51:54.000000 botsh-0.1.1/src/botsh/templates/prompt.jinja2
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.146615 botsh-0.1.1/src/botsh.egg-info/
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3527 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/PKG-INFO
+-rw-r--r--   0 paulbutler   (501) staff       (20)      454 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/SOURCES.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)        1 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/dependency_links.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)       42 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/entry_points.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)      881 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/requires.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)        6 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/top_level.txt
```

### Comparing `botsh-0.1.0/PKG-INFO` & `botsh-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.0
-Summary: A short description of your package
-Home-page: https://github.com/yourusername/your-package-name
-Author: Your Name
-Author-email: your.email@example.com
-Classifier: Development Status :: 3 - Alpha
+Version: 0.1.1
+Summary: A task runner powered by OpenAI and Docker.
+Home-page: https://github.com/drifting-in-space/botsh
+Author: Paul Butler
+Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # `botsh`
 
+[![PyPI version](https://badge.fury.io/py/botsh.svg)](https://badge.fury.io/py/botsh)
+
 `botsh` is a task runner powered by OpenAI and Docker.
 
 Invoke botsh by providing a task as a command line argument.
 
 botsh will create a bare Ubuntu Docker container associated with
 the current directory, or create one if one does not exist. botsh
 will then attach the OpenAI API to a shell running in the container
@@ -39,14 +40,18 @@
 
 Each directory that you run `botsh` in will get its own container,
 which is reused for future invocations of `botsh` in that container.
 You can tell it to wipe 
 
 ## Setup
 
+Install with:
+
+    pip install botsh
+
 `botsh` expects an OpenAI API key to be provided as the `OPENAI_API_KEY`
 environment variable.
 
 `botsh` also requires Docker to be running on the system.
 
 ## Examples
```

### Comparing `botsh-0.1.0/README.md` & `botsh-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # `botsh`
 
+[![PyPI version](https://badge.fury.io/py/botsh.svg)](https://badge.fury.io/py/botsh)
+
 `botsh` is a task runner powered by OpenAI and Docker.
 
 Invoke botsh by providing a task as a command line argument.
 
 botsh will create a bare Ubuntu Docker container associated with
 the current directory, or create one if one does not exist. botsh
 will then attach the OpenAI API to a shell running in the container
@@ -20,14 +22,18 @@
 
 Each directory that you run `botsh` in will get its own container,
 which is reused for future invocations of `botsh` in that container.
 You can tell it to wipe 
 
 ## Setup
 
+Install with:
+
+    pip install botsh
+
 `botsh` expects an OpenAI API key to be provided as the `OPENAI_API_KEY`
 environment variable.
 
 `botsh` also requires Docker to be running on the system.
 
 ## Examples
```

### Comparing `botsh-0.1.0/setup.py` & `botsh-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,25 +18,28 @@
         f"{pkg_name}{pkg_info['version']}"
         for pkg_name, pkg_info in pipfile_lock[mode].items()
     ]
 
 
 setup(
     name="botsh",
-    version="0.1.0",
-    description="A short description of your package",
+    version="0.1.1",
+    description="A task runner powered by OpenAI and Docker.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author="Your Name",
-    author_email="your.email@example.com",
-    url="https://github.com/yourusername/your-package-name",
+    author="Paul Butler",
+    author_email="paul@driftingin.space",
+    url="https://github.com/drifting-in-space/botsh",
     packages=find_packages("src"),
+    package_data={
+        "": ["Pipfile", "Pipfile.lock"],
+    },
+    include_package_data=True,
     package_dir={"": "src"},
     classifiers=[
-        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `botsh-0.1.0/src/botsh/docker_exec.py` & `botsh-0.1.1/src/botsh/docker_exec.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.0/src/botsh/llm.py` & `botsh-0.1.1/src/botsh/llm.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.0/src/botsh/main.py` & `botsh-0.1.1/src/botsh/main.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.0/src/botsh/prompt.py` & `botsh-0.1.1/src/botsh/prompt.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.0/src/botsh/task_driver.py` & `botsh-0.1.1/src/botsh/task_driver.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.0/src/botsh.egg-info/PKG-INFO` & `botsh-0.1.1/src/botsh.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.0
-Summary: A short description of your package
-Home-page: https://github.com/yourusername/your-package-name
-Author: Your Name
-Author-email: your.email@example.com
-Classifier: Development Status :: 3 - Alpha
+Version: 0.1.1
+Summary: A task runner powered by OpenAI and Docker.
+Home-page: https://github.com/drifting-in-space/botsh
+Author: Paul Butler
+Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # `botsh`
 
+[![PyPI version](https://badge.fury.io/py/botsh.svg)](https://badge.fury.io/py/botsh)
+
 `botsh` is a task runner powered by OpenAI and Docker.
 
 Invoke botsh by providing a task as a command line argument.
 
 botsh will create a bare Ubuntu Docker container associated with
 the current directory, or create one if one does not exist. botsh
 will then attach the OpenAI API to a shell running in the container
@@ -39,14 +40,18 @@
 
 Each directory that you run `botsh` in will get its own container,
 which is reused for future invocations of `botsh` in that container.
 You can tell it to wipe 
 
 ## Setup
 
+Install with:
+
+    pip install botsh
+
 `botsh` expects an OpenAI API key to be provided as the `OPENAI_API_KEY`
 environment variable.
 
 `botsh` also requires Docker to be running on the system.
 
 ## Examples
```

### Comparing `botsh-0.1.0/src/botsh.egg-info/requires.txt` & `botsh-0.1.1/src/botsh.egg-info/requires.txt`

 * *Files identical despite different names*

