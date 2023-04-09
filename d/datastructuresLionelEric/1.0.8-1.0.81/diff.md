# Comparing `tmp/datastructuresLionelEric-1.0.8.tar.gz` & `tmp/datastructuresLionelEric-1.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastructuresLionelEric-1.0.8.tar", last modified: Sun Apr  9 22:00:26 2023, max compression
+gzip compressed data, was "datastructuresLionelEric-1.0.81.tar", last modified: Sun Apr  9 22:21:44 2023, max compression
```

## Comparing `datastructuresLionelEric-1.0.8.tar` & `datastructuresLionelEric-1.0.81.tar`

### file list

```diff
@@ -1,44 +1,58 @@
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.143598 datastructuresLionelEric-1.0.8/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.8/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 22:00:26.143412 datastructuresLionelEric-1.0.8/PKG-INFO
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.135681 datastructuresLionelEric-1.0.8/datastructures/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/.DS_Store
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.138342 datastructuresLionelEric-1.0.8/datastructures/Linear/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/CDLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/CSLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/DLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/LLQueue.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-08 22:50:35.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/LLStack.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/SLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.139950 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4716 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5162 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4620 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/DLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1780 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2365 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4657 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/SLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      177 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.140553 datastructuresLionelEric-1.0.8/datastructures/nodes/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/Dnode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/TNode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.141017 datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      476 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/Dnode.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2118 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/TNode.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.141467 datastructuresLionelEric-1.0.8/datastructures/trees/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 21:33:54.000000 datastructuresLionelEric-1.0.8/datastructures/trees/AVL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 21:50:16.000000 datastructuresLionelEric-1.0.8/datastructures/trees/BST.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.142273 datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3696 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/AVL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3364 2023-04-09 21:50:17.000000 datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/BST.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.143132 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 22:00:26.000000 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/PKG-INFO
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1345 2023-04-09 22:00:26.000000 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/SOURCES.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:00:26.000000 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/dependency_links.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:00:26.000000 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/top_level.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 22:00:26.143671 datastructuresLionelEric-1.0.8/setup.cfg
--rw-r--r--   0 lionelhasan   (501) staff       (20)      314 2023-04-09 21:59:45.000000 datastructuresLionelEric-1.0.8/setup.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:21:44.087817 datastructuresLionelEric-1.0.81/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.81/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      152 2023-04-09 22:21:44.087638 datastructuresLionelEric-1.0.81/PKG-INFO
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:21:44.079174 datastructuresLionelEric-1.0.81/datastructures/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.81/datastructures/.DS_Store
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:21:44.081478 datastructuresLionelEric-1.0.81/datastructures/Linear/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/CDLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/CSLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/DLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/LLQueue.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/LLStack.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/SLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:21:44.083624 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8979 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/CDLL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     4716 2023-04-09 22:18:39.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     9916 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/CSLL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5162 2023-04-09 22:18:39.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8342 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/DLL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     4620 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/DLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2516 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/LLQueue.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1780 2023-04-09 22:18:39.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     3403 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/LLStack.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2365 2023-04-09 22:18:39.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8307 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/SLL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     4657 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/SLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      199 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      177 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:21:44.084491 datastructuresLionelEric-1.0.81/datastructures/nodes/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/Dnode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/TNode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:21:44.085312 datastructuresLionelEric-1.0.81/datastructures/nodes/__pycache__/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      629 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/__pycache__/Dnode.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      476 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/__pycache__/Dnode.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2706 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/__pycache__/TNode.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2118 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/__pycache__/TNode.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      198 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.81/datastructures/nodes/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:21:44.085701 datastructuresLionelEric-1.0.81/datastructures/trees/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/trees/AVL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/trees/BST.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:21:44.086795 datastructuresLionelEric-1.0.81/datastructures/trees/__pycache__/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5386 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/trees/__pycache__/AVL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     3696 2023-04-09 22:18:39.000000 datastructuresLionelEric-1.0.81/datastructures/trees/__pycache__/AVL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6289 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/trees/__pycache__/BST.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     3364 2023-04-09 22:18:39.000000 datastructuresLionelEric-1.0.81/datastructures/trees/__pycache__/BST.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      198 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/trees/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 22:18:39.000000 datastructuresLionelEric-1.0.81/datastructures/trees/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2809 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.81/datastructures/trees/main.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:21:44.087428 datastructuresLionelEric-1.0.81/datastructuresLionelEric.egg-info/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      152 2023-04-09 22:21:43.000000 datastructuresLionelEric-1.0.81/datastructuresLionelEric.egg-info/PKG-INFO
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2099 2023-04-09 22:21:44.000000 datastructuresLionelEric-1.0.81/datastructuresLionelEric.egg-info/SOURCES.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:21:43.000000 datastructuresLionelEric-1.0.81/datastructuresLionelEric.egg-info/dependency_links.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:21:43.000000 datastructuresLionelEric-1.0.81/datastructuresLionelEric.egg-info/top_level.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 22:21:44.087874 datastructuresLionelEric-1.0.81/setup.cfg
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      313 2023-04-09 22:18:49.000000 datastructuresLionelEric-1.0.81/setup.py
```

### Comparing `datastructuresLionelEric-1.0.8/.DS_Store` & `datastructuresLionelEric-1.0.81/.DS_Store`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/.DS_Store` & `datastructuresLionelEric-1.0.81/datastructures/.DS_Store`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/CDLL.py` & `datastructuresLionelEric-1.0.81/datastructures/Linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/CSLL.py` & `datastructuresLionelEric-1.0.81/datastructures/Linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/DLL.py` & `datastructuresLionelEric-1.0.81/datastructures/Linear/DLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/LLQueue.py` & `datastructuresLionelEric-1.0.81/datastructures/Linear/LLQueue.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/LLStack.py` & `datastructuresLionelEric-1.0.81/datastructures/Linear/LLStack.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/SLL.py` & `datastructuresLionelEric-1.0.81/datastructures/Linear/SLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc` & `datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr  8 22:45:52 2023 UTC, .py size: 6914 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 a0ee 3164 021b 0000  a.........1d....
+00000000: 610d 0d0a 0000 0000 be39 3364 021b 0000  a........93d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6502 6503 8301 a004 a100 6a05 6a05  ..e.e.......j.j.
 00000050: 5a06 6500 6a07 a008 6509 6506 8301 a101  Z.e.j...e.e.....
 00000060: 0100 6400 6403 6c0a 6d0b 5a0b 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6404 6405 8400 6405 650b 8303 5a0c 6401  d.d...d.e...Z.d.
