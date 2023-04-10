# Comparing `tmp/cellmap-1.0.1.dev202304020858-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304101155-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7855 bytes, number of entries: 5
+Zip file size: 8631 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    37060 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304020858.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304020858.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304020858.dist-info/RECORD
-5 files, 39191 bytes uncompressed, 7101 bytes compressed:  81.9%
+-rw-r--r--  2.0 unx    41120 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101155.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101155.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304101155.dist-info/RECORD
+5 files, 43251 bytes uncompressed, 7877 bytes compressed:  81.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304020858.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304101155.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304020858.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304101155.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304020858.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304101155.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -39,23 +39,29 @@
     if return_mask: return tri_,tri_mask_
     else: return tri_
 
 
 
 def check_arguments(
     adata,
+    verbose = True,
     **kwargs
 ):
     logger = logging.getLogger("argument checking")
-    logger.setLevel(logging.WARNING)
+    if verbose:
+        logger.setLevel(logging.WARNING)
+    else:
+        logger.setLevel(logging.ERROR)
     
     if 'exp_key' in kwargs.keys():
         if kwargs['exp_key'] != None:
             if (kwargs['exp_key'] not in adata.obsm.keys()) and (kwargs['exp_key'] not in adata.layers.keys()):
-                raise KeyError('The key \"%s\" was not found in adata.obsm.obsm. Please modify the argument \"exp_key\".' % kwargs['exp_key'])
+                err_mssg = 'The key \"%s\" was not found in adata.obsm.obsm. Please modify the argument \"exp_key\".' % kwargs['exp_key']
+                logger.exception(err_mssg)
+                raise KeyError(err_mssg)
     
     if 'exp_2d_key' in kwargs.keys():
         if (kwargs['exp_2d_key'] not in adata.obsm.keys()) and (kwargs['exp_2d_key'] not in adata.layers.keys()):
             if 'X_umap' in adata.obsm.keys():
                 logger.warning('The key \"%s\" was not found in adata.obsm, but \"X_umap\" was found insted. \"%s\" was replaced with \"X_umap\".' % (kwargs['exp_2d_key'],kwargs['exp_2d_key']))
                 kwargs['exp_2d_key'] = 'X_umap'
             elif 'X_tsne' in adata.obsm.keys():
@@ -79,21 +85,21 @@
             elif 'velocity_tsne' in adata.obsm.keys():
                 logger.warning('Warning: The key \"%s\" was not found in adata.obsm, but \"velocity_tsne\" was found insted. \"%s\" was replaced with \"velocity_tsne\".' % (kwargs['vel_2d_key'],kwargs['vel_2d_key']))
                 kwargs['vel_2d_key'] = 'velocity_tsne'
             else:
                 raise KeyError('The key \"%s\" was not found in adata.obsm.obsm. Please modify the argument \"vel_2d_key\".' % kwargs['vel_2d_key'])
     
     if 'basis' in kwargs.keys():
-        if (kwargs['basis'] not in adata.obsm.keys()) and (kwargs['basis'] not in adata.layers.keys()):
+        if ('X_%s' % kwargs['basis'] not in adata.obsm.keys()) and ('X_%s' % kwargs['basis'] not in adata.layers.keys()):
             if 'X_umap' in adata.obsm.keys():
                 logger.warning('The key \"%s\" was not found in adata.obsm, but \"X_umap\" was found insted. \"%s\" was replaced with \"X_umap\".' % (kwargs['basis'],kwargs['basis']))
-                kwargs['basis'] = 'X_umap'
+                kwargs['basis'] = 'umap'
             elif 'X_tsne' in adata.obsm.keys():
                 logger.warning('Warning: The key \"%s\" was not found in adata.obsm, but \"X_tsne\" was found insted. \"%s\" was replaced with \"X_tsne\".' % (kwargs['basis'],kwargs['basis']))
-                kwargs['basis'] = 'X_tsne'
+                kwargs['basis'] = 'tsne'
             else:
                 raise KeyError('The key \"%s\" was not found in adata.obsm.obsm. Please modify the argument \"exp_2d_key\".' % kwargs['basis'])
 
     if 'map_key' in kwargs.keys():
         if kwargs['map_key'] == None:
             kwargs['map_key'] = kwargs['exp_2d_key']
     
