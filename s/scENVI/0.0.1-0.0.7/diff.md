# Comparing `tmp/scENVI-0.0.1.tar.gz` & `tmp/scENVI-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scENVI-0.0.1.tar", last modified: Fri Apr  7 17:39:09 2023, max compression
+gzip compressed data, was "scENVI-0.0.7.tar", last modified: Mon Apr 10 18:38:30 2023, max compression
```

## Comparing `scENVI-0.0.1.tar` & `scENVI-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-07 17:39:09.173086 scENVI-0.0.1/
--rw-r--r--   0 havivd    (1777) peer      (6070)        0 2023-03-15 16:56:55.000000 scENVI-0.0.1/LICENSE
--rw-r--r--   0 havivd    (1777) peer      (6070)     1912 2023-04-07 17:39:09.172407 scENVI-0.0.1/PKG-INFO
--rw-r--r--   0 havivd    (1777) peer      (6070)     1415 2023-04-07 17:33:11.000000 scENVI-0.0.1/README.md
--rw-r--r--   0 havivd    (1777) peer      (6070)      573 2023-04-07 17:36:46.000000 scENVI-0.0.1/pyproject.toml
-drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-07 17:39:09.166166 scENVI-0.0.1/scENVI/
--rw-r--r--   0 havivd    (1777) peer      (6070)    78361 2023-04-07 16:41:14.000000 scENVI-0.0.1/scENVI/ENVI.py
--rw-r--r--   0 havivd    (1777) peer      (6070)        0 2023-03-15 16:52:08.000000 scENVI-0.0.1/scENVI/__init__.py
-drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-07 17:39:09.171289 scENVI-0.0.1/scENVI.egg-info/
--rw-r--r--   0 havivd    (1777) peer      (6070)     1912 2023-04-07 17:39:09.167651 scENVI-0.0.1/scENVI.egg-info/PKG-INFO
--rw-r--r--   0 havivd    (1777) peer      (6070)      186 2023-04-07 17:39:09.169156 scENVI-0.0.1/scENVI.egg-info/SOURCES.txt
--rw-r--r--   0 havivd    (1777) peer      (6070)        1 2023-04-07 17:39:09.170422 scENVI-0.0.1/scENVI.egg-info/dependency_links.txt
--rw-r--r--   0 havivd    (1777) peer      (6070)        7 2023-04-07 17:39:09.171503 scENVI-0.0.1/scENVI.egg-info/top_level.txt
--rw-r--r--   0 havivd    (1777) peer      (6070)       38 2023-04-07 17:39:09.173306 scENVI-0.0.1/setup.cfg
+drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-10 18:38:30.913244 scENVI-0.0.7/
+-rw-r--r--   0 havivd    (1777) peer      (6070)        0 2023-03-15 16:56:55.000000 scENVI-0.0.7/LICENSE
+-rw-r--r--   0 havivd    (1777) peer      (6070)     1916 2023-04-10 18:38:30.912462 scENVI-0.0.7/PKG-INFO
+-rw-r--r--   0 havivd    (1777) peer      (6070)     1419 2023-04-07 21:20:08.000000 scENVI-0.0.7/README.md
+-rw-r--r--   0 havivd    (1777) peer      (6070)      819 2023-04-10 18:38:09.000000 scENVI-0.0.7/pyproject.toml
+drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-10 18:38:30.899910 scENVI-0.0.7/scENVI/
+-rw-r--r--   0 havivd    (1777) peer      (6070)    56995 2023-04-10 18:00:17.000000 scENVI-0.0.7/scENVI/ENVI.py
+-rw-r--r--   0 havivd    (1777) peer      (6070)        0 2023-03-15 16:52:08.000000 scENVI-0.0.7/scENVI/__init__.py
+-rw-r--r--   0 havivd    (1777) peer      (6070)     8697 2023-04-10 17:57:36.000000 scENVI-0.0.7/scENVI/output_layer.py
+-rw-r--r--   0 havivd    (1777) peer      (6070)    12047 2023-04-10 17:56:54.000000 scENVI-0.0.7/scENVI/utils.py
+drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-10 18:38:30.911124 scENVI-0.0.7/scENVI.egg-info/
+-rw-r--r--   0 havivd    (1777) peer      (6070)     1916 2023-04-10 18:38:30.907367 scENVI-0.0.7/scENVI.egg-info/PKG-INFO
+-rw-r--r--   0 havivd    (1777) peer      (6070)      254 2023-04-10 18:38:30.908490 scENVI-0.0.7/scENVI.egg-info/SOURCES.txt
+-rw-r--r--   0 havivd    (1777) peer      (6070)        1 2023-04-10 18:38:30.909438 scENVI-0.0.7/scENVI.egg-info/dependency_links.txt
+-rw-r--r--   0 havivd    (1777) peer      (6070)      143 2023-04-10 18:38:30.910384 scENVI-0.0.7/scENVI.egg-info/requires.txt
+-rw-r--r--   0 havivd    (1777) peer      (6070)        7 2023-04-10 18:38:30.911421 scENVI-0.0.7/scENVI.egg-info/top_level.txt
+-rw-r--r--   0 havivd    (1777) peer      (6070)       38 2023-04-10 18:38:30.913472 scENVI-0.0.7/setup.cfg
```

### Comparing `scENVI-0.0.1/PKG-INFO` & `scENVI-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: scENVI
-Version: 0.0.1
+Version: 0.0.7
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ENVI - Integrating scRNA-seq and spatial data to impute missing genes and recosntruct spatial context 
+# ENVI - Integrating scRNA-seq and spatial data to impute missing genes and reconstruct spatial context 
 
 ![alt text](img/envi_schem.png?raw=true)
 
 # Installation 
 Insatll ENVI (and COVET) through pypi:
  
 ```
-pip install --index-url https://test.pypi.org/simple/ ENVI_PeerLab==0.0.9
+!python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps scENVI
 
 ```
 
 # Tutorial
 
 For a notebook on how to run ENVI and analyze the results, go to example notebook.
 
 
 # Usage
 
 To run ENVI:
 ```
-from ENVI_PeerLab import ENVI
+from scENVI import ENVI
 
 model = ENVI.ENVI(spatial_data = st_data, sc_data = sc_data)
 model.Train()
 ENVI_Model.impute()
 ENVI_Model.infer_cov()
 
 ```
