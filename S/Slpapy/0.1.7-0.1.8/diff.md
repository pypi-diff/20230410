# Comparing `tmp/Slpapy-0.1.7.tar.gz` & `tmp/Slpapy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.1.7.tar", last modified: Thu Apr  6 10:30:02 2023, max compression
+gzip compressed data, was "Slpapy-0.1.8.tar", last modified: Mon Apr 10 03:56:31 2023, max compression
```

## Comparing `Slpapy-0.1.7.tar` & `Slpapy-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 10:30:02.070856 Slpapy-0.1.7/
--rw-rw-rw-   0        0        0      159 2023-04-06 10:30:02.070856 Slpapy-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 10:30:02.060856 Slpapy-0.1.7/Slpapy/
--rw-rw-rw-   0        0        0      836 2023-04-06 10:29:52.000000 Slpapy-0.1.7/Slpapy/MZ_ppm_match.py
--rw-rw-rw-   0        0        0      453 2023-04-06 10:17:32.000000 Slpapy-0.1.7/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     6760 2023-04-06 10:29:25.000000 Slpapy-0.1.7/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:30:02.068856 Slpapy-0.1.7/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-04-06 10:30:01.000000 Slpapy-0.1.7/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-06 10:30:01.000000 Slpapy-0.1.7/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 10:30:01.000000 Slpapy-0.1.7/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-06 10:30:01.000000 Slpapy-0.1.7/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-06 10:30:01.000000 Slpapy-0.1.7/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 10:30:02.070856 Slpapy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-04-06 10:29:34.000000 Slpapy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:56:31.844361 Slpapy-0.1.8/
+-rw-rw-rw-   0        0        0      159 2023-04-10 03:56:31.843361 Slpapy-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 03:56:31.832360 Slpapy-0.1.8/Slpapy/
+-rw-rw-rw-   0        0        0     1924 2023-04-10 03:20:00.000000 Slpapy-0.1.8/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.8/Slpapy/MZ_ppm_match.py
+-rw-rw-rw-   0        0        0      453 2023-04-06 10:17:32.000000 Slpapy-0.1.8/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5164 2023-04-10 03:33:43.000000 Slpapy-0.1.8/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:56:31.841361 Slpapy-0.1.8/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 03:56:31.844361 Slpapy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      486 2023-04-10 03:56:14.000000 Slpapy-0.1.8/setup.py
```

### Comparing `Slpapy-0.1.7/Slpapy/MZ_ppm_match.py` & `Slpapy-0.1.8/Slpapy/MZ_ppm_match.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import pandas as pd
 import numpy as np
-import os
+import pandas as pd
 
 
 def Match_mz_value(lib, data, ppm):
+    lib = str(lib)
+    data = str(data)
+    lib = pd.read_csv(f'{lib}', header=0, low_memory=False)
+    data = pd.read_csv(f'{data}', header=0, low_memory=False)
     list = pd.DataFrame()
     list['lib'] = lib
     list['up'] = (ppm / 1000000) * list['lib'] + list['lib']
     list['low'] = -((ppm / 1000000) * list['lib'] - list['lib'])
     list['m/z'] = np.nan
     for i in range(len(lib)):
         for j in range(len(data)):
             if list.loc[i, 'up'] > data[j] > list.loc[i, 'low']:
-                if [abs(list.loc[i, 'lib'] - list.loc[i, 'm/z']) > abs(list.loc[i, 'lib'] - data[j])] or list.loc[i, 'm/z'] == np.nan:
-                    list.loc[i, 'number'] = j+3
+                if [abs(list.loc[i, 'lib'] - list.loc[i, 'm/z']) > abs(list.loc[i, 'lib'] - data[j])] or list.loc[
+                    i, 'm/z'] == np.nan:
+                    list.loc[i, 'number'] = j + 3
                     list.loc[i, 'm/z'] = data[j]
-                    list.loc[i, 'error_ppm'] = (abs(list.loc[i, 'lib'] - data[j])/list.loc[i, 'lib'])*1000000
+                    list.loc[i, 'error_ppm'] = (abs(list.loc[i, 'lib'] - data[j]) / list.loc[i, 'lib']) * 1000000
     list.to_csv('Match_mz_value.csv')
     return list
-
-
```

### Comparing `Slpapy-0.1.7/Slpapy/processing_analyze.py` & `Slpapy-0.1.8/Slpapy/processing_analyze.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,60 +10,15 @@
 from sklearn.cluster import KMeans
 
 sc.settings.verbosity = 3  # 设置日志等级: errors (0), warnings (1), info (2), hints (3)
 sc.logging.print_header()
 sc.settings.set_figure_params(dpi=720, facecolor='white')
 
 
