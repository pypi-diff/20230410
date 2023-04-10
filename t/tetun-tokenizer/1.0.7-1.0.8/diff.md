# Comparing `tmp/tetun_tokenizer-1.0.7.tar.gz` & `tmp/tetun_tokenizer-1.0.8.tar.gz`

## Comparing `tetun_tokenizer-1.0.7.tar` & `tetun_tokenizer-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/.DS_Store
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/Pipfile
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/Pipfile.lock
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/_token
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/tetuntokenizer/__init__.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/tetuntokenizer/tokenizer.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/LICENSE
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/README.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/.DS_Store
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/Pipfile
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/Pipfile.lock
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/_token
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/tetuntokenizer/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/tetuntokenizer/tokenizer.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/LICENSE
+-rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/README.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 tetun_tokenizer-1.0.8/PKG-INFO
```

### Comparing `tetun_tokenizer-1.0.7/.DS_Store` & `tetun_tokenizer-1.0.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.0.7/tetuntokenizer/tokenizer.py` & `tetun_tokenizer-1.0.8/tetuntokenizer/tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import List
 
 PUNCTUATIONS = '.,:;?!-"“”/\\<>()[]{}'
 SPECIAL_CHARS = '#$€%@*&_|=+^`~<<>>'
 
 
 class TetunRegexTokenizer:
-    """Tokenizes a string (or text) using regular expressions."""
+    """Tokenizes a text using regular expressions."""
 
     def __init__(self, patterns: str, split: bool = False) -> None:
         """
         :param patterns: a regular expression to match the tokens.
         :param split: if True, use re.split() to tokenize text, else use re.findall().            
         """
         self.patterns = patterns
@@ -38,58 +38,66 @@
             tokens = re.split(self.patterns, text)
         else:
             tokens = re.findall(self.patterns, text)
         return tokens
 
 
 class TetunStandardTokenizer(TetunRegexTokenizer):
-    """ Tokenize a string (or text) by word, punctuations, and special characters delimiters. """
+    """ Tokenize a text by word, punctuations, or special characters delimiters. """
 
     def __init__(self) -> None:
         patterns = (
-            # e.g.: Área, área, ne'e, Ne'ebé, kompañia, ida-ne'e, ida-ne'ebé, etc.
+            # e.g.: Área, área, ne'e, Ne'ebé, kompañia, ida-ne'e, ida-ne'ebé.
             # e.g. person names: Ângelo, Adão, Érica, etc.
             r"[A-Za-zÂÁáãéêÉÊíÍóÓúÚñç]+(?:[-’'][A-Za-zÂÁáãéêÉÊíÍóÓúÚñç]+)*"
             r"|"
             r"[\d]+[\.\d]*[\,\d]*"
             r"|"
             r"[" + re.escape("".join(PUNCTUATIONS + SPECIAL_CHARS)) + "]"
         )
         super().__init__(patterns)
 
 
 class TetunWhiteSpaceTokenizer(TetunRegexTokenizer):
-    """ Tokenize text by whitespace delimiter. """
+    """ Tokenize a text by whitespace delimiter. """
 
     def __init__(self) -> None:
         patterns = r"\s+"
         super().__init__(patterns, split=True)
 
 
+class TetunSentenceTokenizer(TetunRegexTokenizer):
+    """ Tokenize a text by .?! delimiters. """
+
+    def __init__(self) -> None:
+        patterns = r"(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?|\!)\s"
+        super().__init__(patterns, split=True)
+
+
 class TetunBlankLineTokenizer(TetunRegexTokenizer):
-    """ Tokenize a string (or text), treating any sequence of blank lines as a delimiter. """
+    """ Tokenize a text, treating any sequence of blank lines as a delimiter. """
 
     def __init__(self) -> None:
         patterns = r"s*\n\s*\n\s*"
         super().__init__(patterns, split=True)
 
 
 class TetunSimpleTokenizer(TetunRegexTokenizer):
-    """ Tokenize a string (or text) and numbers and ignore punctuations and special characters. """
+    """ Tokenize strings and numbers and ignore punctuations and special characters. """
 
     def __init__(self) -> None:
         patterns = (
             r"[A-Za-zÂÁáãéêÉÊíÍóÓúÚñç]+(?:[-’'][A-Za-zÂÁáãéêÉÊíÍóÓúÚñç]+)*"
             r"|"
             r"[\d]+[\.\d]*[\,\d]*"
         )
         super().__init__(patterns)
 
 
 class TetunWordTokenizer(TetunRegexTokenizer):
-    """ Tokenize a string (or text) and ignore numbers, punctuations and special characters. """
+    """ Tokenize strings and ignore numbers, punctuations and special characters. """
 
     def __init__(self) -> None:
         patterns = (
             r"[A-Za-zÂÁáãéêÉÊíÍóÓúÚñç]+(?:[-’'][A-Za-zÂÁáãéêÉÊíÍóÓúÚñç]+)*"
         )
         super().__init__(patterns)
```

### Comparing `tetun_tokenizer-1.0.7/LICENSE` & `tetun_tokenizer-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.0.7/README.md` & `tetun_tokenizer-1.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 ### Tetun Tokenizer
 
 Tetun tokenizer is a Python package for tokenizing an input text into tokens. There are several tokenization techniques we built alongside this package as follows:
 1. `TetunStandardTokenizer()`: tokenize the input text by `word`, `punctuations`, and `special characters`.
 2. `TetunWhiteSpaceTokenizer()`: tokenize the input text by `whitespace` delimiter.
