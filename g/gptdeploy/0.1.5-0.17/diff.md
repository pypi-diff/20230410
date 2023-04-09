# Comparing `tmp/gptdeploy-0.1.5.tar.gz` & `tmp/gptdeploy-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gptdeploy-0.1.5.tar", last modified: Tue Apr  4 17:54:26 2023, max compression
+gzip compressed data, was "dist/gptdeploy-0.17.tar", last modified: Sun Apr  9 23:47:10 2023, max compression
```

## Comparing `gptdeploy-0.1.5.tar` & `gptdeploy-0.17.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:54:26.000000 gptdeploy-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-04 17:54:26.000000 gptdeploy-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:54:26.000000 gptdeploy-0.1.5/gptdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-04 17:54:25.000000 gptdeploy-0.1.5/gptdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-04 17:54:26.000000 gptdeploy-0.1.5/gptdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 17:54:25.000000 gptdeploy-0.1.5/gptdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 17:54:25.000000 gptdeploy-0.1.5/gptdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 17:54:25.000000 gptdeploy-0.1.5/gptdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-04 17:54:25.000000 gptdeploy-0.1.5/gptdeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 17:54:26.000000 gptdeploy-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:54:26.000000 gptdeploy-0.1.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/prompt_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/prompt_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:54:26.000000 gptdeploy-0.1.5/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-04 17:54:13.000000 gptdeploy-0.1.5/src/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:47:10.000000 gptdeploy-0.17/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-09 23:46:52.000000 gptdeploy-0.17/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-04-09 23:47:10.000000 gptdeploy-0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-04-09 23:46:52.000000 gptdeploy-0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:47:10.000000 gptdeploy-0.17/gptdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-09 23:47:10.000000 gptdeploy-0.17/gptdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-09 23:46:52.000000 gptdeploy-0.17/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 23:47:10.000000 gptdeploy-0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-09 23:46:52.000000 gptdeploy-0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:47:10.000000 gptdeploy-0.17/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/key_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/prompt_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/prompt_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:47:10.000000 gptdeploy-0.17/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/utils/string_tools.py
```

### Comparing `gptdeploy-0.1.5/setup.py` & `gptdeploy-0.17/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 def read_requirements():
     with open('requirements.txt', 'r', encoding='utf-8') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 setup(
     name='gptdeploy',
-    version='0.1.5',
+    version='0.17',
     description='Use natural language interface to create, deploy and update your microservice infrastructure.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Florian Hönicke',
     author_email='florian.hoenicke@jina.ai',
     url='https://github.com/jina-ai/gptdeploy',
     packages=find_packages(),
     install_requires=read_requirements(),
     entry_points={
         'console_scripts': [
             'gptdeploy=main:main',
         ],
     },
+
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `gptdeploy-0.1.5/src/gpt.py` & `gptdeploy-0.17/src/gpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,95 @@
 import os
 from time import sleep
 from typing import List, Tuple
 
 import openai
 from openai.error import RateLimitError, Timeout
 
+from src.constants import PRICING_GPT4_PROMPT, PRICING_GPT4_GENERATION, PRICING_GPT3_5_TURBO_PROMPT, \
+    PRICING_GPT3_5_TURBO_GENERATION
 from src.prompt_system import system_base_definition
 from src.utils.io import timeout_generator_wrapper, GenerationTimeoutError
 from src.utils.string_tools import print_colored
 
-PRICING_GPT4_PROMPT = 0.03
-PRICING_GPT4_GENERATION = 0.06
-PRICING_GPT3_5_TURBO_PROMPT = 0.002
-PRICING_GPT3_5_TURBO_GENERATION = 0.002
-
-if 'OPENAI_API_KEY' not in os.environ:
-    raise Exception('You need to set OPENAI_API_KEY in your environment')
-openai.api_key = os.environ['OPENAI_API_KEY']
-
-
-try:
-    openai.ChatCompletion.create(
-        model="gpt-4",
-        messages=[{
-            "role": 'system',
-            "content": 'test'
-        }]
-    )
-    supported_model = 'gpt-4'
-    pricing_prompt = PRICING_GPT4_PROMPT
-    pricing_generation = PRICING_GPT4_GENERATION
-except openai.error.InvalidRequestError:
-    supported_model = 'gpt-3.5-turbo'
-    pricing_prompt = PRICING_GPT3_5_TURBO_PROMPT
-    pricing_generation = PRICING_GPT3_5_TURBO_GENERATION
+class GPTSession:
+    def __init__(self):
+        self.get_openai_api_key()
+        if self.is_gpt4_available():
+            self.supported_model = 'gpt-4'
+            self.pricing_prompt = PRICING_GPT4_PROMPT
+            self.pricing_generation = PRICING_GPT4_GENERATION
+        else:
+            self.supported_model = 'gpt-3.5-turbo'
+            self.pricing_prompt = PRICING_GPT3_5_TURBO_PROMPT
+            self.pricing_generation = PRICING_GPT3_5_TURBO_GENERATION
+        self.chars_prompt_so_far = 0
+        self.chars_generation_so_far = 0
+
+    def get_openai_api_key(self):
+        if 'OPENAI_API_KEY' not in os.environ:
+            raise Exception('You need to set OPENAI_API_KEY in your environment')
+        openai.api_key = os.environ['OPENAI_API_KEY']
+
+    def is_gpt4_available(self):
+        try:
+            openai.ChatCompletion.create(
+                model="gpt-4",
+                messages=[{
+                    "role": 'system',
+                    "content": 'test'
+                }]
+            )
+            return True
+        except openai.error.InvalidRequestError:
+            return False
+
+    def cost_callback(self, chars_prompt, chars_generation):
+        self.chars_prompt_so_far += chars_prompt
+        self.chars_generation_so_far += chars_generation
+        print('\n')
+        money_prompt = round(self.chars_prompt_so_far / 3.4 * self.pricing_prompt / 1000, 2)
+        money_generation = round(self.chars_generation_so_far / 3.4 * self.pricing_generation / 1000, 2)
+        print('money prompt:', f'${money_prompt}')
+        print('money generation:', f'${money_generation}')
+        print('total money:', f'${money_prompt + money_generation}')
+        print('\n')
 
-total_chars_prompt = 0
-total_chars_generation = 0
+    def get_conversation(self):
+        return _GPTConversation(self.supported_model, self.cost_callback)
 
 
-class Conversation:
-    def __init__(self, prompt_list: List[Tuple[str, str]] = None, model=supported_model):
+class _GPTConversation:
+    def __init__(self, model: str, cost_callback, prompt_list: List[Tuple[str, str]] = None):
         self.model = model
         if prompt_list is None:
             prompt_list = [('system', system_base_definition)]
         self.prompt_list = prompt_list
+        self.cost_callback = cost_callback
         print_colored('system', system_base_definition, 'magenta')
 
     def query(self, prompt: str):
         print_colored('user', prompt, 'blue')
         self.prompt_list.append(('user', prompt))
         response = self.get_response(self.prompt_list)
         self.prompt_list.append(('assistant', response))
         return response
 
+    def get_response_from_stream(self, response_generator):
+        response_generator_with_timeout = timeout_generator_wrapper(response_generator, 10)
+        complete_string = ''
+        for chunk in response_generator_with_timeout:
+            delta = chunk['choices'][0]['delta']
+            if 'content' in delta:
+                content = delta['content']
+                print_colored('' if complete_string else 'assistent', content, 'green', end='')
+                complete_string += content
+        return complete_string
+
     def get_response(self, prompt_list: List[Tuple[str, str]]):
-        global total_chars_prompt, total_chars_generation
         for i in range(10):
             try:
                 response_generator = openai.ChatCompletion.create(
                     temperature=0,
                     max_tokens=2_000,
                     model=self.model,
                     stream=True,
@@ -67,31 +97,21 @@
                         {
                             "role": prompt[0],
                             "content": prompt[1]
                         }
                         for prompt in prompt_list
                     ]
                 )
-                response_generator_with_timeout = timeout_generator_wrapper(response_generator, 10)
-                total_chars_prompt += sum(len(prompt[1]) for prompt in prompt_list)
-                complete_string = ''
-                for chunk in response_generator_with_timeout:
-                    delta = chunk['choices'][0]['delta']
-                    if 'content' in delta:
-                        content = delta['content']
-                        print_colored('' if complete_string else 'assistent', content, 'green', end='')
-                        complete_string += content
-                        total_chars_generation += len(content)
-                print('\n')
-                money_prompt = round(total_chars_prompt / 3.4 * pricing_prompt / 1000, 2)
-                money_generation = round(total_chars_generation / 3.4 * pricing_generation / 1000, 2)
-                print('money prompt:', f'${money_prompt}')
-                print('money generation:', f'${money_generation}')
-                print('total money:', f'${money_prompt + money_generation}')
-                print('\n')
-                return complete_string
+
+                complete_string = self.get_response_from_stream(response_generator)
+
             except (RateLimitError, Timeout, ConnectionError, GenerationTimeoutError) as e:
                 print(e)
-                print('retrying')
+                print('retrying, be aware that this affects the cost calculation')
                 sleep(3)
                 continue
+            chars_prompt = sum(len(prompt[1]) for prompt in prompt_list)
+            chars_generation = len(complete_string)
+            self.cost_callback(chars_prompt, chars_generation)
+            return complete_string
         raise Exception('Failed to get response')
+
```

### Comparing `gptdeploy-0.1.5/src/jina_cloud.py` & `gptdeploy-0.17/src/jina_cloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 import hashlib
 import json
 import os
-import subprocess
 import re
-from argparse import Namespace
+import subprocess
+import webbrowser
 from pathlib import Path
 
 import hubble
 from hubble.executor.helper import upload_file, archive_package, get_request_header
 from jcloud.flow import CloudFlow
-from jina import Flow
 
 
+def redirect_callback(href):
+    print(
+        f'You need login to Jina first to use GPTDeploy\n'
+        f'Please open this link if it does not open automatically in your browser: {href}'
+    )
+    webbrowser.open(href, new=0, autoraise=True)
+
+
+def jina_auth_login():
+    try:
+        hubble.Client(jsonify=True).get_user_info(log_error=False)
+    except hubble.AuthenticationRequiredError:
+        hubble.login(prompt='login', redirect_callback=redirect_callback)
+
 
 def push_executor(dir_path):
     dir_path = Path(dir_path)
 
     md5_hash = hashlib.md5()
     bytesio = archive_package(dir_path)
     content = bytesio.getvalue()
@@ -62,39 +75,38 @@
 
 
 def deploy_on_jcloud(flow_yaml):
     cloud_flow = CloudFlow(path=flow_yaml)
     return cloud_flow.__enter__().endpoints['gateway']
 
 
-
 def deploy_flow(executor_name, dest_folder):
     flow = f'''
 jtype: Flow
 with:
   name: nowapi
   env:
     JINA_LOG_LEVEL: DEBUG
 jcloud:
   version: 3.14.2.dev18
   labels:
     creator: microchain
-  name: mybelovedocrflow
+  name: gptdeploy
 executors:
   - name: {executor_name.lower()}
     uses: jinaai+docker://{get_user_name()}/{executor_name}:latest
     env:
       JINA_LOG_LEVEL: DEBUG
     jcloud:
       resources:
         instance: C2
         capacity: spot
 '''
     full_flow_path = os.path.join(dest_folder,
-                     'flow.yml')
+                                  'flow.yml')
     with open(full_flow_path, 'w') as f:
         f.write(flow)
 
     # print('try local execution')
     # flow = Flow.load_config(full_flow_path)
     # with flow:
     #     pass
