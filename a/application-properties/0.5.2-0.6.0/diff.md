# Comparing `tmp/application_properties-0.5.2.tar.gz` & `tmp/application_properties-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "application_properties-0.5.2.tar", last modified: Fri Apr  1 22:29:22 2022, max compression
+gzip compressed data, was "application_properties-0.6.0.tar", last modified: Mon Apr 10 01:21:09 2023, max compression
```

## Comparing `application_properties-0.5.2.tar` & `application_properties-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-04-01 22:29:22.067941 application_properties-0.5.2/
--rw-rw-rw-   0        0        0     1058 2021-05-30 03:14:28.000000 application_properties-0.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0       75 2022-04-01 21:16:07.000000 application_properties-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5903 2022-04-01 22:29:22.068942 application_properties-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    12031 2022-04-01 19:13:57.000000 application_properties-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2022-04-01 22:29:22.054931 application_properties-0.5.2/application_properties/
--rw-rw-rw-   0        0        0      553 2022-04-01 21:58:04.000000 application_properties-0.5.2/application_properties/__init__.py
--rw-rw-rw-   0        0        0    13530 2022-04-01 21:53:25.000000 application_properties-0.5.2/application_properties/application_properties.py
--rw-rw-rw-   0        0        0     4911 2022-04-01 21:59:08.000000 application_properties-0.5.2/application_properties/application_properties_facade.py
--rw-rw-rw-   0        0        0     2346 2022-04-01 17:26:48.000000 application_properties-0.5.2/application_properties/application_properties_json_loader.py
--rw-rw-rw-   0        0        0       13 2022-04-01 19:30:08.000000 application_properties-0.5.2/application_properties/py.typed
--rw-rw-rw-   0        0        0       65 2022-04-01 22:27:42.000000 application_properties-0.5.2/application_properties/version.py
-drwxrwxrwx   0        0        0        0 2022-04-01 22:29:22.058933 application_properties-0.5.2/application_properties.egg-info/
--rw-rw-rw-   0        0        0     5903 2022-04-01 22:29:21.000000 application_properties-0.5.2/application_properties.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      783 2022-04-01 22:29:21.000000 application_properties-0.5.2/application_properties.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-01 22:29:21.000000 application_properties-0.5.2/application_properties.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-04-01 22:29:21.000000 application_properties-0.5.2/application_properties.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2021-06-05 01:28:55.000000 application_properties-0.5.2/install-requirements.txt
--rw-rw-rw-   0        0        0      703 2022-04-01 22:29:22.069943 application_properties-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     2691 2022-04-01 21:58:04.000000 application_properties-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-01 22:29:22.067941 application_properties-0.5.2/test/
--rw-rw-rw-   0        0        0    13953 2022-04-01 15:33:56.000000 application_properties-0.5.2/test/test_application_properties.py
--rw-rw-rw-   0        0        0     8524 2022-04-01 15:51:14.000000 application_properties-0.5.2/test/test_application_properties_facade.py
--rw-rw-rw-   0        0        0     6590 2022-04-01 17:50:23.000000 application_properties-0.5.2/test/test_application_properties_json_loader.py
--rw-rw-rw-   0        0        0     3837 2022-04-01 15:28:59.000000 application_properties-0.5.2/test/test_get_boolean.py
--rw-rw-rw-   0        0        0     3821 2022-04-01 15:31:12.000000 application_properties-0.5.2/test/test_get_integer.py
--rw-rw-rw-   0        0        0     6073 2022-04-01 15:53:25.000000 application_properties-0.5.2/test/test_get_string.py
--rw-rw-rw-   0        0        0    12542 2022-04-01 15:53:33.000000 application_properties-0.5.2/test/test_set_manual_property.py
--rw-rw-rw-   0        0        0      510 2021-06-05 04:57:29.000000 application_properties-0.5.2/test/test_version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:21:08.989569 application_properties-0.6.0/
+-rw-rw-rw-   0        0        0     1066 2022-08-24 23:33:16.000000 application_properties-0.6.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       75 2022-08-24 23:33:16.000000 application_properties-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5862 2023-04-10 01:21:08.989569 application_properties-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12928 2022-08-24 23:33:16.000000 application_properties-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 01:21:08.968567 application_properties-0.6.0/application_properties/
+-rw-rw-rw-   0        0        0      553 2022-08-24 23:33:16.000000 application_properties-0.6.0/application_properties/__init__.py
+-rw-rw-rw-   0        0        0    14116 2023-04-10 00:30:33.000000 application_properties-0.6.0/application_properties/application_properties.py
+-rw-rw-rw-   0        0        0     4911 2022-08-24 23:33:16.000000 application_properties-0.6.0/application_properties/application_properties_facade.py
+-rw-rw-rw-   0        0        0     2458 2023-04-09 23:30:24.000000 application_properties-0.6.0/application_properties/application_properties_json_loader.py
+-rw-rw-rw-   0        0        0       13 2022-08-24 23:33:16.000000 application_properties-0.6.0/application_properties/py.typed
+-rw-rw-rw-   0        0        0       65 2023-04-09 23:30:24.000000 application_properties-0.6.0/application_properties/version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:21:08.977565 application_properties-0.6.0/application_properties.egg-info/
+-rw-rw-rw-   0        0        0     5862 2023-04-10 01:21:08.000000 application_properties-0.6.0/application_properties.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2023-04-10 01:21:08.000000 application_properties-0.6.0/application_properties.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:21:08.000000 application_properties-0.6.0/application_properties.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-10 01:21:08.000000 application_properties-0.6.0/application_properties.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2021-06-05 01:28:55.000000 application_properties-0.6.0/install-requirements.txt
+-rw-rw-rw-   0        0        0      696 2023-04-10 01:21:08.995566 application_properties-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     2691 2022-08-24 23:33:16.000000 application_properties-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:21:08.988569 application_properties-0.6.0/test/
+-rw-rw-rw-   0        0        0    13948 2023-04-09 23:30:24.000000 application_properties-0.6.0/test/test_application_properties.py
+-rw-rw-rw-   0        0        0     8524 2022-08-24 23:33:16.000000 application_properties-0.6.0/test/test_application_properties_facade.py
+-rw-rw-rw-   0        0        0     8742 2023-04-09 23:30:24.000000 application_properties-0.6.0/test/test_application_properties_json_loader.py
+-rw-rw-rw-   0        0        0     3837 2022-08-24 23:33:16.000000 application_properties-0.6.0/test/test_get_boolean.py
+-rw-rw-rw-   0        0        0     3821 2022-08-24 23:33:16.000000 application_properties-0.6.0/test/test_get_integer.py
+-rw-rw-rw-   0        0        0     6155 2023-04-10 00:07:55.000000 application_properties-0.6.0/test/test_get_string.py
+-rw-rw-rw-   0        0        0    12542 2022-08-24 23:33:16.000000 application_properties-0.6.0/test/test_set_manual_property.py
+-rw-rw-rw-   0        0        0      510 2021-06-05 04:57:29.000000 application_properties-0.6.0/test/test_version.py
```

### Comparing `application_properties-0.5.2/LICENSE.txt` & `application_properties-0.6.0/LICENSE.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2019 Max Taggart
+Copyright 2020-2022 Jack De Winter
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `application_properties-0.5.2/PKG-INFO` & `application_properties-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: application_properties
-Version: 0.5.2
+Version: 0.6.0
 Summary: A simple, easy to use, unified manner of accessing program properties.
 Home-page: https://github.com/jackdewinter/application_properties
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
-License: UNKNOWN
 Project-URL: Change Log, https://github.com/jackdewinter/application_properties/blob/main/changelog.md
 Keywords: properties
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -98,9 +96,7 @@
 As that document is rather dry, more information is provided in the way of
 examples in the [How To Use This Package section](dd) of the home page.
 
 ## How To Use, And Other Stuff
 
 For more information on this library please consult the various other
 section on the home page.
-
-
```

