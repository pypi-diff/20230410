# Comparing `tmp/langchain_utils-0.1.4.tar.gz` & `tmp/langchain_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.1.4.tar", max compression
+gzip compressed data, was "langchain_utils-0.1.5.tar", max compression
```

## Comparing `langchain_utils-0.1.4.tar` & `langchain_utils-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.4/README.md
--rw-r--r--   0        0        0       22 2023-04-10 02:05:55.970644 langchain_utils-0.1.4/langchain_utils/__init__.py
--rw-r--r--   0        0        0       71 2023-04-09 15:21:28.583065 langchain_utils-0.1.4/langchain_utils/config.py
--rwxr-xr-x   0        0        0     2961 2023-04-10 02:03:10.281229 langchain_utils-0.1.4/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2675 2023-04-09 15:13:41.939409 langchain_utils-0.1.4/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0      559 2023-04-09 15:13:17.822169 langchain_utils-0.1.4/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.1.4/langchain_utils/prompts.py
--rw-r--r--   0        0        0     2857 2023-04-09 15:03:48.493911 langchain_utils-0.1.4/langchain_utils/utils.py
--rw-r--r--   0        0        0     1244 2023-04-10 02:05:55.969971 langchain_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 langchain_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.5/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 02:20:20.575610 langchain_utils-0.1.5/langchain_utils/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-09 15:21:28.583065 langchain_utils-0.1.5/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     3170 2023-04-10 02:19:48.885856 langchain_utils-0.1.5/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     2786 2023-04-10 02:19:30.567185 langchain_utils-0.1.5/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0      559 2023-04-09 15:13:17.822169 langchain_utils-0.1.5/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.1.5/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     3678 2023-04-10 02:18:58.686955 langchain_utils-0.1.5/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1244 2023-04-10 02:20:20.575174 langchain_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 langchain_utils-0.1.5/PKG-INFO
```

### Comparing `langchain_utils-0.1.4/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.1.5/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,26 @@
 Purpose: Get a prompt consisting Title and Transcript of a YouTube Video
 """
 
 import argparse
 import sys
 
 from .utils import deliver_prompts, format_date, get_word_count, deliver_prompts
-from .loaders import load_pdf
-from .config import DEFAULT_PDF_WHAT
+from .loaders import load_youtube_url
 
 
 def get_args():
     """Get command-line arguments"""
 
     parser = argparse.ArgumentParser(
         description='Get a prompt consisting Title and Transcript of a YouTube Video',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
-    parser.add_argument(
-        'pdf_path', help='Path to the PDF file', metavar='PDF Path', type=str
-    )
+    parser.add_argument('youtube_url', metavar='YouTube URL', help='YouTube URL')
     parser.add_argument(
         '-c', '--copy', help='Copy the prompt to clipboard', action='store_true'
     )
     parser.add_argument(
         '-m',
         '--model',
         help='Model to use',
@@ -45,58 +42,51 @@
         '-s',
         '--chunk-size',
         help='Chunk size when splitting transcript, also used to determine whether to split',
         metavar='chunk_size',
         type=int,
         default=2000,
     )
-    parser.add_argument(
-        '-w',
-        '--what',
-        help='Initial knowledge you want to insert before the PDF content in the prompt',
-        type=str,
-        default=DEFAULT_PDF_WHAT,
-    )
+
+    parser.add_argument('-n', '--dry-run', help='Dry run', action='store_true')
 
     args = parser.parse_args()
+    args.youtube_url = args.youtube_url.split('&')[0]
     return args
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
-
-    print(f'Loading PDF from {args.pdf_path} ...', file=sys.stderr)
-    docs = load_pdf(args.pdf_path)
-    texts = [doc.page_content for doc in docs]
-    all_text = '\n'.join(texts)
-    word_count = get_word_count((all_text))
+    print(f'Loading transcript from {args.youtube_url} ...', file=sys.stderr)
+    docs = load_youtube_url(args.youtube_url)
     print(
-        f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
+        f'Loaded transcript. Word count: {get_word_count((t := docs[0].page_content))} Char count: {len(t)}',
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
+    metadata = docs[0].metadata
+    title = metadata['title']
+    author = metadata['author']
+    publish_date = format_date(metadata['publish_date'])
+    what = f'''the transcript of a YouTube video titled "{title}" uploaded by "{author}" on {publish_date}'''
+    print(f'Title: {title}', file=sys.stderr)
+    print(f'Author: {author}', file=sys.stderr)
+    print(f'Publish date: {publish_date}', file=sys.stderr)
     # if args.split or get_token_count(docs[0].page_content) > args.chunk_size:
-    if args.split or word_count > args.chunk_size * 0.75:
+    if args.split or get_word_count(docs[0].page_content) > args.chunk_size * 0.75:
         needs_splitting = True
     else:
         needs_splitting = False
     deliver_prompts(
-        what=args.what,
+        what=what,
         docs=docs,
         should_be_only_one_doc=True,
         needs_splitting=needs_splitting,
         copy=args.copy,
         chunk_size=args.chunk_size,
+        dry_run=args.dry_run,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.1.4/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.1.5/langchain_utils/get_pdf_prompt.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,27 +4,36 @@
 Date   : 2023-04-09
 Purpose: Get a prompt consisting Title and Transcript of a YouTube Video
 """
 
 import argparse
 import sys
 