```

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc` & `datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr  8 22:45:52 2023 UTC, .py size: 8735 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 a0ee 3164 1f22 0000  a.........1d."..
+00000000: 610d 0d0a 0000 0000 be39 3364 1f22 0000  a........93d."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6502 6503 8301 a004 a100 6a05 6a05  ..e.e.......j.j.
 00000050: 5a06 6500 6a07 a008 6509 6506 8301 a101  Z.e.j...e.e.....
 00000060: 0100 6400 6403 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c0c 6d0d 5a0d 0100 4700 6405 6406  d.l.m.Z...G.d.d.
```

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/DLL.cpython-39.pyc` & `datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/DLL.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc` & `datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr  8 22:45:52 2023 UTC, .py size: 1065 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 a0ee 3164 2904 0000  a.........1d)...
+00000000: 610d 0d0a 0000 0000 be39 3364 2904 0000  a........93d)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6502 6503 8301 a004 a100 6a05 6a05  ..e.e.......j.j.
 00000050: 5a06 6500 6a07 a008 6509 6506 8301 a101  Z.e.j...e.e.....
 00000060: 0100 6400 6403 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c0c 6d0d 5a0d 0100 4700 6405 6406  d.l.m.Z...G.d.d.
```

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc` & `datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr  8 22:50:35 2023 UTC, .py size: 1259 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 bbef 3164 eb04 0000  a.........1d....
+00000000: 610d 0d0a 0000 0000 be39 3364 eb04 0000  a........93d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6502 6503 8301 a004 a100 6a05 6a05  ..e.e.......j.j.
 00000050: 5a06 6500 6a07 a008 6509 6506 8301 a101  Z.e.j...e.e.....
 00000060: 0100 6400 6403 6c0a 6d0b 5a0b 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6404 6405 8400 6405 650b 8303 5a0c 6401  d.d...d.e...Z.d.
```

