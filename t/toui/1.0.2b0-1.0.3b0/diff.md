# Comparing `tmp/toui-1.0.2b0.tar.gz` & `tmp/toui-1.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-1.0.2b0.tar", last modified: Tue Mar 28 04:14:41 2023, max compression
+gzip compressed data, was "toui-1.0.3b0.tar", last modified: Mon Apr 10 12:56:08 2023, max compression
```

## Comparing `toui-1.0.2b0.tar` & `toui-1.0.3b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 04:14:41.862377 toui-1.0.2b0/
--rw-rw-rw-   0        0        0     1094 2023-03-22 14:49:00.000000 toui-1.0.2b0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-03-28 04:10:54.000000 toui-1.0.2b0/MANIFEST.in
--rw-rw-rw-   0        0        0     3043 2023-03-28 04:14:41.861375 toui-1.0.2b0/PKG-INFO
--rw-rw-rw-   0        0        0     2607 2023-03-28 03:34:07.000000 toui-1.0.2b0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 04:14:41.806510 toui-1.0.2b0/examples/
--rw-rw-rw-   0        0        0        0 2023-03-20 05:08:45.000000 toui-1.0.2b0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-03-23 04:20:48.000000 toui-1.0.2b0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-03-25 05:34:44.000000 toui-1.0.2b0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-03-28 03:01:53.000000 toui-1.0.2b0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-03-28 03:47:39.000000 toui-1.0.2b0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-03-23 03:41:03.000000 toui-1.0.2b0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-03-28 03:48:59.000000 toui-1.0.2b0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-03-19 17:31:48.000000 toui-1.0.2b0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-03-17 15:14:02.000000 toui-1.0.2b0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-03-28 04:14:41.808511 toui-1.0.2b0/images/
--rw-rw-rw-   0        0        0    29049 2023-03-27 13:51:31.000000 toui-1.0.2b0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-03-28 04:14:41.862377 toui-1.0.2b0/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-03-28 04:12:40.000000 toui-1.0.2b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-28 04:14:41.829392 toui-1.0.2b0/toui/
--rw-rw-rw-   0        0        0      213 2023-03-28 04:14:39.000000 toui-1.0.2b0/toui/__init__.py
--rw-rw-rw-   0        0        0      429 2023-03-26 03:42:04.000000 toui-1.0.2b0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1093 2023-03-28 03:11:10.000000 toui-1.0.2b0/toui/_helpers.py
--rw-rw-rw-   0        0        0     4836 2023-03-28 03:47:22.000000 toui-1.0.2b0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     2380 2023-03-28 03:44:17.000000 toui-1.0.2b0/toui/_signals.py
--rw-rw-rw-   0        0        0    20266 2023-03-28 03:34:07.000000 toui-1.0.2b0/toui/apps.py
--rw-rw-rw-   0        0        0    18875 2023-03-25 04:19:40.000000 toui-1.0.2b0/toui/elements.py
--rw-rw-rw-   0        0        0      168 2023-03-24 12:27:54.000000 toui-1.0.2b0/toui/exceptions.py
--rw-rw-rw-   0        0        0    14434 2023-03-28 03:10:58.000000 toui-1.0.2b0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-03-25 05:57:54.000000 toui-1.0.2b0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-03-28 04:14:41.858374 toui-1.0.2b0/toui.egg-info/
--rw-rw-rw-   0        0        0     3043 2023-03-28 04:14:41.000000 toui-1.0.2b0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-03-28 04:14:41.000000 toui-1.0.2b0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 04:14:41.000000 toui-1.0.2b0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-03-28 04:14:41.000000 toui-1.0.2b0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-28 04:14:41.000000 toui-1.0.2b0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.480316 toui-1.0.3b0/
+-rw-rw-rw-   0        0        0     1094 2023-03-28 04:20:49.000000 toui-1.0.3b0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-03-28 04:20:49.000000 toui-1.0.3b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3054 2023-04-10 12:56:08.478312 toui-1.0.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2618 2023-03-28 05:00:34.000000 toui-1.0.3b0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.208619 toui-1.0.3b0/examples/
+-rw-rw-rw-   0        0        0        0 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.213604 toui-1.0.3b0/images/
+-rw-rw-rw-   0        0        0    29049 2023-03-28 04:20:49.000000 toui-1.0.3b0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-10 12:56:08.481313 toui-1.0.3b0/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-03-28 04:20:49.000000 toui-1.0.3b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.379602 toui-1.0.3b0/toui/
+-rw-rw-rw-   0        0        0      213 2023-04-10 12:54:07.000000 toui-1.0.3b0/toui/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1093 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/_helpers.py
+-rw-rw-rw-   0        0        0     4836 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     2380 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/_signals.py
+-rw-rw-rw-   0        0        0    20266 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/apps.py
+-rw-rw-rw-   0        0        0    18917 2023-04-10 12:45:09.000000 toui-1.0.3b0/toui/elements.py
+-rw-rw-rw-   0        0        0      168 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    14434 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.471334 toui-1.0.3b0/toui.egg-info/
+-rw-rw-rw-   0        0        0     3054 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/top_level.txt
```

### Comparing `toui-1.0.2b0/LICENSE` & `toui-1.0.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/PKG-INFO` & `toui-1.0.3b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 1.0.2b0
+Version: 1.0.3b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -75,21 +75,20 @@
 app.add_pages(main_page)
 
 if __name__ == "__main__":
     app.run()
 ```
 
 # Make the app responsive
-Check this [example](https://toui.readthedocs.io/en/latest/Examples.simple_website.html)
+Check this [example](https://toui.readthedocs.io/en/latest/Examples.example_1_simple_website.html)
 and [other examples](https://toui.readthedocs.io/en/latest/Examples.html) to learn how
 to make the website / desktop app responsive.
 
 # Deploy the app
-You can deploy the web app the same way you deploy a `Flask` app
-[How to deploy Flask app](https://flask.palletsprojects.com/deploying/).
+You can deploy the web app the same way you deploy a `Flask` app ([How to deploy Flask app](https://flask.palletsprojects.com/deploying/)).
 The only difference is that you need to access the `Flask` object first:
 ```python
 app = Website(__name__)
 flask_app = app.flask_app
 ```
 Then you need to deploy the `flask_app` and not the `app`.
```

