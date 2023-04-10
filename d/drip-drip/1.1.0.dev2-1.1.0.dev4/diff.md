# Comparing `tmp/drip-drip-1.1.0.dev2.tar.gz` & `tmp/drip-drip-1.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drip-drip-1.1.0.dev2.tar", last modified: Fri Mar 24 19:50:56 2023, max compression
+gzip compressed data, was "/home/patton/Work/Nest/Workspaces/drip_drip/dist/.tmp-lusef3tx/drip-drip-1.1.0.dev4.tar", last modified: Mon Apr 10 21:19:49 2023, max compression
```

## Comparing `drip-drip-1.1.0.dev2.tar` & `drip-drip-1.1.0.dev4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 patton     (502) staff       (20)        0 2023-03-24 19:50:56.517130 drip-drip-1.1.0.dev2/
--rw-r--r--   0 patton     (502) staff       (20)     2426 2023-01-10 18:19:01.000000 drip-drip-1.1.0.dev2/LICENSE.txt
--rw-r--r--   0 patton     (502) staff       (20)     1439 2023-03-24 19:50:56.516879 drip-drip-1.1.0.dev2/PKG-INFO
--rw-r--r--   0 patton     (502) staff       (20)      898 2022-12-15 19:16:51.000000 drip-drip-1.1.0.dev2/README.md
--rw-r--r--   0 patton     (502) staff       (20)     1168 2023-03-24 19:50:51.000000 drip-drip-1.1.0.dev2/pyproject.toml
--rw-r--r--   0 patton     (502) staff       (20)       38 2023-03-24 19:50:56.517195 drip-drip-1.1.0.dev2/setup.cfg
-drwxr-xr-x   0 patton     (502) staff       (20)        0 2023-03-24 19:50:56.510407 drip-drip-1.1.0.dev2/src/
-drwxr-xr-x   0 patton     (502) staff       (20)        0 2023-03-24 19:50:56.510537 drip-drip-1.1.0.dev2/src/main/
-drwxr-xr-x   0 patton     (502) staff       (20)        0 2023-03-24 19:50:56.510672 drip-drip-1.1.0.dev2/src/main/python/
-drwxr-xr-x   0 patton     (502) staff       (20)        0 2023-03-24 19:50:56.512478 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/
-drwxr-xr-x   0 patton     (502) staff       (20)        0 2023-03-24 19:50:56.514586 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/
--rw-r--r--   0 patton     (502) staff       (20)      363 2022-11-02 23:24:08.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/__init__.py
--rw-r--r--   0 patton     (502) staff       (20)     1832 2023-03-09 19:02:48.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/dropper.py
--rw-r--r--   0 patton     (502) staff       (20)     5080 2023-03-09 20:21:39.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/feeder.py
--rw-r--r--   0 patton     (502) staff       (20)     4409 2023-03-09 19:09:43.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/file_dropper.py
--rw-r--r--   0 patton     (502) staff       (20)        0 2022-11-02 23:00:45.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/py.typed
--rw-r--r--   0 patton     (502) staff       (20)     3143 2023-03-08 16:13:32.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/utils.py
-drwxr-xr-x   0 patton     (502) staff       (20)        0 2023-03-24 19:50:56.516480 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_drip.egg-info/
--rw-r--r--   0 patton     (502) staff       (20)     1439 2023-03-24 19:50:56.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_drip.egg-info/PKG-INFO
--rw-r--r--   0 patton     (502) staff       (20)      614 2023-03-24 19:50:56.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_drip.egg-info/SOURCES.txt
--rw-r--r--   0 patton     (502) staff       (20)        1 2023-03-24 19:50:56.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_drip.egg-info/dependency_links.txt
--rw-r--r--   0 patton     (502) staff       (20)       90 2023-03-24 19:50:56.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_drip.egg-info/entry_points.txt
--rw-r--r--   0 patton     (502) staff       (20)       15 2023-03-24 19:50:56.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_drip.egg-info/top_level.txt
--rw-r--r--   0 patton     (502) staff       (20)     4721 2023-02-08 00:58:32.000000 drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_feed.py
+drwxrwxr-x   0 patton    (1002) patton    (1006)        0 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/
+-rw-rw-r--   0 patton    (1002) patton    (1006)     2426 2023-01-30 21:53:37.000000 drip-drip-1.1.0.dev4/LICENSE.txt
+-rw-rw-r--   0 patton    (1002) patton    (1006)     1439 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/PKG-INFO
+-rw-rw-r--   0 patton    (1002) patton    (1006)      898 2023-01-30 21:53:37.000000 drip-drip-1.1.0.dev4/README.md
+-rw-rw-r--   0 patton    (1002) patton    (1006)     1173 2023-04-10 21:19:38.000000 drip-drip-1.1.0.dev4/pyproject.toml
+-rw-rw-r--   0 patton    (1002) patton    (1006)       38 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/setup.cfg
+drwxrwxr-x   0 patton    (1002) patton    (1006)        0 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/
+drwxrwxr-x   0 patton    (1002) patton    (1006)        0 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/
+drwxrwxr-x   0 patton    (1002) patton    (1006)        0 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/python/
+drwxrwxr-x   0 patton    (1002) patton    (1006)        0 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/
+drwxrwxr-x   0 patton    (1002) patton    (1006)        0 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/
+-rw-rw-r--   0 patton    (1002) patton    (1006)      363 2023-01-30 21:53:37.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/__init__.py
+-rw-rw-r--   0 patton    (1002) patton    (1006)     4726 2023-04-10 21:18:21.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/drip_feed.py
+-rw-rw-r--   0 patton    (1002) patton    (1006)     1832 2023-04-10 21:18:21.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/dropper.py
+-rw-rw-r--   0 patton    (1002) patton    (1006)     5080 2023-04-10 21:18:21.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/feeder.py
+-rw-rw-r--   0 patton    (1002) patton    (1006)     4409 2023-04-10 21:18:21.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/file_dropper.py
+-rw-rw-r--   0 patton    (1002) patton    (1006)        0 2023-01-30 21:53:37.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/py.typed
+-rw-rw-r--   0 patton    (1002) patton    (1006)     3589 2023-04-10 21:18:21.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/utils.py
+drwxrwxr-x   0 patton    (1002) patton    (1006)        0 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip_drip.egg-info/
+-rw-rw-r--   0 patton    (1002) patton    (1006)     1439 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip_drip.egg-info/PKG-INFO
+-rw-rw-r--   0 patton    (1002) patton    (1006)      619 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip_drip.egg-info/SOURCES.txt
+-rw-rw-r--   0 patton    (1002) patton    (1006)        1 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip_drip.egg-info/dependency_links.txt
+-rw-rw-r--   0 patton    (1002) patton    (1006)       95 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip_drip.egg-info/entry_points.txt
+-rw-rw-r--   0 patton    (1002) patton    (1006)       15 2023-04-10 21:19:49.000000 drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip_drip.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `drip-drip-1.1.0.dev2/LICENSE.txt` & `drip-drip-1.1.0.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drip-drip-1.1.0.dev2/PKG-INFO` & `drip-drip-1.1.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drip-drip
-Version: 1.1.0.dev2
+Version: 1.1.0.dev4
 Summary: Provides a utility to control automatic execution when conditions are met.
 Author-email: Simon Patton <sjpatton@lbl.gov>
 License: BSD-3-Clause-LBNL
 Keywords: drip,drip feed,drip-drip
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `drip-drip-1.1.0.dev2/README.md` & `drip-drip-1.1.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `drip-drip-1.1.0.dev2/pyproject.toml` & `drip-drip-1.1.0.dev4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "drip-drip"
-version = "1.1.0.dev2"
+version = "1.1.0.dev4"
 description = "Provides a utility to control automatic execution when conditions are met."
 readme = "README.md"
 authors = [
     { "name"="Simon Patton", "email" ="sjpatton@lbl.gov"}
 ]
 license = { text = "BSD-3-Clause-LBNL" }
 classifiers=[  # Optional
@@ -19,15 +19,15 @@
 ]
 keywords=["drip", "drip feed", "drip-drip"]  # Optional
 # dependencies = [ # Optional
 # ]
 requires-python = ">=3.10.6, <4"
 
 [project.scripts]
-drip_feed = "drip_feed:main"
+drip_feed = "drip.drip_feed:main"
 
 # Note the quotes around drip.dropper in order to escape the dot .
 [project.entry-points."drip.dropper"]
 file_drip = "drip:FileDropper"
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
```