@@ -118,14 +124,19 @@
     key_names = ['expression_key']
     for key in key_names:
         if key in kwargs.keys():
             if kwargs[key] != None:
                 if (kwargs[key] not in adata.obsm.keys()) & (kwargs[key] not in adata.layers.keys()):
                     raise KeyError('The key \"%s\" was not found in adata.obsm or adata.layers. Please modify the argument \"%s\".' % (kwargs[key],key))
     
+    if 'graph_method' in kwargs.keys():
+        if kwargs['graph_method'] != None:
+            if kwargs['graph_method'] not in ['Delauney','knn']:
+                raise KeyError('The key \"%s\" was not found in adata.obsm or adata.layers. Please modify the argument \"%s\".' % (kwargs[key],key))
+
     key = 'obs_key'
     if key in kwargs.keys():
         if type(kwargs[key]) == list:
             key_names = ['cluster_key','potential_key']
             for key_ in key_names:
                 if key_ in kwargs.keys():
                     if kwargs[key_] in kwargs[key]:
@@ -170,23 +181,24 @@
     return cmap
 
 
 def Hodge_decomposition(
     adata,
     exp_key = None,
     vel_key  = 'velocity',
-    exp_2d_key = 'X_umap',
-    vel_2d_key = 'velocity_umap',
+    basis = 'umap',
     potential_key = 'Hodge_potential',
+    potential_vkey = 'potential_velocity',
     rotation_key = 'Hodge_rotation',
+    rotation_vkey = 'rotation_velocity',
     graph_key = 'CM_graph',
     graph_method = 'Delauney',
     alpha = 0.5,
     n_neighbors = 10,
-    contribution_rate = 0.95,
+    contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
     verbose = True,
     logscale_vel = True,
     ):
     """
     Hodge decomposition
@@ -194,17 +206,21 @@
     Parameters
     ----------
     adata: anndata (n_samples, n_features)
     
     exp_key: None or string
     """
     
-    kwargs_arg = check_arguments(adata, exp_key=exp_key, vel_key = vel_key, exp_2d_key=exp_2d_key, vel_2d_key=vel_2d_key, graph_method=graph_method)
-    exp_key,vel_key,exp_2d_key,vel_2d_key = kwargs_arg['exp_key'],kwargs_arg['vel_key'],kwargs_arg['exp_2d_key'],kwargs_arg['vel_2d_key']
+    kwargs_arg = check_arguments(adata, verbose = True, exp_key=exp_key, vel_key = vel_key, basis=basis, graph_method=graph_method)
+    exp_key,vel_key,basis = kwargs_arg['exp_key'],kwargs_arg['vel_key'],kwargs_arg['basis']
     
+    exp_2d_key = 'X_%s' % basis
+    vel_2d_key = 'velocity_%s' % basis
+    pot_vkey_ = '%s_%s' % (potential_vkey,basis)
+    rot_vkey_ = '%s_%s' % (rotation_vkey,basis)
     
     if exp_key == None:
         if scipy.sparse.issparse(adata.X):
             exp_HD = adata.X.toarray()
         else:
             exp_HD = adata.X
     elif exp_key in adata.obsm.keys():
@@ -214,71 +230,108 @@
     
     vel_HD = adata.obsm[vel_key] if vel_key in adata.obsm.keys() else adata.layers[vel_key]
     if logscale_vel:
         vel_HD = (adata.obs['n_counts'].values*vel_HD.T).T/np.exp(exp_HD)
     exp_LD = adata.obsm[exp_2d_key][:,:2] if exp_2d_key in adata.obsm.keys() else adata.layers[exp_2d_key][:,:2]
     vel_LD = adata.obsm[vel_2d_key][:,:2] if vel_2d_key in adata.obsm.keys() else adata.layers[vel_2d_key][:,:2]
     
