# Comparing `tmp/screcode-0.1.2.dev202304092258-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202304100142-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 118764 bytes, number of entries: 6
+Zip file size: 118801 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    56772 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304092258.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304092258.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304092258.dist-info/RECORD
-6 files, 207558 bytes uncompressed, 117860 bytes compressed:  43.2%
+-rw-r--r--  2.0 unx    56947 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304100142.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304100142.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304100142.dist-info/RECORD
+6 files, 207733 bytes uncompressed, 117897 bytes compressed:  43.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202304092258.dist-info/METADATA
+Filename: screcode-0.1.2.dev202304100142.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202304092258.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202304100142.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202304092258.dist-info/RECORD
+Filename: screcode-0.1.2.dev202304100142.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -21,15 +21,15 @@
 		seq_target = 'RNA',
 		version = 1,
 		stat_learning = False,
 		stat_learning_rate = 0.2,
 		stat_learning_seed = 0,
 		decimals = 5,
 		RECODE_key = 'RECODE',
-		anndata_key = 'obsm',
+		anndata_key = 'layers',
 		verbose = True,
 		):
 		""" 
 		RECODE (Resolution of curse of dimensionality in single-cell data analysis). A noise reduction method for single-cell sequencing data. 
 		
 		Parameters
 		----------
@@ -84,15 +84,16 @@
 			self.unit,self.Unit = 'peak','Peak'
 		if seq_target == 'Hi-C':
 			self.unit,self.Unit = 'bin','Bin'
 		self.log_ = {}
 		self.log_['seq_target'] = self.seq_target
 		self.fit_idx = False
 		self.logger = logging.getLogger("argument checking")
-		self.logger.setLevel(logging.WARNING)
+		if self.verbose == True:
+			self.logger.setLevel(logging.WARNING)
 
 	def _check_datatype(
 		self,
 		X
 	):
 		if type(X) == anndata._core.anndata.AnnData:
 			if scipy.sparse.issparse(X.X):
@@ -268,18 +269,18 @@
 		self.significance_ = np.empty(X.shape[1],dtype=object)
 		self.significance_[self.normalized_variance_==0] = 'silent'
 		self.significance_[self.normalized_variance_>0] = 'non-significant'
 		self.significance_[self.normalized_variance_>1] = 'significant'
 
 		if type(X) == anndata._core.anndata.AnnData:
 			X_out = anndata.AnnData.copy(X)
-			if self.anndata_key == 'layers':
-				X_out.layers['RECODE'] = X_RECODE
-			else:
+			if self.anndata_key == 'obsm':
 				X_out.obsm['RECODE'] = X_RECODE
+			else:
+				X_out.layers['RECODE'] = X_RECODE
 			X_out.var['noise_variance_RECODE'] = self.noise_variance_
 			X_out.var['normalized_variance_RECODE'] = self.normalized_variance_
 			X_out.var['significance_RECODE'] = self.significance_
 		else:
 			X_out = X_RECODE
 
 		return X_out
@@ -1539,17 +1540,20 @@
 		n,d = X.shape
 		n_pca = min(n-1,d-1)
 		if self.fast_algorithm:
 			n_pca = min(n_pca,self.fast_algorithm_ell_ub)
 		X_mean = np.mean(X,axis=0)
 
 		if n > d:
-			S = np.dot((X - X_mean).T,(X - X_mean))/(X.shape[0]-1)
-			svd = sklearn.decomposition.TruncatedSVD(n_components=n_pca).fit(S)
-			PCA_Ev = svd.singular_values_
+			# S = np.dot((X - X_mean).T,(X - X_mean))/(X.shape[0]-1)
+			# svd = sklearn.decomposition.TruncatedSVD(n_components=n_pca).fit(S)
+			# PCA_Ev = svd.singular_values_
+			svd = sklearn.decomposition.TruncatedSVD(n_components=n_pca).fit(X-X_mean)
+			SVD_Sv = svd.singular_values_
+			PCA_Ev = (SVD_Sv**2)/(n-1)
 			self.U = svd.components_
 		else:
 			SD = np.dot((X - X_mean),(X - X_mean).T)/(X.shape[0]-1)
 			svd = sklearn.decomposition.TruncatedSVD(n_components=n_pca).fit(SD)
 			PCA_Ev = svd.singular_values_
 			self.U = np.dot((svd.components_.T/np.sqrt(PCA_Ev)).T,(X - X_mean))/np.sqrt(X.shape[0]-1)
```

## Comparing `screcode-0.1.2.dev202304092258.dist-info/METADATA` & `screcode-0.1.2.dev202304100142.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202304092258
+Version: 0.1.2.dev202304100142
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

