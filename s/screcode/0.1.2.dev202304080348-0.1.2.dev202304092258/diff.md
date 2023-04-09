# Comparing `tmp/screcode-0.1.2.dev202304080348-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202304092258-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 118885 bytes, number of entries: 6
+Zip file size: 118764 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    57535 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304080348.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304080348.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304080348.dist-info/RECORD
-6 files, 208321 bytes uncompressed, 117981 bytes compressed:  43.4%
+-rw-r--r--  2.0 unx    56772 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304092258.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304092258.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304092258.dist-info/RECORD
+6 files, 207558 bytes uncompressed, 117860 bytes compressed:  43.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202304080348.dist-info/METADATA
+Filename: screcode-0.1.2.dev202304092258.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202304080348.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202304092258.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202304080348.dist-info/RECORD
+Filename: screcode-0.1.2.dev202304092258.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -307,15 +307,15 @@
 				"No use of the stat_learning option is recommended to keep the accuracy.")
 			np.random.seed(self.stat_learning_seed)
 			X_mat = self._check_datatype(X)
 			cell_stat = np.random.choice(X_mat.shape[0],int(self.stat_learning_rate*X.shape[0]),replace=False)					
 			self.fit(X_mat[cell_stat])
 		else:
 			if X.shape[0] > 20000:
-				self.logger.warning("Warning: RECODE uses high computational resources for data with a large number of cells. \n"
+				self.logger.warning("Warning: Regular RECODE uses high computational resources for data with a large number of cells. \n"
 				"Use of the stat_learning option is recommended as \"RECODE(stat_learning=True)\". ")
 			self.fit(X)
 		X_RECODE = self.transform(X)
 		end_time = datetime.datetime.now()
 		elapsed_time = end_time - start_time
 		hours, remainder = divmod(elapsed_time.seconds, 3600)
 		minutes, seconds = divmod(remainder, 60)
@@ -1549,32 +1549,14 @@
 			self.U = svd.components_
 		else:
 			SD = np.dot((X - X_mean),(X - X_mean).T)/(X.shape[0]-1)
 			svd = sklearn.decomposition.TruncatedSVD(n_components=n_pca).fit(SD)
 			PCA_Ev = svd.singular_values_
 			self.U = np.dot((svd.components_.T/np.sqrt(PCA_Ev)).T,(X - X_mean))/np.sqrt(X.shape[0]-1)
 		
-		# S = np.dot((X - X_mean).T,(X - X_mean))/(X.shape[0]-1)
-		# svd = sklearn.decomposition.TruncatedSVD(n_components=n_pca).fit(S)
-		# PCA_Ev1 = svd.singular_values_
-		# U1 = svd.components_
-
-		# SD = np.dot((X - X_mean),(X - X_mean).T)/(X.shape[0]-1)
-		# svd = sklearn.decomposition.TruncatedSVD(n_components=n_pca).fit(SD)
-		# PCA_Ev2 = svd.singular_values_
-		# U2 = np.dot((svd.components_.T/np.sqrt(PCA_Ev2)).T,(X - X_mean))/np.sqrt(X.shape[0]-1)
-
-		# svd = sklearn.decomposition.TruncatedSVD(n_components=n_pca).fit(X-X_mean)
-		# SVD_Sv = svd.singular_values_
-		# PCA_Ev = (SVD_Sv**2)/(n-1)
-		# U3 =  svd.components_
-		# print(self.U)
-		# print(U1.shape,U2.shape,U3.shape)
-		# print(PCA_Ev1.shape,PCA_Ev2.shape,PCA_Ev.shape)
-		# print(PCA_Ev1-PCA_Ev,PCA_Ev2-PCA_Ev)
 		PCA_Ev_sum_all = np.sum(np.var(X,axis=0,ddof=1))
 		PCA_Ev_NRM = np.array(PCA_Ev,dtype=float)
 		PCA_Ev_sum_diff = PCA_Ev_sum_all - np.sum(PCA_Ev)
 		n_Ev_all = min(n,d)
 		PCA_Ev_NRM = np.array([PCA_Ev[i]-(np.sum(PCA_Ev[i+1:])+PCA_Ev_sum_diff)/(n_Ev_all-i-1) for i in range(len(PCA_Ev_NRM)-1)])
 		PCA_Ev_NRM = np.append(PCA_Ev_NRM,0)
 		PCA_CCR = (PCA_Ev/PCA_Ev_sum_all).cumsum()
```

## Comparing `screcode-0.1.2.dev202304080348.dist-info/METADATA` & `screcode-0.1.2.dev202304092258.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202304080348
+Version: 0.1.2.dev202304092258
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

