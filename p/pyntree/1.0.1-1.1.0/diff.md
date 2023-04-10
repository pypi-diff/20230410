# Comparing `tmp/pyntree-1.0.1.tar.gz` & `tmp/pyntree-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntree-1.0.1.tar", last modified: Tue Apr  4 12:50:57 2023, max compression
+gzip compressed data, was "pyntree-1.1.0.tar", last modified: Mon Apr 10 21:49:51 2023, max compression
```

## Comparing `pyntree-1.0.1.tar` & `pyntree-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-04 12:50:57.627792 pyntree-1.0.1/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11357 2023-03-27 17:16:15.000000 pyntree-1.0.1/LICENSE.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-04-04 12:50:57.627792 pyntree-1.0.1/PKG-INFO
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1585 2023-03-29 03:58:07.000000 pyntree-1.0.1/README.md
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-04 12:50:57.623792 pyntree-1.0.1/pyntree/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     6627 2023-04-03 21:05:08.000000 pyntree-1.0.1/pyntree/__init__.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1128 2023-03-29 03:58:07.000000 pyntree-1.0.1/pyntree/encryption.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      165 2023-04-03 21:05:08.000000 pyntree-1.0.1/pyntree/errors.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     6259 2023-03-29 03:58:07.000000 pyntree-1.0.1/pyntree/file.py
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-04 12:50:57.623792 pyntree-1.0.1/pyntree.egg-info/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-04-04 12:50:57.000000 pyntree-1.0.1/pyntree.egg-info/PKG-INFO
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      298 2023-04-04 12:50:57.000000 pyntree-1.0.1/pyntree.egg-info/SOURCES.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        1 2023-04-04 12:50:57.000000 pyntree-1.0.1/pyntree.egg-info/dependency_links.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      117 2023-04-04 12:50:57.000000 pyntree-1.0.1/pyntree.egg-info/requires.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        8 2023-04-04 12:50:57.000000 pyntree-1.0.1/pyntree.egg-info/top_level.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1298 2023-04-04 12:50:33.000000 pyntree-1.0.1/pyproject.toml
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       23 2023-03-27 16:14:00.000000 pyntree-1.0.1/requirements.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       38 2023-04-04 12:50:57.627792 pyntree-1.0.1/setup.cfg
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-04 12:50:57.627792 pyntree-1.0.1/tests/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     8609 2023-04-04 12:48:59.000000 pyntree-1.0.1/tests/tests.py
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-10 21:49:51.862145 pyntree-1.1.0/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11357 2023-03-27 17:16:15.000000 pyntree-1.1.0/LICENSE.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-04-10 21:49:51.862145 pyntree-1.1.0/PKG-INFO
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1585 2023-03-29 03:58:07.000000 pyntree-1.1.0/README.md
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-10 21:49:51.858145 pyntree-1.1.0/pyntree/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     8585 2023-04-10 21:45:07.000000 pyntree-1.1.0/pyntree/__init__.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1128 2023-03-29 03:58:07.000000 pyntree-1.1.0/pyntree/encryption.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      166 2023-04-10 21:40:01.000000 pyntree-1.1.0/pyntree/errors.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     6259 2023-03-29 03:58:07.000000 pyntree-1.1.0/pyntree/file.py
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-10 21:49:51.858145 pyntree-1.1.0/pyntree.egg-info/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/PKG-INFO
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      298 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/SOURCES.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        1 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/dependency_links.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      117 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/requires.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        8 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/top_level.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1298 2023-04-10 21:49:29.000000 pyntree-1.1.0/pyproject.toml
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       23 2023-03-27 16:14:00.000000 pyntree-1.1.0/requirements.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       38 2023-04-10 21:49:51.862145 pyntree-1.1.0/setup.cfg
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-10 21:49:51.858145 pyntree-1.1.0/tests/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    10991 2023-04-10 21:47:23.000000 pyntree-1.1.0/tests/tests.py
```

### Comparing `pyntree-1.0.1/LICENSE.txt` & `pyntree-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyntree-1.0.1/PKG-INFO` & `pyntree-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntree
-Version: 1.0.1
+Version: 1.1.0
 Summary: pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters.
 Author-email: jvadair <dev@jvadair.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyntree-1.0.1/README.md` & `pyntree-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyntree-1.0.1/pyntree/encryption.py` & `pyntree-1.1.0/pyntree/encryption.py`

 * *Files identical despite different names*

### Comparing `pyntree-1.0.1/pyntree/file.py` & `pyntree-1.1.0/pyntree/file.py`

 * *Files identical despite different names*

### Comparing `pyntree-1.0.1/pyntree.egg-info/PKG-INFO` & `pyntree-1.1.0/pyntree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntree
-Version: 1.0.1
+Version: 1.1.0
 Summary: pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters.
 Author-email: jvadair <dev@jvadair.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyntree-1.0.1/pyproject.toml` & `pyntree-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["dependencies"]
 name = "pyntree"