-from .utils import deliver_prompts, format_date, get_word_count, deliver_prompts
-from .loaders import load_youtube_url
+from .utils import (
+    deliver_prompts,
+    format_date,
+    get_word_count,
+    deliver_prompts,
+    pymupdf_doc_page_info,
+)
+from .loaders import load_pdf
+from .config import DEFAULT_PDF_WHAT
 
 
 def get_args():
     """Get command-line arguments"""
 
     parser = argparse.ArgumentParser(
         description='Get a prompt consisting Title and Transcript of a YouTube Video',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
-    parser.add_argument('youtube_url', metavar='YouTube URL', help='YouTube URL')
+    parser.add_argument(
+        'pdf_path', help='Path to the PDF file', metavar='PDF Path', type=str
+    )
     parser.add_argument(
         '-c', '--copy', help='Copy the prompt to clipboard', action='store_true'
     )
     parser.add_argument(
         '-m',
         '--model',
         help='Model to use',
@@ -42,48 +51,61 @@
         '-s',
         '--chunk-size',
         help='Chunk size when splitting transcript, also used to determine whether to split',
         metavar='chunk_size',
         type=int,
         default=2000,
     )
+    parser.add_argument(
+        '-w',
+        '--what',
+        help='Initial knowledge you want to insert before the PDF content in the prompt',
+        type=str,
+        default=DEFAULT_PDF_WHAT,
+    )
+    parser.add_argument('-n', '--dry-run', help='Dry run', action='store_true')
 
     args = parser.parse_args()
-    args.youtube_url = args.youtube_url.split('&')[0]
     return args
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
-    print(f'Loading transcript from {args.youtube_url} ...', file=sys.stderr)
-    docs = load_youtube_url(args.youtube_url)
+
+    print(f'Loading PDF from {args.pdf_path} ...', file=sys.stderr)
+    docs = load_pdf(args.pdf_path)
+    texts = [doc.page_content for doc in docs]
+    all_text = '\n'.join(texts)
+    word_count = get_word_count((all_text))
     print(
-        f'Loaded transcript. Word count: {get_word_count((t := docs[0].page_content))} Char count: {len(t)}',
+        f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
         file=sys.stderr,
     )
-    metadata = docs[0].metadata
-    title = metadata['title']
-    author = metadata['author']
-    publish_date = format_date(metadata['publish_date'])
-    what = f'''the transcript of a YouTube video titled "{title}" uploaded by "{author}" on {publish_date}'''
-    print(f'Title: {title}', file=sys.stderr)
-    print(f'Author: {author}', file=sys.stderr)
-    print(f'Publish date: {publish_date}', file=sys.stderr)
+    # metadata = docs[0].metadata
+    # title = metadata['title']
+    # author = metadata['author']
+    # publish_date = format_date(metadata['publish_date'])
+    # what = f'''the transcript of a YouTube video titled "{title}" uploaded by "{author}" on {publish_date}'''
+    # print(f'Title: {title}', file=sys.stderr)
+    # print(f'Author: {author}', file=sys.stderr)
+    # print(f'Publish date: {publish_date}', file=sys.stderr)
     # if args.split or get_token_count(docs[0].page_content) > args.chunk_size:
-    if args.split or get_word_count(docs[0].page_content) > args.chunk_size * 0.75:
+    if args.split or word_count > args.chunk_size * 0.75:
         needs_splitting = True
     else:
         needs_splitting = False
     deliver_prompts(
-        what=what,
+        what=args.what,
         docs=docs,
         should_be_only_one_doc=True,
         needs_splitting=needs_splitting,
         copy=args.copy,
         chunk_size=args.chunk_size,
+        extra_chunk_info_fn=pymupdf_doc_page_info,
+        dry_run=args.dry_run,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.1.4/langchain_utils/loaders.py` & `langchain_utils-0.1.5/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.1.4/langchain_utils/utils.py` & `langchain_utils-0.1.5/langchain_utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable
 import sys
 from .prompts import (
     REPLY_OK_IF_YOU_READ_TEMPLATE,
     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_FIRST,
     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_CONTINUED,
 )
 
@@ -28,62 +28,80 @@
     return len(s.split())
 
 
 def format_date(dt: 'datetime') -> str:
     return dt.strftime('%Y-%m-%d')
 
 
+def pymupdf_doc_page_info(document: 'Document') -> str:
+    metadata = document.metadata
+    return f', Page {metadata["page_number"]}/{metadata["total_pages"]}'
+
+
 def deliver_prompts(
     what: str,
     docs: list['Document'],
     should_be_only_one_doc: bool = False,
     needs_splitting: bool = False,
     copy: bool = True,
     chunk_size: int = 2000,
+    extra_chunk_info_fn: Callable[['Document'], str] = lambda doc: '',
+    dry_run: bool = False,
 ):
     from langchain.prompts import PromptTemplate
 
     def deliver_single_doc(document: 'Document'):
         prompt = PromptTemplate.from_template(REPLY_OK_IF_YOU_READ_TEMPLATE)
         content = document.page_content
         formatted_prompt = prompt.format(what=what, content=content)
         if copy:
-            import pyperclip
-
             print(
-                f'Word Count: {get_word_count(formatted_prompt)}, Char count: {len(formatted_prompt)}',
+                f'Word Count: {get_word_count(formatted_prompt)}, Char count: {len(formatted_prompt)}{extra_chunk_info_fn(document)}',
                 file=sys.stderr,
             )
-            pyperclip.copy(formatted_prompt)
-            print('Prompt copied to clipboard.', file=sys.stderr)
+            if not dry_run:
+                import pyperclip
+
+                pyperclip.copy(formatted_prompt)
+                print('Prompt copied to clipboard.', file=sys.stderr)
         else:
             print(formatted_prompt)
 
-    from langchain.text_splitter import TokenTextSplitter
-
     def deliver_multiple_docs(documents: list['Document']):
         for i, doc in enumerate(documents):
             if i == 0:
                 prompt = PromptTemplate.from_template(
                     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_FIRST
                 )
             else:
                 prompt = PromptTemplate.from_template(
                     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_CONTINUED
                 ).partial(x=str(i + 1))
             content = doc.page_content
             formatted_prompt = prompt.format(what=what, content=content)
+            if dry_run:
+                print(
+                    f'Press Enter to copy prompt {i+1}/{num_chunks}. Word Count: {get_word_count(formatted_prompt)}, Char count: {len(formatted_prompt)}{extra_chunk_info_fn(doc)}: '
+                )
+                continue
             input(
-                f'Press Enter to copy prompt {i+1}/{num_chunks}. Word Count: {get_word_count(formatted_prompt)}, Char count: {len(formatted_prompt)}: '
+                f'Press Enter to copy prompt {i+1}/{num_chunks}. Word Count: {get_word_count(formatted_prompt)}, Char count: {len(formatted_prompt)}{extra_chunk_info_fn(doc)}: '
             )
             import pyperclip
 
             pyperclip.copy(formatted_prompt)
 
+    if dry_run:
+        print(
+            f'Dry running. Nothing will be copied to your clipboard, and you don'
+            't need to press Enter to move forward.'
+        )
     if needs_splitting:
+        from langchain.text_splitter import TokenTextSplitter
+
         splitter = TokenTextSplitter(encoding_name='cl100k_base', chunk_size=chunk_size)
         splitted = splitter.split_documents(docs)
         num_chunks = len(splitted)
         deliver_multiple_docs(splitted)
 
     elif should_be_only_one_doc:
         deliver_single_doc(docs[0])
```

### Comparing `langchain_utils-0.1.4/pyproject.toml` & `langchain_utils-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.1.4/PKG-INFO` & `langchain_utils-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

