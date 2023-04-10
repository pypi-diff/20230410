# Comparing `tmp/pi_MCP342x-0.1.tar.gz` & `tmp/pi_MCP342x-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi_MCP342x-0.1.tar", last modified: Wed Mar 29 16:37:00 2023, max compression
+gzip compressed data, was "pi_MCP342x-0.1.1.tar", last modified: Mon Apr 10 17:40:18 2023, max compression
```

## Comparing `pi_MCP342x-0.1.tar` & `pi_MCP342x-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 16:37:00.535904 pi_MCP342x-0.1/
--rw-rw-rw-   0        0        0     1084 2023-03-28 11:20:49.000000 pi_MCP342x-0.1/LICENSE
--rw-rw-rw-   0        0        0      778 2023-03-29 16:37:00.535904 pi_MCP342x-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5018 2023-03-29 12:05:43.000000 pi_MCP342x-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 16:37:00.519907 pi_MCP342x-0.1/pi_MCP342x/
--rw-rw-rw-   0        0        0      199 2023-03-29 16:03:23.000000 pi_MCP342x-0.1/pi_MCP342x/__init__.py
--rw-rw-rw-   0        0        0     3829 2023-03-29 15:40:35.000000 pi_MCP342x-0.1/pi_MCP342x/pi_MCP342x.py
-drwxrwxrwx   0        0        0        0 2023-03-29 16:37:00.534904 pi_MCP342x-0.1/pi_MCP342x.egg-info/
--rw-rw-rw-   0        0        0      778 2023-03-29 16:37:00.000000 pi_MCP342x-0.1/pi_MCP342x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-03-29 16:37:00.000000 pi_MCP342x-0.1/pi_MCP342x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 16:37:00.000000 pi_MCP342x-0.1/pi_MCP342x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-29 16:37:00.000000 pi_MCP342x-0.1/pi_MCP342x.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-29 16:37:00.000000 pi_MCP342x-0.1/pi_MCP342x.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-29 16:37:00.536905 pi_MCP342x-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1595 2023-03-29 16:25:32.000000 pi_MCP342x-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:40:18.983960 pi_MCP342x-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-03-28 11:20:49.000000 pi_MCP342x-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      782 2023-04-10 17:40:18.983960 pi_MCP342x-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5018 2023-03-29 12:05:43.000000 pi_MCP342x-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 17:40:18.964961 pi_MCP342x-0.1.1/pi_MCP342x/
+-rw-rw-rw-   0        0        0      161 2023-04-10 17:36:25.000000 pi_MCP342x-0.1.1/pi_MCP342x/__init__.py
+-rw-rw-rw-   0        0        0     3829 2023-04-04 16:29:54.000000 pi_MCP342x-0.1.1/pi_MCP342x/pi_MCP342x.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:40:18.982960 pi_MCP342x-0.1.1/pi_MCP342x.egg-info/
+-rw-rw-rw-   0        0        0      782 2023-04-10 17:40:18.000000 pi_MCP342x-0.1.1/pi_MCP342x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-10 17:40:18.000000 pi_MCP342x-0.1.1/pi_MCP342x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 17:40:18.000000 pi_MCP342x-0.1.1/pi_MCP342x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 17:40:18.000000 pi_MCP342x-0.1.1/pi_MCP342x.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 17:40:18.000000 pi_MCP342x-0.1.1/pi_MCP342x.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-10 17:40:18.985461 pi_MCP342x-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1629 2023-04-10 17:37:30.000000 pi_MCP342x-0.1.1/setup.py
```

### Comparing `pi_MCP342x-0.1/LICENSE` & `pi_MCP342x-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pi_MCP342x-0.1/PKG-INFO` & `pi_MCP342x-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pi_MCP342x
-Version: 0.1
+Version: 0.1.1
 Summary: Python module to use the MCP342x series of ADCs with the Raspberry Pi
 Home-page: https://github.com/sergiocaponi/pi_MCP342x
-Download-URL: https://github.com/sergiocaponi/pi_MCP342x/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/sergiocaponi/pi_MCP342x/archive/refs/tags/v0.1.1.tar.gz
 Author: Sergio Caponi
 Author-email: contactme@sergiocaponi.com
 License: MIT
 Keywords: Raspberry Pi,ADC,MCP342x,MCP3422,MCP3423,MCP3424
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pi_MCP342x-0.1/README.md` & `pi_MCP342x-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pi_MCP342x-0.1/pi_MCP342x/pi_MCP342x.py` & `pi_MCP342x-0.1.1/pi_MCP342x/pi_MCP342x.py`

 * *Files identical despite different names*

### Comparing `pi_MCP342x-0.1/pi_MCP342x.egg-info/PKG-INFO` & `pi_MCP342x-0.1.1/pi_MCP342x.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pi-MCP342x
-Version: 0.1
+Version: 0.1.1
 Summary: Python module to use the MCP342x series of ADCs with the Raspberry Pi
 Home-page: https://github.com/sergiocaponi/pi_MCP342x
-Download-URL: https://github.com/sergiocaponi/pi_MCP342x/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/sergiocaponi/pi_MCP342x/archive/refs/tags/v0.1.1.tar.gz
 Author: Sergio Caponi
 Author-email: contactme@sergiocaponi.com
 License: MIT
 Keywords: Raspberry Pi,ADC,MCP342x,MCP3422,MCP3423,MCP3424
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pi_MCP342x-0.1/setup.py` & `pi_MCP342x-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from distutils.core import setup
+
+
+
 setup(
 	name = 'pi_MCP342x',         # How you named your package folder (MyLib)
 	packages = ['pi_MCP342x'],   # Chose the same as "name"
-	version = '0.1',      # Start with a small number and increase it with every change you make
+	version = '0.1.1',      # Start with a small number and increase it with every change you make
 	license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
 	description = 'Python module to use the MCP342x series of ADCs with the Raspberry Pi',   # Give a short description about your library
+	readme = 'README.md',
 	author = 'Sergio Caponi',                   # Type in your name
 	author_email = 'contactme@sergiocaponi.com',      # Type in your E-Mail
 	url = 'https://github.com/sergiocaponi/pi_MCP342x',   # Provide either the link to your github or to your website
-	download_url = 'https://github.com/sergiocaponi/pi_MCP342x/archive/refs/tags/v0.1.tar.gz',    # I explain this later on
+	download_url = 'https://github.com/sergiocaponi/pi_MCP342x/archive/refs/tags/v0.1.1.tar.gz',    # I explain this later on
 	keywords = ['Raspberry Pi', 'ADC', 'MCP342x', 'MCP3422', 'MCP3423', 'MCP3424'],   # Keywords that define your package best
 	install_requires=[            # I get to this in a second
 					'smbus2',
 			],
 	classifiers=[
 		'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
 		'Intended Audience :: Developers',      # Define that your audience are developers
```

