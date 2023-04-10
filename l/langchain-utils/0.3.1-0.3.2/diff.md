# Comparing `tmp/langchain_utils-0.3.1.tar.gz` & `tmp/langchain_utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.3.1.tar", max compression
+gzip compressed data, was "langchain_utils-0.3.2.tar", max compression
```

## Comparing `langchain_utils-0.3.1.tar` & `langchain_utils-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4439 2023-04-10 06:32:17.794161 langchain_utils-0.3.1/README.md
--rw-r--r--   0        0        0       22 2023-04-10 06:56:37.246644 langchain_utils-0.3.1/langchain_utils/__init__.py
--rw-r--r--   0        0        0      117 2023-04-10 05:46:38.293069 langchain_utils-0.3.1/langchain_utils/config.py
--rwxr-xr-x   0        0        0     2295 2023-04-10 06:55:46.081945 langchain_utils-0.3.1/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2476 2023-04-10 06:31:07.437695 langchain_utils-0.3.1/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     2085 2023-04-10 06:55:38.534036 langchain_utils-0.3.1/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     1410 2023-04-10 04:52:53.679712 langchain_utils-0.3.1/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.1/langchain_utils/prompts.py
--rw-r--r--   0        0        0     5855 2023-04-10 06:38:03.479798 langchain_utils-0.3.1/langchain_utils/utils.py
--rw-r--r--   0        0        0     1277 2023-04-10 06:26:58.124248 langchain_utils-0.3.1/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     1496 2023-04-10 06:56:37.245292 langchain_utils-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5441 1970-01-01 00:00:00.000000 langchain_utils-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4589 2023-04-10 07:12:43.729444 langchain_utils-0.3.2/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 07:12:48.292778 langchain_utils-0.3.2/langchain_utils/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-10 05:46:38.293069 langchain_utils-0.3.2/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     2690 2023-04-10 07:08:16.747243 langchain_utils-0.3.2/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     2476 2023-04-10 06:31:07.437695 langchain_utils-0.3.2/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     2085 2023-04-10 06:55:38.534036 langchain_utils-0.3.2/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     1410 2023-04-10 04:52:53.679712 langchain_utils-0.3.2/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.2/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     5860 2023-04-10 07:11:30.445800 langchain_utils-0.3.2/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1277 2023-04-10 06:26:58.124248 langchain_utils-0.3.2/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     1496 2023-04-10 07:12:48.292328 langchain_utils-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5591 1970-01-01 00:00:00.000000 langchain_utils-0.3.2/PKG-INFO
```

### Comparing `langchain_utils-0.3.1/README.md` & `langchain_utils-0.3.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 ```
 
 ### `pdfprompt`
 
 ```
 $ pdfprompt --help
 
-usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-n] [-M]
-                 [-w WHAT]
+usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-n]
+                 [-p PAGES [PAGES ...]] [-M] [-w WHAT]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
@@ -75,20 +75,23 @@
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
   -S, --split           Split the prompt into multiple parts (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split (default: 2000)
   -n, --dry-run         Dry run (default: False)
+  -p PAGES [PAGES ...], --pages PAGES [PAGES ...]
+                        Only include specified page numbers (default: None)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a PDF
                         file)
 
+
 ```
 
 ### `ytprompt`
 
 ```
 $ ytprompt --help
```

### Comparing `langchain_utils-0.3.1/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.3.2/langchain_utils/get_pdf_prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,22 @@
         description='Get a prompt consisting the text content of a PDF file'
     )
 
     parser.add_argument(
         'pdf_path', help='Path to the PDF file', metavar='PDF Path', type=str
     )
     parser.add_argument(
+        '-p',
+        '--pages',
+        help='Only include specified page numbers',
+        type=int,
+        nargs='+',
+        default=None,
+    )
+    parser.add_argument(
         '-M',
         '--merge',
         help='Merge contents of all pages before processing',
         action='store_true',
     )
     parser.add_argument(
         '-w',
@@ -49,14 +57,18 @@
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
 
     print(f'Loading PDF from {args.pdf_path} ...', file=sys.stderr)
     docs = load_pdf(args.pdf_path)
+    num_whole_pdf_pages = len(docs)
+    if args.pages:
+        args.pages = [p for p in args.pages if p <= num_whole_pdf_pages and p > 0]
+        docs = [doc for doc in docs if doc.metadata['page_number'] in args.pages]
     texts = [doc.page_content for doc in docs]
     all_text = '\n'.join(texts)
     word_count = get_word_count((all_text))
     print(
         f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
         file=sys.stderr,
     )
```

### Comparing `langchain_utils-0.3.1/langchain_utils/get_url_prompt.py` & `langchain_utils-0.3.2/langchain_utils/get_url_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.1/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.3.2/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.1/langchain_utils/loaders.py` & `langchain_utils-0.3.2/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.1/langchain_utils/utils.py` & `langchain_utils-0.3.2/langchain_utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
         else:
             print(formatted_prompt)
 
     def deliver_multiple_docs(documents: list['Document']):
         if edit:
             print(f'Please copy the prompts after each edits.', file=sys.stderr)
         for i, doc in enumerate(documents):
+            num_chunks = len(documents)
             if i == 0:
                 prompt = PromptTemplate.from_template(
                     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_FIRST
                 )
             else:
                 prompt = PromptTemplate.from_template(
                     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_CONTINUED
@@ -162,15 +163,14 @@
             't need to press Enter to move forward.'
         )
     if needs_splitting:
         from langchain.text_splitter import TokenTextSplitter
 
         splitter = TokenTextSplitter(encoding_name='cl100k_base', chunk_size=chunk_size)
         splitted = splitter.split_documents(documents)
-        num_chunks = len(splitted)
         deliver_multiple_docs(splitted)
 
     elif should_be_only_one_doc:
         deliver_single_doc(documents[0])
     else:
         deliver_multiple_docs(documents)
```

### Comparing `langchain_utils-0.3.1/langchain_utils/utils_argparse.py` & `langchain_utils-0.3.2/langchain_utils/utils_argparse.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.1/pyproject.toml` & `langchain_utils-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.3.1/PKG-INFO` & `langchain_utils-0.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -80,16 +80,16 @@
 ```
 
 ### `pdfprompt`
 
 ```
 $ pdfprompt --help
 
-usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-n] [-M]
-                 [-w WHAT]
+usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-n]
+                 [-p PAGES [PAGES ...]] [-M] [-w WHAT]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
@@ -101,20 +101,23 @@
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
   -S, --split           Split the prompt into multiple parts (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split (default: 2000)
   -n, --dry-run         Dry run (default: False)
+  -p PAGES [PAGES ...], --pages PAGES [PAGES ...]
+                        Only include specified page numbers (default: None)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a PDF
                         file)
 
+
 ```
 
 ### `ytprompt`
 
 ```
 $ ytprompt --help
```

