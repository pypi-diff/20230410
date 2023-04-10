# Comparing `tmp/story_analyzer-0.1.2.tar.gz` & `tmp/story_analyzer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_analyzer-0.1.2.tar", max compression
+gzip compressed data, was "story_analyzer-0.1.3.tar", max compression
```

## Comparing `story_analyzer-0.1.2.tar` & `story_analyzer-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1082 2023-04-10 20:30:17.612223 story_analyzer-0.1.2/LICENSE
--rw-r--r--   0        0        0     2303 2023-04-09 19:41:23.674378 story_analyzer-0.1.2/README.md
--rw-r--r--   0        0        0      712 2023-04-10 21:01:46.851172 story_analyzer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       38 2023-04-10 20:30:17.615556 story_analyzer-0.1.2/story_analyzer/__init__.py
--rw-r--r--   0        0        0      816 2023-04-10 20:58:06.240535 story_analyzer-0.1.2/story_analyzer/archiver.py
--rw-r--r--   0        0        0     9251 2023-04-10 15:04:00.856672 story_analyzer-0.1.2/story_analyzer/book.py
--rw-r--r--   0        0        0       93 2023-04-06 14:36:21.725515 story_analyzer-0.1.2/story_analyzer/data/spacy_models
--rw-r--r--   0        0        0     2943 2023-04-09 19:41:23.677713 story_analyzer-0.1.2/story_analyzer/get_book.py
--rw-r--r--   0        0        0     8157 2023-04-10 20:11:15.818055 story_analyzer-0.1.2/story_analyzer/main.py
--rw-r--r--   0        0        0   534065 2023-04-10 21:00:45.654329 story_analyzer-0.1.2/story_analyzer/out.json
--rw-r--r--   0        0        0      682 2023-04-10 20:30:17.615556 story_analyzer-0.1.2/story_analyzer/parser_models.py
--rw-r--r--   0        0        0     4314 2023-04-10 15:01:04.825619 story_analyzer-0.1.2/story_analyzer/spacy_queries.py
--rw-r--r--   0        0        0        0 2023-04-06 10:18:52.894916 story_analyzer-0.1.2/story_analyzer/tests/__init__.py
--rw-r--r--   0        0        0      422 2023-04-10 19:09:07.390682 story_analyzer-0.1.2/story_analyzer/tests/test_archiver.py
--rw-r--r--   0        0        0      406 2023-04-07 20:53:38.458655 story_analyzer-0.1.2/story_analyzer/tests/test_spacy_queries.py
--rw-r--r--   0        0        0     3363 1970-01-01 00:00:00.000000 story_analyzer-0.1.2/setup.py
--rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 story_analyzer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-10 20:30:17.612223 story_analyzer-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2303 2023-04-09 19:41:23.674378 story_analyzer-0.1.3/README.md
+-rw-r--r--   0        0        0      712 2023-04-10 21:06:17.868607 story_analyzer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-04-10 20:30:17.615556 story_analyzer-0.1.3/story_analyzer/__init__.py
+-rw-r--r--   0        0        0      774 2023-04-10 21:05:39.038498 story_analyzer-0.1.3/story_analyzer/archiver.py
+-rw-r--r--   0        0        0     9251 2023-04-10 15:04:00.856672 story_analyzer-0.1.3/story_analyzer/book.py
+-rw-r--r--   0        0        0       93 2023-04-06 14:36:21.725515 story_analyzer-0.1.3/story_analyzer/data/spacy_models
+-rw-r--r--   0        0        0     2943 2023-04-09 19:41:23.677713 story_analyzer-0.1.3/story_analyzer/get_book.py
+-rw-r--r--   0        0        0     8157 2023-04-10 20:11:15.818055 story_analyzer-0.1.3/story_analyzer/main.py
+-rw-r--r--   0        0        0   534065 2023-04-10 21:00:45.654329 story_analyzer-0.1.3/story_analyzer/out.json
+-rw-r--r--   0        0        0      682 2023-04-10 20:30:17.615556 story_analyzer-0.1.3/story_analyzer/parser_models.py
+-rw-r--r--   0        0        0     4314 2023-04-10 15:01:04.825619 story_analyzer-0.1.3/story_analyzer/spacy_queries.py
+-rw-r--r--   0        0        0        0 2023-04-06 10:18:52.894916 story_analyzer-0.1.3/story_analyzer/tests/__init__.py
+-rw-r--r--   0        0        0      422 2023-04-10 19:09:07.390682 story_analyzer-0.1.3/story_analyzer/tests/test_archiver.py
+-rw-r--r--   0        0        0      406 2023-04-07 20:53:38.458655 story_analyzer-0.1.3/story_analyzer/tests/test_spacy_queries.py
+-rw-r--r--   0        0        0     3363 1970-01-01 00:00:00.000000 story_analyzer-0.1.3/setup.py
+-rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 story_analyzer-0.1.3/PKG-INFO
```

### Comparing `story_analyzer-0.1.2/LICENSE` & `story_analyzer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `story_analyzer-0.1.2/README.md` & `story_analyzer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `story_analyzer-0.1.2/pyproject.toml` & `story_analyzer-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "story-analyzer"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = [
     "Francisco Alexandre Neves <pg50375@alunos.uminho.pt>",
     "Henrique Parola Costa <pg50415@alunos.uminho.pt>",
     "José Pedro Fernandes <pg50525@alunos.uminho.pt>"
 ]
 readme = "README.md"