@@ -60,17 +60,18 @@
 sc_data.uns['COVET_genes'] =  ENVI_Model.CovGenes
 
 ```
 And To run COVET (just on spatial data):
 
 ```
 ENVI.COVET(st_data, k = 8, g = 64,spatial_key = 'spatial')
-'''
+```
 
 COVET information will be in:
 
-'''
+```
 st_data.obsm['COVET'] 
 st_data.obsm['COVET_SQRT'] 
 st_data.uns['COVET_Genes']
-'''
+```
+
```

### Comparing `scENVI-0.0.1/README.md` & `scENVI-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# ENVI - Integrating scRNA-seq and spatial data to impute missing genes and recosntruct spatial context 
+# ENVI - Integrating scRNA-seq and spatial data to impute missing genes and reconstruct spatial context 
 
 ![alt text](img/envi_schem.png?raw=true)
 
 # Installation 
 Insatll ENVI (and COVET) through pypi:
  
 ```
-pip install --index-url https://test.pypi.org/simple/ ENVI_PeerLab==0.0.9
+!python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps scENVI
 
 ```
 
 # Tutorial
 
 For a notebook on how to run ENVI and analyze the results, go to example notebook.
 
 
 # Usage
 
 To run ENVI:
 ```
-from ENVI_PeerLab import ENVI
+from scENVI import ENVI
 
 model = ENVI.ENVI(spatial_data = st_data, sc_data = sc_data)
 model.Train()
 ENVI_Model.impute()
 ENVI_Model.infer_cov()
 
 ```
@@ -46,17 +46,18 @@
 sc_data.uns['COVET_genes'] =  ENVI_Model.CovGenes
 
 ```
 And To run COVET (just on spatial data):
 
 ```
 ENVI.COVET(st_data, k = 8, g = 64,spatial_key = 'spatial')
-'''
+```
 
 COVET information will be in:
 
-'''
+```
 st_data.obsm['COVET'] 
 st_data.obsm['COVET_SQRT'] 
 st_data.uns['COVET_Genes']
-'''
+```
+
```

### Comparing `scENVI-0.0.1/scENVI/ENVI.py` & `scENVI-0.0.7/scENVI/ENVI.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,357 +10,19 @@
 import time
 import sklearn.neural_network
 import pandas as pd
 import scipy.sparse
 import pickle
 import sys
 
+from utils import *
+from output_layer import *
 
