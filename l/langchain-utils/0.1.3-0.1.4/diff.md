# Comparing `tmp/langchain_utils-0.1.3.tar.gz` & `tmp/langchain_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.1.3.tar", max compression
+gzip compressed data, was "langchain_utils-0.1.4.tar", max compression
```

## Comparing `langchain_utils-0.1.3.tar` & `langchain_utils-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-04-09 14:47:07.372336 langchain_utils-0.1.3/langchain_utils/__init__.py
--rwxr-xr-x   0        0        0     4309 2023-04-09 14:45:07.607836 langchain_utils-0.1.3/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0      449 2023-04-09 14:08:17.975001 langchain_utils-0.1.3/langchain_utils/prompts.py
--rw-r--r--   0        0        0      534 2023-04-09 14:36:32.955521 langchain_utils-0.1.3/langchain_utils/utils.py
--rw-r--r--   0        0        0     1119 2023-04-09 14:47:07.371731 langchain_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 langchain_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 02:05:55.970644 langchain_utils-0.1.4/langchain_utils/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-09 15:21:28.583065 langchain_utils-0.1.4/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     2961 2023-04-10 02:03:10.281229 langchain_utils-0.1.4/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     2675 2023-04-09 15:13:41.939409 langchain_utils-0.1.4/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0      559 2023-04-09 15:13:17.822169 langchain_utils-0.1.4/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.1.4/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     2857 2023-04-09 15:03:48.493911 langchain_utils-0.1.4/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1244 2023-04-10 02:05:55.969971 langchain_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 langchain_utils-0.1.4/PKG-INFO
```

### Comparing `langchain_utils-0.1.3/pyproject.toml` & `langchain_utils-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.1.3"
+version = "0.1.4"
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
+get-pdf-prompt = "langchain_utils.get_pdf_prompt:main"
+pdfprompt = "langchain_utils.get_pdf_prompt:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/langchain-utils/issues"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 langchain = "^0.0.135"
 youtube-transcript-api = "^0.5.0"
 pytube = "^12.1.3"
 pyperclip = "^1.8.2"
 tiktoken = "^0.3.3"
+pymupdf = "^1.21.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 better-exceptions = "^0.3.3"
 ipython = "^8.12.0"
 ipykernel = "^6.22.0"
```

### Comparing `langchain_utils-0.1.3/PKG-INFO` & `langchain_utils-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: langchain (>=0.0.135,<0.0.136)
+Requires-Dist: pymupdf (>=1.21.1,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pytube (>=12.1.3,<13.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: youtube-transcript-api (>=0.5.0,<0.6.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/langchain-utils/issues
 Project-URL: Repository, https://github.com/tddschn/langchain-utils
 Description-Content-Type: text/markdown
```