@@ -106,21 +118,21 @@
     lines = file_content.split('\n')
     for index, line in enumerate(lines):
         if 'Client(' in line:
             lines[index] = replacement
             break
     return '\n'.join(lines)
 
+
 def update_client_line_in_file(file_path, host):
     with open(file_path, 'r') as file:
         content = file.read()
 
     replaced_content = replace_client_line(content, f"client = Client(host='{host}')")
 
-
     with open(file_path, 'w') as file:
         file.write(replaced_content)
 
 
 def process_error_message(error_message):
     lines = error_message.split('\n')
     relevant_lines = []
@@ -133,17 +145,16 @@
             last_matching_line_index = index
 
     if last_matching_line_index is not None:
         relevant_lines = lines[last_matching_line_index:]
 
     return '\n'.join(relevant_lines[-25:])
 
-def build_docker(path):
-
 
+def build_docker(path):
     # The command to build the Docker image
     cmd = f"docker build -t micromagic {path}"
 
     # Run the command and capture the output
     process = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     stdout, stderr = process.communicate()
 
@@ -151,8 +162,7 @@
     if process.returncode != 0:
         error_message = stderr.decode("utf-8")
         relevant_error_message = process_error_message(error_message)
         return relevant_error_message
     else:
         print("Docker build completed successfully.")
         return ''
