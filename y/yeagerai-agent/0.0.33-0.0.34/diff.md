# Comparing `tmp/yeagerai-agent-0.0.33.tar.gz` & `tmp/yeagerai-agent-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeagerai-agent-0.0.33.tar", last modified: Mon Apr 10 14:24:40 2023, max compression
+gzip compressed data, was "yeagerai-agent-0.0.34.tar", last modified: Mon Apr 10 14:33:19 2023, max compression
```

## Comparing `yeagerai-agent-0.0.33.tar` & `yeagerai-agent-0.0.34.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-09 11:08:36.000000 yeagerai-agent-0.0.33/LICENSE
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2731 2023-04-10 01:09:09.000000 yeagerai-agent-0.0.33/README.md
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/setup.cfg
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1199 2023-04-10 14:23:44.000000 yeagerai-agent-0.0.33/setup.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.502146 yeagerai-agent-0.0.33/yeagerai/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 13:23:58.000000 yeagerai-agent-0.0.33/yeagerai/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.502146 yeagerai-agent-0.0.33/yeagerai/agent/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       42 2023-04-09 14:58:07.000000 yeagerai-agent-0.0.33/yeagerai/agent/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1161 2023-04-09 18:33:12.000000 yeagerai-agent-0.0.33/yeagerai/agent/master_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/agent/output_parser.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/agent/prompt_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4197 2023-04-09 22:21:35.000000 yeagerai-agent-0.0.33/yeagerai/agent/yeagerai_agent.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/interfaces/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-06 00:28:34.000000 yeagerai-agent-0.0.33/yeagerai/interfaces/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/interfaces/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       65 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/interfaces/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/interfaces/callbacks/local_file_system_n_git.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2684 2023-04-09 21:19:00.000000 yeagerai-agent-0.0.33/yeagerai/interfaces/cli.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/memory/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       46 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/memory/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/memory/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       55 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/memory/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/memory/callbacks/session_memory_handler.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/memory/yeagerai_context.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/toolkit/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      461 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 16:52:27.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1725 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4878 2023-04-09 22:02:27.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/create_tool_source.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-09 13:24:39.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/yeagerai_tool.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      589 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.33/yeagerai/toolkit/yeagerai_toolkit.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:24:40.506146 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1020 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       64 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/entry_points.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       47 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/requires.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-10 14:24:40.000000 yeagerai-agent-0.0.33/yeagerai_agent.egg-info/top_level.txt
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-09 11:08:36.000000 yeagerai-agent-0.0.34/LICENSE
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2731 2023-04-10 01:09:09.000000 yeagerai-agent-0.0.34/README.md
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/setup.cfg
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1199 2023-04-10 14:33:04.000000 yeagerai-agent-0.0.34/setup.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 13:23:58.000000 yeagerai-agent-0.0.34/yeagerai/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/agent/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       56 2023-04-10 14:29:05.000000 yeagerai-agent-0.0.34/yeagerai/agent/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1161 2023-04-09 18:33:12.000000 yeagerai-agent-0.0.34/yeagerai/agent/master_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/agent/output_parser.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/agent/prompt_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4221 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.34/yeagerai/agent/yeagerai_agent.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/interfaces/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-06 00:28:34.000000 yeagerai-agent-0.0.34/yeagerai/interfaces/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/interfaces/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      103 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.34/yeagerai/interfaces/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/interfaces/callbacks/local_file_system_n_git.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2684 2023-04-09 21:19:00.000000 yeagerai-agent-0.0.34/yeagerai/interfaces/cli.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/memory/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       61 2023-04-10 14:29:33.000000 yeagerai-agent-0.0.34/yeagerai/memory/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/memory/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       80 2023-04-10 14:29:46.000000 yeagerai-agent-0.0.34/yeagerai/memory/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/memory/callbacks/session_memory_handler.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/memory/yeagerai_context.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/toolkit/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      541 2023-04-10 14:28:39.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 16:52:27.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1725 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4952 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/create_tool_source.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-09 13:24:39.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/yeagerai_tool.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      589 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.34/yeagerai/toolkit/yeagerai_toolkit.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:33:19.875991 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1020 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       64 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       47 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/requires.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-10 14:33:19.000000 yeagerai-agent-0.0.34/yeagerai_agent.egg-info/top_level.txt
```

### Comparing `yeagerai-agent-0.0.33/LICENSE` & `yeagerai-agent-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/PKG-INFO` & `yeagerai-agent-0.0.34/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.33
+Version: 0.0.34
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.33/README.md` & `yeagerai-agent-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/setup.py` & `yeagerai-agent-0.0.34/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="yeagerai-agent",
-    version="0.0.33",
+    version="0.0.34",
     description="The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.",
     author="YeagerAI LLC",
     author_email="jm@yeager.ai",
     packages=find_packages(),
     install_requires=[
         "langchain",
         "openai",
```

### Comparing `yeagerai-agent-0.0.33/yeagerai/agent/master_template.py` & `yeagerai-agent-0.0.34/yeagerai/agent/master_template.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/yeagerai/agent/output_parser.py` & `yeagerai-agent-0.0.34/yeagerai/agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/yeagerai/agent/prompt_template.py` & `yeagerai-agent-0.0.34/yeagerai/agent/prompt_template.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/yeagerai/agent/yeagerai_agent.py` & `yeagerai-agent-0.0.34/yeagerai/agent/yeagerai_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,17 @@
         self.agent = LLMSingleActionAgent(
             llm_chain=self.llm_chain,
             output_parser=self.output_parser,
             stop=["\nObservation:"],
             allowed_tools=tool_names,
         )
         self.agent_executor = AgentExecutor.from_agent_and_tools(
-            agent=self.agent, tools=self.yeager_kit.get_tools(), verbose=True,
+            agent=self.agent,
+            tools=self.yeager_kit.get_tools(),
+            verbose=True,
         )
 
     def run(self, input):
         try:
             return self.agent_executor.run(input)
         except ValueError:
             return "Final answer: some issues were found while parsing the output."
```

### Comparing `yeagerai-agent-0.0.33/yeagerai/interfaces/callbacks/local_file_system_n_git.py` & `yeagerai-agent-0.0.34/yeagerai/interfaces/callbacks/local_file_system_n_git.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/yeagerai/interfaces/cli.py` & `yeagerai-agent-0.0.34/yeagerai/interfaces/cli.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/yeagerai/memory/callbacks/session_memory_handler.py` & `yeagerai-agent-0.0.34/yeagerai/memory/callbacks/session_memory_handler.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/yeagerai/memory/yeagerai_context.py` & `yeagerai-agent-0.0.34/yeagerai/memory/yeagerai_context.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py` & `yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/yeagerai/toolkit/create_tool_source/create_tool_source.py` & `yeagerai-agent-0.0.34/yeagerai/toolkit/create_tool_source/create_tool_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 from langchain.chat_models import ChatOpenAI
 from langchain import PromptTemplate, LLMChain
 from langchain.prompts.chat import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
 )
