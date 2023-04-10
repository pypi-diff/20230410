# Comparing `tmp/chunkdot-0.1.4.tar.gz` & `tmp/chunkdot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunkdot-0.1.4.tar", max compression
+gzip compressed data, was "chunkdot-0.1.5.tar", max compression
```

## Comparing `chunkdot-0.1.4.tar` & `chunkdot-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1129 2023-03-31 03:15:29.624003 chunkdot-0.1.4/README.md
--rw-r--r--   0        0        0      131 2023-03-31 06:44:44.933244 chunkdot-0.1.4/chunkdot/__init__.py
--rw-r--r--   0        0        0     3251 2023-03-28 22:49:05.870063 chunkdot-0.1.4/chunkdot/chunkdot.py
--rw-r--r--   0        0        0     3212 2023-03-31 06:43:23.566757 chunkdot-0.1.4/chunkdot/cosine_similarity_top_k.py
--rw-r--r--   0        0        0     4094 2023-03-08 12:19:56.965969 chunkdot-0.1.4/chunkdot/numba_argpartition.py
--rw-r--r--   0        0        0     3964 2023-03-31 03:01:38.405020 chunkdot-0.1.4/chunkdot/utils.py
--rw-r--r--   0        0        0      786 2023-03-31 06:44:44.124110 chunkdot-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 chunkdot-0.1.4/setup.py
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 chunkdot-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1129 2023-03-31 03:15:29.624003 chunkdot-0.1.5/README.md
+-rw-r--r--   0        0        0      131 2023-04-10 13:20:40.268489 chunkdot-0.1.5/chunkdot/__init__.py
+-rw-r--r--   0        0        0     3251 2023-03-28 22:49:05.870063 chunkdot-0.1.5/chunkdot/chunkdot.py
+-rw-r--r--   0        0        0     3212 2023-03-31 06:43:23.566757 chunkdot-0.1.5/chunkdot/cosine_similarity_top_k.py
+-rw-r--r--   0        0        0     4094 2023-03-08 12:19:56.965969 chunkdot-0.1.5/chunkdot/numba_argpartition.py
+-rw-r--r--   0        0        0     3964 2023-03-31 03:01:38.405020 chunkdot-0.1.5/chunkdot/utils.py
+-rw-r--r--   0        0        0     1002 2023-04-10 13:20:39.585166 chunkdot-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 chunkdot-0.1.5/setup.py
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 chunkdot-0.1.5/PKG-INFO
```

### Comparing `chunkdot-0.1.4/README.md` & `chunkdot-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `chunkdot-0.1.4/chunkdot/chunkdot.py` & `chunkdot-0.1.5/chunkdot/chunkdot.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.1.4/chunkdot/cosine_similarity_top_k.py` & `chunkdot-0.1.5/chunkdot/cosine_similarity_top_k.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.1.4/chunkdot/numba_argpartition.py` & `chunkdot-0.1.5/chunkdot/numba_argpartition.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.1.4/chunkdot/utils.py` & `chunkdot-0.1.5/chunkdot/utils.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.1.4/setup.py` & `chunkdot-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['numba>=0.56.4,<0.57.0', 'numpy>=1.23,<2.0', 'scipy>=1.10.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'chunkdot',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Multi-threaded matrix multiplication and cosine similarity calculations.',
     'long_description': "# ChunkDot\n\nMulti-threaded matrix multiplication and cosine similarity calculations. Appropriate for the calculation of the K most similar items for a large number of items (~1 Million) by partitioning the item matrix representation (embeddings) and using Numba to accelerate the calculations.\n\n## Usage\n\n```bash\npip install -U chunkdot\n```\n\nCalculate the 50 most similar and dissimilar items for 100K items.\n\n```python\nimport numpy as np\nfrom chunkdot import cosine_similarity_top_k\n\nembeddings = np.random.randn(100000, 256)\n# using all you system's memory\ncosine_similarity_top_k(embeddings, top_k=50)\n# most dissimilar items using 20GB\ncosine_similarity_top_k(embeddings, top_k=-50, max_memory=20E9)\n```\n```\n<100000x100000 sparse matrix of type '<class 'numpy.float64'>'\n with 5000000 stored elements in Compressed Sparse Row format>\n```\n\n## The execution time\n\n```python\nfrom timeit import timeit\nimport numpy as np\nfrom chunkdot import cosine_similarity_top_k\n\nembeddings = np.random.randn(100000, 256)\ntimeit(lambda: cosine_similarity_top_k(embeddings, top_k=50, max_memory=20E9), number=1)\n```\n```\n58.611996899999994\n```\n",
     'author': 'Rodrigo Agundez',
     'author_email': 'rragundez@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/rragundez/chunkdot',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
+    'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `chunkdot-0.1.4/PKG-INFO` & `chunkdot-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: chunkdot
-Version: 0.1.4
+Version: 0.1.5
 Summary: Multi-threaded matrix multiplication and cosine similarity calculations.
+Home-page: https://github.com/rragundez/chunkdot
 Author: Rodrigo Agundez
 Author-email: rragundez@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.11
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Project-URL: Repository, https://github.com/rragundez/chunkdot
 Description-Content-Type: text/markdown
 
 # ChunkDot
 
 Multi-threaded matrix multiplication and cosine similarity calculations. Appropriate for the calculation of the K most similar items for a large number of items (~1 Million) by partitioning the item matrix representation (embeddings) and using Numba to accelerate the calculations.
 
 ## Usage
```

