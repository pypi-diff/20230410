# Comparing `tmp/pi_MCP4725-0.1.2.tar.gz` & `tmp/pi_MCP4725-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi_MCP4725-0.1.2.tar", last modified: Mon Apr 10 18:44:49 2023, max compression
+gzip compressed data, was "pi_MCP4725-0.1.3.tar", last modified: Mon Apr 10 18:57:03 2023, max compression
```

## Comparing `pi_MCP4725-0.1.2.tar` & `pi_MCP4725-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 18:44:49.062708 pi_MCP4725-0.1.2/
--rw-rw-rw-   0        0        0     1002 2023-04-10 18:39:36.000000 pi_MCP4725-0.1.2/DESC.md
--rw-rw-rw-   0        0        0     1084 2023-03-29 11:20:20.000000 pi_MCP4725-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       15 2023-04-10 18:41:16.000000 pi_MCP4725-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1802 2023-04-10 18:44:49.063207 pi_MCP4725-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3331 2023-03-29 16:59:36.000000 pi_MCP4725-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 18:44:49.044702 pi_MCP4725-0.1.2/pi_MCP4725/
--rw-rw-rw-   0        0        0     1436 2023-03-29 11:42:46.000000 pi_MCP4725-0.1.2/pi_MCP4725/MCP4725.py
--rw-rw-rw-   0        0        0       87 2023-04-10 17:52:26.000000 pi_MCP4725-0.1.2/pi_MCP4725/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:44:49.062206 pi_MCP4725-0.1.2/pi_MCP4725.egg-info/
--rw-rw-rw-   0        0        0     1802 2023-04-10 18:44:48.000000 pi_MCP4725-0.1.2/pi_MCP4725.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-10 18:44:48.000000 pi_MCP4725-0.1.2/pi_MCP4725.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 18:44:48.000000 pi_MCP4725-0.1.2/pi_MCP4725.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 18:44:48.000000 pi_MCP4725-0.1.2/pi_MCP4725.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-10 18:44:48.000000 pi_MCP4725-0.1.2/pi_MCP4725.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-10 18:44:49.064206 pi_MCP4725-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1822 2023-04-10 18:37:41.000000 pi_MCP4725-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:57:03.634650 pi_MCP4725-0.1.3/
+-rw-rw-rw-   0        0        0     1002 2023-04-10 18:39:36.000000 pi_MCP4725-0.1.3/DESC.md
+-rw-rw-rw-   0        0        0     1084 2023-03-29 11:20:20.000000 pi_MCP4725-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-04-10 18:41:16.000000 pi_MCP4725-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1802 2023-04-10 18:57:03.635150 pi_MCP4725-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3331 2023-03-29 16:59:36.000000 pi_MCP4725-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 18:57:03.623650 pi_MCP4725-0.1.3/pi_MCP4725/
+-rw-rw-rw-   0        0        0     1436 2023-03-29 11:42:46.000000 pi_MCP4725-0.1.3/pi_MCP4725/MCP4725.py
+-rw-rw-rw-   0        0        0       84 2023-04-10 18:53:38.000000 pi_MCP4725-0.1.3/pi_MCP4725/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:57:03.634150 pi_MCP4725-0.1.3/pi_MCP4725.egg-info/
+-rw-rw-rw-   0        0        0     1802 2023-04-10 18:57:03.000000 pi_MCP4725-0.1.3/pi_MCP4725.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-10 18:57:03.000000 pi_MCP4725-0.1.3/pi_MCP4725.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 18:57:03.000000 pi_MCP4725-0.1.3/pi_MCP4725.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 18:57:03.000000 pi_MCP4725-0.1.3/pi_MCP4725.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 18:57:03.000000 pi_MCP4725-0.1.3/pi_MCP4725.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-10 18:57:03.636149 pi_MCP4725-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1822 2023-04-10 18:54:06.000000 pi_MCP4725-0.1.3/setup.py
```

### Comparing `pi_MCP4725-0.1.2/DESC.md` & `pi_MCP4725-0.1.3/DESC.md`

 * *Files identical despite different names*

### Comparing `pi_MCP4725-0.1.2/LICENSE` & `pi_MCP4725-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pi_MCP4725-0.1.2/PKG-INFO` & `pi_MCP4725-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pi_MCP4725
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python module to use the MCP4725 DAC with the Raspberry Pi
 Home-page: https://github.com/sergiocaponi/pi_MCP4725
-Download-URL: https://github.com/sergiocaponi/pi_MCP4725/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/sergiocaponi/pi_MCP4725/archive/refs/tags/v0.1.3.tar.gz
 Author: Sergio Caponi
 Author-email: contactme@sergiocaponi.com
 License: MIT
 Keywords: Raspberry Pi,DAC,MCP4725
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pi_MCP4725-0.1.2/README.md` & `pi_MCP4725-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pi_MCP4725-0.1.2/pi_MCP4725/MCP4725.py` & `pi_MCP4725-0.1.3/pi_MCP4725/MCP4725.py`

 * *Files identical despite different names*

### Comparing `pi_MCP4725-0.1.2/pi_MCP4725.egg-info/PKG-INFO` & `pi_MCP4725-0.1.3/pi_MCP4725.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pi-MCP4725
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python module to use the MCP4725 DAC with the Raspberry Pi
 Home-page: https://github.com/sergiocaponi/pi_MCP4725
-Download-URL: https://github.com/sergiocaponi/pi_MCP4725/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/sergiocaponi/pi_MCP4725/archive/refs/tags/v0.1.3.tar.gz
 Author: Sergio Caponi
 Author-email: contactme@sergiocaponi.com
 License: MIT
 Keywords: Raspberry Pi,DAC,MCP4725
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pi_MCP4725-0.1.2/setup.py` & `pi_MCP4725-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "DESC.md").read_text()
 
 
 setup(
 	name = 'pi_MCP4725',         # How you named your package folder (MyLib)
 	packages = ['pi_MCP4725'],   # Chose the same as "name"
-	version = '0.1.2',      # Start with a small number and increase it with every change you make
+	version = '0.1.3',      # Start with a small number and increase it with every change you make
 	license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
 	description = 'Python module to use the MCP4725 DAC with the Raspberry Pi',   # Give a short description about your library
 	long_description = long_description,
 	long_description_content_type='text/markdown',
 	author = 'Sergio Caponi',                   # Type in your name
 	author_email = 'contactme@sergiocaponi.com',      # Type in your E-Mail
 	url = 'https://github.com/sergiocaponi/pi_MCP4725',   # Provide either the link to your github or to your website
-	download_url = 'https://github.com/sergiocaponi/pi_MCP4725/archive/refs/tags/v0.1.2.tar.gz',    # I explain this later on
+	download_url = 'https://github.com/sergiocaponi/pi_MCP4725/archive/refs/tags/v0.1.3.tar.gz',    # I explain this later on
 	keywords = ['Raspberry Pi', 'DAC', 'MCP4725'],   # Keywords that define your package best
 	install_requires=[            # I get to this in a second
 					'smbus2',
 			],
 	classifiers=[
 		'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
 		'Intended Audience :: Developers',      # Define that your audience are developers
```

