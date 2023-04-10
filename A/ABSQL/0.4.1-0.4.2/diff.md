# Comparing `tmp/ABSQL-0.4.1.tar.gz` & `tmp/ABSQL-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABSQL-0.4.1.tar", last modified: Mon Mar 20 23:36:08 2023, max compression
+gzip compressed data, was "ABSQL-0.4.2.tar", last modified: Mon Apr 10 17:55:57 2023, max compression
```

## Comparing `ABSQL-0.4.1.tar` & `ABSQL-0.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-20 23:36:08.774464 ABSQL-0.4.1/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-20 23:36:08.770465 ABSQL-0.4.1/ABSQL.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     9281 2023-03-20 23:36:08.000000 ABSQL-0.4.1/ABSQL.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      668 2023-03-20 23:36:08.000000 ABSQL-0.4.1/ABSQL.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-03-20 23:36:08.000000 ABSQL-0.4.1/ABSQL.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       65 2023-03-20 23:36:08.000000 ABSQL-0.4.1/ABSQL.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       12 2023-03-20 23:36:08.000000 ABSQL-0.4.1/ABSQL.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     1071 2022-03-06 17:39:00.000000 ABSQL-0.4.1/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     9281 2023-03-20 23:36:08.774464 ABSQL-0.4.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     8844 2023-02-26 01:17:04.000000 ABSQL-0.4.1/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-20 23:36:08.770465 ABSQL-0.4.1/absql/
--rw-rw-r--   0 chris     (1000) chris     (1000)     3157 2023-03-09 20:15:25.000000 ABSQL-0.4.1/absql/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-20 23:36:08.770465 ABSQL-0.4.1/absql/files/
--rw-rw-r--   0 chris     (1000) chris     (1000)      740 2022-07-21 00:32:47.000000 ABSQL-0.4.1/absql/files/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2981 2023-03-10 10:55:00.000000 ABSQL-0.4.1/absql/files/loader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1678 2023-03-20 23:04:49.000000 ABSQL-0.4.1/absql/files/parsers.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-20 23:36:08.770465 ABSQL-0.4.1/absql/functions/
--rw-rw-r--   0 chris     (1000) chris     (1000)      772 2023-03-10 10:55:45.000000 ABSQL-0.4.1/absql/functions/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2132 2023-02-17 15:50:01.000000 ABSQL-0.4.1/absql/functions/db.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      560 2022-03-27 16:53:20.000000 ABSQL-0.4.1/absql/functions/env.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      350 2022-03-26 20:24:05.000000 ABSQL-0.4.1/absql/functions/time.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-20 23:36:08.770465 ABSQL-0.4.1/absql/render/
--rw-rw-r--   0 chris     (1000) chris     (1000)     2970 2023-02-26 01:19:37.000000 ABSQL-0.4.1/absql/render/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-20 23:36:08.770465 ABSQL-0.4.1/absql/text/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1596 2023-02-17 12:15:22.000000 ABSQL-0.4.1/absql/text/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-20 23:36:08.770465 ABSQL-0.4.1/absql/utils/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1218 2023-03-20 23:07:29.000000 ABSQL-0.4.1/absql/utils/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-03-20 23:36:08.774464 ABSQL-0.4.1/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      825 2023-03-20 23:35:13.000000 ABSQL-0.4.1/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-20 23:36:08.774464 ABSQL-0.4.1/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-03-06 18:00:37.000000 ABSQL-0.4.1/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      814 2023-03-09 20:24:30.000000 ABSQL-0.4.1/tests/test_copy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      586 2023-03-10 10:32:28.000000 ABSQL-0.4.1/tests/test_loader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      740 2022-03-06 21:04:47.000000 ABSQL-0.4.1/tests/test_parse_file.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1236 2023-02-17 15:50:01.000000 ABSQL-0.4.1/tests/test_partial_kwargs.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1775 2022-12-14 21:04:08.000000 ABSQL-0.4.1/tests/test_render.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3200 2022-08-07 01:29:08.000000 ABSQL-0.4.1/tests/test_render_file.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2523 2023-02-25 20:57:59.000000 ABSQL-0.4.1/tests/test_render_text.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      288 2022-07-20 19:42:32.000000 ABSQL-0.4.1/tests/test_set.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      729 2022-12-14 21:04:44.000000 ABSQL-0.4.1/tests/test_text.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1401 2023-03-20 23:35:04.000000 ABSQL-0.4.1/tests/test_utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-10 17:55:57.603561 ABSQL-0.4.2/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-10 17:55:57.599561 ABSQL-0.4.2/ABSQL.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9281 2023-04-10 17:55:57.000000 ABSQL-0.4.2/ABSQL.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      668 2023-04-10 17:55:57.000000 ABSQL-0.4.2/ABSQL.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-04-10 17:55:57.000000 ABSQL-0.4.2/ABSQL.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       65 2023-04-10 17:55:57.000000 ABSQL-0.4.2/ABSQL.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       12 2023-04-10 17:55:57.000000 ABSQL-0.4.2/ABSQL.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1071 2022-03-06 17:39:00.000000 ABSQL-0.4.2/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9281 2023-04-10 17:55:57.603561 ABSQL-0.4.2/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8844 2023-02-26 01:17:04.000000 ABSQL-0.4.2/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-10 17:55:57.599561 ABSQL-0.4.2/absql/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3157 2023-04-10 17:46:28.000000 ABSQL-0.4.2/absql/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-10 17:55:57.599561 ABSQL-0.4.2/absql/files/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      740 2023-04-10 17:43:30.000000 ABSQL-0.4.2/absql/files/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2981 2023-03-10 10:55:00.000000 ABSQL-0.4.2/absql/files/loader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1693 2023-04-10 17:51:24.000000 ABSQL-0.4.2/absql/files/parsers.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-10 17:55:57.603561 ABSQL-0.4.2/absql/functions/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      772 2023-03-10 10:55:45.000000 ABSQL-0.4.2/absql/functions/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2132 2023-02-17 15:50:01.000000 ABSQL-0.4.2/absql/functions/db.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      560 2022-03-27 16:53:20.000000 ABSQL-0.4.2/absql/functions/env.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      350 2022-03-26 20:24:05.000000 ABSQL-0.4.2/absql/functions/time.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-10 17:55:57.603561 ABSQL-0.4.2/absql/render/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2970 2023-04-10 17:51:30.000000 ABSQL-0.4.2/absql/render/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-10 17:55:57.603561 ABSQL-0.4.2/absql/text/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1596 2023-02-17 12:15:22.000000 ABSQL-0.4.2/absql/text/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-10 17:55:57.603561 ABSQL-0.4.2/absql/utils/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1218 2023-03-21 22:02:47.000000 ABSQL-0.4.2/absql/utils/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-04-10 17:55:57.603561 ABSQL-0.4.2/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      825 2023-04-10 17:52:57.000000 ABSQL-0.4.2/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-10 17:55:57.603561 ABSQL-0.4.2/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-03-06 18:00:37.000000 ABSQL-0.4.2/tests/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      814 2023-03-09 20:24:30.000000 ABSQL-0.4.2/tests/test_copy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      586 2023-03-10 10:32:28.000000 ABSQL-0.4.2/tests/test_loader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      740 2022-03-06 21:04:47.000000 ABSQL-0.4.2/tests/test_parse_file.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1236 2023-02-17 15:50:01.000000 ABSQL-0.4.2/tests/test_partial_kwargs.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2019 2023-04-10 17:52:40.000000 ABSQL-0.4.2/tests/test_render.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3200 2023-04-10 17:27:18.000000 ABSQL-0.4.2/tests/test_render_file.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2523 2023-02-25 20:57:59.000000 ABSQL-0.4.2/tests/test_render_text.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      288 2022-07-20 19:42:32.000000 ABSQL-0.4.2/tests/test_set.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      729 2022-12-14 21:04:44.000000 ABSQL-0.4.2/tests/test_text.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1401 2023-03-20 23:35:04.000000 ABSQL-0.4.2/tests/test_utils.py
```

### Comparing `ABSQL-0.4.1/ABSQL.egg-info/PKG-INFO` & `ABSQL-0.4.2/ABSQL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.4.1
+Version: 0.4.2
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/chriscardillo/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.4.1/ABSQL.egg-info/SOURCES.txt` & `ABSQL-0.4.2/ABSQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/LICENSE` & `ABSQL-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/PKG-INFO` & `ABSQL-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.4.1
+Version: 0.4.2
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/chriscardillo/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.4.1/README.md` & `ABSQL-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/absql/__init__.py` & `ABSQL-0.4.2/absql/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/absql/files/__init__.py` & `ABSQL-0.4.2/absql/files/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/absql/files/loader.py` & `ABSQL-0.4.2/absql/files/loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/absql/files/parsers.py` & `ABSQL-0.4.2/absql/files/parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             content = yaml.load(text, Loader=loader)
     return {"metadata": metadata, "content": content}
 
 
 def parse_generic(file_path, loader=None):
     if loader is None:
         loader = generate_loader()