### Comparing `drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/dropper.py` & `drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/dropper.py`

 * *Files identical despite different names*

### Comparing `drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/feeder.py` & `drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/feeder.py`

 * *Files identical despite different names*

### Comparing `drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/file_dropper.py` & `drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/file_dropper.py`

 * *Files identical despite different names*

### Comparing `drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip/utils.py` & `drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,59 @@
-"""Provide utilities to help using the drip-drip package"""
+"""Provide utilities to help using the drip_drip module"""
 
 from typing import Dict, List, Optional, Union
 
 from argparse import Namespace
 from configparser import ConfigParser
+from pathlib import Path
 import os
 
 DEFAULT_INI_FILE = "drip_feed.ini"
 
 
 Configs = dict[str, Union[bool, int, str, None]]
 
 
-def find_config(config_file):
+def find_config(config_file: Optional[str]) -> Path:
     """
     Returns the configuration file depending on the value of the config file passed.
+
+    Args:
+        config_file: the name, if any, of the config file to find.
+
+    Returns:
+        the path to the found config file
+
+    Raises:
+        ValueError: when no config file can be found.
     """
     if None is config_file:
         if "HOME" in os.environ:
             result = os.path.join(os.environ["HOME"], DEFAULT_INI_FILE)
         else:
             raise ValueError(
                 "Can not find INI file $HOME/"
                 + DEFAULT_INI_FILE
                 + ", make sure HOME is defined"
             )
     else:
         result = config_file
     if not os.path.exists(result):