-3. `TetunBlankLineTokenizer()`: tokenize the input text by `blank lines` delimiter.
-4. `TetunSimpleTokenizer()`: tokenize the input text by extracting `only string and number` and ignore punctuations and special characters.
-5. `TetunWordTokenizer()`: tokenize the input text by extracting `only string` and ignore numbers, punctuations, and special characters.
+3. `TetunSentenceTokenizer()`: tokenize the input text by `.?!` delimiters.
+4. `TetunBlankLineTokenizer()`: tokenize the input text by `blank lines` delimiter.
+5. `TetunSimpleTokenizer()`: tokenize the input text by extracting `only string and number` and ignore punctuations and special characters.
+6. `TetunWordTokenizer()`: tokenize the input text by extracting `only string` and ignore numbers, punctuations, and special characters.
 
 ### Installation
 
 To install Tetun tokenizer, run the following command in your console:
 
 ```
 python3 -m pip install tetun-tokenizer
@@ -60,15 +61,33 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak.", "Ha'u", 'iha', '$0.25', 'atu', 'fó', 'ba', 'ita.']
 ```
 
-3. Using `TetunBlankLineTokenizer()` to tokenize a given text.
+3. Using `TetunSentenceTokenizer()` to tokenize a given text.
+
+```python
+from tetuntokenizer.tokenizer import TetunSentenceTokenizer
+
+tetun_tokenizer = TetunSentenceTokenizer()
+
+text = "Ha'u ema-ida ne'ebé baibain de'it. Tebes ká? Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!"
+output = tetun_tokenizer.tokenize(text)
+print(output)
+```
+
+The output will be:
+
+```
+["Ha'u ema-ida ne'ebé baibain de'it.", 'Tebes ká?', 'Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!']
+```
+
+4. Using `TetunBlankLineTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunBlankLineTokenizer
 
 tetun_tokenizer = TetunBlankLineTokenizer()
 
 text = """
@@ -81,15 +100,15 @@
 
 The output will be:
 
 ```
 ["\n            Ha'u mak ita-nia maluk di'ak.\n            Ha'u iha $0.25 atu fó ba ita.\n            "]
 ```
 
-4. Using `TetunSimpleTokenizer()` to tokenize a given text.
+5. Using `TetunSimpleTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunSimpleTokenizer
 
 tetun_tokenizer = TetunSimpleTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
@@ -99,15 +118,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", "Ha'u", 'iha', '0.25', 'atu', 'fó', 'ba', 'ita']
 ```
 
-5. Using `TetunWordTokenizer()` to tokenize a given text.
+6. Using `TetunWordTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunWordTokenizer
 
 tetun_tokenizer = TetunWordTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
```

### Comparing `tetun_tokenizer-1.0.7/PKG-INFO` & `tetun_tokenizer-1.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: tetun_tokenizer
-Version: 1.0.7
+Version: 1.0.8
 Summary: Tetun tokenizer
 Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ### Tetun Tokenizer
 
 Tetun tokenizer is a Python package for tokenizing an input text into tokens. There are several tokenization techniques we built alongside this package as follows:
 1. `TetunStandardTokenizer()`: tokenize the input text by `word`, `punctuations`, and `special characters`.
 2. `TetunWhiteSpaceTokenizer()`: tokenize the input text by `whitespace` delimiter.
-3. `TetunBlankLineTokenizer()`: tokenize the input text by `blank lines` delimiter.
-4. `TetunSimpleTokenizer()`: tokenize the input text by extracting `only string and number` and ignore punctuations and special characters.
-5. `TetunWordTokenizer()`: tokenize the input text by extracting `only string` and ignore numbers, punctuations, and special characters.
+3. `TetunSentenceTokenizer()`: tokenize the input text by `.?!` delimiters.
+4. `TetunBlankLineTokenizer()`: tokenize the input text by `blank lines` delimiter.
+5. `TetunSimpleTokenizer()`: tokenize the input text by extracting `only string and number` and ignore punctuations and special characters.
+6. `TetunWordTokenizer()`: tokenize the input text by extracting `only string` and ignore numbers, punctuations, and special characters.
 
 ### Installation
 
 To install Tetun tokenizer, run the following command in your console:
 
 ```
 python3 -m pip install tetun-tokenizer
@@ -72,15 +73,33 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak.", "Ha'u", 'iha', '$0.25', 'atu', 'fó', 'ba', 'ita.']
 ```
 
-3. Using `TetunBlankLineTokenizer()` to tokenize a given text.
+3. Using `TetunSentenceTokenizer()` to tokenize a given text.
+
+```python
+from tetuntokenizer.tokenizer import TetunSentenceTokenizer
+
+tetun_tokenizer = TetunSentenceTokenizer()
+
+text = "Ha'u ema-ida ne'ebé baibain de'it. Tebes ká? Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!"
+output = tetun_tokenizer.tokenize(text)
+print(output)
+```
+
+The output will be:
+
+```
+["Ha'u ema-ida ne'ebé baibain de'it.", 'Tebes ká?', 'Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!']
+```
+
+4. Using `TetunBlankLineTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunBlankLineTokenizer
 
 tetun_tokenizer = TetunBlankLineTokenizer()
 
 text = """
@@ -93,15 +112,15 @@
 
 The output will be:
 
 ```
 ["\n            Ha'u mak ita-nia maluk di'ak.\n            Ha'u iha $0.25 atu fó ba ita.\n            "]
 ```
 
-4. Using `TetunSimpleTokenizer()` to tokenize a given text.
+5. Using `TetunSimpleTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunSimpleTokenizer
 
 tetun_tokenizer = TetunSimpleTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
@@ -111,15 +130,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", "Ha'u", 'iha', '0.25', 'atu', 'fó', 'ba', 'ita']
 ```
 
-5. Using `TetunWordTokenizer()` to tokenize a given text.
+6. Using `TetunWordTokenizer()` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunWordTokenizer
 
 tetun_tokenizer = TetunWordTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
```

