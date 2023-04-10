# Comparing `tmp/openai_copilot-0.1.0.tar.gz` & `tmp/openai_copilot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_copilot-0.1.0.tar", max compression
+gzip compressed data, was "openai_copilot-0.2.0.tar", max compression
```

## Comparing `openai_copilot-0.1.0.tar` & `openai_copilot-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-03-25 14:19:56.857428 openai_copilot-0.1.0/LICENSE
--rw-r--r--   0        0        0     2768 2023-03-25 15:07:21.850702 openai_copilot-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-25 14:19:56.868078 openai_copilot-0.1.0/openai_copilot/__init__.py
--rw-r--r--   0        0        0     2855 2023-03-25 15:08:01.971660 openai_copilot-0.1.0/openai_copilot/agent.py
--rw-r--r--   0        0        0     1041 2023-03-25 14:44:49.028356 openai_copilot-0.1.0/openai_copilot/cli.py
--rw-r--r--   0        0        0      671 2023-03-25 15:08:13.458787 openai_copilot-0.1.0/openai_copilot/llm.py
--rw-r--r--   0        0        0      669 2023-03-25 14:41:27.382359 openai_copilot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 openai_copilot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-25 14:19:56.857428 openai_copilot-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2968 2023-04-10 14:40:42.139625 openai_copilot-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 14:19:56.868078 openai_copilot-0.2.0/openai_copilot/__init__.py
+-rw-r--r--   0        0        0     2857 2023-04-10 14:19:03.562584 openai_copilot-0.2.0/openai_copilot/agent.py
+-rw-r--r--   0        0        0     1059 2023-04-10 14:39:24.193477 openai_copilot-0.2.0/openai_copilot/cli.py
+-rw-r--r--   0        0        0      671 2023-03-25 15:08:13.458787 openai_copilot-0.2.0/openai_copilot/llm.py
+-rw-r--r--   0        0        0      672 2023-04-10 14:41:11.434065 openai_copilot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3659 1970-01-01 00:00:00.000000 openai_copilot-0.2.0/PKG-INFO
```

### Comparing `openai_copilot-0.1.0/LICENSE` & `openai_copilot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.1.0/README.md` & `openai_copilot-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -32,31 +32,31 @@
 Usage: openai-copilot [OPTIONS]
 
   Your life Copilot powered by OpenAI
 
 Options:
   --version          Show the version and exit.
   --verbose          Enable verbose information of copilot execution steps
-  --model TEXT       OpenAI model to use for copilot execution, default is
+  --model MODEL      OpenAI model to use for copilot execution, default is
                      gpt-3.5-turbo
   --enable-terminal  Enable Copilot to run programs within terminal. Enable
                      with caution since Copilot may execute inappropriate
                      commands
   --help             Show this message and exit.
 ```
 
-Here is a conversation sample:
+Here is a conversation sample (user inputs are after `>>>`)):
 
 ```sh
 # openai-copilot
->>> : What is OpenAI?
-OpenAI is a research organization consisting of the for-profit corporation OpenAI LP and its parent company, the non-profit OpenAI Inc. The company aims to conduct cutting-edge research and development in artificial intelligence (AI) in a way that benefits humanity as a whole. Some notable achievements of OpenAI include the development of advanced language models such as GPT-3 and the creation of AI agents that are capable of playing complex games such as Dota 2.
->>> : What is its latest product?
-OpenAI's latest system is GPT-4, which is OpenAI's most advanced system that produces safer and more useful language models. Additionally, the company also has an API platform that offers their latest models and guides for safety best practices.
->>> :
+>>> What is OpenAI?
+OpenAI is an artificial intelligence research laboratory consisting of the for-profit corporation OpenAI LP and its parent company, the non-profit OpenAI Inc. The company is dedicated to advancing digital intelligence in a way that is safe and beneficial for humanity as a whole. OpenAI was founded in 2015 by a group of technology leaders including Elon Musk, Sam Altman, Greg Brockman, and Ilya Sutskever. Its mission is to develop and promote friendly AI for the betterment of all humans.
+>>> What are the differences between GPT-4 and GPT-3.5?
+According to my search results, one of the main differences between GPT-4 and GPT-3.5 is that while GPT-3.5 is a text-to-text model, GPT-4 is more of a data-to-text model. Additionally, GPT-4 has the advantage of providing more creative replies to prompts. However, it's important to note that GPT-4 is not yet released and there is limited information available about it.
+>>>
 ```
 
 ## Contribution
 
 The project is opensource at github [feiskyer/openai-copilot](https://github.com/feiskyer/openai-copilot) with Apache License.
 
 If you would like to contribute to the project, please follow these guidelines:
```

### Comparing `openai_copilot-0.1.0/openai_copilot/agent.py` & `openai_copilot-0.2.0/openai_copilot/agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 from langchain.agents import Tool, load_tools
 from langchain.memory import ConversationBufferMemory
 from langchain.agents import initialize_agent
 from langchain.tools.python.tool import PythonREPLTool
 from langchain.utilities import GoogleSearchAPIWrapper
 
 
-os.environ["LANGCHAIN_HANDLER"] = "langchain"
-
-
 class CopilotLLM:
     '''Wrapper for LLM chain.'''
 
     def __init__(self, verbose=True, model="gpt-3.5-turbo", additional_tools=None, enable_terminal=False):
         '''Initialize the LLM chain.'''
         self.chain = get_chat_chain(verbose, model, additional_tools=additional_tools,
                                     enable_terminal=enable_terminal)
