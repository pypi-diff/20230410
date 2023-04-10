# Comparing `tmp/memory_compressed_attention-0.0.5.tar.gz` & `tmp/memory_compressed_attention-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_compressed_attention-0.0.5.tar", last modified: Fri Aug 19 03:03:43 2022, max compression
+gzip compressed data, was "memory_compressed_attention-0.0.6.tar", last modified: Mon Apr 10 03:35:40 2023, max compression
```

## Comparing `memory_compressed_attention-0.0.5.tar` & `memory_compressed_attention-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 03:03:43.383509 memory_compressed_attention-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-19 03:03:35.000000 memory_compressed_attention-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-08-19 03:03:43.383509 memory_compressed_attention-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-08-19 03:03:35.000000 memory_compressed_attention-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 03:03:43.379509 memory_compressed_attention-0.0.5/memory_compressed_attention/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-19 03:03:35.000000 memory_compressed_attention-0.0.5/memory_compressed_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-08-19 03:03:35.000000 memory_compressed_attention-0.0.5/memory_compressed_attention/memory_compressed_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 03:03:43.383509 memory_compressed_attention-0.0.5/memory_compressed_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-08-19 03:03:43.000000 memory_compressed_attention-0.0.5/memory_compressed_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-08-19 03:03:43.000000 memory_compressed_attention-0.0.5/memory_compressed_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 03:03:43.000000 memory_compressed_attention-0.0.5/memory_compressed_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-19 03:03:43.000000 memory_compressed_attention-0.0.5/memory_compressed_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-19 03:03:43.000000 memory_compressed_attention-0.0.5/memory_compressed_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-19 03:03:43.383509 memory_compressed_attention-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-08-19 03:03:35.000000 memory_compressed_attention-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/memory_compressed_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/memory_compressed_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/memory_compressed_attention/memory_compressed_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 03:35:40.000000 memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 03:35:40.700474 memory_compressed_attention-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-10 03:35:28.000000 memory_compressed_attention-0.0.6/setup.py
```

### Comparing `memory_compressed_attention-0.0.5/LICENSE` & `memory_compressed_attention-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `memory_compressed_attention-0.0.5/PKG-INFO` & `memory_compressed_attention-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory_compressed_attention
-Version: 0.0.5
+Version: 0.0.6
 Summary: Memory-Compressed Self Attention
 Home-page: https://github.com/lucidrains/memory-compressed-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory_compressed_attention-0.0.5/README.md` & `memory_compressed_attention-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `memory_compressed_attention-0.0.5/memory_compressed_attention/memory_compressed_attention.py` & `memory_compressed_attention-0.0.6/memory_compressed_attention/memory_compressed_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,13 +92,13 @@
             dots.masked_fill_(~mask, mask_value)
             del mask
 
         # attention
         attn = dots.softmax(dim=-1)
 
         # dropout
-        attn = self.dropout(dots)
+        attn = self.dropout(attn)
         out = torch.einsum('bhij,bhjd->bhid', attn, v)
 
         # split heads and combine
         out = out.transpose(1, 2).reshape(b, t, d)
         return self.to_out(out)
```

### Comparing `memory_compressed_attention-0.0.5/memory_compressed_attention.egg-info/PKG-INFO` & `memory_compressed_attention-0.0.6/memory_compressed_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-compressed-attention
-Version: 0.0.5
+Version: 0.0.6
 Summary: Memory-Compressed Self Attention
 Home-page: https://github.com/lucidrains/memory-compressed-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory_compressed_attention-0.0.5/setup.py` & `memory_compressed_attention-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'memory_compressed_attention',
   packages = find_packages(),
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   description = 'Memory-Compressed Self Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/memory-compressed-attention',
   keywords = ['transformers', 'artificial intelligence', 'attention mechanism'],
```

