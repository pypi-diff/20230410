# Comparing `tmp/voltage_imaging_analysis-0.1.4.tar.gz` & `tmp/voltage_imaging_analysis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltage_imaging_analysis-0.1.4.tar", last modified: Mon Apr 10 18:31:32 2023, max compression
+gzip compressed data, was "voltage_imaging_analysis-0.1.5.tar", last modified: Mon Apr 10 18:42:27 2023, max compression
```

## Comparing `voltage_imaging_analysis-0.1.4.tar` & `voltage_imaging_analysis-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.788876 voltage_imaging_analysis-0.1.4/
--rw-r--r--   0 rrsims     (501) staff       (20)     6148 2023-02-14 19:09:47.000000 voltage_imaging_analysis-0.1.4/.DS_Store
--rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:31:32.788665 voltage_imaging_analysis-0.1.4/PKG-INFO
--rw-r--r--   0 rrsims     (501) staff       (20)      101 2023-02-07 14:38:32.000000 voltage_imaging_analysis-0.1.4/README.md
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.786944 voltage_imaging_analysis-0.1.4/dist/
--rw-r--r--   0 rrsims     (501) staff       (20)     9193 2023-02-07 21:30:21.000000 voltage_imaging_analysis-0.1.4/dist/voltage_imaging_analysis-0.1.0.tar.gz
--rw-r--r--   0 rrsims     (501) staff       (20)       38 2023-04-10 18:31:32.788934 voltage_imaging_analysis-0.1.4/setup.cfg
--rw-r--r--   0 rrsims     (501) staff       (20)      697 2023-04-10 18:31:14.000000 voltage_imaging_analysis-0.1.4/setup.py
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.787434 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/
--rw-r--r--   0 rrsims     (501) staff       (20)      125 2023-02-14 19:08:52.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/__init__.py
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.788307 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/__pycache__/
--rw-r--r--   0 rrsims     (501) staff       (20)      321 2023-02-07 14:49:20.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rrsims     (501) staff       (20)    26949 2023-04-10 13:23:54.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.788154 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/
--rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/PKG-INFO
--rw-r--r--   0 rrsims     (501) staff       (20)      466 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 rrsims     (501) staff       (20)        1 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 rrsims     (501) staff       (20)        6 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/requires.txt
--rw-r--r--   0 rrsims     (501) staff       (20)       25 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:42:27.730404 voltage_imaging_analysis-0.1.5/
+-rw-r--r--   0 rrsims     (501) staff       (20)     6148 2023-04-10 18:39:58.000000 voltage_imaging_analysis-0.1.5/.DS_Store
+-rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:42:27.730207 voltage_imaging_analysis-0.1.5/PKG-INFO
+-rw-r--r--   0 rrsims     (501) staff       (20)      101 2023-02-07 14:38:32.000000 voltage_imaging_analysis-0.1.5/README.md
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:42:27.728317 voltage_imaging_analysis-0.1.5/dist/
+-rw-r--r--   0 rrsims     (501) staff       (20)     9000 2023-04-10 18:40:06.000000 voltage_imaging_analysis-0.1.5/dist/voltage_imaging_analysis-0.1.0.tar.gz
+-rw-r--r--   0 rrsims     (501) staff       (20)       38 2023-04-10 18:42:27.730457 voltage_imaging_analysis-0.1.5/setup.cfg
+-rw-r--r--   0 rrsims     (501) staff       (20)      697 2023-04-10 18:42:19.000000 voltage_imaging_analysis-0.1.5/setup.py
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:42:27.729006 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis/
+-rw-r--r--   0 rrsims     (501) staff       (20)      125 2023-04-10 18:39:53.000000 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis/__init__.py
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:42:27.729856 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis/__pycache__/
+-rw-r--r--   0 rrsims     (501) staff       (20)      321 2023-02-07 14:49:20.000000 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rrsims     (501) staff       (20)    10975 2023-04-10 18:39:13.000000 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis/test_1p_analysis.py
+-rw-r--r--   0 rrsims     (501) staff       (20)    29251 2023-04-10 18:39:39.000000 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:42:27.729672 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis.egg-info/
+-rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:42:27.000000 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 rrsims     (501) staff       (20)      511 2023-04-10 18:42:27.000000 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 rrsims     (501) staff       (20)        1 2023-04-10 18:42:27.000000 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 rrsims     (501) staff       (20)        6 2023-04-10 18:42:27.000000 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis.egg-info/requires.txt
+-rw-r--r--   0 rrsims     (501) staff       (20)       25 2023-04-10 18:42:27.000000 voltage_imaging_analysis-0.1.5/voltage_imaging_analysis.egg-info/top_level.txt
```

### Comparing `voltage_imaging_analysis-0.1.4/setup.py` & `voltage_imaging_analysis-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='voltage_imaging_analysis',
-    version='0.1.4',    
+    version='0.1.5',    
     description='Python package used for analysing voltage imaging data.',
     url='https://github.com/rrsims21/voltage_imaging_analysis/',
     author='Ruth Sims',
     author_email='ruth.sims@inserm.fr',
     license='BSD 2-clause',
     packages=['voltage_imaging_analysis'],
     install_requires=[
```

### Comparing `voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py` & `voltage_imaging_analysis-0.1.5/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     if to_whiten_data is True:
         whitened_data = whiten_data(data)
     else:
         whitened_data = data
 
     if no_neighbours==4:
         sz = np.array([[0, 1, 0], [1, 0, 1], [0, 1, 0]]).astype(np.float32)
+        
     if no_neighbours==8:
         sz = np.ones((3, 3)).astype(np.float32)
         sz[1, 1] = 0
 
     if no_neighbours==24:
         sz = np.ones((5, 5)).astype(np.float32)
         sz[2, 2] = 0
@@ -664,8 +665,81 @@
     lag = trace.shape[0] - np.argmax(corr)
 
     if lag < 0:
         trace = np.lib.pad(trace, (0, -1*lag))[-lag:]
     if lag > 0:
         trace = np.lib.pad(trace, (lag, 0))[:-lag]
     
-    return trace, lag
+    return trace, lag
+
+class R_pca:
+    """Class which implements R_pca to decompose matrix into low rank (L) and sparse (S) components.
+
+    Args:
+        D: array to be decomposed
+        mu: not sure
+        lmbda: not sure
+    
+    Returns:
+        resized array a
+    
+    Raises:
+
+    """
+
+    def __init__(self, D, mu=None, lmbda=None):
+        self.D = D
+        self.S = np.zeros(self.D.shape)
+        self.Y = np.zeros(self.D.shape)
+
+        if mu:
+            self.mu = mu
+        else:
+            self.mu = np.prod(self.D.shape) / (4 * np.linalg.norm(self.D, ord=1))
+
+        self.mu_inv = 1 / self.mu
+
+        if lmbda:
+            self.lmbda = lmbda
+        else:
+            self.lmbda = 1 / np.sqrt(np.max(self.D.shape))
+
+    @staticmethod
+    def frobenius_norm(M):
+        return np.linalg.norm(M, ord='fro')
+
+    @staticmethod
+    def shrink(M, tau):
+        return np.sign(M) * np.maximum((np.abs(M) - tau), np.zeros(M.shape))
+
+    def svd_threshold(self, M, tau):
+        U, S, V = np.linalg.svd(M, full_matrices=False)
+        return np.dot(U, np.dot(np.diag(self.shrink(S, tau)), V))
+
+    def fit(self, tol=None, max_iter=1000, iter_print=100):
+        iter = 0
+        err = np.Inf
+        Sk = self.S
+        Yk = self.Y
+        Lk = np.zeros(self.D.shape)
+
+        if tol:
+            _tol = tol
+        else:
+            _tol = 1E-7 * self.frobenius_norm(self.D)
+
+        #this loop implements the principal component pursuit (PCP) algorithm
+        #located in the table on page 29 of https://arxiv.org/pdf/0912.3599.pdf
+        while (err > _tol) and iter < max_iter:
+            Lk = self.svd_threshold(
+                self.D - Sk + self.mu_inv * Yk, self.mu_inv)                            #this line implements step 3
+            Sk = self.shrink(
+                self.D - Lk + (self.mu_inv * Yk), self.mu_inv * self.lmbda)             #this line implements step 4
+            Yk = Yk + self.mu * (self.D - Lk - Sk)                                      #this line implements step 5
+            err = self.frobenius_norm(self.D - Lk - Sk)
+            iter += 1
+            if (iter % iter_print) == 0 or iter == 1 or iter > max_iter or err <= _tol:
+                print('iteration: {0}, error: {1}'.format(iter, err))
+
+        self.L = Lk
+        self.S = Sk
+        return Lk, Sk
```

