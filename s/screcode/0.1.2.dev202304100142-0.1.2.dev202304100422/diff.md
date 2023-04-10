# Comparing `tmp/screcode-0.1.2.dev202304100142-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202304100422-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 118801 bytes, number of entries: 6
+Zip file size: 118714 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    56947 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304100142.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304100142.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304100142.dist-info/RECORD
-6 files, 207733 bytes uncompressed, 117897 bytes compressed:  43.2%
+-rw-r--r--  2.0 unx    56640 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304100422.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304100422.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304100422.dist-info/RECORD
+6 files, 207426 bytes uncompressed, 117810 bytes compressed:  43.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202304100142.dist-info/METADATA
+Filename: screcode-0.1.2.dev202304100422.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202304100142.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202304100422.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202304100142.dist-info/RECORD
+Filename: screcode-0.1.2.dev202304100422.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -1437,25 +1437,20 @@
 		Xmean,
 		ell,
 		version=1,
 		TO_CR = 1
 	):
 		if version==2 and self.RECODE_done == False:
 			U_ell = U[:ell,:]
-			# U_ell_mod = np.copy(U_ell)
 			L_ell = L[:ell,:ell]
 			for i in range(ell):
-				# U[i,U_argsort[i][::-1][U_sort[::-1].cumsum() > TO_CR]] = 0
-				# idx_order = np.argsort(np.abs(U[i]))[::-1]
-				# idx_sparce = np.sort(np.abs(U[i]))[::-1].cumsum() > L_ell[i,i]
 				idx_order = np.argsort(U[i]**2)[::-1]
 				idx_sparce = np.sort(U[i]**2)[::-1].cumsum() > L_ell[i,i]
 				U_ell[i,idx_order[idx_sparce]] = 0
 				U_ell[i] = U_ell[i]/np.sqrt(np.sum(U_ell[i]**2))
-			#U_ell[i,:] = U[i,:]/np.sqrt(np.sum(U[i]**2))
 			return np.dot(np.dot(np.dot(X-Xmean,U_ell.T),L_ell),U_ell)+Xmean
 		else:
 			U_ell = U[:ell,:]
 			L_ell = L[:ell,:ell]
 			return np.dot(np.dot(np.dot(X-Xmean,U_ell.T),L_ell),U_ell)+Xmean
 
 	def _noise_reduct_param(
@@ -1503,15 +1498,14 @@
 					div_max = (j+1)*delta+X_var_min
 					k[j] = len(np.where((X_var_sub<div_max) & (X_var_sub>div_min))[0])
 				error[i] = (2*np.mean(k)-np.var(k))/delta/delta
 		
 		opt_div = int(np.argmin(error)+1)
 
 		k = np.empty([opt_div],dtype=int)
-		k_index = np.empty([opt_div],dtype=list)
 		delta = X_var_range/opt_div
 		for j in range(opt_div):
 				div_min = j*delta+X_var_min
 				div_max = (j+1)*delta+X_var_min
 				k[j] = len(np.where((X_var_sub<=div_max) & (X_var_sub>div_min))[0])
 		idx_k_max = np.argmax(k)
 		div_min = idx_k_max*delta+X_var_min
```

## Comparing `screcode-0.1.2.dev202304100142.dist-info/METADATA` & `screcode-0.1.2.dev202304100422.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202304100142
+Version: 0.1.2.dev202304100422
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