+    ## Compute graph and edge velocities
     n_node_ = exp_HD.shape[0]
     if graph_method == 'Delauney':
         tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
         source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
     elif graph_method == 'knn':
         pca = sklearn.decomposition.PCA()
         exp_HD_pca = pca.fit_transform(exp_HD)
-        n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate])
+        n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate_pca])
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_HD_pca[:,:n_pca])
         distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
         distances, indices = distances[:,1:], indices[:,1:]
         source = np.ravel(np.repeat(np.arange(exp_HD.shape[0]).reshape((-1, 1)),n_neighbors,axis=1))
         target = np.ravel(indices)
     
     if alpha > 0:
         idx_vel_HD = np.isnan(vel_HD[0])==False
         X1,X2 = exp_HD[:,idx_vel_HD][source],exp_HD[:,idx_vel_HD][target]
         V1,V2 = vel_HD[:,idx_vel_HD][source],vel_HD[:,idx_vel_HD][target]
         Dis = np.linalg.norm(X2-X1,axis=1)
         Dis[Dis==0] = 1
+<<<<<<< HEAD
+        edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis/np.sum(idx_vel_HD)
+=======
         edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
         edge_vel_HD_norm = np.linalg.norm(edge_vel_HD)
         if edge_vel_HD_norm > 0: edge_vel_HD = edge_vel_HD/edge_vel_HD_norm
+>>>>>>> 987059fb20c7a26b8af350bfd55a5b8fbc5137fa
     else:
         edge_vel_HD = 0
     
     if alpha < 1:
         idx_vel_LD = np.isnan(vel_LD[0])==False
         X1,X2 = exp_LD[:,idx_vel_LD][source],exp_LD[:,idx_vel_LD][target]
         V1,V2 = vel_LD[:,idx_vel_LD][source],vel_LD[:,idx_vel_LD][target]
         Dis = np.linalg.norm(X2-X1,axis=1)
         Dis[Dis==0] = 1
+<<<<<<< HEAD
+        V1_p,V2_p = V1*(X2-X1),V2*(X2-X1)
+        V1_p[V1_p<0] = 0
+        V2_p[V2_p<0] = 0
+        edge_vel_LD = np.sum(0.5*(V1_p+V2_p),axis=1)/Dis/2
+=======
         edge_vel_LD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
         edge_vel_LD_norm = np.linalg.norm(edge_vel_LD)
         if edge_vel_LD_norm > 0: edge_vel_LD = edge_vel_LD/edge_vel_LD_norm
+>>>>>>> 987059fb20c7a26b8af350bfd55a5b8fbc5137fa
     else:
         edge_vel_LD = 0
     
+    ## Solve potential
     n_edge_ = len(source)
     grad_mat = np.zeros([n_edge_,n_node_],dtype=float)
     grad_mat[tuple(np.vstack((np.arange(n_edge_),source)))] = -1
     grad_mat[tuple(np.vstack((np.arange(n_edge_),target)))] = 1
     div_mat = -grad_mat.T
     lap = -np.dot(div_mat,grad_mat)
     edge_vel = (1-alpha)*edge_vel_LD+alpha*edge_vel_HD
     source_term = np.dot(div_mat,edge_vel)
     lap_inv = np.linalg.pinv(lap)
     potential = np.dot(lap_inv,source_term)
     pot_flow = -np.dot(grad_mat,potential)
     adata.obs[potential_key] = potential - np.min(potential)
 
     rot_flow = edge_vel - pot_flow
