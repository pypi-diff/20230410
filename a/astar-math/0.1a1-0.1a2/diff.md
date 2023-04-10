# Comparing `tmp/astar-math-0.1a1.tar.gz` & `tmp/astar-math-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astar-math-0.1a1.tar", last modified: Sat Mar  5 08:05:34 2022, max compression
+gzip compressed data, was "astar-math-0.1a2.tar", last modified: Sun Mar  6 08:51:13 2022, max compression
```

## Comparing `astar-math-0.1a1.tar` & `astar-math-0.1a2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-03-05 08:05:34.192476 astar-math-0.1a1/
--rw-rw-rw-   0        0        0    11558 2022-03-05 06:27:52.000000 astar-math-0.1a1/LICENSE
--rw-rw-rw-   0        0        0     1846 2022-03-05 08:05:34.191497 astar-math-0.1a1/PKG-INFO
--rw-rw-rw-   0        0        0      653 2022-03-05 07:27:38.000000 astar-math-0.1a1/README.md
-drwxrwxrwx   0        0        0        0 2022-03-05 08:05:34.170535 astar-math-0.1a1/astar_math/
--rw-rw-rw-   0        0        0      180 2022-03-05 07:53:17.000000 astar-math-0.1a1/astar_math/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-05 08:05:34.185634 astar-math-0.1a1/astar_math/linear_algebra/
--rw-rw-rw-   0        0        0       25 2022-03-05 07:21:38.000000 astar-math-0.1a1/astar_math/linear_algebra/__init__.py
--rw-rw-rw-   0        0        0     3387 2022-03-05 07:14:09.000000 astar-math-0.1a1/astar_math/linear_algebra/matrix.py
-drwxrwxrwx   0        0        0        0 2022-03-05 08:05:34.188487 astar-math-0.1a1/astar_math/test/
--rw-rw-rw-   0        0        0       27 2022-03-05 07:27:38.000000 astar-math-0.1a1/astar_math/test/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-05 08:05:34.181504 astar-math-0.1a1/astar_math.egg-info/
--rw-rw-rw-   0        0        0     1846 2022-03-05 08:05:33.000000 astar-math-0.1a1/astar_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2022-03-05 08:05:34.000000 astar-math-0.1a1/astar_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-05 08:05:33.000000 astar-math-0.1a1/astar_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-03-05 08:05:33.000000 astar-math-0.1a1/astar_math.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-03-05 08:05:33.000000 astar-math-0.1a1/astar_math.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-05 08:05:34.192476 astar-math-0.1a1/setup.cfg
--rw-rw-rw-   0        0        0     1419 2022-03-05 08:05:16.000000 astar-math-0.1a1/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-06 08:51:13.462553 astar-math-0.1a2/
+-rw-rw-rw-   0        0        0    11558 2022-03-05 06:27:52.000000 astar-math-0.1a2/LICENSE
+-rw-rw-rw-   0        0        0     1846 2022-03-06 08:51:13.459559 astar-math-0.1a2/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2022-03-05 07:27:38.000000 astar-math-0.1a2/README.md
+drwxrwxrwx   0        0        0        0 2022-03-06 08:51:13.407686 astar-math-0.1a2/astar_math/
+-rw-rw-rw-   0        0        0      180 2022-03-06 08:48:59.000000 astar-math-0.1a2/astar_math/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-06 08:51:13.419618 astar-math-0.1a2/astar_math/linear_algebra/
+-rw-rw-rw-   0        0        0       25 2022-03-05 07:21:38.000000 astar-math-0.1a2/astar_math/linear_algebra/__init__.py
+-rw-rw-rw-   0        0        0     3427 2022-03-06 08:50:03.000000 astar-math-0.1a2/astar_math/linear_algebra/matrix.py
+drwxrwxrwx   0        0        0        0 2022-03-06 08:51:13.423607 astar-math-0.1a2/astar_math/random/
+-rw-rw-rw-   0        0        0       25 2022-03-05 08:24:39.000000 astar-math-0.1a2/astar_math/random/__init__.py
+-rw-rw-rw-   0        0        0     2653 2022-03-05 08:25:10.000000 astar-math-0.1a2/astar_math/random/random.py
+drwxrwxrwx   0        0        0        0 2022-03-06 08:51:13.453575 astar-math-0.1a2/astar_math/test/
+-rw-rw-rw-   0        0        0       27 2022-03-05 07:27:38.000000 astar-math-0.1a2/astar_math/test/__init__.py
+-rw-rw-rw-   0        0        0     3523 2022-03-06 08:48:59.000000 astar-math-0.1a2/astar_math/test/test_matrix.py
+drwxrwxrwx   0        0        0        0 2022-03-06 08:51:13.416626 astar-math-0.1a2/astar_math.egg-info/
+-rw-rw-rw-   0        0        0     1846 2022-03-06 08:51:13.000000 astar-math-0.1a2/astar_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2022-03-06 08:51:13.000000 astar-math-0.1a2/astar_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-06 08:51:13.000000 astar-math-0.1a2/astar_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2022-03-06 08:51:13.000000 astar-math-0.1a2/astar_math.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-03-06 08:51:13.000000 astar-math-0.1a2/astar_math.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-03-06 08:51:13.463549 astar-math-0.1a2/setup.cfg
+-rw-rw-rw-   0        0        0     1419 2022-03-05 08:05:16.000000 astar-math-0.1a2/setup.py
```

### Comparing `astar-math-0.1a1/LICENSE` & `astar-math-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `astar-math-0.1a1/PKG-INFO` & `astar-math-0.1a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astar-math
-Version: 0.1a1
+Version: 0.1a2
 Summary: Python math
 Home-page: https://gitee.com/hoops/astar-mathtool
 Author: A.Star
 Author-email: astar@snowland.ltd
 Maintainer: A.Star
 Maintainer-email: astar@snowland.ltd
 License: Apache v2.0 License
```