-    raw_content = frontmatter_load(file_path)
+    raw_content = frontmatter_load(file_path, loader=loader)
     file_content = raw_content["metadata"] or raw_content["content"]
     return file_content
 
 
 def parse_sql(file_path, loader=None):
     if loader is None:
         loader = generate_loader()
```

### Comparing `ABSQL-0.4.1/absql/functions/__init__.py` & `ABSQL-0.4.2/absql/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/absql/functions/db.py` & `ABSQL-0.4.2/absql/functions/db.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/absql/functions/env.py` & `ABSQL-0.4.2/absql/functions/env.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/absql/render/__init__.py` & `ABSQL-0.4.2/absql/render/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/absql/text/__init__.py` & `ABSQL-0.4.2/absql/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/absql/utils/__init__.py` & `ABSQL-0.4.2/absql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/setup.py` & `ABSQL-0.4.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ABSQL",
-    version="0.4.1",
+    version="0.4.2",
     author="Chris Cardillo",
     author_email="cfcardillo23@gmail.com",
     description="A rendering engine for templated SQL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/chriscardillo/ABSQL",
     packages=setuptools.find_packages(),
```

### Comparing `ABSQL-0.4.1/tests/test_copy.py` & `ABSQL-0.4.2/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/tests/test_loader.py` & `ABSQL-0.4.2/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/tests/test_parse_file.py` & `ABSQL-0.4.2/tests/test_parse_file.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/tests/test_partial_kwargs.py` & `ABSQL-0.4.2/tests/test_partial_kwargs.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/tests/test_render.py` & `ABSQL-0.4.2/tests/test_render.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 def mock_settings_env_vars():
     with mock.patch.dict(os.environ, {"name": "Bob"}):
         yield
 
 
 @pytest.fixture()
 def runner():
-    return Runner(greeting="Hello")
+    def double_it(x):
+        return x + x
+
+    return Runner(extra_constructors={"double_it": double_it}, greeting="Hello")
 
 
 @pytest.fixture()
 def contextless_runner():
     return Runner()
 
 
@@ -65,7 +68,12 @@
     replaced_only = runner.render(
         "{{env_switch(foo='address')}} and {{greeting}}", replace_only=True
     )
     assert replaced_only == "{{ env_switch(foo='address') }} and Hello"
 
     original_2 = runner.render("{{env_switch(foo='address')}} and {{greeting}}")
     assert original_2 == "value_unspecified and Hello"
+
+def test_runner_renders_yaml(runner):
+    got = runner.render("tests/files/constructor.yml")
+    want = "SELECT * FROM tabletable"
+    assert got == want
```

### Comparing `ABSQL-0.4.1/tests/test_render_file.py` & `ABSQL-0.4.2/tests/test_render_file.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/tests/test_render_text.py` & `ABSQL-0.4.2/tests/test_render_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/tests/test_text.py` & `ABSQL-0.4.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.4.1/tests/test_utils.py` & `ABSQL-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

