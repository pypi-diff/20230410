# Comparing `tmp/datastructuresLionelEric-1.0.92.tar.gz` & `tmp/datastructuresLionelEric-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastructuresLionelEric-1.0.92.tar", last modified: Sun Apr  9 22:45:10 2023, max compression
+gzip compressed data, was "datastructuresLionelEric-2.1.tar", last modified: Mon Apr 10 01:53:05 2023, max compression
```

## Comparing `datastructuresLionelEric-1.0.92.tar` & `datastructuresLionelEric-2.1.tar`

### file list

```diff
@@ -1,58 +1,26 @@
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:45:10.390340 datastructuresLionelEric-1.0.92/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.92/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      152 2023-04-09 22:45:10.390161 datastructuresLionelEric-1.0.92/PKG-INFO
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:45:10.377665 datastructuresLionelEric-1.0.92/datastructures/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.92/datastructures/.DS_Store
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:45:10.379962 datastructuresLionelEric-1.0.92/datastructures/Linear/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/CDLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/CSLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/DLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/LLQueue.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-09 22:31:55.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/LLStack.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/SLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:45:10.382236 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8979 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/CDLL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4716 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     9916 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/CSLL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5162 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8342 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/DLL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4620 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/DLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2516 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/LLQueue.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1780 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3403 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/LLStack.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2365 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8307 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/SLL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4657 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/SLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      199 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      177 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.92/datastructures/Linear/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:45:10.382976 datastructuresLionelEric-1.0.92/datastructures/nodes/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/Dnode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/TNode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:45:10.385187 datastructuresLionelEric-1.0.92/datastructures/nodes/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      629 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/__pycache__/Dnode.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      476 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/__pycache__/Dnode.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2706 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/__pycache__/TNode.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2118 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/__pycache__/TNode.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      198 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.92/datastructures/nodes/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:45:10.386802 datastructuresLionelEric-1.0.92/datastructures/trees/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 22:31:55.000000 datastructuresLionelEric-1.0.92/datastructures/trees/AVL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 22:31:55.000000 datastructuresLionelEric-1.0.92/datastructures/trees/BST.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:45:10.388516 datastructuresLionelEric-1.0.92/datastructures/trees/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5386 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/trees/__pycache__/AVL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3696 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.92/datastructures/trees/__pycache__/AVL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6289 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/trees/__pycache__/BST.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3364 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.92/datastructures/trees/__pycache__/BST.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      198 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/trees/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.92/datastructures/trees/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2809 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.92/datastructures/trees/main.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:45:10.389917 datastructuresLionelEric-1.0.92/datastructuresLionelEric.egg-info/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      152 2023-04-09 22:45:10.000000 datastructuresLionelEric-1.0.92/datastructuresLionelEric.egg-info/PKG-INFO
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2099 2023-04-09 22:45:10.000000 datastructuresLionelEric-1.0.92/datastructuresLionelEric.egg-info/SOURCES.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:45:10.000000 datastructuresLionelEric-1.0.92/datastructuresLionelEric.egg-info/dependency_links.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:45:10.000000 datastructuresLionelEric-1.0.92/datastructuresLionelEric.egg-info/top_level.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 22:45:10.390386 datastructuresLionelEric-1.0.92/setup.cfg
--rw-r--r--   0 lionelhasan   (501) staff       (20)      230 2023-04-09 22:44:50.000000 datastructuresLionelEric-1.0.92/setup.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.506030 datastructuresLionelEric-2.1/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      123 2023-04-10 01:53:05.505795 datastructuresLionelEric-2.1/PKG-INFO
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.501399 datastructuresLionelEric-2.1/datastructures/
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.503500 datastructuresLionelEric-2.1/datastructures/Linear/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/CDLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/CSLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/DLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/LLQueue.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/LLStack.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/Linear/SLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:30:12.000000 datastructuresLionelEric-2.1/datastructures/Linear/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.504140 datastructuresLionelEric-2.1/datastructures/nodes/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/nodes/Dnode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/nodes/TNode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:29:58.000000 datastructuresLionelEric-2.1/datastructures/nodes/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.504785 datastructuresLionelEric-2.1/datastructures/trees/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/trees/AVL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 22:51:55.000000 datastructuresLionelEric-2.1/datastructures/trees/BST.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:29:28.000000 datastructuresLionelEric-2.1/datastructures/trees/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-10 01:53:05.505578 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      123 2023-04-10 01:53:05.000000 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/PKG-INFO
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      600 2023-04-10 01:53:05.000000 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/SOURCES.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-10 01:53:05.000000 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/dependency_links.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       15 2023-04-10 01:53:05.000000 datastructuresLionelEric-2.1/datastructuresLionelEric.egg-info/top_level.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-10 01:53:05.506188 datastructuresLionelEric-2.1/setup.cfg
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      351 2023-04-10 01:52:59.000000 datastructuresLionelEric-2.1/setup.py
```

### Comparing `datastructuresLionelEric-1.0.92/datastructures/Linear/CDLL.py` & `datastructuresLionelEric-2.1/datastructures/Linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.92/datastructures/Linear/CSLL.py` & `datastructuresLionelEric-2.1/datastructures/Linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.92/datastructures/Linear/DLL.py` & `datastructuresLionelEric-2.1/datastructures/Linear/DLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.92/datastructures/Linear/LLQueue.py` & `datastructuresLionelEric-2.1/datastructures/Linear/LLQueue.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.92/datastructures/Linear/LLStack.py` & `datastructuresLionelEric-2.1/datastructures/Linear/LLStack.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.92/datastructures/Linear/SLL.py` & `datastructuresLionelEric-2.1/datastructures/Linear/SLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.92/datastructures/nodes/TNode.py` & `datastructuresLionelEric-2.1/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.92/datastructures/trees/AVL.py` & `datastructuresLionelEric-2.1/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.92/datastructures/trees/BST.py` & `datastructuresLionelEric-2.1/datastructures/trees/BST.py`

 * *Files identical despite different names*