### Comparing `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/SLL.cpython-39.pyc` & `datastructuresLionelEric-1.0.81/datastructures/Linear/__pycache__/SLL.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/nodes/.DS_Store` & `datastructuresLionelEric-1.0.81/datastructures/nodes/.DS_Store`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/nodes/TNode.py` & `datastructuresLionelEric-1.0.81/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/TNode.cpython-39.pyc` & `datastructuresLionelEric-1.0.81/datastructures/nodes/__pycache__/TNode.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/trees/AVL.py` & `datastructuresLionelEric-1.0.81/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/trees/BST.py` & `datastructuresLionelEric-1.0.81/datastructures/trees/BST.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/AVL.cpython-39.pyc` & `datastructuresLionelEric-1.0.81/datastructures/trees/__pycache__/AVL.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  9 21:33:54 2023 UTC, .py size: 6667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 422f 3364 0b1a 0000  a.......B/3d....
+00000000: 610d 0d0a 0000 0000 be39 3364 0b1a 0000  a........93d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6502 6503 8301 a004 a100 6a05 6a05  ..e.e.......j.j.
 00000050: 5a06 6500 6a07 a008 6509 6506 8301 a101  Z.e.j...e.e.....
 00000060: 0100 6400 6403 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c0c 6d0d 5a0d 0100 4700 6405 6406  d.l.m.Z...G.d.d.
```

### Comparing `datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/BST.cpython-39.pyc` & `datastructuresLionelEric-1.0.81/datastructures/trees/__pycache__/BST.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  9 21:50:16 2023 UTC, .py size: 5584 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1833 3364 d015 0000  a........33d....
+00000000: 610d 0d0a 0000 0000 be39 3364 d015 0000  a........93d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6502 6503 8301 a004 a100 6a05 6a05  ..e.e.......j.j.
 00000050: 5a06 6500 6a07 a008 6509 6506 8301 a101  Z.e.j...e.e.....
 00000060: 0100 6400 6403 6c0a 6d0b 5a0b 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6404 6405 8400 6405 8302 5a0c 6401 5300  d.d...d...Z.d.S.
```

### Comparing `datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/SOURCES.txt` & `datastructuresLionelEric-1.0.81/datastructuresLionelEric.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,30 +4,44 @@
 datastructures/Linear/CDLL.py
 datastructures/Linear/CSLL.py
 datastructures/Linear/DLL.py
 datastructures/Linear/LLQueue.py
 datastructures/Linear/LLStack.py
 datastructures/Linear/SLL.py
 datastructures/Linear/__init__.py
+datastructures/Linear/__pycache__/CDLL.cpython-311.pyc
 datastructures/Linear/__pycache__/CDLL.cpython-39.pyc
+datastructures/Linear/__pycache__/CSLL.cpython-311.pyc
 datastructures/Linear/__pycache__/CSLL.cpython-39.pyc
+datastructures/Linear/__pycache__/DLL.cpython-311.pyc
 datastructures/Linear/__pycache__/DLL.cpython-39.pyc
+datastructures/Linear/__pycache__/LLQueue.cpython-311.pyc
 datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc
+datastructures/Linear/__pycache__/LLStack.cpython-311.pyc
 datastructures/Linear/__pycache__/LLStack.cpython-39.pyc
+datastructures/Linear/__pycache__/SLL.cpython-311.pyc
 datastructures/Linear/__pycache__/SLL.cpython-39.pyc
+datastructures/Linear/__pycache__/__init__.cpython-311.pyc
 datastructures/Linear/__pycache__/__init__.cpython-39.pyc
 datastructures/nodes/.DS_Store
 datastructures/nodes/Dnode.py
 datastructures/nodes/TNode.py
 datastructures/nodes/__init__.py
+datastructures/nodes/__pycache__/Dnode.cpython-311.pyc
 datastructures/nodes/__pycache__/Dnode.cpython-39.pyc
+datastructures/nodes/__pycache__/TNode.cpython-311.pyc
 datastructures/nodes/__pycache__/TNode.cpython-39.pyc
+datastructures/nodes/__pycache__/__init__.cpython-311.pyc
 datastructures/nodes/__pycache__/__init__.cpython-39.pyc
 datastructures/trees/AVL.py
 datastructures/trees/BST.py
+datastructures/trees/main.py
+datastructures/trees/__pycache__/AVL.cpython-311.pyc
 datastructures/trees/__pycache__/AVL.cpython-39.pyc
+datastructures/trees/__pycache__/BST.cpython-311.pyc
 datastructures/trees/__pycache__/BST.cpython-39.pyc
+datastructures/trees/__pycache__/__init__.cpython-311.pyc
 datastructures/trees/__pycache__/__init__.cpython-39.pyc
 datastructuresLionelEric.egg-info/PKG-INFO
 datastructuresLionelEric.egg-info/SOURCES.txt
 datastructuresLionelEric.egg-info/dependency_links.txt
 datastructuresLionelEric.egg-info/top_level.txt
```