-    source_target = np.hstack((source,target))
-    rot_flow_2 = np.hstack((rot_flow,rot_flow))
-    adata.obs[rotation_key] = np.array([np.mean(rot_flow_2[source_target==i]) for i in range(adata.shape[0])])
+    adata.obs[rotation_key] = np.array([np.mean(np.vstack((rot_flow[source==i],-rot_flow[target==i]))) for i in range(adata.shape[0])])
+
+    ## Compute potential & rotational flow
+    vel_potential = np.zeros([adata.shape[0],2],dtype=float)
+    if graph_method == 'Delauney':
+        tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
+        source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
+        for i in range(adata.shape[0]):
+            idx_s = source == i
+            idx_t = target == i
+            ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
+            ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
+            vel_potential[i] = 2*(np.sum((adata.obs[potential_key][source[idx_s]].values-adata.obs[potential_key][target[idx_s]].values)*ex_s.T,axis=1) + \
+                                np.sum((adata.obs[potential_key][target[idx_t]].values-adata.obs[potential_key][source[idx_t]].values)*ex_t.T,axis=1))
+        adata.obsm[pot_vkey_] = vel_potential
+        adata.obsm[rot_vkey_]  = adata.obsm['velocity_umap']-vel_potential
+    elif graph_method == 'knn':
+        knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
+        knn.fit(exp_LD)
+        distances, indices = knn.kneighbors(exp_LD)
+        distances, indices = distances[:,1:], indices[:,1:]
+        for i in range(adata.shape[0]):
+            ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
+            vel_potential[i] = -2*np.sum((adata.obs[potential_key].values[indices[i]]-adata.obs[potential_key].values[i])*ex_s.T,axis=1)
+        adata.obsm[pot_vkey_] = vel_potential
+        adata.obsm[rot_vkey_]  = adata.obsm['velocity_umap']-vel_potential
 
+    ## Contribution ratio
     log_ = {}
     log_["Contribution_ratio"] = {}
     norm_grad = np.linalg.norm(pot_flow)
     norm_curl = np.linalg.norm(rot_flow)
     log_["Contribution_ratio"]['Potential'] = '{:.2%}'.format(norm_grad/(norm_grad+norm_curl))
     log_["Contribution_ratio"]['Rotation']  = '{:.2%}'.format(norm_curl/(norm_grad+norm_curl))
     adata.uns['CellMap_log'] = log_
@@ -368,15 +421,15 @@
         edge_vel = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
         source_term = np.dot(div_mat,edge_vel)
         potential = np.dot(lap_inv,source_term)
         adata.obs[potential_key+'_Gene_%s' % gene] = potential - np.min(potential)
 
 def view(
     adata,
-    basis = 'X_umap',
+    basis = 'umap',
     potential_key = 'Hodge_potential',
     graph_key = 'CM_graph',
     cluster_key = None,
     show_graph = False,
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
@@ -385,19 +438,20 @@
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
                              potential_key = potential_key,
                              graph_key = graph_key,
                             )
     basis = kwargs_arg['basis']
+    basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
     
-    data_pos = adata.obsm[basis]
+    data_pos = adata.obsm[basis_key]
     fig,ax = plt.subplots(figsize=(15,10))
     sc = ax.scatter(data_pos[:,0],data_pos[:,1],c=adata.obs[potential_key],zorder=10,**kwargs)
     if show_graph:
         tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
         ax.tripcolor(tri_,adata.obs[potential_key],lw=0.5,zorder=0,alpha=0.3,cmap=kwargs['cmap'])
     if cluster_key != None:
         if cluster_key in adata.obs.keys():
@@ -410,15 +464,15 @@
     ax.axis('off')
     ax.set_title(title,fontsize=18)
     plt.colorbar(sc,aspect=20, pad=0.01, orientation='vertical').set_label(potential_key,fontsize=20);
 
 
 def view_cluster(
     adata,
-    basis = 'X_umap',
+    basis = 'umap',
     potential_key = 'Hodge_potential',
     graph_key = 'CM_graph',
     cluster_key = 'clusters',
     show_graph = True,
     cutedge_vol  = None,
     cutedge_length = None,
     n_points = 1000,
@@ -429,19 +483,20 @@
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
                              potential_key = potential_key,
                              graph_key = graph_key,
                             )
     basis = kwargs_arg['basis']
+    basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
 
-    data_pos = adata.obsm[basis]
+    data_pos = adata.obsm[basis_key]
     fig,ax = plt.subplots(figsize=(15,10))
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
     # sc = ax.tripcolor(tri_,adata.obs[potential_key],lw=0.5,zorder=0,alpha=0.75,cmap=kwargs['cmap'])
     sc = ax.tricontourf(tri_,adata.obs[potential_key],zorder=0,alpha=0.9,cmap=kwargs['cmap'],levels=100)
     if cluster_key in adata.obs.keys():
         cluster = adata.obs[cluster_key]
         idx_random = np.zeros(cluster.shape,dtype=bool)
