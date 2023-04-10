# Comparing `tmp/tinymovr-1.2.5.tar.gz` & `tmp/tinymovr-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinymovr-1.2.5.tar", last modified: Thu Apr  6 13:07:46 2023, max compression
+gzip compressed data, was "tinymovr-1.2.7.tar", last modified: Mon Apr 10 19:05:14 2023, max compression
```

## Comparing `tinymovr-1.2.5.tar` & `tinymovr-1.2.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 13:07:46.175089 tinymovr-1.2.5/
--rw-rw-rw-   0        0        0     2245 2023-04-06 13:07:46.175089 tinymovr-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1735 2023-03-13 07:31:22.000000 tinymovr-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-06 13:07:46.176089 tinymovr-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2330 2023-04-04 13:46:51.000000 tinymovr-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:07:46.149089 tinymovr-1.2.5/tinymovr/
--rw-rw-rw-   0        0        0       55 2023-03-10 10:27:34.000000 tinymovr-1.2.5/tinymovr/__init__.py
--rw-rw-rw-   0        0        0     3639 2023-03-10 10:27:34.000000 tinymovr-1.2.5/tinymovr/channel.py
--rw-rw-rw-   0        0        0     2966 2023-04-06 12:59:26.000000 tinymovr-1.2.5/tinymovr/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:07:46.164089 tinymovr-1.2.5/tinymovr/codec/
--rw-rw-rw-   0        0        0       66 2022-06-07 06:55:58.000000 tinymovr-1.2.5/tinymovr/codec/__init__.py
--rw-rw-rw-   0        0        0     3036 2023-03-10 10:27:34.000000 tinymovr-1.2.5/tinymovr/codec/codec.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:07:46.166089 tinymovr-1.2.5/tinymovr/config/
--rw-rw-rw-   0        0        0      167 2023-03-10 10:27:34.000000 tinymovr-1.2.5/tinymovr/config/__init__.py
--rw-rw-rw-   0        0        0     3457 2023-03-10 10:27:34.000000 tinymovr-1.2.5/tinymovr/config/config.py
--rw-rw-rw-   0        0        0     1107 2023-03-10 10:27:34.000000 tinymovr-1.2.5/tinymovr/constants.py
--rw-rw-rw-   0        0        0     3389 2023-03-20 08:12:07.000000 tinymovr-1.2.5/tinymovr/discovery.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:07:46.173090 tinymovr-1.2.5/tinymovr/gui/
--rw-rw-rw-   0        0        0      428 2023-03-10 10:27:34.000000 tinymovr-1.2.5/tinymovr/gui/__init__.py
--rw-rw-rw-   0        0        0     1762 2023-04-06 12:59:26.000000 tinymovr-1.2.5/tinymovr/gui/gui.py
--rw-rw-rw-   0        0        0     9242 2023-03-10 10:27:34.000000 tinymovr-1.2.5/tinymovr/gui/helpers.py
--rw-rw-rw-   0        0        0    12517 2023-03-20 08:12:07.000000 tinymovr-1.2.5/tinymovr/gui/window.py
--rw-rw-rw-   0        0        0     4602 2023-04-04 13:46:51.000000 tinymovr-1.2.5/tinymovr/gui/worker.py
--rw-rw-rw-   0        0        0     3206 2023-03-10 10:27:34.000000 tinymovr-1.2.5/tinymovr/tee.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:07:46.159089 tinymovr-1.2.5/tinymovr.egg-info/
--rw-rw-rw-   0        0        0     2245 2023-04-06 13:07:45.000000 tinymovr-1.2.5/tinymovr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-04-06 13:07:46.000000 tinymovr-1.2.5/tinymovr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 13:07:45.000000 tinymovr-1.2.5/tinymovr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-06 13:07:45.000000 tinymovr-1.2.5/tinymovr.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      135 2023-04-06 13:07:45.000000 tinymovr-1.2.5/tinymovr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 13:07:45.000000 tinymovr-1.2.5/tinymovr.egg-info/top_level.txt
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.320796 tinymovr-1.2.7/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-10 19:05:14.320414 tinymovr-1.2.7/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.2.7/README.md
+-rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-10 19:05:14.320946 tinymovr-1.2.7/setup.cfg
+-rw-r--r--   0 yanconst   (501) staff       (20)     2369 2023-04-10 19:03:18.000000 tinymovr-1.2.7/setup.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.312111 tinymovr-1.2.7/tinymovr/
+-rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3529 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2882 2023-04-10 19:03:18.000000 tinymovr-1.2.7/tinymovr/cli.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.316466 tinymovr-1.2.7/tinymovr/codec/
+-rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.2.7/tinymovr/codec/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/codec/codec.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.317284 tinymovr-1.2.7/tinymovr/config/
+-rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/config/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3358 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/config/config.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/constants.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/discovery.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.319799 tinymovr-1.2.7/tinymovr/gui/
+-rw-r--r--   0 yanconst   (501) staff       (20)      411 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/gui/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1718 2023-04-10 19:03:18.000000 tinymovr-1.2.7/tinymovr/gui/gui.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     8904 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/gui/helpers.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    12186 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/gui/window.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/gui/worker.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3088 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/tee.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.315380 tinymovr-1.2.7/tinymovr.egg-info/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)      549 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/SOURCES.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/dependency_links.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/entry_points.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)      158 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/requires.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/top_level.txt
```

### Comparing `tinymovr-1.2.5/PKG-INFO` & `tinymovr-1.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,60 @@
-Metadata-Version: 2.1
-Name: tinymovr
-Version: 1.2.5
-Summary: Tinymovr Studio
-Home-page: https://github.com/yconst/Tinymovr
-Author: Yannis Chatzikonstantinou
-Author-email: info@tinymovr.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: gui
-
-![Studio Lint Test](https://github.com/yconst/tinymovr/workflows/Tinymovr%20Studio%20Lint%2FTest/badge.svg)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-## Tinymovr Studio Python
-
-This is the Python client library and application that allows easy interfacing with the Tinymovr motor control board.
-
-### Installing using pip
-
-This is the most straightforward method to install Tinymovr studio and have access to hardware. We use pip3 to ensure Tinymovr is installed using Python 3 (required).
-
-    pip3 install tinymovr
-
-### Installing using git clone
-
-First clone the Tinymovr repo to a local directory:
-
-    git clone https://github.com/yconst/Tinymovr
-
-Then cd to the cloned repo directory and install in developer mode:
-
-    cd Tinymovr/studio/Python
-    pip3 install -e .
-
-### Launching the GUI app
-
-    tinymovr
-
-### Launching the command line app
-
-    tinymovr_cli
-
-## Getting Help
-
-[Full documentation is available at Readthedocs](https://tinymovr.readthedocs.io).
-
-Please visit the [Discussions Page](https://github.com/tinymovr/Tinymovr/discussions) and the [Discord Server](https://discord.gg/vNvmpfthug) to ask any questions. If you are unable to find an answer to your question, you are welcome to [start a new discussion](https://github.com/tinymovr/Tinymovr/discussions/new/choose) or ask away at [our Discord server](https://discord.gg/vNvmpfthug).
-
-If you would like to propose a feature or think you have found a bug, [open a new issue](https://github.com/tinymovr/Tinymovr/issues/new).
-
-### More information
-
-[Website and Store](https://tinymovr.com)
-
-[Documentation](https://tinymovr.readthedocs.io)
-
-
-
+Metadata-Version: 2.1
+Name: tinymovr
+Version: 1.2.7
+Summary: Tinymovr Studio
+Home-page: https://github.com/yconst/Tinymovr
+Author: Yannis Chatzikonstantinou
+Author-email: info@tinymovr.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: gui
+
+![Studio Lint Test](https://github.com/yconst/tinymovr/workflows/Tinymovr%20Studio%20Lint%2FTest/badge.svg)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+## Tinymovr Studio Python
+
+This is the Python client library and application that allows easy interfacing with the Tinymovr motor control board.
+
+### Installing using pip
+
+This is the most straightforward method to install Tinymovr studio and have access to hardware. We use pip3 to ensure Tinymovr is installed using Python 3 (required).
+
+    pip3 install tinymovr
+
+### Installing using git clone
+
+First clone the Tinymovr repo to a local directory:
+
+    git clone https://github.com/yconst/Tinymovr
+
+Then cd to the cloned repo directory and install in developer mode:
+
+    cd Tinymovr/studio/Python
+    pip3 install -e .
+
+### Launching the GUI app
+
+    tinymovr
+
+### Launching the command line app
+
+    tinymovr_cli
+
+## Getting Help
+
+[Full documentation is available at Readthedocs](https://tinymovr.readthedocs.io).
+
+Please visit the [Discussions Page](https://github.com/tinymovr/Tinymovr/discussions) and the [Discord Server](https://discord.gg/vNvmpfthug) to ask any questions. If you are unable to find an answer to your question, you are welcome to [start a new discussion](https://github.com/tinymovr/Tinymovr/discussions/new/choose) or ask away at [our Discord server](https://discord.gg/vNvmpfthug).
+
+If you would like to propose a feature or think you have found a bug, [open a new issue](https://github.com/tinymovr/Tinymovr/issues/new).
+
+### More information
+
+[Website and Store](https://tinymovr.com)
+
+[Documentation](https://tinymovr.readthedocs.io)
+
```

### Comparing `tinymovr-1.2.5/README.md` & `tinymovr-1.2.7/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-![Studio Lint Test](https://github.com/yconst/tinymovr/workflows/Tinymovr%20Studio%20Lint%2FTest/badge.svg)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-## Tinymovr Studio Python
-
-This is the Python client library and application that allows easy interfacing with the Tinymovr motor control board.
-
-### Installing using pip
-
-This is the most straightforward method to install Tinymovr studio and have access to hardware. We use pip3 to ensure Tinymovr is installed using Python 3 (required).
-
-    pip3 install tinymovr
-
-### Installing using git clone
-
-First clone the Tinymovr repo to a local directory:
-
-    git clone https://github.com/yconst/Tinymovr
-
-Then cd to the cloned repo directory and install in developer mode:
-
-    cd Tinymovr/studio/Python
-    pip3 install -e .
-
-### Launching the GUI app
-
-    tinymovr
-
-### Launching the command line app
-
-    tinymovr_cli
-
-## Getting Help
-
-[Full documentation is available at Readthedocs](https://tinymovr.readthedocs.io).
-
-Please visit the [Discussions Page](https://github.com/tinymovr/Tinymovr/discussions) and the [Discord Server](https://discord.gg/vNvmpfthug) to ask any questions. If you are unable to find an answer to your question, you are welcome to [start a new discussion](https://github.com/tinymovr/Tinymovr/discussions/new/choose) or ask away at [our Discord server](https://discord.gg/vNvmpfthug).
-
-If you would like to propose a feature or think you have found a bug, [open a new issue](https://github.com/tinymovr/Tinymovr/issues/new).
-
-### More information
-
-[Website and Store](https://tinymovr.com)
-
-[Documentation](https://tinymovr.readthedocs.io)
-
+![Studio Lint Test](https://github.com/yconst/tinymovr/workflows/Tinymovr%20Studio%20Lint%2FTest/badge.svg)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+## Tinymovr Studio Python
+
+This is the Python client library and application that allows easy interfacing with the Tinymovr motor control board.
+
+### Installing using pip
+
+This is the most straightforward method to install Tinymovr studio and have access to hardware. We use pip3 to ensure Tinymovr is installed using Python 3 (required).
+
+    pip3 install tinymovr
+
+### Installing using git clone
+
+First clone the Tinymovr repo to a local directory:
+
+    git clone https://github.com/yconst/Tinymovr
+
+Then cd to the cloned repo directory and install in developer mode:
+
+    cd Tinymovr/studio/Python
+    pip3 install -e .
+
+### Launching the GUI app
+
+    tinymovr
+
+### Launching the command line app
+
+    tinymovr_cli
+
+## Getting Help
+
+[Full documentation is available at Readthedocs](https://tinymovr.readthedocs.io).
+
+Please visit the [Discussions Page](https://github.com/tinymovr/Tinymovr/discussions) and the [Discord Server](https://discord.gg/vNvmpfthug) to ask any questions. If you are unable to find an answer to your question, you are welcome to [start a new discussion](https://github.com/tinymovr/Tinymovr/discussions/new/choose) or ask away at [our Discord server](https://discord.gg/vNvmpfthug).
+
+If you would like to propose a feature or think you have found a bug, [open a new issue](https://github.com/tinymovr/Tinymovr/issues/new).
+
+### More information
+
+[Website and Store](https://tinymovr.com)
+
+[Documentation](https://tinymovr.readthedocs.io)
+
```

### Comparing `tinymovr-1.2.5/setup.py` & `tinymovr-1.2.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,72 @@
-"""
-Tinymovr Setup Module
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-Standard Python module for setting up the Tinymovr package
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import pathlib
-from setuptools import setup, find_packages
-
-# The directory containing this file
-HERE = pathlib.Path(__file__).parent
-
-# The text of the README file
-README = (HERE / "README.md").read_text()
-
-setup(
-    name="tinymovr",
-    # version="", #version will be taken from git tag
-    author="Yannis Chatzikonstantinou",
-    author_email="info@tinymovr.com",
-    description="Tinymovr Studio",
-    long_description=README,
-    long_description_content_type="text/markdown",
-    url="https://github.com/yconst/Tinymovr",
-    packages=find_packages(include=["tinymovr", "tinymovr.*"]),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-        "Operating System :: OS Independent",
-    ],
-    python_requires=">=3.9",
-    setuptools_git_versioning={
-        "enabled": True,
-        "dev_template": "{tag}+post{ccount}",
-        "dirty_template": "{tag}+post{ccount}_dirty",
-    },
-    setup_requires=["setuptools-git-versioning<2"],
-    install_requires=[
-        "ipython",
-        "importlib_resources",
-        "python-can",
-        "python-can-canine",
-        "avlos",
-        "pyserial",
-        "pyusb",
-        "pyyaml",
-        "docopt",
-        "flatten-dict",
-        "pint",
-    ],
-    extras_require={"gui": ["pyside2", "pyqtgraph"]},
-    entry_points={
-        "console_scripts": [
-            "tinymovr_cli=tinymovr.cli:spawn",
-            "tinymovr=tinymovr.gui:spawn",
-        ]
-    },
-)
+"""
+Tinymovr Setup Module
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+Standard Python module for setting up the Tinymovr package
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import pathlib
+from setuptools import setup, find_packages
+
+# The directory containing this file
+HERE = pathlib.Path(__file__).parent
+
+# The text of the README file
+README = (HERE / "README.md").read_text()
+
+setup(
+    name="tinymovr",
+    # version="", #version will be taken from git tag
+    author="Yannis Chatzikonstantinou",
+    author_email="info@tinymovr.com",
+    description="Tinymovr Studio",
+    long_description=README,
+    long_description_content_type="text/markdown",
+    url="https://github.com/yconst/Tinymovr",
+    packages=find_packages(include=["tinymovr", "tinymovr.*"]),
+    package_data={'tinymovr': ['*.yaml']},
+    include_package_data=True,
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "Operating System :: OS Independent",
+    ],
+    python_requires=">=3.9",
+    setuptools_git_versioning={
+        "enabled": True,
+        "dev_template": "{tag}+post{ccount}",
+        "dirty_template": "{tag}+post{ccount}_dirty",
+    },
+    setup_requires=["setuptools-git-versioning<2"],
+    install_requires=[
+        "ipython",
+        "importlib_resources",
+        "python-can",
+        "python-can-canine",
+        "python-can-slcan_disco",
+        "avlos",
+        "pyserial",
+        "pyusb",
+        "pyyaml",
+        "docopt",
+        "flatten-dict",
+        "pint",
+    ],
+    extras_require={"gui": ["pyside2", "pyqtgraph"]},
+    entry_points={
+        "console_scripts": [
+            "tinymovr_cli=tinymovr.cli:spawn",
+            "tinymovr=tinymovr.gui:spawn",
+        ]
+    },
+)
```

### Comparing `tinymovr-1.2.5/tinymovr/channel.py` & `tinymovr-1.2.7/tinymovr/channel.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-"""
-Tinymovr CAN Channel Module
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-Implements a CAN bus communications channel
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from threading import Lock, Event
-import can
-from functools import cached_property
-from avlos.channel import BaseChannel
-from tinymovr.tee import get_tee
-from tinymovr.constants import (
-    CAN_DEV_MASK,
-    CAN_EP_SIZE,
-    CAN_EP_MASK,
-    CAN_SEQ_SIZE,
-    CAN_SEQ_MASK,
-)
-from tinymovr.codec import MultibyteCodec
-
-
-class ResponseError(Exception):
-    def __init__(self, kw, *args, **kwargs):
-        msg = "Node {} did not respond".format(kw)
-        super().__init__(msg, *args, **kwargs)
-        self.kw = kw
-
-
-class CANChannel(BaseChannel):
-    def __init__(self, node_id):
-        self.node_id = node_id
-        get_tee().add(
-            lambda frame: frame.is_remote_frame == False
-            and ids_from_arbitration(frame.arbitration_id)[2] == node_id,
-            self._recv_cb,
-        )
-        self.queue = []
-        self.lock = Lock()
-        self.evt = Event()
-
-    def _recv_cb(self, frame):
-        self.queue.append(frame)
-        self.evt.set()
-
-    def send(self, data, ep_id):
-        rtr = False if data and len(data) else True
-        get_tee().send(self.create_frame(ep_id, rtr, data))
-
-    def recv(self, ep_id, timeout=1.0):
-        with self.lock:
-            if not self.evt.wait(timeout=timeout):
-                print("missed")
-            self.evt.clear()
-            frame_id = arbitration_from_ids(ep_id, 0, self.node_id)
-            index = 0
-            while index < len(self.queue):
-                if self.queue[index].arbitration_id == frame_id:
-                    return self.queue.pop(index).data
-                index += 1  
-            raise ResponseError(self.node_id)
-        
-    def create_frame(self, endpoint_id, rtr=False, payload=None):
-        """
-        Generate a CAN frame using python-can Message class
-        """
-        return can.Message(
-            arbitration_id=arbitration_from_ids(endpoint_id, 0, self.node_id),
-            is_extended_id=True,
-            is_remote_frame=rtr,
-            data=payload,
-        )
-
-    @cached_property
-    def serializer(self):
-        return MultibyteCodec()
-
-
-# TODO: Implement unit test for these functions
-def ids_from_arbitration(arbitration_id):
-    """
-    Generate endpoint, message sequence and node ids
-    from a CAN arbitration id
-    """
-    node_id = (arbitration_id & CAN_DEV_MASK) >> (CAN_EP_SIZE + CAN_SEQ_SIZE)
-    seq_id = (arbitration_id & CAN_SEQ_MASK) >> CAN_EP_SIZE
-    ep_id = arbitration_id & CAN_EP_MASK
-    return ep_id, seq_id, node_id
-
-
-def arbitration_from_ids(ep_id, seq_id, node_id):
-    """
-    Generate a CAN arbitration id from endpoint,
-    message sequence and node ids
-    """
-    return (
-        ep_id & CAN_EP_MASK
-        | ((seq_id << CAN_EP_SIZE) & CAN_SEQ_MASK)
-        | ((node_id << (CAN_EP_SIZE + CAN_SEQ_SIZE)) & CAN_DEV_MASK)
-    )
+"""
+Tinymovr CAN Channel Module
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+Implements a CAN bus communications channel
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from threading import Lock, Event
+import can
+from functools import cached_property
+from avlos.channel import BaseChannel
+from tinymovr.tee import get_tee
+from tinymovr.constants import (
+    CAN_DEV_MASK,
+    CAN_EP_SIZE,
+    CAN_EP_MASK,
+    CAN_SEQ_SIZE,
+    CAN_SEQ_MASK,
+)
+from tinymovr.codec import MultibyteCodec
+
+
+class ResponseError(Exception):
+    def __init__(self, kw, *args, **kwargs):
+        msg = "Node {} did not respond".format(kw)
+        super().__init__(msg, *args, **kwargs)
+        self.kw = kw
+
+
+class CANChannel(BaseChannel):
+    def __init__(self, node_id):
+        self.node_id = node_id
+        get_tee().add(
+            lambda frame: frame.is_remote_frame == False
+            and ids_from_arbitration(frame.arbitration_id)[2] == node_id,
+            self._recv_cb,
+        )
+        self.queue = []
+        self.lock = Lock()
+        self.evt = Event()
+
+    def _recv_cb(self, frame):
+        self.queue.append(frame)
+        self.evt.set()
+
+    def send(self, data, ep_id):
+        rtr = False if data and len(data) else True
+        get_tee().send(self.create_frame(ep_id, rtr, data))
+
+    def recv(self, ep_id, timeout=1.0):
+        with self.lock:
+            if not self.evt.wait(timeout=timeout):
+                print("missed")
+            self.evt.clear()
+            frame_id = arbitration_from_ids(ep_id, 0, self.node_id)
+            index = 0
+            while index < len(self.queue):
+                if self.queue[index].arbitration_id == frame_id:
+                    return self.queue.pop(index).data
+                index += 1  
+            raise ResponseError(self.node_id)
+        
+    def create_frame(self, endpoint_id, rtr=False, payload=None):
+        """
+        Generate a CAN frame using python-can Message class
+        """
+        return can.Message(
+            arbitration_id=arbitration_from_ids(endpoint_id, 0, self.node_id),
+            is_extended_id=True,
+            is_remote_frame=rtr,
+            data=payload,
+        )
+
+    @cached_property
+    def serializer(self):
+        return MultibyteCodec()
+
+
+# TODO: Implement unit test for these functions
+def ids_from_arbitration(arbitration_id):
+    """
+    Generate endpoint, message sequence and node ids
+    from a CAN arbitration id
+    """
+    node_id = (arbitration_id & CAN_DEV_MASK) >> (CAN_EP_SIZE + CAN_SEQ_SIZE)
+    seq_id = (arbitration_id & CAN_SEQ_MASK) >> CAN_EP_SIZE
+    ep_id = arbitration_id & CAN_EP_MASK
+    return ep_id, seq_id, node_id
+
+
+def arbitration_from_ids(ep_id, seq_id, node_id):
+    """
+    Generate a CAN arbitration id from endpoint,
+    message sequence and node ids
+    """
+    return (
+        ep_id & CAN_EP_MASK
+        | ((seq_id << CAN_EP_SIZE) & CAN_SEQ_MASK)
+        | ((node_id << (CAN_EP_SIZE + CAN_SEQ_SIZE)) & CAN_DEV_MASK)
+    )
```

### Comparing `tinymovr-1.2.5/tinymovr/cli.py` & `tinymovr-1.2.7/tinymovr/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-"""Tinymovr Studio CLI
-
-Usage:
-    tinymovr_cli [--bus=<bus>] [--chan=<chan>] [--bitrate=<bitrate>]
-    tinymovr_cli -h | --help
-    tinymovr_cli --version
-
-Options:
-    --bus=<bus>  One or more interfaces to use, first available is used [default: canine,slcan].
-    --chan=<chan>  The bus device "channel".
-    --bitrate=<bitrate>  CAN bitrate [default: 1000000].
-"""
-
-import can
-from canine import CANineBus
-import pkg_resources
-import IPython
-from traitlets.config import Config
-from docopt import docopt
-
-from tinymovr import init_tee, destroy_tee
-from tinymovr.discovery import Discovery
-from tinymovr.constants import app_name, base_node_name
-from tinymovr.config import get_bus_config, configure_logging
-
-"""
-Tinymovr CLI Module
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-The Tinymovr Studio IPython-based command line interface
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-
-def spawn():
-    """
-    Spawns the Tinymovr Studio IPython-based CLI.
-    """
-    version = pkg_resources.require("tinymovr")[0].version
-    arguments = docopt(__doc__, version=app_name + " " + str(version))
-
-    logger = configure_logging()
-
-    buses = arguments["--bus"].rsplit(sep=",")
-    channel = arguments["--chan"]
-    bitrate = int(arguments["--bitrate"])
-
-    if not channel:
-        params = get_bus_config(buses)
-        params["bitrate"] = bitrate
-    else:
-        params = {"bustype": buses[0], "channel": channel, "bitrate": bitrate}
-
-    tms = {}
-    user_ns = {}
-    user_ns["tms"] = tms
-
-    def node_appeared(node, node_id):
-        node_name = "{}{}".format(base_node_name, node_id)
-        print("Found {} with device id {}".format(node_name, node.uid))
-        tms[node_id] = node
-        user_ns[node_name] = node
-
-    def node_disappeared(node_id):
-        node_name = "{}{}".format(base_node_name, node_id)
-        print("Lost {}".format(node_name))
-        del tms[node_id]
-        del user_ns[node_name]
-
-    print(app_name + " " + str(version))
-
-    init_tee(can.Bus(**params))
-    dsc = Discovery(node_appeared, node_disappeared, logger)
-    print("Listening for nodes...")
-
-    c = Config()
-    c.InteractiveShellApp.gui = "tk"
-    c.TerminalIPythonApp.display_banner = False
-    IPython.start_ipython(argv=[], config=c, user_ns=user_ns)
-    logger.debug("Exiting...")
-    destroy_tee()
+"""Tinymovr Studio CLI
+
+Usage:
+    tinymovr_cli [--bus=<bus>] [--chan=<chan>] [--bitrate=<bitrate>]
+    tinymovr_cli -h | --help
+    tinymovr_cli --version
+
+Options:
+    --bus=<bus>  One or more interfaces to use, first available is used [default: canine,slcan_disco].
+    --chan=<chan>  The bus device "channel".
+    --bitrate=<bitrate>  CAN bitrate [default: 1000000].
+"""
+
+import can
+from canine import CANineBus
+import pkg_resources
+import IPython
+from traitlets.config import Config
+from docopt import docopt
+
+from tinymovr import init_tee, destroy_tee
+from tinymovr.discovery import Discovery
+from tinymovr.constants import app_name, base_node_name
+from tinymovr.config import get_bus_config, configure_logging
+
+"""
+Tinymovr CLI Module
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+The Tinymovr Studio IPython-based command line interface
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+
+def spawn():
+    """
+    Spawns the Tinymovr Studio IPython-based CLI.
+    """
+    version = pkg_resources.require("tinymovr")[0].version
+    arguments = docopt(__doc__, version=app_name + " " + str(version))
+
+    logger = configure_logging()
+
+    buses = arguments["--bus"].rsplit(sep=",")
+    channel = arguments["--chan"]
+    bitrate = int(arguments["--bitrate"])
+
+    if not channel:
+        params = get_bus_config(buses)
+        params["bitrate"] = bitrate
+    else:
+        params = {"bustype": buses[0], "channel": channel, "bitrate": bitrate}
+
+    tms = {}
+    user_ns = {}
+    user_ns["tms"] = tms
+
+    def node_appeared(node, node_id):
+        node_name = "{}{}".format(base_node_name, node_id)
+        print("Found {} with device id {}".format(node_name, node.uid))
+        tms[node_id] = node
+        user_ns[node_name] = node
+
+    def node_disappeared(node_id):
+        node_name = "{}{}".format(base_node_name, node_id)
+        print("Lost {}".format(node_name))
+        del tms[node_id]
+        del user_ns[node_name]
+
+    print(app_name + " " + str(version))
+
+    init_tee(can.Bus(**params))
+    dsc = Discovery(node_appeared, node_disappeared, logger)
+    print("Listening for nodes...")
+
+    c = Config()
+    c.InteractiveShellApp.gui = "tk"
+    c.TerminalIPythonApp.display_banner = False
+    IPython.start_ipython(argv=[], config=c, user_ns=user_ns)
+    logger.debug("Exiting...")
+    destroy_tee()
```

### Comparing `tinymovr-1.2.5/tinymovr/codec/codec.py` & `tinymovr-1.2.7/tinymovr/codec/codec.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-"""
-Tinymovr Codecs Module
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-Implements codecs for various datatypes.
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from typing import Dict, List
-import struct
-from avlos.datatypes import DataType
-
-
-class Codec:
-    """
-    Generic codec base class
-    """
-
-    def serialize(self, value) -> bytes:
-        raise NotImplementedError()
-
-    def deserialize(self, buffer: bytes):
-        raise NotImplementedError()
-
-
-class StructCodec(Codec):
-    """
-    Python struct-based codec
-    Adapted from:
-    https://github.com/madcowswe/ODrive/blob/master/Firmware/fibre/python/fibre/remote_object.py
-    """
-
-    def __init__(self, struct_format, target_type: type):
-        self._struct_format = struct_format
-        self._target_type = target_type
-
-    def get_length(self) -> int:
-        return struct.calcsize(self._struct_format)
-
-    def serialize(self, value) -> bytes:
-        value = self._target_type(value)
-        return struct.pack(self._struct_format, value)
-
-    def deserialize(self, buffer: bytes):
-        trimmed_buffer: bytes = buffer[: self.get_length()]
-        value = struct.unpack(self._struct_format, trimmed_buffer)
-        value = value[0] if len(value) == 1 else value
-        return self._target_type(value)
-
-
-codecs: Dict[DataType, StructCodec] = {
-    DataType.BOOL: StructCodec("<?", bool),
-    DataType.INT8: StructCodec("<b", int),
-    DataType.UINT8: StructCodec("<B", int),
-    DataType.INT16: StructCodec("<h", int),
-    DataType.UINT16: StructCodec("<H", int),
-    DataType.INT32: StructCodec("<i", int),
-    DataType.UINT32: StructCodec("<I", int),
-    DataType.FLOAT: StructCodec("<f", float),
-}
-
-
-class MultibyteCodec(Codec):
-    def serialize(self, values, *args) -> bytearray:
-        """
-        Serialize a series of variables to a bytes array
-        """
-        buffer = bytearray()
-        assert len(values) == len(args)
-        for value, dtype in zip(values, args):
-            buffer.extend(codecs[dtype].serialize(value))
-        return buffer
-
-    def deserialize(self, data, *args) -> List:
-        """
-        Deserialize a bytes array to a tuple of values
-        """
-        index: int = 0
-        values = []
-        for dtype in args:
-            values.append(codecs[dtype].deserialize(data[index:]))
-            index += codecs[dtype].get_length()
-        return values
+"""
+Tinymovr Codecs Module
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+Implements codecs for various datatypes.
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from typing import Dict, List
+import struct
+from avlos.datatypes import DataType
+
+
+class Codec:
+    """
+    Generic codec base class
+    """
+
+    def serialize(self, value) -> bytes:
+        raise NotImplementedError()
+
+    def deserialize(self, buffer: bytes):
+        raise NotImplementedError()
+
+
+class StructCodec(Codec):
+    """
+    Python struct-based codec
+    Adapted from:
+    https://github.com/madcowswe/ODrive/blob/master/Firmware/fibre/python/fibre/remote_object.py
+    """
+
+    def __init__(self, struct_format, target_type: type):
+        self._struct_format = struct_format
+        self._target_type = target_type
+
+    def get_length(self) -> int:
+        return struct.calcsize(self._struct_format)
+
+    def serialize(self, value) -> bytes:
+        value = self._target_type(value)
+        return struct.pack(self._struct_format, value)
+
+    def deserialize(self, buffer: bytes):
+        trimmed_buffer: bytes = buffer[: self.get_length()]
+        value = struct.unpack(self._struct_format, trimmed_buffer)
+        value = value[0] if len(value) == 1 else value
+        return self._target_type(value)
+
+
+codecs: Dict[DataType, StructCodec] = {
+    DataType.BOOL: StructCodec("<?", bool),
+    DataType.INT8: StructCodec("<b", int),
+    DataType.UINT8: StructCodec("<B", int),
+    DataType.INT16: StructCodec("<h", int),
+    DataType.UINT16: StructCodec("<H", int),
+    DataType.INT32: StructCodec("<i", int),
+    DataType.UINT32: StructCodec("<I", int),
+    DataType.FLOAT: StructCodec("<f", float),
+}
+
+
+class MultibyteCodec(Codec):
+    def serialize(self, values, *args) -> bytearray:
+        """
+        Serialize a series of variables to a bytes array
+        """
+        buffer = bytearray()
+        assert len(values) == len(args)
+        for value, dtype in zip(values, args):
+            buffer.extend(codecs[dtype].serialize(value))
+        return buffer
+
+    def deserialize(self, data, *args) -> List:
+        """
+        Deserialize a bytes array to a tuple of values
+        """
+        index: int = 0
+        values = []
+        for dtype in args:
+            values.append(codecs[dtype].deserialize(data[index:]))
+            index += codecs[dtype].get_length()
+        return values
```

### Comparing `tinymovr-1.2.5/tinymovr/config/config.py` & `tinymovr-1.2.7/tinymovr/config/config.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-"""
-Tinymovr Configuration Module
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-Implements functions to configure various aspects of Studio.
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import yaml
-import logging
-from importlib_resources import files
-import can
-
-from avlos.deserializer import deserialize
-from tinymovr.codec import DataType
-from tinymovr.channel import CANChannel
-
-dev_def = None
-
-def_path_str = str(files("tinymovr").joinpath("config/device.yaml"))
-with open(def_path_str) as dev_def_raw:
-    dev_def = yaml.safe_load(dev_def_raw)
-
-
-class ProtocolVersionError(Exception):
-    def __init__(self, *args, **kwargs):
-        msg = (
-            "Incompatible protocol versions (hash mismatch)."
-            "Please try upgrading firmware & studio to the same version."
-        )
-        super().__init__(msg, *args, **kwargs)
-
-
-def get_bus_config(suggested_types=None):
-    """
-    Get the bus configuration (interface, channel) for
-    the first of the suggested interface types. Present
-    a pretty exception if none available.
-    """
-    configs = can.interface.detect_available_configs(suggested_types)
-    try:
-        return configs[0]
-    except IndexError as exc:
-        raise can.CanInitializationError("No active interface found") from exc
-
-
-def create_device(node_id):
-    """
-    Create a device with the defined ID.
-    The hash value will be retrieved from the remote.
-    """
-    chan = CANChannel(node_id)
-    node = deserialize(dev_def)
-    # We use the generated node to retrieve the hash from
-    # the remote. This is ok as long as we know that the
-    # hash endpoint will always be the 0th one. If there
-    # is a hash mismatch, we raise an exception, otherwise
-    # we return the device node as is.
-    node._channel = chan
-    # hash_uint32 is local, proto_hash is remote
-    if node.hash_uint32 != node.protocol_hash:
-        raise ProtocolVersionError()
-    return node
-
-
-def create_device_with_hash_msg(heartbeat_msg):
-    """
-    Create a device, the heartbeat msg will be used
-    to decode the actual hash value and id
-    """
-    node_id = heartbeat_msg.arbitration_id & 0x3F
-    chan = CANChannel(node_id)
-    node = deserialize(dev_def)
-    hash, *_ = chan.serializer.deserialize(heartbeat_msg.data[:4], DataType.UINT32)
-    if node.hash_uint32 != hash:  # hash_uint32 is local, hash is remote
-        raise ProtocolVersionError()
-    node._channel = chan
-    return node
-
-
-def configure_logging():
-    """
-    Configure logging for various modules
-    """
-    logging.getLogger("can.io.logger").setLevel(logging.WARNING)
-    logging.getLogger("parso").setLevel(logging.WARNING)
-    logging.getLogger("asyncio").setLevel(logging.WARNING)
-    logger = logging.getLogger("tinymovr")
-    logger.setLevel(logging.DEBUG)
-    return logger
+"""
+Tinymovr Configuration Module
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+Implements functions to configure various aspects of Studio.
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import yaml
+import logging
+from importlib_resources import files
+import can
+
+from avlos.deserializer import deserialize
+from tinymovr.codec import DataType
+from tinymovr.channel import CANChannel
+
+dev_def = None
+
+def_path_str = str(files("tinymovr").joinpath("config/device.yaml"))
+with open(def_path_str) as dev_def_raw:
+    dev_def = yaml.safe_load(dev_def_raw)
+
+
+class ProtocolVersionError(Exception):
+    def __init__(self, *args, **kwargs):
+        msg = (
+            "Incompatible protocol versions (hash mismatch)."
+            "Please try upgrading firmware & studio to the same version."
+        )
+        super().__init__(msg, *args, **kwargs)
+
+
+def get_bus_config(suggested_types=None):
+    """
+    Get the bus configuration (interface, channel) for
+    the first of the suggested interface types. Present
+    a pretty exception if none available.
+    """
+    configs = can.interface.detect_available_configs(suggested_types)
+    try:
+        return configs[0]
+    except IndexError as exc:
+        raise can.CanInitializationError("No active interface found") from exc
+
+
+def create_device(node_id):
+    """
+    Create a device with the defined ID.
+    The hash value will be retrieved from the remote.
+    """
+    chan = CANChannel(node_id)
+    node = deserialize(dev_def)
+    # We use the generated node to retrieve the hash from
+    # the remote. This is ok as long as we know that the
+    # hash endpoint will always be the 0th one. If there
+    # is a hash mismatch, we raise an exception, otherwise
+    # we return the device node as is.
+    node._channel = chan
+    # hash_uint32 is local, proto_hash is remote
+    if node.hash_uint32 != node.protocol_hash:
+        raise ProtocolVersionError()
+    return node
+
+
+def create_device_with_hash_msg(heartbeat_msg):
+    """
+    Create a device, the heartbeat msg will be used
+    to decode the actual hash value and id
+    """
+    node_id = heartbeat_msg.arbitration_id & 0x3F
+    chan = CANChannel(node_id)
+    node = deserialize(dev_def)
+    hash, *_ = chan.serializer.deserialize(heartbeat_msg.data[:4], DataType.UINT32)
+    if node.hash_uint32 != hash:  # hash_uint32 is local, hash is remote
+        raise ProtocolVersionError()
+    node._channel = chan
+    return node
+
+
+def configure_logging():
+    """
+    Configure logging for various modules
+    """
+    logging.getLogger("can.io.logger").setLevel(logging.WARNING)
+    logging.getLogger("parso").setLevel(logging.WARNING)
+    logging.getLogger("asyncio").setLevel(logging.WARNING)
+    logger = logging.getLogger("tinymovr")
+    logger.setLevel(logging.DEBUG)
+    return logger
```

### Comparing `tinymovr-1.2.5/tinymovr/constants.py` & `tinymovr-1.2.7/tinymovr/constants.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""
-Tinymovr Constants
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-Defines various constants used throughout Tinymovr Studio
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import math
-from enum import IntEnum
-
-
-app_name = "Tinymovr Studio"
-base_node_name = "tm"
-HEARTBEAT_BASE = 0x700
-
-CAN_EP_SIZE = 12
-CAN_EP_MASK = (1 << CAN_EP_SIZE) - 1
-CAN_SEQ_SIZE = 9
-CAN_SEQ_MASK = ((1 << CAN_SEQ_SIZE) - 1) << CAN_EP_SIZE
-CAN_DEV_SIZE = 8
-CAN_DEV_MASK = ((1 << CAN_DEV_SIZE) - 1) << (CAN_EP_SIZE + CAN_SEQ_SIZE)
-
+"""
+Tinymovr Constants
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+Defines various constants used throughout Tinymovr Studio
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import math
+from enum import IntEnum
+
+
+app_name = "Tinymovr Studio"
+base_node_name = "tm"
+HEARTBEAT_BASE = 0x700
+
+CAN_EP_SIZE = 12
+CAN_EP_MASK = (1 << CAN_EP_SIZE) - 1
+CAN_SEQ_SIZE = 9
+CAN_SEQ_MASK = ((1 << CAN_SEQ_SIZE) - 1) << CAN_EP_SIZE
+CAN_DEV_SIZE = 8
+CAN_DEV_MASK = ((1 << CAN_DEV_SIZE) - 1) << (CAN_EP_SIZE + CAN_SEQ_SIZE)
+
```

### Comparing `tinymovr-1.2.5/tinymovr/gui/gui.py` & `tinymovr-1.2.7/tinymovr/gui/gui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-"""Tinymovr Studio GUI
-
-Usage:
-    tinymovr [--bus=<bus>] [--chan=<chan>] [--bitrate=<bitrate>]
-    tinymovr -h | --help
-    tinymovr --version
-
-Options:
-    --bus=<bus>  One or more interfaces to use, first available is used [default: canine,slcan].
-    --chan=<chan>  The bus device "channel".
-    --bitrate=<bitrate>  CAN bitrate [default: 1000000].
-"""
-
-import sys
-import pkg_resources
-from docopt import docopt
-from PySide2.QtWidgets import QApplication
-from tinymovr.gui import MainWindow, app_stylesheet
-from tinymovr.constants import app_name
-
-
-"""
-Tinymovr Studio GUI
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-The graphical user interface of Tinymovr Studio
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-# https://www.loekvandenouweland.com/content/pyside2-big-sur-does-not-show-window.html
-import os
-os.environ['QT_MAC_WANTS_LAYER'] = '1'
-
-def spawn():
-    version = pkg_resources.require("tinymovr")[0].version
-    arguments = docopt(__doc__, version=app_name + " " + str(version))
-    app = QApplication(sys.argv)
-    app.setStyleSheet(app_stylesheet)
-    w = MainWindow(app, arguments)
-    w.show()
-    sys.exit(app.exec_())
+"""Tinymovr Studio GUI
+
+Usage:
+    tinymovr [--bus=<bus>] [--chan=<chan>] [--bitrate=<bitrate>]
+    tinymovr -h | --help
+    tinymovr --version
+
+Options:
+    --bus=<bus>  One or more interfaces to use, first available is used [default: canine,slcan_disco].
+    --chan=<chan>  The bus device "channel".
+    --bitrate=<bitrate>  CAN bitrate [default: 1000000].
+"""
+
+import sys
+import pkg_resources
+from docopt import docopt
+from PySide2.QtWidgets import QApplication
+from tinymovr.gui import MainWindow, app_stylesheet
+from tinymovr.constants import app_name
+
+
+"""
+Tinymovr Studio GUI
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+The graphical user interface of Tinymovr Studio
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+# https://www.loekvandenouweland.com/content/pyside2-big-sur-does-not-show-window.html
+import os
+os.environ['QT_MAC_WANTS_LAYER'] = '1'
+
+def spawn():
+    version = pkg_resources.require("tinymovr")[0].version
+    arguments = docopt(__doc__, version=app_name + " " + str(version))
+    app = QApplication(sys.argv)
+    app.setStyleSheet(app_stylesheet)
+    w = MainWindow(app, arguments)
+    w.show()
+    sys.exit(app.exec_())
```

### Comparing `tinymovr-1.2.5/tinymovr/gui/helpers.py` & `tinymovr-1.2.7/tinymovr/gui/helpers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,338 +1,338 @@
-"""
-Tinymovr GUI Helpers
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-Various GUI helper functions
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import time
-import os
-import enum
-import pint
-from PySide2 import QtGui, QtCore
-from PySide2.QtWidgets import QMessageBox, QFileDialog
-from avlos.definitions import RemoteAttribute
-
-
-app_stylesheet = """
-
-/* --------------------------------------- QPushButton -----------------------------------*/
-
-    QPushButton {
-        background-color: #ededef;
-        border-radius: 4px; 
-        margin: 0 0 1px 0;
-    }
-    QPushButton:pressed {
-        background-color: #cdcdcf;
-        border-style: inset;
-    }
-    QPushButton:hover:!pressed
-    {
-    background-color: #eaeaec;
-    }
-
-/* --------------------------------------- QScrollBar -----------------------------------*/
-
-    QScrollBar:horizontal
-    {
-        height: 15px;
-        margin: 3px 15px 3px 15px;
-        border: 1px transparent white;
-        border-radius: 4px;
-        background-color: white;
-    }
-
-    QScrollBar::handle:horizontal
-    {
-        background-color: #dfdfe1;      /* #605F5F; */
-        min-width: 5px;
-        border-radius: 4px;
-    }
-
-    QScrollBar::add-line:horizontal
-    {
-        margin: 0px 3px 0px 3px;
-        border-image: url(:/qss_icons/rc/right_arrow_disabled.png);
-        width: 10px;
-        height: 10px;
-        subcontrol-position: right;
-        subcontrol-origin: margin;
-    }
-
-    QScrollBar::sub-line:horizontal
-    {
-        margin: 0px 3px 0px 3px;
-        border-image: url(:/qss_icons/rc/left_arrow_disabled.png);
-        height: 10px;
-        width: 10px;
-        subcontrol-position: left;
-        subcontrol-origin: margin;
-    }
-
-    QScrollBar::add-line:horizontal:hover,QScrollBar::add-line:horizontal:on
-    {
-        border-image: url(:/qss_icons/rc/right_arrow.png);
-        height: 10px;
-        width: 10px;
-        subcontrol-position: right;
-        subcontrol-origin: margin;
-    }
-
-
-    QScrollBar::sub-line:horizontal:hover, QScrollBar::sub-line:horizontal:on
-    {
-        border-image: url(:/qss_icons/rc/left_arrow.png);
-        height: 10px;
-        width: 10px;
-        subcontrol-position: left;
-        subcontrol-origin: margin;
-    }
-
-    QScrollBar::up-arrow:horizontal, QScrollBar::down-arrow:horizontal
-    {
-        background: none;
-    }
-
-
-    QScrollBar::add-page:horizontal, QScrollBar::sub-page:horizontal
-    {
-        background: none;
-    }
-
-    QScrollBar:vertical
-    {
-        background-color: white;
-        width: 15px;
-        margin: 15px 3px 15px 3px;
-        border: 1px transparent white;
-        border-radius: 4px;
-    }
-
-    QScrollBar::handle:vertical
-    {
-        background-color: #dfdfe1;
-        min-height: 5px;
-        border-radius: 4px;
-    }
-
-    QScrollBar::sub-line:vertical
-    {
-        margin: 3px 0px 3px 0px;
-        border-image: url(:/qss_icons/rc/up_arrow_disabled.png);
-        height: 10px;
-        width: 10px;
-        subcontrol-position: top;
-        subcontrol-origin: margin;
-    }
-
-    QScrollBar::add-line:vertical
-    {
-        margin: 3px 0px 3px 0px;
-        border-image: url(:/qss_icons/rc/down_arrow_disabled.png);
-        height: 10px;
-        width: 10px;
-        subcontrol-position: bottom;
-        subcontrol-origin: margin;
-    }
-
-    QScrollBar::sub-line:vertical:hover,QScrollBar::sub-line:vertical:on
-    {
-        border-image: url(:/qss_icons/rc/up_arrow.png);
-        height: 10px;
-        width: 10px;
-        subcontrol-position: top;
-        subcontrol-origin: margin;
-    }
-
-    QScrollBar::add-line:vertical:hover, QScrollBar::add-line:vertical:on
-    {
-        border-image: url(:/qss_icons/rc/down_arrow.png);
-        height: 10px;
-        width: 10px;
-        subcontrol-position: bottom;
-        subcontrol-origin: margin;
-    }
-
-    QScrollBar::up-arrow:vertical, QScrollBar::down-arrow:vertical
-    {
-        background: none;
-    }
-
-    QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical
-    {
-        background: none;
-    }
-"""
-
-
-def format_value(value, include_unit=True):
-    """
-    Format a numeric value according to its
-    type and return the formatted string
-    """
-    if isinstance(value, enum.IntFlag):
-        return str(value) if value > 0 else "(no flags)"
-    if not include_unit and isinstance(value, pint.Quantity):
-        return str(value.magnitude)
-    if isinstance(value, float):
-        return "{0:.6g}".format(value)
-    return str(value)
-
-
-def load_icon(fname_icon):
-    """
-    Load an image from a file and return it
-    as a QIcon
-    """
-    path_this_dir = os.path.dirname(os.path.abspath(__file__))
-    path_icons = os.path.join(path_this_dir, "..", "..", "resources", "icons")
-    path_icon = os.path.join(path_icons, fname_icon)
-    pixmap = QtGui.QPixmap(path_icon)
-    icon = QtGui.QIcon()
-    icon.addPixmap(pixmap, QtGui.QIcon.Normal)
-    icon.addPixmap(pixmap, QtGui.QIcon.Disabled)
-    return icon
-
-
-def magnitude_of(val):
-    """
-    Extract the magnitude of a pint Quantity
-    and return it, or return the value itself
-    otherwise
-    """
-    if isinstance(val, pint.Quantity):
-        return val.magnitude
-    return val
-
-
-def hold_sema(sema):
-    sema.acquire()
-    try:
-        yield
-    finally:
-        sema.release()
-
-
-class TimedGetter:
-    """
-    An interface class that maintains timing
-    information for the getter function
-    """
-
-    def __init__(self, error_handler):
-        self.error_handler = error_handler
-        self.dt = 0
-
-    def get_value(self, getter):
-        try:
-            get_start_time = time.time()
-            val = getter()
-            get_dt = time.time() - get_start_time
-            self.dt = self.dt * 0.99 + get_dt * 0.01
-            return val
-        except Exception as e:
-            self.error_handler(e)
-
-
-class RateLimitedFunction:
-    """
-    A class that limits the rate of calls to a passed
-    function f
-    """
-
-    def __init__(self, func, rate):
-        self.func = func
-        self.rate = rate
-        self.busy_dt = 0
-        self.meas_dt = 0
-        self.load = 0
-        self.stop = False
-
-    def call(self, *args, **kwargs):
-        if self.busy_dt > 0 and self.busy_dt < self.rate:
-            self.load = self.load * 0.99 + self.busy_dt / self.rate * 0.01
-            time.sleep(self.rate - self.busy_dt)
-            self.meas_dt = self.rate
-        else:
-            self.load = 1
-            self.meas_dt = self.busy_dt
-        start_time = time.time()
-        self.func()
-        self.busy_dt = time.time() - start_time
-
-    def __call__(self, *args, **kwargs):
-        self.call(self, *args, **kwargs)
-
-
-def display_warning(title, text):
-    """
-    Display a pop up message with a warning
-    """
-    msg_box = QMessageBox()
-    msg_box.setIcon(QMessageBox.Warning)
-    msg_box.setText(text)
-    msg_box.setWindowTitle(title)
-    msg_box.exec_()
-
-
-def display_file_open_dialog():
-    """
-    Display the file open dialog
-    """
-    documents_dir = os.path.expanduser("~/Documents")
-    file_name, _ = QFileDialog.getOpenFileName(
-        None, "Select JSON File", "", "JSON Files (*.json)"
-    )
-    return file_name
-
-
-def display_file_save_dialog():
-    """
-    Display the file save dialog
-    """
-    documents_dir = os.path.expanduser("~/Documents")
-    file_name, _ = QFileDialog.getSaveFileName(
-        None, "Save JSON File", documents_dir, "JSON Files (*.json)"
-    )
-    return file_name
-
-
-def check_selected_items(selected_items):
-    if len(selected_items) == 0:
-        display_warning(
-            "Invalid Selection",
-            "No Tinymovr nodes selected.\nSelect a single node",
-        )
-        return False
-    elif len(selected_items) > 1:
-        display_warning(
-            "Invalid Selection",
-            "Multiple Tinymovr nodes selected.\nSelect a single node",
-        )
-        return False
-    return True
-
-
-def get_dynamic_attrs(attr_dict):
-    """
-    Get the attributes that are marked as dynamic in the spec.
-    """
-    dynamic_attrs = []
-    for _, attr in attr_dict.items():
-        if isinstance(attr, RemoteAttribute):
-            if "dynamic" in attr.meta and attr.meta["dynamic"] == True:
-                dynamic_attrs.append(attr)
-        elif hasattr(attr, "remote_attributes"):
-            dynamic_attrs.extend(get_dynamic_attrs(attr.remote_attributes))
-    return dynamic_attrs
+"""
+Tinymovr GUI Helpers
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+Various GUI helper functions
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import time
+import os
+import enum
+import pint
+from PySide2 import QtGui, QtCore
+from PySide2.QtWidgets import QMessageBox, QFileDialog
+from avlos.definitions import RemoteAttribute
+
+
+app_stylesheet = """
+
+/* --------------------------------------- QPushButton -----------------------------------*/
+
+    QPushButton {
+        background-color: #ededef;
+        border-radius: 4px; 
+        margin: 0 0 1px 0;
+    }
+    QPushButton:pressed {
+        background-color: #cdcdcf;
+        border-style: inset;
+    }
+    QPushButton:hover:!pressed
+    {
+    background-color: #eaeaec;
+    }
+
+/* --------------------------------------- QScrollBar -----------------------------------*/
+
+    QScrollBar:horizontal
+    {
+        height: 15px;
+        margin: 3px 15px 3px 15px;
+        border: 1px transparent white;
+        border-radius: 4px;
+        background-color: white;
+    }
+
+    QScrollBar::handle:horizontal
+    {
+        background-color: #dfdfe1;      /* #605F5F; */
+        min-width: 5px;
+        border-radius: 4px;
+    }
+
+    QScrollBar::add-line:horizontal
+    {
+        margin: 0px 3px 0px 3px;
+        border-image: url(:/qss_icons/rc/right_arrow_disabled.png);
+        width: 10px;
+        height: 10px;
+        subcontrol-position: right;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::sub-line:horizontal
+    {
+        margin: 0px 3px 0px 3px;
+        border-image: url(:/qss_icons/rc/left_arrow_disabled.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: left;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::add-line:horizontal:hover,QScrollBar::add-line:horizontal:on
+    {
+        border-image: url(:/qss_icons/rc/right_arrow.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: right;
+        subcontrol-origin: margin;
+    }
+
+
+    QScrollBar::sub-line:horizontal:hover, QScrollBar::sub-line:horizontal:on
+    {
+        border-image: url(:/qss_icons/rc/left_arrow.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: left;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::up-arrow:horizontal, QScrollBar::down-arrow:horizontal
+    {
+        background: none;
+    }
+
+
+    QScrollBar::add-page:horizontal, QScrollBar::sub-page:horizontal
+    {
+        background: none;
+    }
+
+    QScrollBar:vertical
+    {
+        background-color: white;
+        width: 15px;
+        margin: 15px 3px 15px 3px;
+        border: 1px transparent white;
+        border-radius: 4px;
+    }
+
+    QScrollBar::handle:vertical
+    {
+        background-color: #dfdfe1;
+        min-height: 5px;
+        border-radius: 4px;
+    }
+
+    QScrollBar::sub-line:vertical
+    {
+        margin: 3px 0px 3px 0px;
+        border-image: url(:/qss_icons/rc/up_arrow_disabled.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: top;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::add-line:vertical
+    {
+        margin: 3px 0px 3px 0px;
+        border-image: url(:/qss_icons/rc/down_arrow_disabled.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: bottom;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::sub-line:vertical:hover,QScrollBar::sub-line:vertical:on
+    {
+        border-image: url(:/qss_icons/rc/up_arrow.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: top;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::add-line:vertical:hover, QScrollBar::add-line:vertical:on
+    {
+        border-image: url(:/qss_icons/rc/down_arrow.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: bottom;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::up-arrow:vertical, QScrollBar::down-arrow:vertical
+    {
+        background: none;
+    }
+
+    QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical
+    {
+        background: none;
+    }
+"""
+
+
+def format_value(value, include_unit=True):
+    """
+    Format a numeric value according to its
+    type and return the formatted string
+    """
+    if isinstance(value, enum.IntFlag):
+        return str(value) if value > 0 else "(no flags)"
+    if not include_unit and isinstance(value, pint.Quantity):
+        return str(value.magnitude)
+    if isinstance(value, float):
+        return "{0:.6g}".format(value)
+    return str(value)
+
+
+def load_icon(fname_icon):
+    """
+    Load an image from a file and return it
+    as a QIcon
+    """
+    path_this_dir = os.path.dirname(os.path.abspath(__file__))
+    path_icons = os.path.join(path_this_dir, "..", "..", "resources", "icons")
+    path_icon = os.path.join(path_icons, fname_icon)
+    pixmap = QtGui.QPixmap(path_icon)
+    icon = QtGui.QIcon()
+    icon.addPixmap(pixmap, QtGui.QIcon.Normal)
+    icon.addPixmap(pixmap, QtGui.QIcon.Disabled)
+    return icon
+
+
+def magnitude_of(val):
+    """
+    Extract the magnitude of a pint Quantity
+    and return it, or return the value itself
+    otherwise
+    """
+    if isinstance(val, pint.Quantity):
+        return val.magnitude
+    return val
+
+
+def hold_sema(sema):
+    sema.acquire()
+    try:
+        yield
+    finally:
+        sema.release()
+
+
+class TimedGetter:
+    """
+    An interface class that maintains timing
+    information for the getter function
+    """
+
+    def __init__(self, error_handler):
+        self.error_handler = error_handler
+        self.dt = 0
+
+    def get_value(self, getter):
+        try:
+            get_start_time = time.time()
+            val = getter()
+            get_dt = time.time() - get_start_time
+            self.dt = self.dt * 0.99 + get_dt * 0.01
+            return val
+        except Exception as e:
+            self.error_handler(e)
+
+
+class RateLimitedFunction:
+    """
+    A class that limits the rate of calls to a passed
+    function f
+    """
+
+    def __init__(self, func, rate):
+        self.func = func
+        self.rate = rate
+        self.busy_dt = 0
+        self.meas_dt = 0
+        self.load = 0
+        self.stop = False
+
+    def call(self, *args, **kwargs):
+        if self.busy_dt > 0 and self.busy_dt < self.rate:
+            self.load = self.load * 0.99 + self.busy_dt / self.rate * 0.01
+            time.sleep(self.rate - self.busy_dt)
+            self.meas_dt = self.rate
+        else:
+            self.load = 1
+            self.meas_dt = self.busy_dt
+        start_time = time.time()
+        self.func()
+        self.busy_dt = time.time() - start_time
+
+    def __call__(self, *args, **kwargs):
+        self.call(self, *args, **kwargs)
+
+
+def display_warning(title, text):
+    """
+    Display a pop up message with a warning
+    """
+    msg_box = QMessageBox()
+    msg_box.setIcon(QMessageBox.Warning)
+    msg_box.setText(text)
+    msg_box.setWindowTitle(title)
+    msg_box.exec_()
+
+
+def display_file_open_dialog():
+    """
+    Display the file open dialog
+    """
+    documents_dir = os.path.expanduser("~/Documents")
+    file_name, _ = QFileDialog.getOpenFileName(
+        None, "Select JSON File", "", "JSON Files (*.json)"
+    )
+    return file_name
+
+
+def display_file_save_dialog():
+    """
+    Display the file save dialog
+    """
+    documents_dir = os.path.expanduser("~/Documents")
+    file_name, _ = QFileDialog.getSaveFileName(
+        None, "Save JSON File", documents_dir, "JSON Files (*.json)"
+    )
+    return file_name
+
+
+def check_selected_items(selected_items):
+    if len(selected_items) == 0:
+        display_warning(
+            "Invalid Selection",
+            "No Tinymovr nodes selected.\nSelect a single node",
+        )
+        return False
+    elif len(selected_items) > 1:
+        display_warning(
+            "Invalid Selection",
+            "Multiple Tinymovr nodes selected.\nSelect a single node",
+        )
+        return False
+    return True
+
+
+def get_dynamic_attrs(attr_dict):
+    """
+    Get the attributes that are marked as dynamic in the spec.
+    """
+    dynamic_attrs = []
+    for _, attr in attr_dict.items():
+        if isinstance(attr, RemoteAttribute):
+            if "dynamic" in attr.meta and attr.meta["dynamic"] == True:
+                dynamic_attrs.append(attr)
+        elif hasattr(attr, "remote_attributes"):
+            dynamic_attrs.extend(get_dynamic_attrs(attr.remote_attributes))
+    return dynamic_attrs
```

### Comparing `tinymovr-1.2.5/tinymovr/gui/worker.py` & `tinymovr-1.2.7/tinymovr/gui/worker.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-"""
-Tinymovr GUI Worker
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-The GUI Worker class, subclass of QObject, that handles
-updates and IO, running in a separate thread
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import time
-import can
-from canine import CANineBus
-from PySide2 import QtCore
-from PySide2.QtCore import QObject
-from PySide2.QtWidgets import (
-    QApplication,
-)
-from tinymovr.gui import TimedGetter, RateLimitedFunction, get_dynamic_attrs
-from tinymovr.tee import init_tee, destroy_tee
-from tinymovr.discovery import Discovery
-from tinymovr.constants import base_node_name
-
-
-class Worker(QObject):
-
-    update_attrs = QtCore.Signal(dict)
-    regen = QtCore.Signal(dict)
-    handle_error = QtCore.Signal(object)
-
-    def __init__(self, busparams, logger):
-        super().__init__()
-        self.logger = logger
-        self.mutx = QtCore.QMutex()
-        init_tee(can.Bus(**busparams))
-        self._init_containers()
-        self.dsc = Discovery(self._node_appeared, self._node_disappeared, self.logger)
-        self.timed_getter = TimedGetter(lambda e: self.handle_error.emit(e))
-        self._rate_limited_update = RateLimitedFunction(lambda: self._update(), 0.040)
-        self.running = True
-
-    def run(self):
-        while self.running:
-            self._rate_limited_update()  # calls update()
-        destroy_tee()
-
-    @QtCore.Slot()
-    def stop(self):
-        self.running = False
-
-    def force_regen(self):
-        self.mutx.lock()
-        self.regen.emit(dict(self.tms_by_id))
-        self.mutx.unlock()
-
-    def reset(self):
-        self.mutx.lock()
-        self.dsc.reset()
-        self._init_containers()
-        self.regen.emit(dict(self.tms_by_id))
-        self.mutx.unlock()
-
-    @QtCore.Slot(dict)
-    def update_active_attrs(self, d):
-        if d["checked"] == True:
-            self.active_attrs.add(d["attr"])
-        else:
-            self.active_attrs.discard(d["attr"])
-
-    def _get_attr_values(self):
-        vals = {}
-        for attr in self.active_attrs:
-            vals[attr.full_name] = self.timed_getter.get_value(attr.get_value)
-        start_time = time.time()
-        self.dynamic_attrs.sort(
-            key=lambda attr: self.dynamic_attrs_last_update[attr.full_name]
-            if attr.full_name in self.dynamic_attrs_last_update
-            else 0
-        )
-        for attr in self.dynamic_attrs:
-            t = (
-                self.dynamic_attrs_last_update[attr.full_name]
-                if attr.full_name in self.dynamic_attrs_last_update
-                else 0
-            )
-            if (attr.full_name not in vals) and (start_time - t > 0.5):
-                vals[attr.full_name] = self.timed_getter.get_value(attr.get_value)
-                self.dynamic_attrs_last_update[attr.full_name] = start_time
-                break
-        return vals
-
-    def _init_containers(self):
-        self.active_attrs = set()
-        self.dynamic_attrs = []
-        self.tms_by_id = {}
-        self.dynamic_attrs_last_update = {}
-
-    def _update(self):
-        self.mutx.lock()
-        last_updated = self._get_attr_values()
-        if len(last_updated) > 0:
-            self.update_attrs.emit(last_updated)
-        self.mutx.unlock()
-        QApplication.processEvents()
-
-    def _node_appeared(self, node, name):
-        self.mutx.lock()
-        node_name = "{}{}".format(base_node_name, name)
-        self.tms_by_id[node_name] = node
-        node.name = node_name
-        node.include_base_name = True
-        self.dynamic_attrs = get_dynamic_attrs(self.tms_by_id)
-        self.regen.emit(dict(self.tms_by_id))
-        self.mutx.unlock()
-
-    def _node_disappeared(self, name):
-        self.mutx.lock()
-        node_name = "{}{}".format(base_node_name, name)
-        del self.tms_by_id[node_name]
-        self.dynamic_attrs = get_dynamic_attrs(self.tms_by_id)
-        self.regen.emit(dict(self.tms_by_id))
-        self.mutx.unlock()
+"""
+Tinymovr GUI Worker
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+The GUI Worker class, subclass of QObject, that handles
+updates and IO, running in a separate thread
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import time
+import can
+from canine import CANineBus
+from PySide2 import QtCore
+from PySide2.QtCore import QObject
+from PySide2.QtWidgets import (
+    QApplication,
+)
+from tinymovr.gui import TimedGetter, RateLimitedFunction, get_dynamic_attrs
+from tinymovr.tee import init_tee, destroy_tee
+from tinymovr.discovery import Discovery
+from tinymovr.constants import base_node_name
+
+
+class Worker(QObject):
+
+    update_attrs = QtCore.Signal(dict)
+    regen = QtCore.Signal(dict)
+    handle_error = QtCore.Signal(object)
+
+    def __init__(self, busparams, logger):
+        super().__init__()
+        self.logger = logger
+        self.mutx = QtCore.QMutex()
+        init_tee(can.Bus(**busparams))
+        self._init_containers()
+        self.dsc = Discovery(self._node_appeared, self._node_disappeared, self.logger)
+        self.timed_getter = TimedGetter(lambda e: self.handle_error.emit(e))
+        self._rate_limited_update = RateLimitedFunction(lambda: self._update(), 0.040)
+        self.running = True
+
+    def run(self):
+        while self.running:
+            self._rate_limited_update()  # calls update()
+        destroy_tee()
+
+    @QtCore.Slot()
+    def stop(self):
+        self.running = False
+
+    def force_regen(self):
+        self.mutx.lock()
+        self.regen.emit(dict(self.tms_by_id))
+        self.mutx.unlock()
+
+    def reset(self):
+        self.mutx.lock()
+        self.dsc.reset()
+        self._init_containers()
+        self.regen.emit(dict(self.tms_by_id))
+        self.mutx.unlock()
+
+    @QtCore.Slot(dict)
+    def update_active_attrs(self, d):
+        if d["checked"] == True:
+            self.active_attrs.add(d["attr"])
+        else:
+            self.active_attrs.discard(d["attr"])
+
+    def _get_attr_values(self):
+        vals = {}
+        for attr in self.active_attrs:
+            vals[attr.full_name] = self.timed_getter.get_value(attr.get_value)
+        start_time = time.time()
+        self.dynamic_attrs.sort(
+            key=lambda attr: self.dynamic_attrs_last_update[attr.full_name]
+            if attr.full_name in self.dynamic_attrs_last_update
+            else 0
+        )
+        for attr in self.dynamic_attrs:
+            t = (
+                self.dynamic_attrs_last_update[attr.full_name]
+                if attr.full_name in self.dynamic_attrs_last_update
+                else 0
+            )
+            if (attr.full_name not in vals) and (start_time - t > 0.5):
+                vals[attr.full_name] = self.timed_getter.get_value(attr.get_value)
+                self.dynamic_attrs_last_update[attr.full_name] = start_time
+                break
+        return vals
+
+    def _init_containers(self):
+        self.active_attrs = set()
+        self.dynamic_attrs = []
+        self.tms_by_id = {}
+        self.dynamic_attrs_last_update = {}
+
+    def _update(self):
+        self.mutx.lock()
+        last_updated = self._get_attr_values()
+        if len(last_updated) > 0:
+            self.update_attrs.emit(last_updated)
+        self.mutx.unlock()
+        QApplication.processEvents()
+
+    def _node_appeared(self, node, name):
+        self.mutx.lock()
+        node_name = "{}{}".format(base_node_name, name)
+        self.tms_by_id[node_name] = node
+        node.name = node_name
+        node.include_base_name = True
+        self.dynamic_attrs = get_dynamic_attrs(self.tms_by_id)
+        self.regen.emit(dict(self.tms_by_id))
+        self.mutx.unlock()
+
+    def _node_disappeared(self, name):
+        self.mutx.lock()
+        node_name = "{}{}".format(base_node_name, name)
+        del self.tms_by_id[node_name]
+        self.dynamic_attrs = get_dynamic_attrs(self.tms_by_id)
+        self.regen.emit(dict(self.tms_by_id))
+        self.mutx.unlock()
```

### Comparing `tinymovr-1.2.5/tinymovr/tee.py` & `tinymovr-1.2.7/tinymovr/tee.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-"""
-Tinymovr Tee Module
-Copyright Ioannis Chatzikonstantinou 2020-2023
-
-Implements a Tee class to distribute incoming traffic according to rules
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-This program is distributed in the hope that it will be useful, but WITHOUT
-ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <http://www.gnu.org/licenses/>.
-"""
-
-
-import time
-from enum import Enum
-from threading import Thread, Lock
-
-
-tee = None
-
-
-class Client:
-    def __init__(self, filter_cb, recv_cb):
-        self.filter_cb = filter_cb
-        self.recv_cb = recv_cb
-
-
-class TeeState(Enum):
-    INIT = 0
-    RUNNING = 1
-    STOPPING = 2
-    STOPPED = 3
-
-
-class Tee:
-    """
-    Distribute incoming messages based on the boolean result
-    of a filter callback.
-
-    python-can does not allow filtering messages per recipient therefore
-    this class.
-
-    Also implements a simple forwarding mechanism for sending messages, to
-    simplify interfacing with CAN bus objects.
-    """
-
-    def __init__(self, bus, timeout):
-        self.bus = bus
-        self.timeout = timeout
-        self.clients = []
-        self.state = TeeState.INIT
-        self.update_thread = Thread(target=self.update, daemon=True)
-        self.update_thread.start()
-
-    def add(self, filter_cb, recv_cb):
-        self.clients.append(Client(filter_cb, recv_cb))
-
-    def update(self):
-        """ """
-        self.state = TeeState.RUNNING
-        while TeeState.RUNNING == self.state:
-            self._update_once()
-        assert TeeState.STOPPING == self.state
-        self.state = TeeState.STOPPED
-
-    def _update_once(self):
-        """
-        Tries to receive a message from the bus object and if successful,
-        tests reception of each tee instance in the global index.
-        """
-        frame = self.bus.recv(timeout=self.timeout)
-        if frame:
-            for client in self.clients:
-                if client.filter_cb(frame):
-                    client.recv_cb(frame)
-
-    def send(self, frame):
-        """
-        Send a frame by forwarding to the bus object
-        """
-        self.bus.send(frame)
-
-    def stop(self):
-        self.state = TeeState.STOPPING
-        while TeeState.STOPPING == self.state:
-            time.sleep(0.01)
-        assert TeeState.STOPPED == self.state
-
-
-def init_tee(bus, timeout=0.1):
-    """
-    Initializes a tee using a python-can bus instance
-    """
-    global tee
-    assert None == tee
-    tee = Tee(bus, timeout)
-
-
-def destroy_tee():
-    """
-    Destroys the existing tee, stopping its thread.
-    """
-    global tee
-    assert None != tee
-    tee.stop()
-    tee = None
-
-
-def get_tee():
-    """
-    Get the current tee object
-    """
-    return tee
+"""
+Tinymovr Tee Module
+Copyright Ioannis Chatzikonstantinou 2020-2023
+
+Implements a Tee class to distribute incoming traffic according to rules
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
+"""
+
+
+import time
+from enum import Enum
+from threading import Thread, Lock
+
+
+tee = None
+
+
+class Client:
+    def __init__(self, filter_cb, recv_cb):
+        self.filter_cb = filter_cb
+        self.recv_cb = recv_cb
+
+
+class TeeState(Enum):
+    INIT = 0
+    RUNNING = 1
+    STOPPING = 2
+    STOPPED = 3
+
+
+class Tee:
+    """
+    Distribute incoming messages based on the boolean result
+    of a filter callback.
+
+    python-can does not allow filtering messages per recipient therefore
+    this class.
+
+    Also implements a simple forwarding mechanism for sending messages, to
+    simplify interfacing with CAN bus objects.
+    """
+
+    def __init__(self, bus, timeout):
+        self.bus = bus
+        self.timeout = timeout
+        self.clients = []
+        self.state = TeeState.INIT
+        self.update_thread = Thread(target=self.update, daemon=True)
+        self.update_thread.start()
+
+    def add(self, filter_cb, recv_cb):
+        self.clients.append(Client(filter_cb, recv_cb))
+
+    def update(self):
+        """ """
+        self.state = TeeState.RUNNING
+        while TeeState.RUNNING == self.state:
+            self._update_once()
+        assert TeeState.STOPPING == self.state
+        self.state = TeeState.STOPPED
+
+    def _update_once(self):
+        """
+        Tries to receive a message from the bus object and if successful,
+        tests reception of each tee instance in the global index.
+        """
+        frame = self.bus.recv(timeout=self.timeout)
+        if frame:
+            for client in self.clients:
+                if client.filter_cb(frame):
+                    client.recv_cb(frame)
+
+    def send(self, frame):
+        """
+        Send a frame by forwarding to the bus object
+        """
+        self.bus.send(frame)
+
+    def stop(self):
+        self.state = TeeState.STOPPING
+        while TeeState.STOPPING == self.state:
+            time.sleep(0.01)
+        assert TeeState.STOPPED == self.state
+
+
+def init_tee(bus, timeout=0.1):
+    """
+    Initializes a tee using a python-can bus instance
+    """
+    global tee
+    assert None == tee
+    tee = Tee(bus, timeout)
+
+
+def destroy_tee():
+    """
+    Destroys the existing tee, stopping its thread.
+    """
+    global tee
+    assert None != tee
+    tee.stop()
+    tee = None
+
+
+def get_tee():
+    """
+    Get the current tee object
+    """
+    return tee
```

### Comparing `tinymovr-1.2.5/tinymovr.egg-info/PKG-INFO` & `tinymovr-1.2.7/tinymovr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,60 @@
-Metadata-Version: 2.1
-Name: tinymovr
-Version: 1.2.5
-Summary: Tinymovr Studio
-Home-page: https://github.com/yconst/Tinymovr
-Author: Yannis Chatzikonstantinou
-Author-email: info@tinymovr.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: gui
-
-![Studio Lint Test](https://github.com/yconst/tinymovr/workflows/Tinymovr%20Studio%20Lint%2FTest/badge.svg)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-## Tinymovr Studio Python
-
-This is the Python client library and application that allows easy interfacing with the Tinymovr motor control board.
-
-### Installing using pip
-
-This is the most straightforward method to install Tinymovr studio and have access to hardware. We use pip3 to ensure Tinymovr is installed using Python 3 (required).
-
-    pip3 install tinymovr
-
-### Installing using git clone
-
-First clone the Tinymovr repo to a local directory:
-
-    git clone https://github.com/yconst/Tinymovr
-
-Then cd to the cloned repo directory and install in developer mode:
-
-    cd Tinymovr/studio/Python
-    pip3 install -e .
-
-### Launching the GUI app
-
-    tinymovr
-
-### Launching the command line app
-
-    tinymovr_cli
-
-## Getting Help
-
-[Full documentation is available at Readthedocs](https://tinymovr.readthedocs.io).
-
-Please visit the [Discussions Page](https://github.com/tinymovr/Tinymovr/discussions) and the [Discord Server](https://discord.gg/vNvmpfthug) to ask any questions. If you are unable to find an answer to your question, you are welcome to [start a new discussion](https://github.com/tinymovr/Tinymovr/discussions/new/choose) or ask away at [our Discord server](https://discord.gg/vNvmpfthug).
-
-If you would like to propose a feature or think you have found a bug, [open a new issue](https://github.com/tinymovr/Tinymovr/issues/new).
-
-### More information
-
-[Website and Store](https://tinymovr.com)
-
-[Documentation](https://tinymovr.readthedocs.io)
-
-
-
+Metadata-Version: 2.1
+Name: tinymovr
+Version: 1.2.7
+Summary: Tinymovr Studio
+Home-page: https://github.com/yconst/Tinymovr
+Author: Yannis Chatzikonstantinou
+Author-email: info@tinymovr.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: gui
+
+![Studio Lint Test](https://github.com/yconst/tinymovr/workflows/Tinymovr%20Studio%20Lint%2FTest/badge.svg)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+## Tinymovr Studio Python
+
+This is the Python client library and application that allows easy interfacing with the Tinymovr motor control board.
+
+### Installing using pip
+
+This is the most straightforward method to install Tinymovr studio and have access to hardware. We use pip3 to ensure Tinymovr is installed using Python 3 (required).
+
+    pip3 install tinymovr
+
+### Installing using git clone
+
+First clone the Tinymovr repo to a local directory:
+
+    git clone https://github.com/yconst/Tinymovr
+
+Then cd to the cloned repo directory and install in developer mode:
+
+    cd Tinymovr/studio/Python
+    pip3 install -e .
+
+### Launching the GUI app
+
+    tinymovr
+
+### Launching the command line app
+
+    tinymovr_cli
+
+## Getting Help
+
+[Full documentation is available at Readthedocs](https://tinymovr.readthedocs.io).
+
+Please visit the [Discussions Page](https://github.com/tinymovr/Tinymovr/discussions) and the [Discord Server](https://discord.gg/vNvmpfthug) to ask any questions. If you are unable to find an answer to your question, you are welcome to [start a new discussion](https://github.com/tinymovr/Tinymovr/discussions/new/choose) or ask away at [our Discord server](https://discord.gg/vNvmpfthug).
+
+If you would like to propose a feature or think you have found a bug, [open a new issue](https://github.com/tinymovr/Tinymovr/issues/new).
+
+### More information
+
+[Website and Store](https://tinymovr.com)
+
+[Documentation](https://tinymovr.readthedocs.io)
+
```

### Comparing `tinymovr-1.2.5/tinymovr.egg-info/SOURCES.txt` & `tinymovr-1.2.7/tinymovr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

