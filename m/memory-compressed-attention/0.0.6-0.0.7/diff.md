# Comparing `tmp/memory_compressed_attention-0.0.6.tar.gz` & `tmp/memory_compressed_attention-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_compressed_attention-0.0.6.tar", last modified: Mon Apr 10 03:35:40 2023, max compression
+gzip compressed data, was "memory_compressed_attention-0.0.7.tar", last modified: Mon Apr 10 03:40:03 2023, max compression
```

## Comparing `memory_compressed_attention-0.0.6.tar` & `memory_compressed_attention-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/memory_compressed_attention/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/memory_compressed_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/memory_compressed_attention/memory_compressed_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:40:03.850388 memory_compressed_attention-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 03:39:52.000000 memory_compressed_attention-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-10 03:40:03.850388 memory_compressed_attention-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-10 03:39:52.000000 memory_compressed_attention-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:40:03.850388 memory_compressed_attention-0.0.7/memory_compressed_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 03:39:52.000000 memory_compressed_attention-0.0.7/memory_compressed_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-10 03:39:52.000000 memory_compressed_attention-0.0.7/memory_compressed_attention/memory_compressed_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:40:03.850388 memory_compressed_attention-0.0.7/memory_compressed_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-10 03:40:03.000000 memory_compressed_attention-0.0.7/memory_compressed_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-10 03:40:03.000000 memory_compressed_attention-0.0.7/memory_compressed_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 03:40:03.000000 memory_compressed_attention-0.0.7/memory_compressed_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 03:40:03.000000 memory_compressed_attention-0.0.7/memory_compressed_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 03:40:03.000000 memory_compressed_attention-0.0.7/memory_compressed_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 03:40:03.850388 memory_compressed_attention-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-10 03:39:52.000000 memory_compressed_attention-0.0.7/setup.py
```

### Comparing `memory_compressed_attention-0.0.6/LICENSE` & `memory_compressed_attention-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `memory_compressed_attention-0.0.6/PKG-INFO` & `memory_compressed_attention-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory_compressed_attention
-Version: 0.0.6
+Version: 0.0.7
 Summary: Memory-Compressed Self Attention
 Home-page: https://github.com/lucidrains/memory-compressed-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory_compressed_attention-0.0.6/README.md` & `memory_compressed_attention-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `memory_compressed_attention-0.0.6/memory_compressed_attention/memory_compressed_attention.py` & `memory_compressed_attention-0.0.7/memory_compressed_attention/memory_compressed_attention.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,17 @@
         if padding < cf:
             k, v = map(lambda t: F.pad(t, (0, 0, padding, 0)), (k, v))
 
         # compress keys and values
         k, v = map(self.compress_fn, (k, v))
 
         # attach a null key and value, in the case that the first query has no keys to pay attention to
-        k = torch.cat((self.null_k, k), dim=1)
-        v = torch.cat((self.null_v, v), dim=1)
+        nk, nv = map(lambda t: t.expand(b, -1, -1), (self.null_k, self.null_v))
+        k = torch.cat((nk, k), dim=1)
+        v = torch.cat((nv, v), dim=1)
 
         # merge heads
         q, k, v = map(lambda t: t.reshape(*t.shape[:2], h, -1).transpose(1, 2), (q, k, v))
 
         # attention
         dots = torch.einsum('bhid,bhjd->bhij', q, k) * d ** -0.5
```

### Comparing `memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/PKG-INFO` & `memory_compressed_attention-0.0.7/memory_compressed_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-compressed-attention
-Version: 0.0.6
+Version: 0.0.7
 Summary: Memory-Compressed Self Attention
 Home-page: https://github.com/lucidrains/memory-compressed-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory_compressed_attention-0.0.6/setup.py` & `memory_compressed_attention-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'memory_compressed_attention',
   packages = find_packages(),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'Memory-Compressed Self Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/memory-compressed-attention',
   keywords = ['transformers', 'artificial intelligence', 'attention mechanism'],
```

