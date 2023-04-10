# Comparing `tmp/cellsnake-0.2.0.dev8.tar.gz` & `tmp/cellsnake-0.2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellsnake-0.2.0.dev8.tar", last modified: Sun Apr  9 00:36:01 2023, max compression
+gzip compressed data, was "cellsnake-0.2.0.dev9.tar", last modified: Mon Apr 10 13:54:49 2023, max compression
```

## Comparing `cellsnake-0.2.0.dev8.tar` & `cellsnake-0.2.0.dev9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.573568 cellsnake-0.2.0.dev8/
--rw-r--r--   0 sium       (501) staff       (20)     1072 2022-12-02 21:30:51.000000 cellsnake-0.2.0.dev8/LICENSE
--rw-r--r--   0 sium       (501) staff       (20)      300 2023-02-22 13:59:41.000000 cellsnake-0.2.0.dev8/MANIFEST.in
--rw-r--r--   0 sium       (501) staff       (20)     4906 2023-04-09 00:36:01.573360 cellsnake-0.2.0.dev8/PKG-INFO
--rw-r--r--   0 sium       (501) staff       (20)     4458 2023-04-04 13:27:36.000000 cellsnake-0.2.0.dev8/README.md
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.562278 cellsnake-0.2.0.dev8/cellsnake/
--rw-r--r--   0 sium       (501) staff       (20)        0 2022-12-02 21:33:29.000000 cellsnake-0.2.0.dev8/cellsnake/__init__.py
--rw-r--r--   0 sium       (501) staff       (20)        0 2023-02-01 12:33:26.000000 cellsnake-0.2.0.dev8/cellsnake/cellsnake_functions.py
--rwxr-xr-x   0 sium       (501) staff       (20)    13703 2023-04-07 13:12:53.000000 cellsnake-0.2.0.dev8/cellsnake/command_line.py
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.563704 cellsnake-0.2.0.dev8/cellsnake/scrna/
--rw-r--r--   0 sium       (501) staff       (20)     2362 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/config.yaml
--rwxr-xr-x   0 sium       (501) staff       (20)       55 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/install_r_packages.sh
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.563866 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/
--rw-r--r--   0 sium       (501) staff       (20)    23558 2023-04-09 00:07:09.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/Snakefile
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.564062 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/bundle/
--rw-r--r--   0 sium       (501) staff       (20)  2786711 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.559868 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.566297 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.566459 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/
--rw-r--r--   0 sium       (501) staff       (20)     8522 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py
--rwxr-xr-x   0 sium       (501) staff       (20)     4148 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py
--rwxr-xr-x   0 sium       (501) staff       (20)     8607 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/k2sc.py
--rwxr-xr-x   0 sium       (501) staff       (20)     4158 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.567688 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/
--rw-r--r--   0 sium       (501) staff       (20)     2179 2023-02-08 21:49:02.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/extra_functions.smk
--rw-r--r--   0 sium       (501) staff       (20)      351 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/integration.smk
--rw-r--r--   0 sium       (501) staff       (20)     5712 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/microbiome.smk
--rw-r--r--   0 sium       (501) staff       (20)     1050 2022-12-02 22:51:49.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/params_detect.smk
--rw-r--r--   0 sium       (501) staff       (20)      181 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/params_write.smk
--rw-r--r--   0 sium       (501) staff       (20)    20702 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/seurat.smk
--rw-r--r--   0 sium       (501) staff       (20)      306 2023-04-09 00:07:09.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/subset.smk
--rw-r--r--   0 sium       (501) staff       (20)     1337 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/test.smk
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.573109 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/
--rwxr-xr-x   0 sium       (501) staff       (20)     3016 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-cellchat.R
--rwxr-xr-x   0 sium       (501) staff       (20)    17388 2023-02-27 13:17:03.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3319 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-celltypist.R
--rwxr-xr-x   0 sium       (501) staff       (20)      761 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-celltypist.py
--rwxr-xr-x   0 sium       (501) staff       (20)     4459 2023-02-28 14:02:58.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1132 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1241 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3449 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-dimplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1828 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-dotplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1714 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-find-markers.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3563 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R
--rwxr-xr-x   0 sium       (501) staff       (20)     6918 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-functions.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3205 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2212 2023-02-20 22:44:59.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-gsea.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2945 2022-12-03 20:20:58.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-harmony.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2648 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-install-packages.R
--rwxr-xr-x   0 sium       (501) staff       (20)     4595 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kegg.R
--rwxr-xr-x   0 sium       (501) staff       (20)     4464 2023-01-31 11:27:53.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py
--rwxr-xr-x   0 sium       (501) staff       (20)     2937 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1952 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3289 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1253 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2461 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-metrics.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2835 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3375 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2497 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-monocle3.R
--rwxr-xr-x   0 sium       (501) staff       (20)        0 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-music-decon.R
--rwxr-xr-x   0 sium       (501) staff       (20)     6679 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R
--rwxr-xr-x   0 sium       (501) staff       (20)     6898 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-read-qc.R
--rwxr-xr-x   0 sium       (501) staff       (20)     4568 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2068 2023-04-04 09:59:25.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2636 2023-03-22 10:39:26.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3548 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1363 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-technicals.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1703 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1217 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-volcano.R
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.563337 cellsnake-0.2.0.dev8/cellsnake.egg-info/
--rw-r--r--   0 sium       (501) staff       (20)     4906 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/PKG-INFO
--rw-r--r--   0 sium       (501) staff       (20)     3123 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/SOURCES.txt
--rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/dependency_links.txt
--rw-r--r--   0 sium       (501) staff       (20)       58 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/entry_points.txt
--rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/not-zip-safe
--rw-r--r--   0 sium       (501) staff       (20)      159 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/requires.txt
--rw-r--r--   0 sium       (501) staff       (20)       10 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/top_level.txt
--rw-r--r--   0 sium       (501) staff       (20)      152 2023-03-28 08:51:31.000000 cellsnake-0.2.0.dev8/reqs.txt
--rw-r--r--   0 sium       (501) staff       (20)      159 2023-03-28 12:37:22.000000 cellsnake-0.2.0.dev8/requirements.txt
--rw-r--r--   0 sium       (501) staff       (20)       38 2023-04-09 00:36:01.573615 cellsnake-0.2.0.dev8/setup.cfg
--rw-r--r--   0 sium       (501) staff       (20)     1674 2023-04-07 13:10:17.000000 cellsnake-0.2.0.dev8/setup.py
--rw-r--r--   0 sium       (501) staff       (20)   953080 2023-02-27 13:02:47.000000 cellsnake-0.2.0.dev8/test_counts.txt
--rw-r--r--   0 sium       (501) staff       (20)      340 2023-02-27 13:02:48.000000 cellsnake-0.2.0.dev8/test_meta.txt
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.687710 cellsnake-0.2.0.dev9/
+-rw-r--r--   0 sium       (501) staff       (20)     1072 2022-12-02 21:30:51.000000 cellsnake-0.2.0.dev9/LICENSE
+-rw-r--r--   0 sium       (501) staff       (20)      300 2023-02-22 13:59:41.000000 cellsnake-0.2.0.dev9/MANIFEST.in
+-rw-r--r--   0 sium       (501) staff       (20)     4906 2023-04-10 13:54:49.687497 cellsnake-0.2.0.dev9/PKG-INFO
+-rw-r--r--   0 sium       (501) staff       (20)     4458 2023-04-04 13:27:36.000000 cellsnake-0.2.0.dev9/README.md
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.677093 cellsnake-0.2.0.dev9/cellsnake/
+-rw-r--r--   0 sium       (501) staff       (20)        0 2022-12-02 21:33:29.000000 cellsnake-0.2.0.dev9/cellsnake/__init__.py
+-rw-r--r--   0 sium       (501) staff       (20)        0 2023-02-01 12:33:26.000000 cellsnake-0.2.0.dev9/cellsnake/cellsnake_functions.py
+-rwxr-xr-x   0 sium       (501) staff       (20)    13703 2023-04-10 13:53:11.000000 cellsnake-0.2.0.dev9/cellsnake/command_line.py
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.678251 cellsnake-0.2.0.dev9/cellsnake/scrna/
+-rw-r--r--   0 sium       (501) staff       (20)     2362 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/config.yaml
+-rwxr-xr-x   0 sium       (501) staff       (20)       55 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/install_r_packages.sh
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.678373 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/
+-rw-r--r--   0 sium       (501) staff       (20)    23558 2023-04-09 00:07:09.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/Snakefile
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.678527 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/bundle/
+-rw-r--r--   0 sium       (501) staff       (20)  2786711 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.674775 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.680910 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.681055 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/
+-rw-r--r--   0 sium       (501) staff       (20)     8522 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     4148 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     8607 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/k2sc.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     4158 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.682176 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/
+-rw-r--r--   0 sium       (501) staff       (20)     2179 2023-02-08 21:49:02.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/extra_functions.smk
+-rw-r--r--   0 sium       (501) staff       (20)      351 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/integration.smk
+-rw-r--r--   0 sium       (501) staff       (20)     5712 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/microbiome.smk
+-rw-r--r--   0 sium       (501) staff       (20)     1050 2022-12-02 22:51:49.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/params_detect.smk
+-rw-r--r--   0 sium       (501) staff       (20)      181 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/params_write.smk
+-rw-r--r--   0 sium       (501) staff       (20)    20702 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/seurat.smk
+-rw-r--r--   0 sium       (501) staff       (20)      306 2023-04-09 00:07:09.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/subset.smk
+-rw-r--r--   0 sium       (501) staff       (20)     1337 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/test.smk
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.687263 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/
+-rwxr-xr-x   0 sium       (501) staff       (20)     3016 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-cellchat.R
+-rwxr-xr-x   0 sium       (501) staff       (20)    17388 2023-02-27 13:17:03.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3319 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-celltypist.R
+-rwxr-xr-x   0 sium       (501) staff       (20)      761 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-celltypist.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     4459 2023-02-28 14:02:58.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1132 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1241 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3449 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-dimplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1828 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-dotplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1714 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-find-markers.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3563 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     7044 2023-04-10 13:12:21.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-functions.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3205 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2212 2023-02-20 22:44:59.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-gsea.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2945 2022-12-03 20:20:58.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-harmony.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2648 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-install-packages.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4595 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kegg.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4464 2023-01-31 11:27:53.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     2937 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1952 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3289 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1253 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2461 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-metrics.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2835 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3375 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2497 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-monocle3.R
+-rwxr-xr-x   0 sium       (501) staff       (20)        0 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-music-decon.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     6808 2023-04-10 13:12:21.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     6898 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-read-qc.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4568 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2068 2023-04-04 09:59:25.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2636 2023-03-22 10:39:26.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3548 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1363 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-technicals.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1703 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1217 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-volcano.R
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.677996 cellsnake-0.2.0.dev9/cellsnake.egg-info/
+-rw-r--r--   0 sium       (501) staff       (20)     4906 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/PKG-INFO
+-rw-r--r--   0 sium       (501) staff       (20)     3123 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/SOURCES.txt
+-rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/dependency_links.txt
+-rw-r--r--   0 sium       (501) staff       (20)       58 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/entry_points.txt
+-rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/not-zip-safe
+-rw-r--r--   0 sium       (501) staff       (20)      159 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/requires.txt
+-rw-r--r--   0 sium       (501) staff       (20)       10 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/top_level.txt
+-rw-r--r--   0 sium       (501) staff       (20)      152 2023-03-28 08:51:31.000000 cellsnake-0.2.0.dev9/reqs.txt
+-rw-r--r--   0 sium       (501) staff       (20)      159 2023-03-28 12:37:22.000000 cellsnake-0.2.0.dev9/requirements.txt
+-rw-r--r--   0 sium       (501) staff       (20)       38 2023-04-10 13:54:49.687766 cellsnake-0.2.0.dev9/setup.cfg
+-rw-r--r--   0 sium       (501) staff       (20)     1674 2023-04-10 13:53:06.000000 cellsnake-0.2.0.dev9/setup.py
+-rw-r--r--   0 sium       (501) staff       (20)   953080 2023-02-27 13:02:47.000000 cellsnake-0.2.0.dev9/test_counts.txt
+-rw-r--r--   0 sium       (501) staff       (20)      340 2023-02-27 13:02:48.000000 cellsnake-0.2.0.dev9/test_meta.txt
```

### Comparing `cellsnake-0.2.0.dev8/LICENSE` & `cellsnake-0.2.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/PKG-INFO` & `cellsnake-0.2.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellsnake
-Version: 0.2.0.dev8
+Version: 0.2.0.dev9
 Summary: cellsnake
 Home-page: https://github.com/sinanugur/cellsnake
 Author: Sinan U. Umu
 Author-email: sinanugur@gmail.com
 Keywords: scRNA single-cell RNA analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cellsnake-0.2.0.dev8/README.md` & `cellsnake-0.2.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/command_line.py` & `cellsnake-0.2.0.dev9/cellsnake/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 import cellsnake
 cellsnake_path=os.path.dirname(cellsnake.__file__)
 options = ["clustree","clusteringTree","minimal","standard","advanced"] #and integration
 
 
 __author__ = 'Sinan U. Umu'
