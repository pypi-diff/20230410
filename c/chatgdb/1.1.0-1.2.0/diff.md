# Comparing `tmp/chatgdb-1.1.0.tar.gz` & `tmp/chatgdb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgdb-1.1.0.tar", max compression
+gzip compressed data, was "chatgdb-1.2.0.tar", max compression
```

## Comparing `chatgdb-1.1.0.tar` & `chatgdb-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-10 02:21:45.761529 chatgdb-1.1.0/LICENSE
--rw-r--r--   0        0        0     3614 2023-04-10 02:21:45.764862 chatgdb-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-10 01:32:55.050988 chatgdb-1.1.0/chatgdb/__init__.py
--rw-r--r--   0        0        0     1159 2023-04-10 01:57:51.202881 chatgdb-1.1.0/chatgdb/cli.py
--rw-r--r--   0        0        0     2068 2023-04-10 02:21:45.764862 chatgdb-1.1.0/chatgdb/gdb.py
--rw-r--r--   0        0        0     1517 2023-04-10 02:21:45.764862 chatgdb-1.1.0/chatgdb/lldb.py
--rw-r--r--   0        0        0     4049 2023-04-10 02:21:45.764862 chatgdb-1.1.0/chatgdb/utils.py
--rw-r--r--   0        0        0      567 2023-04-10 02:21:45.764862 chatgdb-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4580 1970-01-01 00:00:00.000000 chatgdb-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-10 02:21:45.761529 chatgdb-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3687 2023-04-10 03:11:24.037695 chatgdb-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 01:32:55.050988 chatgdb-1.2.0/chatgdb/__init__.py
+-rw-r--r--   0        0        0     1546 2023-04-10 02:50:27.091641 chatgdb-1.2.0/chatgdb/cli.py
+-rw-r--r--   0        0        0     2068 2023-04-10 02:46:58.868798 chatgdb-1.2.0/chatgdb/gdb.py
+-rw-r--r--   0        0        0     1517 2023-04-10 02:21:45.764862 chatgdb-1.2.0/chatgdb/lldb.py
+-rw-r--r--   0        0        0     4706 2023-04-10 03:06:51.735888 chatgdb-1.2.0/chatgdb/utils.py
+-rw-r--r--   0        0        0      567 2023-04-10 03:08:56.058486 chatgdb-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4653 1970-01-01 00:00:00.000000 chatgdb-1.2.0/PKG-INFO
```

### Comparing `chatgdb-1.1.0/LICENSE` & `chatgdb-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgdb-1.1.0/README.md` & `chatgdb-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,19 @@
 ```pip3 install chatgdb```. 
 
 It will create an executable called ```chatgdb``` that you will have to use to set your api key. 
 To do that, run the command
 
 ```chatgdb -k <API KEY> ```
 
-Without the API key, you won't be able to make requests to OpenAI. The API key is stored in
-text in the same directory as the installed script, which is currently in your python site packages
+You also need to set the model to use. There are two possible options, ```gpt-3.5-turbo``` and ```gpt-4```:
+
+```chatgdb -m <MODEL>```
+
+This information is stored in text in the same directory as the installed script, which is currently in your python site packages
 folder along with the main script. You can easily find this location by running the following in your terminal:
 
 ``` python -m site --user-site```
 
 Optionally, you can also download the compressed files in the releases page to get the scripts directly.
 If you do this, navigate to the ```chatgdb``` folder, and you can install with
```

### Comparing `chatgdb-1.1.0/chatgdb/cli.py` & `chatgdb-1.2.0/chatgdb/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import argparse
 from os.path import abspath, dirname
 from inspect import getfile, currentframe
 from urllib.request import Request, urlopen
 import json
 
+PATH = dirname(abspath(getfile(currentframe())))
+
 
 def set_key(key):
     """Set the api key for ChatGDB"""
-    path = dirname(abspath(getfile(currentframe()))) + "/.secret.txt"
-    with open(path, "w") as f:
+    with open(PATH + "/.secret.txt", "w") as f:
         f.write("OPENAI_KEY=\"" + key + "\"")
 
 
+def set_model(model):
+    """Set the model for ChatGDB"""
+    with open(PATH + "/.model.txt", "w") as f:
+        f.write("MODEL=\"" + model + "\"")
+
+
 def version():
     """Return version information"""
     with urlopen(Request("https://pypi.org/pypi/chatgdb/json"), timeout=10) as f:
         return json.load(f)["info"]["version"]
 
 
 def main():
@@ -24,22 +31,30 @@
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument(
         '-k',
         "--key",
         type=str,
         help="Provide an api key for ChatGDB")
     parser.add_argument(
+        '-m',
+        "--model",
+        type=str,
+        choices=["gpt-3.5-turbo", "gpt-4"],
+        help="Provide a model for ChatGDB (gpt-3.5-turbo or gpt-4)")
+    parser.add_argument(
         '-v',
         "--version",
         action="version",
         version="%(prog)s " + version(),
         help="Print the version of ChatGDB")
 
     args = parser.parse_args()
     if args.key:
         set_key(args.key)