-        raise ValueError("Can not find INI file " + result + ", is does not exist")
-    return result
+        raise ValueError("Can not find INI file " + result + ", it does not exist")
+    return Path(result)
 
 
-def read_envar_values(mapping: Dict[str, str]):
+def read_envar_values(mapping: Dict[str, str]) -> Namespace:
     """
     Create a argparse.Namespace instance populated by the values of the
     envrionmental variables specified by the keys of the mapping.
+
+    Args:
+        mapping: the mapping of environmental variables to the
+                matching option name.
     """
     result = {}
     for key in mapping.keys():
         value = os.getenv(key)
         if None is not value:
             option = mapping[key]
             result[option] = value
@@ -52,18 +66,20 @@
     strings: Optional[List[str]] = None,
     integers: Optional[List[str]] = None,
     booleans: Optional[List[str]] = None,
 ) -> Configs:
     """
     Reads the supplied configuration ini
 
-    :param config_file: the path to the file containing the configuration information.
-    :param section: the section within the file containing the configuration for this instance.
-    :param booleans: a List of keys that should be returned as bools.
-    :param integers: a List of keys that should be returned as integers.
+    Args:
+        config_file: the path to the file containing the configuration information.
+        section: the section within the file containing the configuration for this instance.
+        booleans: a List of keys that should be returned as strings.
+        booleans: a List of keys that should be returned as bools.
+        integers: a List of keys that should be returned as integers.
     """
 
     config_parser = ConfigParser()
     filepath = find_config(config_file)
 
     config_parser.read(filepath)
     config: Configs = {}
```

### Comparing `drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_drip.egg-info/PKG-INFO` & `drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip_drip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drip-drip
-Version: 1.1.0.dev2
+Version: 1.1.0.dev4
 Summary: Provides a utility to control automatic execution when conditions are met.
 Author-email: Simon Patton <sjpatton@lbl.gov>
 License: BSD-3-Clause-LBNL
 Keywords: drip,drip feed,drip-drip
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_drip.egg-info/SOURCES.txt` & `drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip_drip.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE.txt
 README.md
 pyproject.toml
-src/main/python/drip_pkg/drip_feed.py
 src/main/python/drip_pkg/drip/__init__.py