### Comparing `application_properties-0.5.2/README.md` & `application_properties-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,16 @@
 # application_properties
 
-[![GitHub top language](https://img.shields.io/github/languages/top/jackdewinter/application_properties)](https://github.com/jackdewinter/application_properties)
-![platforms](https://img.shields.io/badge/platform-windows%20%7C%20macos%20%7C%20linux-lightgrey)
-[![Python Versions](https://img.shields.io/pypi/pyversions/application_properties.svg)](https://pypi.org/project/application_properties)
-[![Version](https://img.shields.io/pypi/v/application_properties.svg)](https://pypi.org/project/application_properties)
-
-<!--
-[![GitHub Workflow Status (event)](https://img.shields.io/github/workflow/status/jackdewinter/application_properties/Main)](https://github.com/jackdewinter/application_properties/actions/workflows/main.yml)
-[![Codecov](https://img.shields.io/codecov/c/github/jackdewinter/application_properties)](https://app.codecov.io/gh/jackdewinter/application_properties)
--->
-![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/application_properties/black/master)
-![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/application_properties/flake8/master)
-![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/application_properties/pylint/master)
-[![Stars](https://img.shields.io/github/stars/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/stargazers)
-[![Downloads](https://img.shields.io/pypi/dm/application_properties.svg)](https://pypistats.org/packages/application_properties)
-
-[![Issues](https://img.shields.io/github/issues/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/issues)
-[![License](https://img.shields.io/github/license/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/blob/main/LICENSE.txt)
-[![Contributors](https://img.shields.io/github/contributors/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/graphs/contributors)
-[![Forks](https://img.shields.io/github/forks/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/network/members)
-
-[![LinkedIn](https://img.shields.io/badge/-LinkedIn-black.svg?logo=linkedin&colorB=555)](https://www.linkedin.com/in/jackdewinter/)
+|   |   |
+|---|---|
+|Project|[![Version](https://img.shields.io/pypi/v/application_properties.svg)](https://pypi.org/project/application_properties)  [![Python Versions](https://img.shields.io/pypi/pyversions/application_properties.svg)](https://pypi.org/project/application_properties)  ![platforms](https://img.shields.io/badge/platform-windows%20%7C%20macos%20%7C%20linux-lightgrey)  [![License](https://img.shields.io/github/license/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/blob/main/LICENSE.txt)  [![GitHub top language](https://img.shields.io/github/languages/top/jackdewinter/application_properties)](https://github.com/jackdewinter/application_properties)|
+|Quality|[![GitHub Workflow Status (event)](https://img.shields.io/github/workflow/status/jackdewinter/application_properties/Main)](https://github.com/jackdewinter/application_properties/actions/workflows/main.yml)  [![Issues](https://img.shields.io/github/issues/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/issues)  [![codecov](https://codecov.io/gh/jackdewinter/pymarkdown/branch/main/graph/badge.svg?token=PD5TKS8NQQ)](https://codecov.io/gh/jackdewinter/application_properties)  [![Sourcery](https://img.shields.io/badge/Sourcery-enabled-brightgreen)](https://sourcery.ai)  ![snyk](https://img.shields.io/snyk/vulnerabilities/github/jackdewinter/application_properties) |
+|  |![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/application_properties/black/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/application_properties/flake8/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/application_properties/pylint/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/application_properties/mypy/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/application_properties/pyroma/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/application_properties/pre-commit/main)|
+|Community|[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/jackdewinter/application_properties/graphs/commit-activity) [![Stars](https://img.shields.io/github/stars/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/stargazers)  [![Forks](https://img.shields.io/github/forks/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/network/members)  [![Contributors](https://img.shields.io/github/contributors/jackdewinter/application_properties.svg)](https://github.com/jackdewinter/application_properties/graphs/contributors)  [![Downloads](https://img.shields.io/pypi/dm/project_summarizer.svg)](https://pypistats.org/packages/project_summarizer)|
+|Maintainers|[![LinkedIn](https://img.shields.io/badge/-LinkedIn-black.svg?logo=linkedin&colorB=555)](https://www.linkedin.com/in/jackdewinter/)|
 
 The `application_properties` package was born out of necessity.
 During the creation of the [PyMarkdown](https://github.com/jackdewinter/pymarkdown) project,
 there was a distinct need for a configuration subsystem that was able to handle more
 complex configuration scenarios.
 
 The `application_properties` library has the following advnatages:
```

### Comparing `application_properties-0.5.2/application_properties/__init__.py` & `application_properties-0.6.0/application_properties/__init__.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.5.2/application_properties/application_properties.py` & `application_properties-0.6.0/application_properties/application_properties.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,24 +61,27 @@
 
     def enable_strict_mode(self) -> None:
         """
         Sets struct mode to True to enable it.
         """
         self.__strict_mode = True
 
-    def load_from_dict(self, config_map: Dict[Any, Any]) -> None:
+    def load_from_dict(
+        self, config_map: Dict[Any, Any], clear_map: bool = True
+    ) -> None:
         """
         Load the properties from a provided dictionary.
         """
 
         if not isinstance(config_map, dict):
             raise ValueError("Specified parameter was not a dictionary.")
 
         LOGGER.debug("Loading from dictionary: {%s}", str(config_map))
-        self.__flat_property_map.clear()
+        if clear_map:
+            self.__flat_property_map.clear()
         self.__scan_map(config_map, "")
 
     @staticmethod
     def verify_full_part_form(property_key: str) -> str:
         """
         Given one part of a full key, verify that it is composed properly.
         """
@@ -169,40 +172,39 @@
 
         if (
             property_value.startswith(
                 ApplicationProperties.__manual_property_type_prefix
             )
             and len(property_value) >= 2
         ):
-            if property_value[1] == ApplicationProperties.__manual_property_type_string:
-                composed_property_value = property_value[2:]
-            elif (
-                property_value[1]
-                == ApplicationProperties.__manual_property_type_integer
-            ):
-                try:
-                    composed_property_value = int(property_value[2:])
-                except ValueError as this_exception:
-                    raise ValueError(
-                        f"Manual property value '{property_value}' cannot be translated into an integer."
-                    ) from this_exception
-            elif (
-                property_value[1]
-                == ApplicationProperties.__manual_property_type_boolean
-            ):
-                composed_property_value = property_value[2:].lower() == "true"
-            else:
-                composed_property_value = property_value[1:]
+            composed_property_value = self.__adjust_property_type(property_value)
         self.__flat_property_map[property_key] = copy.deepcopy(composed_property_value)
         LOGGER.debug(
             "Adding configuration '%s' : {%s}",
             property_key,
             str(composed_property_value),
         )
 
+    def __adjust_property_type(self, property_value: str) -> Any:
+        composed_property_value: Any = None
+        if property_value[1] == ApplicationProperties.__manual_property_type_string:
+            composed_property_value = property_value[2:]
+        elif property_value[1] == ApplicationProperties.__manual_property_type_integer:
+            try:
+                composed_property_value = int(property_value[2:])
+            except ValueError as this_exception:
+                raise ValueError(
+                    f"Manual property value '{property_value}' cannot be translated into an integer."
+                ) from this_exception
+        elif property_value[1] == ApplicationProperties.__manual_property_type_boolean:
+            composed_property_value = property_value[2:].lower() == "true"
+        else:
+            composed_property_value = property_value[1:]
+        return composed_property_value
+
     # pylint: disable=unidiomatic-typecheck
     # pylint: disable=too-many-arguments
     # pylint: disable=broad-except
     # pylint: disable=raise-missing-from
     def get_property(
         self,
         property_name: str,
@@ -232,37 +234,54 @@
                 + f"either be None or a '{property_type.__name__}' value."
             )
 
         property_value = default_value
         property_name = property_name.lower()
         LOGGER.debug("property_name=%s", property_name)
         if property_name in self.__flat_property_map:
-            found_value = self.__flat_property_map[property_name]
-            is_eligible = type(found_value) == property_type
-            if not is_eligible and strict_mode:
-                raise ValueError(
-                    f"The value for property '{property_name}' must be of type '{property_type.__name__}'."
-                )
-            if is_eligible and valid_value_fn:
-                try:
-                    valid_value_fn(found_value)
-                except Exception as this_exception:
-                    is_eligible = False
-                    if strict_mode:
-                        raise ValueError(
-                            f"The value for property '{property_name}' is not valid: {str(this_exception)}"
-                        ) from this_exception
-            if is_eligible:
-                property_value = found_value
+            property_value = self.__get_present_property(
+                property_name,
+                property_value,
+                property_type,
+                strict_mode,
+                valid_value_fn,
+            )
         elif is_required:
             raise ValueError(
                 f"A value for property '{property_name}' must be provided."
             )
         return property_value
 
+    def __get_present_property(
+        self,
+        property_name: str,
+        property_value: Any,
+        property_type: type,
+        strict_mode: bool,
+        valid_value_fn: Optional[Callable[[Any], Any]],
+    ) -> Any:
+        found_value = self.__flat_property_map[property_name]
+        is_eligible = type(found_value) == property_type
+        if not is_eligible and strict_mode:
+            raise ValueError(
+                f"The value for property '{property_name}' must be of type '{property_type.__name__}'."
+            )
+        if is_eligible and valid_value_fn:
+            try:
+                valid_value_fn(found_value)
+            except Exception as this_exception:
+                is_eligible = False
+                if strict_mode:
+                    raise ValueError(
+                        f"The value for property '{property_name}' is not valid: {str(this_exception)}"
+                    ) from this_exception
+        if is_eligible:
+            property_value = found_value
+        return property_value
+
     # pylint: enable=unidiomatic-typecheck
     # pylint: enable=too-many-arguments
     # pylint: enable=broad-except
     # pylint: enable=raise-missing-from
 
     def get_boolean_property(
         self,
```

### Comparing `application_properties-0.5.2/application_properties/application_properties_facade.py` & `application_properties-0.6.0/application_properties/application_properties_facade.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.5.2/application_properties/application_properties_json_loader.py` & `application_properties-0.6.0/application_properties/application_properties_json_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     """
 
     @staticmethod
     def load_and_set(
         properties_object: ApplicationProperties,
         configuration_file: str,
         handle_error_fn: Optional[Callable[[str, Exception], None]] = None,
+        clear_property_map: bool = True,
     ) -> None:
         """
         Load the specified file and set it into the given properties object.
         """
 
         if not handle_error_fn:
 
@@ -48,15 +49,17 @@
                 f"Specified configuration file '{configuration_file}' "
                 + f"was not loaded ({str(this_exception)})."
             )
             handle_error_fn(formatted_error, this_exception)
 
         if configuration_map:
             try:
-                properties_object.load_from_dict(configuration_map)
+                properties_object.load_from_dict(
+                    configuration_map, clear_map=clear_property_map
+                )
             except ValueError as this_exception:
                 formatted_error = (
                     f"Specified configuration file '{configuration_file}' "
                     + f"is not valid ({str(this_exception)})."
                 )
                 handle_error_fn(formatted_error, this_exception)
```

### Comparing `application_properties-0.5.2/application_properties.egg-info/PKG-INFO` & `application_properties-0.6.0/application_properties.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: application-properties
-Version: 0.5.2
+Version: 0.6.0
 Summary: A simple, easy to use, unified manner of accessing program properties.
 Home-page: https://github.com/jackdewinter/application_properties
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
-License: UNKNOWN
 Project-URL: Change Log, https://github.com/jackdewinter/application_properties/blob/main/changelog.md
 Keywords: properties
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -98,9 +96,7 @@
 As that document is rather dry, more information is provided in the way of
 examples in the [How To Use This Package section](dd) of the home page.
 
 ## How To Use, And Other Stuff
 
 For more information on this library please consult the various other
 section on the home page.
-
-
```

### Comparing `application_properties-0.5.2/application_properties.egg-info/SOURCES.txt` & `application_properties-0.6.0/application_properties.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `application_properties-0.5.2/setup.cfg` & `application_properties-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 000000a0: 3430 322c 2045 3530 312c 2057 3239 312c  402, E501, W291,
 000000b0: 2057 3530 332c 2057 3239 330d 0a6d 6178   W503, W293..max
 000000c0: 2d6c 696e 652d 6c65 6e67 7468 203d 2038  -line-length = 8
 000000d0: 380d 0a6d 6178 2d63 6f6d 706c 6578 6974  8..max-complexit
 000000e0: 7920 3d20 3138 0d0a 7365 6c65 6374 203d  y = 18..select =
 000000f0: 2042 2c43 2c45 2c46 2c57 2c54 340d 0a0d   B,C,E,F,W,T4...
 00000100: 0a5b 7079 6c69 6e74 5d0d 0a64 6973 6162  .[pylint]..disab
-00000110: 6c65 203d 2043 3033 3031 2c20 4330 3333  le = C0301, C033
-00000120: 302c 2057 3035 3131 2c20 6475 706c 6963  0, W0511, duplic
-00000130: 6174 652d 636f 6465 0d0a 6578 7465 6e73  ate-code..extens
-00000140: 696f 6e2d 706b 672d 7768 6974 656c 6973  ion-pkg-whitelis
-00000150: 7420 3d20 7769 6e33 3261 7069 0d0a 0d0a  t = win32api....
-00000160: 5b74 6f6f 6c3a 7079 7465 7374 5d0d 0a74  [tool:pytest]..t
-00000170: 6573 7470 6174 6873 203d 202e 2f74 6573  estpaths = ./tes
-00000180: 740d 0a63 6163 6865 5f64 6972 203d 202e  t..cache_dir = .
-00000190: 2f62 7569 6c64 2f74 6573 742f 2e70 7974  /build/test/.pyt
-000001a0: 6573 745f 6361 6368 650d 0a6a 756e 6974  est_cache..junit
-000001b0: 5f66 616d 696c 7920 3d20 7875 6e69 7432  _family = xunit2
-000001c0: 0d0a 6164 646f 7074 7320 3d20 2d2d 7469  ..addopts = --ti
-000001d0: 6d65 6f75 743d 3130 202d 2d68 746d 6c3d  meout=10 --html=
-000001e0: 7265 706f 7274 2f72 6570 6f72 742e 6874  report/report.ht
-000001f0: 6d6c 202d 2d63 6f76 202d 2d63 6f76 2d62  ml --cov --cov-b
-00000200: 7261 6e63 6820 2d2d 636f 762d 6661 696c  ranch --cov-fail
-00000210: 2d75 6e64 6572 3d38 3020 2d2d 7374 7269  -under=80 --stri
-00000220: 6374 2d6d 6172 6b65 7273 202d 7261 202d  ct-markers -ra -
-00000230: 2d63 6f76 2d72 6570 6f72 7420 786d 6c3a  -cov-report xml:
-00000240: 7265 706f 7274 2f63 6f76 6572 6167 652e  report/coverage.
-00000250: 786d 6c20 2d2d 636f 762d 7265 706f 7274  xml --cov-report
-00000260: 2068 746d 6c3a 7265 706f 7274 2f63 6f76   html:report/cov
-00000270: 6572 6167 6520 2d2d 6a75 6e69 7478 6d6c  erage --junitxml
-00000280: 3d72 6570 6f72 742f 7465 7374 732e 786d  =report/tests.xm
-00000290: 6c0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  l....[egg_info].
-000002a0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000002b0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000110: 6c65 203d 2043 3033 3031 2c20 5730 3531  le = C0301, W051
+00000120: 312c 2064 7570 6c69 6361 7465 2d63 6f64  1, duplicate-cod
+00000130: 650d 0a65 7874 656e 7369 6f6e 2d70 6b67  e..extension-pkg
+00000140: 2d77 6869 7465 6c69 7374 203d 2077 696e  -whitelist = win
+00000150: 3332 6170 690d 0a0d 0a5b 746f 6f6c 3a70  32api....[tool:p
+00000160: 7974 6573 745d 0d0a 7465 7374 7061 7468  ytest]..testpath
+00000170: 7320 3d20 2e2f 7465 7374 0d0a 6361 6368  s = ./test..cach
+00000180: 655f 6469 7220 3d20 2e2f 6275 696c 642f  e_dir = ./build/
+00000190: 7465 7374 2f2e 7079 7465 7374 5f63 6163  test/.pytest_cac
+000001a0: 6865 0d0a 6a75 6e69 745f 6661 6d69 6c79  he..junit_family
+000001b0: 203d 2078 756e 6974 320d 0a61 6464 6f70   = xunit2..addop
+000001c0: 7473 203d 202d 2d74 696d 656f 7574 3d31  ts = --timeout=1
+000001d0: 3020 2d2d 6874 6d6c 3d72 6570 6f72 742f  0 --html=report/
+000001e0: 7265 706f 7274 2e68 746d 6c20 2d2d 636f  report.html --co
+000001f0: 7620 2d2d 636f 762d 6272 616e 6368 202d  v --cov-branch -
+00000200: 2d63 6f76 2d66 6169 6c2d 756e 6465 723d  -cov-fail-under=
+00000210: 3830 202d 2d73 7472 6963 742d 6d61 726b  80 --strict-mark
+00000220: 6572 7320 2d72 6120 2d2d 636f 762d 7265  ers -ra --cov-re
+00000230: 706f 7274 2078 6d6c 3a72 6570 6f72 742f  port xml:report/
+00000240: 636f 7665 7261 6765 2e78 6d6c 202d 2d63  coverage.xml --c
+00000250: 6f76 2d72 6570 6f72 7420 6874 6d6c 3a72  ov-report html:r
+00000260: 6570 6f72 742f 636f 7665 7261 6765 202d  eport/coverage -
+00000270: 2d6a 756e 6974 786d 6c3d 7265 706f 7274  -junitxml=report
+00000280: 2f74 6573 7473 2e78 6d6c 0d0a 0d0a 5b65  /tests.xml....[e
+00000290: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000002a0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000002b0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `application_properties-0.5.2/setup.py` & `application_properties-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.5.2/test/test_application_properties.py` & `application_properties-0.6.0/test/test_application_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
 
 
 def __sample_string_validation_function(property_value):
     """
     Simple string validation that throws an error if not "1" or "2".
     """
     if property_value not in ["1", "2"]:
-        raise ValueError("Value '" + str(property_value) + "' is not '1' or '2'")
+        raise ValueError(f"Value '{str(property_value)}' is not '1' or '2'")
 
 
 def test_properties_get_generic_with_strict_mode_and_bad_validity():
     """
     Test a fetching a configuration value where strict mode is on and the value is not valid.
     """
```

### Comparing `application_properties-0.5.2/test/test_application_properties_facade.py` & `application_properties-0.6.0/test/test_application_properties_facade.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.5.2/test/test_application_properties_json_loader.py` & `application_properties-0.6.0/test/test_application_properties_json_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -197,7 +197,68 @@
             "' is not valid (Keys strings cannot contain the separator character '.'.)."
             in new_stdout.getvalue()
         )
         assert not new_stderr.getvalue()
     finally:
         if configuration_file and os.path.exists(configuration_file):
             os.remove(configuration_file)
+
+
+def test_json_loader_pair_valid_json():
+    """
+    Test to make sure that we can load more than one configuration file and not have
+    the configurations stomp on each other in an unpredictable manner.
+    """
+
+    # Arrange
+    supplied_configuration_first = {
+        "plugins": {"md999": {"test_value_a": 2, "test_value_b": 3}}
+    }
+    supplied_configuration_second = {
+        "plugins": {"md999": {"test_value_b": 4, "test_value_c": 5}}
+    }
+    expected_value_a = 2
+    expected_value_b = 4
+    expected_value_c = 5
+
+    configuration_file_first = None
+    try:
+        configuration_file_first = write_temporary_configuration(
+            supplied_configuration_first
+        )
+        configuration_file_second = write_temporary_configuration(
+            supplied_configuration_second
+        )
+        application_properties = ApplicationProperties()
+
+        # Act
+        ApplicationPropertiesJsonLoader.load_and_set(
+            application_properties,
+            configuration_file_first,
+            None,
+            clear_property_map=False,
+        )
+        ApplicationPropertiesJsonLoader.load_and_set(
+            application_properties,
+            configuration_file_second,
+            None,
+            clear_property_map=False,
+        )
+        actual_value_a = application_properties.get_integer_property(
+            "plugins.md999.test_value_a", -1
+        )
+        actual_value_b = application_properties.get_integer_property(
+            "plugins.md999.test_value_b", -1
+        )
+        actual_value_c = application_properties.get_integer_property(
+            "plugins.md999.test_value_c", -1
+        )
+
+        # Assert
+        assert expected_value_a == actual_value_a
+        assert expected_value_b == actual_value_b
+        assert expected_value_c == actual_value_c
+    finally:
+        if configuration_file_first and os.path.exists(configuration_file_first):
+            os.remove(configuration_file_first)
+        if configuration_file_second and os.path.exists(configuration_file_second):
+            os.remove(configuration_file_second)
```

### Comparing `application_properties-0.5.2/test/test_get_boolean.py` & `application_properties-0.6.0/test/test_get_boolean.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.5.2/test/test_get_integer.py` & `application_properties-0.6.0/test/test_get_integer.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.5.2/test/test_get_string.py` & `application_properties-0.6.0/test/test_get_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 
 def __sample_string_validation_function(property_value):
     """
     Simple string validation that throws an error if not "1" or "2".
     """
     if property_value not in ["1", "2"]:
-        raise ValueError("Value '" + str(property_value) + "' is not '1' or '2'")
+        raise ValueError(f"Value '{str(property_value)}' is not '1' or '2'")
 
 
 def test_properties_get_string_with_found_value_not_validated():
     """
     Test fetching a configuration value that is present and does not adhere to the validation function.
     """
 
@@ -119,22 +119,26 @@
         "property", "-", __sample_string_validation_function
     )
 
     # Assert
     assert expected_value == actual_value
 
 
+# pylint: disable=broad-exception-raised
 def bad_validation_function(property_value):
     """
     Test validation function that always throws an exception.
     """
     # sourcery skip: raise-specific-error
     raise Exception(f"huh? {str(property_value)}")
 
 
+# pylint: enable=broad-exception-raised
+
+
 def test_properties_get_string_with_found_value_validation_raises_error():
     """
     Test fetching a configuration value that is present and the validation function raises an error.
     """
 
     # Arrange
     config_map = {"property": "1"}
```

### Comparing `application_properties-0.5.2/test/test_set_manual_property.py` & `application_properties-0.6.0/test/test_set_manual_property.py`

 * *Files identical despite different names*

