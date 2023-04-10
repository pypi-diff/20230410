# Comparing `tmp/eAwaiter-0.0.2.tar.gz` & `tmp/eAwaiter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eAwaiter-0.0.2.tar", last modified: Sun Apr  9 12:06:05 2023, max compression
+gzip compressed data, was "eAwaiter-0.0.3.tar", last modified: Mon Apr 10 15:00:50 2023, max compression
```

## Comparing `eAwaiter-0.0.2.tar` & `eAwaiter-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/
--rw-r--r--   0 skrci     (1000) skrci     (1000)     1062 2023-03-23 13:33:26.000000 eAwaiter-0.0.2/LICENSE
--rw-r--r--   0 skrci     (1000) skrci     (1000)     2931 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/PKG-INFO
--rw-r--r--   0 skrci     (1000) skrci     (1000)     2479 2023-04-06 14:27:23.000000 eAwaiter-0.0.2/README.md
-drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/eAwaiter.egg-info/
--rw-r--r--   0 skrci     (1000) skrci     (1000)     2931 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/PKG-INFO
--rw-r--r--   0 skrci     (1000) skrci     (1000)      331 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/SOURCES.txt
--rw-r--r--   0 skrci     (1000) skrci     (1000)        1 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/dependency_links.txt
--rw-r--r--   0 skrci     (1000) skrci     (1000)       40 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/requires.txt
--rw-r--r--   0 skrci     (1000) skrci     (1000)        7 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/top_level.txt
--rw-r--r--   0 skrci     (1000) skrci     (1000)      100 2023-03-23 14:29:52.000000 eAwaiter-0.0.2/pyproject.toml
--rw-r--r--   0 skrci     (1000) skrci     (1000)      576 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/setup.cfg
--rw-r--r--   0 skrci     (1000) skrci     (1000)       70 2023-03-23 14:24:15.000000 eAwaiter-0.0.2/setup.py
-drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/waiter/
--rw-r--r--   0 skrci     (1000) skrci     (1000)       13 2023-03-13 17:05:32.000000 eAwaiter-0.0.2/waiter/__init__.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)     6517 2023-03-26 10:04:06.000000 eAwaiter-0.0.2/waiter/api_navigator.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)     1510 2023-03-26 10:03:56.000000 eAwaiter-0.0.2/waiter/dataclasses.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)      390 2023-03-13 17:10:11.000000 eAwaiter-0.0.2/waiter/exceptions.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)     1650 2023-03-26 10:04:19.000000 eAwaiter-0.0.2/waiter/helpers.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)     8392 2023-04-07 22:04:12.000000 eAwaiter-0.0.2/waiter/waiter.py
+drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-04-10 15:00:50.115120 eAwaiter-0.0.3/
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     1062 2023-03-23 13:33:26.000000 eAwaiter-0.0.3/LICENSE
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     2931 2023-04-10 15:00:50.118454 eAwaiter-0.0.3/PKG-INFO
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     2479 2023-04-06 14:27:23.000000 eAwaiter-0.0.3/README.md
+drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-04-10 15:00:50.115120 eAwaiter-0.0.3/eAwaiter.egg-info/
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     2931 2023-04-10 15:00:50.000000 eAwaiter-0.0.3/eAwaiter.egg-info/PKG-INFO
+-rw-r--r--   0 skrci     (1000) skrci     (1000)      331 2023-04-10 15:00:50.000000 eAwaiter-0.0.3/eAwaiter.egg-info/SOURCES.txt
+-rw-r--r--   0 skrci     (1000) skrci     (1000)        1 2023-04-10 15:00:50.000000 eAwaiter-0.0.3/eAwaiter.egg-info/dependency_links.txt
+-rw-r--r--   0 skrci     (1000) skrci     (1000)       40 2023-04-10 15:00:50.000000 eAwaiter-0.0.3/eAwaiter.egg-info/requires.txt
+-rw-r--r--   0 skrci     (1000) skrci     (1000)        7 2023-04-10 15:00:50.000000 eAwaiter-0.0.3/eAwaiter.egg-info/top_level.txt
+-rw-r--r--   0 skrci     (1000) skrci     (1000)      100 2023-03-23 14:29:52.000000 eAwaiter-0.0.3/pyproject.toml
+-rw-r--r--   0 skrci     (1000) skrci     (1000)      576 2023-04-10 15:00:50.118454 eAwaiter-0.0.3/setup.cfg
+-rw-r--r--   0 skrci     (1000) skrci     (1000)       70 2023-03-23 14:24:15.000000 eAwaiter-0.0.3/setup.py
+drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-04-10 15:00:50.115120 eAwaiter-0.0.3/waiter/
+-rw-r--r--   0 skrci     (1000) skrci     (1000)       13 2023-03-13 17:05:32.000000 eAwaiter-0.0.3/waiter/__init__.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     6574 2023-04-10 10:51:27.000000 eAwaiter-0.0.3/waiter/api_navigator.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     1510 2023-03-26 10:03:56.000000 eAwaiter-0.0.3/waiter/dataclasses.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)      390 2023-03-13 17:10:11.000000 eAwaiter-0.0.3/waiter/exceptions.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     1650 2023-03-26 10:04:19.000000 eAwaiter-0.0.3/waiter/helpers.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     8392 2023-04-09 12:14:11.000000 eAwaiter-0.0.3/waiter/waiter.py
```

### Comparing `eAwaiter-0.0.2/LICENSE` & `eAwaiter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eAwaiter-0.0.2/PKG-INFO` & `eAwaiter-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eAwaiter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to manage your eAsistent meals automatically.
 Home-page: https://github.com/5KRC1/eAwaiter
 Author: 5krc1
 Author-email: skrci@dasadweb.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eAwaiter-0.0.2/README.md` & `eAwaiter-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `eAwaiter-0.0.2/eAwaiter.egg-info/PKG-INFO` & `eAwaiter-0.0.3/eAwaiter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eAwaiter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to manage your eAsistent meals automatically.
 Home-page: https://github.com/5KRC1/eAwaiter
 Author: 5krc1
 Author-email: skrci@dasadweb.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eAwaiter-0.0.2/setup.cfg` & `eAwaiter-0.0.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eAwaiter
-version = 0.0.2
+version = 0.0.3
 author = 5krc1
 author_email = skrci@dasadweb.com
 description = Package to manage your eAsistent meals automatically.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/5KRC1/eAwaiter
 license = MIT
```