@@ -460,15 +515,15 @@
     ax.set_title(title,fontsize=18)
     plt.colorbar(sc,aspect=20, pad=0.01, orientation='vertical').set_label(potential_key,fontsize=20)
     ax.axis('off')
 
 
 def view_surface(
     adata,
-    basis = 'X_umap',
+    basis = 'umap',
     potential_key = 'Hodge_potential',
     graph_key = 'CM_graph',
     cluster_key = None,
     show_graph = False,
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
@@ -477,20 +532,20 @@
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
                              potential_key = potential_key,
                              graph_key = graph_key,
                             )
     basis = kwargs_arg['basis']
-
+    basis_key = 'X_%s' % basis
 
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
     
-    data_pos = adata.obsm[basis]
+    data_pos = adata.obsm[basis_key]
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
     fig,ax = plt.subplots(figsize=(15,10))
     cntr = ax.tricontourf(tri_,adata.obs[potential_key],cmap=kwargs['cmap'],levels=100,zorder=2)
     fig.colorbar(cntr, shrink=0.75, orientation='vertical').set_label(potential_key,fontsize=20)
     if show_graph: ax.triplot(tri_,color='w',lw=0.5,zorder=10,alpha=1)
     ax.set_xlim(np.min(data_pos[:,0])-0.02*(np.max(data_pos[:,0])-np.min(data_pos[:,0])),np.max(data_pos[:,0])+0.02*(np.max(data_pos[:,0])-np.min(data_pos[:,0])))
     ax.set_ylim(np.min(data_pos[:,1])-0.02*(np.max(data_pos[:,1])-np.min(data_pos[:,1])),np.max(data_pos[:,1])+0.02*(np.max(data_pos[:,1])-np.min(data_pos[:,1])))
@@ -502,20 +557,45 @@
         if cluster_key in adata.obs.keys():
             cluster = adata.obs[cluster_key]
             for c in np.unique(cluster):
                 txt = ax.text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=20,ha='center', va='center',fontweight='bold')
                 txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
                 texts.append(txt)
 
-def view_surface_genes                                                                                                                                                                                                                        (
+def view_stream(
+    adata,
+    basis = 'umap',
+    vkey = 'velocity',
+    potential_key = 'Hodge_potential',
+    potential_vkey = 'potential_velocity',
+    rotation_key = 'Hodge_rotation',
+    rotation_vkey = 'rotation_velocity',
+    density = 4,
+    alpha=0.5,
+    **kwargs
+    ):
+    
+    kwargs_arg = check_arguments(adata,basis = basis)
+    basis = kwargs_arg['basis']
+    
+    fig,ax = plt.subplots(1,3,figsize=(24,8),tight_layout=True)
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=vkey, title='RNA velocity',ax=ax[0],
+                                     show=False,density=density,alpha=alpha,fontsize=18,legend_fontsize=16, legend_loc=None,arrow_size=2,linewidth=2)
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=potential_vkey, title='Potential flow',ax=ax[1],
+                                     show=False,density=density,alpha=alpha,fontsize=18,legend_fontsize=16, legend_loc=None,arrow_size=2,linewidth=2)
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rotation_vkey, title='Rotational flow',ax=ax[2],
+                                     show=False,density=density,alpha=alpha,fontsize=18,legend_fontsize=16, legend_loc=None,arrow_size=2,linewidth=2)
+
+
+def view_surface_genes(
     adata,
     genes,
     exp_key = None,
+    basis = 'umap',
     vel_key  = 'velocity',
-    basis = 'X_umap',
     potential_key = 'Hodge_potential',
     graph_key = 'CM_graph',
     cluster_key = None,
     show_graph = False,
     cutedge_vol  = None,
     cutedge_length = None,
     logscale_vel = True,
@@ -524,14 +604,15 @@
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
                              potential_key = potential_key,
                              graph_key = graph_key,
                             )
     basis = kwargs_arg['basis']
