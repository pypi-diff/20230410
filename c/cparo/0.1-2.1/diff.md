# Comparing `tmp/cparo-0.1.tar.gz` & `tmp/cparo-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cparo-0.1.tar", last modified: Sun Apr  2 13:19:42 2023, max compression
+gzip compressed data, was "cparo-2.1.tar", last modified: Mon Apr 10 06:14:54 2023, max compression
```

## Comparing `cparo-0.1.tar` & `cparo-2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 13:19:42.068924 cparo-0.1/
--rw-rw-rw-   0        0        0       50 2023-04-02 13:19:42.067636 cparo-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-02 13:19:42.036599 cparo-0.1/cparo/
--rw-rw-rw-   0        0        0        0 2023-04-02 12:54:45.000000 cparo-0.1/cparo/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-04-02 13:15:55.000000 cparo-0.1/cparo/paro.py
-drwxrwxrwx   0        0        0        0 2023-04-02 13:19:42.064956 cparo-0.1/cparo.egg-info/
--rw-rw-rw-   0        0        0       50 2023-04-02 13:19:41.000000 cparo-0.1/cparo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-04-02 13:19:41.000000 cparo-0.1/cparo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 13:19:41.000000 cparo-0.1/cparo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-02 13:19:41.000000 cparo-0.1/cparo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-02 13:19:41.000000 cparo-0.1/cparo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-02 13:19:41.000000 cparo-0.1/cparo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-02 13:19:42.068924 cparo-0.1/setup.cfg
--rw-rw-rw-   0        0        0      292 2023-04-02 13:19:36.000000 cparo-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:14:54.953900 cparo-2.1/
+-rw-rw-rw-   0        0        0       50 2023-04-10 06:14:54.950837 cparo-2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 06:14:54.909383 cparo-2.1/cparo/
+-rw-rw-rw-   0        0        0        0 2023-04-02 12:54:45.000000 cparo-2.1/cparo/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-04-10 06:14:28.000000 cparo-2.1/cparo/paro.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:14:54.941988 cparo-2.1/cparo.egg-info/
+-rw-rw-rw-   0        0        0       50 2023-04-10 06:14:54.000000 cparo-2.1/cparo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-04-10 06:14:54.000000 cparo-2.1/cparo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 06:14:54.000000 cparo-2.1/cparo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 06:14:54.000000 cparo-2.1/cparo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-10 06:14:54.000000 cparo-2.1/cparo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-10 06:14:54.000000 cparo-2.1/cparo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 06:14:54.954723 cparo-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      292 2023-04-10 06:14:43.000000 cparo-2.1/setup.py
```

### Comparing `cparo-0.1/cparo/paro.py` & `cparo-2.1/cparo/paro.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,13 +14,17 @@
         url = "https://raw.githubusercontent.com/Pranavkak/cheaters/main/dfs.txt"
     elif(problem == "bbfs"):
         url = "https://raw.githubusercontent.com/Pranavkak/cheaters/main/bbfs.txt"
     elif(problem == "bdfs"):
         url = "https://raw.githubusercontent.com/Pranavkak/cheaters/main/bdfs.txt"
     elif(problem == "8"):
         url = "https://raw.githubusercontent.com/Pranavkak/cheaters/main/8.txt"
+    elif(problem == "a"):
+        url = "https://raw.githubusercontent.com/Pranavkak/cheaters/main/a.txt"
+    elif(problem == "ao"):
+        url = "https://raw.githubusercontent.com/Pranavkak/cheaters/main/ao.txt"
 
     response = requests.get(url)
     content = response.content.decode()  # decode the bytes into a string
 
     pyperclip.copy(content)
```