+src/main/python/drip_pkg/drip/drip_feed.py
 src/main/python/drip_pkg/drip/dropper.py
 src/main/python/drip_pkg/drip/feeder.py
 src/main/python/drip_pkg/drip/file_dropper.py
 src/main/python/drip_pkg/drip/py.typed
 src/main/python/drip_pkg/drip/utils.py
 src/main/python/drip_pkg/drip_drip.egg-info/PKG-INFO
 src/main/python/drip_pkg/drip_drip.egg-info/SOURCES.txt
```

### Comparing `drip-drip-1.1.0.dev2/src/main/python/drip_pkg/drip_feed.py` & `drip-drip-1.1.0.dev4/src/main/python/drip_pkg/drip/drip_feed.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import argparse
 from importlib.metadata import entry_points
 import logging
 import os
 import sys
 
-import drip
+from . import utils, Dropper, Feeder
 
 _ENVARS_MAPPING = {
     "DRIP_INI_FILE": "INI_FILE",
     "DRIP_INI_SECTION": "INI_SECTION",
     "DRIP_BATCH_SIZE": "BATCH_SIZE",
     "DRIP_PAUSE_INTERVAL": "PAUSE_INTERVAL",
     "DRIP_REFILL_INTERVAL": "REFILL_INTERVAL",
@@ -39,15 +39,15 @@
     )
     parser.add_argument(
         "-i",
         "--drip_ini",
         dest="INI_FILE",
         help="The path to the configuration file for the drip.Dropper class,"
         + " the default is $HOME/"
-        + drip.utils.DEFAULT_INI_FILE,
+        + utils.DEFAULT_INI_FILE,
     )
     parser.add_argument(
         "-s",
         "--ini_section",
         dest="INI_SECTION",
         default="drip_feed",
         help="The section of the INI file to use for this execution,"
@@ -92,15 +92,15 @@
             dest="DROPPER_CLASS",
             nargs=1,
             help="The package:Class defining to drip:Dropper subclass to execute",
         )
     return parser
 
 
-def select_dropper_class(name) -> Type[drip.Dropper]:
+def select_dropper_class(name) -> Type[Dropper]:
     """
     Returns the selected drop.Dropper class object.
     """
     droppers = entry_points(group="drip.dropper")
     known_values = []
     logging.debug("Begin known Droppers:")
     for entry in droppers:
@@ -119,15 +119,15 @@
     Main routine that executes an instance of a drop.Dropper class.
     """
     # Test for environmental definition of dropper class.
     dropper_name = None
     if "DRIP_DROPPER" in os.environ:
         dropper_name = os.environ["DRIP_DROPPER"]
     parser = _create_argument_parser(None is dropper_name)
-    envar_values = drip.utils.read_envar_values(_ENVARS_MAPPING)
+    envar_values = utils.read_envar_values(_ENVARS_MAPPING)
     options = parser.parse_args(namespace=envar_values)
 
     if None is options.LOG_FILE:
         logging.basicConfig(stream=sys.stdout, level=_LOG_LEVELS[options.LOG_LEVEL])
     else:
         logging.basicConfig(
             filename=options.LOG_FILE, level=_LOG_LEVELS[options.LOG_LEVEL]
@@ -139,18 +139,18 @@
             logging.debug("    %s = %s", option, options.__dict__[option])
     logging.debug("End options:")
     if None is dropper_name:
         dropper_name = options.DROPPER_CLASS[0]
     dropper_class = select_dropper_class(dropper_name)
     logging.info("Drip feeding using the %s Class", dropper_name)
 
-    ini_file = drip.utils.find_config(options.INI_FILE)
-    dropper = dropper_class(ini_file, options.INI_SECTION)
+    ini_file = utils.find_config(options.INI_FILE)
+    dropper = dropper_class(str(ini_file), options.INI_SECTION)
 
-    feeder = drip.Feeder(
+    feeder = Feeder(
         dropper,
         batch_size=int(options.BATCH_SIZE),
         pause_interval=int(options.PAUSE_INTERVAL),
         refill_interval=int(options.REFILL_INTERVAL),
     )
 
     feeder.run()
```