```

### Comparing `story_analyzer-0.1.2/story_analyzer/archiver.py` & `story_analyzer-0.1.3/story_analyzer/archiver.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import copy
 class Archiver:
     def __init__(self):
         self.home = os.path.expanduser("~")
         self.path: str = os.path.join(self.home, ".story", "db", "archive")
 
     def addStory(self, title: str, bookObj : dict):
-        print(os.path.dirname(self.path))
         os.makedirs(os.path.dirname(self.path), exist_ok=True)
         db: Shelf = shelve.open(self.path)
         if title in db.keys():
             copyDict : dict = copy.deepcopy(db[title])
             copyDict.update(bookObj)
             db[title] = copyDict
         else:
```

### Comparing `story_analyzer-0.1.2/story_analyzer/book.py` & `story_analyzer-0.1.3/story_analyzer/book.py`

 * *Files identical despite different names*

### Comparing `story_analyzer-0.1.2/story_analyzer/get_book.py` & `story_analyzer-0.1.3/story_analyzer/get_book.py`

 * *Files identical despite different names*

### Comparing `story_analyzer-0.1.2/story_analyzer/main.py` & `story_analyzer-0.1.3/story_analyzer/main.py`

 * *Files identical despite different names*

### Comparing `story_analyzer-0.1.2/story_analyzer/out.json` & `story_analyzer-0.1.3/story_analyzer/out.json`

 * *Files identical despite different names*

### Comparing `story_analyzer-0.1.2/story_analyzer/parser_models.py` & `story_analyzer-0.1.3/story_analyzer/parser_models.py`

 * *Files identical despite different names*

### Comparing `story_analyzer-0.1.2/story_analyzer/spacy_queries.py` & `story_analyzer-0.1.3/story_analyzer/spacy_queries.py`

 * *Files identical despite different names*

### Comparing `story_analyzer-0.1.2/setup.py` & `story_analyzer-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'transformers>=4.27.4,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['story_analyzer = story_analyzer.main:main']}
 
 setup_kwargs = {
     'name': 'story-analyzer',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '# Story Analyzer\n\nGet all the details of a story. From summaries to character information, explore your book like never before!\n\n![Banner](banner.jpg)\n\n## Features\n\n* Quiz game\n* Translation \n* Summarization  \n* Most relevant topics\n* Characteres list \n* Lines list\n* Number of sentences\n* Match of input phrase with a storie excert\n\n## Usage\n\n```\nusage: main.py [-h] [-m {local,web}] [-q] [-t [{English,Spanish,French,German,Italian,Portuguese}]] [-d] [-s] [-l] [-c] [-a [ACTIONS]]\n               [--save title] [-p PROJECTION]\n               input output\n\nBook Analyzer: get insight informations of your storie\n\npositional arguments:\n  input                 input file path or book name (only in web mode)\n  output                output file path\n\noptions:\n  -h, --help            show this help message and exit\n  -m {local,web}, --mode {local,web}\n                        app modes\n  -q, --quiz            quiz game\n  -t [{English,Spanish,French,German,Italian,Portuguese}], --translate [{English,Spanish,French,German,Italian,Portuguese}]\n                        translate the book\n  -d, --discussions     list the book discussions (topics)\n  -s, --summary         summarize the book\n  -l, --language        detect book language\n  -c, --characters      get informations of the book characters\n  -a [ACTIONS], --actions [ACTIONS]\n                        get the top most actions of a book\n  --save title          the book will be saved and so will any queries invoked deemed savable.\n  -p PROJECTION, --projection PROJECTION\n                        project queries in the text range. Projection type is [<bottom>;<higher>]\n  -sa, --sentiment-analysis\n                        get the sentiment analysis of the book\n```\n\n## Dependencies\n\n* Quiz game is made with https://huggingface.co/gpt2\n* Transaltion is made with https://huggingface.co/docs/transformers/main/en/model_doc/t5#overview\n* Summarization is made with https://huggingface.co/docs/transformers/model_doc/pegasus\n* Most Relevent Topics is made with https://radimrehurek.com/gensim/\n* Language detection is made with https://huggingface.co/papluca/xlm-roberta-base-language-detection\n* Actions, Characters and places list is made with https://spacy.io/\n* HTML extraction is made with https://www.crummy.com/software/BeautifulSoup/bs4/doc/',
     'author': 'Francisco Alexandre Neves',
     'author_email': 'pg50375@alunos.uminho.pt',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `story_analyzer-0.1.2/PKG-INFO` & `story_analyzer-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: story-analyzer
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: Francisco Alexandre Neves
 Author-email: pg50375@alunos.uminho.pt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

