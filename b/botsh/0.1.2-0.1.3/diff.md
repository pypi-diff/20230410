# Comparing `tmp/botsh-0.1.2.tar.gz` & `tmp/botsh-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botsh-0.1.2.tar", last modified: Mon Apr 10 14:41:40 2023, max compression
+gzip compressed data, was "botsh-0.1.3.tar", last modified: Mon Apr 10 16:06:21 2023, max compression
```

## Comparing `botsh-0.1.2.tar` & `botsh-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.946276 botsh-0.1.2/
--rw-r--r--   0 paulbutler   (501) staff       (20)       54 2023-04-10 14:28:50.000000 botsh-0.1.2/MANIFEST.in
--rw-r--r--   0 paulbutler   (501) staff       (20)     3527 2023-04-10 14:41:40.946043 botsh-0.1.2/PKG-INFO
--rw-r--r--   0 paulbutler   (501) staff       (20)      234 2023-04-10 14:12:58.000000 botsh-0.1.2/Pipfile
--rw-r--r--   0 paulbutler   (501) staff       (20)    64876 2023-04-10 14:13:02.000000 botsh-0.1.2/Pipfile.lock
--rw-r--r--   0 paulbutler   (501) staff       (20)     2888 2023-04-10 14:19:23.000000 botsh-0.1.2/README.md
--rw-r--r--   0 paulbutler   (501) staff       (20)       38 2023-04-10 14:41:40.946342 botsh-0.1.2/setup.cfg
--rw-r--r--   0 paulbutler   (501) staff       (20)     1597 2023-04-10 14:40:26.000000 botsh-0.1.2/setup.py
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.941098 botsh-0.1.2/src/
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.944502 botsh-0.1.2/src/botsh/
--rw-r--r--   0 paulbutler   (501) staff       (20)        0 2023-04-10 09:30:05.000000 botsh-0.1.2/src/botsh/__init__.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     3264 2023-04-10 14:41:08.000000 botsh-0.1.2/src/botsh/docker_exec.py
--rw-r--r--   0 paulbutler   (501) staff       (20)      317 2023-04-10 11:28:56.000000 botsh-0.1.2/src/botsh/history.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     1479 2023-04-10 13:40:08.000000 botsh-0.1.2/src/botsh/llm.py
--rw-r--r--   0 paulbutler   (501) staff       (20)       46 2023-04-10 12:14:03.000000 botsh-0.1.2/src/botsh/logging.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     2718 2023-04-10 14:39:56.000000 botsh-0.1.2/src/botsh/main.py
--rw-r--r--   0 paulbutler   (501) staff       (20)      972 2023-04-10 12:28:06.000000 botsh-0.1.2/src/botsh/prompt.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     2164 2023-04-10 13:51:16.000000 botsh-0.1.2/src/botsh/task_driver.py
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.945718 botsh-0.1.2/src/botsh/templates/
--rw-r--r--   0 paulbutler   (501) staff       (20)     1099 2023-04-10 13:51:54.000000 botsh-0.1.2/src/botsh/templates/prompt.jinja2
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.945596 botsh-0.1.2/src/botsh.egg-info/
--rw-r--r--   0 paulbutler   (501) staff       (20)     3527 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/PKG-INFO
--rw-r--r--   0 paulbutler   (501) staff       (20)      454 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/SOURCES.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)        1 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/dependency_links.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)       42 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/entry_points.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)      881 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/requires.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)        6 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/top_level.txt
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.516873 botsh-0.1.3/
+-rw-r--r--   0 paulbutler   (501) staff       (20)       54 2023-04-10 14:28:50.000000 botsh-0.1.3/MANIFEST.in
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3791 2023-04-10 16:06:21.516674 botsh-0.1.3/PKG-INFO
+-rw-r--r--   0 paulbutler   (501) staff       (20)      234 2023-04-10 14:12:58.000000 botsh-0.1.3/Pipfile
+-rw-r--r--   0 paulbutler   (501) staff       (20)    64876 2023-04-10 14:13:02.000000 botsh-0.1.3/Pipfile.lock
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3152 2023-04-10 16:05:16.000000 botsh-0.1.3/README.md
+-rw-r--r--   0 paulbutler   (501) staff       (20)       38 2023-04-10 16:06:21.516914 botsh-0.1.3/setup.cfg
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1597 2023-04-10 16:05:22.000000 botsh-0.1.3/setup.py
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.512266 botsh-0.1.3/src/
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.515121 botsh-0.1.3/src/botsh/
+-rw-r--r--   0 paulbutler   (501) staff       (20)        0 2023-04-10 09:30:05.000000 botsh-0.1.3/src/botsh/__init__.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3264 2023-04-10 14:41:08.000000 botsh-0.1.3/src/botsh/docker_exec.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)      317 2023-04-10 11:28:56.000000 botsh-0.1.3/src/botsh/history.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1479 2023-04-10 13:40:08.000000 botsh-0.1.3/src/botsh/llm.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)       46 2023-04-10 12:14:03.000000 botsh-0.1.3/src/botsh/logging.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2718 2023-04-10 14:39:56.000000 botsh-0.1.3/src/botsh/main.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)      972 2023-04-10 12:28:06.000000 botsh-0.1.3/src/botsh/prompt.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2164 2023-04-10 13:51:16.000000 botsh-0.1.3/src/botsh/task_driver.py
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.516315 botsh-0.1.3/src/botsh/templates/
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1099 2023-04-10 13:51:54.000000 botsh-0.1.3/src/botsh/templates/prompt.jinja2
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.516125 botsh-0.1.3/src/botsh.egg-info/
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3791 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/PKG-INFO
+-rw-r--r--   0 paulbutler   (501) staff       (20)      454 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/SOURCES.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)        1 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/dependency_links.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)       42 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/entry_points.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)      881 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/requires.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)        6 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/top_level.txt
```

### Comparing `botsh-0.1.2/PKG-INFO` & `botsh-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.2
+Version: 0.1.3
 Summary: A task runner powered by OpenAI and Docker.
 Home-page: https://github.com/drifting-in-space/botsh
 Author: Paul Butler
 Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,23 +29,14 @@
 will then attach the OpenAI API to a shell running in the container
 to attempt to complete the given task.
 
 The AI is explicitly told that it is allowed to install software,
 and will typically install programs as needed to complete its task.
 Installed software remains confined to the container.
 