### Comparing `toui-1.0.2b0/README.md` & `toui-1.0.3b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,21 +61,20 @@
 app.add_pages(main_page)
 
 if __name__ == "__main__":
     app.run()
 ```
 
 # Make the app responsive
-Check this [example](https://toui.readthedocs.io/en/latest/Examples.simple_website.html)
+Check this [example](https://toui.readthedocs.io/en/latest/Examples.example_1_simple_website.html)
 and [other examples](https://toui.readthedocs.io/en/latest/Examples.html) to learn how
 to make the website / desktop app responsive.
 
 # Deploy the app
-You can deploy the web app the same way you deploy a `Flask` app
-[How to deploy Flask app](https://flask.palletsprojects.com/deploying/).
+You can deploy the web app the same way you deploy a `Flask` app ([How to deploy Flask app](https://flask.palletsprojects.com/deploying/)).
 The only difference is that you need to access the `Flask` object first:
 ```python
 app = Website(__name__)
 flask_app = app.flask_app
 ```
 Then you need to deploy the `flask_app` and not the `app`.
```

### Comparing `toui-1.0.2b0/examples/advanced_example_1_toui_blueprint.py` & `toui-1.0.3b0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/examples/example_1_simple_website.py` & `toui-1.0.3b0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/examples/example_2_simple_desktop_app.py` & `toui-1.0.3b0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/examples/example_3_updating_page.py` & `toui-1.0.3b0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/examples/example_4_function_with_arg.py` & `toui-1.0.3b0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/examples/example_5_user_variables.py` & `toui-1.0.3b0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/images/logo.png` & `toui-1.0.3b0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/setup.py` & `toui-1.0.3b0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/toui/_helpers.py` & `toui-1.0.3b0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/toui/_javascript_templates.py` & `toui-1.0.3b0/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/toui/_signals.py` & `toui-1.0.3b0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/toui/apps.py` & `toui-1.0.3b0/toui/apps.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/toui/elements.py` & `toui-1.0.3b0/toui/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,16 +420,17 @@
         style = self.get_attr('style')
         parser = tinycss.make_parser("page3")
         declarations = parser.parse_style_attr(style)[0]
         for declaration in declarations:
             if declaration.name == property:
                 property_value = ""
                 for v in declaration.value:
-                    property_value += str(v.value) + str(v.unit)
-                    style += str(v.value)
+                    property_value += str(v.value)
+                    if v.unit is not None:
+                        property_value += str(v.unit)
                 return property_value
 
     def set_style_property(self, property, value):
         """
         Sets the value of a CSS property inside ``style`` attribute.
 
         Parameters
```

### Comparing `toui-1.0.2b0/toui/pages.py` & `toui-1.0.3b0/toui/pages.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/toui/structure.py` & `toui-1.0.3b0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.2b0/toui.egg-info/PKG-INFO` & `toui-1.0.3b0/toui.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 1.0.2b0
+Version: 1.0.3b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -75,21 +75,20 @@
 app.add_pages(main_page)
 
 if __name__ == "__main__":
     app.run()
 ```
 
 # Make the app responsive
-Check this [example](https://toui.readthedocs.io/en/latest/Examples.simple_website.html)
+Check this [example](https://toui.readthedocs.io/en/latest/Examples.example_1_simple_website.html)
 and [other examples](https://toui.readthedocs.io/en/latest/Examples.html) to learn how
 to make the website / desktop app responsive.
 
 # Deploy the app
-You can deploy the web app the same way you deploy a `Flask` app
-[How to deploy Flask app](https://flask.palletsprojects.com/deploying/).
+You can deploy the web app the same way you deploy a `Flask` app ([How to deploy Flask app](https://flask.palletsprojects.com/deploying/)).
 The only difference is that you need to access the `Flask` object first:
 ```python
 app = Website(__name__)
 flask_app = app.flask_app
 ```
 Then you need to deploy the `flask_app` and not the `app`.
```

### Comparing `toui-1.0.2b0/toui.egg-info/SOURCES.txt` & `toui-1.0.3b0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