### Comparing `eAwaiter-0.0.2/waiter/api_navigator.py` & `eAwaiter-0.0.3/waiter/api_navigator.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
         return True, eAsistentMeal("", meal_id, date_str, False, False)
 
     def check_double_div(self, container: Tag, meal_id: str, date: datetime, date_str: str) -> [bool, dict]:
         """
         Either: past (not selected),
                 past (selected),
                 future (not loaded)
+                present (no meal)
         """
         if not len(container.find_all("div")) == 2:
             return False, {}
 
         selected = False
         changable = False
         second_div = container.find_all("div")[1]
@@ -125,15 +126,15 @@
         if len(list(container.findChildren(recursive=False))) > 2:
             # selected or signed off
             selected = True \
                     if container.find("span").text == "Prijavljen" \
                     else False
 
         meal_text = second_div.text.strip()
-        if meal_text.split(" ")[0] in ["Prijava", "Naročen"]:
+        if meal_text.split(" ")[0] in ["Prijava", "Naročen", "Izbira", "Odjavljen"]:
             # future
             today = datetime.today()
             changable = True \
                     if (date - today).days > 9 \
                     else False
             selected = True \
                     if meal_text.split(" ")[0] == "Naročen" \
```

### Comparing `eAwaiter-0.0.2/waiter/dataclasses.py` & `eAwaiter-0.0.3/waiter/dataclasses.py`

 * *Files identical despite different names*

### Comparing `eAwaiter-0.0.2/waiter/helpers.py` & `eAwaiter-0.0.3/waiter/helpers.py`

 * *Files identical despite different names*

### Comparing `eAwaiter-0.0.2/waiter/waiter.py` & `eAwaiter-0.0.3/waiter/waiter.py`

 * *Files identical despite different names*