-
```

### Comparing `gptdeploy-0.1.5/src/prompt_system.py` & `gptdeploy-0.17/src/prompt_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,62 +8,57 @@
 ```python
 # this executor binary files as input and returns the length of each binary file as output
 from jina import Executor, requests, DocumentArray, Document
 class MyInfoExecutor(Executor):
     def __init__(self, **kwargs):
         super().__init__()
 
-    @requests(on='/process') # this decorator is needed for every executor endpoint
+    @requests() # each executor must have exactly this decorator without parameters
     def foo(self, docs: DocumentArray, **kwargs) => DocumentArray:
         for d in docs:
             d.load_uri_to_blob()
-            d.tags['my_info'] = {'byte_length': len(d.blob)} # tags can only be a flat dictionary where keys are strings and values are strings, ints, floats, or bools
             d.blob = None
         return docs
 ```
 
 An executor gets a DocumentArray as input and returns a DocumentArray as output. 
 '''
 
-docarray_example = '''
+docarray_example = f'''
 A DocumentArray is a python class that can be seen as a list of Documents.
 A Document is a python class that represents a single document.
 Here is the protobuf definition of a Document:
 
-message DocumentProto {
+message DocumentProto {{
   // A hexdigest that represents a unique document ID
   string id = 1;
 
-  oneof content {
+  oneof content {{
     // the raw binary content of this document, which often represents the original document when comes into jina
     bytes blob = 2;
 
     // the ndarray of the image/audio/video document
     NdArrayProto tensor = 3;
 
     // a text document
     string text = 4;
-  }
+  }}
 
   // a uri of the document is a remote url starts with http or https or data URI scheme
   string uri = 5;
 
   // list of the sub-documents of this document (recursive structure)
   repeated DocumentProto chunks = 6;
 
   // the matched documents on the same level (recursive structure)
   repeated DocumentProto matches = 7;
 
   // the embedding of this document
   NdArrayProto embedding = 8;
-
-  // a structured data value, consisting of field which map to dynamically typed values.
-  google.protobuf.Struct tags = 9;
-
-}
+}}
 
 Here is an example of how a DocumentArray can be defined:
 
 from jina import DocumentArray, Document
 
 d1 = Document(text='hello')
 
@@ -72,24 +67,27 @@
 response = requests.get(url)
 obj_data = response.content
 d2 = Document(blob=obj_data) # blob is bytes like b'\\x89PNG\\r\\n\\x1a\\n\
 
 d3 = Document(tensor=numpy.array([1, 2, 3]), chunks=[Document(uri=/local/path/to/file)]
 d4 = Document(
    uri='https://docs.docarray.org/img/logo.png',
-   tags={'foo': 'bar'},
 )
 d5 = Document()
 d5.tensor = np.ones((2,4))
 d5.uri = 'https://audio.com/audio.mp3'
 d6 = Document()
 d6.blob # like b'RIFF\\x00\\x00\\x00\\x00WAVEfmt \\x10\\x00...'
 docs = DocumentArray([
    d1, d2, d3, d4
 ])
+d7 = Document()
+d7.text = 'test string'
+d8 = Document()
+d8.text = json.dumps([{{"id": "1", "text": ["hello", 'test']}}, {{"id": "2", "text": "world"}}])
 # the document has a helper function load_uri_to_blob:
 # For instance, d4.load_uri_to_blob() downloads the file from d4.uri and stores it in d4.blob. 
 # If d4.uri was something like 'https://website.web/img.jpg', then d4.blob would be something like  b'\\xff\\xd8\\xff\\xe0\\x00\\x10JFIF\\x00\\x01\\x01... 
 '''
 
 
 client_example = f'''
@@ -98,15 +96,15 @@
 
 **client.py**
 ```python
 from jina import Client, Document, DocumentArray
 client = Client(host='{FLOW_URL_PLACEHOLDER}')
 d = Document(uri='...')
 d.load_uri_to_blob()
-response = client.post('/process', inputs=DocumentArray([d]))
+response = client.post('/', inputs=DocumentArray([d])) # the client must be called on '/'
 print(response[0].text)
 ```
 '''
 
 
 system_base_definition = f'''
 You are a principal engineer working at Jina - an open source company."
```

### Comparing `gptdeploy-0.1.5/src/prompt_tasks.py` & `gptdeploy-0.17/src/prompt_tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     REQUIREMENTS_FILE_TAG, TEST_EXECUTOR_FILE_TAG
 
 
 def general_guidelines():
     return (
         "The code you write is production ready. "
         "Every file starts with comments describing what the code is doing before the first import. "
-        "Comments can only be written between tags. "
+        "Comments can only be written within code blocks. "
         "Then all imports are listed. "
         "It is important to import all modules that could be needed in the executor code. "
         "Always import: "
         "from jina import Executor, DocumentArray, Document, requests "
         "Start from top-level and then fully implement all methods. "
         "\n"
     )
@@ -42,21 +42,23 @@
 
 def test_executor_file_task(executor_name, test_scenario):
     return _task(
         "Write a small unit test for the executor. "
         "Start the test with an extensive comment about the test case. "
         + (
             f"Write a single test case that tests the following scenario: '{test_scenario}'. "
+            f"In case the test scenario is not precise enough, test the most general case without any assumptions."
             if test_scenario else ""
         )
         + "Use the following import to import the executor: "
           f"from executor import {executor_name} "
         + not_allowed()
-        + "The test is not allowed to open local files. "
-        + "The test is not allowed to mock a function of the executor. ",
+        + "The test must not open local files. "
+        + "The test must not mock a function of the executor. "
+        + "The test must not use other data than the one provided in the test scenario. ",
         TEST_EXECUTOR_FILE_TAG,
         TEST_EXECUTOR_FILE_NAME
     )
 
 def requirements_file_task():
     return _task(
         "Write the content of the requirements.txt file. "
@@ -121,15 +123,16 @@
         f"Write the whole content of {file_name} - even if you decided to change only a small thing or even nothing. ",
         tag_name,
         file_name
     )
 
 def not_allowed():
     return '''
