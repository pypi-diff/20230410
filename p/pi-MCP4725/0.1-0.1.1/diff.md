# Comparing `tmp/pi_MCP4725-0.1.tar.gz` & `tmp/pi_MCP4725-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi_MCP4725-0.1.tar", last modified: Wed Mar 29 17:05:26 2023, max compression
+gzip compressed data, was "pi_MCP4725-0.1.1.tar", last modified: Mon Apr 10 17:58:33 2023, max compression
```

## Comparing `pi_MCP4725-0.1.tar` & `pi_MCP4725-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 17:05:26.087273 pi_MCP4725-0.1/
--rw-rw-rw-   0        0        0     1084 2023-03-29 11:20:20.000000 pi_MCP4725-0.1/LICENSE
--rw-rw-rw-   0        0        0     1153 2023-03-29 17:05:26.087273 pi_MCP4725-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3331 2023-03-29 16:59:36.000000 pi_MCP4725-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 17:05:26.077266 pi_MCP4725-0.1/pi_MCP4725/
--rw-rw-rw-   0        0        0     1436 2023-03-29 11:42:46.000000 pi_MCP4725-0.1/pi_MCP4725/MCP4725.py
-drwxrwxrwx   0        0        0        0 2023-03-29 17:05:26.086273 pi_MCP4725-0.1/pi_MCP4725.egg-info/
--rw-rw-rw-   0        0        0     1153 2023-03-29 17:05:26.000000 pi_MCP4725-0.1/pi_MCP4725.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-03-29 17:05:26.000000 pi_MCP4725-0.1/pi_MCP4725.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 17:05:26.000000 pi_MCP4725-0.1/pi_MCP4725.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-29 17:05:26.000000 pi_MCP4725-0.1/pi_MCP4725.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-29 17:05:26.000000 pi_MCP4725-0.1/pi_MCP4725.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-29 17:05:26.087775 pi_MCP4725-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1782 2023-03-29 17:05:16.000000 pi_MCP4725-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:58:33.022525 pi_MCP4725-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-03-29 11:20:20.000000 pi_MCP4725-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1151 2023-04-10 17:58:33.023027 pi_MCP4725-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3331 2023-03-29 16:59:36.000000 pi_MCP4725-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 17:58:33.009364 pi_MCP4725-0.1.1/pi_MCP4725/
+-rw-rw-rw-   0        0        0     1436 2023-03-29 11:42:46.000000 pi_MCP4725-0.1.1/pi_MCP4725/MCP4725.py
+-rw-rw-rw-   0        0        0       87 2023-04-10 17:52:26.000000 pi_MCP4725-0.1.1/pi_MCP4725/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:58:33.022026 pi_MCP4725-0.1.1/pi_MCP4725.egg-info/
+-rw-rw-rw-   0        0        0     1151 2023-04-10 17:58:32.000000 pi_MCP4725-0.1.1/pi_MCP4725.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-04-10 17:58:32.000000 pi_MCP4725-0.1.1/pi_MCP4725.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 17:58:32.000000 pi_MCP4725-0.1.1/pi_MCP4725.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 17:58:32.000000 pi_MCP4725-0.1.1/pi_MCP4725.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 17:58:32.000000 pi_MCP4725-0.1.1/pi_MCP4725.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-10 17:58:33.024025 pi_MCP4725-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1820 2023-04-10 17:52:31.000000 pi_MCP4725-0.1.1/setup.py
```

### Comparing `pi_MCP4725-0.1/LICENSE` & `pi_MCP4725-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pi_MCP4725-0.1/README.md` & `pi_MCP4725-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pi_MCP4725-0.1/pi_MCP4725/MCP4725.py` & `pi_MCP4725-0.1.1/pi_MCP4725/MCP4725.py`

 * *Files identical despite different names*

### Comparing `pi_MCP4725-0.1/pi_MCP4725.egg-info/PKG-INFO` & `pi_MCP4725-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
-Name: pi-MCP4725
-Version: 0.1
+Name: pi_MCP4725
+Version: 0.1.1
 Summary: Python module to use the MCP4725 DAC with the Raspberry Pi
 Home-page: https://github.com/sergiocaponi/pi_MCP4725
 Download-URL: https://github.com/sergiocaponi/pi_MCP4725/archive/refs/tags/v0.1.tar.gz
 Author: Sergio Caponi
 Author-email: contactme@sergiocaponi.com
 License: MIT
 Keywords: Raspberry Pi,DAC,MCP4725
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A Python module for the Raspberry Pi to interface with the [MCP4725](https://ww1.microchip.com/downloads/en/devicedoc/22039d.pdf) I²C Digital-to-Analogue Converter.
-
-# Installation
-
-## Compatibility
-
-Tested on Python 3.9 on a Raspberry Pi Zero W v1.1, but should be compatible with most Raspberry Pi models running the latest version of Python.
-
-Module works with Microchip's MCP4725 DAC.
+A Python module for the Raspberry Pi to interface with the MCP4725 IÂ²C Digital-to-Analogue Converter. (https://ww1.microchip.com/downloads/en/devicedoc/22039d.pdf) 
+
+Tested on Python 3.9 on a Raspberry Pi Zero W v1.1, but should be compatible with most Raspberry Pi models running the latest version of Python.
+
+Module works with Microchip's MCP4725 DAC.
```

### Comparing `pi_MCP4725-0.1/setup.py` & `pi_MCP4725-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from codecs import open
-from os import path
-
 from distutils.core import setup
 
-here = path.abspath(path.dirname(__file__))
-with open(path.join(here, 'desc.md'), 'rb', 'utf-8') as f:
-    full_description = f.read()
+# read the contents of your description file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "DESC.md").read_text()
 
 
 setup(
 	name = 'pi_MCP4725',         # How you named your package folder (MyLib)
 	packages = ['pi_MCP4725'],   # Chose the same as "name"
-	version = '0.1',      # Start with a small number and increase it with every change you make
+	version = '0.1.1',      # Start with a small number and increase it with every change you make
 	license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
 	description = 'Python module to use the MCP4725 DAC with the Raspberry Pi',   # Give a short description about your library
-	long_description = full_description,
+	long_description = long_description,
+	long_description_content_type='text/markdown',
 	author = 'Sergio Caponi',                   # Type in your name
 	author_email = 'contactme@sergiocaponi.com',      # Type in your E-Mail
 	url = 'https://github.com/sergiocaponi/pi_MCP4725',   # Provide either the link to your github or to your website
 	download_url = 'https://github.com/sergiocaponi/pi_MCP4725/archive/refs/tags/v0.1.tar.gz',    # I explain this later on
 	keywords = ['Raspberry Pi', 'DAC', 'MCP4725'],   # Keywords that define your package best
 	install_requires=[            # I get to this in a second
 					'smbus2',
```

