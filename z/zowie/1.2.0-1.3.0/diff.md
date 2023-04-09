# Comparing `tmp/zowie-1.2.0.tar.gz` & `tmp/zowie-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zowie-1.2.0.tar", last modified: Sun Oct 24 20:45:31 2021, max compression
+gzip compressed data, was "zowie-1.3.0.tar", last modified: Sun Apr  9 22:31:39 2023, max compression
```

## Comparing `zowie-1.2.0.tar` & `zowie-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2021-10-24 20:45:31.147053 zowie-1.2.0/
--rw-r--r--   0 mhucka     (511) staff       (20)     1622 2021-10-23 16:36:18.000000 zowie-1.2.0/LICENSE
--rw-r--r--   0 mhucka     (511) staff       (20)    31646 2021-10-24 20:45:31.147358 zowie-1.2.0/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)    30913 2021-10-24 20:42:28.000000 zowie-1.2.0/README.md
--rw-r--r--   0 mhucka     (511) staff       (20)      878 2021-10-24 20:45:31.148082 zowie-1.2.0/setup.cfg
--rw-r--r--   0 mhucka     (511) staff       (20)      809 2021-10-11 03:59:03.000000 zowie-1.2.0/setup.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2021-10-24 20:45:31.141924 zowie-1.2.0/zowie/
--rw-r--r--   0 mhucka     (511) staff       (20)     1503 2021-10-24 20:20:28.000000 zowie-1.2.0/zowie/__init__.py
--rw-r--r--   0 mhucka     (511) staff       (20)    15487 2021-10-23 16:36:18.000000 zowie-1.2.0/zowie/__main__.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1639 2021-10-11 03:59:03.000000 zowie-1.2.0/zowie/exceptions.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1458 2021-10-11 03:59:03.000000 zowie-1.2.0/zowie/exit_codes.py
--rw-r--r--   0 mhucka     (511) staff       (20)     4056 2021-10-11 03:59:03.000000 zowie-1.2.0/zowie/keyring_utils.py
--rw-r--r--   0 mhucka     (511) staff       (20)     8652 2021-10-23 16:36:18.000000 zowie-1.2.0/zowie/main_body.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2021-10-24 20:45:31.146709 zowie-1.2.0/zowie/methods/
--rw-r--r--   0 mhucka     (511) staff       (20)     1148 2021-10-23 16:36:18.000000 zowie-1.2.0/zowie/methods/__init__.py
--rw-r--r--   0 mhucka     (511) staff       (20)     2696 2021-10-23 16:36:18.000000 zowie-1.2.0/zowie/methods/base.py
--rw-r--r--   0 mhucka     (511) staff       (20)     5162 2021-10-23 16:36:18.000000 zowie-1.2.0/zowie/methods/findercomment.py
--rw-r--r--   0 mhucka     (511) staff       (20)     3694 2021-10-11 03:59:03.000000 zowie-1.2.0/zowie/methods/pdfproducer.py
--rw-r--r--   0 mhucka     (511) staff       (20)     3560 2021-10-11 03:59:03.000000 zowie-1.2.0/zowie/methods/pdfsubject.py
--rw-r--r--   0 mhucka     (511) staff       (20)     6702 2021-10-19 12:19:40.000000 zowie-1.2.0/zowie/methods/wherefrom.py
--rw-r--r--   0 mhucka     (511) staff       (20)     8751 2021-10-23 16:36:18.000000 zowie-1.2.0/zowie/zotero.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2021-10-24 20:45:31.144310 zowie-1.2.0/zowie.egg-info/
--rw-r--r--   0 mhucka     (511) staff       (20)    31646 2021-10-24 20:45:31.000000 zowie-1.2.0/zowie.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)      537 2021-10-24 20:45:31.000000 zowie-1.2.0/zowie.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2021-10-24 20:45:31.000000 zowie-1.2.0/zowie.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (511) staff       (20)       63 2021-10-24 20:45:31.000000 zowie-1.2.0/zowie.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2021-10-24 20:45:31.000000 zowie-1.2.0/zowie.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (511) staff       (20)      318 2021-10-24 20:45:31.000000 zowie-1.2.0/zowie.egg-info/requires.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        6 2021-10-24 20:45:31.000000 zowie-1.2.0/zowie.egg-info/top_level.txt
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 22:31:39.554838 zowie-1.3.0/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1622 2023-04-09 21:50:21.000000 zowie-1.3.0/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    30642 2023-04-09 22:31:39.554921 zowie-1.3.0/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    29916 2023-04-09 21:50:21.000000 zowie-1.3.0/README.md
+-rw-r--r--   0 mhucka     (503) staff       (20)      891 2023-04-09 22:31:39.555193 zowie-1.3.0/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1627 2023-04-09 21:50:21.000000 zowie-1.3.0/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 22:31:39.551507 zowie-1.3.0/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)      411 2021-11-16 03:02:37.000000 zowie-1.3.0/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      378 2021-11-16 03:02:37.000000 zowie-1.3.0/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      606 2021-11-16 03:02:37.000000 zowie-1.3.0/tests/test_keyring_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 22:31:39.552730 zowie-1.3.0/zowie/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1503 2023-04-09 22:30:55.000000 zowie-1.3.0/zowie/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15487 2023-04-09 21:58:40.000000 zowie-1.3.0/zowie/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1639 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4056 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/keyring_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     8655 2023-04-09 22:14:19.000000 zowie-1.3.0/zowie/main_body.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 22:31:39.554734 zowie-1.3.0/zowie/methods/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1148 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/methods/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2696 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/methods/base.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5162 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/methods/findercomment.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3694 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/methods/pdfproducer.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3560 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/methods/pdfsubject.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6702 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/methods/wherefrom.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     8751 2021-11-16 03:02:37.000000 zowie-1.3.0/zowie/zotero.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 22:31:39.553938 zowie-1.3.0/zowie.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    30642 2023-04-09 22:31:39.000000 zowie-1.3.0/zowie.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      615 2023-04-09 22:31:39.000000 zowie-1.3.0/zowie.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-09 22:31:39.000000 zowie-1.3.0/zowie.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       62 2023-04-09 22:31:39.000000 zowie-1.3.0/zowie.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-09 22:31:39.000000 zowie-1.3.0/zowie.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      319 2023-04-09 22:31:39.000000 zowie-1.3.0/zowie.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        6 2023-04-09 22:31:39.000000 zowie-1.3.0/zowie.egg-info/top_level.txt
```

### Comparing `zowie-1.2.0/LICENSE` & `zowie-1.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-2021 by Michael Hucka and the California Institute of
+Copyright (c) 2020-2023 by Michael Hucka and the California Institute of
 Technology (Pasadena, California, USA).  All rights not granted herein
 are expressly reserved by the copyright holders.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
