# Comparing `tmp/cellmap-1.0.1.dev202304101155-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304101210-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 8631 bytes, number of entries: 5
+Zip file size: 8542 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    41120 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101155.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101155.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304101155.dist-info/RECORD
-5 files, 43251 bytes uncompressed, 7877 bytes compressed:  81.8%
+-rw-r--r--  2.0 unx    40790 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101210.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101210.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304101210.dist-info/RECORD
+5 files, 42921 bytes uncompressed, 7788 bytes compressed:  81.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304101155.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304101210.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304101155.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304101210.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304101155.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304101210.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -188,15 +188,15 @@
     basis = 'umap',
     potential_key = 'Hodge_potential',
     potential_vkey = 'potential_velocity',
     rotation_key = 'Hodge_rotation',
     rotation_vkey = 'rotation_velocity',
     graph_key = 'CM_graph',
     graph_method = 'Delauney',
-    alpha = 0.5,
+    alpha = 0.2,
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
     verbose = True,
     logscale_vel = True,
     ):
@@ -252,40 +252,31 @@
     
     if alpha > 0:
         idx_vel_HD = np.isnan(vel_HD[0])==False
         X1,X2 = exp_HD[:,idx_vel_HD][source],exp_HD[:,idx_vel_HD][target]
         V1,V2 = vel_HD[:,idx_vel_HD][source],vel_HD[:,idx_vel_HD][target]
         Dis = np.linalg.norm(X2-X1,axis=1)
         Dis[Dis==0] = 1
-<<<<<<< HEAD
         edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis/np.sum(idx_vel_HD)
-=======
-        edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
+        # edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
         edge_vel_HD_norm = np.linalg.norm(edge_vel_HD)
         if edge_vel_HD_norm > 0: edge_vel_HD = edge_vel_HD/edge_vel_HD_norm
->>>>>>> 987059fb20c7a26b8af350bfd55a5b8fbc5137fa
     else:
         edge_vel_HD = 0
     
     if alpha < 1:
         idx_vel_LD = np.isnan(vel_LD[0])==False
         X1,X2 = exp_LD[:,idx_vel_LD][source],exp_LD[:,idx_vel_LD][target]
         V1,V2 = vel_LD[:,idx_vel_LD][source],vel_LD[:,idx_vel_LD][target]
         Dis = np.linalg.norm(X2-X1,axis=1)
         Dis[Dis==0] = 1
-<<<<<<< HEAD
         V1_p,V2_p = V1*(X2-X1),V2*(X2-X1)
         V1_p[V1_p<0] = 0
         V2_p[V2_p<0] = 0
         edge_vel_LD = np.sum(0.5*(V1_p+V2_p),axis=1)/Dis/2
-=======
-        edge_vel_LD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
-        edge_vel_LD_norm = np.linalg.norm(edge_vel_LD)
-        if edge_vel_LD_norm > 0: edge_vel_LD = edge_vel_LD/edge_vel_LD_norm
->>>>>>> 987059fb20c7a26b8af350bfd55a5b8fbc5137fa
     else:
         edge_vel_LD = 0
     
     ## Solve potential
     n_edge_ = len(source)
     grad_mat = np.zeros([n_edge_,n_node_],dtype=float)
     grad_mat[tuple(np.vstack((np.arange(n_edge_),source)))] = -1
```

## Comparing `cellmap-1.0.1.dev202304101155.dist-info/METADATA` & `cellmap-1.0.1.dev202304101210.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304101155
+Version: 1.0.1.dev202304101210
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