-def resave(input_file, head):
-    # 指定输入和输出文件路径
-    input_file = str(input_file)
-    output_file = f'{input_file}' + "-1.csv"
-
-    # 增加字段大小限制
-    csv.field_size_limit(104857600)  # 1MB
-
-    # 打开输入和输出文件
-    with open(input_file, 'r', encoding='utf-8') as input_csv_file, open(output_file, 'w', newline='',
-                                                                         encoding='utf-8') as output_csv_file:
-        # 创建CSV读取器和写入器对象
-        input_csv_reader = csv.reader(input_csv_file, delimiter=';')
-        output_csv_writer = csv.writer(output_csv_file)
-
-        # 跳过前6行
-        for _ in range(int(head)):
-            next(input_csv_reader)
-
-        # 逐行读取并写入新的CSV文件
-        for row in input_csv_reader:
-            output_csv_writer.writerow(row)
-
-
-def Data_reconstruction(TIC, XY):
-    TIC = str(TIC)
-    XY = str(XY)
-    # 文件修整重排
-    resave(TIC, 9)
-    resave(XY, 7)
-    # 重新读取并转换保存为AnnData对象
-    df = pd.read_csv(f'{TIC}' + "-1.csv", header=1, index_col='m/z', low_memory=False)
-    df1 = pd.read_csv(f'{XY}' + "-1.csv", header=1, index_col='Spot index', low_memory=False)
-    # 建一个基本的 AnnData 对象
-    counts = csr_matrix(df.T, dtype=np.float32)
-    adata = ad.AnnData(counts)
-    # 为x和y轴提供索引
-    adata.obs_names = df.columns
-    adata.var['m/z'] = df.index
-    print(adata.obs_names[:])
-    print(adata.var_names[:])
-    # 标注坐标位置
-    adata.obs["X"] = df1.x.values
-    adata.obs["Y"] = df1.y.values
-    adata.write(f'{XY}' + ".h5ad")
-    return adata
+
 
 
 def XYadata(adata):
     df = preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])
     counts = csr_matrix(df, dtype=np.float32)
     XYmatrix = ad.AnnData(counts)
     # 为x和y轴提供索引
@@ -80,36 +35,40 @@
     # 显示在所有细胞中在每个单细胞中产生最高计数分数的脂质
     # sc.pl.highest_expr_genes(adata, n_top=20, save='_highest_expr_protein.png')
     # 小提琴图：表达基因的数量，每个细胞包含的表达量，线粒体基因表达量的百分比。
     adata.var['mt'] = adata.var_names.str.startswith('MT-')  # 将线粒体基因标记为 mt
     sc.pp.calculate_qc_metrics(adata, qc_vars=['mt'], percent_top=None,
                                log1p=False, inplace=True)
     sc.pl.violin(adata, 'total_counts', jitter=0.4, multi_panel=True,
-                 save='_n_genes_by_counts_and_total_counts_and_pct_counts_mt.png')
+                 save='_total_counts.png')
     # 归一化，使得不同细胞样本间可比
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     # 存储数据
     adata.raw = adata
     sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
     sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
     adata = adata[:, adata.var.highly_variable]
     # 回归每个细胞的总计数和表达的线粒体基因的百分比的影响。
-    sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
+    #sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
+    mz=pd.DataFrame()
+    #保存mz值
+    mz['mz']=adata.var_names
+    mz.to_csv('mz.csv')
     adata.write('./pp_done.h5ad')
     return adata
 
 
 def se_analyze(adata):
-    # 将每个基因缩放到单位方差。阈值超过标准偏差 10。
-    sc.pp.scale(adata, max_value=10)
+    # 将每个脂质缩放到单位方差。阈值超过标准偏差 10。，如非高斯分布，则不建议使用
+    #sc.pp.scale(adata, max_value=10)
     # 绘制 PCA 图降维
     sc.tl.pca(adata, svd_solver='arpack')  #
     # Neighborhood graph使用数据矩阵的 PCA 表示来计算细胞的邻域图
-    sc.pp.neighbors(adata, n_neighbors=20, n_pcs=50, )
+    sc.pp.neighbors(adata, n_neighbors=20, n_pcs=30, )
     # sc.pp.neighbors(adata, n_neighbors=20, n_pcs=30, )#YONG
     sc.tl.umap(adata, min_dist=0.3, alpha=10, spread=1)  #
     # Leiden 图聚类
     # 计算
     sc.tl.leiden(adata, resolution=0.3)
     return adata
```

