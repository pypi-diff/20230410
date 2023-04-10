# Comparing `tmp/caep-0.1.5.tar.gz` & `tmp/caep-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caep-0.1.5.tar", last modified: Tue Mar 28 14:28:18 2023, max compression
+gzip compressed data, was "caep-0.1.6.tar", last modified: Mon Apr 10 07:37:22 2023, max compression
```

## Comparing `caep-0.1.5.tar` & `caep-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-28 14:28:18.138058 caep-0.1.5/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-0.1.5/LICENSE
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-03-28 14:28:18.138058 caep-0.1.5/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9157 2023-03-28 14:28:15.000000 caep-0.1.5/README.md
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-28 14:28:18.134724 caep-0.1.5/caep/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-0.1.5/caep/__init__.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8026 2023-03-28 14:28:15.000000 caep-0.1.5/caep/config.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-0.1.5/caep/example.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1396 2023-03-28 05:50:28.000000 caep-0.1.5/caep/helpers.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11081 2023-01-30 11:31:45.000000 caep-0.1.5/caep/schema.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-0.1.5/caep/xdg.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-28 14:28:18.138058 caep-0.1.5/caep.egg-info/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-03-28 14:28:18.000000 caep-0.1.5/caep.egg-info/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      343 2023-03-28 14:28:18.000000 caep-0.1.5/caep.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-03-28 14:28:18.000000 caep-0.1.5/caep.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       23 2023-03-28 14:28:18.000000 caep-0.1.5/caep.egg-info/requires.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-03-28 14:28:18.000000 caep-0.1.5/caep.egg-info/top_level.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-0.1.5/caep.egg-info/zip-safe
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-03-28 14:28:18.138058 caep-0.1.5/setup.cfg
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      953 2023-03-28 14:28:15.000000 caep-0.1.5/setup.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-28 14:28:18.138058 caep-0.1.5/tests/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-0.1.5/tests/test_config.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1455 2023-03-28 05:50:28.000000 caep-0.1.5/tests/test_helpers.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9429 2023-03-28 14:28:15.000000 caep-0.1.5/tests/test_schema.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-10 07:37:22.935539 caep-0.1.6/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-0.1.6/LICENSE
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-04-10 07:37:22.935539 caep-0.1.6/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9157 2023-03-28 14:28:15.000000 caep-0.1.6/README.md
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-10 07:37:22.932205 caep-0.1.6/caep/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-0.1.6/caep/__init__.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8106 2023-04-10 07:37:20.000000 caep-0.1.6/caep/config.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-0.1.6/caep/example.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1396 2023-03-28 05:50:28.000000 caep-0.1.6/caep/helpers.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11081 2023-01-30 11:31:45.000000 caep-0.1.6/caep/schema.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-0.1.6/caep/xdg.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-10 07:37:22.932205 caep-0.1.6/caep.egg-info/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      343 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       23 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/requires.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/top_level.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-0.1.6/caep.egg-info/zip-safe
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-04-10 07:37:22.935539 caep-0.1.6/setup.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      953 2023-04-10 07:37:20.000000 caep-0.1.6/setup.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-10 07:37:22.935539 caep-0.1.6/tests/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-0.1.6/tests/test_config.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1455 2023-03-28 05:50:28.000000 caep-0.1.6/tests/test_helpers.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9448 2023-04-10 07:37:20.000000 caep-0.1.6/tests/test_schema.py
```

### Comparing `caep-0.1.5/LICENSE` & `caep-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `caep-0.1.5/PKG-INFO` & `caep-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.5
+Version: 0.1.6
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caep-0.1.5/README.md` & `caep-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `caep-0.1.5/caep/config.py` & `caep-0.1.6/caep/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,13 +267,15 @@
 
     if cp and section_name:
         # Add (empty) section. In this way we can still access
         # the DEFAULT section
         if not cp.has_section(section_name):
             cp.add_section(section_name)
         config = dict(cp[section_name])
+    elif cp and cp.has_section("DEFAULT"):
+        config = dict(cp["DEFAULT"])
     else:
         config = {}
 
     parser.set_defaults(**all_defaults(parser, config))
 
     return parser.parse_args(remainder_argv)
```

### Comparing `caep-0.1.5/caep/example.py` & `caep-0.1.6/caep/example.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.5/caep/helpers.py` & `caep-0.1.6/caep/helpers.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.5/caep/schema.py` & `caep-0.1.6/caep/schema.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.5/caep/xdg.py` & `caep-0.1.6/caep/xdg.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.5/caep.egg-info/PKG-INFO` & `caep-0.1.6/caep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.5
+Version: 0.1.6
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caep-0.1.5/setup.py` & `caep-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), "rb") as f:
     long_description = f.read().decode("utf-8")
 
 setup(
     name="caep",
-    version="0.1.5",
+    version="0.1.6",
     author="mnemonic AS",
     zip_safe=True,
     author_email="opensource@mnemonic.no",
     description="Config Argument Env Parser (CAEP)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="ISC",
```

### Comparing `caep-0.1.5/tests/test_config.py` & `caep-0.1.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.5/tests/test_helpers.py` & `caep-0.1.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.5/tests/test_schema.py` & `caep-0.1.6/tests/test_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ test config """
+
 import ipaddress
 import os
 import shlex
 from pathlib import Path
 from typing import Dict, List, Optional, Set, Type
 
 import pytest
@@ -18,15 +19,14 @@
     split_list,
 )
 
 INI_TEST_FILE = os.path.join(os.path.dirname(__file__), "data/config_testdata.ini")
 
 
 class Arguments(BaseModel):
-
     str_arg: str = Field(description="Required String Argument")
     number: int = Field(default=1, description="Integer with default value")
     enabled: bool = Field(default=False, description="Boolean with default value")
 
     flag1: bool = Field(default=True, description="Boolean with default value")
 
     float_arg: float = Field(default=0.5, description="Float with default value")
@@ -237,15 +237,15 @@
     assert config.flag1 is True
 
 
 def test_schema_ini_default_only() -> None:
     """all arguments from ini file and default section"""
     commandline = shlex.split(f"--config {INI_TEST_FILE}")
 
-    config = parse_args(Arguments, commandline)
+    config = caep.load(Arg2, "Program description", opts=commandline)
 
     assert config.number == 3
 
 
 def test_argparse_env() -> None:
     """all arguments from env"""
 
@@ -304,37 +304,34 @@
 
     assert config.number == 10
     assert config.str_arg == "arg1"
     assert config.enabled is True
 
 
 def test_escape_split() -> None:
-
     assert escape_split("A\\,B\\,C,1\\,2\\,3") == ["A,B,C", "1,2,3"]
     assert escape_split("ABC 123", split=" ") == ["ABC", "123"]
 
     # Escaped slash
     assert escape_split("A\\\\BC 123", split=" ") == ["A\\BC", "123"]
 
 
 def test_split_list() -> None:
-
     # Default split = ","
     assert split_list("a,b,c", ArrayInfo(array_type=str))
 
     # Configure split value
     assert split_list("a b c", ArrayInfo(array_type=str, split=" "))
 
     # min_size
     with pytest.raises(FieldError):
         assert split_list("", ArrayInfo(array_type=str, min_size=1))
 
 
 def test_split_dict() -> None:
-
     # Defaults
     d = split_dict("a:b,b:c,c: value X", DictInfo(dict_type=str))
 
     assert d is not None
 
     assert d["c"] == "value X"
```

