# Comparing `tmp/lmah88-1.1.tar.gz` & `tmp/lmah88-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmah88-1.1.tar", last modified: Sun Apr  9 20:06:46 2023, max compression
+gzip compressed data, was "lmah88-1.4.tar", last modified: Mon Apr 10 01:18:23 2023, max compression
```

## Comparing `lmah88-1.1.tar` & `lmah88-1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 20:06:46.558764 lmah88-1.1/
-drwxrwxrwx   0        0        0        0 2023-04-09 20:06:46.511886 lmah88-1.1/Linear/
--rw-rw-rw-   0        0        0     4154 2023-04-09 06:11:13.000000 lmah88-1.1/Linear/DoublyCLL.py
--rw-rw-rw-   0        0        0     8673 2023-04-09 06:11:13.000000 lmah88-1.1/Linear/DoublyLL.py
--rw-rw-rw-   0        0        0     2272 2023-04-09 06:11:13.000000 lmah88-1.1/Linear/LLQueue.py
--rw-rw-rw-   0        0        0     1981 2023-04-08 00:28:46.000000 lmah88-1.1/Linear/LLStack.py
--rw-rw-rw-   0        0        0     4109 2023-04-09 06:11:13.000000 lmah88-1.1/Linear/SinglyCLL.py
--rw-rw-rw-   0        0        0     7497 2023-04-08 00:28:46.000000 lmah88-1.1/Linear/SinglyLL.py
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 lmah88-1.1/Linear/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:06:46.511886 lmah88-1.1/Nodes/
--rw-rw-rw-   0        0        0      122 2023-04-07 16:51:25.000000 lmah88-1.1/Nodes/DoublyNode.py
--rw-rw-rw-   0        0        0      105 2023-04-07 16:51:25.000000 lmah88-1.1/Nodes/SinglyNode.py
--rw-rw-rw-   0        0        0     1813 2023-04-09 06:11:17.000000 lmah88-1.1/Nodes/TNode.py
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 lmah88-1.1/Nodes/__init__.py
--rw-rw-rw-   0        0        0      111 2023-04-09 20:06:46.558764 lmah88-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 20:06:46.511886 lmah88-1.1/Trees/
--rw-rw-rw-   0        0        0     8802 2023-04-09 06:11:17.000000 lmah88-1.1/Trees/AVL.py
--rw-rw-rw-   0        0        0     4950 2023-04-09 06:11:17.000000 lmah88-1.1/Trees/BST.py
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 lmah88-1.1/Trees/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:06:46.543141 lmah88-1.1/lmah88.egg-info/
--rw-rw-rw-   0        0        0      111 2023-04-09 20:06:46.000000 lmah88-1.1/lmah88.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-04-09 20:06:46.000000 lmah88-1.1/lmah88.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 20:06:46.000000 lmah88-1.1/lmah88.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-09 20:06:46.000000 lmah88-1.1/lmah88.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 20:06:46.558764 lmah88-1.1/setup.cfg
--rw-rw-rw-   0        0        0      260 2023-04-09 20:06:39.000000 lmah88-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:06:46.558764 lmah88-1.1/test/
--rw-rw-rw-   0        0        0    10058 2023-04-09 17:14:55.000000 lmah88-1.1/test/AVL_test.py
--rw-rw-rw-   0        0        0     4790 2023-04-09 06:11:13.000000 lmah88-1.1/test/BST_test.py
--rw-rw-rw-   0        0        0     5959 2023-04-09 06:11:13.000000 lmah88-1.1/test/DoublyCLL_test.py
--rw-rw-rw-   0        0        0     4900 2023-04-09 06:11:13.000000 lmah88-1.1/test/DoublyLL_test.py
--rw-rw-rw-   0        0        0     3937 2023-04-09 06:11:13.000000 lmah88-1.1/test/LLQueue_test.py
--rw-rw-rw-   0        0        0     4010 2023-04-09 06:11:13.000000 lmah88-1.1/test/LLStack_test.py
--rw-rw-rw-   0        0        0     5679 2023-04-09 06:11:13.000000 lmah88-1.1/test/SinglyCLL_test.py
--rw-rw-rw-   0        0        0     5820 2023-04-09 06:11:13.000000 lmah88-1.1/test/SinglyLL_test.py
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 lmah88-1.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:18:23.873898 lmah88-1.4/
+drwxrwxrwx   0        0        0        0 2023-04-10 01:18:23.811391 lmah88-1.4/Linear/
+-rw-rw-rw-   0        0        0     4154 2023-04-09 06:11:13.000000 lmah88-1.4/Linear/DoublyCLL.py
+-rw-rw-rw-   0        0        0     8673 2023-04-09 06:11:13.000000 lmah88-1.4/Linear/DoublyLL.py
+-rw-rw-rw-   0        0        0     2272 2023-04-09 06:11:13.000000 lmah88-1.4/Linear/LLQueue.py
+-rw-rw-rw-   0        0        0     1981 2023-04-08 00:28:46.000000 lmah88-1.4/Linear/LLStack.py
+-rw-rw-rw-   0        0        0     4109 2023-04-09 06:11:13.000000 lmah88-1.4/Linear/SinglyCLL.py
+-rw-rw-rw-   0        0        0     7497 2023-04-08 00:28:46.000000 lmah88-1.4/Linear/SinglyLL.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 lmah88-1.4/Linear/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:18:23.811391 lmah88-1.4/Nodes/
+-rw-rw-rw-   0        0        0      122 2023-04-07 16:51:25.000000 lmah88-1.4/Nodes/DoublyNode.py
+-rw-rw-rw-   0        0        0      105 2023-04-07 16:51:25.000000 lmah88-1.4/Nodes/SinglyNode.py
+-rw-rw-rw-   0        0        0     1813 2023-04-09 06:11:17.000000 lmah88-1.4/Nodes/TNode.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 lmah88-1.4/Nodes/__init__.py
+-rw-rw-rw-   0        0        0      111 2023-04-10 01:18:23.873898 lmah88-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 01:18:23.827015 lmah88-1.4/Trees/
+-rw-rw-rw-   0        0        0     8802 2023-04-09 06:11:17.000000 lmah88-1.4/Trees/AVL.py
+-rw-rw-rw-   0        0        0     4950 2023-04-09 06:11:17.000000 lmah88-1.4/Trees/BST.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 lmah88-1.4/Trees/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:18:23.842642 lmah88-1.4/lmah88.egg-info/
+-rw-rw-rw-   0        0        0      111 2023-04-10 01:18:23.000000 lmah88-1.4/lmah88.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2023-04-10 01:18:23.000000 lmah88-1.4/lmah88.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:18:23.000000 lmah88-1.4/lmah88.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-10 01:18:23.000000 lmah88-1.4/lmah88.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 01:18:23.889525 lmah88-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      260 2023-04-10 01:18:09.000000 lmah88-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:18:23.873898 lmah88-1.4/test/
+-rw-rw-rw-   0        0        0    10058 2023-04-09 17:14:55.000000 lmah88-1.4/test/AVL_test.py
+-rw-rw-rw-   0        0        0     4790 2023-04-09 06:11:13.000000 lmah88-1.4/test/BST_test.py
+-rw-rw-rw-   0        0        0     5959 2023-04-09 06:11:13.000000 lmah88-1.4/test/DoublyCLL_test.py
+-rw-rw-rw-   0        0        0     4900 2023-04-09 06:11:13.000000 lmah88-1.4/test/DoublyLL_test.py
+-rw-rw-rw-   0        0        0     3937 2023-04-09 06:11:13.000000 lmah88-1.4/test/LLQueue_test.py
+-rw-rw-rw-   0        0        0     4010 2023-04-09 06:11:13.000000 lmah88-1.4/test/LLStack_test.py
+-rw-rw-rw-   0        0        0     5679 2023-04-09 06:11:13.000000 lmah88-1.4/test/SinglyCLL_test.py
+-rw-rw-rw-   0        0        0     5820 2023-04-09 06:11:13.000000 lmah88-1.4/test/SinglyLL_test.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 lmah88-1.4/test/__init__.py
```

### Comparing `lmah88-1.1/Linear/DoublyCLL.py` & `lmah88-1.4/Linear/DoublyCLL.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/Linear/DoublyLL.py` & `lmah88-1.4/Linear/DoublyLL.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/Linear/LLQueue.py` & `lmah88-1.4/Linear/LLQueue.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/Linear/LLStack.py` & `lmah88-1.4/Linear/LLStack.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/Linear/SinglyCLL.py` & `lmah88-1.4/Linear/SinglyCLL.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/Linear/SinglyLL.py` & `lmah88-1.4/Linear/SinglyLL.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/Nodes/TNode.py` & `lmah88-1.4/Nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/Trees/AVL.py` & `lmah88-1.4/Trees/AVL.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/Trees/BST.py` & `lmah88-1.4/Trees/BST.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/lmah88.egg-info/SOURCES.txt` & `lmah88-1.4/lmah88.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/test/AVL_test.py` & `lmah88-1.4/test/AVL_test.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/test/BST_test.py` & `lmah88-1.4/test/BST_test.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/test/DoublyCLL_test.py` & `lmah88-1.4/test/DoublyCLL_test.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/test/DoublyLL_test.py` & `lmah88-1.4/test/DoublyLL_test.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/test/LLQueue_test.py` & `lmah88-1.4/test/LLQueue_test.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/test/LLStack_test.py` & `lmah88-1.4/test/LLStack_test.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/test/SinglyCLL_test.py` & `lmah88-1.4/test/SinglyCLL_test.py`

 * *Files identical despite different names*

### Comparing `lmah88-1.1/test/SinglyLL_test.py` & `lmah88-1.4/test/SinglyLL_test.py`

 * *Files identical despite different names*