-When `botsh` is invoked, the current working directory is mounted
-into the container and can be modified by programs the agent runs.
-The filesystem outside of the current working directory is sealed
-off from the container.
-
-Each directory that you run `botsh` in will get its own container,
-which is reused for future invocations of `botsh` in that container.
-You can tell it to wipe 
-
 ## Setup
 
 Install with:
 
     pip install botsh
 
 `botsh` expects an OpenAI API key to be provided as the `OPENAI_API_KEY`
@@ -66,14 +57,31 @@
 These observations relate to the default model, `text-davinci-003`. Using GPT-4 may improve things.
 
 - It works best if you explicitly specify the files/paths you want to work with (use relative references).
   It is not good at figuring out what you mean.
 - It often gets stuck in loops if it can't complete a task rather than giving up, despite the prompt
   telling it not to.
 
+## Container re-use
+
+When `botsh` is invoked, the current working directory is mounted
+into the container and can be modified by programs the agent runs.
+The filesystem outside of the current working directory is sealed
+off from the container.
+
+Each directory that you run `botsh` in will get its own container,
+which is reused for future invocations of `botsh` in that container.
+
+You can pass `--wipe` to discard the existing container and start a
+new one before running your task. You can also pass `--rm` to remove
+a container at the end of your task.
+
+Containers are also removed if you purge containers in Docker with
+`docker container prune`
+
 ## Usage
 
 ```
 usage: botsh [-h] [--max-rounds MAX_ROUNDS] [--model MODEL] [--image IMAGE] [--shell-command SHELL_COMMAND] [--save-transcript] [--wipe] prompt
 
 Task runner powered by OpenAI and Docker. Invoke botsh by providing a task as a command line argument. botsh will create a bare Ubuntu Docker container associated with the current directory, or create one if one does not exist. botsh will then attach the OpenAI API to a shell running in the container to attempt to complete the given task.
```

### Comparing `botsh-0.1.2/Pipfile.lock` & `botsh-0.1.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `botsh-0.1.2/README.md` & `botsh-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,14 @@
 will then attach the OpenAI API to a shell running in the container
 to attempt to complete the given task.
 
 The AI is explicitly told that it is allowed to install software,
 and will typically install programs as needed to complete its task.
 Installed software remains confined to the container.
 
-When `botsh` is invoked, the current working directory is mounted
-into the container and can be modified by programs the agent runs.
-The filesystem outside of the current working directory is sealed
-off from the container.
-
-Each directory that you run `botsh` in will get its own container,
-which is reused for future invocations of `botsh` in that container.
-You can tell it to wipe 
-
 ## Setup
 
 Install with:
 
     pip install botsh
 
 `botsh` expects an OpenAI API key to be provided as the `OPENAI_API_KEY`
@@ -48,14 +39,31 @@
 These observations relate to the default model, `text-davinci-003`. Using GPT-4 may improve things.
 
 - It works best if you explicitly specify the files/paths you want to work with (use relative references).
   It is not good at figuring out what you mean.
 - It often gets stuck in loops if it can't complete a task rather than giving up, despite the prompt
   telling it not to.
 