### Comparing `astar-math-0.1a1/README.md` & `astar-math-0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `astar-math-0.1a1/astar_math/linear_algebra/matrix.py` & `astar-math-0.1a2/astar_math/linear_algebra/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,36 +19,37 @@
         result2: 表示0解，若无，表示无解
     """
     size_x, size_y = a.shape
     if len(b.shape) == 1:
         vector_b = np.expand_dims(b, 1)
     else:
         vector_b = b
+    assert size_x == vector_b.shape[0]
     rank_a = matrix_rank(a)
     if np.allclose(b, 0):
         # 齐次线性方程组
-        if rank_a < size_x:
+        if rank_a < size_y:
             # 存在无穷解
             A_mat = a
             index = np.argmax(~np.isclose(A_mat, 0), axis=1)
-            pivot_variable = np.zeros(size_y, dtype=bool)
-            pivot_variable[index] = True
+            pivot_variable = np.ones(size_y, dtype=bool)
+            pivot_variable[index] = False
             free_variable = ~pivot_variable
             free_variable_index = np.where(free_variable)[0]
             fai = np.empty((size_y, size_y - rank_a))
             for i, free_ind in enumerate(free_variable_index):
                 fai_i = np.zeros((size_y, 1))
                 fai_i[free_ind, 0] = 1
                 fai_i[pivot_variable, :1] = inv(A_mat[:rank_a, pivot_variable]) @ (
                     -A_mat[:rank_a, free_ind:free_ind + 1])
                 fai[:, i] = fai_i[:, 0]
-            return True, fai, np.empty((size_x, 0))
+            return True, fai, np.zeros((size_y, 1))
         else:
             # 仅仅存在0解
-            return True, np.empty((size_x, 0)), np.zeros((size_x, 1))
+            return True, np.empty((size_y, 0)), np.zeros((size_y, 1))
     else:
         # 非齐次线性方程组
         extend_a = np.hstack((a, vector_b))
         rank_ex = matrix_rank(extend_a)
         if rank_a < rank_ex:
             # 无解
             return False, np.empty((size_y, 0)), np.empty((size_y, 0))
```

### Comparing `astar-math-0.1a1/astar_math.egg-info/PKG-INFO` & `astar-math-0.1a2/astar_math.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astar-math
-Version: 0.1a1
+Version: 0.1a2
 Summary: Python math
 Home-page: https://gitee.com/hoops/astar-mathtool
 Author: A.Star
 Author-email: astar@snowland.ltd
 Maintainer: A.Star
 Maintainer-email: astar@snowland.ltd
 License: Apache v2.0 License
```

### Comparing `astar-math-0.1a1/setup.py` & `astar-math-0.1a2/setup.py`

 * *Files identical despite different names*