-__version__= '0.2.0.dev8'
+__version__= '0.2.0.dev9'
 __logo__="""
              _  _                     _           
             | || |                   | |          
   ___   ___ | || | ___  _ __    __ _ | | __  ___  
  / __| / _ \| || |/ __|| '_ \  / _` || |/ / / _ \ 
 | (__ |  __/| || |\__ \| | | || (_| ||   < |  __/ 
  \___| \___||_||_||___/|_| |_| \__,_||_|\_\ \___|
```

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/config.yaml` & `cellsnake-0.2.0.dev9/cellsnake/scrna/config.yaml`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/Snakefile` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/Snakefile`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/k2sc.py` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/k2sc.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/extra_functions.smk` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/extra_functions.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/microbiome.smk` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/microbiome.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/params_detect.smk` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/params_detect.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/seurat.smk` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/seurat.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/test.smk` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/test.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-cellchat.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-cellchat.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-celltypist.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-celltypist.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-celltypist.py` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-celltypist.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-dimplot.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-dimplot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-dotplot.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-dotplot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-find-markers.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-find-markers.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-functions.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-functions.R`

 * *Files 2% similar despite different names*

```diff
@@ -445,11 +445,13 @@
   if (n <= 10) {
     return(palette10)
   }
   if (n > 50 && n <= 75) {
     return(palette75)
   }
 
-
+  if (!requireNamespace("randomcoloR", quietly = TRUE)) {
+    remotes::install_github("chris-mcginnis-ucsf/DoubletFinder")
+  }
 
   randomcoloR::distinctColorPalette(n)
 }
```

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-gsea.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-gsea.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-harmony.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-harmony.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-install-packages.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-install-packages.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kegg.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kegg.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-metrics.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-metrics.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-monocle3.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-monocle3.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,17 @@
 if (opt$tsne) {
   scrna <- RunTSNE(scrna, dims = 1:dimensionReduction, check_duplicates = FALSE)
 }
 
 
 
 if (opt$doublet.filter) {
+  if (!requireNamespace("DoubletFinder", quietly = TRUE)) {
+    remotes::install_github("chris-mcginnis-ucsf/DoubletFinder")
+  }
   require(DoubletFinder)
 
   homotypic.prop <- modelHomotypic(scrna$seurat_clusters)
   nExp_poi <- round(0.075 * nrow(scrna@meta.data)) ## Assuming 7.5% doublet formation rate - tailor for your dataset
   nExp_poi.adj <- round(nExp_poi * (1 - homotypic.prop))
 
   ## Run DoubletFinder with varying classification stringencies ----------------------------------------------------------------
```

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-read-qc.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-read-qc.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-technicals.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-technicals.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-volcano.R` & `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-volcano.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/cellsnake.egg-info/PKG-INFO` & `cellsnake-0.2.0.dev9/cellsnake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellsnake
-Version: 0.2.0.dev8
+Version: 0.2.0.dev9
 Summary: cellsnake
 Home-page: https://github.com/sinanugur/cellsnake
 Author: Sinan U. Umu
 Author-email: sinanugur@gmail.com
 Keywords: scRNA single-cell RNA analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cellsnake-0.2.0.dev8/cellsnake.egg-info/SOURCES.txt` & `cellsnake-0.2.0.dev9/cellsnake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev8/setup.py` & `cellsnake-0.2.0.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 with open("README.md","r") as readme:
     long_description=readme.read()
 
 setup(
     name="cellsnake",
-    version="0.2.0.dev8",
+    version="0.2.0.dev9",
     packages=find_packages(exclude=('tests*','testing*')),
     long_description=long_description,
     long_description_content_type="text/markdown",
     #extras_require={"dev":["pytest>=3.7"]},
     install_requires=requirements,
     include_package_data=True,
     zip_safe=False,
```

### Comparing `cellsnake-0.2.0.dev8/test_counts.txt` & `cellsnake-0.2.0.dev9/test_counts.txt`

 * *Files identical despite different names*

