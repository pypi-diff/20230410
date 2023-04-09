# Comparing `tmp/promtstd-1.0.1.tar.gz` & `tmp/promtstd-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promtstd-1.0.1.tar", max compression
+gzip compressed data, was "promtstd-1.0.2.tar", max compression
```

## Comparing `promtstd-1.0.1.tar` & `promtstd-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    24421 2023-04-09 21:41:56.602431 promtstd-1.0.1/README.md
--rw-r--r--   0        0        0     1779 2023-04-09 21:19:05.190064 promtstd-1.0.1/promtstd/__main__.py
--rw-r--r--   0        0        0     2678 2023-04-09 21:18:15.362169 promtstd-1.0.1/promtstd/lib_linter.py
--rw-r--r--   0        0        0    11092 2023-04-09 21:07:09.223441 promtstd-1.0.1/promtstd/lib_main.py
--rw-r--r--   0        0        0     2996 2023-04-09 20:14:04.713460 promtstd-1.0.1/promtstd/lib_re.py
--rw-r--r--   0        0        0     3292 2023-04-09 19:37:17.459748 promtstd-1.0.1/promtstd/lib_types.py
--rw-r--r--   0        0        0     2644 2023-04-09 21:13:03.306803 promtstd-1.0.1/promtstd/test/test_main.py
--rw-r--r--   0        0        0      422 2023-04-09 21:05:56.003557 promtstd-1.0.1/promtstd/test/utils.py
--rw-r--r--   0        0        0     1390 2023-04-09 22:00:46.112538 promtstd-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    25641 1970-01-01 00:00:00.000000 promtstd-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    24578 2023-04-09 22:10:37.104524 promtstd-1.0.2/README.md
+-rw-r--r--   0        0        0     1779 2023-04-09 21:19:05.190064 promtstd-1.0.2/promtstd/__main__.py
+-rw-r--r--   0        0        0     2678 2023-04-09 21:18:15.362169 promtstd-1.0.2/promtstd/lib_linter.py
+-rw-r--r--   0        0        0    11092 2023-04-09 21:07:09.223441 promtstd-1.0.2/promtstd/lib_main.py
+-rw-r--r--   0        0        0     3003 2023-04-09 22:29:01.528981 promtstd-1.0.2/promtstd/lib_re.py
+-rw-r--r--   0        0        0     3292 2023-04-09 19:37:17.459748 promtstd-1.0.2/promtstd/lib_types.py
+-rw-r--r--   0        0        0     2644 2023-04-09 22:29:58.852930 promtstd-1.0.2/promtstd/test/test_main.py
+-rw-r--r--   0        0        0      422 2023-04-09 21:05:56.003557 promtstd-1.0.2/promtstd/test/utils.py
+-rw-r--r--   0        0        0     1390 2023-04-09 22:37:30.628305 promtstd-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    25798 1970-01-01 00:00:00.000000 promtstd-1.0.2/PKG-INFO
```

### Comparing `promtstd-1.0.1/README.md` & `promtstd-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 1. Оформление заголовков с нужными именами и уровнем для файле `Файл_С_Промтом.md`
 
   ```md
   # meta
   # doc
   # base_promt
   # tools
+  ## Название для вспомогательного прмота 1
+  ## Название для вспомогательного прмота ...
   # expl
   ## Название для примера запроса 1
   ### Название для примера ответа 1 
   ### Название для примера ответа ...
   ## Название для примера запроса 2
   ### Название для примера ответа 2
   ### Название для примера ответа ...
@@ -247,15 +249,15 @@
 
 1. Your first response will be to ask me what the prompt should be about. I will provide my answer, but we will need to improve it through continual iterations by going through the next steps.
 
 2. Based on my input, you will generate 3 sections. a) Revised prompt (provide your rewritten prompt. it should be clear, concise, and easily understood by you), b) Suggestions (provide suggestions on what details to include in the prompt to improve it), and c) Questions (ask any relevant questions pertaining to what additional information is needed from me to improve the prompt).
 
 3. We will continue this iterative process with me providing additional information to you and you updating the prompt in the Revised prompt section until it's complete.
 
-Задавай мне вопросы и пиши ответы на русском языке
+Задавай мне вопросы и пиши ответы на русском языке.
 ```
 
 # tools
 
 ## Если нужно модифицировать уже существующий промт, то напишите 2 сообщением
 
 ```promt
```

### Comparing `promtstd-1.0.1/promtstd/__main__.py` & `promtstd-1.0.2/promtstd/__main__.py`

 * *Files identical despite different names*

### Comparing `promtstd-1.0.1/promtstd/lib_linter.py` & `promtstd-1.0.2/promtstd/lib_linter.py`

 * *Files identical despite different names*

### Comparing `promtstd-1.0.1/promtstd/lib_main.py` & `promtstd-1.0.2/promtstd/lib_main.py`

 * *Files identical despite different names*

