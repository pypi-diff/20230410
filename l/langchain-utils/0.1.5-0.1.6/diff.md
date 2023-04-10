# Comparing `tmp/langchain_utils-0.1.5.tar.gz` & `tmp/langchain_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.1.5.tar", max compression
+gzip compressed data, was "langchain_utils-0.1.6.tar", max compression
```

## Comparing `langchain_utils-0.1.5.tar` & `langchain_utils-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.5/README.md
--rw-r--r--   0        0        0       22 2023-04-10 02:20:20.575610 langchain_utils-0.1.5/langchain_utils/__init__.py
--rw-r--r--   0        0        0       71 2023-04-09 15:21:28.583065 langchain_utils-0.1.5/langchain_utils/config.py
--rwxr-xr-x   0        0        0     3170 2023-04-10 02:19:48.885856 langchain_utils-0.1.5/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2786 2023-04-10 02:19:30.567185 langchain_utils-0.1.5/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0      559 2023-04-09 15:13:17.822169 langchain_utils-0.1.5/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.1.5/langchain_utils/prompts.py
--rw-r--r--   0        0        0     3678 2023-04-10 02:18:58.686955 langchain_utils-0.1.5/langchain_utils/utils.py
--rw-r--r--   0        0        0     1244 2023-04-10 02:20:20.575174 langchain_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 langchain_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.6/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 02:22:30.016306 langchain_utils-0.1.6/langchain_utils/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-09 15:21:28.583065 langchain_utils-0.1.6/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     3331 2023-04-10 02:21:54.768927 langchain_utils-0.1.6/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     2947 2023-04-10 02:22:24.008293 langchain_utils-0.1.6/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0      559 2023-04-09 15:13:17.822169 langchain_utils-0.1.6/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.1.6/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     3678 2023-04-10 02:18:58.686955 langchain_utils-0.1.6/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1244 2023-04-10 02:22:30.015745 langchain_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 langchain_utils-0.1.6/PKG-INFO
```

### Comparing `langchain_utils-0.1.5/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.1.6/langchain_utils/get_pdf_prompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Date   : 2023-04-09
 Purpose: Get a prompt consisting Title and Transcript of a YouTube Video
 """
 
 import argparse
 import sys
 
+from . import __version__
 from .utils import (
     deliver_prompts,
     format_date,
     get_word_count,
     deliver_prompts,
     pymupdf_doc_page_info,
 )
@@ -27,14 +28,20 @@
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     parser.add_argument(
         'pdf_path', help='Path to the PDF file', metavar='PDF Path', type=str
     )
     parser.add_argument(
+        '-V',
+        '--version',
+        action='version',
+        version=f'%(prog)s {__version__}',
+    )
+    parser.add_argument(
         '-c', '--copy', help='Copy the prompt to clipboard', action='store_true'
     )
     parser.add_argument(
         '-m',
         '--model',
         help='Model to use',
         metavar='model',
```

### Comparing `langchain_utils-0.1.5/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.1.6/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,35 @@
 Date   : 2023-04-09
 Purpose: Get a prompt consisting Title and Transcript of a YouTube Video
 """
 
 import argparse
 import sys
 
+from . import __version__
 from .utils import deliver_prompts, format_date, get_word_count, deliver_prompts
 from .loaders import load_youtube_url
 
 
 def get_args():
     """Get command-line arguments"""
 
     parser = argparse.ArgumentParser(
         description='Get a prompt consisting Title and Transcript of a YouTube Video',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     parser.add_argument('youtube_url', metavar='YouTube URL', help='YouTube URL')
     parser.add_argument(
+        '-V',
+        '--version',
+        action='version',
+        version=f'%(prog)s {__version__}',
+    )
+    parser.add_argument(
         '-c', '--copy', help='Copy the prompt to clipboard', action='store_true'
     )
     parser.add_argument(
         '-m',
         '--model',
         help='Model to use',
         metavar='model',
```

### Comparing `langchain_utils-0.1.5/langchain_utils/loaders.py` & `langchain_utils-0.1.6/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.1.5/langchain_utils/utils.py` & `langchain_utils-0.1.6/langchain_utils/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.1.5/pyproject.toml` & `langchain_utils-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.1.5/PKG-INFO` & `langchain_utils-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

