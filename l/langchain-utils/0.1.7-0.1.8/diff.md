# Comparing `tmp/langchain_utils-0.1.7.tar.gz` & `tmp/langchain_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.1.7.tar", max compression
+gzip compressed data, was "langchain_utils-0.1.8.tar", max compression
```

## Comparing `langchain_utils-0.1.7.tar` & `langchain_utils-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.7/README.md
--rw-r--r--   0        0        0       22 2023-04-10 02:45:57.248793 langchain_utils-0.1.7/langchain_utils/__init__.py
--rw-r--r--   0        0        0       71 2023-04-09 15:21:28.583065 langchain_utils-0.1.7/langchain_utils/config.py
--rwxr-xr-x   0        0        0     3260 2023-04-10 02:44:39.403745 langchain_utils-0.1.7/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2952 2023-04-10 02:26:03.291439 langchain_utils-0.1.7/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0      559 2023-04-09 15:13:17.822169 langchain_utils-0.1.7/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.1.7/langchain_utils/prompts.py
--rw-r--r--   0        0        0     3865 2023-04-10 02:45:28.117968 langchain_utils-0.1.7/langchain_utils/utils.py
--rw-r--r--   0        0        0     1244 2023-04-10 02:45:57.248256 langchain_utils-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 langchain_utils-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.8/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 04:53:43.895562 langchain_utils-0.1.8/langchain_utils/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-09 15:21:28.583065 langchain_utils-0.1.8/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     3260 2023-04-10 02:44:39.403745 langchain_utils-0.1.8/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     3427 2023-04-10 04:15:08.852973 langchain_utils-0.1.8/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     2952 2023-04-10 02:26:03.291439 langchain_utils-0.1.8/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     1410 2023-04-10 04:52:53.679712 langchain_utils-0.1.8/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.1.8/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     4053 2023-04-10 04:01:15.826309 langchain_utils-0.1.8/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1496 2023-04-10 04:53:43.893492 langchain_utils-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 langchain_utils-0.1.8/PKG-INFO
```

### Comparing `langchain_utils-0.1.7/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.1.8/langchain_utils/get_pdf_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.1.7/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.1.8/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.1.7/langchain_utils/utils.py` & `langchain_utils-0.1.8/langchain_utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,22 @@
     metadata = document.metadata
     if 'page_number' in metadata:
         return f', Page {metadata["page_number"]}/{metadata["total_pages"]}'
     else:
         return ''
 
 
+def url_source_info(document: 'Document') -> str:
+    metadata = document.metadata
+    if 'source' in metadata:
+        return f', URL: {metadata["source"]}'
+    else:
+        return ''
+
+
 def deliver_prompts(
     what: str,
     documents: list['Document'],
     should_be_only_one_doc: bool = False,
     needs_splitting: bool = False,
     copy: bool = True,
     chunk_size: int = 2000,
```

### Comparing `langchain_utils-0.1.7/pyproject.toml` & `langchain_utils-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
 classifiers = ["Topic :: Utilities"]
 keywords = ["langchain", "utils", "LLM", "prompts", "CLI"]
 
 [tool.poetry.scripts]
 get-youtube-transcript-prompt = "langchain_utils.get_youtube_transcript_prompt:main"
 ytprompt = "langchain_utils.get_youtube_transcript_prompt:main"
+get-url-prompt = "langchain_utils.get_url_prompt:main"
+urlprompt = "langchain_utils.get_url_prompt:main"
 get-pdf-prompt = "langchain_utils.get_pdf_prompt:main"
 pdfprompt = "langchain_utils.get_pdf_prompt:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/langchain-utils/issues"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 langchain = "^0.0.135"
 youtube-transcript-api = "^0.5.0"
 pytube = "^12.1.3"
 pyperclip = "^1.8.2"
 tiktoken = "^0.3.3"
 pymupdf = "^1.21.1"
+# must use this version of unstructured, or it won't be able to parse certain htmls
+unstructured = "0.5.2"
+selenium = "^4.8.3"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 better-exceptions = "^0.3.3"
 ipython = "^8.12.0"
 ipykernel = "^6.22.0"
 rich = "^13.3.3"
 pyinstrument = "^4.4.0"
+icecream = "^2.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `langchain_utils-0.1.7/PKG-INFO` & `langchain_utils-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: langchain (>=0.0.135,<0.0.136)
 Requires-Dist: pymupdf (>=1.21.1,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pytube (>=12.1.3,<13.0.0)
+Requires-Dist: selenium (>=4.8.3,<5.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
+Requires-Dist: unstructured (==0.5.2)
 Requires-Dist: youtube-transcript-api (>=0.5.0,<0.6.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/langchain-utils/issues
 Project-URL: Repository, https://github.com/tddschn/langchain-utils
 Description-Content-Type: text/markdown
```