### Comparing `promtstd-1.0.1/promtstd/lib_re.py` & `promtstd-1.0.2/promtstd/lib_re.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class RePromt:
     """Класс который хранит регулярные выражения"""
 
     #
     ## Для парсинга Markdown
     #
     # ? Заголовок первого уровня
-    h1_pattern = r"(\n#{{1}} {header}\n)(?P<{group_name}>(.*\s*(?!#{{1}} ))+)"
+    h1_pattern = r"((?:\n|\A)#{{1}} {header}\n)(?P<{group_name}>(.*\s*(?!#{{1}} ))+)"
     # ? Комментарии в Markdown
     md_comment = compile(r"%[^%]+%")
     # ? Парсинг markdown словарей
     md_dict = compile(r"- (?P<key>[\w\d_ -]+)~(?P<value>[^\n]+)\n?")
     # ? Парсинг markdown списка
     md_list = compile(r"- (?P<is_select>\[x\] )?(?P<item>[^\n]+)")
     # ? Найти выбранные элементы списка
```

### Comparing `promtstd-1.0.1/promtstd/lib_types.py` & `promtstd-1.0.2/promtstd/lib_types.py`

 * *Files identical despite different names*

### Comparing `promtstd-1.0.1/promtstd/test/test_main.py` & `promtstd-1.0.2/promtstd/test/test_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         (
             Path("Написать программу на Python.md"),
             "16d759c4861baaf145f01c0557a001fa813532cd5e1e780ef372d96f7d2646b2",
             "bc5b2707b03165d4d3e427beb1eebaef6796e2a7ca6a2190050d3738d8dbae10",
         ),
         (
             Path("Создание промтов вместе с ChatGpt.md"),
-            "7aad7e05aaa03bad52c5fd4626f2c6519114ca6abdde11e9b2daeeee6b9365cc",
-            "7065e774d0a958706b20cd0011c0d7f2b8c577d844a94f8cd1ea6a3ed7edbeeb",
+            "13565a0d94fc8ee52038c74cf5e248c3ec0eb1e668b175ecb12b8ad759f0234b",
+            "9bbf0eeea796c29c093ceb90581558fac97022aee3e76e9e304e857ec08e618a",
         ),
         # ?
         # ? Сюда добавлять новые примеры тестовых файлов
         # ?
     ],
 )
 def test_parse_promt_md_to_json(file_in: Path, hash_in: str, hash_out: str):
```

### Comparing `promtstd-1.0.1/pyproject.toml` & `promtstd-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promtstd"
-version = "1.0.1"
+version = "1.0.2"
 description = "promtstd robot - универсальный стандарт для хранения и использования промтов в AI. books Основан на Markdown, обеспечивает легкость чтения и структурированность. "
 authors = ["Denis Kustov <pro-progerkustov@yandex.ru>"]
 readme = "README.md"
 homepage = "https://github.com/denisxab/promtstd"
 repository = "https://github.com/denisxab/promtstd"
 keywords=[
     "стандарт промтов",
```

### Comparing `promtstd-1.0.1/PKG-INFO` & `promtstd-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promtstd
-Version: 1.0.1
+Version: 1.0.2
 Summary: promtstd robot - универсальный стандарт для хранения и использования промтов в AI. books Основан на Markdown, обеспечивает легкость чтения и структурированность. 
 Home-page: https://github.com/denisxab/promtstd
 Keywords: стандарт промтов,promtstd,promt,ai,хранение промтов,использование промтов,разработка AI,искусственный интеллект,Markdown,унификация,структурирование,синтаксис,взаимодействие разработчиков,метаинформация,шаблоны,примеры,вспомогательные промты
 Author: Denis Kustov
 Author-email: pro-progerkustov@yandex.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -80,14 +80,16 @@
 1. Оформление заголовков с нужными именами и уровнем для файле `Файл_С_Промтом.md`
 
   ```md
   # meta
   # doc
   # base_promt
   # tools
+  ## Название для вспомогательного прмота 1
+  ## Название для вспомогательного прмота ...
   # expl
   ## Название для примера запроса 1
   ### Название для примера ответа 1 
   ### Название для примера ответа ...
   ## Название для примера запроса 2
   ### Название для примера ответа 2
   ### Название для примера ответа ...
@@ -263,15 +265,15 @@
 
 1. Your first response will be to ask me what the prompt should be about. I will provide my answer, but we will need to improve it through continual iterations by going through the next steps.
 
 2. Based on my input, you will generate 3 sections. a) Revised prompt (provide your rewritten prompt. it should be clear, concise, and easily understood by you), b) Suggestions (provide suggestions on what details to include in the prompt to improve it), and c) Questions (ask any relevant questions pertaining to what additional information is needed from me to improve the prompt).
 
 3. We will continue this iterative process with me providing additional information to you and you updating the prompt in the Revised prompt section until it's complete.
 
-Задавай мне вопросы и пиши ответы на русском языке
+Задавай мне вопросы и пиши ответы на русском языке.
 ```
 
 # tools
 
 ## Если нужно модифицировать уже существующий промт, то напишите 2 сообщением
 
 ```promt
```