```

### Comparing `zowie-1.2.0/PKG-INFO` & `zowie-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: zowie
-Version: 1.2.0
+Version: 1.3.0
 Summary: Write Zotero select links into article attachment files
 Home-page: https://github.com/mhucka/zowie
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause
 Project-URL: Source Code, https://github.com/mhucka/zowie
 Project-URL: Bug Tracker, https://github.com/mhucka/zowie/issues
 Keywords: Python,utilities
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Zowie<img width="10%" align="right" src="https://github.com/mhucka/zowie/raw/main/.graphics/zowie-icon.png">
 
 Zowie ("**Zo**tero link **w**r**i**t**e**r") is a command-line program for macOS that writes Zotero _select_ links into the file attachments contained in a Zotero database.
 
 [![License](https://img.shields.io/badge/License-BSD-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.6+-brightgreen.svg?style=flat-square)](http://shields.io)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/2154)](https://data.caltech.edu/records/2154)
 [![GitHub stars](https://img.shields.io/github/stars/mhucka/zowie.svg?style=flat-square&color=lightgray&label=Stars)](https://github.com/mhucka/zowie/stargazers)
 [![Latest release](https://img.shields.io/github/v/release/mhucka/zowie.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/mhucka/zowie/releases)
 [![PyPI](https://img.shields.io/pypi/v/zowie.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/zowie/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Known issues and limitations](#known-issues-and-limitations)
+* [Additional tips](#additional-tips)
 * [Getting help](#getting-help)
 * [Contributing](#contributing)
 * [License](#license)
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
@@ -50,77 +49,53 @@
 Enter Zowie (a loose acronym for _"**Zo**tero link **w**r**i**t**e**r"_, and pronounced like [the interjection](https://www.merriam-webster.com/dictionary/zowie)).  Zowie scans through the files on your disk in a local Zotero database, looks up the Zotero bibliographic record corresponding to each file found, and writes a [Zotero select link](https://forums.zotero.org/discussion/78053/given-the-pdf-file-of-an-article-how-can-you-find-out-its-uri#latest) into the file and/or certain macOS Finder/Spotlight metadata fields (depending on the user's choice).  A Zotero select link has the form `zotero://select/...` and when opened on macOS, causes the Zotero desktop application to open that item in your database.  Zowie thus makes it possible to go from a file opened in an application other than Zotero (e.g., DEVONthink, Adobe Acrobat), to the Zotero record corresponding to that file.
 
 Regretfully, Zowie can **only** work with Zotero libraries that use normal/local data storage; **it cannot work when Zotero is configured to use linked attachments**.
 
 
 ## Installation
 
-There are multiple ways of installing Zowie, ranging from downloading a self-contained, single-file, ready-to-run application, to installing it as a typical Python program using `pip`.  Please choose the alternative that suits you.
+There are multiple ways of installing Zowie, ranging from downloading a self-contained, single-file, ready-to-run program, to installing it as a typical Python program using `pip`.  Please choose the alternative that suits you and your Mac environment.
 
 
-### _Alternative 1: downloading the ready-to-run application_
+### _Alternative 1: downloading the ready-to-run program_
 
-Depending on the version of macOS you are using, please see the relevant section below.
-
-<details><summary><img alt="macOS 10.15 and later" align="top" height="26px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/mac-os-32.png">&nbsp;<strong>macOS version 10.15 (Catalina) or later</strong></summary>
-
-First, you need a Python interpreter version 3.8 or higher on your computer. Happily, that's the version provided by macOS 10.15 and later, but if you have never run `python3` on your computer, then the first time you do, macOS will ask if you want to install certain additional software components. (Let it do so.) Check the version of the program `python3` that you get by running the following command in a terminal and inspecting the results:
+On macOS Catalina (10.15) or later, you can use a ready-to-run version of Zowie that only needs a Python interpreter version 3.8 or higher on your computer. That's the case for macOS 10.15 and later, but before you can use it, you may need to let macOS install some additional software components from Apple. To test it, run the following command in a terminal and **take note of the version of Python** that it prints:
 ```sh
 python3 --version
 ```
-
-Next, go to the [GitHub page for the latest Zowie release](https://github.com/mhucka/zowie/releases) and:
-1. Find a ZIP file with a name that contains your version of Python
-2. Click on that ZIP file to download it
-3. Unzip the file (if your browser did not automatically unzip it for you)
-4. Open the folder thus created (it will have a name like `zowie-1.2.0-macos-python3.8`)
-5. Look inside for `zowie` and move it to a location where you put other command-line programs (such as `/usr/local/bin`). 
-
-If you want to put it in `/usr/local/bin` but that folder does not exist on your computer yet, you can create it by opening a terminal window and running the following command (_prior_ to moving `zowie` into `/usr/local/bin`):
-
-```shell
-sudo mkdir /usr/local/bin
+**If this is the first time** you've run `python3` on your system, macOS will either ask you if you want to install certain additional software components, or it may produce an error about 
+`xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools) ...`. In either case, the solution is to run the following command in the terminal:
 ```
-
-The following is an example command that you can type in a terminal to move Zowie there:
-
-```shell
-sudo mv zowie /usr/local/bin
+xcode-select --install
 ```
+In the pop-up dialog box that this brings up, **click the _Install_ button** and agree to let it install the [Command Line Tools](https://developer.apple.com/library/archive/technotes/tn2339/_index.html) package from Apple.
 
-</details>
-<p> </p>
-<details><summary><img alt="macOS before 10.15" align="top" height="26px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/mac-os-32.png">&nbsp;<strong>macOS 10.14 (Mojave) and earlier</strong></summary>
-
-A runnable version of Zowie created using a different method is available for macOS before 10.15, for which Apple did not provide Python version 3. This copy of Zowie works like any normal command-line program and does **not** require Python.  (However, it **does not run on macOS Catalina or later** due to Apple security issues.)
-
-1. Go to the page on GitHub for [the latest release](https://github.com/mhucka/zowie/releases/latest).
-2.  <img align="right" width="400px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/binary-release.png"/>Find the **Assets** section of the latest release.
-3. Click on `zowie.zip` to download it.
-4. Unzip the file; this will leave you with a file named `zowie`, which is the program itself.
-5. Move `zowie` to a folder where you put other command-line programs (e.g. `/usr/local/bin`). 
+Next,
+1. <img align="right" width="350px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/shiv-releases.png"/>Go to the [latest release on GitHub](https://github.com/mhucka/zowie/releases) and find the **Assets**
+2. **Download** the ZIP file whose name contains the version of Python on your computer (which you determined by running `python3 --version` above)
+3. **Unzip** the file (if your browser didn't unzip it)
+4. **Open the folder** that gets created (it will have a name like `zowie-1.2.0-macos-python3.8`)
+5. Look inside for `zowie` and **move it** to a location where you put other command-line programs (such as `/usr/local/bin`). 
 
 If you want to put it in `/usr/local/bin` but that folder does not exist on your computer yet, you can create it by opening a terminal window and running the following command (_prior_ to moving `zowie` into `/usr/local/bin`):
 
 ```shell
 sudo mkdir /usr/local/bin
 ```
 
 The following is an example command that you can type in a terminal to move Zowie there:
 
 ```shell
 sudo mv zowie /usr/local/bin
 ```
 
-</details>
-
 
 ### _Alternative 2: installing Zowie using `pipx`_
 
-You can use [pipx](https://pypa.github.io/pipx/) to install Zowie. Pipx will install it into a separate Python environment that isolates the dependencies needed by Zowie from other Python programs on your system, and yet the resulting `zowie` command wil be executable from any shell &ndash; like any normal application on your computer. If you do not already have `pipx` on your system, it can be installed in a variety of easy ways and it is best to consult [Pipx's installation guide](https://pypa.github.io/pipx/installation/) for instructions. Once you have pipx on your system, you can install Zowie with the following command:
+You can use [pipx](https://pypa.github.io/pipx/) to install Zowie. Pipx will install it into a separate Python environment that isolates the dependencies needed by Zowie from other Python programs on your system, and yet the resulting `zowie` command wil be executable from any shell &ndash; like any normal program on your computer. If you do not already have `pipx` on your system, it can be installed in a variety of easy ways and it is best to consult [Pipx's installation guide](https://pypa.github.io/pipx/installation/) for instructions. Once you have pipx on your system, you can install Zowie with the following command:
 ```sh
 pipx install zowie
 ```
 
 Pipx can also let you run Zowie directly using `pipx run zowie`, although in that case, you must always prefix every Zowie command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
 
 
@@ -323,27 +298,32 @@
 * If you use [DEVONthink](https://www.devontechnologies.com/apps/devonthink) in a scheme in which you index your Zotero folder and use Zowie to write the Zotero select link into the Finder comments of files, beware of the following situation. If you use a DEVONthink smart rule to copy the comment string into the "URL" field, DEVONthink will (after reindexing the file) suddenly display an _empty_ Finder comment, even though the comment is still there. This is due to a [deliberate behavior in DEVONthink](https://discourse.devontechnologies.com/t/some-finder-comments-not-showing-in-devonthink/66864/30) and not a problem with Zowie, as discussed in the [section on special-case behavior](#special-case-behavior). Using the `-s` option will avoid this, but at the cost of adding an extra character to the Finder comment, so make sure to account for the added space character in any scripts or other actions you take on the Finder comment.
 
 * [DEVONthink](https://www.devontechnologies.com/apps/devonthink) bases the "URL" value of a file on the file's [`com.apple.metadata:kMDItemWhereFroms`](https://developer.apple.com/documentation/coreservices/kmditemwherefroms) extended attribute.  The original hope behind Zowie was to make it write Zotero select links directly into that attribute value. Unfortunately, it turns out that if a file has already been indexed by DEVONthink, then [it will _not_ detect any changes to the `com.apple.metadata:kMDItemWhereFroms` attribute](https://discourse.devontechnologies.com/t/some-finder-comments-not-showing-in-devonthink/66864/38) made by an external program. Thus, if you index your Zotero folder within DEVONthink, you cannot use Zowie's `wherefroms` method to update the "URL" field directly. You are advised instead to use Zowie's `findercomment` method (the default) in combination with smart rules in DEVONthink, as discussed in [the wiki](https://github.com/mhucka/zowie/wiki/Example:-using-Zowie-with-DEVONthink). I share your frustration.
 
 * For reasons I have not had time to investigate, the binary version of `zowie` takes a very long time to start up on macOS 10.15 (Catalina) and 11.1 (Big Sur).  On my test system inside a virtual machine running on a fast iMac, it takes 10 seconds or more before the first output from `zowie` appears.
 
 
+## Additional tips
+
+In the [wiki associated with the Zowie project in GitHub](https://github.com/mhucka/zowie/wiki), I have started writing some notes about how I personally use Zowie to combine Zotero with DEVONthink.
+
+
 ## Getting help
 
 If you find an issue, please submit it in [the GitHub issue tracker](https://github.com/mhucka/zowie/issues) for this repository.
 
 
 ## Contributing
 
 I would be happy to receive your help and participation if you are interested.  Everyone is asked to read and respect the [code of conduct](CONDUCT.md) when participating in this project.  Development generally takes place on the `development` branch.
 
 
 ## License
 
-This software is Copyright (C) 2020-2021, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
+This software is Copyright (C) 2020&ndash;2023, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
 
 
 ## Acknowledgments
 
 This work is a personal project developed by the author, using computing facilities and other resources of the [California Institute of Technology Library](https://www.library.caltech.edu).
 
 The [vector artwork](https://thenounproject.com/term/tag-exclamation-point/326951/) of an exclamation point circled by a zigzag, used as the icon for this repository, was created by  [Alfredo @ IconsAlfredo.com](https://thenounproject.com/AlfredoCreates/) from the Noun Project.  It is licensed under the Creative Commons [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/) license.
@@ -367,9 +347,7 @@
 * [pyzotero](https://github.com/urschrei/pyzotero) &ndash; a Python API client for Zotero
 * [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
 * [Shiv](https://github.com/linkedin/shiv) &ndash; command-line utility for creating self-contained Python zipapps
 * [Sidetrack](https://github.com/caltechlibrary/sidetrack) &ndash; simple debug logging/tracing package
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 The [developers of DEVONthink](https://www.devontechnologies.com/about), especially Jim Neumann and Christian Grunenberg, quickly and consistently replied to my many questions on the [DEVONtechnologies forums](https://discourse.devontechnologies.com).
-
-
```

### Comparing `zowie-1.2.0/README.md` & `zowie-1.3.0/zowie.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,45 @@
+Metadata-Version: 2.1
+Name: zowie
+Version: 1.3.0
+Summary: Write Zotero select links into article attachment files
+Home-page: https://github.com/mhucka/zowie
+Author: Michael Hucka
+Author-email: mhucka@caltech.edu
+License: BSD 3-clause
+Project-URL: Source Code, https://github.com/mhucka/zowie
+Project-URL: Bug Tracker, https://github.com/mhucka/zowie/issues
+Keywords: Python,utilities
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Zowie<img width="10%" align="right" src="https://github.com/mhucka/zowie/raw/main/.graphics/zowie-icon.png">
 
 Zowie ("**Zo**tero link **w**r**i**t**e**r") is a command-line program for macOS that writes Zotero _select_ links into the file attachments contained in a Zotero database.
 
 [![License](https://img.shields.io/badge/License-BSD-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.6+-brightgreen.svg?style=flat-square)](http://shields.io)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/2154)](https://data.caltech.edu/records/2154)
 [![GitHub stars](https://img.shields.io/github/stars/mhucka/zowie.svg?style=flat-square&color=lightgray&label=Stars)](https://github.com/mhucka/zowie/stargazers)
 [![Latest release](https://img.shields.io/github/v/release/mhucka/zowie.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/mhucka/zowie/releases)
 [![PyPI](https://img.shields.io/pypi/v/zowie.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/zowie/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Known issues and limitations](#known-issues-and-limitations)
+* [Additional tips](#additional-tips)
 * [Getting help](#getting-help)
 * [Contributing](#contributing)
 * [License](#license)
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
@@ -29,77 +49,53 @@
 Enter Zowie (a loose acronym for _"**Zo**tero link **w**r**i**t**e**r"_, and pronounced like [the interjection](https://www.merriam-webster.com/dictionary/zowie)).  Zowie scans through the files on your disk in a local Zotero database, looks up the Zotero bibliographic record corresponding to each file found, and writes a [Zotero select link](https://forums.zotero.org/discussion/78053/given-the-pdf-file-of-an-article-how-can-you-find-out-its-uri#latest) into the file and/or certain macOS Finder/Spotlight metadata fields (depending on the user's choice).  A Zotero select link has the form `zotero://select/...` and when opened on macOS, causes the Zotero desktop application to open that item in your database.  Zowie thus makes it possible to go from a file opened in an application other than Zotero (e.g., DEVONthink, Adobe Acrobat), to the Zotero record corresponding to that file.
 
 Regretfully, Zowie can **only** work with Zotero libraries that use normal/local data storage; **it cannot work when Zotero is configured to use linked attachments**.
 
 
 ## Installation
 
-There are multiple ways of installing Zowie, ranging from downloading a self-contained, single-file, ready-to-run application, to installing it as a typical Python program using `pip`.  Please choose the alternative that suits you.
-
-
-### _Alternative 1: downloading the ready-to-run application_
+There are multiple ways of installing Zowie, ranging from downloading a self-contained, single-file, ready-to-run program, to installing it as a typical Python program using `pip`.  Please choose the alternative that suits you and your Mac environment.
 
-Depending on the version of macOS you are using, please see the relevant section below.
 
-<details><summary><img alt="macOS 10.15 and later" align="top" height="26px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/mac-os-32.png">&nbsp;<strong>macOS version 10.15 (Catalina) or later</strong></summary>
+### _Alternative 1: downloading the ready-to-run program_
 
-First, you need a Python interpreter version 3.8 or higher on your computer. Happily, that's the version provided by macOS 10.15 and later, but if you have never run `python3` on your computer, then the first time you do, macOS will ask if you want to install certain additional software components. (Let it do so.) Check the version of the program `python3` that you get by running the following command in a terminal and inspecting the results:
+On macOS Catalina (10.15) or later, you can use a ready-to-run version of Zowie that only needs a Python interpreter version 3.8 or higher on your computer. That's the case for macOS 10.15 and later, but before you can use it, you may need to let macOS install some additional software components from Apple. To test it, run the following command in a terminal and **take note of the version of Python** that it prints:
 ```sh
 python3 --version
 ```
-
-Next, go to the [GitHub page for the latest Zowie release](https://github.com/mhucka/zowie/releases) and:
-1. Find a ZIP file with a name that contains your version of Python
-2. Click on that ZIP file to download it
-3. Unzip the file (if your browser did not automatically unzip it for you)
-4. Open the folder thus created (it will have a name like `zowie-1.2.0-macos-python3.8`)
-5. Look inside for `zowie` and move it to a location where you put other command-line programs (such as `/usr/local/bin`). 
-
-If you want to put it in `/usr/local/bin` but that folder does not exist on your computer yet, you can create it by opening a terminal window and running the following command (_prior_ to moving `zowie` into `/usr/local/bin`):
-
-```shell
-sudo mkdir /usr/local/bin
+**If this is the first time** you've run `python3` on your system, macOS will either ask you if you want to install certain additional software components, or it may produce an error about 
+`xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools) ...`. In either case, the solution is to run the following command in the terminal:
 ```
-
-The following is an example command that you can type in a terminal to move Zowie there:
-
-```shell
-sudo mv zowie /usr/local/bin
+xcode-select --install
 ```
+In the pop-up dialog box that this brings up, **click the _Install_ button** and agree to let it install the [Command Line Tools](https://developer.apple.com/library/archive/technotes/tn2339/_index.html) package from Apple.
 
-</details>
-<p> </p>
-<details><summary><img alt="macOS before 10.15" align="top" height="26px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/mac-os-32.png">&nbsp;<strong>macOS 10.14 (Mojave) and earlier</strong></summary>
-
-A runnable version of Zowie created using a different method is available for macOS before 10.15, for which Apple did not provide Python version 3. This copy of Zowie works like any normal command-line program and does **not** require Python.  (However, it **does not run on macOS Catalina or later** due to Apple security issues.)
-
-1. Go to the page on GitHub for [the latest release](https://github.com/mhucka/zowie/releases/latest).
-2.  <img align="right" width="400px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/binary-release.png"/>Find the **Assets** section of the latest release.
-3. Click on `zowie.zip` to download it.
-4. Unzip the file; this will leave you with a file named `zowie`, which is the program itself.
-5. Move `zowie` to a folder where you put other command-line programs (e.g. `/usr/local/bin`). 
+Next,
+1. <img align="right" width="350px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/shiv-releases.png"/>Go to the [latest release on GitHub](https://github.com/mhucka/zowie/releases) and find the **Assets**
+2. **Download** the ZIP file whose name contains the version of Python on your computer (which you determined by running `python3 --version` above)
+3. **Unzip** the file (if your browser didn't unzip it)
+4. **Open the folder** that gets created (it will have a name like `zowie-1.2.0-macos-python3.8`)
+5. Look inside for `zowie` and **move it** to a location where you put other command-line programs (such as `/usr/local/bin`). 
 
 If you want to put it in `/usr/local/bin` but that folder does not exist on your computer yet, you can create it by opening a terminal window and running the following command (_prior_ to moving `zowie` into `/usr/local/bin`):
 
 ```shell
 sudo mkdir /usr/local/bin
 ```
 
 The following is an example command that you can type in a terminal to move Zowie there:
 
 ```shell
 sudo mv zowie /usr/local/bin
 ```
 
-</details>
-
 
 ### _Alternative 2: installing Zowie using `pipx`_
 
-You can use [pipx](https://pypa.github.io/pipx/) to install Zowie. Pipx will install it into a separate Python environment that isolates the dependencies needed by Zowie from other Python programs on your system, and yet the resulting `zowie` command wil be executable from any shell &ndash; like any normal application on your computer. If you do not already have `pipx` on your system, it can be installed in a variety of easy ways and it is best to consult [Pipx's installation guide](https://pypa.github.io/pipx/installation/) for instructions. Once you have pipx on your system, you can install Zowie with the following command:
+You can use [pipx](https://pypa.github.io/pipx/) to install Zowie. Pipx will install it into a separate Python environment that isolates the dependencies needed by Zowie from other Python programs on your system, and yet the resulting `zowie` command wil be executable from any shell &ndash; like any normal program on your computer. If you do not already have `pipx` on your system, it can be installed in a variety of easy ways and it is best to consult [Pipx's installation guide](https://pypa.github.io/pipx/installation/) for instructions. Once you have pipx on your system, you can install Zowie with the following command:
 ```sh
 pipx install zowie
 ```
 
 Pipx can also let you run Zowie directly using `pipx run zowie`, although in that case, you must always prefix every Zowie command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
 
 
@@ -302,27 +298,32 @@
 * If you use [DEVONthink](https://www.devontechnologies.com/apps/devonthink) in a scheme in which you index your Zotero folder and use Zowie to write the Zotero select link into the Finder comments of files, beware of the following situation. If you use a DEVONthink smart rule to copy the comment string into the "URL" field, DEVONthink will (after reindexing the file) suddenly display an _empty_ Finder comment, even though the comment is still there. This is due to a [deliberate behavior in DEVONthink](https://discourse.devontechnologies.com/t/some-finder-comments-not-showing-in-devonthink/66864/30) and not a problem with Zowie, as discussed in the [section on special-case behavior](#special-case-behavior). Using the `-s` option will avoid this, but at the cost of adding an extra character to the Finder comment, so make sure to account for the added space character in any scripts or other actions you take on the Finder comment.
 
 * [DEVONthink](https://www.devontechnologies.com/apps/devonthink) bases the "URL" value of a file on the file's [`com.apple.metadata:kMDItemWhereFroms`](https://developer.apple.com/documentation/coreservices/kmditemwherefroms) extended attribute.  The original hope behind Zowie was to make it write Zotero select links directly into that attribute value. Unfortunately, it turns out that if a file has already been indexed by DEVONthink, then [it will _not_ detect any changes to the `com.apple.metadata:kMDItemWhereFroms` attribute](https://discourse.devontechnologies.com/t/some-finder-comments-not-showing-in-devonthink/66864/38) made by an external program. Thus, if you index your Zotero folder within DEVONthink, you cannot use Zowie's `wherefroms` method to update the "URL" field directly. You are advised instead to use Zowie's `findercomment` method (the default) in combination with smart rules in DEVONthink, as discussed in [the wiki](https://github.com/mhucka/zowie/wiki/Example:-using-Zowie-with-DEVONthink). I share your frustration.
 
 * For reasons I have not had time to investigate, the binary version of `zowie` takes a very long time to start up on macOS 10.15 (Catalina) and 11.1 (Big Sur).  On my test system inside a virtual machine running on a fast iMac, it takes 10 seconds or more before the first output from `zowie` appears.
 
 
+## Additional tips
+
+In the [wiki associated with the Zowie project in GitHub](https://github.com/mhucka/zowie/wiki), I have started writing some notes about how I personally use Zowie to combine Zotero with DEVONthink.
+
+
 ## Getting help
 
 If you find an issue, please submit it in [the GitHub issue tracker](https://github.com/mhucka/zowie/issues) for this repository.
 
 
 ## Contributing
 
 I would be happy to receive your help and participation if you are interested.  Everyone is asked to read and respect the [code of conduct](CONDUCT.md) when participating in this project.  Development generally takes place on the `development` branch.
 
 
 ## License
 
-This software is Copyright (C) 2020-2021, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
+This software is Copyright (C) 2020&ndash;2023, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
 
 
 ## Acknowledgments
 
 This work is a personal project developed by the author, using computing facilities and other resources of the [California Institute of Technology Library](https://www.library.caltech.edu).
 
 The [vector artwork](https://thenounproject.com/term/tag-exclamation-point/326951/) of an exclamation point circled by a zigzag, used as the icon for this repository, was created by  [Alfredo @ IconsAlfredo.com](https://thenounproject.com/AlfredoCreates/) from the Noun Project.  It is licensed under the Creative Commons [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/) license.
```

### Comparing `zowie-1.2.0/setup.cfg` & `zowie-1.3.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [metadata]
 name = zowie
-version = 1.2.0
+version = 1.3.0
 description = Write Zotero select links into article attachment files
 author = Michael Hucka
 author_email = mhucka@caltech.edu
 license = BSD 3-clause
 license_files = LICENSE
 url = https://github.com/mhucka/zowie
 project_urls = 
 	Source Code = https://github.com/mhucka/zowie
 	Bug Tracker = https://github.com/mhucka/zowie/issues
 keywords = Python, utilities
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: BSD License
 	Intended Audience :: Science/Research
 	Operating System :: MacOS :: MacOS X
-	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.8
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 zip_safe = False
-python_requires = >= 3.6
+python_requires = >= 3.8
 
 [options.entry_points]
 console_scripts = 
 	zowie = zowie.__main__:console_scripts_main
 
 [egg_info]
 tag_build =
```

### Comparing `zowie-1.2.0/zowie/__init__.py` & `zowie-1.3.0/zowie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Package metadata ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '1.2.0'
+__version__     = '1.3.0'
 __description__ = 'Write Zotero select links into article attachment files'
 __url__         = 'https://github.com/mhucka/zowie'
 __author__      = 'Michael Hucka'
 __email__       = 'mhucka@caltech.edu'
 __license__     = 'BSD 3-clause'
```

### Comparing `zowie-1.2.0/zowie/__main__.py` & `zowie-1.3.0/zowie/__main__.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/exceptions.py` & `zowie-1.3.0/zowie/exceptions.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/exit_codes.py` & `zowie-1.3.0/zowie/exit_codes.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/keyring_utils.py` & `zowie-1.3.0/zowie/keyring_utils.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/main_body.py` & `zowie-1.3.0/zowie/main_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             self._targets.append(file)
         if __debug__: log(f'gathered {pluralized("file", self._targets, True)}')
 
         if self.after_date:
             if __debug__: log(f'filtering files by date {self.after_date_str}')
             kept = []
             tzinfo = self.after_date.tzinfo
-            for file in self.files:
+            for file in self._targets:
                 mtime = datetime.fromtimestamp(Path(file).stat().st_mtime)
                 if mtime.replace(tzinfo = tzinfo) >= self.after_date:
                     if __debug__: log(f'keeping {file}')
                     kept.append(file)
             self._targets = kept
 
         if not self._targets:
```

### Comparing `zowie-1.2.0/zowie/methods/__init__.py` & `zowie-1.3.0/zowie/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/methods/base.py` & `zowie-1.3.0/zowie/methods/base.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/methods/findercomment.py` & `zowie-1.3.0/zowie/methods/findercomment.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/methods/pdfproducer.py` & `zowie-1.3.0/zowie/methods/pdfproducer.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/methods/pdfsubject.py` & `zowie-1.3.0/zowie/methods/pdfsubject.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/methods/wherefrom.py` & `zowie-1.3.0/zowie/methods/wherefrom.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie/zotero.py` & `zowie-1.3.0/zowie/zotero.py`

 * *Files identical despite different names*

### Comparing `zowie-1.2.0/zowie.egg-info/PKG-INFO` & `zowie-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,25 @@
-Metadata-Version: 2.1
-Name: zowie
-Version: 1.2.0
-Summary: Write Zotero select links into article attachment files
-Home-page: https://github.com/mhucka/zowie
-Author: Michael Hucka
-Author-email: mhucka@caltech.edu
-License: BSD 3-clause
-Project-URL: Source Code, https://github.com/mhucka/zowie
-Project-URL: Bug Tracker, https://github.com/mhucka/zowie/issues
-Keywords: Python,utilities
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Zowie<img width="10%" align="right" src="https://github.com/mhucka/zowie/raw/main/.graphics/zowie-icon.png">
 
 Zowie ("**Zo**tero link **w**r**i**t**e**r") is a command-line program for macOS that writes Zotero _select_ links into the file attachments contained in a Zotero database.
 
 [![License](https://img.shields.io/badge/License-BSD-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.6+-brightgreen.svg?style=flat-square)](http://shields.io)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/2154)](https://data.caltech.edu/records/2154)
 [![GitHub stars](https://img.shields.io/github/stars/mhucka/zowie.svg?style=flat-square&color=lightgray&label=Stars)](https://github.com/mhucka/zowie/stargazers)
 [![Latest release](https://img.shields.io/github/v/release/mhucka/zowie.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/mhucka/zowie/releases)
 [![PyPI](https://img.shields.io/pypi/v/zowie.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/zowie/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Known issues and limitations](#known-issues-and-limitations)
+* [Additional tips](#additional-tips)
 * [Getting help](#getting-help)
 * [Contributing](#contributing)
 * [License](#license)
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
@@ -50,77 +29,53 @@
 Enter Zowie (a loose acronym for _"**Zo**tero link **w**r**i**t**e**r"_, and pronounced like [the interjection](https://www.merriam-webster.com/dictionary/zowie)).  Zowie scans through the files on your disk in a local Zotero database, looks up the Zotero bibliographic record corresponding to each file found, and writes a [Zotero select link](https://forums.zotero.org/discussion/78053/given-the-pdf-file-of-an-article-how-can-you-find-out-its-uri#latest) into the file and/or certain macOS Finder/Spotlight metadata fields (depending on the user's choice).  A Zotero select link has the form `zotero://select/...` and when opened on macOS, causes the Zotero desktop application to open that item in your database.  Zowie thus makes it possible to go from a file opened in an application other than Zotero (e.g., DEVONthink, Adobe Acrobat), to the Zotero record corresponding to that file.
 
 Regretfully, Zowie can **only** work with Zotero libraries that use normal/local data storage; **it cannot work when Zotero is configured to use linked attachments**.
 
 
 ## Installation
 
-There are multiple ways of installing Zowie, ranging from downloading a self-contained, single-file, ready-to-run application, to installing it as a typical Python program using `pip`.  Please choose the alternative that suits you.
-
-
-### _Alternative 1: downloading the ready-to-run application_
+There are multiple ways of installing Zowie, ranging from downloading a self-contained, single-file, ready-to-run program, to installing it as a typical Python program using `pip`.  Please choose the alternative that suits you and your Mac environment.
 
-Depending on the version of macOS you are using, please see the relevant section below.
 
-<details><summary><img alt="macOS 10.15 and later" align="top" height="26px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/mac-os-32.png">&nbsp;<strong>macOS version 10.15 (Catalina) or later</strong></summary>
+### _Alternative 1: downloading the ready-to-run program_
 
-First, you need a Python interpreter version 3.8 or higher on your computer. Happily, that's the version provided by macOS 10.15 and later, but if you have never run `python3` on your computer, then the first time you do, macOS will ask if you want to install certain additional software components. (Let it do so.) Check the version of the program `python3` that you get by running the following command in a terminal and inspecting the results:
+On macOS Catalina (10.15) or later, you can use a ready-to-run version of Zowie that only needs a Python interpreter version 3.8 or higher on your computer. That's the case for macOS 10.15 and later, but before you can use it, you may need to let macOS install some additional software components from Apple. To test it, run the following command in a terminal and **take note of the version of Python** that it prints:
 ```sh
 python3 --version
 ```
-
-Next, go to the [GitHub page for the latest Zowie release](https://github.com/mhucka/zowie/releases) and:
-1. Find a ZIP file with a name that contains your version of Python
-2. Click on that ZIP file to download it
-3. Unzip the file (if your browser did not automatically unzip it for you)
-4. Open the folder thus created (it will have a name like `zowie-1.2.0-macos-python3.8`)
-5. Look inside for `zowie` and move it to a location where you put other command-line programs (such as `/usr/local/bin`). 
-
-If you want to put it in `/usr/local/bin` but that folder does not exist on your computer yet, you can create it by opening a terminal window and running the following command (_prior_ to moving `zowie` into `/usr/local/bin`):
-
-```shell
-sudo mkdir /usr/local/bin
+**If this is the first time** you've run `python3` on your system, macOS will either ask you if you want to install certain additional software components, or it may produce an error about 
+`xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools) ...`. In either case, the solution is to run the following command in the terminal:
 ```
-
-The following is an example command that you can type in a terminal to move Zowie there:
-
-```shell
-sudo mv zowie /usr/local/bin
+xcode-select --install
 ```
+In the pop-up dialog box that this brings up, **click the _Install_ button** and agree to let it install the [Command Line Tools](https://developer.apple.com/library/archive/technotes/tn2339/_index.html) package from Apple.
 
-</details>
-<p> </p>
-<details><summary><img alt="macOS before 10.15" align="top" height="26px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/mac-os-32.png">&nbsp;<strong>macOS 10.14 (Mojave) and earlier</strong></summary>
-
-A runnable version of Zowie created using a different method is available for macOS before 10.15, for which Apple did not provide Python version 3. This copy of Zowie works like any normal command-line program and does **not** require Python.  (However, it **does not run on macOS Catalina or later** due to Apple security issues.)
-
-1. Go to the page on GitHub for [the latest release](https://github.com/mhucka/zowie/releases/latest).
-2.  <img align="right" width="400px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/binary-release.png"/>Find the **Assets** section of the latest release.
-3. Click on `zowie.zip` to download it.
-4. Unzip the file; this will leave you with a file named `zowie`, which is the program itself.
-5. Move `zowie` to a folder where you put other command-line programs (e.g. `/usr/local/bin`). 
+Next,
+1. <img align="right" width="350px" src="https://github.com/mhucka/zowie/raw/develop/.graphics/shiv-releases.png"/>Go to the [latest release on GitHub](https://github.com/mhucka/zowie/releases) and find the **Assets**
+2. **Download** the ZIP file whose name contains the version of Python on your computer (which you determined by running `python3 --version` above)
+3. **Unzip** the file (if your browser didn't unzip it)
+4. **Open the folder** that gets created (it will have a name like `zowie-1.2.0-macos-python3.8`)
+5. Look inside for `zowie` and **move it** to a location where you put other command-line programs (such as `/usr/local/bin`). 
 
 If you want to put it in `/usr/local/bin` but that folder does not exist on your computer yet, you can create it by opening a terminal window and running the following command (_prior_ to moving `zowie` into `/usr/local/bin`):
 
 ```shell
 sudo mkdir /usr/local/bin
 ```
 
 The following is an example command that you can type in a terminal to move Zowie there:
 
 ```shell
 sudo mv zowie /usr/local/bin
 ```
 
-</details>
-
 
 ### _Alternative 2: installing Zowie using `pipx`_
 
-You can use [pipx](https://pypa.github.io/pipx/) to install Zowie. Pipx will install it into a separate Python environment that isolates the dependencies needed by Zowie from other Python programs on your system, and yet the resulting `zowie` command wil be executable from any shell &ndash; like any normal application on your computer. If you do not already have `pipx` on your system, it can be installed in a variety of easy ways and it is best to consult [Pipx's installation guide](https://pypa.github.io/pipx/installation/) for instructions. Once you have pipx on your system, you can install Zowie with the following command:
+You can use [pipx](https://pypa.github.io/pipx/) to install Zowie. Pipx will install it into a separate Python environment that isolates the dependencies needed by Zowie from other Python programs on your system, and yet the resulting `zowie` command wil be executable from any shell &ndash; like any normal program on your computer. If you do not already have `pipx` on your system, it can be installed in a variety of easy ways and it is best to consult [Pipx's installation guide](https://pypa.github.io/pipx/installation/) for instructions. Once you have pipx on your system, you can install Zowie with the following command:
 ```sh
 pipx install zowie
 ```
 
 Pipx can also let you run Zowie directly using `pipx run zowie`, although in that case, you must always prefix every Zowie command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
 
 
@@ -323,27 +278,32 @@
 * If you use [DEVONthink](https://www.devontechnologies.com/apps/devonthink) in a scheme in which you index your Zotero folder and use Zowie to write the Zotero select link into the Finder comments of files, beware of the following situation. If you use a DEVONthink smart rule to copy the comment string into the "URL" field, DEVONthink will (after reindexing the file) suddenly display an _empty_ Finder comment, even though the comment is still there. This is due to a [deliberate behavior in DEVONthink](https://discourse.devontechnologies.com/t/some-finder-comments-not-showing-in-devonthink/66864/30) and not a problem with Zowie, as discussed in the [section on special-case behavior](#special-case-behavior). Using the `-s` option will avoid this, but at the cost of adding an extra character to the Finder comment, so make sure to account for the added space character in any scripts or other actions you take on the Finder comment.
 
 * [DEVONthink](https://www.devontechnologies.com/apps/devonthink) bases the "URL" value of a file on the file's [`com.apple.metadata:kMDItemWhereFroms`](https://developer.apple.com/documentation/coreservices/kmditemwherefroms) extended attribute.  The original hope behind Zowie was to make it write Zotero select links directly into that attribute value. Unfortunately, it turns out that if a file has already been indexed by DEVONthink, then [it will _not_ detect any changes to the `com.apple.metadata:kMDItemWhereFroms` attribute](https://discourse.devontechnologies.com/t/some-finder-comments-not-showing-in-devonthink/66864/38) made by an external program. Thus, if you index your Zotero folder within DEVONthink, you cannot use Zowie's `wherefroms` method to update the "URL" field directly. You are advised instead to use Zowie's `findercomment` method (the default) in combination with smart rules in DEVONthink, as discussed in [the wiki](https://github.com/mhucka/zowie/wiki/Example:-using-Zowie-with-DEVONthink). I share your frustration.
 
 * For reasons I have not had time to investigate, the binary version of `zowie` takes a very long time to start up on macOS 10.15 (Catalina) and 11.1 (Big Sur).  On my test system inside a virtual machine running on a fast iMac, it takes 10 seconds or more before the first output from `zowie` appears.
 
 
+## Additional tips
+
+In the [wiki associated with the Zowie project in GitHub](https://github.com/mhucka/zowie/wiki), I have started writing some notes about how I personally use Zowie to combine Zotero with DEVONthink.
+
+
 ## Getting help
 
 If you find an issue, please submit it in [the GitHub issue tracker](https://github.com/mhucka/zowie/issues) for this repository.
 
 
 ## Contributing
 
 I would be happy to receive your help and participation if you are interested.  Everyone is asked to read and respect the [code of conduct](CONDUCT.md) when participating in this project.  Development generally takes place on the `development` branch.
 
 
 ## License
 
-This software is Copyright (C) 2020-2021, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
+This software is Copyright (C) 2020&ndash;2023, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
 
 
 ## Acknowledgments
 
 This work is a personal project developed by the author, using computing facilities and other resources of the [California Institute of Technology Library](https://www.library.caltech.edu).
 
 The [vector artwork](https://thenounproject.com/term/tag-exclamation-point/326951/) of an exclamation point circled by a zigzag, used as the icon for this repository, was created by  [Alfredo @ IconsAlfredo.com](https://thenounproject.com/AlfredoCreates/) from the Noun Project.  It is licensed under the Creative Commons [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/) license.
@@ -367,9 +327,7 @@
 * [pyzotero](https://github.com/urschrei/pyzotero) &ndash; a Python API client for Zotero
 * [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
 * [Shiv](https://github.com/linkedin/shiv) &ndash; command-line utility for creating self-contained Python zipapps
 * [Sidetrack](https://github.com/caltechlibrary/sidetrack) &ndash; simple debug logging/tracing package
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 The [developers of DEVONthink](https://www.devontechnologies.com/about), especially Jim Neumann and Christian Grunenberg, quickly and consistently replied to my many questions on the [DEVONtechnologies forums](https://discourse.devontechnologies.com).
-
-
```

### Comparing `zowie-1.2.0/zowie.egg-info/SOURCES.txt` & `zowie-1.3.0/zowie.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
+tests/test_exceptions.py
+tests/test_exit_codes.py
+tests/test_keyring_utils.py
 zowie/__init__.py
 zowie/__main__.py
 zowie/exceptions.py
 zowie/exit_codes.py
 zowie/keyring_utils.py
 zowie/main_body.py
 zowie/zotero.py
```