@@ -30,22 +27,23 @@
                 return str(e).split("Could not parse LLM output:")[1]
             else:
                 raise e
 
 
 def get_chat_chain(verbose=True, model="gpt-3.5-turbo", additional_tools=None,
                    agent="chat-conversational-react-description",
-                   enable_terminal=False, max_iterations=30):
+                   enable_terminal=False, max_iterations=30,
+                   max_tokens=1024):
     '''Initialize the LLM chain with useful tools.'''
     if os.getenv("OPENAI_API_TYPE") == "azure":
         if model == "gpt-3.5-turbo":
             model = "gpt-35-turbo"
-        llm = ChatOpenAI(engine=model, max_tokens=512)
+        llm = ChatOpenAI(engine=model, max_tokens=max_tokens)
     else:
-        llm = ChatOpenAI(model=model, max_tokens=512)
+        llm = ChatOpenAI(model=model, max_tokens=max_tokens)
 
     default_tools = ["human"]
     if enable_terminal:
         default_tools += ["terminal"]
     tools = load_tools(default_tools, llm)
 
     if os.getenv("OPENAI_COPILOT_ENABLE_PYTHON"):
```

### Comparing `openai_copilot-0.1.0/openai_copilot/cli.py` & `openai_copilot-0.2.0/openai_copilot/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 @click.option("--enable-terminal", is_flag=True, default=False, help="Enable Copilot to run programs within terminal. Enable with caution since Copilot may execute inappropriate commands")
 def cli(verbose, model, enable_terminal):
     '''Your life Copilot powered by OpenAI'''
     init_openai()
     chain = CopilotLLM(
         verbose=verbose, model=model, enable_terminal=enable_terminal)
     while True:
-        instructions = click.prompt(">>> ")
+        instructions = click.prompt(">>>", prompt_suffix=' ')
         result = chain.run(instructions)
         click.echo(click.style(result, fg='green'))
 
 
 def main():
     cli()
```

### Comparing `openai_copilot-0.1.0/openai_copilot/llm.py` & `openai_copilot-0.2.0/openai_copilot/llm.py`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.1.0/pyproject.toml` & `openai_copilot-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "openai-copilot"
-version = "0.1.0"
+version = "0.2.0"
 description = "OpenAI Copilot"
 authors = ["Pengfei Ni <feiskyer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_copilot"}]
 homepage = "https://github.com/feiskyer/openai-copilot"
 repository = "https://github.com/feiskyer/openai-copilot"
 keywords = ["copilot", "openai", "chatgpt"]
 
 [tool.poetry.scripts]
 openai-copilot = 'openai_copilot.cli:main'
 
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = ">=3.10,<4"
 langchain = ">=0.0.120"
 requests = ">=2.28"
 openai = ">=0.27"
 google-api-python-client = ">=2.80.0"
 click = ">=8.1.0"
 
 [build-system]
```

### Comparing `openai_copilot-0.1.0/PKG-INFO` & `openai_copilot-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openai-copilot
-Version: 0.1.0
+Version: 0.2.0
 Summary: OpenAI Copilot
 Home-page: https://github.com/feiskyer/openai-copilot
 Keywords: copilot,openai,chatgpt
 Author: Pengfei Ni
 Author-email: feiskyer@gmail.com
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.0)
 Requires-Dist: google-api-python-client (>=2.80.0)
 Requires-Dist: langchain (>=0.0.120)
 Requires-Dist: openai (>=0.27)
@@ -52,31 +52,31 @@
 Usage: openai-copilot [OPTIONS]
 
   Your life Copilot powered by OpenAI
 
 Options:
   --version          Show the version and exit.
   --verbose          Enable verbose information of copilot execution steps
-  --model TEXT       OpenAI model to use for copilot execution, default is
+  --model MODEL      OpenAI model to use for copilot execution, default is
                      gpt-3.5-turbo
   --enable-terminal  Enable Copilot to run programs within terminal. Enable
                      with caution since Copilot may execute inappropriate
                      commands
   --help             Show this message and exit.
 ```
 
-Here is a conversation sample:
+Here is a conversation sample (user inputs are after `>>>`)):
 
 ```sh
 # openai-copilot
->>> : What is OpenAI?
-OpenAI is a research organization consisting of the for-profit corporation OpenAI LP and its parent company, the non-profit OpenAI Inc. The company aims to conduct cutting-edge research and development in artificial intelligence (AI) in a way that benefits humanity as a whole. Some notable achievements of OpenAI include the development of advanced language models such as GPT-3 and the creation of AI agents that are capable of playing complex games such as Dota 2.
->>> : What is its latest product?
-OpenAI's latest system is GPT-4, which is OpenAI's most advanced system that produces safer and more useful language models. Additionally, the company also has an API platform that offers their latest models and guides for safety best practices.
->>> :
+>>> What is OpenAI?
+OpenAI is an artificial intelligence research laboratory consisting of the for-profit corporation OpenAI LP and its parent company, the non-profit OpenAI Inc. The company is dedicated to advancing digital intelligence in a way that is safe and beneficial for humanity as a whole. OpenAI was founded in 2015 by a group of technology leaders including Elon Musk, Sam Altman, Greg Brockman, and Ilya Sutskever. Its mission is to develop and promote friendly AI for the betterment of all humans.
+>>> What are the differences between GPT-4 and GPT-3.5?
+According to my search results, one of the main differences between GPT-4 and GPT-3.5 is that while GPT-3.5 is a text-to-text model, GPT-4 is more of a data-to-text model. Additionally, GPT-4 has the advantage of providing more creative replies to prompts. However, it's important to note that GPT-4 is not yet released and there is limited information available about it.
+>>>
 ```
 
 ## Contribution
 
 The project is opensource at github [feiskyer/openai-copilot](https://github.com/feiskyer/openai-copilot) with Apache License.
 
 If you would like to contribute to the project, please follow these guidelines:
```

