# Comparing `tmp/tulp-0.3.2.tar.gz` & `tmp/tulp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulp-0.3.2.tar", last modified: Sun Apr  9 15:39:18 2023, max compression
+gzip compressed data, was "tulp-0.4.0.tar", last modified: Mon Apr 10 14:07:30 2023, max compression
```

## Comparing `tulp-0.3.2.tar` & `tulp-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-09 15:39:18.130696 tulp-0.3.2/
--rw-rw-r--   0 fede      (1000) fede      (1000)      599 2023-04-09 15:39:18.130696 tulp-0.3.2/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)     5010 2023-04-09 15:35:50.000000 tulp-0.3.2/README.md
--rw-rw-r--   0 fede      (1000) fede      (1000)     3977 2023-04-09 15:21:27.000000 tulp-0.3.2/filteringPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     2230 2023-04-09 15:21:27.000000 tulp-0.3.2/requestPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)       38 2023-04-09 15:39:18.130696 tulp-0.3.2/setup.cfg
--rw-rw-r--   0 fede      (1000) fede      (1000)      871 2023-04-09 15:39:11.000000 tulp-0.3.2/setup.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-09 15:39:18.130696 tulp-0.3.2/tulp.egg-info/
--rw-rw-r--   0 fede      (1000) fede      (1000)      599 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)      260 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/SOURCES.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/dependency_links.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       53 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/entry_points.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        7 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/requires.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       57 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/top_level.txt
--rwxrwxr-x   0 fede      (1000) fede      (1000)     5092 2023-04-09 15:21:27.000000 tulp-0.3.2/tulp.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1008 2023-04-09 15:28:22.000000 tulp-0.3.2/tulpconfig.py
--rw-rw-r--   0 fede      (1000) fede      (1000)      972 2023-04-09 15:21:27.000000 tulp-0.3.2/tulplogger.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-10 14:07:30.321810 tulp-0.4.0/
+-rw-rw-r--   0 fede      (1000) fede      (1000)      684 2023-04-10 13:46:44.000000 tulp-0.4.0/LICENSE
+-rw-rw-r--   0 fede      (1000) fede      (1000)     5605 2023-04-10 14:07:30.321810 tulp-0.4.0/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)     5010 2023-04-09 15:35:50.000000 tulp-0.4.0/README.md
+-rw-rw-r--   0 fede      (1000) fede      (1000)      900 2023-04-10 14:07:30.321810 tulp-0.4.0/setup.cfg
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-04-10 13:18:19.000000 tulp-0.4.0/setup.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-10 14:07:30.321810 tulp-0.4.0/tulp/
+-rw-rw-r--   0 fede      (1000) fede      (1000)       74 2023-04-10 13:37:14.000000 tulp-0.4.0/tulp/__init__.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3977 2023-04-09 15:21:27.000000 tulp-0.4.0/tulp/filteringPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2230 2023-04-09 15:21:27.000000 tulp-0.4.0/tulp/requestPrompt.py
+-rwxrwxr-x   0 fede      (1000) fede      (1000)     5231 2023-04-10 14:05:27.000000 tulp-0.4.0/tulp/tulp.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1008 2023-04-10 14:01:41.000000 tulp-0.4.0/tulp/tulpconfig.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      991 2023-04-10 14:01:12.000000 tulp-0.4.0/tulp/tulplogger.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)       18 2023-04-10 13:49:07.000000 tulp-0.4.0/tulp/version.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-10 14:07:30.321810 tulp-0.4.0/tulp.egg-info/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     5605 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)      359 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/SOURCES.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/dependency_links.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/entry_points.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       15 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/requires.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        5 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/top_level.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-10 13:32:42.000000 tulp-0.4.0/tulp.egg-info/zip-safe
```

### Comparing `tulp-0.3.2/README.md` & `tulp-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tulp-0.3.2/filteringPrompt.py` & `tulp-0.4.0/tulp/filteringPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-0.3.2/requestPrompt.py` & `tulp-0.4.0/tulp/requestPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-0.3.2/tulp.py` & `tulp-0.4.0/tulp/tulp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/python3
 import openai
 import argparse
 import sys
 import os
 import math
-import tulplogger
-import tulpconfig
+import tulp.tulplogger as tulplogger
+import tulp.tulpconfig as tulpconfig
+import tulp.version as version
 
 log = tulplogger.Logger()
 config = tulpconfig.TulipConfig()
 
 def run():
 
+    log.info(f"Running tulp v{version.VERSION}.")
     openai_key = config.openai_api_key
     if not openai_key:
         log.error(f'OpenAI API key not found. Please set the TULP_OPENAI_API_KEY environment variable or add it to {tulpconfig.CONFIG_FILE}')
         sys.exit(1)
 
     openai.api_key = openai_key
     prev_context=None
@@ -53,19 +55,19 @@
         instructions = prompt
 
 
 
 
     instructionFunction=None
     if instructions:
-        import filteringPrompt
-        instructionFunction=filteringPrompt.getBaseMessages
+        import tulp.filteringPrompt
+        instructionFunction=tulp.filteringPrompt.getBaseMessages
     else:
-        import requestPrompt
-        instructionFunction=requestPrompt.getBaseMessages
+        import tulp.requestPrompt
+        instructionFunction=tulp.requestPrompt.getBaseMessages
 
     user_messages=[]
     # Split input text into chunks to fit within max token window
     max_chars = config.max_chars  # Maximum number of chars that we will send to GPT
     if len(input_text) > max_chars:
         log.warning(f"Warning: input is to big, we will split processing in chunks of less than {max_chars}")
     input_lines = input_text.splitlines()
```

### Comparing `tulp-0.3.2/tulpconfig.py` & `tulp-0.4.0/tulp/tulpconfig.py`

 * *Files identical despite different names*

### Comparing `tulp-0.3.2/tulplogger.py` & `tulp-0.4.0/tulp/tulplogger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import sys
-import tulpconfig
+import tulp.tulpconfig as tulpconfig
 
 config = tulpconfig.TulipConfig()
 
 class Logger:
     def __init__(self):
         self.log_level = config.log_level
```

