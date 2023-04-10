# Comparing `tmp/langchain_utils-0.1.6.tar.gz` & `tmp/langchain_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.1.6.tar", max compression
+gzip compressed data, was "langchain_utils-0.1.7.tar", max compression
```

## Comparing `langchain_utils-0.1.6.tar` & `langchain_utils-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.6/README.md
--rw-r--r--   0        0        0       22 2023-04-10 02:22:30.016306 langchain_utils-0.1.6/langchain_utils/__init__.py
--rw-r--r--   0        0        0       71 2023-04-09 15:21:28.583065 langchain_utils-0.1.6/langchain_utils/config.py
--rwxr-xr-x   0        0        0     3331 2023-04-10 02:21:54.768927 langchain_utils-0.1.6/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2947 2023-04-10 02:22:24.008293 langchain_utils-0.1.6/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0      559 2023-04-09 15:13:17.822169 langchain_utils-0.1.6/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.1.6/langchain_utils/prompts.py
--rw-r--r--   0        0        0     3678 2023-04-10 02:18:58.686955 langchain_utils-0.1.6/langchain_utils/utils.py
--rw-r--r--   0        0        0     1244 2023-04-10 02:22:30.015745 langchain_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 langchain_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.7/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 02:45:57.248793 langchain_utils-0.1.7/langchain_utils/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-09 15:21:28.583065 langchain_utils-0.1.7/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     3260 2023-04-10 02:44:39.403745 langchain_utils-0.1.7/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     2952 2023-04-10 02:26:03.291439 langchain_utils-0.1.7/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0      559 2023-04-09 15:13:17.822169 langchain_utils-0.1.7/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.1.7/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     3865 2023-04-10 02:45:28.117968 langchain_utils-0.1.7/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1244 2023-04-10 02:45:57.248256 langchain_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 langchain_utils-0.1.7/PKG-INFO
```

### Comparing `langchain_utils-0.1.6/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.1.7/langchain_utils/get_pdf_prompt.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,14 +51,20 @@
     parser.add_argument(
         '-S',
         '--split',
         help='Split the prompt into multiple parts',
         action='store_true',
     )
     parser.add_argument(
+        '-M',
+        '--merge',
+        help='Merge contents of all pages before processing',
+        action='store_true',
+    )
+    parser.add_argument(
         '-s',
         '--chunk-size',
         help='Chunk size when splitting transcript, also used to determine whether to split',
         metavar='chunk_size',
         type=int,
         default=2000,
     )
@@ -85,31 +91,30 @@
     texts = [doc.page_content for doc in docs]
     all_text = '\n'.join(texts)
     word_count = get_word_count((all_text))
     print(
         f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
         file=sys.stderr,
     )
-    # metadata = docs[0].metadata
-    # title = metadata['title']
-    # author = metadata['author']
-    # publish_date = format_date(metadata['publish_date'])
-    # what = f'''the transcript of a YouTube video titled "{title}" uploaded by "{author}" on {publish_date}'''
-    # print(f'Title: {title}', file=sys.stderr)
-    # print(f'Author: {author}', file=sys.stderr)
-    # print(f'Publish date: {publish_date}', file=sys.stderr)
-    # if args.split or get_token_count(docs[0].page_content) > args.chunk_size:
+    if args.merge:
+        from langchain.docstore.document import Document
+
+        merged = Document(
+            page_content=all_text,
+            metadata={
+                k: v for k, v in docs[0].metadata.items() if k not in {'page_number'}
+            },
+        )
     if args.split or word_count > args.chunk_size * 0.75:
         needs_splitting = True
     else:
         needs_splitting = False
     deliver_prompts(
         what=args.what,
-        docs=docs,
-        should_be_only_one_doc=True,
+        documents=[merged] if args.merge else docs,  # type: ignore
         needs_splitting=needs_splitting,
         copy=args.copy,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=pymupdf_doc_page_info,
         dry_run=args.dry_run,
     )
```

### Comparing `langchain_utils-0.1.6/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.1.7/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     # if args.split or get_token_count(docs[0].page_content) > args.chunk_size:
     if args.split or get_word_count(docs[0].page_content) > args.chunk_size * 0.75:
         needs_splitting = True
     else:
         needs_splitting = False
     deliver_prompts(
         what=what,
-        docs=docs,
+        documents=docs,
         should_be_only_one_doc=True,
         needs_splitting=needs_splitting,
         copy=args.copy,
         chunk_size=args.chunk_size,
         dry_run=args.dry_run,
     )
```

### Comparing `langchain_utils-0.1.6/langchain_utils/loaders.py` & `langchain_utils-0.1.7/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.1.6/langchain_utils/utils.py` & `langchain_utils-0.1.7/langchain_utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-from typing import TYPE_CHECKING, Callable
+from typing import TYPE_CHECKING, Callable, NoReturn
 import sys
 from .prompts import (
     REPLY_OK_IF_YOU_READ_TEMPLATE,
     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_FIRST,
     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_CONTINUED,
 )
 
@@ -30,20 +30,23 @@
 
 def format_date(dt: 'datetime') -> str:
     return dt.strftime('%Y-%m-%d')
 
 
 def pymupdf_doc_page_info(document: 'Document') -> str:
     metadata = document.metadata
-    return f', Page {metadata["page_number"]}/{metadata["total_pages"]}'
+    if 'page_number' in metadata:
+        return f', Page {metadata["page_number"]}/{metadata["total_pages"]}'
+    else:
+        return ''
 
 
 def deliver_prompts(
     what: str,
-    docs: list['Document'],
+    documents: list['Document'],
     should_be_only_one_doc: bool = False,
     needs_splitting: bool = False,
     copy: bool = True,
     chunk_size: int = 2000,
     extra_chunk_info_fn: Callable[['Document'], str] = lambda doc: '',
     dry_run: bool = False,
 ):
@@ -95,15 +98,19 @@
             f'Dry running. Nothing will be copied to your clipboard, and you don'
             't need to press Enter to move forward.'
         )
     if needs_splitting:
         from langchain.text_splitter import TokenTextSplitter
 
         splitter = TokenTextSplitter(encoding_name='cl100k_base', chunk_size=chunk_size)
-        splitted = splitter.split_documents(docs)
+        splitted = splitter.split_documents(documents)
         num_chunks = len(splitted)
         deliver_multiple_docs(splitted)
 
     elif should_be_only_one_doc:
-        deliver_single_doc(docs[0])
+        deliver_single_doc(documents[0])
     else:
-        deliver_multiple_docs(docs)
+        deliver_multiple_docs(documents)
+
+
+def assert_never(a: NoReturn) -> NoReturn:
+    raise RuntimeError("Should not get here")
```

### Comparing `langchain_utils-0.1.6/pyproject.toml` & `langchain_utils-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.1.6/PKG-INFO` & `langchain_utils-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