-from .create_tool_master_prompt import CREATE_TOOL_MASTER_PROMPT
+from yeagerai.toolkit.create_tool_source.create_tool_master_prompt import (
+    CREATE_TOOL_MASTER_PROMPT,
+)
 
 
 class CreateToolSourceAPIWrapper(BaseModel):
     session_path: str
     model_name: str
     request_timeout: int
     streaming: bool
@@ -24,15 +26,17 @@
 
     def run(self, solution_sketch_n_tool_tests: str) -> str:
         # Split the solution sketch and tool tests
         try:
             solution_sketch = solution_sketch_n_tool_tests.split(
                 "######SPLIT_TOKEN########"
             )[0]
-            tool_tests = solution_sketch_n_tool_tests.split("######SPLIT_TOKEN########")[1]
+            tool_tests = solution_sketch_n_tool_tests.split(
+                "######SPLIT_TOKEN########"
+            )[1]
         except IndexError:
             return "You have not provided the split token ######SPLIT_TOKEN########, retry it providing it between the solution sketch and the tool tests."
         # Initialize ChatOpenAI with API key and model name
         chat = ChatOpenAI(
             openai_api_key=self.openai_api_key,
             model_name=self.model_name,
             request_timeout=self.request_timeout,
```

### Comparing `yeagerai-agent-0.0.33/yeagerai/toolkit/yeagerai_toolkit.py` & `yeagerai-agent-0.0.34/yeagerai/toolkit/yeagerai_toolkit.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.33/yeagerai_agent.egg-info/PKG-INFO` & `yeagerai-agent-0.0.34/yeagerai_agent.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.33
+Version: 0.0.34
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.33/yeagerai_agent.egg-info/SOURCES.txt` & `yeagerai-agent-0.0.34/yeagerai_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

