# Comparing `tmp/langchain_utils-0.2.1.tar.gz` & `tmp/langchain_utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.2.1.tar", max compression
+gzip compressed data, was "langchain_utils-0.2.2.tar", max compression
```

## Comparing `langchain_utils-0.2.1.tar` & `langchain_utils-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4052 2023-04-10 05:23:04.033834 langchain_utils-0.2.1/README.md
--rw-r--r--   0        0        0       22 2023-04-10 05:46:56.102220 langchain_utils-0.2.1/langchain_utils/__init__.py
--rw-r--r--   0        0        0      117 2023-04-10 05:46:38.293069 langchain_utils-0.2.1/langchain_utils/config.py
--rwxr-xr-x   0        0        0     3178 2023-04-10 05:17:55.040881 langchain_utils-0.2.1/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     3344 2023-04-10 05:46:50.936167 langchain_utils-0.2.1/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     2952 2023-04-10 02:26:03.291439 langchain_utils-0.2.1/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     1410 2023-04-10 04:52:53.679712 langchain_utils-0.2.1/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.2.1/langchain_utils/prompts.py
--rw-r--r--   0        0        0     4053 2023-04-10 04:01:15.826309 langchain_utils-0.2.1/langchain_utils/utils.py
--rw-r--r--   0        0        0     1496 2023-04-10 05:46:56.101518 langchain_utils-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5054 1970-01-01 00:00:00.000000 langchain_utils-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4051 2023-04-10 05:47:33.656483 langchain_utils-0.2.2/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 05:47:39.134689 langchain_utils-0.2.2/langchain_utils/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-10 05:46:38.293069 langchain_utils-0.2.2/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     3178 2023-04-10 05:17:55.040881 langchain_utils-0.2.2/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     3344 2023-04-10 05:46:50.936167 langchain_utils-0.2.2/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     2952 2023-04-10 02:26:03.291439 langchain_utils-0.2.2/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     1410 2023-04-10 04:52:53.679712 langchain_utils-0.2.2/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.2.2/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     4053 2023-04-10 04:01:15.826309 langchain_utils-0.2.2/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1496 2023-04-10 05:47:39.134248 langchain_utils-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5053 1970-01-01 00:00:00.000000 langchain_utils-0.2.2/PKG-INFO
```

### Comparing `langchain_utils-0.2.1/README.md` & `langchain_utils-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
   -c, --copy            Copy the prompt to clipboard (default: False)
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
   -S, --split           Split the prompt into multiple parts (default: False)
   -M, --merge           Merge contents of all pages before processing (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to determine whether to split (default: 2000)
-  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF content in the prompt (default: the content of a PDF file)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF content in the prompt (default: the content of a webpage)
   -j, --javascript      Use JavaScript to render the page (default: False)
   -n, --dry-run         Dry run (default: False)
 ```
 
 ### `pdfprompt`
 
 ```
```

### Comparing `langchain_utils-0.2.1/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.2.2/langchain_utils/get_pdf_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.2.1/langchain_utils/get_url_prompt.py` & `langchain_utils-0.2.2/langchain_utils/get_url_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.2.1/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.2.2/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.2.1/langchain_utils/loaders.py` & `langchain_utils-0.2.2/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.2.1/langchain_utils/utils.py` & `langchain_utils-0.2.2/langchain_utils/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.2.1/pyproject.toml` & `langchain_utils-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.2.1/PKG-INFO` & `langchain_utils-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -62,15 +62,15 @@
   -c, --copy            Copy the prompt to clipboard (default: False)
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
   -S, --split           Split the prompt into multiple parts (default: False)
   -M, --merge           Merge contents of all pages before processing (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to determine whether to split (default: 2000)
-  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF content in the prompt (default: the content of a PDF file)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF content in the prompt (default: the content of a webpage)
   -j, --javascript      Use JavaScript to render the page (default: False)
   -n, --dry-run         Dry run (default: False)
 ```
 
 ### `pdfprompt`
 
 ```
```