+    basis_key = 'X_%s' % basis
     
     if exp_key == None:
         if scipy.sparse.issparse(adata.X):
             exp_HD = adata.X.toarray()
         else:
             exp_HD = adata.X
     elif exp_key in adata.obsm.keys():
@@ -541,15 +622,15 @@
     
     vel_HD = adata.obsm[vel_key] if vel_key in adata.obsm.keys() else adata.layers[vel_key]
     if logscale_vel:
         vel_HD = (1e+4*vel_HD.T/adata.obs['n_counts'].values).T/np.power(2,exp_HD)
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
     
-    data_pos = adata.obsm[basis]
+    data_pos = adata.obsm[basis_key]
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
     
     for gene in genes:
         fig,ax = plt.subplots(1,3,figsize=(45,10))
         cntr = ax[0].tricontourf(tri_,np.squeeze(exp_HD[:,adata.var.index==gene]),cmap=kwargs['cmap'],levels=100,zorder=2)
         fig.colorbar(cntr, shrink=0.75, orientation='vertical',ax=ax[0]).set_label('gene expression',fontsize=20)
         ax[0].set_title('%s_expression' % gene,fontsize=18)
@@ -572,15 +653,15 @@
                     for c in np.unique(cluster):
                         txt = ax[ax_i].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=20,ha='center', va='center',fontweight='bold')
                         txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
                         texts.append(txt)
 
 def view_surface_3D(
     adata,
-    basis = 'X_umap',
+    basis = 'umap',
     potential_key = 'Hodge_potential',
     graph_key = 'CM_graph',
     cluster_key = None,
     cutedge_vol  = 1,
     cutedge_length = 1,
     elev = 30,
     azim = -60,
@@ -591,19 +672,20 @@
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
                              potential_key = potential_key,
                              graph_key = graph_key,
                             )
     basis = kwargs_arg['basis']
+    basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
 
-    data_pos = adata.obsm[basis]
+    data_pos = adata.obsm[basis_key]
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
     fig = plt.figure(figsize=(15,15))
     ax = fig.add_subplot(111, projection='3d')
     cntr = ax.plot_trisurf(tri_,adata.obs[potential_key],cmap=kwargs['cmap'],zorder=2)
     ax.set_box_aspect(aspect = (1,1,0.8))
     fig.colorbar(cntr, shrink=0.5, orientation='vertical').set_label(potential_key,fontsize=20)
     ax.set_title(title,fontsize=18)
@@ -618,15 +700,15 @@
         # from adjustText import adjust_text
         # adjust_text(texts)
     ax.view_init(elev=elev, azim=azim)
 
 
 def view_surface_3D_cluster(
     adata,
-    basis = 'X_umap',
+    basis = 'umap',
     potential_key = 'Hodge_potential',
     graph_key = 'CM_graph',
     cluster_key = 'clusters',
     cutedge_vol  = 1,
     cutedge_length = 1,
     elev = 30,
     azim = -60,
@@ -639,15 +721,17 @@
     if cluster_key in adata.obs.keys():
         kwargs_arg = check_arguments(adata,
                                  basis = basis,
                                  potential_key = potential_key,
                                  graph_key = graph_key,
                                 )
         basis = kwargs_arg['basis']
-        data_pos = adata.obsm[basis]
+        basis_key = 'X_%s' % basis
+
+        data_pos = adata.obsm[basis_key]
         tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
         if 'cmap' not in kwargs:
             kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
         fig = plt.figure(figsize=(15,15))
         ax = fig.add_subplot(111, projection='3d')
         cntr = ax.plot_trisurf(tri_,adata.obs[potential_key],cmap=kwargs['cmap'],zorder=2,alpha=0.9)#,cmap=cmap_CellMap,levels=100)
         ax.set_box_aspect(aspect = (1,1,0.8))
@@ -682,34 +766,35 @@
     else:
         print('There is no cluster key \"%s\" in adata.obs' % cluster_key)
 
 
 def write(
     adata,
     filename = 'CellMap',
-    basis = 'X_umap',
+    basis = 'umap',
     potential_key = 'Hodge_potential',
     cluster_key = 'clusters',
     obs_key = None,
     genes = None,
     expression_key = None,
     use_HVG = True,
     n_HVG = 10,
 ):
     kwargs = check_arguments(adata,basis=basis,potential_key=potential_key,cluster_key=cluster_key,obs_key=obs_key,genes=genes,expression_key=expression_key)
     basis,obs_key,genes = kwargs['basis'],kwargs['obs_key'],kwargs['genes']
+    basis_key = 'X_%s' % basis
     
     if expression_key == None:
         if scipy.sparse.issparse(adata.X): data_exp = adata.X.toarray()
         else: data_exp = adata.X
     else:
         data_exp = adata.layers[expression_key]
     
     pd_out = pd.DataFrame({
-        'X':adata.obsm[basis][:,0],'Y':adata.obsm[basis][:,1],
+        'X':adata.obsm[basis_key][:,0],'Y':adata.obsm[basis_key][:,1],
         'Potential':adata.obs[potential_key],
         'Annotation':adata.obs[cluster_key]
     },index=adata.obs.index)
     pd_out.index.name='CellID'
     
     if obs_key != None:
         for arg in obs_key:
@@ -733,15 +818,15 @@
     display(pd_out)
     
     pd_out.to_csv('%s.csv' % filename)
 
 
 def create_dgraph_potential(
     adata,
-    basis = 'X_umap',
+    basis = 'umap',
     map_key = None,
     potential_key = 'Hodge_potential',
     graph_key = 'CM_graph',
     cutedge_vol  = None,
     cutedge_length = None,
     ):
     """
@@ -755,16 +840,17 @@
     """
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
                              map_key = map_key
                             )
     basis,map_key = kwargs_arg['basis'],kwargs_arg['map_key']