-The executor is not allowed to use the GPU.
-The executor is not allowed to access a database.
-The executor is not allowed to access a display.
-The executor is not allowed to access external apis. 
-The executor is not allowed to load data from the local file system it did not create.
-The executor is not allowed to use a pre-trained model.
-The executor is not allowed to train a model.
+The executor must not use the GPU.
+The executor must not access a database.
+The executor must not access a display.
+The executor must not access external apis except unless it is explicitly mentioned in the description or test case (e.g. by mentioning the api that should be used or by providing a URL to access the data). 
+The executor must not load data from the local file system unless it was created by the executor itself.
+The executor must not use a pre-trained model unless it is explicitly mentioned in the description.
+The executor must not train a model.
+The executor must not use Document.tags.
 '''
```

### Comparing `gptdeploy-0.1.5/src/server.py` & `gptdeploy-0.17/src/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from fastapi import FastAPI
 from fastapi.exceptions import RequestValidationError
-from jina import Flow
-from pydantic import BaseModel, HttpUrl
+from pydantic import BaseModel
 from typing import Optional, Dict
 
 from starlette.middleware.cors import CORSMiddleware
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 from main import main
```

### Comparing `gptdeploy-0.1.5/src/utils/io.py` & `gptdeploy-0.17/src/utils/io.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,18 +30,8 @@
                     future = executor.submit(next, gen)
                     yield future.result(timeout=timeout)
             except StopIteration:
                 break
             except concurrent.futures.TimeoutError:
                 raise GenerationTimeoutError(f"Generation took longer than {timeout} seconds")
 
-    return wrapper()
-
-# def my_generator():
-#     for i in range(10):
-#         sleep(3)
-#         yield 1
-#
-#
-# my_generator_with_timeout = timeout_generator_wrapper(my_generator, 2.9)
-# for item in my_generator_with_timeout():
-#     print(item)
+    return wrapper()
```

### Comparing `gptdeploy-0.1.5/src/utils/string_tools.py` & `gptdeploy-0.17/src/utils/string_tools.py`

 * *Files identical despite different names*