+    elif args.model:
+        set_model(args.model)
     else:
         parser.print_help()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chatgdb-1.1.0/chatgdb/gdb.py` & `chatgdb-1.2.0/chatgdb/gdb.py`

 * *Files identical despite different names*

### Comparing `chatgdb-1.1.0/chatgdb/lldb.py` & `chatgdb-1.2.0/chatgdb/lldb.py`

 * *Files identical despite different names*

### Comparing `chatgdb-1.1.0/chatgdb/utils.py` & `chatgdb-1.2.0/chatgdb/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from urllib.error import HTTPError, URLError
 from urllib.request import Request, urlopen
 from os.path import abspath, dirname
 from inspect import getfile, currentframe
 
 
 def get_key():
-    """Gets api key from .env file
+    """Gets api key from secret file
 
     Returns: (str) api key
     """
     key = []
     secret = ""
     # gets path of this script - OS independent
     path = dirname(abspath(getfile(currentframe()))) + "/.secret.txt"
@@ -20,20 +20,44 @@
         with open(path) as f:
             key = [line.strip() for line in f]
         for k in key:
             if k.startswith("OPENAI_KEY"):
                 secret = k.split('"')[1::2]
     except FileNotFoundError:
         print("Could not find api key. Please make sure you've run the CLI "
-              "tool and set up your api key")
+              "tool and set up your model")
         quit("Exiting...")
 
     return secret[0]
 
 
+def get_model():
+    """Gets model from model file
+
+    Returns: (str) model
+    """
+    model = []
+    model_name = ""
+    # gets path of this script - OS independent
+    path = dirname(abspath(getfile(currentframe()))) + "/.model.txt"
+    try:
+        # get appropriate api key
+        with open(path) as f:
+            model = [line.strip() for line in f]
+        for m in model:
+            if m.startswith("MODEL"):
+                model_name = m.split('"')[1::2]
+    except FileNotFoundError:
+        print("Could not find model. Please make sure you've run the CLI "
+              "tool and set up your model")
+        quit("Exiting...")
+
+    return model_name[0]
+
+
 def make_request(url, headers=None, data=None):
     """Makes API request
 
     Params:
     url (str): url to make request to
     headers (dict, optional): headers to send with request. Defaults to None.
     data (bytes, optional): data to send with request. Defaults to None.
@@ -70,44 +94,43 @@
 
 
 HEADERS = {
     "Authorization": "Bearer " + get_key(),
     "Content-Type": "application/json"
 }
 URL = "https://api.openai.com/v1/chat/completions"
-MODEL = "gpt-3.5-turbo"
 
 
 def explain_helper(prev_command, command, prompt):
     """Generates explanation for either the previous command or a user query
 
     Params:
     prev_command (str): previous command
     command (str): user query
     prompt (str): prompt to use for explanation
     """
     question = prompt + prev_command if command == "" else command
-    data = {"model": MODEL,
+    data = {"model": get_model(),
             "messages": [{"role": "user",
                           "content": question}]}
     body, response = make_request(URL, HEADERS, data=bytes(json.dumps(data),
                                                            encoding="utf-8"))
     body = json.loads(body)
     explanation = body['choices'][0]['message']['content']
     print(explanation)
 
 
 def chat_helper(command, prompt):
     """Generates GDB/LLDB command based on user input
-    
+
     Params:
     command (str): user input
     prompt (str): prompt to use for command generation
     """
-    data = {"model": MODEL,
+    data = {"model": get_model(),
             "messages": [{"role": "user",
                           "content": prompt + command}]}
 
     body, response = make_request(URL, HEADERS, data=bytes(json.dumps(data),
                                                            encoding="utf-8"))
     body = json.loads(body)
     command = body['choices'][0]['message']['content']
```

### Comparing `chatgdb-1.1.0/pyproject.toml` & `chatgdb-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ChatGDB"
-version = "1.1.0"
+version = "1.2.0"
 authors = ["Pranay Gosar <gosarpranay@gmail.com>"]
 description = "Harness the power of ChatGPT directly inside the GDB debugger!"
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/pgosar/chatgdb"
 keywords = ["gdb", "debugger", "chatgpt"]
```

### Comparing `chatgdb-1.1.0/PKG-INFO` & `chatgdb-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgdb
-Version: 1.1.0
+Version: 1.2.0
 Summary: Harness the power of ChatGPT directly inside the GDB debugger!
 Home-page: https://github.com/pgosar/chatgdb
 License: MIT
 Keywords: gdb,debugger,chatgpt
 Author: Pranay Gosar
 Author-email: gosarpranay@gmail.com
 Requires-Python: >=3.3,<4.0
@@ -49,16 +49,19 @@
 ```pip3 install chatgdb```. 
 
 It will create an executable called ```chatgdb``` that you will have to use to set your api key. 
 To do that, run the command
 
 ```chatgdb -k <API KEY> ```
 
-Without the API key, you won't be able to make requests to OpenAI. The API key is stored in
-text in the same directory as the installed script, which is currently in your python site packages
+You also need to set the model to use. There are two possible options, ```gpt-3.5-turbo``` and ```gpt-4```:
+
+```chatgdb -m <MODEL>```
+
+This information is stored in text in the same directory as the installed script, which is currently in your python site packages
 folder along with the main script. You can easily find this location by running the following in your terminal:
 
 ``` python -m site --user-site```
 
 Optionally, you can also download the compressed files in the releases page to get the scripts directly.
 If you do this, navigate to the ```chatgdb``` folder, and you can install with
```