-version = "1.0.1"
+version = "1.1.0"
 description = "pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters."
 readme = "README.md"
 authors = [{ name = "jvadair", email = "dev@jvadair.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `pyntree-1.0.1/tests/tests.py` & `pyntree-1.1.0/tests/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -190,14 +190,29 @@
         os.remove('tests/testing_savedict.json')
 
     def test_node_in_node(self):
         db = Node({'a': Node()})
         db.save('tests/testing_save_NiN.pyn')
         os.remove('tests/testing_save_NiN.pyn')
 
+    def test_save_after_password_set(self):
+        db = Node({'a': 'b'})
+        db.file.password = 'testing'
+        db.save('tests/testing_encrypted_setpwd.pyn')
+        self.assertEqual(Node('tests/testing_encrypted_setpwd.pyn', password='testing')(), {'a': 'b'})
+        os.remove('tests/testing_encrypted_setpwd.pyn')
+
+    def test_save_after_password_change(self):
+        db = Node('tests/testing_encrypted_changepwd.pyn', password='testing1')
+        db.a = 'b'
+        db.file.password = 'testing2'
+        db.save('tests/testing_encrypted_changepwd.pyn')
+        self.assertEqual(Node('tests/testing_encrypted_changepwd.pyn', password='testing2')(), {'a': 'b'})
+        os.remove('tests/testing_encrypted_changepwd.pyn')
+
 
 class DeletionTests(unittest.TestCase):
     def test_layer_0(self):
         db = Node({'a': {'b': {'c': 'd'}}, 'b': "test"})
         db.delete()
         self.assertEqual(db(), {})
 
@@ -258,13 +273,85 @@
 
     def test_name_layer_0_file(self):
         self.assertEqual(Node('tests/sample.txt')._name, 'tests/sample.txt')
 
     def test_name_layer_1(self):
         self.assertEqual(self.db.val1._name, 'val1')
 
+    def test_get_children(self):
+        self.assertEqual(self.db._children[0](), 'h')
+
+    def test_where(self):
+        db = Node({
+            "a": {
+                "b": 2
+            },
+            "b": {
+                "b": 2
+            },
+            "c": {
+                "b": 3
+            }
+        })
+        matches = db.where(b=2)
+        self.assertEqual(len(matches), 2)
+        self.assertTrue(type(matches[0]) is Node)
+        self.assertEqual(str(matches[0]), str({"b": 2}))
+
+    def test_containing(self):
+        db = Node({
+            "a": {
+                "h": 2
+            },
+            "b": {
+                "b": 2
+            },
+            "c": {
+                "b": 3
+            }
+        })
+        matches = db.containing('b')
+        self.assertEqual(len(matches), 2)
+        self.assertTrue(type(matches[0]) is Node)
+        self.assertEqual(str(matches[0]), str({"b": 2}))
+
     def test_getdict(self):
-        self.assertEqual(str(dict(self.db)), str({'val1': 'h', 'val2': 'b'}))
+        db = Node({'a': {'b': {'c': 1}}})
+        self.assertEqual(str(dict(db)), str({'a': {'b': {'c': 1}}}))
+
+
+# noinspection PyCallingNonCallable
+class ArithmeticTests(unittest.TestCase):
+    def test_iadd_int(self):
+        db = Node()
+        db.a = 1
+        db.a += 1
+        self.assertEqual(db.a(), 2)
+
+    def test_iadd_str(self):
+        db = Node()
+        db.a = 'a'
+        db.a += 'bc'
+        self.assertEqual(db.a(), 'abc')
+
+    def test_isub_int(self):
+        db = Node()
+        db.a = 1
+        db.a -= 1
+        self.assertEqual(db.a(), 0)
+
+    def test_imul_int(self):
+        db = Node()
+        db.a = 2
+        db.a *= 3
+        self.assertEqual(db.a(), 6)
+
+    def test_imul_str(self):
+        db = Node()
+        db.a = 'a'
+        db.a *= 3
+        self.assertEqual(db.a(), 'aaa')
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

