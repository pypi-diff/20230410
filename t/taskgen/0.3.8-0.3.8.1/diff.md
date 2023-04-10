# Comparing `tmp/taskgen-0.3.8.tar.gz` & `tmp/taskgen-0.3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen-0.3.8.tar", last modified: Sun Apr  9 20:55:28 2023, max compression
+gzip compressed data, was "taskgen-0.3.8.1.tar", last modified: Mon Apr 10 08:45:43 2023, max compression
```

## Comparing `taskgen-0.3.8.tar` & `taskgen-0.3.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-04-09 20:55:28.221231 taskgen-0.3.8/
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2632 2023-04-09 20:55:28.221047 taskgen-0.3.8/PKG-INFO
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2108 2023-02-25 14:50:29.000000 taskgen-0.3.8/README.md
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)       38 2023-04-09 20:55:28.221284 taskgen-0.3.8/setup.cfg
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     1293 2023-04-08 21:48:53.000000 taskgen-0.3.8/setup.py
-drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-04-09 20:55:28.219773 taskgen-0.3.8/taskgen/
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2390 2023-04-08 21:51:45.000000 taskgen-0.3.8/taskgen/__init__.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2128 2023-04-08 21:46:42.000000 taskgen-0.3.8/taskgen/config.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    16514 2023-04-09 20:53:57.000000 taskgen-0.3.8/taskgen/converters.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    14818 2023-04-09 20:25:40.000000 taskgen-0.3.8/taskgen/functions.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    10426 2023-04-09 17:48:01.000000 taskgen-0.3.8/taskgen/html.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    21693 2023-04-09 15:32:02.000000 taskgen-0.3.8/taskgen/main.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     8654 2023-04-08 21:41:31.000000 taskgen-0.3.8/taskgen/moodle.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     1633 2023-04-08 21:41:38.000000 taskgen-0.3.8/taskgen/stats.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     7072 2023-04-09 20:27:26.000000 taskgen-0.3.8/taskgen/tex.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      323 2023-04-09 20:20:45.000000 taskgen-0.3.8/taskgen/variable_types.py
-drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-04-09 20:55:28.220836 taskgen-0.3.8/taskgen.egg-info/
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2632 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/PKG-INFO
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      361 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/SOURCES.txt
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)        1 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/dependency_links.txt
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      175 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/requires.txt
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)        8 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/top_level.txt
+drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-04-10 08:45:43.339219 taskgen-0.3.8.1/
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2634 2023-04-10 08:45:43.339023 taskgen-0.3.8.1/PKG-INFO
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2108 2023-02-25 14:50:29.000000 taskgen-0.3.8.1/README.md
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)       38 2023-04-10 08:45:43.339273 taskgen-0.3.8.1/setup.cfg
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     1295 2023-04-10 08:35:16.000000 taskgen-0.3.8.1/setup.py
+drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-04-10 08:45:43.337774 taskgen-0.3.8.1/taskgen/
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2392 2023-04-10 08:35:09.000000 taskgen-0.3.8.1/taskgen/__init__.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2128 2023-04-08 21:46:42.000000 taskgen-0.3.8.1/taskgen/config.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    16161 2023-04-10 08:34:34.000000 taskgen-0.3.8.1/taskgen/converters.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    14818 2023-04-09 20:25:40.000000 taskgen-0.3.8.1/taskgen/functions.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    10426 2023-04-09 17:48:01.000000 taskgen-0.3.8.1/taskgen/html.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    21693 2023-04-09 15:32:02.000000 taskgen-0.3.8.1/taskgen/main.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     8824 2023-04-09 22:04:20.000000 taskgen-0.3.8.1/taskgen/moodle.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     1633 2023-04-08 21:41:38.000000 taskgen-0.3.8.1/taskgen/stats.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     7072 2023-04-09 20:27:26.000000 taskgen-0.3.8.1/taskgen/tex.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      323 2023-04-09 20:20:45.000000 taskgen-0.3.8.1/taskgen/variable_types.py
+drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-04-10 08:45:43.338780 taskgen-0.3.8.1/taskgen.egg-info/
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2634 2023-04-10 08:45:43.000000 taskgen-0.3.8.1/taskgen.egg-info/PKG-INFO
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      361 2023-04-10 08:45:43.000000 taskgen-0.3.8.1/taskgen.egg-info/SOURCES.txt
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)        1 2023-04-10 08:45:43.000000 taskgen-0.3.8.1/taskgen.egg-info/dependency_links.txt
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      175 2023-04-10 08:45:43.000000 taskgen-0.3.8.1/taskgen.egg-info/requires.txt
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)        8 2023-04-10 08:45:43.000000 taskgen-0.3.8.1/taskgen.egg-info/top_level.txt
```

### Comparing `taskgen-0.3.8/PKG-INFO` & `taskgen-0.3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskgen
-Version: 0.3.8
+Version: 0.3.8.1
 Summary: Ядро генератора банка задач на базе MiKTeX и Jupyter Notebook
 Home-page: https://github.com/artyom-zolotarevskiy/taskgen-core
 Author: Артём Золотаревский
 Author-email: artyom@zolotarevskiy.ru
 Project-URL: Bug Tracker, https://github.com/artyom-zolotarevskiy/taskgen-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `taskgen-0.3.8/README.md` & `taskgen-0.3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `taskgen-0.3.8/setup.py` & `taskgen-0.3.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         line
         for line in lineiter
         if line and not line.startswith("#") and not line.startswith("git+")
     ]
 
 
 setup(name='taskgen',
-      version='0.3.8',
+      version='0.3.8.1',
       author='Артём Золотаревский',
       author_email='artyom@zolotarevskiy.ru',
       description='Ядро генератора банка задач на базе MiKTeX и Jupyter Notebook',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/artyom-zolotarevskiy/taskgen-core',
       project_urls={
```

### Comparing `taskgen-0.3.8/taskgen/__init__.py` & `taskgen-0.3.8.1/taskgen/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,13 +34,13 @@
 from taskgen.variable_types import *
 from taskgen.main import *
 
 format = "%(asctime)s: %(message)s"
 logging.basicConfig(format=format, level=logging.INFO, datefmt="%H:%M:%S")
 
 __title__ = 'artyom-zolotarevskiy'
-__version__ = '0.3.8'
+__version__ = '0.3.8.1'
 __url__ = 'https://github.com/artyom-zolotarevskiy/taskgen-core'
 __author__ = 'Артём Золотаревский'
 __author_email__ = 'artyom@zolotarevskiy.ru'
 
 __all__ = ["config", "functions", "converters", "stats", "tex", "html", "moodle", "variable_types", "main"]
```

### Comparing `taskgen-0.3.8/taskgen/config.py` & `taskgen-0.3.8.1/taskgen/config.py`

 * *Files identical despite different names*

### Comparing `taskgen-0.3.8/taskgen/converters.py` & `taskgen-0.3.8.1/taskgen/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import json
 import base64
 import shutil
 import logging
 import shlex
 import subprocess as subp
+import time
 from binascii import crc32
 from PyPDF2 import PdfFileMerger, PdfFileReader
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
@@ -69,20 +70,17 @@
         print('Дожидаемся полной инициализации...')
 
         # дожидаемся загрузки страницы
         element = WebDriverWait(driver, 10).until(ec.presence_of_element_located((By.TAG_NAME, 'body')))
 
         # дожидаемся полной инициализации LaTex на странице
         WebDriverWait(driver, 10).until(__latex_is_loaded)
+        time.sleep(0.5)
 
         # получаем pdf
-
-        last_num_pages = -1
-        last_pdf_file = None
-
         print_options = {
             'scale': 1,
         }
 
         if in_one_page and 'with-solution' not in filename:
             print('Подбираем коэффициент масштабирования...')
             while 0.125 <= print_options['scale'] <= 1.975:
@@ -90,31 +88,22 @@
                 result = base64.b64decode(result['data'])
 
                 pdf_file = io.BytesIO(result)
                 pdf_reader = PdfFileReader(pdf_file)
                 num_pages = pdf_reader.numPages
                 # print('При масштабировании {} кол-во страниц: {}'.format(print_options['scale'], num_pages))
 
-                if last_num_pages > 1 and num_pages == 1:
-                    break
-                elif last_num_pages == 1 and num_pages == 2:
-                    result = last_pdf_file
+                if num_pages == 1:
                     break
-                elif num_pages == 1:
-                    print_options['scale'] += scale_step
                 else:
                     print_options['scale'] -= scale_step
-
-                last_num_pages = num_pages
-                last_pdf_file = result
         else:
             result = __send_devtools(driver, "Page.printToPDF", print_options)
             result = base64.b64decode(result['data'])
 
-
         # сохраняем pdf
         print('Сохраняем файл...', '\n')
         with open(os.path.join(output, os.path.splitext(filename)[0] + '.pdf'), 'wb') as file:
             file.write(result)
 
     driver.close()
     print('Все html файлы в директории', source, 'сконвертированы в pdf!')
@@ -342,8 +331,8 @@
             # список всех файлов с подстановками
             subs_files_list = glob.glob(os.path.join(substitutions_directory, 'substitution_*.tex'))
             merged_latex_file = merge_tex(subs_files_list)
             # сохраняем объединенный файл подстановок
             with open(os.path.join(substitutions_directory, 'substitutions_merged.tex'), 'w', encoding='utf-8') as file:
                 file.write(merged_latex_file)
         mergedTex2HtmlWithSlicing(file_path, remove_tmp_folder=remove_tmp_folder)
-    logging.info('Файлы подстановок сконвертированы в HTML!')
+    logging.info('Файлы подстановок сконвертированы в HTML!')
```

### Comparing `taskgen-0.3.8/taskgen/functions.py` & `taskgen-0.3.8.1/taskgen/functions.py`

 * *Files identical despite different names*

### Comparing `taskgen-0.3.8/taskgen/html.py` & `taskgen-0.3.8.1/taskgen/html.py`

 * *Files identical despite different names*

### Comparing `taskgen-0.3.8/taskgen/main.py` & `taskgen-0.3.8.1/taskgen/main.py`

 * *Files identical despite different names*

### Comparing `taskgen-0.3.8/taskgen/moodle.py` & `taskgen-0.3.8.1/taskgen/moodle.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,27 @@
         answer_template = file.read()
 
     # обходим каждый вопрос
     variant_src = ''
     answers_xml = ''
     last_answer_index = 0
     for problem_number, substitution_tex_file in enumerate(structure):
-        # путь к соответствующем html файлу условия
+        # путь к соответствующему html файлу условия
         problem_html_file = os.path.join(os.path.dirname(os.path.dirname(substitution_tex_file)),
                                          'html',
                                          os.path.splitext(os.path.basename(substitution_tex_file))[
                                              0] + '_problem.html')
         with open(problem_html_file, 'r', encoding='utf-8') as file:
             problem_html_src = file.read()
 
-        # путь к соответствующем html файлу ответов
+        # заменяем названия датасетов
+        # встраиваем изображения
+        # встраиваем датасеты
+
+        # путь к соответствующему html файлу ответов
         answer_html_file = os.path.join(os.path.dirname(os.path.dirname(substitution_tex_file)),
                                           'html',
                                           os.path.splitext(os.path.basename(substitution_tex_file))[
                                               0] + '_answer.html')
         with open(answer_html_file, 'r', encoding='utf-8') as file:
             answer_html_src = file.read()
```

### Comparing `taskgen-0.3.8/taskgen/stats.py` & `taskgen-0.3.8.1/taskgen/stats.py`

 * *Files identical despite different names*

### Comparing `taskgen-0.3.8/taskgen/tex.py` & `taskgen-0.3.8.1/taskgen/tex.py`

 * *Files identical despite different names*

### Comparing `taskgen-0.3.8/taskgen.egg-info/PKG-INFO` & `taskgen-0.3.8.1/taskgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskgen
-Version: 0.3.8
+Version: 0.3.8.1
 Summary: Ядро генератора банка задач на базе MiKTeX и Jupyter Notebook
 Home-page: https://github.com/artyom-zolotarevskiy/taskgen-core
 Author: Артём Золотаревский
 Author-email: artyom@zolotarevskiy.ru
 Project-URL: Bug Tracker, https://github.com/artyom-zolotarevskiy/taskgen-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

