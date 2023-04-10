# Comparing `tmp/datastructuresLionelEric-2.1.tar.gz` & `tmp/datastructuresLionelEric-2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastructuresLionelEric-2.1.tar", last modified: Mon Apr 10 01:53:05 2023, max compression
+gzip compressed data, was "datastructuresLionelEric-2.12.tar", last modified: Mon Apr 10 02:02:44 2023, max compression
```

## Comparing `datastructuresLionelEric-2.1.tar` & `datastructuresLionelEric-2.12.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.506030 datastructuresLionelEric-2.1/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      123 2023-04-10 01:53:05.505795 datastructuresLionelEric-2.1/PKG-INFO
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.501399 datastructuresLionelEric-2.1/datastructures/
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.503500 datastructuresLionelEric-2.1/datastructures/Linear/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/CDLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/CSLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/DLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/LLQueue.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/LLStack.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/SLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:30:12.000000 datastructuresLionelEric-2.1/datastructures/Linear/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.504140 datastructuresLionelEric-2.1/datastructures/nodes/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/nodes/Dnode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/nodes/TNode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:29:58.000000 datastructuresLionelEric-2.1/datastructures/nodes/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.504785 datastructuresLionelEric-2.1/datastructures/trees/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/trees/AVL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/trees/BST.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:29:28.000000 datastructuresLionelEric-2.1/datastructures/trees/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.505578 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      123 2023-04-10 01:53:05.000000 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/PKG-INFO
--rw-r--r--   0 lionelhasan   (501) staff       (20)      600 2023-04-10 01:53:05.000000 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/SOURCES.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-10 01:53:05.000000 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/dependency_links.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       15 2023-04-10 01:53:05.000000 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/top_level.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-10 01:53:05.506188 datastructuresLionelEric-2.1/setup.cfg
--rw-r--r--   0 lionelhasan   (501) staff       (20)      351 2023-04-10 01:52:59.000000 datastructuresLionelEric-2.1/setup.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 02:02:44.751477 datastructuresLionelEric-2.12/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      171 2023-04-10 02:02:44.751320 datastructuresLionelEric-2.12/PKG-INFO
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 02:02:44.747336 datastructuresLionelEric-2.12/datastructures/
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 02:02:44.749321 datastructuresLionelEric-2.12/datastructures/Linear/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/Linear/CDLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/Linear/CSLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/Linear/DLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/Linear/LLQueue.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/Linear/LLStack.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/Linear/SLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:30:12.000000 datastructuresLionelEric-2.12/datastructures/Linear/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 02:02:44.749779 datastructuresLionelEric-2.12/datastructures/nodes/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/nodes/Dnode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/nodes/TNode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:29:58.000000 datastructuresLionelEric-2.12/datastructures/nodes/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 02:02:44.750199 datastructuresLionelEric-2.12/datastructures/trees/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/trees/AVL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.12/datastructures/trees/BST.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:29:28.000000 datastructuresLionelEric-2.12/datastructures/trees/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 02:02:44.751070 datastructuresLionelEric-2.12/datastructuresLionelEric.egg-info/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      171 2023-04-10 02:02:44.000000 datastructuresLionelEric-2.12/datastructuresLionelEric.egg-info/PKG-INFO
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      600 2023-04-10 02:02:44.000000 datastructuresLionelEric-2.12/datastructuresLionelEric.egg-info/SOURCES.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-10 02:02:44.000000 datastructuresLionelEric-2.12/datastructuresLionelEric.egg-info/dependency_links.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       15 2023-04-10 02:02:44.000000 datastructuresLionelEric-2.12/datastructuresLionelEric.egg-info/top_level.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-10 02:02:44.751526 datastructuresLionelEric-2.12/setup.cfg
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      330 2023-04-10 02:02:16.000000 datastructuresLionelEric-2.12/setup.py
```

### Comparing `datastructuresLionelEric-2.1/datastructures/Linear/CDLL.py` & `datastructuresLionelEric-2.12/datastructures/Linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-2.1/datastructures/Linear/CSLL.py` & `datastructuresLionelEric-2.12/datastructures/Linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-2.1/datastructures/Linear/DLL.py` & `datastructuresLionelEric-2.12/datastructures/Linear/DLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-2.1/datastructures/Linear/LLQueue.py` & `datastructuresLionelEric-2.12/datastructures/Linear/LLQueue.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-2.1/datastructures/Linear/LLStack.py` & `datastructuresLionelEric-2.12/datastructures/Linear/LLStack.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-2.1/datastructures/Linear/SLL.py` & `datastructuresLionelEric-2.12/datastructures/Linear/SLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-2.1/datastructures/nodes/TNode.py` & `datastructuresLionelEric-2.12/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-2.1/datastructures/trees/AVL.py` & `datastructuresLionelEric-2.12/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-2.1/datastructures/trees/BST.py` & `datastructuresLionelEric-2.12/datastructures/trees/BST.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/SOURCES.txt` & `datastructuresLionelEric-2.12/datastructuresLionelEric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