+    basis_key = 'X_%s' % basis
     
-    data_pos = adata.obsm[basis]
+    data_pos = adata.obsm[basis_key]
     triangles = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length).triangles
     tri_,idx_tri = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
     triangles = tri_.triangles[idx_tri]
     n_node_ = data_pos.shape[0]
     graph_ = scipy.sparse.lil_matrix(np.zeros([n_node_,n_node_]))
     idx_set = [[0,1],[1,2],[2,0]]
     # idx = np.isnan(data_vel[0])==False
@@ -774,19 +860,16 @@
         graph_[tuple(triangles[weight>min_weight][:,[id_x,id_y]].T[::-1])] = 1
         graph_[tuple(triangles[weight<-min_weight][:,[id_y,id_x]].T[::-1])] = 1
     return scipy.sparse.coo_matrix(graph_)
 
 
 def create_dgraph(
     adata,
-    basis = 'X_umap',
-    vel_key  = 'velocity_umap',
-    map_key = None,
-    potential_key = 'Hodge_potential',
-    graph_key = 'CM_graph',
+    basis = 'umap',
+    vel_key  = 'velocity',
     cutedge_vol  = None,
     cutedge_length = None,
     ):
     """
     Hodge decomposition
 
     Parameters
@@ -798,18 +881,18 @@
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
                              vel_key = vel_key,
                              map_key = map_key
                             )
     basis,vel_key,map_key = kwargs_arg['basis'],kwargs_arg['vel_key'],kwargs_arg['map_key']
+    basis_key = 'X_%s' % basis
     
-    data_pos = adata.obsm[basis]
-    data_vel = adata.obsm[vel_key]
-    map_pos  = adata.obsm[map_key][:,:2]
+    data_pos = adata.obsm[basis_key]
+    data_vel = adata.obsm['%s_%s' % (vel_key,basis)]
     triangles = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length).triangles
     tri_,idx_tri = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
     triangles = tri_.triangles[idx_tri]
     n_node_ = data_pos.shape[0]
     graph_ = scipy.sparse.lil_matrix(np.zeros([n_node_,n_node_]))
     idx_set = [[0,1],[1,2],[2,0]]
     idx = np.isnan(data_vel[0])==False
```

## Comparing `cellmap-1.0.1.dev202304020858.dist-info/METADATA` & `cellmap-1.0.1.dev202304101155.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304020858
+Version: 1.0.1.dev202304101155
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

