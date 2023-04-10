# Comparing `tmp/yeagerai-agent-0.0.32.tar.gz` & `tmp/yeagerai-agent-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeagerai-agent-0.0.32.tar", last modified: Mon Apr 10 14:20:35 2023, max compression
+gzip compressed data, was "yeagerai-agent-0.0.33.tar", last modified: Mon Apr 10 14:24:40 2023, max compression
```

## Comparing `yeagerai-agent-0.0.32.tar` & `yeagerai-agent-0.0.33.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.910380 yeagerai-agent-0.0.32/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-09 11:08:36.000000 yeagerai-agent-0.0.32/LICENSE
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:20:35.910380 yeagerai-agent-0.0.32/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2731 2023-04-10 01:09:09.000000 yeagerai-agent-0.0.32/README.md
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-10 14:20:35.910380 yeagerai-agent-0.0.32/setup.cfg
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1190 2023-04-10 14:20:31.000000 yeagerai-agent-0.0.32/setup.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.906381 yeagerai-agent-0.0.32/yeagerai/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 13:23:58.000000 yeagerai-agent-0.0.32/yeagerai/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.906381 yeagerai-agent-0.0.32/yeagerai/agent/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       42 2023-04-09 14:58:07.000000 yeagerai-agent-0.0.32/yeagerai/agent/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1161 2023-04-09 18:33:12.000000 yeagerai-agent-0.0.32/yeagerai/agent/master_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/agent/output_parser.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/agent/prompt_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4197 2023-04-09 22:21:35.000000 yeagerai-agent-0.0.32/yeagerai/agent/yeagerai_agent.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.906381 yeagerai-agent-0.0.32/yeagerai/interfaces/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-06 00:28:34.000000 yeagerai-agent-0.0.32/yeagerai/interfaces/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.906381 yeagerai-agent-0.0.32/yeagerai/interfaces/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       65 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/interfaces/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/interfaces/callbacks/local_file_system_n_git.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2684 2023-04-09 21:19:00.000000 yeagerai-agent-0.0.32/yeagerai/interfaces/cli.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.906381 yeagerai-agent-0.0.32/yeagerai/memory/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       46 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/memory/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.906381 yeagerai-agent-0.0.32/yeagerai/memory/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       55 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/memory/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/memory/callbacks/session_memory_handler.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/memory/yeagerai_context.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.906381 yeagerai-agent-0.0.32/yeagerai/toolkit/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      461 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/toolkit/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.906381 yeagerai-agent-0.0.32/yeagerai/toolkit/create_tool_source/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 16:52:27.000000 yeagerai-agent-0.0.32/yeagerai/toolkit/create_tool_source/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1725 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4878 2023-04-09 22:02:27.000000 yeagerai-agent-0.0.32/yeagerai/toolkit/create_tool_source/create_tool_source.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-09 13:24:39.000000 yeagerai-agent-0.0.32/yeagerai/toolkit/yeagerai_tool.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      589 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.32/yeagerai/toolkit/yeagerai_toolkit.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:20:35.906381 yeagerai-agent-0.0.32/yeagerai_agent.egg-info/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:20:35.000000 yeagerai-agent-0.0.32/yeagerai_agent.egg-info/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1020 2023-04-10 14:20:35.000000 yeagerai-agent-0.0.32/yeagerai_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-10 14:20:35.000000 yeagerai-agent-0.0.32/yeagerai_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       55 2023-04-10 14:20:35.000000 yeagerai-agent-0.0.32/yeagerai_agent.egg-info/entry_points.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       47 2023-04-10 14:20:35.000000 yeagerai-agent-0.0.32/yeagerai_agent.egg-info/requires.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-10 14:20:35.000000 yeagerai-agent-0.0.32/yeagerai_agent.egg-info/top_level.txt
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-09 11:08:36.000000 yeagerai-agent-0.0.33/LICENSE
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2731 2023-04-10 01:09:09.000000 yeagerai-agent-0.0.33/README.md
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/setup.cfg
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1199 2023-04-10 14:23:44.000000 yeagerai-agent-0.0.33/setup.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.502146 yeagerai-agent-0.0.33/yeagerai/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 13:23:58.000000 yeagerai-agent-0.0.33/yeagerai/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.502146 yeagerai-agent-0.0.33/yeagerai/agent/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       42 2023-04-09 14:58:07.000000 yeagerai-agent-0.0.33/yeagerai/agent/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1161 2023-04-09 18:33:12.000000 yeagerai-agent-0.0.33/yeagerai/agent/master_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/agent/output_parser.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/agent/prompt_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4197 2023-04-09 22:21:35.000000 yeagerai-agent-0.0.33/yeagerai/agent/yeagerai_agent.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/interfaces/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-06 00:28:34.000000 yeagerai-agent-0.0.33/yeagerai/interfaces/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/interfaces/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       65 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/interfaces/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/interfaces/callbacks/local_file_system_n_git.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2684 2023-04-09 21:19:00.000000 yeagerai-agent-0.0.33/yeagerai/interfaces/cli.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/memory/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       46 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/memory/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/memory/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       55 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/memory/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/memory/callbacks/session_memory_handler.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/memory/yeagerai_context.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/toolkit/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      461 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 16:52:27.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1725 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4878 2023-04-09 22:02:27.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/create_tool_source.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-09 13:24:39.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/yeagerai_tool.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      589 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/yeagerai_toolkit.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1020 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       64 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       47 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/requires.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/top_level.txt
```

### Comparing `yeagerai-agent-0.0.32/LICENSE` & `yeagerai-agent-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/PKG-INFO` & `yeagerai-agent-0.0.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.32
+Version: 0.0.33
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.32/README.md` & `yeagerai-agent-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/setup.py` & `yeagerai-agent-0.0.33/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name="yeagerai-agent",
-    version="0.0.32",
+    version="0.0.33",
     description="The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.",
     author="YeagerAI LLC",
     author_email="jm@yeager.ai",
     packages=find_packages(),
     install_requires=[
         "langchain",
         "openai",
         "GitPython",
         "click",
         "python-dotenv",
     ],
     entry_points={
         "console_scripts": [
-            "yeagerai-agent = interfaces.cli:main",
+            "yeagerai-agent = yeagerai.interfaces.cli:main",
         ],
     },
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

