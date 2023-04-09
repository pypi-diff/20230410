# Comparing `tmp/datastructuresLionelEric-1.0.84.tar.gz` & `tmp/datastructuresLionelEric-1.0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastructuresLionelEric-1.0.84.tar", last modified: Sun Apr  9 22:28:00 2023, max compression
+gzip compressed data, was "datastructuresLionelEric-1.0.89.tar", last modified: Sun Apr  9 22:33:59 2023, max compression
```

## Comparing `datastructuresLionelEric-1.0.84.tar` & `datastructuresLionelEric-1.0.89.tar`

### file list

```diff
@@ -1,10 +1,58 @@
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:28:00.677659 datastructuresLionelEric-1.0.84/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.84/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      162 2023-04-09 22:28:00.677503 datastructuresLionelEric-1.0.84/PKG-INFO
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:28:00.677305 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      162 2023-04-09 22:28:00.000000 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/PKG-INFO
--rw-r--r--   0 lionelhasan   (501) staff       (20)      210 2023-04-09 22:28:00.000000 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/SOURCES.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:28:00.000000 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/dependency_links.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:28:00.000000 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/top_level.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 22:28:00.677702 datastructuresLionelEric-1.0.84/setup.cfg
--rw-r--r--   0 lionelhasan   (501) staff       (20)      240 2023-04-09 22:27:57.000000 datastructuresLionelEric-1.0.84/setup.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:33:59.026243 datastructuresLionelEric-1.0.89/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.89/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      152 2023-04-09 22:33:59.025989 datastructuresLionelEric-1.0.89/PKG-INFO
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:33:59.013941 datastructuresLionelEric-1.0.89/datastructures/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.89/datastructures/.DS_Store
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:33:59.016269 datastructuresLionelEric-1.0.89/datastructures/Linear/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/CDLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/CSLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/DLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/LLQueue.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-09 22:31:55.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/LLStack.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/SLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:33:59.018605 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8979 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/CDLL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     4716 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     9916 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/CSLL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5162 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8342 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/DLL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     4620 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/DLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2516 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/LLQueue.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1780 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     3403 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/LLStack.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2365 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8307 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/SLL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     4657 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/SLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      199 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      177 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.89/datastructures/Linear/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:33:59.019372 datastructuresLionelEric-1.0.89/datastructures/nodes/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/Dnode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/TNode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:33:59.020808 datastructuresLionelEric-1.0.89/datastructures/nodes/__pycache__/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      629 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/__pycache__/Dnode.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      476 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/__pycache__/Dnode.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2706 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/__pycache__/TNode.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2118 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/__pycache__/TNode.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      198 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.89/datastructures/nodes/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:33:59.021399 datastructuresLionelEric-1.0.89/datastructures/trees/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 22:31:55.000000 datastructuresLionelEric-1.0.89/datastructures/trees/AVL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 22:31:55.000000 datastructuresLionelEric-1.0.89/datastructures/trees/BST.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:33:59.023748 datastructuresLionelEric-1.0.89/datastructures/trees/__pycache__/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5386 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/trees/__pycache__/AVL.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     3696 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.89/datastructures/trees/__pycache__/AVL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6289 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/trees/__pycache__/BST.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     3364 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.89/datastructures/trees/__pycache__/BST.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      198 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/trees/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 22:31:56.000000 datastructuresLionelEric-1.0.89/datastructures/trees/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2809 2023-04-09 22:18:38.000000 datastructuresLionelEric-1.0.89/datastructures/trees/main.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:33:59.025288 datastructuresLionelEric-1.0.89/datastructuresLionelEric.egg-info/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      152 2023-04-09 22:33:58.000000 datastructuresLionelEric-1.0.89/datastructuresLionelEric.egg-info/PKG-INFO
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2099 2023-04-09 22:33:58.000000 datastructuresLionelEric-1.0.89/datastructuresLionelEric.egg-info/SOURCES.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:33:58.000000 datastructuresLionelEric-1.0.89/datastructuresLionelEric.egg-info/dependency_links.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:33:58.000000 datastructuresLionelEric-1.0.89/datastructuresLionelEric.egg-info/top_level.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 22:33:59.026296 datastructuresLionelEric-1.0.89/setup.cfg
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      313 2023-04-09 22:31:09.000000 datastructuresLionelEric-1.0.89/setup.py
```

### Comparing `datastructuresLionelEric-1.0.84/.DS_Store` & `datastructuresLionelEric-1.0.89/.DS_Store`

 * *Files identical despite different names*

