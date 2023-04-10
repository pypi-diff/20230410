# Comparing `tmp/langchain_utils-0.3.2.tar.gz` & `tmp/langchain_utils-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.3.2.tar", max compression
+gzip compressed data, was "langchain_utils-0.3.3.tar", max compression
```

## Comparing `langchain_utils-0.3.2.tar` & `langchain_utils-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4589 2023-04-10 07:12:43.729444 langchain_utils-0.3.2/README.md
--rw-r--r--   0        0        0       22 2023-04-10 07:12:48.292778 langchain_utils-0.3.2/langchain_utils/__init__.py
--rw-r--r--   0        0        0      117 2023-04-10 05:46:38.293069 langchain_utils-0.3.2/langchain_utils/config.py
--rwxr-xr-x   0        0        0     2690 2023-04-10 07:08:16.747243 langchain_utils-0.3.2/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2476 2023-04-10 06:31:07.437695 langchain_utils-0.3.2/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     2085 2023-04-10 06:55:38.534036 langchain_utils-0.3.2/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     1410 2023-04-10 04:52:53.679712 langchain_utils-0.3.2/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.2/langchain_utils/prompts.py
--rw-r--r--   0        0        0     5860 2023-04-10 07:11:30.445800 langchain_utils-0.3.2/langchain_utils/utils.py
--rw-r--r--   0        0        0     1277 2023-04-10 06:26:58.124248 langchain_utils-0.3.2/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     1496 2023-04-10 07:12:48.292328 langchain_utils-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5591 1970-01-01 00:00:00.000000 langchain_utils-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     4589 2023-04-10 07:12:43.729444 langchain_utils-0.3.3/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 07:40:34.715694 langchain_utils-0.3.3/langchain_utils/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-10 05:46:38.293069 langchain_utils-0.3.3/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     2716 2023-04-10 07:40:32.060389 langchain_utils-0.3.3/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     2502 2023-04-10 07:36:50.130151 langchain_utils-0.3.3/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     2111 2023-04-10 07:40:28.101477 langchain_utils-0.3.3/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     1410 2023-04-10 04:52:53.679712 langchain_utils-0.3.3/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.3/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     6275 2023-04-10 07:40:14.894333 langchain_utils-0.3.3/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1467 2023-04-10 07:33:58.876416 langchain_utils-0.3.3/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     1496 2023-04-10 07:40:34.714657 langchain_utils-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5591 1970-01-01 00:00:00.000000 langchain_utils-0.3.3/PKG-INFO
```

### Comparing `langchain_utils-0.3.2/README.md` & `langchain_utils-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.2/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.3.3/langchain_utils/get_pdf_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,12 +90,13 @@
         documents=[merged] if args.merge else docs,  # type: ignore
         needs_splitting=needs_splitting,
         copy=args.copy,
         edit=args.edit,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=pymupdf_doc_page_info,
         dry_run=args.dry_run,
+        parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.3.2/langchain_utils/get_url_prompt.py` & `langchain_utils-0.3.3/langchain_utils/get_url_prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,12 +83,13 @@
         needs_splitting=needs_splitting,
         copy=args.copy,
         edit=args.edit,
         should_be_only_one_doc=True,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=url_source_info,
         dry_run=args.dry_run,
+        parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.3.2/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.3.3/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,12 +55,13 @@
         documents=docs,
         should_be_only_one_doc=True,
         needs_splitting=needs_splitting,
         copy=args.copy,
         edit=args.edit,
         chunk_size=args.chunk_size,
         dry_run=args.dry_run,
+        parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.3.2/langchain_utils/loaders.py` & `langchain_utils-0.3.3/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.2/langchain_utils/utils.py` & `langchain_utils-0.3.3/langchain_utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     should_be_only_one_doc: bool = False,
     needs_splitting: bool = False,
     copy: bool = True,
     edit: bool = False,
     chunk_size: int = 2000,
     extra_chunk_info_fn: Callable[['Document'], str] = lambda doc: '',
     dry_run: bool = False,
+    parts: list[int] | None = None,
 ):
     from langchain.prompts import PromptTemplate
 
     def deliver_single_doc(document: 'Document'):
         prompt = PromptTemplate.from_template(REPLY_OK_IF_YOU_READ_TEMPLATE)
         content = document.page_content
         formatted_prompt = prompt.format(what=what, content=content)
@@ -163,14 +164,22 @@
             't need to press Enter to move forward.'
         )
     if needs_splitting:
         from langchain.text_splitter import TokenTextSplitter
 
         splitter = TokenTextSplitter(encoding_name='cl100k_base', chunk_size=chunk_size)
         splitted = splitter.split_documents(documents)
+        if parts:
+            len_splitted = len(splitted)
+            parts = list({part for part in parts if 0 <= part - 1 < len_splitted})
+            print(
+                f'Selecting {len(parts)} parts out of {len_splitted}.', file=sys.stderr
+            )
+            print(f'Using parts: {parts}', file=sys.stderr)
+            splitted = [splitted[i - 1] for i in parts]
         deliver_multiple_docs(splitted)
 
     elif should_be_only_one_doc:
         deliver_single_doc(documents[0])
     else:
         deliver_multiple_docs(documents)
```

### Comparing `langchain_utils-0.3.2/langchain_utils/utils_argparse.py` & `langchain_utils-0.3.3/langchain_utils/utils_argparse.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,9 +38,17 @@
         '-s',
         '--chunk-size',
         help='Chunk size when splitting transcript, also used to determine whether to split',
         metavar='chunk_size',
         type=int,
         default=2000,
     )
+    parser.add_argument(
+        '-P',
+        '--parts',
+        help='Parts to select in the processes list of Documents',
+        type=int,
+        nargs='+',
+        default=None,
+    )
     parser.add_argument('-n', '--dry-run', help='Dry run', action='store_true')
     return parser
```

### Comparing `langchain_utils-0.3.2/pyproject.toml` & `langchain_utils-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.3.2/PKG-INFO` & `langchain_utils-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