### Comparing `yeagerai-agent-0.0.32/yeagerai/agent/master_template.py` & `yeagerai-agent-0.0.33/yeagerai/agent/master_template.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/agent/output_parser.py` & `yeagerai-agent-0.0.33/yeagerai/agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/agent/prompt_template.py` & `yeagerai-agent-0.0.33/yeagerai/agent/prompt_template.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/agent/yeagerai_agent.py` & `yeagerai-agent-0.0.33/yeagerai/agent/yeagerai_agent.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/interfaces/callbacks/local_file_system_n_git.py` & `yeagerai-agent-0.0.33/yeagerai/interfaces/callbacks/local_file_system_n_git.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/interfaces/cli.py` & `yeagerai-agent-0.0.33/yeagerai/interfaces/cli.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/memory/callbacks/session_memory_handler.py` & `yeagerai-agent-0.0.33/yeagerai/memory/callbacks/session_memory_handler.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/memory/yeagerai_context.py` & `yeagerai-agent-0.0.33/yeagerai/memory/yeagerai_context.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py` & `yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/toolkit/create_tool_source/create_tool_source.py` & `yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/create_tool_source.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai/toolkit/yeagerai_toolkit.py` & `yeagerai-agent-0.0.33/yeagerai/toolkit/yeagerai_toolkit.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.32/yeagerai_agent.egg-info/PKG-INFO` & `yeagerai-agent-0.0.33/yeagerai_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.32
+Version: 0.0.33
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.32/yeagerai_agent.egg-info/SOURCES.txt` & `yeagerai-agent-0.0.33/yeagerai_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