-class HiddenPrints:
-    def __enter__(self):
-        self._original_stdout = sys.stdout
-        sys.stdout = open(os.devnull, 'w')
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        sys.stdout.close()
-        
-
-class LinearLayer(tf.keras.layers.Layer):
-    """
-    Costume keras linear layer
 
-    Args:
-        units (int): number of neurons in the layer
-        input_dim (int): dimension of input to layer
-        kernel_init (keras initializer): initializer for neural weights
-        bias_init (keras initializer): initializer of neural biases
-    """
-    def __init__(self, units, input_dim, kernel_init, bias_init, name):
-        super(LinearLayer, self).__init__()
-        self.w = self.add_weight(
-            shape=(input_dim, units), initializer=kernel_init, trainable=True, name = name + '/kernel')
-        self.b = self.add_weight(shape=(units,), initializer=bias_init, trainable=True, name = name + '/bias')
-
-    def call(self, inputs):
-        return tf.matmul(inputs, self.w) + self.b
-
-class ConstantLayer(tf.keras.layers.Layer):
-    """
-    Costume keras constant layer, biases only
-
-    Args:
-        units (int): number of neurons in the layer
-        input_dim (int): dimension of input to layer
-        bias_init (keras initializer): initializer of neural biases
-        comm_disp (bool): if True, spatial_dist and sc_dist share dispersion parameter(s)
-        const_disp (bool): if True, dispertion parameter(s) are only per gene, rather there per gene per sample
-    """
-    def __init__(self, units, input_dim, bias_init, name):
-        super(ConstantLayer, self).__init__()
-        self.b = self.add_weight(shape=(units,), initializer=bias_init, trainable=True, name = name + '/bias')
-
-    def call(self, inputs):
-        return tf.tile(self.b[None, :], [inputs.shape[0], 1])
-    
-class ENVIOutputLayer(tf.keras.layers.Layer):
-    """
-    Costume keras layer for ENVI expression decoder output
-
-    Args:
-        units (int): number of neurons in the layer
-        input_dim (int): dimension of input to layer
-        kernel_init (keras initializer): initializer for neural weights
-        bias_init (keras initializer): initializer of neural biases
-        spatial_dist (str): distribution used to describe spatial data (default pois, could be 'pois', 'nb', 'zinb', 'norm' or 'full_norm') 
-        sc_dist (str): distribution used to describe sinlge cell data (default nb, could be 'pois', 'nb', 'zinb', 'norm' or 'full_norm')
-    """
-    def __init__(self, 
-                 input_dim, 
-                 units, 
-                 kernel_init,
-                 bias_init,
-                 spatial_dist = 'pois',
-                 sc_dist = 'nb',
-                 comm_disp = False,
-                 const_disp = False,
-                 name = 'dec_exp_output'):
-        super(ENVIOutputLayer, self).__init__()
-        
-        self.input_dim = input_dim
-        self.units = units
-        
-        self.spatial_dist = spatial_dist
-        self.sc_dist = sc_dist
-        self.comm_disp = comm_disp
-        self.const_disp = const_disp
-        
-        self.kernel_init = kernel_init
-        self.bias_init = bias_init
-        
-        self.r = LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_r')  
-        
-        if(self.comm_disp):  
-            
-            if(self.spatial_dist == 'zinb'):
-                self.p_spatial = (ConstantLayer(units, input_dim, bias_init, name = name + '_p_spatial')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_p_spatial'))
-                                    
-                self.d_spatial = (ConstantLayer(units, input_dim, bias_init + '_d_spatial')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_d_spatial'))
-
-            elif(self.spatial_dist == 'nb' or self.spatial_dist == 'full_norm'):
-                self.p_spatial = (ConstantLayer(units, input_dim, bias_init, name = name + '_p_spatial')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_p_spatial'))
-                
-            if(self.sc_dist == 'zinb'):
-                self.p_sc = (self.p_spatial if (self.spatial_dist == 'zinb' or self.spatial_dist == 'nb' or self.spatial_dist == 'full_norm') 
-                            else (ConstantLayer(units, input_dim, bias_init, name = name + '_p_sc') 
-                                  if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_p_sc')))
-                                    
-                self.d_sc = (self.d_spatial if (self.spatial_dist == 'zinb') 
-                            else (ConstantLayer(units, input_dim, bias_init, name = name + '_d_sc') 
-                                  if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_d_sc')))
-
-            elif(self.sc_dist == 'nb' or self.sc_dist == 'full_norm'):
-                
-                self.p_sc = (self.p_spatial if (self.spatial_dist == 'zinb' or self.spatial_dist == 'nb' or self.spatial_dist == 'full_norm') 
-                            else (ConstantLayer(units, input_dim, bias_init, name = name + '_p_sc') 
-                                  if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_r_sc')))
-                
-                
-            if(self.spatial_dist == 'zinb' or self.sc_dist == 'zinb'):
-                self.p_spatial = (ConstantLayer(units, input_dim, bias_init, name = name + '_p_spatial')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_p_spatial'))
-                                
-                self.p_sc = self.p_spatial
-                
-                self.d_spatial = (ConstantLayer(units, input_dim, bias_init, name = name + '_d_spatial')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_d_spatial'))
-                
-                self.d_sc = self.d_spatial
-
-            elif(self.spatial_dist == 'nb' or self.sc_dist == 'nb' or self.spatial_dist == 'full_norm' or self.sc_dist == 'full_norm'):
-                
-                self.p_spatial = (ConstantLayer(units, input_dim, kernel_init, name = name + '_p_spatial')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_p_spatial'))
-                
-                self.p_sc = self.p_spatial
-        
-        else:  
-            
-            if(self.spatial_dist == 'zinb'):
-                self.p_spatial = (ConstantLayer(units, input_dim, bias_init, name = name + '_p_spatial')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_p_spatial'))
-                                    
-                self.d_spatial = (ConstantLayer(units, input_dim, bias_init, name = name + '_d_spatial')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_d_spatial'))
-
-            elif(self.spatial_dist == 'nb' or self.spatial_dist == 'full_norm'):
-                self.p_spatial = (ConstantLayer(units, input_dim, bias_init, name = name + '_p_spatial')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_p_spatial'))
-                
-            if(self.sc_dist == 'zinb'):
-                self.p_sc = (ConstantLayer(units, input_dim, bias_init, name = name + '_p_sc')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_p_sc'))
-                                    
-                self.d_sc = (ConstantLayer(units, input_dim, bias_init, name = name + '_d_sc')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_d_sc'))
-
-            elif(self.sc_dist == 'nb' or self.sc_dist == 'full_norm'):
-                self.p_sc = (ConstantLayer(units, input_dim, bias_init, name = name + '_p_sc')
-                          if self.const_disp else LinearLayer(units, input_dim, kernel_init, bias_init, name = name + '_p_sc'))
-            
-    
-    
-    def call(self, inputs, mode = 'spatial'):
-        r = self.r(inputs)
-         
-        if(getattr(self, mode + '_dist') == 'zinb'):
-                p = getattr(self, 'p_' + mode)(inputs)
-                d = getattr(self, 'd_' + mode)(inputs)
-                return(r,p,d)
-                
-        if(getattr(self, mode + '_dist') == 'nb' or getattr(self, mode + '_dist') == 'full_norm'):
-                p = getattr(self, 'p_' + mode)(inputs)
-                return(r,p)
-        
-        return(r)
-    
-    
-def NormalNorm(arr):
-    """
-    z-scores data
-
-    Args:
-        arr (array): array to z-score
-    Return:
-        zscore_arr: arr z-scored
-    """
-    arr = np.asarray(arr)
-    arr = (arr - arr.mean(axis = 0, keepdims = True))/arr.std(axis = 0, keepdims = True)
-    return(arr)
-    
-def MatSqrtTF(Mats):
-    """
-    Computes psuedo matrix square root with tensorfow linear algebra on cpu
-
-    Args:
-        Mats (array): Matrices to compute square root of 
-    Return:
-        SqrtMats (np.array): psuedo matrix square of Mats
-    """
-    with tf.device('/CPU:0'):
-        e,v = tf.linalg.eigh(Mats)
-        e = tf.where(e < 0, 0, e)
-        e = tf.math.sqrt(e)
-        return(tf.linalg.matmul(tf.linalg.matmul(v, tf.linalg.diag(e)), v, transpose_b = True).numpy())
-
-
-def BatchKNN(data, batch, k):
-    
-    kNNGraphIndex = np.zeros(shape = (data.shape[0], k))
-    WeightedIndex = np.zeros(shape = (data.shape[0] ,k))
-    
-    for val in np.unique(batch):
-        val_ind = np.where(batch == val)[0]
-        
-        batch_knn = sklearn.neighbors.kneighbors_graph(data[val_ind], n_neighbors=k, mode='distance', n_jobs=-1).tocoo()
-        batch_knn_ind = np.reshape(np.asarray(batch_knn.col), [data[val_ind].shape[0], k])
-        
-        batch_knn_weight = scipy.special.softmax(-np.reshape(batch_knn.data, [data[val_ind].shape[0], k]), axis = -1)
-        
-        kNNGraphIndex[val_ind] = val_ind[batch_knn_ind]
-        WeightedIndex[val_ind] = batch_knn_weight
-    return(kNNGraphIndex.astype('int'), WeightedIndex)
-    
-    
-def GetNeighExp(spatial_data, kNN, spatial_key = 'spatial', batch_key = -1, data_key = None):
-    
-    """
-    Computing Niche mean expression based on cell expression and location
-
-    Args:
-        spatial_data (anndata): anndata with spatial data, with obsm 'spatial' indicating spatial location of spot/segmented cell
-        kNN (int): number of nearest neighbours to define niche
-        spatial_key (str): obsm key name with physical location of spots/cells (default 'spatial')
-        batch_key (str): obs key name of batch/sample of spatial data (default -1)
-        data_key (str): obsm key to compute niche mean across (defualt None, uses gene expression .X)
-
-    Return:
-        NeighExp: Average geene expression in niche 
-        kNNGraphIndex: indices of nearest spatial neighbours per cell
-    """
-    
-    if(data_key is None):
-        Data = spatial_data.X
-    else:
-        Data = spatial_data.obsm[data_key]
-        
-    if(batch_key == -1):        
-        kNNGraph = sklearn.neighbors.kneighbors_graph(spatial_data.obsm[spatial_key], n_neighbors=kNN, mode='distance', n_jobs=-1).tocoo()
-        kNNGraph = scipy.sparse.coo_matrix((np.ones_like(kNNGraph.data), (kNNGraph.row, kNNGraph.col)), shape=kNNGraph.shape)
-        kNNGraphIndex = np.reshape(np.asarray(kNNGraph.col), [spatial_data.obsm[spatial_key].shape[0], kNN])
-    else:
-        kNNGraphIndex, _ = BatchKNN(spatial_data.obsm[spatial_key], spatial_data.obs[batch_key], kNN)
-    
-    
-    return(Data[kNNGraphIndex[np.arange(spatial_data.obsm[spatial_key].shape[0])]])
-
-
-
-def GetCovMats(spatial_data, kNN, spatial_key = 'spatial', batch_key = -1, MeanExp = None, weighted = False, cov_pc = 1):
-    
-        
-    """
-    Wrapper to compute niche covariance based on cell expression and location
-
-    Args:
-        spatial_data (anndata): anndata with spatial data, with obsm 'spatial' indicating spatial location of spot/segmented cell
-        kNN (int): number of nearest neighbours to define niche
-        spatial_key (str): obsm key name with physical location of spots/cells (default 'spatial')
-        batch_key (str): obs key name of batch/sample of spatial data (default -1)
-        MeanExp (np.array): expression vector to shift niche covariance with
-        weighted (bool): if True, weights covariance by spatial distance
-    Return:
-        CovMats: niche covariance matrices
-        kNNGraphIndex: indices of nearest spatial neighbours per cell
-    """
-    ExpData = spatial_data[:, spatial_data.var.highly_variable].X
-    
-    if(cov_pc > 0):
-        ExpData = np.log(ExpData + cov_pc)
-    
-    if(batch_key == -1 or batch_key not in spatial_data.obs.columns):        
-        kNNGraph = sklearn.neighbors.kneighbors_graph(spatial_data.obsm[spatial_key], n_neighbors=kNN, mode='distance', n_jobs=-1).tocoo()
-        kNNGraph = scipy.sparse.coo_matrix((np.ones_like(kNNGraph.data), (kNNGraph.row, kNNGraph.col)), shape=kNNGraph.shape)
-        kNNGraphIndex = np.reshape(np.asarray(kNNGraph.col), [spatial_data.obsm[spatial_key].shape[0], kNN])
-        WeightedIndex = scipy.special.softmax(-np.reshape(kNNGraph.data, [spatial_data.obsm[spatial_key].shape[0], kNN]), axis = -1)
-    else:
-        kNNGraphIndex, WeightedIndex = BatchKNN(spatial_data.obsm[spatial_key], spatial_data.obs[batch_key], kNN)
-        
-    if not weighted:
-        WeightedIndex = np.ones_like(WeightedIndex)/kNN
-        
-    if(MeanExp is None):
-        DistanceMatWeighted = (ExpData.mean(axis = 0)[None, None, :] - ExpData[kNNGraphIndex[np.arange(ExpData.shape[0])]]) * np.sqrt(WeightedIndex)[:, :, None] * np.sqrt(1 / (1 - np.sum(np.square(WeightedIndex), axis= -1)))[:, None, None]
-    else:
-        DistanceMatWeighted = (MeanExp[:, None, :] - ExpData[kNNGraphIndex[np.arange(ExpData.shape[0])]]) * np.sqrt(WeightedIndex)[:, :, None] * np.sqrt(1 / (1 - np.sum(np.square(WeightedIndex), axis= -1)))[:, None, None]
-
-    CovMats = np.matmul(DistanceMatWeighted.transpose([0,2,1]), DistanceMatWeighted)
-    CovMats = CovMats + CovMats.mean() * 0.00001 * np.expand_dims(np.identity(CovMats.shape[-1]), axis=0) 
-    return(CovMats, kNNGraphIndex)
-
-def GetCov(spatial_data, k, g, genes, cov_dist, spatial_key = 'spatial', batch_key = -1, cov_pc = 1):
-    
-    """
-    Compte niche covariance matrices for spatial data
-
-    Args:
-        spatial_data (anndata): anndata with spatial data, with obsm 'spatial' indicating spatial location of spot/segmented cell
-        k (int): number of nearest neighbours to define niche
-        g (int): number of HVG to compute niche covariance matricies
-        genes (list of str): list of genes to keep for niche covariance
-        cov_dist (str): distribution to transform niche covariance matrices to fit into
-        batch_key (str): obs key for batch informationm (default -1, for no batch)
-
-    Return:
-        CovMats: raw, untransformed niche covariance matrices
-        CovMatsSQRT: covariance matrices transformed into chosen cov_dist
-        NeighExp: Average geene expression in niche 
-        CovGenes: Genes used for niche covariance 
-    """
-        
-        
-    spatial_data.layers['log'] = np.log(spatial_data.X + 1)
-
-    if(g == -1):
-        CovGeneSet = np.arange(spatial_data.shape[-1])
-        spatial_data.var.highly_variable = True
-    else:
-        sc.pp.highly_variable_genes(spatial_data, n_top_genes = g, layer = 'log')
-        if(g == 0):
-            spatial_data.var.highly_variable = False
-        if(len(genes) > 0):
-            spatial_data.var['highly_variable'][genes] = True
-    
-    CovGeneSet = np.where(np.asarray(spatial_data.var.highly_variable))[0]
-    CovGenes = spatial_data.var_names[CovGeneSet]
-    
-    CovMats, kNNGraphIndex = GetCovMats(spatial_data, k, spatial_key = spatial_key, batch_key = batch_key, weighted = False, cov_pc = cov_pc)
-    NicheMat = spatial_data.X[kNNGraphIndex[np.arange(spatial_data.shape[0])]]
-    
-    if(cov_dist == 'norm'):
-        CovMatsSQRT = CovMats.reshape([CovMats.shape[0], -1])
-        CovMatsSQRT = (CovMatsSQRT - CovMatsSQRT.mean(axis = 0, keepdims = True)) / CovMatsSQRT.std(axis = 0, keepdims = True)
-    if(cov_dist == 'OT'):
-        CovMatsSQRT = MatSqrtTF(CovMats)
-    else:
-        CovMatsSQRT = np.copy(CovMats)
-    
-    return(CovMats.astype('float32'), CovMatsSQRT.astype('float32'), NicheMat.astype('float32'), CovGenes)
 
 
 def COVET(data, k=8, g=64,  genes=[], spatial_key = 'spatial', batch_key = -1, cov_pc = 1):
     
     """
     Compte niche covariance matrices for spatial data
 
@@ -369,25 +31,25 @@
         k (int): number of nearest neighbours to define niche
         g (int): number of HVG to compute niche covariance matricies
         genes (list of str): list of genes to keep for niche covariance (if empty, just uses HVG)
         batch_key (str): obs key for batch informationm (default -1, for no batch)
         cov_pc (float): log psuedo-count for COVET computation (if 0, use unlogged values)
 
     Return:
-        CovMats: raw, untransformed niche covariance matrices
-        CovMatsSQRT: covariance matrices transformed into chosen cov_dist
+        COVET: raw, untransformed niche covariance matrices
+        COVET_SQRT: covariance matrices transformed into chosen cov_dist
         NeighExp: Average geene expression in niche 
         CovGenes: Genes used for niche covariance 
     """
       
     
-    CovMats, CovMatsSQRT, _, CovGenes = GetCov(data, k, g, genes, 'OT', spatial_key = spatial_key, batch_key = batch_key, cov_pc = cov_pc)
+    COVET, COVET_SQRT, _, CovGenes = GetCov(data, k, g, genes, 'OT', spatial_key = spatial_key, batch_key = batch_key, cov_pc = cov_pc)
 
-    data.obsm['COVET'] = CovMats.astype('float32')
-    data.obsm['COVET_SQRT'] = CovMatsSQRT.astype('float32')
+    data.obsm['COVET'] = COVET.astype('float32')
+    data.obsm['COVET_SQRT'] = COVET_SQRT.astype('float32')
     data.uns['COVET_Genes'] = CovGenes
 
     return(data)
 
 class ENVI():
     
     """
@@ -543,19 +205,19 @@
             print("Computing COVET Matrices")
 
 
             self.num_cov_genes = min(num_cov_genes, self.spatial_data.shape[-1])
             self.cov_genes = cov_genes
             self.cov_pc = cov_pc
 
-            self.spatial_data.obsm['CovMats'], self.spatial_data.obsm['CovMatsSQRT'], self.spatial_data.obsm['NicheMat'], self.CovGenes = GetCov(self.spatial_data, self.k_nearest, self.num_cov_genes, self.cov_genes, self.cov_dist, spatial_key = self.spatial_key, batch_key = self.batch_key, cov_pc = self.cov_pc)
+            self.spatial_data.obsm['COVET'], self.spatial_data.obsm['COVET_SQRT'], self.spatial_data.obsm['NicheMat'], self.CovGenes = GetCov(self.spatial_data, self.k_nearest, self.num_cov_genes, self.cov_genes, self.cov_dist, spatial_key = self.spatial_key, batch_key = self.batch_key, cov_pc = self.cov_pc)
 
 
             self.overlap_num = self.overlap_genes.shape[0]
-            self.cov_gene_num = self.spatial_data.obsm['CovMatsSQRT'].shape[-1]
+            self.cov_gene_num = self.spatial_data.obsm['COVET_SQRT'].shape[-1]
             self.full_trans_gene_num = self.sc_data.shape[-1]
 
 
 
 
             if((self.agg != 'sum') and (self.agg != 'mean')):
                 self.agg_spatial = self.spatial_data.var[self.agg].astype('float32') 
@@ -1134,15 +796,15 @@
         """
         Infer covariance niche composition for single cell data
         
         Args:
             NumDiv (int): number of splits for forward pass to allow to fit in gpu
             revert (bool): if True, computes actual covariance, if False, computes transformed covariance (default False)
         Return:
-            no return, adds 'CovMatsSQRT' or 'CovMats' to ENVI.sc_data.obsm
+            no return, adds 'COVET_SQRT' or 'COVET' to ENVI.sc_data.obsm
         """
         
         if(data is None):
             self.sc_data.obsm['COVET_SQRT'] = np.concatenate([self.cov_decode(np.array_split(self.sc_data.obsm['envi_latent'], NumDiv, axis = 0)[_]) 
                                      for _ in range(NumDiv)], axis = 0)
             self.sc_data.obsm['COVET'] = np.concatenate([np.linalg.matrix_power(np.array_split(self.sc_data.obsm['COVET_SQRT'], NumDiv, axis = 0)[_], 2) 
                              for _ in range(NumDiv)], axis = 0)
@@ -1158,15 +820,15 @@
         """
         Reconstruct covariance niche composition for spatial data
         
         Args:
             NumDiv (int): number of splits for forward pass to allow to fit in gpu
   
         Return:
-            no return, adds 'CovMatsSQRT' or 'CovMats' to ENVI.sc_data.obsm
+            no return, adds 'COVET_SQRT' or 'COVET' to ENVI.sc_data.obsm
         """
             
         self.spatial_data.obsm['COVET_SQRT_envi'] = np.concatenate([self.cov_decode(np.array_split(self.spatial_data.obsm['envi_latent'], NumDiv, axis = 0)[_]) 
                                  for _ in range(NumDiv)], axis = 0)
         self.spatial_data.obsm['COVET_envi'] = np.concatenate([np.linalg.matrix_power(np.array_split(self.spatial_data.obsm['COVET_SQRT_envi'], NumDiv, axis = 0)[_], 2) 
                          for _ in range(NumDiv)], axis = 0)
 
@@ -1212,16 +874,16 @@
         if(cluster):
             import phenograph
 
         if(data is None):
             self.infer_COVET(16, False)
 
             if(pred_key is None):
-                CovFit = self.spatial_data.obsm['CovMatsSQRT']
-                CovPred = self.sc_data.obsm['CovMatsSQRT']
+                CovFit = self.spatial_data.obsm['COVET_SQRT']
+                CovPred = self.sc_data.obsm['COVET_SQRT']
 
                 NeighFit = self.spatial_data.obsm['niche_by_type']
 
                 if(norm_reg):
                     NeighFit = NeighFit/self.spatial_data.obsm['cell_type_enc'].sum(axis = 0, keepdims = True)
                     NeighFit = NeighFit/NeighFit.sum(axis = 1, keepdims = True) * self.k_nearest
 
@@ -1246,16 +908,16 @@
                     regressor.fit(CovFit.reshape([CovFit.shape[0], -1]), NeighFit)
                     NeighPred = regressor.predict(CovPred.reshape([CovPred.shape[0], -1]))
                     self.sc_data.obsm['niche_by_type'] = pd.DataFrame(NeighPred, columns = CellTypeName, index = self.sc_data.obs_names)
             else:
 
                 NeighPred = np.zeros(shape = (self.sc_data.shape[0], NeighCellType.shape[-1]))
                 for val in np.unique(self.sc_data.obs[pred_key]):
-                    CovFit = self.spatial_data.obsm['CovMatsSQRT'][self.spatial_data.obs[pred_key] == val]
-                    CovPred = self.sc_data.obsm['CovMatsSQRT'][self.sc_data.obs[pred_key] == val]
+                    CovFit = self.spatial_data.obsm['COVET_SQRT'][self.spatial_data.obs[pred_key] == val]
+                    CovPred = self.sc_data.obsm['COVET_SQRT'][self.sc_data.obs[pred_key] == val]
 
                     NeighFit = np.asarray(self.spatial_data.obsm['niche_by_type'][self.spatial_data.obs[pred_key] == val])
 
                     if(norm_reg):
                         NeighFit = NeighFit/self.spatial_data.obsm['cell_type_enc'].sum(axis = 0, keepdims = True)
                         NeighFit = NeighFit/NeighFit.sum(axis = 1, keepdims = True) * self.k_nearest
 
@@ -1280,15 +942,15 @@
 
                 self.sc_data.obsm['niche_by_type'] = pd.DataFrame(NeighPred, columns = CellTypeName, index = self.sc_data.obs_names)
         else:
             
             sc_cov_mats = self.infer_COVET(16, False, data)
 
             if(pred_key is None):
-                CovFit = self.spatial_data.obsm['CovMatsSQRT']
+                CovFit = self.spatial_data.obsm['COVET_SQRT']
                 CovPred = sc_cov_mats
 
                 NeighFit = self.spatial_data.obsm['niche_by_type']
 
                 if(norm_reg):
                     NeighFit = NeighFit/self.spatial_data.obsm['cell_type_enc'].sum(axis = 0, keepdims = True)
                     NeighFit = NeighFit/NeighFit.sum(axis = 1, keepdims = True) * self.k_nearest
@@ -1314,15 +976,15 @@
                     regressor.fit(CovFit.reshape([CovFit.shape[0], -1]), NeighFit)
                     NeighPred = regressor.predict(CovPred.reshape([CovPred.shape[0], -1]))
                     niche_by_type = pd.DataFrame(NeighPred, columns = CellTypeName, index = data.obs_names)
             else:
 
                 NeighPred = np.zeros(shape = (data.shape[0], NeighCellType.shape[-1]))
                 for val in np.unique(self.sc_data.obs[pred_key]):
-                    CovFit = self.spatial_data.obsm['CovMatsSQRT'][self.spatial_data.obs[pred_key] == val]
+                    CovFit = self.spatial_data.obsm['COVET_SQRT'][self.spatial_data.obs[pred_key] == val]
                     CovPred = sc_cov_mats[data.obs[pred_key] == val]
 
                     NeighFit = np.asarray(self.spatial_data.obsm['niche_by_type'][self.spatial_data.obs[pred_key] == val])
 
                     if(norm_reg):
                         NeighFit = NeighFit/self.spatial_data.obsm['cell_type_enc'].sum(axis = 0, keepdims = True)
                         NeighFit = NeighFit/NeighFit.sum(axis = 1, keepdims = True) * self.k_nearest
@@ -1347,15 +1009,15 @@
                         regressor.fit(CovFit.reshape([CovFit.shape[0], -1]), NeighFit)
                         NeighPred[data.obs[pred_key] == val] = regressor.predict(CovPred.reshape([CovPred.shape[0], -1]))
 
                 niche_by_type = pd.DataFrame(NeighPred, columns = CellTypeName, index = data.obs_names)
             
             return(niche_by_type)
 #         print("Finished Niche Reconstruction! See 'niche_by_type' in obsm of ENVI.sc_data")
-    
+
     @tf.function
     def compute_apply_gradients(self, spatial_sample, cov_sample, sc_sample):
                 
         """
         Applies gradient descent step given training batch
         
         Args:
@@ -1381,16 +1043,16 @@
 
         gradients = tape.gradient(loss, self.trainable_variables)
         nan = False
         
 #         for grad in gradients:
 #             if(tf.reduce_sum(tf.cast(tf.math.is_nan(grad), tf.int8)) > 0):
 #                 nan = True
-        if(tf.math.is_nan(loss)):
-            nan = True
+        # if(tf.math.is_nan(loss)):
+        #     nan = True
             
         if(nan):
             return(spatial_like,  cov_like, sc_like, kl, True)
         else:
             self.optimizer.apply_gradients(zip(gradients, self.trainable_variables))
         return (spatial_like,  cov_like, sc_like, kl, False)
 
@@ -1415,15 +1077,15 @@
 
         self.LR = LR
         self.optimizer = tf.keras.optimizers.Adam(self.LR)
 
         
         
         spatial_data_train = self.spatial_data.X.astype(tf.keras.backend.floatx())
-        cov_data_train = self.spatial_data.obsm['CovMatsSQRT'].astype(tf.keras.backend.floatx())
+        cov_data_train = self.spatial_data.obsm['COVET_SQRT'].astype(tf.keras.backend.floatx())
         sc_data_train = self.sc_data.X.astype(tf.keras.backend.floatx())
         
 
         ## Run Dummy:
         log_pos_pdf(tf.ones([5], tf.float32), tf.ones([5], tf.float32))
         
         start_time = time.time()
@@ -1496,124 +1158,7 @@
             import os
             if not os.path.exists(directory):
                 os.makedirs(directory)
 
             with open(self.save_path, 'wb') as handle:
                 pickle.dump(attribute_list, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
-
-
-@tf.function
-def LogNormalKL(mean, log_std, agg = None):
-    KL = 0.5 * (tf.square(mean) + tf.square(tf.exp(log_std)) - 2 * log_std)
-    if(agg is None):
-        return(KL)
-    if(not isinstance(agg, (str))):
-        return(tf.reduce_mean(KL, axis = -1))
-    if(agg == 'sum'):
-        return(tf.reduce_sum(KL, axis = -1))
-    return(tf.reduce_mean(KL, axis = -1))
-     
-    
-@tf.function        
-def NormalKL(mean, log_std, agg = None):
-    KL = 0.5 * (tf.square(mean) + tf.square(tf.exp(log_std)) - 2 * log_std)
-    if(agg is None):
-        return(KL)
-    if(not isinstance(agg, (str))):
-        return(tf.reduce_mean(KL, axis = -1))
-    if(agg == 'sum'):
-        return(tf.reduce_sum(KL, axis = -1))
-    
-    return(tf.reduce_mean(KL, axis = -1))
-
-@tf.function    
-def log_pos_pdf(sample, l, agg = None):
-    log_prob = tfp.distributions.Poisson(rate=l).log_prob(sample)
-    if(agg is None):
-        return(log_prob)
-    if(not isinstance(agg, (str))):
-        return(tf.reduce_mean(log_prob * agg[None, :log_prob.shape[-1]], axis = -1))
-    if(agg == 'sum'):
-        return(tf.reduce_sum(log_prob, axis = -1))
-    return(tf.reduce_mean(log_prob, axis = -1))
-
-@tf.function
-def log_nb_pdf(sample, r, p, agg = None):
-    # log_prob = tfp.distributions.NegativeBinomial(total_count=r, logits=p).log_prob(sample)
-    log_prob = tfp.distributions.NegativeBinomial(total_count=r, logits=p).log_prob(sample)
-    #log_prob = log_nb(sample, r, p)
-    if(agg is None):
-        return(log_prob)
-    if(not isinstance(agg, (str))):
-        return(tf.reduce_mean(log_prob * agg[None, :log_prob.shape[-1]], axis = -1))
-    if(agg == 'sum'):
-        return(tf.reduce_sum(log_prob, axis = -1))
-    return(tf.reduce_mean(log_prob, axis = -1))
-
-@tf.function
-def log_zinb_pdf(sample, r, p, d, agg = None):
-    log_prob = tfp.distributions.Mixture(
-        cat=tfp.distributions.Categorical(probs=tf.stack([d, 1-d], -1)),
-        components=[tfp.distributions.Deterministic(loc = tf.zeros_like(d)), tfp.distributions.NegativeBinomial(total_count = r, logits = p)]).log_prob(sample)
-
-    
-    if(agg is None):
-        return(log_prob)
-    if(not isinstance(agg, (str))):
-        return(tf.reduce_mean(log_prob * agg[None, :log_prob.shape[-1]], axis = -1))
-    if(agg == 'sum'):
-        return(tf.reduce_sum(log_prob, axis = -1))
-    return(tf.reduce_mean(log_prob, axis = -1))
-
-@tf.function   
-def OTDistance(sample, mean, agg = None):
-    sample = tf.reshape(sample, [sample.shape[0], -1])
-    mean = tf.reshape(mean, [mean.shape[0], -1])
-    log_prob = - tf.square(sample - mean)
-    if(agg is None):
-        return(log_prob)
-    if(not isinstance(agg, (str))):
-        return(tf.reduce_mean(log_prob, axis = -1))
-    if(agg == 'sum'):
-        return(tf.reduce_sum(log_prob, axis = -1))
-    return(tf.reduce_mean(log_prob, axis = -1))
-
-@tf.function    
-def log_normal_pdf(sample, mean, scale, agg = None):
-    log_prob = tfp.distributions.Normal(loc = mean, scale = tf.exp(scale)).log_prob(sample)
-    if(agg is None):
-        return(log_prob)
-    if(not isinstance(agg, (str))):
-        return(tf.reduce_mean(log_prob * agg[None, :log_prob.shape[-1]], axis = -1))
-    if(agg == 'sum'):
-        return(tf.reduce_sum(log_prob, axis = -1))
-    return(tf.reduce_mean(log_prob, axis = -1))
-
-@tf.function
-def trace_log(Mat):
-    return(tf.reduce_mean(tf.math.log(tf.linalg.diag_part(Mat)), axis = -1))
-
-@tf.function
-def log_wish_pdf(sample, scale, agg = 'mean'):
-    if(agg == 'mean'):
-        return(tfp.distributions.WishartTriL(df = sample.shape[-1], scale_tril = scale, input_output_cholesky = True).log_prob(sample)/(sample.shape[-1] ** 2))
-    elif(agg == 'mean'):
-        return(tfp.distributions.WishartTriL(df = sample.shape[-1], scale_tril = scale, input_output_cholesky = True).log_prob(sample))
-
-# @tf.function
-# def Sinkhorn(OT_mat, env_mat, reg = 0.1):
-#     M =  tf.reduce_sum(tf.square(OT_mat), axis = 1)[None, :, None] - 2 * tf.matmul(OT_mat, env_mats, transpose_b = True) + tf.reduce_sum(tf.square(env_mats), axis = -1)[:, None, :]
-#     M = tf.square(M)
-#     M  = tf.transpose(M, [0,2,1])/tf.stop_gradient(tf.reduce_max(M, axis = (1,2))[:, None, None])
-#     K = tf.exp(-M/reg)
-
-#     u = np.ones([env_mats.shape[0], env_mats.shape[1]])#/env_mats.shape[1]    
-
-#     for i in range(100):
-
-#         v = (1/env_mats.shape[1])/tf.squeeze(tf.matmul(K, u[:, :, None], transpose_a = True)) #tf.squeeze(tf.matmul(K, u[:, :, None], transpose_a = True)
-#         u = (1/env_mats.shape[1])/tf.squeeze(tf.matmul(K, v[:, :, None], transpose_a = False))
-
-#     T = u[:, :, None] * (K * v[:, None, :])
-
-#     return(tf.reduce_sum(T * M, axis = [1,2]))
```

### Comparing `scENVI-0.0.1/scENVI.egg-info/PKG-INFO` & `scENVI-0.0.7/scENVI.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: scENVI
-Version: 0.0.1
+Version: 0.0.7
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ENVI - Integrating scRNA-seq and spatial data to impute missing genes and recosntruct spatial context 
+# ENVI - Integrating scRNA-seq and spatial data to impute missing genes and reconstruct spatial context 
 
 ![alt text](img/envi_schem.png?raw=true)
 
 # Installation 
 Insatll ENVI (and COVET) through pypi:
  
 ```
-pip install --index-url https://test.pypi.org/simple/ ENVI_PeerLab==0.0.9
+!python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps scENVI
 
 ```
 
 # Tutorial
 
 For a notebook on how to run ENVI and analyze the results, go to example notebook.
 
 
 # Usage
 
 To run ENVI:
 ```
-from ENVI_PeerLab import ENVI
+from scENVI import ENVI
 
 model = ENVI.ENVI(spatial_data = st_data, sc_data = sc_data)
 model.Train()
 ENVI_Model.impute()
 ENVI_Model.infer_cov()
 
 ```
@@ -60,17 +60,18 @@
 sc_data.uns['COVET_genes'] =  ENVI_Model.CovGenes
 
 ```
 And To run COVET (just on spatial data):
 
 ```
 ENVI.COVET(st_data, k = 8, g = 64,spatial_key = 'spatial')
-'''
+```
 
 COVET information will be in:
 
-'''
+```
 st_data.obsm['COVET'] 
 st_data.obsm['COVET_SQRT'] 
 st_data.uns['COVET_Genes']
-'''
+```
+
```

