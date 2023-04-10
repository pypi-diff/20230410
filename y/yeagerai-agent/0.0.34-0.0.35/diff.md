# Comparing `tmp/yeagerai-agent-0.0.34.tar.gz` & `tmp/yeagerai-agent-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeagerai-agent-0.0.34.tar", last modified: Mon Apr 10 14:33:19 2023, max compression
+gzip compressed data, was "yeagerai-agent-0.0.35.tar", last modified: Mon Apr 10 14:38:59 2023, max compression
```

## Comparing `yeagerai-agent-0.0.34.tar` & `yeagerai-agent-0.0.35.tar`

### file list

```diff
@@ -1,41 +1,49 @@
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-09 11:08:36.000000 yeagerai-agent-0.0.34/LICENSE
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2731 2023-04-10 01:09:09.000000 yeagerai-agent-0.0.34/README.md
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/setup.cfg
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1199 2023-04-10 14:33:04.000000 yeagerai-agent-0.0.34/setup.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 13:23:58.000000 yeagerai-agent-0.0.34/yeagerai/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/agent/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       56 2023-04-10 14:29:05.000000 yeagerai-agent-0.0.34/yeagerai/agent/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1161 2023-04-09 18:33:12.000000 yeagerai-agent-0.0.34/yeagerai/agent/master_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/agent/output_parser.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/agent/prompt_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4221 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.34/yeagerai/agent/yeagerai_agent.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/interfaces/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-06 00:28:34.000000 yeagerai-agent-0.0.34/yeagerai/interfaces/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/interfaces/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      103 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.34/yeagerai/interfaces/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/interfaces/callbacks/local_file_system_n_git.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2684 2023-04-09 21:19:00.000000 yeagerai-agent-0.0.34/yeagerai/interfaces/cli.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/memory/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       61 2023-04-10 14:29:33.000000 yeagerai-agent-0.0.34/yeagerai/memory/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/memory/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       80 2023-04-10 14:29:46.000000 yeagerai-agent-0.0.34/yeagerai/memory/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/memory/callbacks/session_memory_handler.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/memory/yeagerai_context.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/toolkit/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      541 2023-04-10 14:28:39.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 16:52:27.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1725 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4952 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/create_tool_source.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-09 13:24:39.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/yeagerai_tool.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      589 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/yeagerai_toolkit.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1020 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       64 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/entry_points.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       47 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/requires.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/top_level.txt
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.575943 yeagerai-agent-0.0.35/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-09 11:08:36.000000 yeagerai-agent-0.0.35/LICENSE
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:38:59.575943 yeagerai-agent-0.0.35/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2731 2023-04-10 01:09:09.000000 yeagerai-agent-0.0.35/README.md
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-10 14:38:59.575943 yeagerai-agent-0.0.35/setup.cfg
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1199 2023-04-10 14:38:20.000000 yeagerai-agent-0.0.35/setup.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.571943 yeagerai-agent-0.0.35/yeagerai/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 13:23:58.000000 yeagerai-agent-0.0.35/yeagerai/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.571943 yeagerai-agent-0.0.35/yeagerai/agent/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       56 2023-04-10 14:29:05.000000 yeagerai-agent-0.0.35/yeagerai/agent/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1161 2023-04-09 18:33:12.000000 yeagerai-agent-0.0.35/yeagerai/agent/master_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.35/yeagerai/agent/output_parser.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.35/yeagerai/agent/prompt_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4221 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.35/yeagerai/agent/yeagerai_agent.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.571943 yeagerai-agent-0.0.35/yeagerai/interfaces/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-06 00:28:34.000000 yeagerai-agent-0.0.35/yeagerai/interfaces/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.571943 yeagerai-agent-0.0.35/yeagerai/interfaces/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      103 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.35/yeagerai/interfaces/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.35/yeagerai/interfaces/callbacks/local_file_system_n_git.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2684 2023-04-09 21:19:00.000000 yeagerai-agent-0.0.35/yeagerai/interfaces/cli.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.571943 yeagerai-agent-0.0.35/yeagerai/memory/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       61 2023-04-10 14:29:33.000000 yeagerai-agent-0.0.35/yeagerai/memory/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.571943 yeagerai-agent-0.0.35/yeagerai/memory/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       80 2023-04-10 14:29:46.000000 yeagerai-agent-0.0.35/yeagerai/memory/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.35/yeagerai/memory/callbacks/session_memory_handler.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.35/yeagerai/memory/yeagerai_context.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.571943 yeagerai-agent-0.0.35/yeagerai/toolkit/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      541 2023-04-10 14:28:39.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.571943 yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_mocked_tests/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:37:27.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_mocked_tests/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4106 2023-04-10 14:30:31.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2628 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests_master_prompt.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.571943 yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_source/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 16:52:27.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_source/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1725 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4952 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_source/create_tool_source.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.575943 yeagerai-agent-0.0.35/yeagerai/toolkit/design_solution_sketch/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:37:07.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/design_solution_sketch/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2842 2023-04-10 14:32:50.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3263 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-09 13:24:39.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/yeagerai_tool.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      589 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.35/yeagerai/toolkit/yeagerai_toolkit.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:38:59.575943 yeagerai-agent-0.0.35/yeagerai_agent.egg-info/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:38:59.000000 yeagerai-agent-0.0.35/yeagerai_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1426 2023-04-10 14:38:59.000000 yeagerai-agent-0.0.35/yeagerai_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-10 14:38:59.000000 yeagerai-agent-0.0.35/yeagerai_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       64 2023-04-10 14:38:59.000000 yeagerai-agent-0.0.35/yeagerai_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       47 2023-04-10 14:38:59.000000 yeagerai-agent-0.0.35/yeagerai_agent.egg-info/requires.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-10 14:38:59.000000 yeagerai-agent-0.0.35/yeagerai_agent.egg-info/top_level.txt
```

### Comparing `yeagerai-agent-0.0.34/LICENSE` & `yeagerai-agent-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/PKG-INFO` & `yeagerai-agent-0.0.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.34
+Version: 0.0.35
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.34/README.md` & `yeagerai-agent-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/setup.py` & `yeagerai-agent-0.0.35/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="yeagerai-agent",
-    version="0.0.34",
+    version="0.0.35",
     description="The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.",
     author="YeagerAI LLC",
     author_email="jm@yeager.ai",
     packages=find_packages(),
     install_requires=[
         "langchain",
         "openai",
```

### Comparing `yeagerai-agent-0.0.34/yeagerai/agent/master_template.py` & `yeagerai-agent-0.0.35/yeagerai/agent/master_template.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/agent/output_parser.py` & `yeagerai-agent-0.0.35/yeagerai/agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/agent/prompt_template.py` & `yeagerai-agent-0.0.35/yeagerai/agent/prompt_template.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/agent/yeagerai_agent.py` & `yeagerai-agent-0.0.35/yeagerai/agent/yeagerai_agent.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/interfaces/callbacks/local_file_system_n_git.py` & `yeagerai-agent-0.0.35/yeagerai/interfaces/callbacks/local_file_system_n_git.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/interfaces/cli.py` & `yeagerai-agent-0.0.35/yeagerai/interfaces/cli.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/memory/callbacks/session_memory_handler.py` & `yeagerai-agent-0.0.35/yeagerai/memory/callbacks/session_memory_handler.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/memory/yeagerai_context.py` & `yeagerai-agent-0.0.35/yeagerai/memory/yeagerai_context.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/toolkit/__init__.py` & `yeagerai-agent-0.0.35/yeagerai/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py` & `yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/create_tool_source.py` & `yeagerai-agent-0.0.35/yeagerai/toolkit/create_tool_source/create_tool_source.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai/toolkit/yeagerai_toolkit.py` & `yeagerai-agent-0.0.35/yeagerai/toolkit/yeagerai_toolkit.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.34/yeagerai_agent.egg-info/PKG-INFO` & `yeagerai-agent-0.0.35/yeagerai_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.34
+Version: 0.0.35
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.34/yeagerai_agent.egg-info/SOURCES.txt` & `yeagerai-agent-0.0.35/yeagerai_agent.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -14,16 +14,22 @@
 yeagerai/memory/__init__.py
 yeagerai/memory/yeagerai_context.py
 yeagerai/memory/callbacks/__init__.py
 yeagerai/memory/callbacks/session_memory_handler.py
 yeagerai/toolkit/__init__.py
 yeagerai/toolkit/yeagerai_tool.py
 yeagerai/toolkit/yeagerai_toolkit.py
+yeagerai/toolkit/create_tool_mocked_tests/__init__.py
+yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py
+yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests_master_prompt.py
 yeagerai/toolkit/create_tool_source/__init__.py
 yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
 yeagerai/toolkit/create_tool_source/create_tool_source.py
+yeagerai/toolkit/design_solution_sketch/__init__.py
+yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py
+yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py
 yeagerai_agent.egg-info/PKG-INFO
 yeagerai_agent.egg-info/SOURCES.txt
 yeagerai_agent.egg-info/dependency_links.txt
 yeagerai_agent.egg-info/entry_points.txt
 yeagerai_agent.egg-info/requires.txt
 yeagerai_agent.egg-info/top_level.txt
```

