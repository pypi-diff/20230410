# Comparing `tmp/ynam-0.4.0.post1.tar.gz` & `tmp/ynam-0.4.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynam-0.4.0.post1.tar", last modified: Wed Mar  1 17:45:42 2023, max compression
+gzip compressed data, was "ynam-0.4.0.post2.tar", last modified: Mon Apr 10 21:33:38 2023, max compression
```

## Comparing `ynam-0.4.0.post1.tar` & `ynam-0.4.0.post2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 snow       (501) staff       (20)        0 2023-03-01 17:45:42.490467 ynam-0.4.0.post1/
--rw-r--r--   0 snow       (501) staff       (20)    11343 2022-09-02 19:20:59.000000 ynam-0.4.0.post1/LICENSE
--rw-r--r--   0 snow       (501) staff       (20)      301 2023-03-01 17:45:42.490528 ynam-0.4.0.post1/PKG-INFO
--rw-r--r--   0 snow       (501) staff       (20)     5272 2023-01-31 17:56:53.000000 ynam-0.4.0.post1/README.md
--rw-r--r--   0 snow       (501) staff       (20)      103 2023-03-01 17:45:42.490918 ynam-0.4.0.post1/setup.cfg
--rw-r--r--   0 snow       (501) staff       (20)     1074 2023-03-01 17:45:16.000000 ynam-0.4.0.post1/setup.py
-drwxr-xr-x   0 snow       (501) staff       (20)        0 2023-03-01 17:45:42.487982 ynam-0.4.0.post1/src/
-drwxr-xr-x   0 snow       (501) staff       (20)        0 2023-03-01 17:45:42.489647 ynam-0.4.0.post1/src/ynam/
--rw-r--r--   0 snow       (501) staff       (20)        0 2022-09-02 21:39:49.000000 ynam-0.4.0.post1/src/ynam/__init__.py
--rw-r--r--   0 snow       (501) staff       (20)       31 2022-09-13 19:14:10.000000 ynam-0.4.0.post1/src/ynam/__main__.py
--rw-r--r--   0 snow       (501) staff       (20)      288 2023-03-01 17:44:16.000000 ynam-0.4.0.post1/src/ynam/_version.py
--rwxr-xr-x   0 snow       (501) staff       (20)     2475 2023-02-07 15:59:21.000000 ynam-0.4.0.post1/src/ynam/main.py
--rw-r--r--   0 snow       (501) staff       (20)     2537 2023-03-01 17:41:05.000000 ynam-0.4.0.post1/src/ynam/mint_api.py
--rw-r--r--   0 snow       (501) staff       (20)     2010 2023-01-25 18:44:07.000000 ynam-0.4.0.post1/src/ynam/quickstart.py
--rw-r--r--   0 snow       (501) staff       (20)    26169 2023-01-25 18:44:07.000000 ynam-0.4.0.post1/src/ynam/ynab_api.py
--rw-r--r--   0 snow       (501) staff       (20)     4726 2023-03-01 17:40:50.000000 ynam-0.4.0.post1/src/ynam/ynam_parser.py
--rw-r--r--   0 snow       (501) staff       (20)     1702 2023-01-31 17:56:53.000000 ynam-0.4.0.post1/src/ynam/ynam_secrets.py
-drwxr-xr-x   0 snow       (501) staff       (20)        0 2023-03-01 17:45:42.490349 ynam-0.4.0.post1/src/ynam.egg-info/
--rw-r--r--   0 snow       (501) staff       (20)      301 2023-03-01 17:45:42.000000 ynam-0.4.0.post1/src/ynam.egg-info/PKG-INFO
--rw-r--r--   0 snow       (501) staff       (20)      424 2023-03-01 17:45:42.000000 ynam-0.4.0.post1/src/ynam.egg-info/SOURCES.txt
--rw-r--r--   0 snow       (501) staff       (20)        1 2023-03-01 17:45:42.000000 ynam-0.4.0.post1/src/ynam.egg-info/dependency_links.txt
--rw-r--r--   0 snow       (501) staff       (20)       40 2023-03-01 17:45:42.000000 ynam-0.4.0.post1/src/ynam.egg-info/entry_points.txt
--rw-r--r--   0 snow       (501) staff       (20)        8 2023-03-01 17:45:42.000000 ynam-0.4.0.post1/src/ynam.egg-info/requires.txt
--rw-r--r--   0 snow       (501) staff       (20)        5 2023-03-01 17:45:42.000000 ynam-0.4.0.post1/src/ynam.egg-info/top_level.txt
+drwxr-xr-x   0 snow       (501) staff       (20)        0 2023-04-10 21:33:38.184655 ynam-0.4.0.post2/
+-rw-r--r--   0 snow       (501) staff       (20)    11343 2022-09-02 19:20:59.000000 ynam-0.4.0.post2/LICENSE
+-rw-r--r--   0 snow       (501) staff       (20)      301 2023-04-10 21:33:38.184724 ynam-0.4.0.post2/PKG-INFO
+-rw-r--r--   0 snow       (501) staff       (20)     5272 2023-01-31 17:56:53.000000 ynam-0.4.0.post2/README.md
+-rw-r--r--   0 snow       (501) staff       (20)      103 2023-04-10 21:33:38.184969 ynam-0.4.0.post2/setup.cfg
+-rw-r--r--   0 snow       (501) staff       (20)     1074 2023-03-01 17:45:16.000000 ynam-0.4.0.post2/setup.py
+drwxr-xr-x   0 snow       (501) staff       (20)        0 2023-04-10 21:33:38.181446 ynam-0.4.0.post2/src/
+drwxr-xr-x   0 snow       (501) staff       (20)        0 2023-04-10 21:33:38.183778 ynam-0.4.0.post2/src/ynam/
+-rw-r--r--   0 snow       (501) staff       (20)        0 2022-09-02 21:39:49.000000 ynam-0.4.0.post2/src/ynam/__init__.py
+-rw-r--r--   0 snow       (501) staff       (20)       31 2022-09-13 19:14:10.000000 ynam-0.4.0.post2/src/ynam/__main__.py
+-rw-r--r--   0 snow       (501) staff       (20)      288 2023-04-10 21:32:38.000000 ynam-0.4.0.post2/src/ynam/_version.py
+-rwxr-xr-x   0 snow       (501) staff       (20)     2475 2023-02-07 15:59:21.000000 ynam-0.4.0.post2/src/ynam/main.py
+-rw-r--r--   0 snow       (501) staff       (20)     2537 2023-03-01 17:41:05.000000 ynam-0.4.0.post2/src/ynam/mint_api.py
+-rw-r--r--   0 snow       (501) staff       (20)     2010 2023-01-25 18:44:07.000000 ynam-0.4.0.post2/src/ynam/quickstart.py
+-rw-r--r--   0 snow       (501) staff       (20)    26169 2023-01-25 18:44:07.000000 ynam-0.4.0.post2/src/ynam/ynab_api.py
+-rw-r--r--   0 snow       (501) staff       (20)     4726 2023-03-01 17:51:46.000000 ynam-0.4.0.post2/src/ynam/ynam_parser.py
+-rw-r--r--   0 snow       (501) staff       (20)     1756 2023-04-10 21:31:47.000000 ynam-0.4.0.post2/src/ynam/ynam_secrets.py
+drwxr-xr-x   0 snow       (501) staff       (20)        0 2023-04-10 21:33:38.184530 ynam-0.4.0.post2/src/ynam.egg-info/
+-rw-r--r--   0 snow       (501) staff       (20)      301 2023-04-10 21:33:38.000000 ynam-0.4.0.post2/src/ynam.egg-info/PKG-INFO
+-rw-r--r--   0 snow       (501) staff       (20)      424 2023-04-10 21:33:38.000000 ynam-0.4.0.post2/src/ynam.egg-info/SOURCES.txt
+-rw-r--r--   0 snow       (501) staff       (20)        1 2023-04-10 21:33:38.000000 ynam-0.4.0.post2/src/ynam.egg-info/dependency_links.txt
+-rw-r--r--   0 snow       (501) staff       (20)       40 2023-04-10 21:33:38.000000 ynam-0.4.0.post2/src/ynam.egg-info/entry_points.txt
+-rw-r--r--   0 snow       (501) staff       (20)        8 2023-04-10 21:33:38.000000 ynam-0.4.0.post2/src/ynam.egg-info/requires.txt
+-rw-r--r--   0 snow       (501) staff       (20)        5 2023-04-10 21:33:38.000000 ynam-0.4.0.post2/src/ynam.egg-info/top_level.txt
```

### Comparing `ynam-0.4.0.post1/LICENSE` & `ynam-0.4.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `ynam-0.4.0.post1/README.md` & `ynam-0.4.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `ynam-0.4.0.post1/setup.py` & `ynam-0.4.0.post2/setup.py`

 * *Files identical despite different names*

### Comparing `ynam-0.4.0.post1/src/ynam/main.py` & `ynam-0.4.0.post2/src/ynam/main.py`

 * *Files identical despite different names*

### Comparing `ynam-0.4.0.post1/src/ynam/mint_api.py` & `ynam-0.4.0.post2/src/ynam/mint_api.py`

 * *Files identical despite different names*

### Comparing `ynam-0.4.0.post1/src/ynam/quickstart.py` & `ynam-0.4.0.post2/src/ynam/quickstart.py`

 * *Files identical despite different names*

### Comparing `ynam-0.4.0.post1/src/ynam/ynab_api.py` & `ynam-0.4.0.post2/src/ynam/ynab_api.py`

 * *Files identical despite different names*

### Comparing `ynam-0.4.0.post1/src/ynam/ynam_parser.py` & `ynam-0.4.0.post2/src/ynam/ynam_parser.py`

 * *Files identical despite different names*

### Comparing `ynam-0.4.0.post1/src/ynam/ynam_secrets.py` & `ynam-0.4.0.post2/src/ynam/ynam_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     mint_password: str = None
     mint_mfa_seed: str = None
 
 
 def _loadSecrets() -> dict:
     fileSecrets = {}
     path = arg('secrets_file')
+    os.makedirs(os.path.dirname(path), exist_ok=True)
     if os.path.exists(path):
         with open(path) as file:
             try:
                 fileSecrets = json.load(file)
             except JSONDecodeError:
                 logger.warn(
                     f'Error reading {file.name}; assuming it to be empty')
```

