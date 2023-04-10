# Comparing `tmp/screcode-0.1.2.dev202304100422-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202304101152-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 118714 bytes, number of entries: 6
+Zip file size: 118728 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    56640 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304100422.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304100422.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304100422.dist-info/RECORD
-6 files, 207426 bytes uncompressed, 117810 bytes compressed:  43.2%
+-rw-r--r--  2.0 unx    56674 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304101152.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304101152.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304101152.dist-info/RECORD
+6 files, 207460 bytes uncompressed, 117824 bytes compressed:  43.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202304100422.dist-info/METADATA
+Filename: screcode-0.1.2.dev202304101152.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202304100422.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202304101152.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202304100422.dist-info/RECORD
+Filename: screcode-0.1.2.dev202304101152.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -84,16 +84,18 @@
 			self.unit,self.Unit = 'peak','Peak'
 		if seq_target == 'Hi-C':
 			self.unit,self.Unit = 'bin','Bin'
 		self.log_ = {}
 		self.log_['seq_target'] = self.seq_target
 		self.fit_idx = False
 		self.logger = logging.getLogger("argument checking")
-		if self.verbose == True:
+		if verbose:
 			self.logger.setLevel(logging.WARNING)
+		else:
+			self.logger.setLevel(logging.ERROR)
 
 	def _check_datatype(
 		self,
 		X
 	):
 		if type(X) == anndata._core.anndata.AnnData:
 			if scipy.sparse.issparse(X.X):
```

## Comparing `screcode-0.1.2.dev202304100422.dist-info/METADATA` & `screcode-0.1.2.dev202304101152.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202304100422
+Version: 0.1.2.dev202304101152
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