+## Container re-use
+
+When `botsh` is invoked, the current working directory is mounted
+into the container and can be modified by programs the agent runs.
+The filesystem outside of the current working directory is sealed
+off from the container.
+
+Each directory that you run `botsh` in will get its own container,
+which is reused for future invocations of `botsh` in that container.
+
+You can pass `--wipe` to discard the existing container and start a
+new one before running your task. You can also pass `--rm` to remove
+a container at the end of your task.
+
+Containers are also removed if you purge containers in Docker with
+`docker container prune`
+
 ## Usage
 
 ```
 usage: botsh [-h] [--max-rounds MAX_ROUNDS] [--model MODEL] [--image IMAGE] [--shell-command SHELL_COMMAND] [--save-transcript] [--wipe] prompt
 
 Task runner powered by OpenAI and Docker. Invoke botsh by providing a task as a command line argument. botsh will create a bare Ubuntu Docker container associated with the current directory, or create one if one does not exist. botsh will then attach the OpenAI API to a shell running in the container to attempt to complete the given task.
```

### Comparing `botsh-0.1.2/setup.py` & `botsh-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         f"{pkg_name}{pkg_info['version']}"
         for pkg_name, pkg_info in pipfile_lock[mode].items()
     ]
 
 
 setup(
     name="botsh",
-    version="0.1.2",
+    version="0.1.3",
     description="A task runner powered by OpenAI and Docker.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Paul Butler",
     author_email="paul@driftingin.space",
     url="https://github.com/drifting-in-space/botsh",
     packages=find_packages("src"),
```

### Comparing `botsh-0.1.2/src/botsh/docker_exec.py` & `botsh-0.1.3/src/botsh/docker_exec.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.2/src/botsh/llm.py` & `botsh-0.1.3/src/botsh/llm.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.2/src/botsh/main.py` & `botsh-0.1.3/src/botsh/main.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.2/src/botsh/prompt.py` & `botsh-0.1.3/src/botsh/prompt.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.2/src/botsh/task_driver.py` & `botsh-0.1.3/src/botsh/task_driver.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.2/src/botsh/templates/prompt.jinja2` & `botsh-0.1.3/src/botsh/templates/prompt.jinja2`

 * *Files identical despite different names*

### Comparing `botsh-0.1.2/src/botsh.egg-info/PKG-INFO` & `botsh-0.1.3/src/botsh.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.2
+Version: 0.1.3
 Summary: A task runner powered by OpenAI and Docker.
 Home-page: https://github.com/drifting-in-space/botsh
 Author: Paul Butler
 Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,23 +29,14 @@
 will then attach the OpenAI API to a shell running in the container
 to attempt to complete the given task.
 
 The AI is explicitly told that it is allowed to install software,
 and will typically install programs as needed to complete its task.
 Installed software remains confined to the container.
 
-When `botsh` is invoked, the current working directory is mounted
-into the container and can be modified by programs the agent runs.
-The filesystem outside of the current working directory is sealed
-off from the container.
-
-Each directory that you run `botsh` in will get its own container,
-which is reused for future invocations of `botsh` in that container.
-You can tell it to wipe 
-
 ## Setup
 
 Install with:
 
     pip install botsh
 
 `botsh` expects an OpenAI API key to be provided as the `OPENAI_API_KEY`
@@ -66,14 +57,31 @@
 These observations relate to the default model, `text-davinci-003`. Using GPT-4 may improve things.
 
 - It works best if you explicitly specify the files/paths you want to work with (use relative references).
   It is not good at figuring out what you mean.
 - It often gets stuck in loops if it can't complete a task rather than giving up, despite the prompt
   telling it not to.
 
+## Container re-use
+
+When `botsh` is invoked, the current working directory is mounted
+into the container and can be modified by programs the agent runs.
+The filesystem outside of the current working directory is sealed
+off from the container.
+
+Each directory that you run `botsh` in will get its own container,
+which is reused for future invocations of `botsh` in that container.
+
+You can pass `--wipe` to discard the existing container and start a
+new one before running your task. You can also pass `--rm` to remove
+a container at the end of your task.
+
+Containers are also removed if you purge containers in Docker with
+`docker container prune`
+
 ## Usage
 
 ```
 usage: botsh [-h] [--max-rounds MAX_ROUNDS] [--model MODEL] [--image IMAGE] [--shell-command SHELL_COMMAND] [--save-transcript] [--wipe] prompt
 
 Task runner powered by OpenAI and Docker. Invoke botsh by providing a task as a command line argument. botsh will create a bare Ubuntu Docker container associated with the current directory, or create one if one does not exist. botsh will then attach the OpenAI API to a shell running in the container to attempt to complete the given task.
```

### Comparing `botsh-0.1.2/src/botsh.egg-info/requires.txt` & `botsh-0.1.3/src/botsh.egg-info/requires.txt`

 * *Files identical despite different names*

