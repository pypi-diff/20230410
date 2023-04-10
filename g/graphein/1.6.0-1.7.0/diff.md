# Comparing `tmp/graphein-1.6.0.tar.gz` & `tmp/graphein-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/graphein-1.6.0.tar", last modified: Sat Mar 18 20:04:57 2023, max compression
+gzip compressed data, was "graphein-1.7.0.tar", last modified: Mon Apr 10 16:06:12 2023, max compression
```

## Comparing `graphein-1.6.0.tar` & `graphein-1.7.0.tar`

### file list

```diff
@@ -1,217 +1,225 @@
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/.requirements/
--rw-r--r--   0 arianjamasb   (501) staff       (20)      250 2023-03-18 20:04:36.000000 graphein-1.6.0/.requirements/base.in
--rw-r--r--   0 arianjamasb   (501) staff       (20)      131 2022-08-01 23:49:57.000000 graphein-1.6.0/.requirements/dev.in
--rw-r--r--   0 arianjamasb   (501) staff       (20)      185 2023-03-18 20:04:36.000000 graphein-1.6.0/.requirements/docs.in
--rw-r--r--   0 arianjamasb   (501) staff       (20)       76 2023-03-18 20:04:36.000000 graphein-1.6.0/.requirements/extras.in
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1074 2023-03-18 20:04:36.000000 graphein-1.6.0/LICENSE
--rw-r--r--   0 arianjamasb   (501) staff       (20)      170 2023-03-18 20:04:36.000000 graphein-1.6.0/MANIFEST.in
--rw-r--r--   0 arianjamasb   (501) staff       (20)    20752 2023-03-18 20:04:57.000000 graphein-1.6.0/PKG-INFO
--rw-r--r--   0 arianjamasb   (501) staff       (20)    17385 2023-03-18 20:04:36.000000 graphein-1.6.0/README.md
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/
--rw-r--r--   0 arianjamasb   (501) staff       (20)      773 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1546 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/cli.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/grn/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/grn/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2448 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/grn/config.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2932 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/grn/edges.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/grn/features/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/grn/features/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1191 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/grn/features/node_features.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5542 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/grn/graphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     8784 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/grn/parse_regnetwork.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4844 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/grn/parse_trrust.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/ml/
--rw-r--r--   0 arianjamasb   (501) staff       (20)      371 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/ml/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    23533 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/ml/clustering.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    15666 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ml/conversion.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/ml/datasets/
--rw-r--r--   0 arianjamasb   (501) staff       (20)      128 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/ml/datasets/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    28325 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ml/datasets/torch_geometric_dataset.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3523 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/ml/diffusion.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/ml/metrics/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       70 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ml/metrics/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4047 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ml/metrics/gdt.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2908 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ml/metrics/tm_score.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)      829 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/ml/utils.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4912 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ml/visualisation.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/molecule/
--rw-r--r--   0 arianjamasb   (501) staff       (20)      181 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     9566 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/atoms.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1880 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/chembl.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3449 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/config.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/molecule/edges/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       46 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/edges/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1080 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/molecule/edges/atomic.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5273 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/molecule/edges/distance.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/molecule/features/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       63 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/features/__init__.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/molecule/features/edges/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       21 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/features/edges/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4426 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/molecule/features/edges/bonds.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/molecule/features/graph/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       24 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/features/graph/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4206 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/features/graph/molecule.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/molecule/features/nodes/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       25 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/features/nodes/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    10208 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/features/nodes/atom_type.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    15060 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/molecule/graphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    14611 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/utils.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5898 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/visualisation.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3427 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/molecule/zinc.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/ppi/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/ppi/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     9820 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/ppi/config.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2785 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ppi/edges.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/ppi/features/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/ppi/features/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2476 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ppi/features/node_features.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2644 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ppi/graph_metadata.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5010 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ppi/graphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    10238 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ppi/parse_biogrid.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     6354 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/ppi/parse_stringdb.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     7569 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/ppi/visualisation.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/protein/
--rw-r--r--   0 arianjamasb   (501) staff       (20)      551 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    10435 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/analysis.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     9696 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/config.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/protein/edges/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       76 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/edges/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    12698 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/edges/atomic.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    47106 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/edges/distance.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    10128 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/edges/intramolecular.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/protein/features/
--rw-r--r--   0 arianjamasb   (501) staff       (20)      140 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/__init__.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/protein/features/data/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/data/__init__.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/protein/features/graph/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       49 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/graph/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1521 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/graph/dynamics.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2033 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/graph/structure.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/protein/features/nodes/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       70 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/nodes/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1940 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/features/nodes/aaindex.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     8475 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/features/nodes/amino_acid.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     7076 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/nodes/amino_acid_properties.csv
--rw-r--r--   0 arianjamasb   (501) staff       (20)     8019 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/features/nodes/dssp.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     6319 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/features/nodes/geometry.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)      843 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/nodes/meiler_embeddings.csv
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/protein/features/pretrained_models/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/pretrained_models/__init__.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/protein/features/sequence/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       92 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/sequence/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    10532 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/features/sequence/embeddings.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    60796 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/features/sequence/propy.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3981 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/sequence/sequence.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4412 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/features/sequence/utils.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2280 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/features/utils.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2709 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/folding_utils.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    44708 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/graphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     7527 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/protein/meshes.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    69642 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/resi_atoms.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    29741 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/subgraphs.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/protein/tensor/
--rw-r--r--   0 arianjamasb   (501) staff       (20)      317 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    16877 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/angles.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    51845 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/data.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3117 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/dataloader.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    21274 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/dataset.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5903 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/edges.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    12810 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/geometry.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    15887 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/io.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3354 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/plot.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    13105 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/pnerf.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     8769 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/reconstruction.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4939 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/representation.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     8678 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/sequence.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     6191 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/testing.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5848 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/tensor/types.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    15801 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/utils.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    34682 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/protein/visualisation.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/rna/
--rw-r--r--   0 arianjamasb   (501) staff       (20)      143 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/rna/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3458 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/rna/config.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     6049 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/rna/constants.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/rna/edges/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       74 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/rna/edges/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4749 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/rna/edges/atomic.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5674 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/rna/edges/base_pairing.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)       74 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/rna/edges/distance.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/rna/features/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/rna/features/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1305 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/rna/features/atom.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    13449 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/rna/graphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5362 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/rna/nussinov.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    18809 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/rna/subgraphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1960 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/rna/utils.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2559 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/rna/visualisation.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/testing/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       21 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/testing/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     6405 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/testing/utils.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/utils/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/utils/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1213 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/utils/config.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3100 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/utils/config_parser.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein/utils/pymol/
--rw-r--r--   0 arianjamasb   (501) staff       (20)       20 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/utils/pymol/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)      112 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/utils/pymol/compat.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3068 2022-08-01 23:49:57.000000 graphein-1.6.0/graphein/utils/pymol/core.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    13835 2023-03-18 20:04:36.000000 graphein-1.6.0/graphein/utils/utils.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/graphein.egg-info/
--rw-r--r--   0 arianjamasb   (501) staff       (20)    20752 2023-03-18 20:04:56.000000 graphein-1.6.0/graphein.egg-info/PKG-INFO
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5435 2023-03-18 20:04:56.000000 graphein-1.6.0/graphein.egg-info/SOURCES.txt
--rw-r--r--   0 arianjamasb   (501) staff       (20)        1 2023-03-18 20:04:56.000000 graphein-1.6.0/graphein.egg-info/dependency_links.txt
--rw-r--r--   0 arianjamasb   (501) staff       (20)       48 2023-03-18 20:04:56.000000 graphein-1.6.0/graphein.egg-info/entry_points.txt
--rw-r--r--   0 arianjamasb   (501) staff       (20)      667 2023-03-18 20:04:56.000000 graphein-1.6.0/graphein.egg-info/requires.txt
--rw-r--r--   0 arianjamasb   (501) staff       (20)       15 2023-03-18 20:04:56.000000 graphein-1.6.0/graphein.egg-info/top_level.txt
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1081 2022-08-01 23:49:58.000000 graphein-1.6.0/pyproject.toml
--rw-r--r--   0 arianjamasb   (501) staff       (20)       38 2023-03-18 20:04:57.000000 graphein-1.6.0/setup.cfg
--rw-r--r--   0 arianjamasb   (501) staff       (20)     5590 2023-03-18 20:04:36.000000 graphein-1.6.0/setup.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/__init__.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/grn/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/grn/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1258 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/grn/test_graphs.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/ml/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/ml/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2544 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/ml/test_conversion.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3033 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/ml/test_torch_geometric_dataset.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/ppi/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/ppi/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1601 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/ppi/test_graphs.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/protein/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/protein/__init__.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/protein/edges/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/protein/edges/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    12961 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/edges/test_distance.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/protein/nodes/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/protein/nodes/__init__.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/protein/nodes/features/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/protein/nodes/features/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     7140 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/protein/nodes/features/test_amino_acid.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4371 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/protein/nodes/features/test_geometry.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/protein/tensor/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/tensor/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     4362 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/tensor/test_angles.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)      424 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/tensor/test_data.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2937 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/tensor/test_geometry.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3218 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/tensor/test_io.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)      989 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/tensor/test_reconstruction.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2458 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/tensor/test_representation.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1056 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/tensor/test_sequence.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    17994 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/test_graphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)    12342 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/protein/test_subgraphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3075 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/protein/test_utils.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/rna/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/rna/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     3396 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/rna/test_graphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)      355 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/rna/test_nussinov.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     9377 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/rna/test_subgraphs.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)      293 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/test_graphein.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/testing/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/testing/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     2786 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/testing/utils.py
-drwxr-xr-x   0 arianjamasb   (501) staff       (20)        0 2023-03-18 20:04:57.000000 graphein-1.6.0/tests/utils/
--rw-r--r--   0 arianjamasb   (501) staff       (20)        0 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/utils/__init__.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1005 2023-03-18 20:04:36.000000 graphein-1.6.0/tests/utils/test_cli.py
--rw-r--r--   0 arianjamasb   (501) staff       (20)     1325 2022-08-01 23:49:58.000000 graphein-1.6.0/tests/utils/test_yml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.608590 graphein-1.7.0/.requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-10 16:05:54.000000 graphein-1.7.0/.requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-10 16:05:54.000000 graphein-1.7.0/.requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 16:05:54.000000 graphein-1.7.0/.requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-10 16:05:54.000000 graphein-1.7.0/.requirements/extras.in
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 16:05:54.000000 graphein-1.7.0/.requirements/torch_cpu.in
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 16:05:54.000000 graphein-1.7.0/.requirements/torch_gpu.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-10 16:05:54.000000 graphein-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 16:05:54.000000 graphein-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-04-10 16:06:12.624590 graphein-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-04-10 16:05:54.000000 graphein-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.608590 graphein-1.7.0/graphein/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.608590 graphein-1.7.0/graphein/grn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/grn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/grn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/grn/edges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.608590 graphein-1.7.0/graphein/grn/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/grn/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/grn/features/node_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/grn/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/grn/parse_regnetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/grn/parse_trrust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.608590 graphein-1.7.0/graphein/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23451 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15673 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.608590 graphein-1.7.0/graphein/ml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/datasets/foldcomp_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68512 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/datasets/pdb_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28220 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/datasets/torch_geometric_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.612590 graphein-1.7.0/graphein/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/metrics/gdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/metrics/tm_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ml/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.612590 graphein-1.7.0/graphein/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/chembl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.612590 graphein-1.7.0/graphein/molecule/edges/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/edges/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/edges/distance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.612590 graphein-1.7.0/graphein/molecule/features/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.612590 graphein-1.7.0/graphein/molecule/features/edges/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/features/edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/features/edges/bonds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.612590 graphein-1.7.0/graphein/molecule/features/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/features/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/features/graph/molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.612590 graphein-1.7.0/graphein/molecule/features/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/features/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/features/nodes/atom_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/molecule/zinc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.612590 graphein-1.7.0/graphein/ppi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/edges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.612590 graphein-1.7.0/graphein/ppi/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/features/node_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/graph_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/parse_biogrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/parse_stringdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/ppi/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.616590 graphein-1.7.0/graphein/protein/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.616590 graphein-1.7.0/graphein/protein/edges/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/edges/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47106 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/edges/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/edges/intramolecular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.616590 graphein-1.7.0/graphein/protein/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.616590 graphein-1.7.0/graphein/protein/features/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.616590 graphein-1.7.0/graphein/protein/features/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/graph/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/graph/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.616590 graphein-1.7.0/graphein/protein/features/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/nodes/aaindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/nodes/amino_acid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/nodes/amino_acid_properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/nodes/dssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/nodes/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/nodes/meiler_embeddings.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.616590 graphein-1.7.0/graphein/protein/features/pretrained_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/pretrained_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.616590 graphein-1.7.0/graphein/protein/features/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/sequence/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60796 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/sequence/propy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/sequence/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/sequence/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/folding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69642 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/resi_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29741 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/subgraphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/graphein/protein/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51950 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/pnerf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/tensor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34710 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/protein/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/graphein/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/graphein/rna/edges/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/edges/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/edges/base_pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/edges/distance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/graphein/rna/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/features/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/nussinov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18809 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/subgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/rna/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/graphein/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/graphein/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/utils/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/utils/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/graphein/utils/pymol/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/utils/pymol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/utils/pymol/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/utils/pymol/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-04-10 16:05:55.000000 graphein-1.7.0/graphein/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.608590 graphein-1.7.0/graphein.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-04-10 16:06:12.000000 graphein-1.7.0/graphein.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-10 16:06:12.000000 graphein-1.7.0/graphein.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:06:12.000000 graphein-1.7.0/graphein.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 16:06:12.000000 graphein-1.7.0/graphein.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-10 16:06:12.000000 graphein-1.7.0/graphein.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 16:06:12.000000 graphein-1.7.0/graphein.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-10 16:05:55.000000 graphein-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:06:12.624590 graphein-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-10 16:05:55.000000 graphein-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/datasets/pdb_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.620590 graphein-1.7.0/tests/grn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/grn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/grn/test_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/ml/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/ml/test_torch_geometric_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/ppi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/ppi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/ppi/test_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/protein/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/protein/edges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/edges/test_distance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/protein/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/protein/nodes/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/nodes/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/nodes/features/test_amino_acid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/nodes/features/test_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/protein/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/tensor/test_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/tensor/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/tensor/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/tensor/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/tensor/test_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/tensor/test_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/tensor/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/test_subgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/protein/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/rna/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/rna/test_nussinov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/rna/test_subgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/test_graphein.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:06:12.624590 graphein-1.7.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/utils/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-10 16:05:55.000000 graphein-1.7.0/tests/utils/test_yml_parser.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `graphein-1.6.0/LICENSE` & `graphein-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/PKG-INFO` & `graphein-1.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,290 +1,19 @@
 Metadata-Version: 2.1
 Name: graphein
-Version: 1.6.0
+Version: 1.7.0
 Summary: Protein & Interactomic Graph Construction for Machine Learning
 Home-page: https://github.com/a-r-j/graphein
 Author: Arian Jamasb
 Author-email: arian@jamasb.io
 License: MIT
 Project-URL: homepage, https://github.com/a-r-j/graphein
 Project-URL: changelog, https://github.com/a-r-j/graphein/blob/master/CHANGELOG.md
 Project-URL: issue, https://github.com/a-r-j/graphein/issues
 Project-URL: documentation, https://graphein.ai/
-Description: 
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/a-r-j/graphein-binder/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fa-r-j%252Fgraphein%26urlpath%3Dlab%252Ftree%252Fgraphein%252Fnotebooks%26branch%3Dmaster)
-        [![PyPI version](https://badge.fury.io/py/graphein.svg)](https://badge.fury.io/py/graphein)
-        ![supported python versions](https://img.shields.io/pypi/pyversions/graphein)
-        [![Docs](https://assets.readthedocs.org/static/projects/badges/passing-flat.svg)](http://www.graphein.ai)
-        [![DOI:10.1101/2020.07.15.204701](https://zenodo.org/badge/DOI/10.1101/2020.07.15.204701.svg)](https://doi.org/10.1101/2020.07.15.204701)
-        [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
-        [![CodeFactor](https://www.codefactor.io/repository/github/a-r-j/graphein/badge)](https://www.codefactor.io/repository/github/a-r-j/graphein)
-        [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=a-r-j_graphein&metric=alert_status)](https://sonarcloud.io/dashboard?id=a-r-j_graphein)
-        [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=a-r-j_graphein&metric=bugs)](https://sonarcloud.io/dashboard?id=a-r-j_graphein)
-        [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=a-r-j_graphein&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=a-r-j_graphein)
-        [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=a-r-j_graphein&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=a-r-j_graphein)
-        [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/graphein)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-        
-        <p align="center">
-          <a href="https://www.graphein.ai/#gh-light-mode-only">
-            <img src="./imgs/graphein.png" width="100%"/>
-          </a>
-          <a href="https://www.graphein.ai/#gh-dark-mode-only">
-            <img src="./imgs/graphein_dark.png" width="100%"/>
-          </a>
-        </p>
-        
-        <br></br>
-        
-        [Documentation](http://www.graphein.ai) | [Paper](https://www.biorxiv.org/content/10.1101/2020.07.15.204701v1) | [Tutorials](http://graphein.ai/notebooks_index.html) | [Installation](#installation)
-        
-        Protein & Interactomic Graph Library
-        
-        This package provides functionality for producing geometric representations of protein and RNA structures, and biological interaction networks. We provide compatibility with standard PyData formats, as well as graph objects designed for ease of use with popular deep learning libraries.
-        
-        ## What's New?
-        
-        |   |   |
-        |---|---|
-        | [Protein Tensor Module](http://graphein.ai/notebooks/protein_tensors.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_tensors.ipynb)   |
-        | [Constructing molecular graphs](http://graphein.ai/notebooks/molecule_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/molecule_tutorial.ipynb)   |
-        | [Ready-to-go Dataloaders for PyTorch Geometric](http://graphein.ai/notebooks/dataloader_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/dataloader_tutorial.ipynb)   |
-        | [Extracting subgraphs from protein graphs](http://graphein.ai/notebooks/subgraphing_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/subgraphing_tutorial.ipynb)   |
-        | [Protein Graph Analytics](http://graphein.ai/notebooks/protein_graph_analytics.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_graph_analytics.ipynb) |
-        | [Graphein CLI](http://graphein.ai/getting_started/usage.html)  |   |
-        | [Protein Graph Creation from AlphaFold2!](http://graphein.ai/notebooks/alphafold_protein_graph_tutorial.html)  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) |
-        | [Protein Graph Visualisation!](http://graphein.ai/notebooks/interactive_plotly_example.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/interactive_plotly_example.ipynb)
-        | [RNA Graph Construction from Dotbracket notation](http://graphein.ai/modules/graphein.rna.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/rna_graph_tutorial.ipynb) |
-        | [Protein - Protein Interaction Network Support & Structural Interactomics (Using AlphaFold2!)](http://graphein.ai/notebooks/ppi_tutorial.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/ppi_graph.ipynb) |
-        | [High and Low-level API for massive flexibility - create your own bespoke workflows!](http://graphein.ai/notebooks/residue_graphs.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) |
-        
-        ## Example usage
-        
-        Graphein provides both a programmatic API and a command-line interface for constructing graphs.
-        
-        ### CLI
-        
-        Graphein configs can be specified as `.yaml` files to batch process graphs from the commandline.
-        
-        [Docs](http://graphein.ai/getting_started/usage.html)
-        
-        ```bash
-        graphein -c config.yaml -p path/to/pdbs -o path/to/output
-        ```
-        
-        ### Creating a Protein Graph
-        
-        |   |   |   |
-        |---|---|---|
-        [Tutorial (Residue-level)](http://graphein.ai/notebooks/residue_graphs.html) | [Tutorial (Atomic)](http://graphein.ai/notebooks/atom_graph_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.protein.html#module-graphein.protein.graphs)
-        | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) | [![Open In Colab(https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/atom_graph_tutorial.ipynb) | |
-        
-        ```python
-        from graphein.protein.config import ProteinGraphConfig
-        from graphein.protein.graphs import construct_graph
-        
-        config = ProteinGraphConfig()
-        g = construct_graph(config=config, pdb_code="3eiy")
-        ```
-        
-        ### Creating a Protein Graph from the AlphaFold Protein Structure Database
-        
-        |   |   |
-        |---|---|
-        | [Tutorial](http://graphein.ai/notebooks/alphafold_protein_graph_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.protein.html#module-graphein.protein.graphs) |
-        | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb)|
-        
-        ```python
-        from graphein.protein.config import ProteinGraphConfig
-        from graphein.protein.graphs import construct_graph
-        from graphein.protein.utils import download_alphafold_structure
-        
-        config = ProteinGraphConfig()
-        fp = download_alphafold_structure("Q5VSL9", aligned_score=False)
-        g = construct_graph(config=config, pdb_path=fp)
-        ```
-        
-        ### Creating a Protein Mesh
-        
-        |   |   |
-        |---|---|
-        | [Tutorial](http://graphein.ai/notebooks/protein_mesh_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.protein.html#module-graphein.protein.meshes) |
-        | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_mesh_tutorial.ipynb) | |
-        
-        ```python
-        from graphein.protein.config import ProteinMeshConfig
-        from graphein.protein.meshes import create_mesh
-        
-        verts, faces, aux = create_mesh(pdb_code="3eiy", config=config)
-        ```
-        
-        ### Creating Molecular Graphs
-        
-        Graphein can create molecular graphs from smiles strings as well as `.sdf`, `.mol2`, and `.pdb` files
-        
-        |   |   |
-        |---|---|
-        | [Tutorial](http://graphein.ai/notebooks/molecule_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.molecule.html) |
-        | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/molecule_tutorial.ipynb) | |
-        
-        ```python
-        from graphein.molecule.config import MoleculeGraphConfig
-        from graphein.molecule.graphs import construct_graph
-        
-        g = create_graph(smiles="CC(=O)OC1=CC=CC=C1C(=O)O", config=config)
-        
-        ```
-        
-        ### Creating an RNA Graph
-        
-        |   |   |
-        |---|---|
-        |[Tutorial](http://graphein.ai/notebooks/rna_notebooks.html) | [Docs](http://graphein.ai/modules/graphein.rna.html) |
-        |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/rna_graph_tutorial.ipynb) | |
-        
-        ```python
-        from graphein.rna.graphs import construct_rna_graph
-        # Build the graph from a dotbracket & optional sequence
-        rna = construct_rna_graph(dotbracket='..(((((..(((...)))..)))))...',
-                                  sequence='UUGGAGUACACAACCUGUACACUCUUUC')
-        ```
-        
-        ### Creating a Protein-Protein Interaction Graph
-        
-        |   |   |
-        |---|---|
-        | [Tutorial](http://graphein.ai/notebooks/ppi_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.ppi.html) |
-        | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/ppi_graph.ipynb)|
-        
-        ```python
-        from graphein.ppi.config import PPIGraphConfig
-        from graphein.ppi.graphs import compute_ppi_graph
-        from graphein.ppi.edges import add_string_edges, add_biogrid_edges
-        
-        config = PPIGraphConfig()
-        protein_list = ["CDC42", "CDK1", "KIF23", "PLK1", "RAC2", "RACGAP1", "RHOA", "RHOB"]
-        
-        g = compute_ppi_graph(config=config,
-                              protein_list=protein_list,
-                              edge_construction_funcs=[add_string_edges, add_biogrid_edges]
-                             )
-        ```
-        
-        ### Creating a Gene Regulatory Network Graph
-        
-        |   |   |
-        |---|---|
-        |[Tutorial](http://graphein.ai/notebooks/grn_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.grn.html) |
-        | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/grn_tutorial.ipynb) |
-        
-        ```python
-        from graphein.grn.config import GRNGraphConfig
-        from graphein.grn.graphs import compute_grn_graph
-        from graphein.grn.edges import add_regnetwork_edges, add_trrust_edges
-        
-        config = GRNGraphConfig()
-        gene_list = ["AATF", "MYC", "USF1", "SP1", "TP53", "DUSP1"]
-        
-        g = compute_grn_graph(
-            gene_list=gene_list,
-            edge_construction_funcs=[
-                partial(add_trrust_edges, trrust_filtering_funcs=config.trrust_config.filtering_functions),
-                partial(add_regnetwork_edges, regnetwork_filtering_funcs=config.regnetwork_config.filtering_functions),
-            ],
-        )
-        ```
-        
-        ## Installation
-        
-        ### Pip
-        
-        The simplest install is via pip. *N.B this does not install ML/DL libraries which are required for conversion to their data formats and for generating protein structure meshes with PyTorch 3D.* [Further details](http://graphein.ai//getting_started/installation.html)
-        
-        ```bash
-        pip install graphein # For base install
-        pip install graphein[extras] # For additional featurisation dependencies
-        pip install graphein[dev] # For dev dependencies
-        pip install graphein[all] # To get the lot
-        ```
-        
-        However, there are a number of (optional) utilities ([DSSP](https://anaconda.org/salilab/dssp), [PyMol](https://pymol.org/2/), [GetContacts](https://getcontacts.github.io/)) that are not available via PyPI:
-        
-        ```
-        conda install -c salilab dssp # Required for computing secondary structural features
-        conda install -c schrodinger pymol # Required for PyMol visualisations & mesh generation
-        
-        # GetContacts - used as an alternative way to compute intramolecular interactions
-        conda install -c conda-forge vmd-python
-        git clone https://github.com/getcontacts/getcontacts
-        
-        # Add folder to PATH
-        echo "export PATH=\$PATH:`pwd`/getcontacts" >> ~/.bashrc
-        source ~/.bashrc
-        To test the installation, run:
-        
-        cd getcontacts/example/5xnd
-        get_dynamic_contacts.py --topology 5xnd_topology.pdb \
-                                --trajectory 5xnd_trajectory.dcd \
-                                --itypes hb \
-                                --output 5xnd_hbonds.tsv
-        ```
-        
-        ### Conda environment
-        
-        The dev environment includes GPU Builds (CUDA 11.1) for each of the deep learning libraries integrated into graphein.
-        
-        ```bash
-        git clone https://www.github.com/a-r-j/graphein
-        cd graphein
-        conda env create -f environment-dev.yml
-        pip install -e .
-        ```
-        
-        A lighter install can be performed with:
-        
-        ```bash
-        git clone https://www.github.com/a-r-j/graphein
-        cd graphein
-        conda env create -f environment.yml
-        pip install -e .
-        ```
-        
-        ### Dockerfile
-        
-        We provide two `docker-compose` files for CPU (`docker-compose.cpu.yml`) and GPU usage (`docker-compose.yml`) locally. For GPU usage please ensure that you have [NVIDIA Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html) installed. Ensure that you install the locally mounted volume after entering the container (`pip install -e .`). This will also setup the dev environment locally.
-        
-        To build (GPU) run:
-        
-        ```
-        docker-compose up -d --build # start the container
-        docker-compose down # stop the container
-        ```
-        
-        ## Citing Graphein
-        
-        Please consider citing graphein if it proves useful in your work.
-        
-        ```bibtex
-        @article {Jamasb2020.07.15.204701,
-         author = {Jamasb, Arian R. and Vi{\~n}as, Ramon and Ma, Eric J. and Harris, Charlie and Huang, Kexin and Hall, Dominic and Li{\'o}, Pietro and Blundell, Tom L.},
-         title = {Graphein - a Python Library for Geometric Deep Learning and Network Analysis on Protein Structures and Interaction Networks},
-         elocation-id = {2020.07.15.204701},
-         year = {2021},
-         doi = {10.1101/2020.07.15.204701},
-         publisher = {Cold Spring Harbor Laboratory},
-         abstract = {Geometric deep learning has well-motivated applications in the context of biology, a domain where relational structure in datasets can be meaningfully leveraged. Currently, efforts in both geometric deep learning and, more broadly, deep learning applied to biomolecular tasks have been hampered by a scarcity of appropriate datasets accessible to domain specialists and machine learning researchers alike. However, there has been little exploration of how to best to integrate and construct geometric representations of these datatypes. To address this, we introduce Graphein as a turn-key tool for transforming raw data from widely-used bioinformatics databases into machine learning-ready datasets in a high-throughput and flexible manner. Graphein is a Python library for constructing graph and surface-mesh representations of protein structures and biological interaction networks for computational analysis. Graphein provides utilities for data retrieval from widely-used bioinformatics databases for structural data, including the Protein Data Bank, the recently-released AlphaFold Structure Database, and for biomolecular interaction networks from STRINGdb, BioGrid, TRRUST and RegNetwork. The library interfaces with popular geometric deep learning libraries: DGL, PyTorch Geometric and PyTorch3D though remains framework agnostic as it is built on top of the PyData ecosystem to enable inter-operability with scientific computing tools and libraries. Graphein is designed to be highly flexible, allowing the user to specify each step of the data preparation, scalable to facilitate working with large protein complexes and interaction graphs, and contains useful pre-processing tools for preparing experimental files. Graphein facilitates network-based, graph-theoretic and topological analyses of structural and interaction datasets in a high-throughput manner. As example workflows, we make available two new protein structure-related datasets, previously unused by the geometric deep learning community. We envision that Graphein will facilitate developments in computational biology, graph representation learning and drug discovery.Availability and implementation Graphein is written in Python. Source code, example usage and tutorials, datasets, and documentation are made freely available under the MIT License at the following URL: graphein.aiCompeting Interest StatementThe authors have declared no competing interest.},
-         URL = {https://www.biorxiv.org/content/early/2021/10/12/2020.07.15.204701},
-         eprint = {https://www.biorxiv.org/content/early/2021/10/12/2020.07.15.204701.full.pdf},
-         journal = {bioRxiv}
-        }
-        
-        ```
-        
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
@@ -295,7 +24,277 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: extras
 Provides-Extra: all
+License-File: LICENSE
+
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/a-r-j/graphein-binder/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fa-r-j%252Fgraphein%26urlpath%3Dlab%252Ftree%252Fgraphein%252Fnotebooks%26branch%3Dmaster)
+[![PyPI version](https://badge.fury.io/py/graphein.svg)](https://badge.fury.io/py/graphein)
+![supported python versions](https://img.shields.io/pypi/pyversions/graphein)
+[![Docs](https://assets.readthedocs.org/static/projects/badges/passing-flat.svg)](http://www.graphein.ai)
+[![DOI:10.1101/2020.07.15.204701](https://zenodo.org/badge/DOI/10.1101/2020.07.15.204701.svg)](https://doi.org/10.1101/2020.07.15.204701)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![CodeFactor](https://www.codefactor.io/repository/github/a-r-j/graphein/badge)](https://www.codefactor.io/repository/github/a-r-j/graphein)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=a-r-j_graphein&metric=alert_status)](https://sonarcloud.io/dashboard?id=a-r-j_graphein)
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=a-r-j_graphein&metric=bugs)](https://sonarcloud.io/dashboard?id=a-r-j_graphein)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=a-r-j_graphein&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=a-r-j_graphein)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=a-r-j_graphein&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=a-r-j_graphein)
+[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/graphein)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+
+<p align="center">
+  <a href="https://www.graphein.ai/#gh-light-mode-only">
+    <img src="./imgs/graphein.png" width="100%"/>
+  </a>
+  <a href="https://www.graphein.ai/#gh-dark-mode-only">
+    <img src="./imgs/graphein_dark.png" width="100%"/>
+  </a>
+</p>
+
+<br></br>
+
+[Documentation](http://www.graphein.ai) | [Paper](https://www.biorxiv.org/content/10.1101/2020.07.15.204701v1) | [Tutorials](http://graphein.ai/notebooks_index.html) | [Installation](#installation)
+
+Protein & Interactomic Graph Library
+
+This package provides functionality for producing geometric representations of protein and RNA structures, and biological interaction networks. We provide compatibility with standard PyData formats, as well as graph objects designed for ease of use with popular deep learning libraries.
+
+## What's New?
+
+|   |   |   |
+|---|---|---|
+| 1.7.0 | [FoldComp Datasets](http://graphein.ai/notebooks/foldcomp.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/foldcomp.ipynb)   |
+| 1.7.0 | [Creating Datasets from the PDB](http://graphein.ai/notebooks/creating_datasets_from_the_pdb.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/creating_datasets_from_the_pdb.ipynb)   |
+| 1.6.0 | [Protein Tensor Module](http://graphein.ai/notebooks/protein_tensors.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_tensors.ipynb)   |
+| 1.5.0 | [Protein Graph Creation from AlphaFold2!](http://graphein.ai/notebooks/alphafold_protein_graph_tutorial.html)  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) |
+| 1.5.0 | [RNA Graph Construction from Dotbracket notation](http://graphein.ai/modules/graphein.rna.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/rna_graph_tutorial.ipynb) |
+| 1.4.0 | [Constructing molecular graphs](http://graphein.ai/notebooks/molecule_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/molecule_tutorial.ipynb)   |
+| 1.3.0 | [Ready-to-go Dataloaders for PyTorch Geometric](http://graphein.ai/notebooks/dataloader_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/dataloader_tutorial.ipynb)   |
+| 1.2.0 | [Extracting subgraphs from protein graphs](http://graphein.ai/notebooks/subgraphing_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/subgraphing_tutorial.ipynb)   |
+| 1.2.0 | [Protein Graph Analytics](http://graphein.ai/notebooks/protein_graph_analytics.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_graph_analytics.ipynb) |
+| 1.2.0 | [Graphein CLI](http://graphein.ai/getting_started/usage.html)  |   |
+| 1.2.0 |[Protein Graph Visualisation!](http://graphein.ai/notebooks/interactive_plotly_example.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/interactive_plotly_example.ipynb)
+| 1.1.0 | [Protein - Protein Interaction Network Support & Structural Interactomics (Using AlphaFold2!)](http://graphein.ai/notebooks/ppi_tutorial.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/ppi_graph.ipynb) |
+| 1.0.0 | [High and Low-level API for massive flexibility - create your own bespoke workflows!](http://graphein.ai/notebooks/residue_graphs.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) |
+
+## Example usage
+
+Graphein provides both a programmatic API and a command-line interface for constructing graphs.
+
+### CLI
+
+Graphein configs can be specified as `.yaml` files to batch process graphs from the commandline.
+
+[Docs](http://graphein.ai/getting_started/usage.html)
+
+```bash
+graphein -c config.yaml -p path/to/pdbs -o path/to/output
+```
+
+### Creating a Protein Graph
+
+|   |   |   |
+|---|---|---|
+[Tutorial (Residue-level)](http://graphein.ai/notebooks/residue_graphs.html) | [Tutorial (Atomic)](http://graphein.ai/notebooks/atom_graph_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.protein.html#module-graphein.protein.graphs)
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) | [![Open In Colab(https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/atom_graph_tutorial.ipynb) | |
+
+```python
+from graphein.protein.config import ProteinGraphConfig
+from graphein.protein.graphs import construct_graph
+
+config = ProteinGraphConfig()
+g = construct_graph(config=config, pdb_code="3eiy")
+```
+
+### Creating a Protein Graph from the AlphaFold Protein Structure Database
+
+|   |   |
+|---|---|
+| [Tutorial](http://graphein.ai/notebooks/alphafold_protein_graph_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.protein.html#module-graphein.protein.graphs) |
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb)|
+
+```python
+from graphein.protein.config import ProteinGraphConfig
+from graphein.protein.graphs import construct_graph
+from graphein.protein.utils import download_alphafold_structure
+
+config = ProteinGraphConfig()
+fp = download_alphafold_structure("Q5VSL9", aligned_score=False)
+g = construct_graph(config=config, path=fp)
+```
+
+### Creating a Protein Mesh
+
+|   |   |
+|---|---|
+| [Tutorial](http://graphein.ai/notebooks/protein_mesh_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.protein.html#module-graphein.protein.meshes) |
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_mesh_tutorial.ipynb) | |
+
+```python
+from graphein.protein.config import ProteinMeshConfig
+from graphein.protein.meshes import create_mesh
+
+verts, faces, aux = create_mesh(pdb_code="3eiy", config=config)
+```
+
+### Creating Molecular Graphs
+
+Graphein can create molecular graphs from smiles strings as well as `.sdf`, `.mol2`, and `.pdb` files
+
+|   |   |
+|---|---|
+| [Tutorial](http://graphein.ai/notebooks/molecule_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.molecule.html) |
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/molecule_tutorial.ipynb) | |
+
+```python
+from graphein.molecule.config import MoleculeGraphConfig
+from graphein.molecule.graphs import construct_graph
+
+g = create_graph(smiles="CC(=O)OC1=CC=CC=C1C(=O)O", config=config)
+
+```
+
+### Creating an RNA Graph
+
+|   |   |
+|---|---|
+|[Tutorial](http://graphein.ai/notebooks/rna_notebooks.html) | [Docs](http://graphein.ai/modules/graphein.rna.html) |
+|[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/rna_graph_tutorial.ipynb) | |
+
+```python
+from graphein.rna.graphs import construct_rna_graph
+# Build the graph from a dotbracket & optional sequence
+rna = construct_rna_graph(dotbracket='..(((((..(((...)))..)))))...',
+                          sequence='UUGGAGUACACAACCUGUACACUCUUUC')
+```
+
+### Creating a Protein-Protein Interaction Graph
+
+|   |   |
+|---|---|
+| [Tutorial](http://graphein.ai/notebooks/ppi_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.ppi.html) |
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/ppi_graph.ipynb)|
+
+```python
+from graphein.ppi.config import PPIGraphConfig
+from graphein.ppi.graphs import compute_ppi_graph
+from graphein.ppi.edges import add_string_edges, add_biogrid_edges
+
+config = PPIGraphConfig()
+protein_list = ["CDC42", "CDK1", "KIF23", "PLK1", "RAC2", "RACGAP1", "RHOA", "RHOB"]
+
+g = compute_ppi_graph(config=config,
+                      protein_list=protein_list,
+                      edge_construction_funcs=[add_string_edges, add_biogrid_edges]
+                     )
+```
+
+### Creating a Gene Regulatory Network Graph
+
+|   |   |
+|---|---|
+|[Tutorial](http://graphein.ai/notebooks/grn_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.grn.html) |
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/grn_tutorial.ipynb) |
+
+```python
+from graphein.grn.config import GRNGraphConfig
+from graphein.grn.graphs import compute_grn_graph
+from graphein.grn.edges import add_regnetwork_edges, add_trrust_edges
+
+config = GRNGraphConfig()
+gene_list = ["AATF", "MYC", "USF1", "SP1", "TP53", "DUSP1"]
+
+g = compute_grn_graph(
+    gene_list=gene_list,
+    edge_construction_funcs=[
+        partial(add_trrust_edges, trrust_filtering_funcs=config.trrust_config.filtering_functions),
+        partial(add_regnetwork_edges, regnetwork_filtering_funcs=config.regnetwork_config.filtering_functions),
+    ],
+)
+```
+
+## Installation
+
+### Pip
+
+The simplest install is via pip. *N.B this does not install ML/DL libraries which are required for conversion to their data formats and for generating protein structure meshes with PyTorch 3D.* [Further details](http://graphein.ai//getting_started/installation.html)
+
+```bash
+pip install graphein # For base install
+pip install graphein[extras] # For additional featurisation dependencies
+pip install graphein[dev] # For dev dependencies
+pip install graphein[all] # To get the lot
+```
+
+However, there are a number of (optional) utilities ([DSSP](https://anaconda.org/salilab/dssp), [PyMol](https://pymol.org/2/), [GetContacts](https://getcontacts.github.io/)) that are not available via PyPI:
+
+```
+conda install -c salilab dssp # Required for computing secondary structural features
+conda install -c schrodinger pymol # Required for PyMol visualisations & mesh generation
+
+# GetContacts - used as an alternative way to compute intramolecular interactions
+conda install -c conda-forge vmd-python
+git clone https://github.com/getcontacts/getcontacts
+
+# Add folder to PATH
+echo "export PATH=\$PATH:`pwd`/getcontacts" >> ~/.bashrc
+source ~/.bashrc
+To test the installation, run:
+
+cd getcontacts/example/5xnd
+get_dynamic_contacts.py --topology 5xnd_topology.pdb \
+                        --trajectory 5xnd_trajectory.dcd \
+                        --itypes hb \
+                        --output 5xnd_hbonds.tsv
+```
+
+### Conda environment
+
+The dev environment includes GPU Builds (CUDA 11.1) for each of the deep learning libraries integrated into graphein.
+
+```bash
+git clone https://www.github.com/a-r-j/graphein
+cd graphein
+conda env create -f environment-dev.yml
+pip install -e .
+```
+
+A lighter install can be performed with:
+
+```bash
+git clone https://www.github.com/a-r-j/graphein
+cd graphein
+conda env create -f environment.yml
+pip install -e .
+```
+
+### Dockerfile
+
+We provide two `docker-compose` files for CPU (`docker-compose.cpu.yml`) and GPU usage (`docker-compose.yml`) locally. For GPU usage please ensure that you have [NVIDIA Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html) installed. Ensure that you install the locally mounted volume after entering the container (`pip install -e .`). This will also setup the dev environment locally.
+
+To build (GPU) run:
+
+```
+docker-compose up -d --build # start the container
+docker-compose down # stop the container
+```
+
+## Citing Graphein
+
+Please consider citing graphein if it proves useful in your work.
+
+```bibtex
+@inproceedings{jamasb2022graphein,
+  title={Graphein - a Python Library for Geometric Deep Learning and Network Analysis on Biomolecular Structures and Interaction Networks},
+  author={Arian Rokkum Jamasb and Ramon Vi{\~n}as Torn{\'e} and Eric J Ma and Yuanqi Du and Charles Harris and Kexin Huang and Dominic Hall and Pietro Lio and Tom Leon Blundell},
+  booktitle={Advances in Neural Information Processing Systems},
+  editor={Alice H. Oh and Alekh Agarwal and Danielle Belgrave and Kyunghyun Cho},
+  year={2022},
+  url={https://openreview.net/forum?id=9xRZlV6GfOX}
+}
+
+```
```

#### html2text {}

```diff
@@ -1,16 +1,26 @@
-Metadata-Version: 2.1 Name: graphein Version: 1.6.0 Summary: Protein &
+Metadata-Version: 2.1 Name: graphein Version: 1.7.0 Summary: Protein &
 Interactomic Graph Construction for Machine Learning Home-page: https://
 github.com/a-r-j/graphein Author: Arian Jamasb Author-email: arian@jamasb.io
 License: MIT Project-URL: homepage, https://github.com/a-r-j/graphein Project-
 URL: changelog, https://github.com/a-r-j/graphein/blob/master/CHANGELOG.md
 Project-URL: issue, https://github.com/a-r-j/graphein/issues Project-URL:
-documentation, https://graphein.ai/ Description: [![Binder](https://
-mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/a-r-j/graphein-binder/
-master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fa-r-
+documentation, https://graphein.ai/ Platform: any Classifier: License :: OSI
+Approved :: MIT License Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
+System :: POSIX Classifier: Operating System :: Unix Classifier: Operating
+System :: MacOS Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: extras Provides-Extra: all License-File:
+LICENSE [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/
+v2/gh/a-r-j/graphein-binder/master?urlpath=git-
+pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fa-r-
 j%252Fgraphein%26urlpath%3Dlab%252Ftree%252Fgraphein%252Fnotebooks%26branch%3Dmaster)
 [![PyPI version](https://badge.fury.io/py/graphein.svg)](https://badge.fury.io/
 py/graphein) ![supported python versions](https://img.shields.io/pypi/
 pyversions/graphein) [![Docs](https://assets.readthedocs.org/static/projects/
 badges/passing-flat.svg)](http://www.graphein.ai) [![DOI:10.1101/
 2020.07.15.204701](https://zenodo.org/badge/DOI/10.1101/2020.07.15.204701.svg)]
 (https://doi.org/10.1101/2020.07.15.204701) [![Project Status: Active â The
@@ -39,84 +49,93 @@
 [Documentation](http://www.graphein.ai) | [Paper](https://www.biorxiv.org/
 content/10.1101/2020.07.15.204701v1) | [Tutorials](http://graphein.ai/
 notebooks_index.html) | [Installation](#installation) Protein & Interactomic
 Graph Library This package provides functionality for producing geometric
 representations of protein and RNA structures, and biological interaction
 networks. We provide compatibility with standard PyData formats, as well as
 graph objects designed for ease of use with popular deep learning libraries. ##
-What's New? | | | |---|---| | [Protein Tensor Module](http://graphein.ai/
-notebooks/protein_tensors.html) | [![Open In Colab](https://
+What's New? | | | | |---|---|---| | 1.7.0 | [FoldComp Datasets](http://
+graphein.ai/notebooks/foldcomp.html) | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-protein_tensors.ipynb) | | [Constructing molecular graphs](http://graphein.ai/
-notebooks/molecule_tutorial.html) | [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-molecule_tutorial.ipynb) | | [Ready-to-go Dataloaders for PyTorch Geometric]
-(http://graphein.ai/notebooks/dataloader_tutorial.html) | [![Open In Colab]
+foldcomp.ipynb) | | 1.7.0 | [Creating Datasets from the PDB](http://
+graphein.ai/notebooks/creating_datasets_from_the_pdb.html) | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-dataloader_tutorial.ipynb) | | [Extracting subgraphs from protein graphs](http:
-//graphein.ai/notebooks/subgraphing_tutorial.html) | [![Open In Colab](https://
+creating_datasets_from_the_pdb.ipynb) | | 1.6.0 | [Protein Tensor Module](http:
+//graphein.ai/notebooks/protein_tensors.html) | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-subgraphing_tutorial.ipynb) | | [Protein Graph Analytics](http://graphein.ai/
-notebooks/protein_graph_analytics.html) | [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-protein_graph_analytics.ipynb) | | [Graphein CLI](http://graphein.ai/
-getting_started/usage.html) | | | [Protein Graph Creation from AlphaFold2!]
+protein_tensors.ipynb) | | 1.5.0 | [Protein Graph Creation from AlphaFold2!]
 (http://graphein.ai/notebooks/alphafold_protein_graph_tutorial.html) | [![Open
 In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-residue_graphs.ipynb) | | [Protein Graph Visualisation!](http://graphein.ai/
-notebooks/interactive_plotly_example.html) | [![Open In Colab](https://
+residue_graphs.ipynb) | | 1.5.0 | [RNA Graph Construction from Dotbracket
+notation](http://graphein.ai/modules/graphein.rna.html) | [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+rna_graph_tutorial.ipynb) | | 1.4.0 | [Constructing molecular graphs](http://
+graphein.ai/notebooks/molecule_tutorial.html) | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-interactive_plotly_example.ipynb) | [RNA Graph Construction from Dotbracket
-notation](http://graphein.ai/modules/graphein.rna.html) | [![Open In Colab]
+molecule_tutorial.ipynb) | | 1.3.0 | [Ready-to-go Dataloaders for PyTorch
+Geometric](http://graphein.ai/notebooks/dataloader_tutorial.html) | [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+dataloader_tutorial.ipynb) | | 1.2.0 | [Extracting subgraphs from protein
+graphs](http://graphein.ai/notebooks/subgraphing_tutorial.html) | [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+subgraphing_tutorial.ipynb) | | 1.2.0 | [Protein Graph Analytics](http://
+graphein.ai/notebooks/protein_graph_analytics.html) | [![Open In Colab](https:/
+/colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+protein_graph_analytics.ipynb) | | 1.2.0 | [Graphein CLI](http://graphein.ai/
+getting_started/usage.html) | | | 1.2.0 |[Protein Graph Visualisation!](http://
+graphein.ai/notebooks/interactive_plotly_example.html) | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-rna_graph_tutorial.ipynb) | | [Protein - Protein Interaction Network Support &
-Structural Interactomics (Using AlphaFold2!)](http://graphein.ai/notebooks/
-ppi_tutorial.html) | [![Open In Colab](https://colab.research.google.com/
+interactive_plotly_example.ipynb) | 1.1.0 | [Protein - Protein Interaction
+Network Support & Structural Interactomics (Using AlphaFold2!)](http://
+graphein.ai/notebooks/ppi_tutorial.html) | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+ppi_graph.ipynb) | | 1.0.0 | [High and Low-level API for massive flexibility -
+create your own bespoke workflows!](http://graphein.ai/notebooks/
+residue_graphs.html) | [![Open In Colab](https://colab.research.google.com/
+assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/
+graphein/blob/master/notebooks/residue_graphs.ipynb) | ## Example usage
+Graphein provides both a programmatic API and a command-line interface for
+constructing graphs. ### CLI Graphein configs can be specified as `.yaml` files
+to batch process graphs from the commandline. [Docs](http://graphein.ai/
+getting_started/usage.html) ```bash graphein -c config.yaml -p path/to/pdbs -
+o path/to/output ``` ### Creating a Protein Graph | | | | |---|---|---|
+[Tutorial (Residue-level)](http://graphein.ai/notebooks/residue_graphs.html) |
+[Tutorial (Atomic)](http://graphein.ai/notebooks/atom_graph_tutorial.html) |
+[Docs](http://graphein.ai/modules/graphein.protein.html#module-
+graphein.protein.graphs) | [![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/
-graphein/blob/master/notebooks/ppi_graph.ipynb) | | [High and Low-level API for
-massive flexibility - create your own bespoke workflows!](http://graphein.ai/
-notebooks/residue_graphs.html) | [![Open In Colab](https://
+graphein/blob/master/notebooks/residue_graphs.ipynb) | [![Open In Colab(https:/
+/colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-residue_graphs.ipynb) | ## Example usage Graphein provides both a programmatic
-API and a command-line interface for constructing graphs. ### CLI Graphein
-configs can be specified as `.yaml` files to batch process graphs from the
-commandline. [Docs](http://graphein.ai/getting_started/usage.html) ```bash
-graphein -c config.yaml -p path/to/pdbs -o path/to/output ``` ### Creating a
-Protein Graph | | | | |---|---|---| [Tutorial (Residue-level)](http://
-graphein.ai/notebooks/residue_graphs.html) | [Tutorial (Atomic)](http://
-graphein.ai/notebooks/atom_graph_tutorial.html) | [Docs](http://graphein.ai/
-modules/graphein.protein.html#module-graphein.protein.graphs) | [![Open In
-Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+atom_graph_tutorial.ipynb) | | ```python from graphein.protein.config import
+ProteinGraphConfig from graphein.protein.graphs import construct_graph config =
+ProteinGraphConfig() g = construct_graph(config=config, pdb_code="3eiy") ```
+### Creating a Protein Graph from the AlphaFold Protein Structure Database | |
+| |---|---| | [Tutorial](http://graphein.ai/notebooks/
+alphafold_protein_graph_tutorial.html) | [Docs](http://graphein.ai/modules/
+graphein.protein.html#module-graphein.protein.graphs) | | [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-residue_graphs.ipynb) | [![Open In Colab(https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/
-master/notebooks/atom_graph_tutorial.ipynb) | | ```python from
-graphein.protein.config import ProteinGraphConfig from graphein.protein.graphs
-import construct_graph config = ProteinGraphConfig() g = construct_graph
-(config=config, pdb_code="3eiy") ``` ### Creating a Protein Graph from the
-AlphaFold Protein Structure Database | | | |---|---| | [Tutorial](http://
-graphein.ai/notebooks/alphafold_protein_graph_tutorial.html) | [Docs](http://
-graphein.ai/modules/graphein.protein.html#module-graphein.protein.graphs) | |
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
 residue_graphs.ipynb)| ```python from graphein.protein.config import
 ProteinGraphConfig from graphein.protein.graphs import construct_graph from
 graphein.protein.utils import download_alphafold_structure config =
 ProteinGraphConfig() fp = download_alphafold_structure("Q5VSL9",
-aligned_score=False) g = construct_graph(config=config, pdb_path=fp) ``` ###
+aligned_score=False) g = construct_graph(config=config, path=fp) ``` ###
 Creating a Protein Mesh | | | |---|---| | [Tutorial](http://graphein.ai/
 notebooks/protein_mesh_tutorial.html) | [Docs](http://graphein.ai/modules/
 graphein.protein.html#module-graphein.protein.meshes) | | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
 protein_mesh_tutorial.ipynb) | | ```python from graphein.protein.config import
 ProteinMeshConfig from graphein.protein.meshes import create_mesh verts, faces,
@@ -189,58 +208,15 @@
 compose.yml`) locally. For GPU usage please ensure that you have [NVIDIA
 Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-
 toolkit/install-guide.html) installed. Ensure that you install the locally
 mounted volume after entering the container (`pip install -e .`). This will
 also setup the dev environment locally. To build (GPU) run: ``` docker-compose
 up -d --build # start the container docker-compose down # stop the container
 ``` ## Citing Graphein Please consider citing graphein if it proves useful in
-your work. ```bibtex @article {Jamasb2020.07.15.204701, author = {Jamasb, Arian
-R. and Vi{\~n}as, Ramon and Ma, Eric J. and Harris, Charlie and Huang, Kexin
-and Hall, Dominic and Li{\'o}, Pietro and Blundell, Tom L.}, title = {Graphein
-- a Python Library for Geometric Deep Learning and Network Analysis on Protein
-Structures and Interaction Networks}, elocation-id = {2020.07.15.204701}, year
-= {2021}, doi = {10.1101/2020.07.15.204701}, publisher = {Cold Spring Harbor
-Laboratory}, abstract = {Geometric deep learning has well-motivated
-applications in the context of biology, a domain where relational structure in
-datasets can be meaningfully leveraged. Currently, efforts in both geometric
-deep learning and, more broadly, deep learning applied to biomolecular tasks
-have been hampered by a scarcity of appropriate datasets accessible to domain
-specialists and machine learning researchers alike. However, there has been
-little exploration of how to best to integrate and construct geometric
-representations of these datatypes. To address this, we introduce Graphein as a
-turn-key tool for transforming raw data from widely-used bioinformatics
-databases into machine learning-ready datasets in a high-throughput and
-flexible manner. Graphein is a Python library for constructing graph and
-surface-mesh representations of protein structures and biological interaction
-networks for computational analysis. Graphein provides utilities for data
-retrieval from widely-used bioinformatics databases for structural data,
-including the Protein Data Bank, the recently-released AlphaFold Structure
-Database, and for biomolecular interaction networks from STRINGdb, BioGrid,
-TRRUST and RegNetwork. The library interfaces with popular geometric deep
-learning libraries: DGL, PyTorch Geometric and PyTorch3D though remains
-framework agnostic as it is built on top of the PyData ecosystem to enable
-inter-operability with scientific computing tools and libraries. Graphein is
-designed to be highly flexible, allowing the user to specify each step of the
-data preparation, scalable to facilitate working with large protein complexes
-and interaction graphs, and contains useful pre-processing tools for preparing
-experimental files. Graphein facilitates network-based, graph-theoretic and
-topological analyses of structural and interaction datasets in a high-
-throughput manner. As example workflows, we make available two new protein
-structure-related datasets, previously unused by the geometric deep learning
-community. We envision that Graphein will facilitate developments in
-computational biology, graph representation learning and drug
-discovery.Availability and implementation Graphein is written in Python. Source
-code, example usage and tutorials, datasets, and documentation are made freely
-available under the MIT License at the following URL: graphein.aiCompeting
-Interest StatementThe authors have declared no competing interest.}, URL =
-{https://www.biorxiv.org/content/early/2021/10/12/2020.07.15.204701}, eprint =
-{https://www.biorxiv.org/content/early/2021/10/12/2020.07.15.204701.full.pdf},
-journal = {bioRxiv} } ``` Platform: any Classifier: License :: OSI Approved ::
-MIT License Classifier: Development Status :: 5 - Production/Stable Classifier:
-Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-dev Provides-Extra: extras Provides-Extra: all
+your work. ```bibtex @inproceedings{jamasb2022graphein, title={Graphein - a
+Python Library for Geometric Deep Learning and Network Analysis on Biomolecular
+Structures and Interaction Networks}, author={Arian Rokkum Jamasb and Ramon Vi
+{\~n}as Torn{\'e} and Eric J Ma and Yuanqi Du and Charles Harris and Kexin
+Huang and Dominic Hall and Pietro Lio and Tom Leon Blundell}, booktitle=
+{Advances in Neural Information Processing Systems}, editor={Alice H. Oh and
+Alekh Agarwal and Danielle Belgrave and Kyunghyun Cho}, year={2022}, url=
+{https://openreview.net/forum?id=9xRZlV6GfOX} } ```
```

### Comparing `graphein-1.6.0/README.md` & `graphein-1.7.0/graphein.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: graphein
+Version: 1.7.0
+Summary: Protein & Interactomic Graph Construction for Machine Learning
+Home-page: https://github.com/a-r-j/graphein
+Author: Arian Jamasb
+Author-email: arian@jamasb.io
+License: MIT
+Project-URL: homepage, https://github.com/a-r-j/graphein
+Project-URL: changelog, https://github.com/a-r-j/graphein/blob/master/CHANGELOG.md
+Project-URL: issue, https://github.com/a-r-j/graphein/issues
+Project-URL: documentation, https://graphein.ai/
+Platform: any
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: extras
+Provides-Extra: all
+License-File: LICENSE
+
+
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/a-r-j/graphein-binder/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fa-r-j%252Fgraphein%26urlpath%3Dlab%252Ftree%252Fgraphein%252Fnotebooks%26branch%3Dmaster)
 [![PyPI version](https://badge.fury.io/py/graphein.svg)](https://badge.fury.io/py/graphein)
 ![supported python versions](https://img.shields.io/pypi/pyversions/graphein)
 [![Docs](https://assets.readthedocs.org/static/projects/badges/passing-flat.svg)](http://www.graphein.ai)
 [![DOI:10.1101/2020.07.15.204701](https://zenodo.org/badge/DOI/10.1101/2020.07.15.204701.svg)](https://doi.org/10.1101/2020.07.15.204701)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![CodeFactor](https://www.codefactor.io/repository/github/a-r-j/graphein/badge)](https://www.codefactor.io/repository/github/a-r-j/graphein)
@@ -28,27 +61,29 @@
 
 Protein & Interactomic Graph Library
 
 This package provides functionality for producing geometric representations of protein and RNA structures, and biological interaction networks. We provide compatibility with standard PyData formats, as well as graph objects designed for ease of use with popular deep learning libraries.
 
 ## What's New?
 
-|   |   |
-|---|---|
-| [Protein Tensor Module](http://graphein.ai/notebooks/protein_tensors.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_tensors.ipynb)   |
-| [Constructing molecular graphs](http://graphein.ai/notebooks/molecule_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/molecule_tutorial.ipynb)   |
-| [Ready-to-go Dataloaders for PyTorch Geometric](http://graphein.ai/notebooks/dataloader_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/dataloader_tutorial.ipynb)   |
-| [Extracting subgraphs from protein graphs](http://graphein.ai/notebooks/subgraphing_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/subgraphing_tutorial.ipynb)   |
-| [Protein Graph Analytics](http://graphein.ai/notebooks/protein_graph_analytics.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_graph_analytics.ipynb) |
-| [Graphein CLI](http://graphein.ai/getting_started/usage.html)  |   |
-| [Protein Graph Creation from AlphaFold2!](http://graphein.ai/notebooks/alphafold_protein_graph_tutorial.html)  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) |
-| [Protein Graph Visualisation!](http://graphein.ai/notebooks/interactive_plotly_example.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/interactive_plotly_example.ipynb)
-| [RNA Graph Construction from Dotbracket notation](http://graphein.ai/modules/graphein.rna.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/rna_graph_tutorial.ipynb) |
-| [Protein - Protein Interaction Network Support & Structural Interactomics (Using AlphaFold2!)](http://graphein.ai/notebooks/ppi_tutorial.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/ppi_graph.ipynb) |
-| [High and Low-level API for massive flexibility - create your own bespoke workflows!](http://graphein.ai/notebooks/residue_graphs.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) |
+|   |   |   |
+|---|---|---|
+| 1.7.0 | [FoldComp Datasets](http://graphein.ai/notebooks/foldcomp.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/foldcomp.ipynb)   |
+| 1.7.0 | [Creating Datasets from the PDB](http://graphein.ai/notebooks/creating_datasets_from_the_pdb.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/creating_datasets_from_the_pdb.ipynb)   |
+| 1.6.0 | [Protein Tensor Module](http://graphein.ai/notebooks/protein_tensors.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_tensors.ipynb)   |
+| 1.5.0 | [Protein Graph Creation from AlphaFold2!](http://graphein.ai/notebooks/alphafold_protein_graph_tutorial.html)  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) |
+| 1.5.0 | [RNA Graph Construction from Dotbracket notation](http://graphein.ai/modules/graphein.rna.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/rna_graph_tutorial.ipynb) |
+| 1.4.0 | [Constructing molecular graphs](http://graphein.ai/notebooks/molecule_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/molecule_tutorial.ipynb)   |
+| 1.3.0 | [Ready-to-go Dataloaders for PyTorch Geometric](http://graphein.ai/notebooks/dataloader_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/dataloader_tutorial.ipynb)   |
+| 1.2.0 | [Extracting subgraphs from protein graphs](http://graphein.ai/notebooks/subgraphing_tutorial.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/subgraphing_tutorial.ipynb)   |
+| 1.2.0 | [Protein Graph Analytics](http://graphein.ai/notebooks/protein_graph_analytics.html)  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/protein_graph_analytics.ipynb) |
+| 1.2.0 | [Graphein CLI](http://graphein.ai/getting_started/usage.html)  |   |
+| 1.2.0 |[Protein Graph Visualisation!](http://graphein.ai/notebooks/interactive_plotly_example.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/interactive_plotly_example.ipynb)
+| 1.1.0 | [Protein - Protein Interaction Network Support & Structural Interactomics (Using AlphaFold2!)](http://graphein.ai/notebooks/ppi_tutorial.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/ppi_graph.ipynb) |
+| 1.0.0 | [High and Low-level API for massive flexibility - create your own bespoke workflows!](http://graphein.ai/notebooks/residue_graphs.html) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/residue_graphs.ipynb) |
 
 ## Example usage
 
 Graphein provides both a programmatic API and a command-line interface for constructing graphs.
 
 ### CLI
 
@@ -85,15 +120,15 @@
 ```python
 from graphein.protein.config import ProteinGraphConfig
 from graphein.protein.graphs import construct_graph
 from graphein.protein.utils import download_alphafold_structure
 
 config = ProteinGraphConfig()
 fp = download_alphafold_structure("Q5VSL9", aligned_score=False)
-g = construct_graph(config=config, pdb_path=fp)
+g = construct_graph(config=config, path=fp)
 ```
 
 ### Creating a Protein Mesh
 
 |   |   |
 |---|---|
 | [Tutorial](http://graphein.ai/notebooks/protein_mesh_tutorial.html) | [Docs](http://graphein.ai/modules/graphein.protein.html#module-graphein.protein.meshes) |
@@ -249,21 +284,17 @@
 ```
 
 ## Citing Graphein
 
 Please consider citing graphein if it proves useful in your work.
 
 ```bibtex
-@article {Jamasb2020.07.15.204701,
- author = {Jamasb, Arian R. and Vi{\~n}as, Ramon and Ma, Eric J. and Harris, Charlie and Huang, Kexin and Hall, Dominic and Li{\'o}, Pietro and Blundell, Tom L.},
- title = {Graphein - a Python Library for Geometric Deep Learning and Network Analysis on Protein Structures and Interaction Networks},
- elocation-id = {2020.07.15.204701},
- year = {2021},
- doi = {10.1101/2020.07.15.204701},
- publisher = {Cold Spring Harbor Laboratory},
- abstract = {Geometric deep learning has well-motivated applications in the context of biology, a domain where relational structure in datasets can be meaningfully leveraged. Currently, efforts in both geometric deep learning and, more broadly, deep learning applied to biomolecular tasks have been hampered by a scarcity of appropriate datasets accessible to domain specialists and machine learning researchers alike. However, there has been little exploration of how to best to integrate and construct geometric representations of these datatypes. To address this, we introduce Graphein as a turn-key tool for transforming raw data from widely-used bioinformatics databases into machine learning-ready datasets in a high-throughput and flexible manner. Graphein is a Python library for constructing graph and surface-mesh representations of protein structures and biological interaction networks for computational analysis. Graphein provides utilities for data retrieval from widely-used bioinformatics databases for structural data, including the Protein Data Bank, the recently-released AlphaFold Structure Database, and for biomolecular interaction networks from STRINGdb, BioGrid, TRRUST and RegNetwork. The library interfaces with popular geometric deep learning libraries: DGL, PyTorch Geometric and PyTorch3D though remains framework agnostic as it is built on top of the PyData ecosystem to enable inter-operability with scientific computing tools and libraries. Graphein is designed to be highly flexible, allowing the user to specify each step of the data preparation, scalable to facilitate working with large protein complexes and interaction graphs, and contains useful pre-processing tools for preparing experimental files. Graphein facilitates network-based, graph-theoretic and topological analyses of structural and interaction datasets in a high-throughput manner. As example workflows, we make available two new protein structure-related datasets, previously unused by the geometric deep learning community. We envision that Graphein will facilitate developments in computational biology, graph representation learning and drug discovery.Availability and implementation Graphein is written in Python. Source code, example usage and tutorials, datasets, and documentation are made freely available under the MIT License at the following URL: graphein.aiCompeting Interest StatementThe authors have declared no competing interest.},
- URL = {https://www.biorxiv.org/content/early/2021/10/12/2020.07.15.204701},
- eprint = {https://www.biorxiv.org/content/early/2021/10/12/2020.07.15.204701.full.pdf},
- journal = {bioRxiv}
+@inproceedings{jamasb2022graphein,
+  title={Graphein - a Python Library for Geometric Deep Learning and Network Analysis on Biomolecular Structures and Interaction Networks},
+  author={Arian Rokkum Jamasb and Ramon Vi{\~n}as Torn{\'e} and Eric J Ma and Yuanqi Du and Charles Harris and Kexin Huang and Dominic Hall and Pietro Lio and Tom Leon Blundell},
+  booktitle={Advances in Neural Information Processing Systems},
+  editor={Alice H. Oh and Alekh Agarwal and Danielle Belgrave and Kyunghyun Cho},
+  year={2022},
+  url={https://openreview.net/forum?id=9xRZlV6GfOX}
 }
 
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,25 @@
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/a-
-r-j/graphein-binder/master?urlpath=git-
+Metadata-Version: 2.1 Name: graphein Version: 1.7.0 Summary: Protein &
+Interactomic Graph Construction for Machine Learning Home-page: https://
+github.com/a-r-j/graphein Author: Arian Jamasb Author-email: arian@jamasb.io
+License: MIT Project-URL: homepage, https://github.com/a-r-j/graphein Project-
+URL: changelog, https://github.com/a-r-j/graphein/blob/master/CHANGELOG.md
+Project-URL: issue, https://github.com/a-r-j/graphein/issues Project-URL:
+documentation, https://graphein.ai/ Platform: any Classifier: License :: OSI
+Approved :: MIT License Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
+System :: POSIX Classifier: Operating System :: Unix Classifier: Operating
+System :: MacOS Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: extras Provides-Extra: all License-File:
+LICENSE [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/
+v2/gh/a-r-j/graphein-binder/master?urlpath=git-
 pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fa-r-
 j%252Fgraphein%26urlpath%3Dlab%252Ftree%252Fgraphein%252Fnotebooks%26branch%3Dmaster)
 [![PyPI version](https://badge.fury.io/py/graphein.svg)](https://badge.fury.io/
 py/graphein) ![supported python versions](https://img.shields.io/pypi/
 pyversions/graphein) [![Docs](https://assets.readthedocs.org/static/projects/
 badges/passing-flat.svg)](http://www.graphein.ai) [![DOI:10.1101/
 2020.07.15.204701](https://zenodo.org/badge/DOI/10.1101/2020.07.15.204701.svg)]
@@ -33,84 +49,93 @@
 [Documentation](http://www.graphein.ai) | [Paper](https://www.biorxiv.org/
 content/10.1101/2020.07.15.204701v1) | [Tutorials](http://graphein.ai/
 notebooks_index.html) | [Installation](#installation) Protein & Interactomic
 Graph Library This package provides functionality for producing geometric
 representations of protein and RNA structures, and biological interaction
 networks. We provide compatibility with standard PyData formats, as well as
 graph objects designed for ease of use with popular deep learning libraries. ##
-What's New? | | | |---|---| | [Protein Tensor Module](http://graphein.ai/
-notebooks/protein_tensors.html) | [![Open In Colab](https://
+What's New? | | | | |---|---|---| | 1.7.0 | [FoldComp Datasets](http://
+graphein.ai/notebooks/foldcomp.html) | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-protein_tensors.ipynb) | | [Constructing molecular graphs](http://graphein.ai/
-notebooks/molecule_tutorial.html) | [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-molecule_tutorial.ipynb) | | [Ready-to-go Dataloaders for PyTorch Geometric]
-(http://graphein.ai/notebooks/dataloader_tutorial.html) | [![Open In Colab]
+foldcomp.ipynb) | | 1.7.0 | [Creating Datasets from the PDB](http://
+graphein.ai/notebooks/creating_datasets_from_the_pdb.html) | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-dataloader_tutorial.ipynb) | | [Extracting subgraphs from protein graphs](http:
-//graphein.ai/notebooks/subgraphing_tutorial.html) | [![Open In Colab](https://
+creating_datasets_from_the_pdb.ipynb) | | 1.6.0 | [Protein Tensor Module](http:
+//graphein.ai/notebooks/protein_tensors.html) | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-subgraphing_tutorial.ipynb) | | [Protein Graph Analytics](http://graphein.ai/
-notebooks/protein_graph_analytics.html) | [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-protein_graph_analytics.ipynb) | | [Graphein CLI](http://graphein.ai/
-getting_started/usage.html) | | | [Protein Graph Creation from AlphaFold2!]
+protein_tensors.ipynb) | | 1.5.0 | [Protein Graph Creation from AlphaFold2!]
 (http://graphein.ai/notebooks/alphafold_protein_graph_tutorial.html) | [![Open
 In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-residue_graphs.ipynb) | | [Protein Graph Visualisation!](http://graphein.ai/
-notebooks/interactive_plotly_example.html) | [![Open In Colab](https://
+residue_graphs.ipynb) | | 1.5.0 | [RNA Graph Construction from Dotbracket
+notation](http://graphein.ai/modules/graphein.rna.html) | [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+rna_graph_tutorial.ipynb) | | 1.4.0 | [Constructing molecular graphs](http://
+graphein.ai/notebooks/molecule_tutorial.html) | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-interactive_plotly_example.ipynb) | [RNA Graph Construction from Dotbracket
-notation](http://graphein.ai/modules/graphein.rna.html) | [![Open In Colab]
+molecule_tutorial.ipynb) | | 1.3.0 | [Ready-to-go Dataloaders for PyTorch
+Geometric](http://graphein.ai/notebooks/dataloader_tutorial.html) | [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+dataloader_tutorial.ipynb) | | 1.2.0 | [Extracting subgraphs from protein
+graphs](http://graphein.ai/notebooks/subgraphing_tutorial.html) | [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+subgraphing_tutorial.ipynb) | | 1.2.0 | [Protein Graph Analytics](http://
+graphein.ai/notebooks/protein_graph_analytics.html) | [![Open In Colab](https:/
+/colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+protein_graph_analytics.ipynb) | | 1.2.0 | [Graphein CLI](http://graphein.ai/
+getting_started/usage.html) | | | 1.2.0 |[Protein Graph Visualisation!](http://
+graphein.ai/notebooks/interactive_plotly_example.html) | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-rna_graph_tutorial.ipynb) | | [Protein - Protein Interaction Network Support &
-Structural Interactomics (Using AlphaFold2!)](http://graphein.ai/notebooks/
-ppi_tutorial.html) | [![Open In Colab](https://colab.research.google.com/
+interactive_plotly_example.ipynb) | 1.1.0 | [Protein - Protein Interaction
+Network Support & Structural Interactomics (Using AlphaFold2!)](http://
+graphein.ai/notebooks/ppi_tutorial.html) | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
+ppi_graph.ipynb) | | 1.0.0 | [High and Low-level API for massive flexibility -
+create your own bespoke workflows!](http://graphein.ai/notebooks/
+residue_graphs.html) | [![Open In Colab](https://colab.research.google.com/
+assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/
+graphein/blob/master/notebooks/residue_graphs.ipynb) | ## Example usage
+Graphein provides both a programmatic API and a command-line interface for
+constructing graphs. ### CLI Graphein configs can be specified as `.yaml` files
+to batch process graphs from the commandline. [Docs](http://graphein.ai/
+getting_started/usage.html) ```bash graphein -c config.yaml -p path/to/pdbs -
+o path/to/output ``` ### Creating a Protein Graph | | | | |---|---|---|
+[Tutorial (Residue-level)](http://graphein.ai/notebooks/residue_graphs.html) |
+[Tutorial (Atomic)](http://graphein.ai/notebooks/atom_graph_tutorial.html) |
+[Docs](http://graphein.ai/modules/graphein.protein.html#module-
+graphein.protein.graphs) | [![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/github/a-r-j/
-graphein/blob/master/notebooks/ppi_graph.ipynb) | | [High and Low-level API for
-massive flexibility - create your own bespoke workflows!](http://graphein.ai/
-notebooks/residue_graphs.html) | [![Open In Colab](https://
+graphein/blob/master/notebooks/residue_graphs.ipynb) | [![Open In Colab(https:/
+/colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-residue_graphs.ipynb) | ## Example usage Graphein provides both a programmatic
-API and a command-line interface for constructing graphs. ### CLI Graphein
-configs can be specified as `.yaml` files to batch process graphs from the
-commandline. [Docs](http://graphein.ai/getting_started/usage.html) ```bash
-graphein -c config.yaml -p path/to/pdbs -o path/to/output ``` ### Creating a
-Protein Graph | | | | |---|---|---| [Tutorial (Residue-level)](http://
-graphein.ai/notebooks/residue_graphs.html) | [Tutorial (Atomic)](http://
-graphein.ai/notebooks/atom_graph_tutorial.html) | [Docs](http://graphein.ai/
-modules/graphein.protein.html#module-graphein.protein.graphs) | [![Open In
-Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+atom_graph_tutorial.ipynb) | | ```python from graphein.protein.config import
+ProteinGraphConfig from graphein.protein.graphs import construct_graph config =
+ProteinGraphConfig() g = construct_graph(config=config, pdb_code="3eiy") ```
+### Creating a Protein Graph from the AlphaFold Protein Structure Database | |
+| |---|---| | [Tutorial](http://graphein.ai/notebooks/
+alphafold_protein_graph_tutorial.html) | [Docs](http://graphein.ai/modules/
+graphein.protein.html#module-graphein.protein.graphs) | | [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
-residue_graphs.ipynb) | [![Open In Colab(https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/github/a-r-j/graphein/blob/
-master/notebooks/atom_graph_tutorial.ipynb) | | ```python from
-graphein.protein.config import ProteinGraphConfig from graphein.protein.graphs
-import construct_graph config = ProteinGraphConfig() g = construct_graph
-(config=config, pdb_code="3eiy") ``` ### Creating a Protein Graph from the
-AlphaFold Protein Structure Database | | | |---|---| | [Tutorial](http://
-graphein.ai/notebooks/alphafold_protein_graph_tutorial.html) | [Docs](http://
-graphein.ai/modules/graphein.protein.html#module-graphein.protein.graphs) | |
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
 residue_graphs.ipynb)| ```python from graphein.protein.config import
 ProteinGraphConfig from graphein.protein.graphs import construct_graph from
 graphein.protein.utils import download_alphafold_structure config =
 ProteinGraphConfig() fp = download_alphafold_structure("Q5VSL9",
-aligned_score=False) g = construct_graph(config=config, pdb_path=fp) ``` ###
+aligned_score=False) g = construct_graph(config=config, path=fp) ``` ###
 Creating a Protein Mesh | | | |---|---| | [Tutorial](http://graphein.ai/
 notebooks/protein_mesh_tutorial.html) | [Docs](http://graphein.ai/modules/
 graphein.protein.html#module-graphein.protein.meshes) | | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/a-r-j/graphein/blob/master/notebooks/
 protein_mesh_tutorial.ipynb) | | ```python from graphein.protein.config import
 ProteinMeshConfig from graphein.protein.meshes import create_mesh verts, faces,
@@ -183,49 +208,15 @@
 compose.yml`) locally. For GPU usage please ensure that you have [NVIDIA
 Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-
 toolkit/install-guide.html) installed. Ensure that you install the locally
 mounted volume after entering the container (`pip install -e .`). This will
 also setup the dev environment locally. To build (GPU) run: ``` docker-compose
 up -d --build # start the container docker-compose down # stop the container
 ``` ## Citing Graphein Please consider citing graphein if it proves useful in
-your work. ```bibtex @article {Jamasb2020.07.15.204701, author = {Jamasb, Arian
-R. and Vi{\~n}as, Ramon and Ma, Eric J. and Harris, Charlie and Huang, Kexin
-and Hall, Dominic and Li{\'o}, Pietro and Blundell, Tom L.}, title = {Graphein
-- a Python Library for Geometric Deep Learning and Network Analysis on Protein
-Structures and Interaction Networks}, elocation-id = {2020.07.15.204701}, year
-= {2021}, doi = {10.1101/2020.07.15.204701}, publisher = {Cold Spring Harbor
-Laboratory}, abstract = {Geometric deep learning has well-motivated
-applications in the context of biology, a domain where relational structure in
-datasets can be meaningfully leveraged. Currently, efforts in both geometric
-deep learning and, more broadly, deep learning applied to biomolecular tasks
-have been hampered by a scarcity of appropriate datasets accessible to domain
-specialists and machine learning researchers alike. However, there has been
-little exploration of how to best to integrate and construct geometric
-representations of these datatypes. To address this, we introduce Graphein as a
-turn-key tool for transforming raw data from widely-used bioinformatics
-databases into machine learning-ready datasets in a high-throughput and
-flexible manner. Graphein is a Python library for constructing graph and
-surface-mesh representations of protein structures and biological interaction
-networks for computational analysis. Graphein provides utilities for data
-retrieval from widely-used bioinformatics databases for structural data,
-including the Protein Data Bank, the recently-released AlphaFold Structure
-Database, and for biomolecular interaction networks from STRINGdb, BioGrid,
-TRRUST and RegNetwork. The library interfaces with popular geometric deep
-learning libraries: DGL, PyTorch Geometric and PyTorch3D though remains
-framework agnostic as it is built on top of the PyData ecosystem to enable
-inter-operability with scientific computing tools and libraries. Graphein is
-designed to be highly flexible, allowing the user to specify each step of the
-data preparation, scalable to facilitate working with large protein complexes
-and interaction graphs, and contains useful pre-processing tools for preparing
-experimental files. Graphein facilitates network-based, graph-theoretic and
-topological analyses of structural and interaction datasets in a high-
-throughput manner. As example workflows, we make available two new protein
-structure-related datasets, previously unused by the geometric deep learning
-community. We envision that Graphein will facilitate developments in
-computational biology, graph representation learning and drug
-discovery.Availability and implementation Graphein is written in Python. Source
-code, example usage and tutorials, datasets, and documentation are made freely
-available under the MIT License at the following URL: graphein.aiCompeting
-Interest StatementThe authors have declared no competing interest.}, URL =
-{https://www.biorxiv.org/content/early/2021/10/12/2020.07.15.204701}, eprint =
-{https://www.biorxiv.org/content/early/2021/10/12/2020.07.15.204701.full.pdf},
-journal = {bioRxiv} } ```
+your work. ```bibtex @inproceedings{jamasb2022graphein, title={Graphein - a
+Python Library for Geometric Deep Learning and Network Analysis on Biomolecular
+Structures and Interaction Networks}, author={Arian Rokkum Jamasb and Ramon Vi
+{\~n}as Torn{\'e} and Eric J Ma and Yuanqi Du and Charles Harris and Kexin
+Huang and Dominic Hall and Pietro Lio and Tom Leon Blundell}, booktitle=
+{Advances in Neural Information Processing Systems}, editor={Alice H. Oh and
+Alekh Agarwal and Danielle Belgrave and Kyunghyun Cho}, year={2022}, url=
+{https://openreview.net/forum?id=9xRZlV6GfOX} } ```
```

### Comparing `graphein-1.6.0/graphein/__init__.py` & `graphein-1.7.0/graphein/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from graphein.utils.utils import *
 
 # from .protein import *
 # from .rna import *
 from .testing import *
 
 __author__ = "Arian Jamasb <arian@jamasb.io>"
-__version__ = "1.6.0"
+__version__ = "1.7.0"
 
 
 logger.configure(
     handlers=[
         {"sink": RichHandler(rich_tracebacks=True), "format": "{message}"}
     ]
 )
```

### Comparing `graphein-1.6.0/graphein/grn/config.py` & `graphein-1.7.0/graphein/grn/config.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/grn/edges.py` & `graphein-1.7.0/graphein/grn/edges.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/grn/graphs.py` & `graphein-1.7.0/graphein/grn/graphs.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/grn/parse_regnetwork.py` & `graphein-1.7.0/graphein/grn/parse_regnetwork.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/grn/parse_trrust.py` & `graphein-1.7.0/graphein/grn/parse_trrust.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ml/clustering.py` & `graphein-1.7.0/graphein/ml/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,16 @@
 import os
 import random
 import sys
 from typing import Dict, List, Optional
 
 import networkx as nx
 import numpy as np
-import pandas as pd
 from Bio import SeqIO
 
-from graphein.protein.utils import is_tool
-
 
 def build_fasta_file_from_mapping(
     pdb_sequence_mapping: Dict[str, str],
     fasta_out: str,
 ):
     """
     Builds a fasta database from a mapping of PDBs (or other identifier) to sequences.
@@ -42,15 +39,15 @@
 
 def build_fasta_file_from_graphs(
     graphs: List[nx.Graph], fasta_out: str, chains: Optional[List[str]] = None
 ):
     if chains is None:
         chains = ["A"] * len(graphs)
     mapping = {
-        g.name + "_" + chain: g.graph[f"sequence_{chain}"]
+        f"{g.name}_{chain}": g.graph[f"sequence_{chain}"]
         for g, chain in zip(graphs, chains)
     }
 
     build_fasta_file_from_mapping(mapping, fasta_out)
 
 
 def get_seq_records(
@@ -100,17 +97,15 @@
                     with contextlib.suppress(ValueError):
                         good = _verify_alphabet(record.seq)
                     if not good:
                         sys.stderr.write(
                             f"WARNING in {get_seq_records.__name__} sequence {record.seq.id} from file "
                             f"{filename} is not compatible with declared alphabet {str(alphabet)}\n"
                         )
-    if return_as_dictionary:
-        return SeqIO.to_dict(records)
-    return records
+    return SeqIO.to_dict(records) if return_as_dictionary else records
 
 
 def create_pairs_for_clustering(
     fasta_file: str,
     seq_id_low_thresh: float = 25.0,
     use_very_loose_condition: bool = False,
     out_file: Optional[str] = None,
@@ -493,16 +488,16 @@
         c_sizes += [len(c)]
         num_ids += len(c)
     print(f"{num_ids} ids in {len(clusters)} clusters")
     random.seed(a=42)  # for reproducibility
     n = 0
     in_other_tests = []
     while n < number_of_sets:
-        train_set_name = train_set_key + f"_{n:02}"
-        test_set_name = test_set_key + f"_{n:02}"
+        train_set_name = f"{train_set_key}_{n:02}"
+        test_set_name = f"{test_set_key}_{n:02}"
         with open(train_set_name, mode="w") as train:
             with open(test_set_name, mode="w") as test:
                 ids_in_test = []
                 labs_in_test = []
                 test_rel_size = 0.0
                 seq_in_test = 0
                 while test_rel_size < fraction_in_test:
```

### Comparing `graphein-1.6.0/graphein/ml/conversion.py` & `graphein-1.7.0/graphein/ml/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import List, Optional
 
 import networkx as nx
 import numpy as np
 import torch
 from loguru import logger as log
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 try:
     import torch
 except ImportError:
     import_message(
         submodule="graphein.ml.conversion",
         package="torch",
```

### Comparing `graphein-1.6.0/graphein/ml/datasets/torch_geometric_dataset.py` & `graphein-1.7.0/graphein/ml/datasets/torch_geometric_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from graphein.protein.config import ProteinGraphConfig
 from graphein.protein.graphs import construct_graphs_mp
 from graphein.protein.utils import (
     download_alphafold_structure,
     download_pdb,
     download_pdb_multiprocessing,
 )
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 try:
     import torch
     from torch_geometric.data import Data, Dataset, InMemoryDataset
 except ImportError:
     import_message(
         "graphein.ml.datasets.torch_geometric_dataset",
@@ -37,15 +37,15 @@
 
 
 class InMemoryProteinGraphDataset(InMemoryDataset):
     def __init__(
         self,
         root: str,
         name: str,
-        pdb_paths: Optional[List[str]] = None,
+        paths: Optional[List[str]] = None,
         pdb_codes: Optional[List[str]] = None,
         uniprot_ids: Optional[List[str]] = None,
         graph_label_map: Optional[Dict[str, torch.Tensor]] = None,
         node_label_map: Optional[Dict[str, torch.Tensor]] = None,
         chain_selection_map: Optional[Dict[str, List[str]]] = None,
         graphein_config: ProteinGraphConfig = ProteinGraphConfig(),
         graph_format_convertor: GraphFormatConvertor = GraphFormatConvertor(
@@ -69,17 +69,17 @@
         create_dataset.html#creating-in-memory-datasets>`__ for the accompanying
         tutorial.
 
         :param root: Root directory where the dataset should be saved.
         :type root: str
         :param name: Name of the dataset. Will be saved to ``data_$name.pt``.
         :type name: str
-        :param pdb_paths: List of full path of pdb files to load. Defaults to
-            ``None``.
-        :type pdb_paths: Optional[List[str]], optional
+        :param paths: List of full path of PDB or MMTF files to load. Defaults
+            to ``None``.
+        :type paths: Optional[List[str]], optional
         :param pdb_codes: List of PDB codes to download and parse from the PDB.
             Defaults to None.
         :type pdb_codes: Optional[List[str]], optional
         :param uniprot_ids: List of Uniprot IDs to download and parse from
             Alphafold Database. Defaults to ``None``.
         :type uniprot_ids: Optional[List[str]], optional
         :param graph_label_map: Dictionary mapping PDB/Uniprot IDs to
@@ -135,31 +135,31 @@
         )
         self.uniprot_ids = (
             [up.upper() for up in uniprot_ids]
             if uniprot_ids is not None
             else None
         )
 
-        self.pdb_paths = pdb_paths
-        if self.pdb_paths is None:
+        self.paths = paths
+        if self.paths is None:
             if self.pdb_codes and self.uniprot_ids:
                 self.structures = self.pdb_codes + self.uniprot_ids
             elif self.pdb_codes:
                 self.structures = pdb_codes
             elif self.uniprot_ids:
                 self.structures = uniprot_ids
         # Use local saved pdb_files instead of download or move them to
         # self.root/raw dir
         else:
-            if isinstance(self.pdb_paths, list):
+            if isinstance(self.paths, list):
                 self.structures = [
-                    os.path.splitext(os.path.split(pdb_path)[-1])[0]
-                    for pdb_path in self.pdb_paths
+                    os.path.splitext(os.path.split(path)[-1])[0]
+                    for path in self.paths
                 ]
-                self.pdb_path, _ = os.path.split(self.pdb_paths[0])
+                self.path, _ = os.path.split(self.paths[0])
 
         if self.pdb_codes and self.uniprot_ids:
             self.structures = self.pdb_codes + self.uniprot_ids
         elif self.pdb_codes:
             self.structures = pdb_codes
         elif self.uniprot_ids:
             self.structures = uniprot_ids
@@ -197,16 +197,16 @@
     @property
     def processed_file_names(self) -> List[str]:
         """Name of the processed file."""
         return [f"data_{self.name}.pt"]
 
     @property
     def raw_dir(self) -> str:
-        if self.pdb_paths is not None:
-            return self.pdb_path  # replace raw dir with user local pdb_path
+        if self.paths is not None:
+            return self.path  # replace raw dir with user local path
         else:
             return os.path.join(self.root, "raw")
 
     def download(self):
         """Download the PDB files from RCSB or Alphafold."""
         self.config.pdb_dir = Path(self.raw_dir)
         if self.pdb_codes:
@@ -272,15 +272,15 @@
             ]
         else:
             chain_selections = None
 
         # Create graph objects
         print("Constructing Graphs...")
         graphs = construct_graphs_mp(
-            pdb_path_it=structure_files,
+            path_it=structure_files,
             config=self.config,
             chain_selections=chain_selections,
             return_dict=True,
             num_cores=self.num_cores,
         )
         # Transform graphs
         if self.graph_transformation_funcs is not None:
@@ -325,15 +325,15 @@
         print("Done!")
 
 
 class ProteinGraphDataset(Dataset):
     def __init__(
         self,
         root: str,
-        pdb_paths: Optional[List[str]] = None,
+        paths: Optional[List[str]] = None,
         pdb_codes: Optional[List[str]] = None,
         uniprot_ids: Optional[List[str]] = None,
         # graph_label_map: Optional[Dict[str, int]] = None,
         graph_labels: Optional[List[torch.Tensor]] = None,
         node_labels: Optional[List[torch.Tensor]] = None,
         chain_selections: Optional[List[str]] = None,
         # node_label_map: Optional[Dict[str, int]] = None,
@@ -354,17 +354,17 @@
 
         Dataset base class for creating graph datasets.
         See `here <https://pytorch-geometric.readthedocs.io/en/latest/notes/
         create_dataset.html>`__ for the accompanying tutorial.
 
         :param root: Root directory where the dataset should be saved.
         :type root: str
-        :param pdb_paths: List of full path of pdb files to load. Defaults to
-            ``None``.
-        :type pdb_paths: Optional[List[str]], optional
+        :param paths: List of full path of PDB or MMTF files to load. Defaults
+            to ``None``.
+        :type paths: Optional[List[str]], optional
         :param pdb_codes: List of PDB codes to download and parse from the PDB.
             Defaults to ``None``.
         :type pdb_codes: Optional[List[str]], optional
         :param uniprot_ids: List of Uniprot IDs to download and parse from
             Alphafold Database. Defaults to ``None``.
         :type uniprot_ids: Optional[List[str]], optional
         :param graph_label_map: Dictionary mapping PDB/Uniprot IDs to
@@ -418,31 +418,31 @@
             else None
         )
         self.uniprot_ids = (
             [up.upper() for up in uniprot_ids]
             if uniprot_ids is not None
             else None
         )
-        self.pdb_paths = pdb_paths
-        if self.pdb_paths is None:
+        self.paths = paths
+        if self.paths is None:
             if self.pdb_codes and self.uniprot_ids:
                 self.structures = self.pdb_codes + self.uniprot_ids
             elif self.pdb_codes:
                 self.structures = pdb_codes
             elif self.uniprot_ids:
                 self.structures = uniprot_ids
         # Use local saved pdb_files instead of download or move them to
         # self.root/raw dir
         else:
-            if isinstance(self.pdb_paths, list):
+            if isinstance(self.paths, list):
                 self.structures = [
-                    os.path.splitext(os.path.split(pdb_path)[-1])[0]
-                    for pdb_path in self.pdb_paths
+                    os.path.splitext(os.path.split(path)[-1])[0]
+                    for path in self.paths
                 ]
-                self.pdb_path, _ = os.path.split(self.pdb_paths[0])
+                self.path, _ = os.path.split(self.paths[0])
 
         # Labels & Chains
 
         self.examples: Dict[int, str] = dict(enumerate(self.structures))
 
         if graph_labels is not None:
             self.graph_label_map = dict(enumerate(graph_labels))
@@ -492,16 +492,16 @@
                 )
             ]
         else:
             return [f"{pdb}.pt" for pdb in self.structures]
 
     @property
     def raw_dir(self) -> str:
-        if self.pdb_paths is not None:
-            return self.pdb_path  # replace raw dir with user local pdb_path
+        if self.paths is not None:
+            return self.path  # replace raw dir with user local path
         else:
             return os.path.join(self.root, "raw")
 
     def validate_input(self):
         if self.graph_label_map is not None:
             assert len(self.structures) == len(
                 self.graph_label_map
@@ -603,15 +603,15 @@
             else:
                 chain_selections = ["all"] * len(chunk)
 
             # Create graph objects
             file_names = [f"{self.raw_dir}/{pdb}.pdb" for pdb in pdbs]
 
             graphs = construct_graphs_mp(
-                pdb_path_it=file_names,
+                path_it=file_names,
                 config=self.config,
                 chain_selections=chain_selections,
                 return_dict=False,
             )
             if self.graph_transformation_funcs is not None:
                 graphs = [self.transform_graphein_graphs(g) for g in graphs]
```

### Comparing `graphein-1.6.0/graphein/ml/diffusion.py` & `graphein-1.7.0/graphein/ml/diffusion.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ml/metrics/gdt.py` & `graphein-1.7.0/graphein/ml/metrics/gdt.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ml/metrics/tm_score.py` & `graphein-1.7.0/graphein/ml/metrics/tm_score.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Union
 
+import numpy as np
 import torch
+from torch_geometric.utils import unbatch
 from torchmetrics import Metric
 
 from ...protein.tensor.types import AtomTensor, CoordTensor
 
 
 def tm_score(
     y_hat: Union[CoordTensor, AtomTensor], y: Union[CoordTensor, AtomTensor]
@@ -63,16 +65,16 @@
 
     @property
     def higher_is_better(self):
         return True
 
     def update(
         self,
-        pred: Union[COORD_TENSOR, ATOM_TENSOR],
-        target: Union[COORD_TENSOR, ATOM_TENSOR],
+        pred: Union[CoordTensor, AtomTensor],
+        target: Union[CoordTensor, AtomTensor],
         batch: torch.Tensor,
     ):
         y = unbatch(target, batch)
         y_hat = unbatch(pred, batch)
 
         for i, j in zip(y, y_hat):
             self.correct += tm_score(i, j)
```

### Comparing `graphein-1.6.0/graphein/ml/utils.py` & `graphein-1.7.0/graphein/ml/utils.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ml/visualisation.py` & `graphein-1.7.0/graphein/ml/visualisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 from typing import Optional, Tuple
 
 import matplotlib.pyplot as plt
 import networkx as nx
 import plotly.graph_objects as go
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 from ..protein.visualisation import plotly_protein_structure_graph
 from .conversion import GraphFormatConvertor
 
 try:
     from torch_geometric.data import Data
 except ImportError:
     import_message(
         submodule="graphein.ml.conversion",
         package="torch_geometric",
         pip_install=True,
-        conda_channel="rusty1s",
+        conda_channel="pyg",
     )
 
 try:
     import torch
 except ImportError:
     import_message(
         submodule="graphein.ml.visualisation",
```

### Comparing `graphein-1.6.0/graphein/molecule/atoms.py` & `graphein-1.7.0/graphein/molecule/atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 # License: MIT
 # Project Website: https://github.com/a-r-j/graphein
 # Code Repository: https://github.com/a-r-j/graphein
 from __future__ import annotations
 
 from typing import Dict, List
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 try:
     import rdkit.Chem as Chem
 except ImportError:
-    import_message("graphein.molecule.atoms", "rdkit", "rdkit", True)
+    import_message(
+        "graphein.molecule.atoms", "rdkit", "rdkit", True, extras=True
+    )
 
 
 BASE_ATOMS: List[str] = [
     "C",
     "H",
     "O",
     "N",
```

### Comparing `graphein-1.6.0/graphein/molecule/chembl.py` & `graphein-1.7.0/graphein/molecule/chembl.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/molecule/config.py` & `graphein-1.7.0/graphein/molecule/config.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/molecule/edges/atomic.py` & `graphein-1.7.0/graphein/molecule/edges/atomic.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/molecule/edges/distance.py` & `graphein-1.7.0/graphein/molecule/edges/distance.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/molecule/features/edges/bonds.py` & `graphein-1.7.0/graphein/molecule/features/edges/bonds.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/molecule/features/graph/molecule.py` & `graphein-1.7.0/graphein/molecule/features/graph/molecule.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,26 @@
     get_max_ring_size,
     get_mol_weight,
     get_morgan_fp,
     get_morgan_fp_np,
     get_qed_score,
     get_shape_moments,
 )
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 try:
     from rdkit import Chem
     from rdkit.Chem import Descriptors
 except ImportError:
     import_message(
-        "graphe in.molecule.features.graph.molecule", "rdkit", "rdkit", True
+        "graphe in.molecule.features.graph.molecule",
+        "rdkit",
+        "rdkit",
+        True,
+        extras=True,
     )
 
 
 def mol_descriptors(
     g: nx.Graph,
     descriptor_list: Optional[List[str]] = None,
     return_array: bool = False,
```

### Comparing `graphein-1.6.0/graphein/molecule/features/nodes/atom_type.py` & `graphein-1.7.0/graphein/molecule/features/nodes/atom_type.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/molecule/graphs.py` & `graphein-1.7.0/graphein/molecule/graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 from typing import Callable, Dict, List, Optional, Union
 
 import networkx as nx
 import numpy as np
 from loguru import logger as log
 from tqdm.contrib.concurrent import process_map, thread_map
 
+from graphein.utils.dependencies import import_message
 from graphein.utils.utils import (
     annotate_edge_metadata,
     annotate_graph_metadata,
     annotate_node_metadata,
     compute_edges,
-    import_message,
 )
 
 from .chembl import get_smiles_from_chembl
 from .config import MoleculeGraphConfig
 from .edges.atomic import add_atom_bonds
 from .utils import compute_fragments
 from .zinc import get_smiles_from_zinc
```

### Comparing `graphein-1.6.0/graphein/molecule/utils.py` & `graphein-1.7.0/graphein/molecule/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import Any, List, Optional, Tuple, Union
 
 import networkx as nx
 import numpy as np
 from scipy.sparse import csr_matrix
 from scipy.sparse.csgraph import minimum_spanning_tree
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 try:
     import rdkit
     from rdkit import Chem as Chem
     from rdkit import DataStructs
     from rdkit.Chem import AllChem
     from rdkit.Chem.Descriptors import (
@@ -34,20 +34,24 @@
         MolWt,
         NumHAcceptors,
         NumHDonors,
     )
     from rdkit.Chem.Descriptors3D import NPR1, NPR2
     from rdkit.Chem.rdMolTransforms import ComputeCentroid
 except ImportError:
-    import_message("graphein.molecule.utils", "rdkit", "rdkit", True)
+    import_message(
+        "graphein.molecule.utils", "rdkit", "rdkit", True, extras=True
+    )
 
 try:
     import selfies as sf
 except ImportError:
-    import_message("graphein.molecule.utils", "selfies", None, True)
+    import_message(
+        "graphein.molecule.utils", "selfies", None, True, extras=True
+    )
 
 
 MST_MAX_WEIGHT: int = 100
 MAX_NCAND: int = 2000
 
 
 def get_center(
```

### Comparing `graphein-1.6.0/graphein/molecule/visualisation.py` & `graphein-1.7.0/graphein/molecule/visualisation.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/molecule/zinc.py` & `graphein-1.7.0/graphein/molecule/zinc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 
 import ssl
 from typing import Dict, List
 from urllib.error import URLError
 
 from tqdm.rich import tqdm
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 try:
     from smilite import *
 except ImportError:
-    import_message("graphein.molecule.zinc", "smilite", "smilite", True)
+    import_message(
+        "graphein.molecule.zinc", "smilite", "smilite", True, extras=True
+    )
 
 
 def get_smiles_from_zinc(zinc_id: str, backend="zinc15") -> str:
     """
     Gets the corresponding SMILE string for a ZINC ID query from
     the ZINC online database (https://zinc.docking.org/). Requires an internet connection.
```

### Comparing `graphein-1.6.0/graphein/ppi/config.py` & `graphein-1.7.0/graphein/ppi/config.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ppi/edges.py` & `graphein-1.7.0/graphein/ppi/edges.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ppi/features/node_features.py` & `graphein-1.7.0/graphein/ppi/features/node_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,17 @@
 # Author: Ramon Vinas, Arian Jamasb <arian@jamasb.io>
 # License: MIT
 # Project Website: https://github.com/a-r-j/graphein
 # Code Repository: https://github.com/a-r-j/graphein
 from typing import Any, Dict
 
 import networkx as nx
+from bioservices import HGNC, UniProt
 from loguru import logger as log
 
-from graphein.utils.utils import import_message
-
-try:
-    from bioservices import HGNC, UniProt
-except ImportError:
-    message = import_message(
-        submodule="graphein.ppi.features.nodes_features",
-        package="bioservices",
-        conda_channel="bioconda",
-        pip_install=True,
-    )
-    log.warning(message)
-
 
 def add_sequence_to_nodes(n: str, d: Dict[str, Any]):
     """
     Maps UniProt ACC to UniProt ID. Retrieves sequence from UniProt and adds it to the node as a feature
 
     :param n: Graph node.
     :type n: str
```

### Comparing `graphein-1.6.0/graphein/ppi/graph_metadata.py` & `graphein-1.7.0/graphein/ppi/graph_metadata.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ppi/graphs.py` & `graphein-1.7.0/graphein/ppi/graphs.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ppi/parse_biogrid.py` & `graphein-1.7.0/graphein/ppi/parse_biogrid.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ppi/parse_stringdb.py` & `graphein-1.7.0/graphein/ppi/parse_stringdb.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/ppi/visualisation.py` & `graphein-1.7.0/graphein/ppi/visualisation.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/__init__.py` & `graphein-1.7.0/graphein/protein/__init__.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/analysis.py` & `graphein-1.7.0/graphein/protein/analysis.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/config.py` & `graphein-1.7.0/graphein/protein/config.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/edges/atomic.py` & `graphein-1.7.0/graphein/protein/edges/atomic.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/edges/distance.py` & `graphein-1.7.0/graphein/protein/edges/distance.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/edges/intramolecular.py` & `graphein-1.7.0/graphein/protein/edges/intramolecular.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/features/graph/dynamics.py` & `graphein-1.7.0/graphein/protein/features/graph/dynamics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import networkx as nx
 import numpy as np
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 try:
     import prody
 except ImportError:
     message = import_message(
         "graphein.protein.features.graph.dynamics", "prody", "prody", True
     )
```

### Comparing `graphein-1.6.0/graphein/protein/features/graph/structure.py` & `graphein-1.7.0/graphein/protein/features/graph/structure.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/features/nodes/aaindex.py` & `graphein-1.7.0/graphein/protein/features/nodes/aaindex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Functions for adding node features from AAIndex."""
 from typing import Dict, Tuple
 
 import networkx as nx
 from loguru import logger as log
 
-from graphein.utils.utils import import_message, protein_letters_3to1_all_caps
+from graphein.utils.dependencies import import_message
+from graphein.utils.utils import protein_letters_3to1_all_caps
 
 try:
     from pyaaisc import Aaindex
 except ImportError:
     message = import_message(
         submodule="graphein.protein.features.nodes.aaindex",
         package="pyaaisc",
         pip_install=True,
+        extras=True,
     )
     log.warning(message)
 
 
 def fetch_AAIndex(accession: str) -> Tuple[str, Dict[str, float]]:
     """
     Fetches AAindex1 dictionary from an accession code. The dictionary maps one-letter AA codes to float values
```

### Comparing `graphein-1.6.0/graphein/protein/features/nodes/amino_acid.py` & `graphein-1.7.0/graphein/protein/features/nodes/amino_acid.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/features/nodes/amino_acid_properties.csv` & `graphein-1.7.0/graphein/protein/features/nodes/amino_acid_properties.csv`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/features/nodes/dssp.py` & `graphein-1.7.0/graphein/protein/features/nodes/dssp.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from typing import Any, Dict, Optional
 
 import networkx as nx
 import pandas as pd
 from Bio.PDB.DSSP import dssp_dict_from_pdb_file, residue_max_acc
 
 from graphein.protein.resi_atoms import STANDARD_AMINO_ACID_MAPPING_1_TO_3
-from graphein.protein.utils import is_tool, save_pdb_df_to_pdb
+from graphein.protein.utils import save_pdb_df_to_pdb
+from graphein.utils.dependencies import is_tool
 
 DSSP_COLS = [
     "chain",
     "resnum",
     "icode",
     "aa",
     "ss",
@@ -80,29 +81,29 @@
     :type dssp_config: DSSPConfig, optional
     :return: Protein graph with DSSP dataframe added
     :rtype: nx.Graph
     """
 
     config = G.graph["config"]
     pdb_code = G.graph["pdb_code"]
-    pdb_path = G.graph["pdb_path"]
+    path = G.graph["path"]
     pdb_name = G.graph["name"]
 
     # Extract DSSP executable
     executable = dssp_config.executable
 
     # Ensure that DSSP is on PATH and is marked as an executable.
     assert is_tool(
         executable
     ), "DSSP must be on PATH and marked as an executable"
 
     pdb_file = None
-    if pdb_path:
-        if os.path.isfile(pdb_path):
-            pdb_file = pdb_path
+    if path:
+        if os.path.isfile(path):
+            pdb_file = path
     else:
         if config.pdb_dir:
             if os.path.isfile(config.pdb_dir / (pdb_code + ".pdb")):
                 pdb_file = config.pdb_dir / (pdb_code + ".pdb")
 
     # Check for existence of pdb file. If not, reconstructs it from the raw df.
     if pdb_file:
```

### Comparing `graphein-1.6.0/graphein/protein/features/nodes/geometry.py` & `graphein-1.7.0/graphein/protein/features/nodes/geometry.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/features/nodes/meiler_embeddings.csv` & `graphein-1.7.0/graphein/protein/features/nodes/meiler_embeddings.csv`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/features/sequence/embeddings.py` & `graphein-1.7.0/graphein/protein/features/sequence/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import numpy as np
 from loguru import logger as log
 
 from graphein.protein.features.sequence.utils import (
     compute_feature_over_chains,
     subset_by_node_feature_value,
 )
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 try:
     import torch
 except ImportError:
     message = import_message(
         submodule="graphein.protein.features.sequence.embeddings",
         package="torch",
@@ -35,14 +35,15 @@
 try:
     import biovec
 except ImportError:
     message = import_message(
         submodule="graphein.protein.features.sequence.embeddings",
         package="biovec",
         pip_install=True,
+        extras=True,
     )
     log.warning(message)
 
 
 @lru_cache()
 def _load_esm_model(model_name: str = "esm1b_t33_650M_UR50S"):
     """
```

### Comparing `graphein-1.6.0/graphein/protein/features/sequence/propy.py` & `graphein-1.7.0/graphein/protein/features/sequence/propy.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/features/sequence/sequence.py` & `graphein-1.7.0/graphein/protein/features/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/features/sequence/utils.py` & `graphein-1.7.0/graphein/protein/features/sequence/utils.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/features/utils.py` & `graphein-1.7.0/graphein/protein/features/utils.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/graphs.py` & `graphein-1.7.0/graphein/protein/graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 # Graphein
 # Author: Arian Jamasb <arian@jamasb.io>, Eric Ma, Charlie Harris
 # License: MIT
 # Project Website: https://github.com/a-r-j/graphein
 # Code Repository: https://github.com/a-r-j/graphein
 from __future__ import annotations
 
+import os
 import traceback
 from contextlib import nullcontext
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 from Bio.PDB.Polypeptide import three_to_one
+from biopandas.mmtf import PandasMmtf
 from biopandas.pdb import PandasPdb
 from loguru import logger as log
 from rich.progress import Progress
 from tqdm.contrib.concurrent import process_map
 from typing_extensions import Literal
 
 from graphein.protein.config import (
@@ -64,51 +66,56 @@
     """
     return filter_dataframe(
         df, by_column="atom_name", list_of_values=RNA_ATOMS, boolean=True
     )
 
 
 def read_pdb_to_dataframe(
-    pdb_path: Optional[os.Pathlike] = None,
+    path: Optional[Union[str, os.PathLike]] = None,
     pdb_code: Optional[str] = None,
     uniprot_id: Optional[str] = None,
     model_index: int = 1,
 ) -> pd.DataFrame:
     """
     Reads PDB file to ``PandasPDB`` object.
 
     Returns ``atomic_df``, which is a DataFrame enumerating all atoms and
     their cartesian coordinates in 3D space. Also contains associated metadata
     from the PDB file.
 
-    :param pdb_path: path to PDB file. Defaults to ``None``.
-    :type pdb_path: str, optional
+    :param path: path to PDB or MMTF file. Defaults to ``None``.
+    :type path: str, optional
     :param pdb_code: 4-character PDB accession. Defaults to ``None``.
     :type pdb_code: str, optional
     :param uniprot_id: UniProt ID to build graph from AlphaFoldDB. Defaults to
         ``None``.
     :type uniprot_id: str, optional
     :param model_index: Index of model to read. Only relevant for structures
         containing ensembles. Defaults to ``1``.
     :type model_index: int, optional
     :returns: ``pd.DataFrame`` containing protein structure
     :rtype: pd.DataFrame
     """
-    if pdb_code is None and pdb_path is None and uniprot_id is None:
+    if pdb_code is None and path is None and uniprot_id is None:
         raise NameError(
-            "One of pdb_code, pdb_path or uniprot_id must be specified!"
+            "One of pdb_code, path or uniprot_id must be specified!"
         )
 
-    if pdb_path is not None:
-        if isinstance(pdb_path, Path):
-            pdb_path = os.fsdecode(pdb_path)
-        atomic_df = PandasPdb().read_pdb(pdb_path)
+    if path is not None:
+        if isinstance(path, Path):
+            path = os.fsdecode(path)
+        if path.endswith(".pdb"):
+            atomic_df = PandasPdb().read_pdb(path)
+        elif path.endswith(".mmtf"):
+            atomic_df = PandasMmtf().read_mmtf(path)
+        else:
+            raise ValueError("File must be either .pdb or .mmtf")
     elif uniprot_id is not None:
         atomic_df = PandasPdb().fetch_pdb(
-            uniprot_id=uniprot_id, source="alphafold2-v2"
+            uniprot_id=uniprot_id, source="alphafold2-v3"
         )
     else:
         atomic_df = PandasPdb().fetch_pdb(pdb_code)
 
     atomic_df = atomic_df.get_model(model_index)
     if len(atomic_df.df["ATOM"]) == 0:
         raise ValueError(f"No model found for index: {model_index}")
@@ -482,15 +489,15 @@
 
 def initialise_graph_with_metadata(
     protein_df: pd.DataFrame,
     raw_pdb_df: pd.DataFrame,
     granularity: str,
     name: Optional[str] = None,
     pdb_code: Optional[str] = None,
-    pdb_path: Optional[str] = None,
+    path: Optional[str] = None,
 ) -> nx.Graph:
     """
     Initializes the nx Graph object with initial metadata.
 
     :param protein_df: Processed DataFrame of protein structure.
     :type protein_df: pd.DataFrame
     :param raw_pdb_df: Unprocessed dataframe of protein structure for comparison
@@ -503,34 +510,34 @@
     :type granularity: str
     :param name: specified given name for the graph. If None, the PDB code or
         the file name will be used to name the graph.
     :type name: Optional[str], defaults to ``None``
     :param pdb_code: PDB ID / Accession code, if the PDB is available on the
         PDB database.
     :type pdb_code: Optional[str], defaults to ``None``.
-    :param pdb_path: path to local PDB file, if constructing a graph from a
+    :param path: path to local PDB or MMTF file, if constructing a graph from a
         local file.
-    :type pdb_path: Optional[str], defaults to ``None``.
+    :type path: Optional[str], defaults to ``None``.
     :return: Returns initial protein structure graph with metadata.
     :rtype: nx.Graph
     """
-    if pdb_path is not None and isinstance(pdb_path, Path):
-        pdb_path = os.fsdecode(pdb_path)
+    if path is not None and isinstance(path, Path):
+        path = os.fsdecode(path)
 
     # Get name for graph if no name was provided
     if name is None:
-        if pdb_path is not None:
-            name = get_protein_name_from_filename(pdb_path)
+        if path is not None:
+            name = get_protein_name_from_filename(path)
         else:
             name = pdb_code
 
     G = nx.Graph(
         name=name,
         pdb_code=pdb_code,
-        pdb_path=pdb_path,
+        path=path,
         chain_ids=list(protein_df["chain_id"].unique()),
         pdb_df=protein_df,
         raw_pdb_df=raw_pdb_df,
         rgroup_df=compute_rgroup_dataframe(remove_insertions(raw_pdb_df)),
         coords=np.asarray(protein_df[["x_coord", "y_coord", "z_coord"]]),
     )
 
@@ -675,46 +682,46 @@
 
     return add_distance_to_edges(G)
 
 
 def construct_graph(
     config: Optional[ProteinGraphConfig] = None,
     name: Optional[str] = None,
-    pdb_path: Optional[os.Pathlike] = None,
+    path: Optional[Union[str, os.PathLike]] = None,
     uniprot_id: Optional[str] = None,
     pdb_code: Optional[str] = None,
     df: Optional[pd.DataFrame] = None,
     chain_selection: str = "all",
     model_index: int = 1,
     df_processing_funcs: Optional[List[Callable]] = None,
     edge_construction_funcs: Optional[List[Callable]] = None,
     edge_annotation_funcs: Optional[List[Callable]] = None,
     node_annotation_funcs: Optional[List[Callable]] = None,
     graph_annotation_funcs: Optional[List[Callable]] = None,
     verbose: bool = True,
 ) -> nx.Graph:
     """
-    Constructs protein structure graph from a ``pdb_code``, ``pdb_path``,
+    Constructs protein structure graph from a ``pdb_code``, ``path``,
     ``uniprot_id`` or a BioPandas DataFrame containing ``ATOM`` data.
 
     Users can provide a :class:`~graphein.protein.config.ProteinGraphConfig`
     object to specify construction parameters.
 
     However, config parameters can be overridden by passing arguments directly
     to the function.
 
     :param config: :class:`~graphein.protein.config.ProteinGraphConfig` object.
         If ``None``, defaults to config in ``graphein.protein.config``.
     :type config: graphein.protein.config.ProteinGraphConfig, optional
     :param name: an optional given name for the graph. the PDB ID or PDB file
         name will be used if not specified.
     :type name: str, optional
-    :param pdb_path: Path to ``pdb_file`` when constructing a graph from a
+    :param path: Path to PDB or MMTF file when constructing a graph from a
         local pdb file. Default is ``None``.
-    :type pdb_path: Optional[str], defaults to ``None``
+    :type path: Optional[str], defaults to ``None``
     :param pdb_code: A 4-character PDB ID / accession to be used to construct
         the graph, if available. Default is ``None``.
     :type pdb_code: Optional[str], defaults to ``None``
     :param uniprot_id: UniProt accession ID to build graph from AlphaFold2DB.
         Default is ``None``.
     :type uniprot_id: str, optional
     :param df: Pandas dataframe containing ATOM data to build graph from.
@@ -744,26 +751,21 @@
     :param verbose: Controls the verbosity.
         Default is ``True``.
     :type verbose: bool
     :return: Protein Structure Graph
     :rtype: nx.Graph
     """
 
-    if (
-        pdb_code is None
-        and pdb_path is None
-        and uniprot_id is None
-        and df is None
-    ):
+    if pdb_code is None and path is None and uniprot_id is None and df is None:
         raise ValueError(
             "Either a PDB ID, UniProt ID, a dataframe or a path to a local PDB file"
             " must be specified to construct a graph"
         )
-    if pdb_path is not None and isinstance(pdb_path, Path):
-        pdb_path = os.fsdecode(pdb_path)
+    if path is not None and isinstance(path, Path):
+        path = os.fsdecode(path)
 
     # If no config is provided, use default
     if config is None:
         config = ProteinGraphConfig()
 
     # Use progress tracking context if in verbose mode
     context = Progress(transient=True) if verbose else nullcontext()
@@ -796,15 +798,15 @@
         config.edge_metadata_functions = (
             edge_annotation_funcs
             if config.edge_metadata_functions is None
             else config.edge_metadata_functions
         )
         if df is None:
             raw_df = read_pdb_to_dataframe(
-                pdb_path,
+                path,
                 pdb_code,
                 uniprot_id,
                 model_index=model_index,
             )
         else:
             raw_df = df
 
@@ -828,15 +830,15 @@
             task3 = progress.add_task("Initializing graph...", total=1)
         # Initialise graph with metadata
         g = initialise_graph_with_metadata(
             protein_df=protein_df,
             raw_pdb_df=raw_df,
             name=name,
             pdb_code=pdb_code,
-            pdb_path=pdb_path,
+            path=path,
             granularity=config.granularity,
         )
         # Add nodes to graph
         g = add_nodes_to_graph(g)
 
         # Add config to graph
         g.graph["config"] = config
@@ -874,16 +876,16 @@
 ) -> Union[nx.Graph, None]:
     """
     Protein graph constructor for use in multiprocessing several protein
     structure graphs.
 
     :param args: Tuple of pdb code/path and the chain selection for that PDB.
     :type args: Tuple[str, str]
-    :param use_pdb_code: Whether we are using ``"pdb_code"``s, ``pdb_path``s or
-        ``"uniprot_id"``s.
+    :param use_pdb_code: Whether we are using ``"pdb_code"``s, ``path``s
+        (to PDB or MMTF files) or ``"uniprot_id"``s.
     :type use_pdb_code: bool
     :param config: Protein structure graph construction config
         (see: :class:`graphein.protein.config.ProteinGraphConfig`).
     :type config: ProteinGraphConfig
     :return: Protein structure graph or ``None`` if an error is encountered.
     :rtype: Union[nx.Graph, None]
     """
@@ -893,17 +895,17 @@
     )
     func = partial(construct_graph, config=config)
     try:
         if source == "pdb_code":
             return func(
                 pdb_code=args[0], chain_selection=args[1], model_index=args[2]
             )
-        elif source == "pdb_path":
+        elif source == "path":
             return func(
-                pdb_path=args[0], chain_selection=args[1], model_index=args[2]
+                path=args[0], chain_selection=args[1], model_index=args[2]
             )
         elif source == "uniprot_id":
             return func(
                 uniprot_id=args[0],
                 chain_selection=args[1],
                 model_index=args[2],
             )
@@ -915,32 +917,32 @@
         )
         log.info(ex)
         return None
 
 
 def construct_graphs_mp(
     pdb_code_it: Optional[List[str]] = None,
-    pdb_path_it: Optional[List[str]] = None,
+    path_it: Optional[List[str]] = None,
     uniprot_id_it: Optional[List[str]] = None,
     chain_selections: Optional[List[str]] = None,
     model_indices: Optional[List[str]] = None,
     config: ProteinGraphConfig = ProteinGraphConfig(),
     num_cores: int = 16,
     return_dict: bool = True,
     out_path: Optional[str] = None,
 ) -> Union[List[nx.Graph], Dict[str, nx.Graph]]:
     """
     Constructs protein graphs for a list of pdb codes or pdb paths using
     multiprocessing.
 
     :param pdb_code_it: List of pdb codes to use for protein graph construction
     :type pdb_code_it: Optional[List[str]], defaults to ``None``
-    :param pdb_path_it: List of paths to PDB files to use for protein graph
+    :param path_it: List of paths to PDB or MMTF files to use for protein graph
         construction.
-    :type pdb_path_it: Optional[List[str]], defaults to ``None``
+    :type path_it: Optional[List[str]], defaults to ``None``
     :param chain_selections: List of chains to select from the protein
         structures (e.g. ``["ABC", "A", "L", "CD"...]``).
     :type chain_selections: Optional[List[str]], defaults to ``None``
     :param model_indices: List of model indices to use for protein graph
         construction. Only relevant for structures containing ensembles of
         models.
     :type model_indices: Optional[List[str]], defaults to ``None``
@@ -957,24 +959,24 @@
         saved to disk.
     :type out_path: Optional[str], defaults to ``None``
     :return: Iterable of protein graphs. ``None`` values indicate there was a
         problem in constructing the graph for this particular pdb.
     :rtype: Union[List[nx.Graph], Dict[str, nx.Graph]]
     """
     assert (
-        pdb_code_it is not None or pdb_path_it is not None
+        pdb_code_it is not None or path_it is not None
     ), "Iterable of pdb codes, pdb paths or uniprot IDs required."
 
     if pdb_code_it is not None:
         pdbs = pdb_code_it
         source = "pdb_code"
 
-    if pdb_path_it is not None:
-        pdbs = pdb_path_it
-        source = "pdb_path"
+    if path_it is not None:
+        pdbs = path_it
+        source = "path"
 
     if uniprot_id_it is not None:
         pdbs = uniprot_id_it
         source = "uniprot_id"
 
     if chain_selections is None:
         chain_selections = ["all"] * len(pdbs)
```

### Comparing `graphein-1.6.0/graphein/protein/meshes.py` & `graphein-1.7.0/graphein/protein/meshes.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import os
 import time
 from typing import List, NamedTuple, Optional, Tuple
 
 from loguru import logger as log
 
 from graphein.protein.config import ProteinMeshConfig
+from graphein.utils.dependencies import import_message
 from graphein.utils.pymol import MolViewer
-from graphein.utils.utils import import_message
 
 try:
     from pytorch3d.structures import Meshes
 except ImportError:
     message = import_message(
         submodule="graphein.protein.meshes",
         package="pytorch3d",
```

### Comparing `graphein-1.6.0/graphein/protein/resi_atoms.py` & `graphein-1.7.0/graphein/protein/resi_atoms.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/subgraphs.py` & `graphein-1.7.0/graphein/protein/subgraphs.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/tensor/angles.py` & `graphein-1.7.0/graphein/protein/tensor/angles.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 # Code Repository: https://github.com/a-r-j/graphein
 import copy
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 from loguru import logger as log
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 from ..resi_atoms import ATOM_NUMBERING, CHI_ANGLES_ATOMS
 from .testing import has_nan
 from .types import AtomTensor, CoordTensor, DihedralTensor, TorsionTensor
 
 try:
     from einops import rearrange
 except ImportError:
     message = import_message(
         "graphein.protein.tensor.angles",
         "einops",
         pip_install=True,
+        extras=True,
     )
 
 try:
     from torch_geometric.utils import to_dense_batch
 except ImportError:
     message = import_message(
         "graphein.protein.tensor.angles",
```

### Comparing `graphein-1.6.0/graphein/protein/tensor/data.py` & `graphein-1.7.0/graphein/protein/tensor/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         # From a BioPandas DataFrame
         p = PandasPdb().fetch_pdb("4hhb")
         df = p.df["ATOM"]
         protein = gpt.Protein().from_dataframe(df)
 
         # From a PyG Data object
         data = gpt.io.protein_to_pyg(
-            pdb_code="4hhb", # Can alternatively pass a path or a uniprot ID (for AF2) with pdb_path=... and uniprot_id=...
+            pdb_code="4hhb", # Can alternatively pass a path or a uniprot ID (for AF2) with path=... and uniprot_id=...
             chain_selection="ABCD", # Select all 4 chains
             deprotonate=True, # Deprotonate the structure
             keep_insertions=False, # Remove insertions
             keep_hets=[], # Remove HETATMs
             model_index=1, # Select the first model
             # Can select a subset of atoms with atom_types=...
             )
@@ -190,15 +190,15 @@
         :param atoms_to_keep: List of atom names to preserve.
             See :ref:`graphein.protein.resi_atoms.PROTEIN_ATOMS`
         :type atoms_to_keep: List[str]
         :return: ``Protein` object populated with attributes.
         :rtype: Protein
         """
         self.id = id
-        self.x = protein_df_to_tensor(
+        self.coords = protein_df_to_tensor(
             df, atoms_to_keep=atoms_to_keep, fill_value=self.fill_value
         )
         self.residues = get_sequence(
             df,
             chains="all",
             insertions=False,
             list_of_three=True,
@@ -221,15 +221,15 @@
         Example:
 
         .. code-block:: python
 
             >>> import graphein.protein.tensor as gpt
 
             >>> data = gpt.io.protein_to_pyg(
-                ... pdb_code="4hhb", # Can alternatively pass a path or a uniprot ID (for AF2) with pdb_path=... and uniprot_id=...
+                ... pdb_code="4hhb", # Can alternatively pass a path or a uniprot ID (for AF2) with path=... and uniprot_id=...
                 ... chain_selection="ABCD", # Select all 4 chains
                 ... deprotonate=True, # Deprotonate the structure
                 ... keep_insertions=False, # Remove insertions
                 ... keep_hets=[], # Remove HETATMs
                 ... model_index=1, # Select the first model
                 ... # Can select a subset of atoms with atom_types=...
                 ... )
@@ -275,27 +275,27 @@
         cache: Optional[str] = None,
         **kwargs,
     ) -> Union[pd.DataFrame, PandasPdb]:
         """Compute a Pandas DataFrame from a ``Protein`` object.
 
         .. see:: :func:`graphein.protein.tensor.io.to_dataframe`
 
-        :param x: AtomTensor, defaults to ``None`` (uses ``Protein.x``)
+        :param x: AtomTensor, defaults to ``None`` (uses ``Protein.coords``)
         :type x: Optional[Union[AtomTensor, BackboneTensor]], optional
         :param cache: Whether to store the dataframe as a ``Protein`` attribute,
             defaults to ``None``.
         :type cache: Optional[str], optional
         :param kwargs: Keyword args for
             :func:`graphein.protein.tensor.io.to_dataframe`
         :return: DataFrame of protein structure.
         :rtype: Union[pd.DataFrame, PandasPdb]
         """
 
         if x is None:
-            x = self.x
+            x = self.coords
         out = to_dataframe(
             x=x,
             fill_value=self.fill_value,
             residue_types=self.residue_type,
             chains=self.chains,
             **kwargs,
         )
@@ -324,28 +324,28 @@
 
 
         .. see:: :func:`graphein.protein.tensor.io.to_pdb`
 
         .. seealso:: :meth:`graphein.protein.tensor.io.to_dataframe`
 
 
-        :param x: ``AtomTensor``, defaults to ``None`` (uses ``Protein.x``)
+        :param x: ``AtomTensor``, defaults to ``None`` (uses ``Protein.coords``)
         :type x: Optional[Union[AtomTensor, BackboneTensor]], optional
         :param out_path: Path to output file, defaults to ``None``
             (``{Protein.id}.pdb``)
         :type out_path: Optional[str], optional
         :param gz: Whether or not to gzip the output, defaults to ``False``
         :type gz: bool, optional
         :param kwargs: Additional arguments to pass to
             :func:`graphein.protein.tensor.io.to_pdb`
         """
         if out_path is None:
             out_path = self.id + ".pdb"
         if x is None:
-            x = self.x
+            x = self.coords
         to_pdb(x, out_path, gz, **kwargs)
 
     def from_pdb_code(
         self,
         pdb_code: str,
         chain_selection: str = "all",
         deprotonate: bool = True,
@@ -372,26 +372,26 @@
             data.graph_labels = graph_labels
 
         self.from_data(data)
         return self
 
     def from_pdb_file(
         self,
-        pdb_path: str,
+        path: str,
         chain_selection: str = "all",
         deprotonate: bool = True,
         keep_insertions=False,
         keep_hets: List[str] = [],
         model_index: int = 1,
         atom_types: List[str] = PROTEIN_ATOMS,
         node_labels: Optional[torch.Tensor] = None,
         graph_labels: Optional[torch.Tensor] = None,
     ) -> "Protein":
         data = protein_to_pyg(
-            pdb_path=pdb_path,
+            path=path,
             chain_selection=chain_selection,
             deprotonate=deprotonate,
             keep_insertions=keep_insertions,
             keep_hets=keep_hets,
             model_index=model_index,
             atom_types=atom_types,
         )
@@ -497,15 +497,15 @@
             object with the provided string as the attribute name. Default is
             ``None`` (not stored).
         :type cache: Optional[str]
         :return: Alpha carbon coordinates
         :rtype: graphein.protein.tensor.types.CoordTensor
         """
 
-        out = get_c_alpha(self.x)
+        out = get_c_alpha(self.coords)
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     def backbone(self, cache: Optional[str] = None) -> BackboneTensor:
         """
         Returns the backbone coordinates of the protein as a tensor
@@ -525,15 +525,15 @@
         :param cache: If provided, the result will be cached in the ``Protein``
             object with the provided string as the attribute name. Default is
             ``None`` (not stored).
         :type cache: Optional[str]
         :return: Backbone coordinates ``[Length x 4 x 3]``
         :rtype: graphein.protein.tensor.types.BackboneTensor
         """
-        out = get_backbone(self.x)
+        out = get_backbone(self.coords)
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     def backbone_frames(
         self, cache: Optional[str] = None
     ) -> Tuple[BackboneFrameTensor, CoordTensor]:
@@ -545,15 +545,15 @@
         :param cache: If provided, the result will be cached in the ``Protein``
             object with the provided string as the attribute name. Default is
             ``None`` (not stored).
         :type cache: Optional[str]
         :return: _description_
         :rtype: Tuple[BackboneFrameTensor, CoordTensor]
         """
-        out = get_backbone_frames(self.x)
+        out = get_backbone_frames(self.coords)
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     def idealize_backbone(
         self,
         x: Optional[Union[AtomTensor, BackboneTensor]] = None,
@@ -574,42 +574,42 @@
         :param inplace: Whether or not to optimise the backbone inplace,
             defaults to ``False``.
         :type inplace: bool, optional
         :return: Idealised backbone coordinates
         :rtype: AtomTensor
         """
         if x is None:
-            x = self.x
+            x = self.coords
         return idealize_backbone(x, lr=lr, n_iter=n_iter, inplace=inplace)
 
     def full_atom_coords(self, cache: Optional[str] = None) -> CoordTensor:
         """Gets the full atom coordinates of the protein. Returns tensor of
         shape ``[Length x 3]``.
 
         .. see:: :func:`graphein.protein.tensor.representation.get_full_atom_coords`
 
         :param cache: Whether or not to store the coordinates as an attribute,
             defaults to ``None`` (note stored).
         :type cache: Optional[str], optional
         :return: Tensor of atom positions.
         :rtype: CoordTensor
         """
-        out = get_full_atom_coords(self.x, fill_value=self.fill_value)
+        out = get_full_atom_coords(self.coords, fill_value=self.fill_value)
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     # Angles
     def dihedrals(
         self, rad: bool = True, embed: bool = True, cache: Optional[str] = None
     ) -> DihedralTensor:
         """
         .. see:: :func:`graphein.protein.tensor.angles.dihedrals`
         """
-        out = dihedrals(self.x, rad=rad, embed=embed)
+        out = dihedrals(self.coords, rad=rad, embed=embed)
 
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     def sidechain_torsion(self, cache: Optional[str] = None) -> TorsionTensor:
         """
@@ -618,15 +618,15 @@
         .. see:: :func:`graphein.protein.tensor.angles.sidechain_torsion`
 
         :param: cache: If provided, the result will be cached in the ``Protein``
             under the provided string as the attribute name. Default is ``None``
             , (not stored).
         :type cache: Optional[str]
         """
-        return sidechain_torsion(self.x, self.residues)
+        return sidechain_torsion(self.coords, self.residues)
 
     def kappa(
         self,
         cache: Optional[str] = None,
         rad: bool = True,
         embed: bool = True,
     ) -> torch.Tensor:
@@ -636,15 +636,15 @@
         .. see:: :func:`graphein.protein.tensor.angles.kappa`
 
         :param: cache: If provided, the result will be cached in the ``Protein``
             under the provided string as the attribute name. Default is ``None``,
             (not stored).
         :type cache: Optional[str]
         """
-        out = kappa(self.x, rad=rad, embed=embed)
+        out = kappa(self.coords, rad=rad, embed=embed)
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     def alpha(
         self, cache: Optional[str] = None, rad: bool = True, embed: bool = True
     ) -> torch.Tensor:
@@ -654,15 +654,15 @@
         .. see:: :func:`graphein.protein.tensor.angles.alpha`
 
         :param cache: If provided, the result will be cached in the ``Protein``
             under the provided string as the attribute name. Default is ``None``,
             (not stored).
         :type cache: Optional[str]
         """
-        out = alpha(self.x, rad=rad, embed=embed)
+        out = alpha(self.coords, rad=rad, embed=embed)
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     def align_to(
         self,
         other: "Protein",
@@ -673,16 +673,16 @@
         """Aligns the ``Protein`` to another (``other``) tensor using the Kabsch
         algorithm.
 
         .. see:: :func:`graphein.protein.tensor.geometry.kabsch`
 
         """
         out = kabsch(
-            self.x,
-            other.x,
+            self.coords,
+            other.coords,
             ca_only=ca_only,
             fill_value=self.fill_value,
             return_transformed=return_transformed,
         )
         if cache and return_transformed:
             setattr(self, cache, out)
         elif cache:
@@ -706,27 +706,27 @@
 
         .. see:: :func:`graphein.protein.tensor.testing.is_complete_structure`
 
         :return: Boolean indicating whether or not the ``Protein`` has a
             complete structure.
         :rtype: bool
         """
-        return is_complete_structure(self.x, self.residues)
+        return is_complete_structure(self.coords, self.residues)
 
     def has_complete_backbone(self) -> bool:
         """
         Checks if a ``Protein`` as all backbone atoms present.
 
         .. see:: :func:`graphein.protein.tensor.testing.has_complete_backbone`
 
         :return: Boolean indicating whether or not the ``Protein`` has a
             complete backbone.
         :rtype: bool
         """
-        return has_complete_backbone(self.x)
+        return has_complete_backbone(self.coords)
 
     def __eq__(self, __o: object) -> bool:
         # sourcery skip: merge-duplicate-blocks, merge-else-if-into-elif
         for i in self.keys:
             attr_self = getattr(self, i)
             attr_other = getattr(__o, i)
 
@@ -751,15 +751,15 @@
         """
         if x is None:
             x = self.alpha_carbon()
         return plot_distance_matrix(x)
 
     def plot_dihedrals(self) -> go.Figure:
         dh = (
-            dihedrals(self.x)
+            dihedrals(self.coords)
             if "dihedrals" not in self.keys
             else self.dihedrals
         )
         return plot_dihedrals(dh)
 
     def plot_structure(
         self, atoms: List[str] = ["N", "CA", "C", "O"], lines: bool = True
@@ -777,15 +777,15 @@
 
 
         .. seealso:: :meth:`graphein.protein.tensor.plot.plot_structure`
 
         """
         residue_ids = self.residue_id if hasattr(self, "residue_id") else None
         return plot_structure(
-            self.x, atoms=atoms, lines=lines, residue_ids=residue_ids
+            self.coords, atoms=atoms, lines=lines, residue_ids=residue_ids
         )
 
     def apply_structural_noise(
         self,
         x: Optional[Union[AtomTensor, CoordTensor]] = None,
         magnitude: float = 0.1,
         gaussian: bool = True,
@@ -794,21 +794,21 @@
     ) -> Union[AtomTensor, CoordTensor]:
         """
         Applies noise to the structure of the protein.
 
         .. see:: :func:`graphein.protein.tensor.geometry.apply_structural_noise`
 
         :param x: Coordinates to apply noise to, defaults to ``None``. If
-            ``None`` (default), ``self.x`` is used.
+            ``None`` (default), ``self.coords`` is used.
         :param cache: If provided, the result will be cached in the ``Protein``
             under the provided string as the attribute name. Default is ``None``,
             (not stored).
         """
         if x is None:
-            x = self.x
+            x = self.coords
         out = apply_structural_noise(
             x,
             magnitude=magnitude,
             gaussian=gaussian,
             return_transformed=return_transformed,
         )
         if cache is not None:
@@ -832,24 +832,25 @@
 
         if hasattr(batch, "_slice_dict"):
             self._slice_dict = batch._slice_dict
 
         if hasattr(batch, "_inc_dict"):
             self._inc_dict = batch._inc_dict
 
+        if hasattr(batch, "_num_graphs"):
+            self._num_graphs = batch._num_graphs
+
         # self.fill_value = fill_value
         return self
 
     @classmethod
     def from_protein_list(cls, proteins: List[Protein]):
         # sourcery skip: class-extract-method
         proteins = [Protein().from_data(p) for p in proteins]
         batch = Batch.from_data_list(proteins)
-        # self.from_batch(batch)
-        # return self
         return cls().from_batch(batch)
 
     def from_pdb_codes(
         self,
         pdb_codes: List[str],
         chain_selection: Optional[List[str]] = None,
         node_labels: Optional[List[torch.Tensor]] = None,
@@ -882,27 +883,27 @@
         ]
         batch = Batch.from_data_list(proteins)
         self.from_batch(batch)
         return self
 
     def from_pdb_files(
         self,
-        pdb_paths: List[str],
+        paths: List[str],
         chain_selection: Optional[List[str]] = None,
         node_labels: Optional[List[torch.Tensor]] = None,
         graph_labels: Optional[List[torch.Tensor]] = None,
         model_index: Optional[List[int]] = None,
         atom_types: List[str] = PROTEIN_ATOMS,
         deprotonate: bool = True,
         keep_insertions: bool = False,
         keep_hets: List[str] = [],
     ):
         proteins = [
             Protein().from_pdb_file(
-                pdb_path=pdb,
+                path=pdb,
                 chain_selection=chain_selection[i]
                 if chain_selection is not None
                 else "all",
                 deprotonate=deprotonate,
                 keep_insertions=keep_insertions,
                 keep_hets=keep_hets,
                 model_index=model_index[i] if model_index is not None else 1,
@@ -910,15 +911,15 @@
                 node_labels=node_labels[i]
                 if node_labels is not None
                 else None,
                 graph_labels=graph_labels[i]
                 if graph_labels is not None
                 else None,
             )
-            for i, pdb in enumerate(pdb_paths)
+            for i, pdb in enumerate(paths)
         ]
         batch = Batch.from_data_list(proteins)
         self.from_batch(batch)
         return self
 
     def to_batch(self) -> Batch:
         """Returns the ProteinBatch as a torch_geometric.data.Batch object."""
@@ -956,15 +957,15 @@
             object with the provided string as the attribute name. Default is
             ``None`` (not stored).
         :type cache: Optional[str]
         :return: Alpha carbon coordinates
         :rtype: graphein.protein.tensor.types.CoordTensor
         """
 
-        out = get_c_alpha(self.x)
+        out = get_c_alpha(self.coords)
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     def backbone(self, cache: Optional[str] = None) -> BackboneTensor:
         """
 
@@ -982,15 +983,15 @@
         :param cache: If provided, the result will be cached in the ``Protein``
             object with the provided string as the attribute name. Default is
             ``None`` (not stored).
         :type cache: Optional[str]
         :return: Backbone coordinates ``[Length x 4 x 3]``
         :rtype: graphein.protein.tensor.types.BackboneTensor
         """
-        out = get_backbone(self.x)
+        out = get_backbone(self.coords)
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     def backbone_frames(
         self, cache: Optional[str] = None
     ) -> Tuple[BackboneFrameTensor, CoordTensor]:
@@ -1002,15 +1003,15 @@
         :param cache: If provided, the result will be cached in the ``Protein``
             object with the provided string as the attribute name. Default is
             ``None`` (not stored).
         :type cache: Optional[str]
         :return: _description_
         :rtype: Tuple[BackboneFrameTensor, CoordTensor]
         """
-        out = get_backbone_frames(self.x)
+        out = get_backbone_frames(self.coords)
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     def edges(
         self,
         edge_type: str = "knn_10",
@@ -1060,27 +1061,27 @@
         )
         if cache is not None:
             setattr(self, cache, out)
         return out
 
     # Testing
     def is_complete(self) -> bool:
-        return is_complete_structure(self.x, self.residues)
+        return is_complete_structure(self.coords, self.residues)
 
     def has_complete_backbone(self) -> bool:
         """Returns ``True`` if the protein has a complete backbone, else
         ``False``
 
         .. see:: :func:`graphein.protein.tensor.testing.is_complete_structure`
 
         .. seealso:: :meth:`graphein.protein.tensor.data.ProteinBatch.is_complete`
 
             :meth:`graphein.protein.tensor.testing.has_complete_backbone`
         """
-        return has_complete_backbone(self.x, fill_value=self.fill_value)
+        return has_complete_backbone(self.coords, fill_value=self.fill_value)
 
     def protein_apply(
         self, func: Callable[["Protein"], Any], rebatch: bool = False
     ) -> Union["ProteinBatch", List[Any]]:
         """Applies a function ``func`` to each ``Protein`` in the batch and
         returns the result as a list of ``Proteins`` or a new ``ProteinBatch``.
 
@@ -1090,15 +1091,15 @@
             from graphein.protein.tensor.plot import plot_structure
 
             batch = gpt.data.ProteinBatch().from_pdb_codes(
                 pdb_codes=["3eiy", "4hhb", "1a0q"]
                 )
 
             def single_plot(protein: gpt.Protein()):
-                return plot_structure(protein.x, lines=False)
+                return plot_structure(protein.coords, lines=False)
 
             plots = batch.protein_apply(single_plot)
             plots[2]
 
 
         .. note::
 
@@ -1128,15 +1129,15 @@
         the batch. Returns the result of ``func``.
 
         ..code-block::
 
             from graphein.protein.tensor.plot import plot_structure
 
             def single_plot(protein: gpt.Protein()):
-            return plot_structure(protein.x, lines=False)
+            return plot_structure(protein.coords, lines=False)
 
             plot = batch.apply_to(single_plot, 2)
 
         .. seealso:: :meth:`graphein.protein.tensor.data.ProteinBatch.apply`
 
         :param func: Function to apply to each ``Protein`` in the batch.
         :type func: Callable[["Protein"], Any]
@@ -1273,34 +1274,34 @@
     ) -> Union[AtomTensor, CoordTensor]:
         """
         Applies noise to the structure of the proteins in the batch.
 
         .. see:: :func:`graphein.protein.tensor.geometry.apply_structural_noise`
 
         :param x: Coordinates to apply noise to, defaults to ``None``. If
-            ``None`` (default), ``self.x`` is used.
+            ``None`` (default), ``self.coords`` is used.
         :param cache: If provided, the result will be cached in the
             ``ProteinBatch`` under the provided string as the attribute name.
             Default is ``None``, (not stored).
         """
         if x is None:
-            x = self.x
+            x = self.coords
         out = apply_structural_noise(
             x,
             magnitude=magnitude,
             gaussian=gaussian,
             return_transformed=return_transformed,
         )
         if cache is not None:
             setattr(self, cache, out)
         return out
 
 
 def to_protein(
-    pdb_path: Optional[str] = None,
+    path: Optional[str] = None,
     pdb_code: Optional[str] = None,
     uniprot_id: Optional[str] = None,
     chain_selection: str = "all",
     deprotonate: bool = True,
     keep_insertions: bool = False,
     keep_hets: List[str] = [],
     model_index: int = 1,
@@ -1316,26 +1317,26 @@
         import graphein.protein.tensor as gpt
 
 
         # From PDB code
         gpt.data.to_protein(pdb_code="3eiy", ...)
 
         # From PDB Path
-        gpt.io.to_protein(pdb_path="3eiy.pdb", ...)
+        gpt.io.to_protein(path="3eiy.pdb", ...)
 
         # From UniProt ID
         gpt.io.to_protein(uniprot_id="Q5VSL9", ...)
 
     .. seealso::
 
         :func:`graphein.protein.tensor.io.protein_to_pyg`
         :func:`graphein.protein.tensor.data.to_protein_mp`
 
 
-    :param pdb_path: Path to PDB file. Default is ``None``.
+    :param path: Path to PDB or MMTF file. Default is ``None``.
     :param pdb_code: PDB accesion code. Default is ``None``.
     :param uniprot_id: UniProt ID. Default is ``None``.
     :param chain_selection: Selection of chains to include (e.g. ``"ABC"``) or
         ``"all"``. Default is ``"all"``.
     :param deprotonate: Whether or not to remove Hydrogens. Default is ``True``.
     :param keep_insertions: Whether or not to keep insertions.
     :param keep_hets: List of heteroatoms to include. E.g. ``["HOH"]``.
@@ -1344,15 +1345,15 @@
         :const:`graphein.protein.resi_atoms.PROTEIN_ATOMS`
     :returns: ``Data`` object with attributes: ``x`` (AtomTensor), ``residues``
         (list of 3-letter residue codes), id (ID of protein), residue_id (E.g.
         ``"A:SER:1"``), residue_type (torch.Tensor), ``chains`` (torch.Tensor).
     :rtype: Protein
     """
     data = protein_to_pyg(
-        pdb_path=pdb_path,
+        path=path,
         pdb_code=pdb_code,
         uniprot_id=uniprot_id,
         chain_selection=chain_selection,
         keep_insertions=keep_insertions,
         deprotonate=deprotonate,
         keep_hets=keep_hets,
         model_index=model_index,
@@ -1380,17 +1381,17 @@
     )
     try:
         if source == "pdb_code":
             return func(
                 pdb_code=args[0],
                 chain_selection=args[1],  # , model_index=args[2]
             )
-        elif source == "pdb_path":
+        elif source == "path":
             return func(
-                pdb_path=args[0],
+                path=args[0],
                 chain_selection=args[1],  # , model_index=args[2]
             )
         elif source == "uniprot_id":
             return func(
                 uniprot_id=args[0],
                 chain_selection=args[1],
                 # model_index=args[2],
@@ -1400,15 +1401,15 @@
             f"Graph construction error (PDB={args[0]})! {traceback.format_exc()}"
         )
         log.info(ex)
         return None
 
 
 def to_protein_mp(
-    pdb_paths: Optional[str] = None,
+    paths: Optional[str] = None,
     pdb_codes: Optional[str] = None,
     uniprot_ids: Optional[str] = None,
     chain_selections: Optional[List[str]] = None,
     deprotonate: bool = True,
     keep_insertions: bool = False,
     keep_hets: List[str] = [],
     model_index: int = 1,
@@ -1425,27 +1426,27 @@
 
         import graphein.protein.tensor as gpt
 
         # From PDB codes
         gpt.data.to_protein_mp(pdb_codes=["3eiy", "4hhb", ..., num_cores=8])
 
         # From PDB Paths
-        gpt.io.to_protein_mp(pdb_paths=["3eiy.pdb", "4hhb.pdb", ...])
+        gpt.io.to_protein_mp(paths=["3eiy.pdb", "4hhb.pdb", ...])
 
         # From UniProt IDs
         gpt.io.to_protein_mp(uniprot_ids=["Q5VSL9", ...])
 
 
     .. seealso::
 
         :func:`graphein.protein.tensor.io.protein_to_pyg`
         :func:`graphein.protein.tensor.data.to_protein`
 
 
-    :param pdb_paths: Path to PDB file. Default is ``None``.
+    :param paths: Path to PDB or MMTF files. Default is ``None``.
     :param pdb_codes: PDB accesion code. Default is ``None``.
     :param uniprot_ids: UniProt ID. Default is ``None``.
     :param chain_selections: Selection of chains to include (e.g. ``"ABC"``) or
         ``"all"``. Default is ``"all"``.
     :param deprotonate: Whether or not to remove Hydrogens. Default is ``True``.
     :param keep_insertions: Whether or not to keep insertions.
     :param keep_hets: List of heteroatoms to include. E.g. ``["HOH"]``.
@@ -1455,26 +1456,24 @@
     :param num_cores: Number of cores to use for multiprocessing.
     :returns: ``Data`` object with attributes: ``x`` (AtomTensor), ``residues``
         (list of 3-letter residue codes), id (ID of protein), residue_id (E.g.
         ``"A:SER:1"``), residue_type (torch.Tensor), ``chains`` (torch.Tensor).
     :rtype: List[Protein]
     """
     assert (
-        pdb_codes is not None
-        or pdb_paths is not None
-        or uniprot_ids is not None
+        pdb_codes is not None or paths is not None or uniprot_ids is not None
     ), "Iterable of pdb codes, pdb paths or uniprot IDs required."
 
     if pdb_codes is not None:
         pdbs = pdb_codes
         source = "pdb_code"
 
-    if pdb_paths is not None:
-        pdbs = pdb_paths
-        source = "pdb_path"
+    if paths is not None:
+        pdbs = paths
+        source = "path"
 
     if uniprot_ids is not None:
         pdbs = uniprot_ids
         source = "uniprot_id"
 
     if chain_selections is None:
         chain_selections = ["all"] * len(pdbs)
```

### Comparing `graphein-1.6.0/graphein/protein/tensor/dataloader.py` & `graphein-1.7.0/graphein/protein/tensor/dataloader.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/tensor/dataset.py` & `graphein-1.7.0/graphein/protein/tensor/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from tqdm import tqdm
 
 from graphein.protein.utils import (  # download_pdb,
     download_alphafold_structure,
     download_pdb_multiprocessing,
     read_fasta,
 )
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 from ..folding_utils import esmfold
 from .data import Protein, ProteinBatch, to_protein_mp
 
 try:
     import torch
     from torch_geometric.data import Data, Dataset, InMemoryDataset
@@ -44,15 +44,15 @@
 class ProteinDataset(Dataset):
     def __init__(
         self,
         root: str,
         pdb_dir: str,
         out_dir: str,
         overwrite: bool = False,
-        pdb_paths: Optional[List[str]] = None,
+        paths: Optional[List[str]] = None,
         pdb_codes: Optional[List[str]] = None,
         uniprot_ids: Optional[List[str]] = None,
         sequences: Optional[Union[List[str], str]] = None,
         graph_labels: Optional[List[torch.Tensor]] = None,
         node_labels: Optional[List[torch.Tensor]] = None,
         chain_selections: Optional[List[str]] = None,
         graph_transformation_funcs: Optional[List[Callable]] = None,
@@ -77,17 +77,17 @@
         :type pdb_dir: str, optional
         :param out_dir: Directory to save output files to. If not specified
             (``out_dir=None``), will default to ``root/processed``. Defaults to
             ``None``.
         :param overwrite: Whether to overwrite existing files. Defaults to
             ``False``.
         :type overwrite: bool, optional
-        :param pdb_paths: List of full path of pdb files to load. Defaults to
+        :param paths: List of full path of PDB or MMTF files to load. Defaults to
             ``None``.
-        :type pdb_paths: Optional[List[str]], optional
+        :type paths: Optional[List[str]], optional
         :param pdb_codes: List of PDB codes to download and parse from the PDB.
             Defaults to ``None``.
         :type pdb_codes: Optional[List[str]], optional
         :param uniprot_ids: List of Uniprot IDs to download and parse from
             Alphafold Database. Defaults to ``None``.
         :type uniprot_ids: Optional[List[str]], optional
         :param sequences: List of protein sequences to predict structures of with
@@ -149,31 +149,31 @@
             if uniprot_ids is not None
             else None
         )
         if sequences is not None:
             self.sequences = sequences
             self.fold_sequences()
 
-        self.pdb_paths = pdb_paths
-        if self.pdb_paths is None:
+        self.paths = paths
+        if self.paths is None:
             if self.pdb_codes and self.uniprot_ids:
                 self.structures = self.pdb_codes + self.uniprot_ids
             elif self.pdb_codes:
                 self.structures = pdb_codes
             elif self.uniprot_ids:
                 self.structures = uniprot_ids
         # Use local saved pdb_files instead of download or move them to
         # self.root/raw dir
         else:
-            if isinstance(self.pdb_paths, list):
+            if isinstance(self.paths, list):
                 self.structures = [
-                    os.path.splitext(os.path.split(pdb_path)[-1])[0]
-                    for pdb_path in self.pdb_paths
+                    os.path.splitext(os.path.split(path)[-1])[0]
+                    for path in self.paths
                 ]
-                self.pdb_path, _ = os.path.split(self.pdb_paths[0])
+                self.path, _ = os.path.split(self.paths[0])
 
         # Labels & chains
         self.chain_selections = chain_selections
         if self.chain_selections is not None:
             self.chain_selections = [
                 chain if chain is not None else "all"
                 for chain in self.chain_selections
@@ -406,15 +406,15 @@
             # Create graph objects
             file_names: List[str] = [f"{self.raw_dir}/{pdb}" for pdb in pdbs]
             file_names: List[str] = [
                 f if f.endswith(".pdb") else f"{f}.pdb" for f in file_names
             ]
             print(file_names)
             graphs = to_protein_mp(
-                pdb_paths=file_names,
+                paths=file_names,
                 # config=self.config,
                 # TODO args
                 chain_selections=chains,
                 num_cores=self.num_cores,
             )
 
             if self.graph_transformation_funcs is not None:
```

### Comparing `graphein-1.6.0/graphein/protein/tensor/edges.py` & `graphein-1.7.0/graphein/protein/tensor/edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utilities for computing edges."""
 from typing import Optional
 
 from loguru import logger as log
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 from .types import CoordTensor, EdgeTensor, OptTensor
 
 try:
     import torch
 except ImportError:
     message = import_message(
```

### Comparing `graphein-1.6.0/graphein/protein/tensor/geometry.py` & `graphein-1.7.0/graphein/protein/tensor/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # License: MIT
 # Project Website: https://github.com/a-r-j/graphein
 # Code Repository: https://github.com/a-r-j/graphein
 from typing import List, Tuple, Union
 
 from loguru import logger as log
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 from ..resi_atoms import (
     CHI_ANGLES_ATOMS,
     IDEAL_BB_BOND_ANGLES,
     IDEAL_BB_BOND_LENGTHS,
 )
 from .angles import get_backbone_bond_angles, get_backbone_bond_lengths
```

### Comparing `graphein-1.6.0/graphein/protein/tensor/io.py` & `graphein-1.7.0/graphein/protein/tensor/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Utilities for parsing proteins into and out of tensors."""
 # Graphein
 # Author: Arian Jamasb <arian@jamasb.io>
 # License: MIT
 # Project Website: https://github.com/a-r-j/graphein
 # Code Repository: https://github.com/a-r-j/graphein
 
+import os
 from typing import List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from biopandas.pdb import PandasPdb
 from loguru import logger as log
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 from ..graphs import (
     deprotonate_structure,
     filter_hetatms,
     read_pdb_to_dataframe,
     remove_insertions,
     select_chains,
@@ -90,15 +91,15 @@
     else:
         ids = df["residue_id"].values
 
     return len(set(ids))
 
 
 def protein_to_pyg(
-    pdb_path: Optional[str] = None,
+    path: Optional[Union[str, os.PathLike]] = None,
     pdb_code: Optional[str] = None,
     uniprot_id: Optional[str] = None,
     chain_selection: str = "all",
     deprotonate: bool = True,
     keep_insertions: bool = False,
     keep_hets: List[str] = [],
     model_index: int = 1,
@@ -113,21 +114,24 @@
 
         import graphein.protein.tensor as gpt
 
         # From PDB code
         gpt.io.protein_to_pyg(pdb_code="3eiy")
 
         # From PDB Path
-        gpt.io.protein_to_pyg(pdb_path="3eiy.pdb")
+        gpt.io.protein_to_pyg(path="3eiy.pdb")
+
+        # From MMTF Path
+        gpt.io.protein_to_pyg(path="3eiy.mmtf")
 
         # From UniProt ID
-        gpt.io.protein_to_pyg(pdb_path="Q5VSL9")
+        gpt.io.protein_to_pyg(uniprot_id="Q5VSL9")
 
 
-    :param pdb_path: Path to PDB file. Default is ``None``.
+    :param path: Path to PDB or MMTF file. Default is ``None``.
     :param pdb_code: PDB accesion code. Default is ``None``.
     :param uniprot_id: UniProt ID. Default is ``None``.
     :param chain_selection: Selection of chains to include (e.g. ``"ABC"``) or
         ``"all"``. Default is ``"all"``.
     :param deprotonate: Whether or not to remove Hydrogens. Default is ``True``.
     :param keep_insertions: Whether or not to keep insertions.
     :param keep_hets: List of heteroatoms to include. E.g. ``["HOH"]``.
@@ -137,19 +141,19 @@
     :returns: ``Data`` object with attributes: ``x`` (AtomTensor), ``residues``
         (list of 3-letter residue codes), id (ID of protein), residue_id (E.g.
         ``"A:SER:1"``), residue_type (torch.Tensor), ``chains`` (torch.Tensor).
     :rtype: torch_geometric.data.Data
     """
 
     # Get ID
-    if pdb_path is not None:
+    if path is not None:
         id = (
-            pdb_path.split("/")[-1] + "_" + chain_selection
+            path.split("/")[-1] + "_" + chain_selection
             if chain_selection != "all"
-            else pdb_path
+            else path
         )
     elif pdb_code is not None:
         id = (
             pdb_code + "_" + chain_selection
             if chain_selection != "all"
             else pdb_code
         )
@@ -157,15 +161,15 @@
         id = (
             uniprot_id + "_" + chain_selection
             if chain_selection != "all"
             else uniprot_id
         )
 
     df = read_pdb_to_dataframe(
-        pdb_path=pdb_path,
+        path=path,
         pdb_code=pdb_code,
         uniprot_id=uniprot_id,
         model_index=model_index,
     )
     df = select_chains(df, chain_selection)
     if deprotonate:
         df = deprotonate_structure(df)
@@ -184,15 +188,15 @@
         + ":"
         + df["residue_number"].astype(str)
     )
     if keep_insertions:
         df["residue_id"] = df.residue_id + ":" + df.insertion
 
     return Data(
-        x=protein_df_to_tensor(df, atoms_to_keep=atom_types),
+        coords=protein_df_to_tensor(df, atoms_to_keep=atom_types),
         residues=get_sequence(
             df,
             chains=chain_selection,
             insertions=keep_insertions,
             list_of_three=True,
         ),
         id=id,
@@ -311,15 +315,15 @@
     used.
 
     .. code-block:: python
 
         import graphein.protein.tensor as gpt
 
         protein = gpt.Protein().from_pdb_code("3eiy")
-        to_dataframe(protein.x)
+        to_dataframe(protein.coords)
 
     .. seealso::
 
         :class:`graphein.protein.tensor.types.AtomTensor`
         :meth:`graphein.protein.tensor.io.to_pdb`
         :meth:`graphein.protein.tensor.sequence.infer_residue_types`
```

### Comparing `graphein-1.6.0/graphein/protein/tensor/plot.py` & `graphein-1.7.0/graphein/protein/tensor/plot.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/tensor/pnerf.py` & `graphein-1.7.0/graphein/protein/tensor/pnerf.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/tensor/reconstruction.py` & `graphein-1.7.0/graphein/protein/tensor/reconstruction.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/protein/tensor/representation.py` & `graphein-1.7.0/graphein/protein/tensor/representation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Project Website: https://github.com/a-r-j/graphein
 # Code Repository: https://github.com/a-r-j/graphein
 
 from typing import List, Tuple, Union
 
 from loguru import logger as log
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 from .reconstruction import get_ideal_backbone_coords
 from .types import AtomTensor, BackboneFrameTensor, BackboneTensor, CoordTensor
 
 try:
     import torch
 except ImportError:
```

### Comparing `graphein-1.6.0/graphein/protein/tensor/sequence.py` & `graphein-1.7.0/graphein/protein/tensor/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Code Repository: https://github.com/a-r-j/graphein
 from functools import lru_cache
 from typing import Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 from loguru import logger as log
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 from ..resi_atoms import (
     ATOM_NUMBERING_MODIFIED,
     RESI_THREE_TO_1,
     STANDARD_AMINO_ACIDS,
     STANDARD_RESIDUE_ATOMS,
 )
```

### Comparing `graphein-1.6.0/graphein/protein/tensor/testing.py` & `graphein-1.7.0/graphein/protein/tensor/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utilities for sanity checking protein tensors."""
 from functools import partial
 from typing import List, Tuple, Union
 
 from loguru import logger as log
 
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 from ..resi_atoms import (
     ATOM_NUMBERING_MODIFIED,
     STANDARD_AMINO_ACID_MAPPING_1_TO_3,
 )
 from .sequence import get_atom_indices
 from .types import AtomTensor, BackboneTensor, CoordTensor, ResidueTensor
```

### Comparing `graphein-1.6.0/graphein/protein/tensor/types.py` & `graphein-1.7.0/graphein/protein/tensor/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,57 +5,57 @@
 # Graphein
 # Author: Arian Jamasb <arian@jamasb.io>
 # License: MIT
 # Project Website: https://github.com/a-r-j/graphein
 # Code Repository: https://github.com/a-r-j/graphein
 from typing import NewType, Optional, Union
 
-import torch
-from torchtyping import TensorType
+from jaxtyping import Float
+from torch import Tensor
 
 # Positions
-AtomTensor = NewType("AtomTensor", TensorType[-1, 37, 3])
+AtomTensor = NewType("AtomTensor", Float[Tensor, "-1 37 3"])
 """
-``TensorType[-1, 37, 3]``
+``torch.float[-1, 37, 3]``
 
 Tensor of atom coordinates. The first dimension is the length of the protein,
 the second the number of canonical atom types. The last dimension contains the
 x,y,z positions.
 
 .. seealso:: :class:`ResidueTensor` :class:`CoordTensor`
 """
 
-BackboneTensor = NewType("BackboneTensor", TensorType[-1, 4, 3])
+BackboneTensor = NewType("BackboneTensor", Float[Tensor, "-1 4 3"])
 """
-``TensorType[-1, 4, 3]``
+``torch.float[-1, 4, 3]``
 
 Tensor of backbone atomic coordinates. The first dimension is the length of the
 protein (or batch), the second dimension corresponds to ``[N, Ca, C, O]`` atoms
 and the last dimension contains the x,y,z coordinates.
 
 .. seealso:: :ref:`graphein.protein.tensor.types.AtomTensor
 
 """
 
-ResidueTensor = NewType("ResidueTensor", TensorType[37, 3])
+ResidueTensor = NewType("ResidueTensor", Float[Tensor, "37 3"])
 """
-``TensorType[37, 3]``
+``torch.float[37, 3]``
 
 Tensor of atom coordinates for a residue. Each index in dimension one
 corresponds to an atom (See: :ref:`graphein.protein.resi_atoms.ATOM_NUMBERING`).
 The last dimension contains the x,y,z positions. Missing atoms are denoted by a
 fill value (default = ``1e-5``).
 
 .. seealso:: :class:`AtomTensor` :class:`CoordTensor`
 """
 
 
-CoordTensor = NewType("CoordTensor", TensorType[-1, 3])
+CoordTensor = NewType("CoordTensor", Float[Tensor, "-1 3"])
 """
-``TensorType[-1, 3]``
+``torch.float[-1, 3]``
 
 Tensor of coordinates. The first dimension is the length of the protein
 (or batch of proteins), the last dimension contains the x,y,z positions."""
 
 PositionTensor = NewType("PositionTensor", Union[AtomTensor, CoordTensor])
 """
 Union[:ref:`graphein.protein.tensor.types.AtomTensor,
@@ -64,63 +64,63 @@
 
 Union of ``AtomTensor`` and ``CoordTensor``.
 
 .. seealso:: :class:`AtomTensor`, :class:`CoordTensor`
 """
 
 # Represenations
-BackboneFrameTensor = NewType("BackboneFrameTensor", TensorType[-1, 3, 3])
+BackboneFrameTensor = NewType("BackboneFrameTensor", Float[Tensor, "-1 3 3"])
 """
-``TensorType[-1, 3, 3]``
+``torch.float[-1, 3, 3]``
 
 Tensor of backbone frames as rotation matrices. The first dimension is the
 length of the protein, the second and third dimensions specify a rotation matrix
 relative to an idealised residue.
 
 .. seealso::
     :ref:`graphein.protein.tensor.reconstruction.get_ideal_backbone_coords
 """
 
-ResidueFrameTensor = NewType("ResidueFrameTensor", TensorType[3, 3])
+ResidueFrameTensor = NewType("ResidueFrameTensor", Float[Tensor, "3 3"])
 """
-``TensorType[3, 3]``
+``torch.float[3, 3]``
 
 .. seealso:: :class:`BackboneFrameTensor`
 """
 
 
 # Rotations
-EulerAngleTensor = NewType("EulerAngleTensor", TensorType[-1, 3])
+EulerAngleTensor = NewType("EulerAngleTensor", Float[Tensor, "-1 3"])
 
-QuaternionTensor = NewType("QuaternionTensor", TensorType[-1, 4])
+QuaternionTensor = NewType("QuaternionTensor", Float[Tensor, "-1 4"])
 """
-``TensorType[-1, 4]``
+``torch.float[-1, 4]``
 
 Tensor of quaternions. The first dimension is the length of the protein
 (or batch), the second dimension is the quaternion.
 
 .. see:: https://en.wikipedia.org/wiki/Quaternion
 """
 
 
-TransformTensor = NewType("TransformTensor", TensorType[-1, 4, 4])
+TransformTensor = NewType("TransformTensor", Float[Tensor, "-1 4 4"])
 
 
-RotationMatrix2D = NewType("RotationMatrix2D", TensorType[2, 2])
+RotationMatrix2D = NewType("RotationMatrix2D", Float[Tensor, "2 2"])
 """
-``TensorType[2, 2]``
+``torch.float[2, 2]``
 
 Specifies a 2D rotation matrix.
 
 .. seealso:: :class:`RotationMatrix3D` :class:`RotationMatrix` :class:`RotationTensor`
 """
 
-RotationMatrix3D = NewType("RotationMatrix3D", TensorType[3, 3])
+RotationMatrix3D = NewType("RotationMatrix3D", Float[Tensor, "3 3"])
 """
-``TensorType[3, 3]``
+``torch.float[3, 3]``
 
 Specifies a 3D rotation matrix.
 
 .. seealso:: :class:`RotationMatrix2D` :class:`RotationMatrix` :class:`RotationTensor`
 """
 
 RotationMatrix = NewType(
@@ -131,76 +131,79 @@
 
 Specifies a rotation matrix in either 2D or 3D.
 
 .. seealso:: :class:`RotationMatrix2D` :class:`RotationMatrix3D` :class:`RotationTensor`
 """
 
 
-RotationMatrixTensor = NewType("RotationMatrixTensor", TensorType[-1, 3, 3])
+RotationMatrixTensor = NewType("RotationMatrixTensor", Float[Tensor, "-1 3 3"])
 
 RotationTensor = NewType(
     "RotationTensor", Union[QuaternionTensor, RotationMatrixTensor]
 )
 
 
 # Angles
 DihedralTensor = NewType(
-    "DihedralTensor", Union[TensorType[-1, 3], TensorType[-1, 6]]
+    "DihedralTensor", Union[Float[Tensor, "-1 3"], Float[Tensor, "-1 6"]]
 )
 """
-``Union[TensorType[-1, 3], TensorType[-1, 6]]``
+``Union[torch.float[-1, 3], torch.float[-1, 6]]``
 
 Tensor of backbone dihedral angles (phi, psi, omega). Either in degrees/radians
 or embedded on the unit sphere ``[cos(phi), sin(phi), cos(psi), sin(psi), ...]``
 
 .. seealso::
 
     :meth:graphein.protein.tensor.angles.dihedrals,
     :meth:graphein.protein.tensor.angles.dihedrals_to_rad
     :meth:graphein.protein.tensor.plot.plot_dihedrals
 
 """
 
 TorsionTensor = NewType(
-    "TorsionTensor", Union[TensorType[-1, 4], TensorType[-1, 8]]
+    "TorsionTensor", Union[Float[Tensor, "-1 4"], Float[Tensor, "-1 8"]]
 )
 """
-``Union[TensorType[-1, 4], TensorType[-1, 8]]``
+``Union[torch.float[-1, 4], torch.float[-1, 8]]``
 
 Tensor of sidechain torsion angles ``[chi1, chi2, chi3, chi4]``. Either in
 degrees/radians or embedded on the unit sphere:
 ``[cos(chi1), sin(chi1), cos(chi2), sin(chi2), ...]``.
 
 .. seealso::
 
     :meth:graphein.protein.tensor.angles.sidechain_torsions,
     :meth:graphein.protein.tensor.angles.torsions_to_rad
 
 """
 
-BackboneFrameTensor = NewType("BackboneFrameTensor", TensorType[-1, 3, 3])
+BackboneFrameTensor = NewType("BackboneFrameTensor", Float[Tensor, "-1 3 3"])
 """
-``TensorType[-1, 3, 3]``
+``torch.float[-1, 3, 3]``
 
 Tensor of backbone frames as rotation matrices. The first dimension is the
 length of the protein, the second and third dimensions specify a rotation matrix
 relative to an idealised residue.
 
 .. seealso::
 
     :meth:`graphein.protein.tensor.reconstruction.get_ideal_backbone_coords`
     :meth:`graphein.protein.tensor.representation.get_backbone_frames`
 """
 
-ResidueFrameTensor = NewType("ResidueFrameTensor", TensorType[3, 3])
+ResidueFrameTensor = NewType("ResidueFrameTensor", Float[Tensor, "3 3"])
 """
-``TensorType[-1, 3, 3]``
+``torch.float[-1, 3, 3]``
 
 .. seealso:: :class:`BackboneFrameTensor`
 """
 
-EdgeTensor = NewType("EdgeTensor", TensorType[2, -1])
+EdgeTensor = NewType("EdgeTensor", Float[Tensor, "2 -1"])
 
 
-ScalarTensor = NewType("ScalarTensor", TensorType[-1])
+OrientationTensor = NewType("OrientationTensor", Float[Tensor, "-1 2 3"])
 
-OptTensor = NewType("OptTensor", Optional[torch.Tensor])
+
+ScalarTensor = NewType("ScalarTensor", Float[Tensor, "-1"])
+
+OptTensor = NewType("OptTensor", Optional[Tensor])
```

### Comparing `graphein-1.6.0/graphein/protein/utils.py` & `graphein-1.7.0/graphein/protein/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,25 +87,28 @@
 
     return sequences
 
 
 def download_pdb_multiprocessing(
     pdb_codes: List[str],
     out_dir: Union[str, Path],  # type: ignore
+    format: str = "pdb",
     overwrite: bool = False,
     strict: bool = False,
     max_workers: int = 16,
     chunksize: int = 32,
 ) -> List[Path]:
     """Downloads PDB structures in parallel.
 
     :param pdb_codes: List of PDB codes to download.
     :type pdb_codes: List[str]
     :param out_dir: Path to directory to download PDB structures to.
     :type out_dir: Union[str, Path]
+    :param format: Filetype to download. ``pdb`` or ``mmtf``.
+    :type format: str
     :param overwrite: Whether to overwrite existing files, defaults to
         ``False``.
     :type overwrite: bool
     :param strict: Whether to check for successful download of each file,
         defaults to ``False``.
     :type strict: bool
     :param max_workers: Number of workers to uses, defaults to 16
@@ -113,24 +116,29 @@
     :param chunksize: Chunk to split list into for each worker, defaults to 32
     :type chunksize: int
     :return: List of Paths to downloaded PDB files.
     :rtype: List[Path]
     """
     out_dir: Path = Path(out_dir)
     func = partial(
-        download_pdb, out_dir=out_dir, overwrite=overwrite, strict=strict
+        download_pdb,
+        out_dir=out_dir,
+        format=format,
+        overwrite=overwrite,
+        strict=strict,
     )
     return process_map(
         func, pdb_codes, max_workers=max_workers, chunksize=chunksize
     )
 
 
 def download_pdb(
     pdb_code: str,
     out_dir: Optional[Union[str, Path]] = None,
+    format: str = "pdb",
     check_obsolete: bool = False,
     overwrite: bool = False,
     strict: bool = True,
 ) -> Path:
     """
     Download PDB structure from PDB.
 
@@ -138,84 +146,98 @@
     obsolete PDB codes (ftp://ftp.wwpdb.org/pub/pdb/data/status/obsolete.dat)
 
     :param pdb_code: 4 character PDB accession code.
     :type pdb_code: str
     :param out_dir: Path to directory to download PDB structure to. If ``None``,
         will download to a temporary directory.
     :type out_dir: Optional[Union[str, Path]]
+    :param format: Filetype to download. ``pdb`` or ``mmtf``.
+    :type format: str
     :param check_obsolete: Whether to check for obsolete PDB codes,
         defaults to ``False``. If an obsolete PDB code is found, the updated PDB
         is downloaded.
     :type check_obsolete: bool
     :param overwrite: If ``True``, will overwrite existing files.
     :type overwrite: bool
     :param strict: If ``True``, will raise an exception if the PDB file is not
         found.
     :type strict: bool
     :return: returns filepath to downloaded structure.
     :rtype: Path
     """
     pdb_code = pdb_code.lower()
+    if format == "pdb":
+        BASE_URL = "https://files.rcsb.org/download/"
+        extension = ".pdb"
+    elif format == "mmtf":
+        BASE_URL = "https://mmtf.rcsb.org/v1.0/full/"
+        extension = ".mmtf.gz"
+    else:
+        raise ValueError(f"Invalid format: {format}. Must be 'pdb' or 'mmtf'.")
 
     # Make output directory if it doesn't exist or set it to tempdir if None
     if out_dir is not None:
         out_dir = Path(out_dir)
     else:
         out_dir = Path(tempfile.TemporaryDirectory().name)
 
     os.makedirs(Path(out_dir), exist_ok=True)
 
     if check_obsolete:
         obs_map = get_obsolete_mapping()
         try:
             new_pdb = obs_map[pdb_code.lower()].lower()
             log.info(
-                "{pdb_code} is deprecated. Downloading {new_pdb} instead."
+                f"{pdb_code} is deprecated. Downloading {new_pdb} instead."
+            )
+            return download_pdb(
+                new_pdb, out_dir, format=format, overwrite=overwrite
             )
-            return download_pdb(new_pdb, out_dir, overwrite=overwrite)
         except KeyError:
             log.warning(
                 f"PDB {pdb_code} not found. Possibly too large; large \
                     structures are only provided as mmCIF files."
             )
             return
 
     # Check if PDB already exists
-    if os.path.exists(out_dir / f"{pdb_code}.pdb") and not overwrite:
-        log.info(f"{pdb_code} already exists: {out_dir / f'{pdb_code}.pdb'}")
-        return out_dir / f"{pdb_code}.pdb"
+    if os.path.exists(out_dir / f"{pdb_code}{extension}") and not overwrite:
+        log.info(
+            f"{pdb_code} already exists: {out_dir / f'{pdb_code}{extension}'}"
+        )
+        return out_dir / f"{pdb_code}{extension}"
 
     # Download
     try:
         wget.download(
-            f"https://files.rcsb.org/download/{pdb_code}.pdb",
-            out=str(out_dir / f"{pdb_code}.pdb"),
+            f"{BASE_URL}{pdb_code}{extension}",
+            out=str(out_dir / f"{pdb_code}{extension}"),
         )
     except HTTPError:
         log.warning(f"PDB {pdb_code} not found.")
 
     # Check file exists
     if strict:
         assert os.path.exists(
-            out_dir / f"{pdb_code}.pdb"
-        ), "{pdb_code} download failed. Not found in {out_dir}"
-    log.info("{pdb_code} downloaded to {out_dir}")
-    return out_dir / f"{pdb_code}.pdb"
+            out_dir / f"{pdb_code}{extension}"
+        ), f"{pdb_code} download failed. Not found in {out_dir}"
+    log.info(f"{pdb_code} downloaded to {out_dir}")
+    return out_dir / f"{pdb_code}{extension}"
 
 
-def get_protein_name_from_filename(pdb_path: str) -> str:
+def get_protein_name_from_filename(path: str) -> str:
     """
-    Extracts a filename from a ``pdb_path``
+    Extracts a filename from a ``path``
 
-    :param pdb_path: Path to extract filename from.
-    :type pdb_path: str
+    :param path: Path to extract filename from.
+    :type path: str
     :return: file name.
     :rtype: str
     """
-    _, tail = os.path.split(pdb_path)
+    _, tail = os.path.split(path)
     tail = os.path.splitext(tail)[0]
     return tail
 
 
 def filter_dataframe(
     dataframe: pd.DataFrame,
     by_column: str,
@@ -448,28 +470,14 @@
         ppd.df["ATOM"] = atom_df
     if hetatms:
         ppd.df["HETATM"] = hetatm_df
     ppd.to_pdb(path=path, records=None, gz=gz, append_newline=True)
     log.info(f"Successfully saved rgroup data to {path}")
 
 
-def is_tool(name: str) -> bool:
-    """Checks whether ``name`` is on ``PATH`` and is marked as an executable.
-
-    Source:
-    https://stackoverflow.com/questions/11210104/check-if-a-program-exists-from-a-python-script
-
-    :param name: Name of program to check for execution ability.
-    :type name: str
-    :return: Whether ``name`` is on PATH and is marked as an executable.
-    :rtype: bool
-    """
-    return which(name) is not None
-
-
 def esmfold(
     sequence: str,
     out_path: Optional[str] = None,
     version: int = 1,
     format: str = "pdb",
 ):
     """Fold a protein sequence using the ESMFold model from the ESMFold server at
@@ -500,7 +508,49 @@
     header = "\n".join(
         [f"data_{sequence}", "#", f"_entry.id\t{sequence}", "#\n"]
     )
     cif = header + cif
     if out_path is not None:
         with open(out_path, "w") as f:
             f.write(cif)
+
+
+def extract_chains_to_file(
+    pdb_file: str, chains: List[str], out_dir: str, models: List[int] = [1]
+) -> List[str]:
+    """Extracts chains from a PDB file to separate files.
+
+    .. code-block::python
+
+        extract_chains_to_file("4hhb.pdb", ["A", "B"], ".", [1])
+
+    This will create new files ``./4hhb_A.pdb`` and ``./4hhb_B.pdb``.
+
+
+    :param pdb_file: PDB file
+    :type pdb_file: str
+    :param chains: List of chains to extract
+    :type chains: List[str]
+    :param out_file: Directory of output files
+    :type out_file: str
+    :param models: List of indices of models from which to extract chains,
+        defaults to ``[1]``.
+    :type models: List[int], optional
+    :return: List of output file paths
+    :rtype: List[str]
+    """
+    fname = os.path.basename(pdb_file)
+    fname = fname.split(".")[0]
+
+    ppdb = PandasPdb().read_pdb(pdb_file).get_models(models)
+
+    out_files = []
+    for chain in chains:
+        out_path = os.path.join(out_dir, f"{fname}_{chain}.pdb")
+        out_files.append(out_path)
+        df = ppdb.df["ATOM"].loc[ppdb.df["ATOM"]["chain_id"] == chain]
+        out_df = PandasPdb()
+        out_df.df["ATOM"] = df
+        out_df.to_pdb(
+            path=out_path, records=None, gz=False, append_newline=True
+        )
+    return out_files
```

### Comparing `graphein-1.6.0/graphein/protein/visualisation.py` & `graphein-1.7.0/graphein/protein/visualisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import plotly.express as px
 import plotly.graph_objects as go
 import seaborn as sns
 from loguru import logger as log
 from mpl_toolkits.mplot3d import Axes3D
 
 from graphein.protein.subgraphs import extract_k_hop_subgraph
-from graphein.utils.utils import import_message
+from graphein.utils.dependencies import import_message
 
 try:
     from pytorch3d.ops import sample_points_from_meshes
 except ImportError:
     message = import_message(
         submodule="graphein.protein.visualisation",
         package="pytorch3d",
@@ -37,14 +37,15 @@
 try:
     from mpl_chord_diagram import chord_diagram
 except ImportError:
     import_message(
         submodule="graphein.protein.visualisation",
         package="mpl_chord_diagram",
         pip_install=True,
+        extras=True,
     )
 
 
 def plot_pointcloud(mesh: Meshes, title: str = "") -> Axes3D:
     """
     Plots pytorch3d Meshes object as pointcloud.
```

### Comparing `graphein-1.6.0/graphein/rna/config.py` & `graphein-1.7.0/graphein/rna/config.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/rna/constants.py` & `graphein-1.7.0/graphein/rna/constants.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/rna/edges/atomic.py` & `graphein-1.7.0/graphein/rna/edges/atomic.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/rna/edges/base_pairing.py` & `graphein-1.7.0/graphein/rna/edges/base_pairing.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/rna/features/atom.py` & `graphein-1.7.0/graphein/rna/features/atom.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/rna/graphs.py` & `graphein-1.7.0/graphein/rna/graphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # Graphein
 # Author: Arian Jamasb <arian@jamasb.io>, Emmanuele Rossi, Eric Ma
 # License: MIT
 # Project Website: https://github.com/a-r-j/graphein
 # Code Repository: https://github.com/a-r-j/graphein
 # This submodule is heavily inspired by: https://github.com/emalgorithm/rna-design/blob/aec77a18abe4850958d6736ec185a6f8cbfdf20c/src/util.py#L9
 
-from typing import Callable, List, Optional
+import os
+from typing import Callable, List, Optional, Union
 
 import networkx as nx
 from loguru import logger as log
 
 import graphein.protein.graphs as gp
 from graphein.rna.config import BpRNAConfig, RNAGraphConfig
 from graphein.rna.constants import (
@@ -90,39 +91,39 @@
                 in the sequence {db}."
         )
 
 
 def construct_rna_graph_3d(
     config: Optional[RNAGraphConfig] = None,
     name: Optional[str] = None,
-    pdb_path: Optional[str] = None,
+    path: Optional[Union[str, os.PathLike]] = None,
     pdb_code: Optional[str] = None,
     chain_selection: str = "all",
     model_index: int = 1,
     rna_df_processing_funcs: Optional[List[Callable]] = None,
     edge_construction_funcs: Optional[List[Callable]] = None,
     edge_annotation_funcs: Optional[List[Callable]] = None,
     node_annotation_funcs: Optional[List[Callable]] = None,
     graph_annotation_funcs: Optional[List[Callable]] = None,
 ) -> nx.Graph:
     """
-    Constructs RNA structure graph from a ``pdb_code`` or ``pdb_path``.
+    Constructs RNA structure graph from a ``pdb_code`` or ``path``.
 
     Users can provide a :class:`~graphein.rna.config.RNAGraphConfig`
     object to specify construction parameters.
 
     However, config parameters can be overridden by passing arguments directly
     to the function.
 
     :param config: :class:`~graphein.rna.config.RNAGraphConfig` object. If
         ``None``, defaults to config in ``graphein.rna.config``.
     :type config: graphein.protein.config.RNAGraphConfig, optional
-    :param pdb_path: Path to ``pdb_file`` to build graph from. Default is
+    :param path: Path to PDB or MMTF to build graph from. Default is
         ``None``.
-    :type pdb_path: str, optional
+    :type path: str, optional
     :param pdb_code: 4-character PDB accession pdb_code to build graph from.
         Default is ``None``.
     :type pdb_code: str, optional
     :param chain_selection: String of nucleotide chains to include in graph.
         E.g ``"ABDF"`` or ``"all"``. Default is ``"all"``.
     :type chain_selection: str
     :param model_index: Index of model to use in the case of structural
@@ -148,16 +149,16 @@
     """
 
     # If no config is provided, use default
     if config is None:
         config = RNAGraphConfig()
 
     # Get name from pdb_file is no pdb_code is provided
-    if pdb_path and (pdb_code is None):
-        pdb_code = gp.get_protein_name_from_filename(pdb_path)
+    if path and (pdb_code is None):
+        pdb_code = gp.get_protein_name_from_filename(path)
 
     # If config params are provided, overwrite them
     config.rna_df_processing_functions = (
         rna_df_processing_funcs
         if config.rna_df_processing_functions is None
         else config.rna_df_processing_functions
     )
@@ -179,15 +180,15 @@
     config.edge_metadata_functions = (
         edge_annotation_funcs
         if config.edge_metadata_functions is None
         else config.edge_metadata_functions
     )
 
     raw_df = gp.read_pdb_to_dataframe(
-        pdb_path,
+        path,
         pdb_code,
         model_index=model_index,
     )
 
     raw_df = gp.sort_dataframe(raw_df)
     protein_df = gp.process_dataframe(
         raw_df,
@@ -199,15 +200,15 @@
 
     # Initialise graph with metadata
     g = gp.initialise_graph_with_metadata(
         protein_df=protein_df,
         raw_pdb_df=raw_df,
         name=name,
         pdb_code=pdb_code,
-        pdb_path=pdb_path,
+        path=path,
         granularity=config.granularity,
     )
     # Add nodes to graph
     g = gp.add_nodes_to_graph(g)
 
     # Add config to graph
     g.graph["config"] = config
@@ -339,30 +340,30 @@
 def construct_graph(
     dotbracket: Optional[str] = None,
     sequence: Optional[str] = None,
     bprna_id: Optional[str] = None,
     use_nussinov: bool = False,
     name: Optional[str] = None,
     config: Optional[RNAGraphConfig] = None,
-    pdb_path: Optional[str] = None,
+    path: Optional[str] = None,
     pdb_code: Optional[str] = None,
     chain_selection: str = "all",
     rna_df_processing_funcs: Optional[List[Callable]] = None,
     edge_construction_funcs: Optional[List[Callable]] = None,
     edge_annotation_funcs: Optional[List[Callable]] = None,
     node_annotation_funcs: Optional[List[Callable]] = None,
     graph_annotation_funcs: Optional[List[Callable]] = None,
 ) -> nx.Graph:
     # TODO Docstring
 
-    if pdb_path is not None or pdb_code is not None:
+    if path is not None or pdb_code is not None:
         return construct_rna_graph_3d(
             config=config,
             name=name,
-            pdb_path=pdb_path,
+            path=path,
             pdb_code=pdb_code,
             chain_selection=chain_selection,
             rna_df_processing_funcs=rna_df_processing_funcs,
             edge_construction_funcs=edge_construction_funcs,
             edge_annotation_funcs=edge_annotation_funcs,
             node_annotation_funcs=node_annotation_funcs,
             graph_annotation_funcs=graph_annotation_funcs,
```

### Comparing `graphein-1.6.0/graphein/rna/nussinov.py` & `graphein-1.7.0/graphein/rna/nussinov.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/rna/subgraphs.py` & `graphein-1.7.0/graphein/rna/subgraphs.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/rna/utils.py` & `graphein-1.7.0/graphein/rna/utils.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/rna/visualisation.py` & `graphein-1.7.0/graphein/rna/visualisation.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/testing/utils.py` & `graphein-1.7.0/graphein/testing/utils.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/utils/config.py` & `graphein-1.7.0/graphein/utils/config.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/utils/config_parser.py` & `graphein-1.7.0/graphein/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/utils/pymol/core.py` & `graphein-1.7.0/graphein/utils/pymol/core.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/graphein/utils/utils.py` & `graphein-1.7.0/graphein/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -329,57 +329,14 @@
     :returns: Single-letter amino acid code
     :rtype: str
     """
     amino_acid = amino_acid[0] + amino_acid[1:].lower()
     return protein_letters_3to1[amino_acid]
 
 
-def import_message(
-    submodule: str,
-    package: str,
-    conda_channel: Optional[str] = None,
-    pip_install: bool = False,
-) -> str:
-    """
-    Return warning if package is not found.
-    Generic message for indicating to the user when a function relies on an
-    optional module / package that is not currently installed. Includes
-    installation instructions. Typically used in conjunction without optional featurisation libraries
-
-    :param submodule: graphein submodule that needs an external dependency.
-    :type submodule: str
-    :param package: External package this submodule relies on.
-    :type package: str
-    :param conda_channel: Conda channel package can be installed from, if at all. Defaults to ``None``.
-    :type conda_channel: str, optional
-    :param pip_install: Whether package can be installed via pip. Defaults to ``False``.
-    :type pip_install: bool
-    """
-    is_conda = os.path.exists(os.path.join(sys.prefix, "conda-meta"))
-    installable = True
-    if is_conda:
-        if conda_channel is None:
-            installable = False
-            installation = f"{package} cannot be installed via conda"
-        else:
-            installation = f"conda install -c {conda_channel} {package}"
-    elif pip_install:
-        installation = f"pip install {package}"
-    else:
-        installable = False
-        installation = f"{package} cannot be installed via pip"
-
-    message = f"To use the Graphein submodule {submodule}, you need to install: {package} "
-    if installable:
-        message += f"\nTo do so, use the following command: {installation}"
-    else:
-        message += f"\n{installation}"
-    return message
-
-
 def ping(host: str) -> bool:
     """
     Returns ``True`` if host (str) responds to a ping request.
     Remember that a host may not respond to a ping (ICMP) request even if the host name is valid.
 
     :param host: IP or hostname
     :type host: str
```

### Comparing `graphein-1.6.0/graphein.egg-info/SOURCES.txt` & `graphein-1.7.0/graphein.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 README.md
 pyproject.toml
 setup.py
 .requirements/base.in
 .requirements/dev.in
 .requirements/docs.in
 .requirements/extras.in
+.requirements/torch_cpu.in
+.requirements/torch_gpu.in
 graphein/__init__.py
 graphein/cli.py
 graphein.egg-info/PKG-INFO
 graphein.egg-info/SOURCES.txt
 graphein.egg-info/dependency_links.txt
 graphein.egg-info/entry_points.txt
 graphein.egg-info/requires.txt
@@ -26,14 +28,16 @@
 graphein/ml/__init__.py
 graphein/ml/clustering.py
 graphein/ml/conversion.py
 graphein/ml/diffusion.py
 graphein/ml/utils.py
 graphein/ml/visualisation.py
 graphein/ml/datasets/__init__.py
+graphein/ml/datasets/foldcomp_dataset.py
+graphein/ml/datasets/pdb_data.py
 graphein/ml/datasets/torch_geometric_dataset.py
 graphein/ml/metrics/__init__.py
 graphein/ml/metrics/gdt.py
 graphein/ml/metrics/tm_score.py
 graphein/molecule/__init__.py
 graphein/molecule/atoms.py
 graphein/molecule/chembl.py
@@ -125,20 +129,23 @@
 graphein/rna/features/__init__.py
 graphein/rna/features/atom.py
 graphein/testing/__init__.py
 graphein/testing/utils.py
 graphein/utils/__init__.py
 graphein/utils/config.py
 graphein/utils/config_parser.py
+graphein/utils/dependencies.py
 graphein/utils/utils.py
 graphein/utils/pymol/__init__.py
 graphein/utils/pymol/compat.py
 graphein/utils/pymol/core.py
 tests/__init__.py
 tests/test_graphein.py
+tests/datasets/__init__.py
+tests/datasets/pdb_data.py
 tests/grn/__init__.py
 tests/grn/test_graphs.py
 tests/ml/__init__.py
 tests/ml/test_conversion.py
 tests/ml/test_torch_geometric_dataset.py
 tests/ppi/__init__.py
 tests/ppi/test_graphs.py
```

### Comparing `graphein-1.6.0/graphein.egg-info/requires.txt` & `graphein-1.7.0/graphein.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-biopandas>=0.4.1
+pandas<2.0.0
+biopandas==0.5.0.dev0
 biopython
 bioservices>=1.10.0
 deepdiff
 loguru
 matplotlib>=3.4.3
 multipledispatch
 networkx
@@ -11,36 +12,36 @@
 plotly
 pydantic
 rich
 rich-click
 seaborn
 pyyaml<6.0,>=5.1
 scikit-learn
-scipy
+scipy>=1.8
 tqdm
-typing_extensions
+typing_extensions==4.5.0
 wget
 xarray
-torchtyping
+jaxtyping
 
 [all]
-pytest-xdist
-interrogate
-nbstripout
-black
 isort
 pytest
-nbval
 pandoc
-pytest-cov
-pycodestyle
+black
+nbstripout
 pre-commit
+pydocstyle
+pytest-cov
+pytest-xdist
+nbval
 flake8
+interrogate
 hypothesis
-pydocstyle
+pycodestyle
 
 [dev]
 black
 flake8
 hypothesis
 interrogate
 isort
```

### Comparing `graphein-1.6.0/pyproject.toml` & `graphein-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/setup.py` & `graphein-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         os.system("git push --tags")
 
         sys.exit()
 
 
 setup(
     name="graphein",
-    version="1.6.0",
+    version="1.7.0",
     description="Protein & Interactomic Graph Construction for Machine Learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Arian Jamasb",
     author_email="arian@jamasb.io",
     url="https://github.com/a-r-j/graphein",
     project_urls={
```

### Comparing `graphein-1.6.0/tests/grn/test_graphs.py` & `graphein-1.7.0/tests/grn/test_graphs.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/ml/test_conversion.py` & `graphein-1.7.0/tests/ml/test_conversion.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/ml/test_torch_geometric_dataset.py` & `graphein-1.7.0/tests/ml/test_torch_geometric_dataset.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/ppi/test_graphs.py` & `graphein-1.7.0/tests/ppi/test_graphs.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/protein/edges/test_distance.py` & `graphein-1.7.0/tests/protein/edges/test_distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 DATA_PATH = Path(__file__).resolve().parent.parent / "test_data" / "4hhb.pdb"
 
 
 def generate_graph():
     """Generate PDB network.
     This is a helper function.
     """
-    return construct_graph(pdb_path=str(DATA_PATH))
+    return construct_graph(path=str(DATA_PATH))
 
 
 @pytest.fixture(scope="module")
 def net():
     """Generate proteingraph from 2VUI.pdb."""
     return generate_graph()
 
@@ -183,15 +183,15 @@
 
         assert condition1 or condition2
 
 
 def test_add_peptide_bonds():
     file_path = Path(__file__).parent.parent / "test_data/4hhb.pdb"
     # Peptide bonds are default
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     for u, v in G.edges():
         assert abs(int(u.split(":")[2]) - int(v.split(":")[2])) == 1
 
 
 def test_add_sequence_distance_edges():
     D = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
@@ -199,15 +199,15 @@
 
     for d in D:
         config = ProteinGraphConfig(
             edge_construction_functions=[
                 partial(add_sequence_distance_edges, d=d)
             ]
         )
-        G = construct_graph(pdb_path=str(file_path), config=config)
+        G = construct_graph(path=str(file_path), config=config)
         for u, v in G.edges():
             assert abs(int(u.split(":")[2]) - int(v.split(":")[2])) == d
 
 
 def test_salt_bridge_interactions():
     """
     Test to ensure salt bridges are only between anionic and cationic residues.
```

### Comparing `graphein-1.6.0/tests/protein/nodes/features/test_amino_acid.py` & `graphein-1.7.0/tests/protein/nodes/features/test_amino_acid.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/protein/nodes/features/test_geometry.py` & `graphein-1.7.0/tests/protein/nodes/features/test_geometry.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/protein/tensor/test_angles.py` & `graphein-1.7.0/tests/protein/tensor/test_angles.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/protein/tensor/test_geometry.py` & `graphein-1.7.0/tests/protein/tensor/test_geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,26 +69,28 @@
     assert torch.allclose(
         coords_aligned, coords, atol=1e-6
     ), "Coords differ too much after alignment"
 
 
 def test_idealise_backbone():
     protein = gpt.Protein().from_pdb_code(pdb_code="5caj", chain_selection="A")
-    protein.x = protein.x[:20, :, :]
+    protein.coords = protein.coords[:20, :, :]
 
     ideal = protein.idealize_backbone(n_iter=100)
 
-    IDEAL_BL = torch.tensor(IDEAL_BB_BOND_LENGTHS, device=protein.x.device)
-    IDEAL_BA = torch.tensor(IDEAL_BB_BOND_ANGLES, device=protein.x.device)
+    IDEAL_BL = torch.tensor(
+        IDEAL_BB_BOND_LENGTHS, device=protein.coords.device
+    )
+    IDEAL_BA = torch.tensor(IDEAL_BB_BOND_ANGLES, device=protein.coords.device)
 
     ideal_bl = IDEAL_BL - get_backbone_bond_lengths(ideal[:, :4, :])
-    true_bl = IDEAL_BL - get_backbone_bond_lengths(protein.x[:, :4, :])
+    true_bl = IDEAL_BL - get_backbone_bond_lengths(protein.coords[:, :4, :])
 
     ideal_ba = IDEAL_BA - get_backbone_bond_angles(ideal[:, :4, :])
-    true_ba = IDEAL_BA - get_backbone_bond_angles(protein.x[:, :4, :])
+    true_ba = IDEAL_BA - get_backbone_bond_angles(protein.coords[:, :4, :])
 
     assert torch.mean(torch.abs(ideal_ba)) < torch.mean(
         torch.abs(true_ba)
     ), "Bond angles not more idealised"
     assert torch.mean(torch.abs(ideal_bl)) < torch.mean(
         torch.abs(true_bl)
     ), "Bond lengths not more idealised"
```

### Comparing `graphein-1.6.0/tests/protein/tensor/test_io.py` & `graphein-1.7.0/tests/protein/tensor/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     assert positions.shape[0] == num_residues, "Incorrect number of residues."
     assert positions.shape[1] == 4, "Incorrect number of atoms."
     assert positions.shape[2] == 3, "Incorrect number of coordinates."
 
 
 def test_to_pdb():
     protein = Protein().from_pdb_code("4hhb")
-    to_pdb(protein.x, "test.pdb")
+    to_pdb(protein.coords, "test.pdb")
     assert os.path.exists("test.pdb"), "File does not exist"
 
     ppdb1 = PandasPdb().read_pdb("test.pdb")
     ppdb2 = PandasPdb().fetch_pdb("4hhb")
 
     assert_frame_equal(
         ppdb1.df["ATOM"][["x_coord", "y_coord", "z_coord"]][:50],
```

### Comparing `graphein-1.6.0/tests/protein/tensor/test_reconstruction.py` & `graphein-1.7.0/tests/protein/tensor/test_reconstruction.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/protein/tensor/test_representation.py` & `graphein-1.7.0/tests/protein/tensor/test_representation.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/protein/tensor/test_sequence.py` & `graphein-1.7.0/tests/protein/tensor/test_sequence.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/protein/test_graphs.py` & `graphein-1.7.0/tests/protein/test_graphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,26 @@
 from graphein.protein.graphs import (
     compute_chain_graph,
     compute_secondary_structure_graph,
     construct_graph,
     construct_graphs_mp,
     read_pdb_to_dataframe,
 )
-from graphein.protein.utils import is_tool
+from graphein.utils.dependencies import is_tool
 
 DATA_PATH = Path(__file__).resolve().parent / "test_data" / "4hhb.pdb"
 
 DSSP_AVAILABLE = is_tool("mkdssp")
 
 
 def generate_graph():
     """Generate PDB network.
     This is a helper function.
     """
-    return construct_graph(pdb_path=str(DATA_PATH))
+    return construct_graph(path=str(DATA_PATH))
 
 
 @pytest.fixture(scope="module")
 def net():
     """Generate proteingraph from 2VUI.pdb."""
     return generate_graph()
 
@@ -85,15 +85,15 @@
 # Example-based Graph Construction test
 def test_construct_graph():
     """Example-based test that graph construction works correctly.
 
     Uses 4hhb PDB file as an example test case.
     """
     file_path = Path(__file__).parent / "test_data" / "4hhb.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
     assert isinstance(G, nx.Graph)
     assert len(G) == 574
 
     # Check number of peptide bonds
     peptide_bond_edges = [
         (u, v)
         for u, v, d in G.edges(data=True)
@@ -129,25 +129,25 @@
     dssp_prot_config = ProteinGraphConfig(**dssp_config_functions)
 
     g_pdb = construct_graph(
         config=dssp_prot_config, pdb_code="6rew"
     )  # should download 6rew.pdb to pdb_dir
 
     assert g_pdb.graph["pdb_code"] == "6rew"
-    assert g_pdb.graph["pdb_path"] is None
+    assert g_pdb.graph["path"] is None
     assert g_pdb.graph["name"] == g_pdb.graph["pdb_code"]
     assert len(g_pdb.graph["dssp_df"]) == 1365
 
     file_path = str(
         Path(__file__).parent / "test_data" / "alphafold_structure.pdb"
     )
-    g_local = construct_graph(config=dssp_prot_config, pdb_path=file_path)
+    g_local = construct_graph(config=dssp_prot_config, path=file_path)
 
     assert g_local.graph["pdb_code"] is None
-    assert g_local.graph["pdb_path"] == file_path
+    assert g_local.graph["path"] == file_path
     assert g_local.graph["name"] == "alphafold_structure"
     assert len(g_local.graph["dssp_df"]) == 382
 
 
 def test_construct_graphs_mp():
     graph_list = [
         "2olg",
@@ -181,24 +181,24 @@
 
 def test_chain_selection():
     """Example-based test that chain selection works correctly.
 
     Uses 4hhb PDB file as an example test case.
     """
     file_path = Path(__file__).parent / "test_data" / "4hhb.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     # Check default construction contains all chains
     assert G.graph["chain_ids"] == ["A", "B", "C", "D"]
     # Check nodes contain residues from chains
     for n, d in G.nodes(data=True):
         assert d["chain_id"] in ["A", "B", "C", "D"]
 
     # Check graph contains only chain selection
-    G = construct_graph(pdb_path=str(file_path), chain_selection="AD")
+    G = construct_graph(path=str(file_path), chain_selection="AD")
     assert G.graph["chain_ids"] == ["A", "D"]
     # Check nodes only contain residues from chain selection
     for n, d in G.nodes(data=True):
         assert d["chain_id"] in ["A", "D"]
 
 
 # Edge construction tests
@@ -221,15 +221,15 @@
             pi_stacking,
             salt_bridge,
             t_stacking,
             van_der_waals,
         ]
     }
     config = ProteinGraphConfig(**edge_functions)
-    G = construct_graph(pdb_path=str(file_path), config=config)
+    G = construct_graph(path=str(file_path), config=config)
     # Todo complete
 """
 
 
 def test_distance_edges():
     """Example-based test that distance-based edge construction works correctly
 
@@ -254,15 +254,15 @@
                 add_distance_threshold,
                 threshold=12,
                 long_interaction_threshold=10,
             ),
         ]
     }
     config = ProteinGraphConfig(**edge_functions)
-    G = construct_graph(pdb_path=str(file_path), config=config)
+    G = construct_graph(path=str(file_path), config=config)
     assert G is not None
 
 
 # Featurisation tests
 @pytest.mark.skipif(not DSSP_AVAILABLE, reason="DSSP not installed.")
 def test_node_features():
     # Todo this test requires attention
@@ -284,15 +284,15 @@
             psi,
             secondary_structure,
             # partial(aaindex1, accession="FAUJ880111"),
         ],
         "dssp_config": DSSPConfig(),
     }
     config = ProteinGraphConfig(**config_params)
-    G = construct_graph(pdb_path=str(file_path), config=config)
+    G = construct_graph(path=str(file_path), config=config)
 
     # Check for existence of features
     for _, d in G.nodes(data=True):
         # Todo these functions return pd.Series, rather than adding to the node
         assert "meiler" in d.keys()
         assert "expasy" in d.keys()
         assert "rsa" in d.keys()
@@ -314,15 +314,15 @@
             # esm_sequence_embedding,
             # esm_residue_embedding,
             biovec_sequence_embedding,
             molecular_weight,
         ]
     }
     config = ProteinGraphConfig(**sequence_feature_functions)
-    G = construct_graph(pdb_path=str(file_path), config=config)
+    G = construct_graph(path=str(file_path), config=config)
 
     # Check for existence on sequence-based features as node-level features
     # for n, d in G.nodes(data=True):
     # Todo this can probably be improved.
     # This only checks for the existence and shape of the esm_embedding for each
     # node
     # assert "esm_embedding" in d
@@ -490,15 +490,15 @@
             add_disulfide_interactions,
             add_peptide_bonds,
             add_hydrogen_bond_interactions,
         ],
         graph_metadata_functions=[secondary_structure],
         dssp_config=DSSPConfig(),
     )
-    g = construct_graph(pdb_path=str(file_path), config=config)
+    g = construct_graph(path=str(file_path), config=config)
 
     h = compute_secondary_structure_graph(g, remove_non_ss=False)
     # Check number of residues preserved
     res_counts = sum(d["residue_counts"] for _, d in h.nodes(data=True))
     assert res_counts == len(
         g
     ), "Residue counts in SS graph should match number of residues in original \
@@ -528,15 +528,15 @@
             add_disulfide_interactions,
             add_peptide_bonds,
             add_hydrogen_bond_interactions,
         ],
         graph_metadata_functions=[secondary_structure],
         dssp_config=DSSPConfig(),
     )
-    g = construct_graph(pdb_path=str(file_path), config=config)
+    g = construct_graph(path=str(file_path), config=config)
     h = compute_chain_graph(g)
     assert len(h.edges) == len(g.edges), "Number of edges do not match"
 
     h = compute_chain_graph(g, return_weighted_graph=True)
     node_sum = sum(d["num_residues"] for _, d in h.nodes(data=True))
     assert node_sum == len(g), "Number of residues do not match"
```

### Comparing `graphein-1.6.0/tests/protein/test_subgraphs.py` & `graphein-1.7.0/tests/protein/test_subgraphs.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     extract_subgraph_from_chains,
     extract_subgraph_from_node_list,
     extract_subgraph_from_point,
     extract_subgraph_from_residue_types,
     extract_subgraph_from_secondary_structure,
     extract_surface_subgraph,
 )
-from graphein.protein.utils import is_tool
+from graphein.utils.dependencies import is_tool
 
 DSSP_AVAILABLE = is_tool("mkdssp")
 
 
 def test_node_list_subgraphing():
     """Tests subgraph extraction from a list of nodes."""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
     NODE_LIST = ["C:ALA:28", "C:ARG:31", "D:LEU:75", "A:THR:38"]
 
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     g = extract_subgraph_from_node_list(G, NODE_LIST, filter_dataframe=True)
 
     # Check we get back a graph and it contains the correct nodes
     assert isinstance(g, nx.Graph)
     assert len(g) == len(NODE_LIST)
     for n in g.nodes():
@@ -84,15 +84,15 @@
 
     assert all(elem not in NODE_LIST for elem in returned_node_list)
 
 
 def test_extract_subgraph_from_atom_types():
     """Tests subgraph extraction from a list of allowed atom types"""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     ATOM_TYPES = ["CA"]
     g = extract_subgraph_from_atom_types(G, ATOM_TYPES, filter_dataframe=True)
     assert isinstance(g, nx.Graph)
     assert len(g) == len(G)
 
 
@@ -100,15 +100,15 @@
     """Tests subgraph extraction from a list of nodes."""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
     RESIDUE_TYPES = ["ALA", "SER", "GLY"]
     ALANINES = 72
     SERINES = 32
     GLYCINES = 40
 
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     g = extract_subgraph_from_residue_types(
         G, RESIDUE_TYPES, filter_dataframe=True
     )
 
     # Check we get back a graph and it contains the correct nodes
     assert isinstance(g, nx.Graph)
@@ -161,15 +161,15 @@
 
     assert all(elem not in RESIDUE_TYPES for elem in returned_node_list)
 
 
 def test_extract_subgraph_from_point():
     """Tests subgraph extraction from a spherical selection."""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     POINT = np.array([0.0, 0.0, 0.0])
     RADIUS = 10
     s_g = extract_subgraph_from_point(G, POINT, RADIUS, filter_dataframe=True)
 
     # Check all nodes are within the sphere
     for n, d in s_g.nodes(data=True):
@@ -193,15 +193,15 @@
         if np.linalg.norm(d["coords"] - POINT) > RADIUS:
             assert n in s_g.nodes()
 
 
 def test_extract_subgraph_from_chains():
     """Tests subgraph extraction from chains."""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     CHAINS = ["A", "C"]
     s_g = extract_subgraph_from_chains(G, CHAINS, filter_dataframe=True)
 
     # Test we only selected the correct chains
     for n, d in s_g.nodes(data=True):
         assert d["chain_id"] in CHAINS
@@ -228,15 +228,15 @@
             assert n not in s_g.nodes()
 
 
 # @pytest.mark.skip(reason="TODO")
 def test_extract_subgraph_from_sequence_position():
     """Tests subgraph extraction from sequence position."""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     SEQ_POS = list(range(1, 50, 2))
 
     s_g = extract_subgraph_by_sequence_position(
         G,
         SEQ_POS,
         filter_dataframe=True,
@@ -268,15 +268,15 @@
 
 def test_extract_subgraph_from_bond_type():
     """Tests subgraph extraction from bond type"""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
     config = ProteinGraphConfig(
         edge_construction_functions=[add_peptide_bonds, add_ionic_interactions]
     )
-    G = construct_graph(pdb_path=str(file_path))  # , config=config)
+    G = construct_graph(path=str(file_path))  # , config=config)
 
     BOND_TYPES = ["ionic"]
 
     s_g = extract_subgraph_by_bond_type(G, BOND_TYPES, filter_dataframe=True)
 
     for u, v, d in G.edges(data=True):
         if d["kind"] in BOND_TYPES:
@@ -300,15 +300,15 @@
         for bond in list(d["kind"]):
             assert bond not in BOND_TYPES
 
 
 def test_extract_k_hop_subgraph():
     """Tests k-hop subgraph extraction."""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     CENTRAL_NODE = "B:SER:49"
     K = 1
     s_g = extract_k_hop_subgraph(G, CENTRAL_NODE, K, filter_dataframe=True)
 
     for n in s_g.nodes():
         if n != CENTRAL_NODE:
@@ -321,15 +321,15 @@
 @pytest.mark.skipif(not DSSP_AVAILABLE, reason="DSSP not installed.")
 def test_surface_subgraph():
     """Tests surface subgraph extraction."""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
     config = ProteinGraphConfig(
         graph_metadata_functions=[rsa], dssp_config=DSSPConfig()
     )
-    G = construct_graph(pdb_path=str(file_path), config=config)
+    G = construct_graph(path=str(file_path), config=config)
 
     RSA_THRESHOLD: float = 0.2
     s_g = extract_surface_subgraph(G, RSA_THRESHOLD, filter_dataframe=True)
 
     for n, d in s_g.nodes(data=True):
         assert d["rsa"] >= RSA_THRESHOLD
 
@@ -342,15 +342,15 @@
 def test_secondary_structure_subgraph():
     """Tests secondary subgraph extraction."""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
     config = ProteinGraphConfig(
         graph_metadata_functions=[secondary_structure],
         dssp_config=DSSPConfig(),
     )
-    G = construct_graph(pdb_path=str(file_path), config=config)
+    G = construct_graph(path=str(file_path), config=config)
 
     SS_ELEMENTS: List[str] = ["H"]
     s_g = extract_subgraph_from_secondary_structure(
         G, SS_ELEMENTS, filter_dataframe=True
     )
 
     for _, d in s_g.nodes(data=True):
@@ -365,15 +365,15 @@
 def test_successful_pickle():
     """Tests subgraphs can be successfully pickled and unpickled"""
     file_path = Path(__file__).parent / "test_data/4hhb.pdb"
     config = ProteinGraphConfig(
         graph_metadata_functions=[secondary_structure],
         dssp_config=DSSPConfig(),
     )
-    G = construct_graph(pdb_path=str(file_path), config=config)
+    G = construct_graph(path=str(file_path), config=config)
     s_g = extract_subgraph_from_residue_types(
         G,
         residue_types=["ALA", "SER", "MET"],
         update_coords=True,
         filter_dataframe=True,
         recompute_distmat=True,
     )
```

### Comparing `graphein-1.6.0/tests/protein/test_utils.py` & `graphein-1.7.0/tests/protein/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     # Check for equivalence between saved and existing DFs.
     # We drop the line_idx columns as these will be renumbered
     assert_frame_equal(
         a.drop(["line_idx"], axis=1),
         g.graph["pdb_df"].drop(["line_idx", "node_id", "residue_id"], axis=1),
     )
-    h = construct_graph(pdb_path="/tmp/test_graph.pdb")
+    h = construct_graph(path="/tmp/test_graph.pdb")
 
     # We check for isomorphism rather than equality as array features are not
     # comparable
     assert nx.is_isomorphic(g, h)
 
 
 def test_save_pdb_df_to_pdb():
@@ -51,15 +51,15 @@
     assert_frame_equal(
         a.drop(["line_idx"], axis=1),
         g.graph["pdb_df"].drop(["line_idx", "node_id", "residue_id"], axis=1),
     )
 
     # Now check for raw, unprocessed DF
     save_pdb_df_to_pdb(g.graph["raw_pdb_df"], "/tmp/test_pdb.pdb")
-    h = construct_graph(pdb_path="/tmp/test_pdb.pdb")
+    h = construct_graph(path="/tmp/test_pdb.pdb")
 
     # We check for isomorphism rather than equality as array features are not
     # comparable
     assert nx.is_isomorphic(g, h)
 
 
 def test_save_rgroup_df_to_pdb():
```

### Comparing `graphein-1.6.0/tests/rna/test_graphs.py` & `graphein-1.7.0/tests/rna/test_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,27 +76,27 @@
 
     for _, _, d in g.edges(data=True):
         assert "kind" in d.keys()
         assert "bond_length" in d.keys()
 
     assert "name" in g.graph.keys()
     assert "pdb_code" in g.graph.keys()
-    assert "pdb_path" in g.graph.keys()
+    assert "path" in g.graph.keys()
     assert "chain_ids" in g.graph.keys()
     assert "pdb_df" in g.graph.keys()
     assert "raw_pdb_df" in g.graph.keys()
     assert "coords" in g.graph.keys()
 
 
 def test_construct_graph():
     """Example-based test that graph construction works correctly.
     Uses 4hhb PDB file as an example test case.
     """
     file_path = Path(__file__).parent / "test_data/2jyf.pdb"
-    g = construct_graph(pdb_path=str(file_path))
+    g = construct_graph(path=str(file_path))
 
     for n, d in g.nodes(data=True):
         assert isinstance(n, str)
         assert "coords" in d.keys()
         assert "chain_id" in d.keys()
         assert "residue_name" in d.keys()
         assert "residue_number" in d.keys()
@@ -105,12 +105,12 @@
 
     for _, _, d in g.edges(data=True):
         assert "kind" in d.keys()
         assert "bond_length" in d.keys()
 
     assert "name" in g.graph.keys()
     assert "pdb_code" in g.graph.keys()
-    assert "pdb_path" in g.graph.keys()
+    assert "path" in g.graph.keys()
     assert "chain_ids" in g.graph.keys()
     assert "pdb_df" in g.graph.keys()
     assert "raw_pdb_df" in g.graph.keys()
     assert "coords" in g.graph.keys()
```

### Comparing `graphein-1.6.0/tests/rna/test_subgraphs.py` & `graphein-1.7.0/tests/rna/test_subgraphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     NODE_LIST = [
         "A:A:4:121:N3",
         "A:A:4:122:C4",
         "A:U:5:134:P",
         "A:U:5:135:OP1",
     ]
 
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     g = extract_subgraph_from_node_list(G, NODE_LIST, filter_dataframe=True)
 
     # Check we get back a graph and it contains the correct nodes
     assert isinstance(g, nx.Graph)
     assert len(g) == len(NODE_LIST)
     for n in g.nodes():
@@ -74,15 +74,15 @@
 
     assert all(elem not in NODE_LIST for elem in returned_node_list)
 
 
 def test_extract_subgraph_from_atom_types():
     """Tests subgraph extraction from a list of allowed atom types"""
     file_path = Path(__file__).parent / "test_data/2jyf.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     ATOM_TYPES = ["P"]
     g = extract_subgraph_from_atom_types(G, ATOM_TYPES, filter_dataframe=True)
     assert isinstance(g, nx.Graph)
     assert len(g) == 84
 
 
@@ -90,15 +90,15 @@
     """Tests subgraph extraction from a list of nodes."""
     file_path = Path(__file__).parent / "test_data/2jyf.pdb"
     RESIDUE_TYPES = ["A", "G"]
 
     A_COUNT = 484  # TODO
     G_COUNT = 592  # TODO
 
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     g = extract_subgraph_from_residue_types(
         G, RESIDUE_TYPES, filter_dataframe=True
     )
 
     # Check we get back a graph and it contains the correct nodes
     assert isinstance(g, nx.Graph)
@@ -147,15 +147,15 @@
 
     assert all(elem not in RESIDUE_TYPES for elem in returned_node_list)
 
 
 def test_extract_subgraph_from_point():
     """Tests subgraph extraction from a spherical selection."""
     file_path = Path(__file__).parent / "test_data/2jyf.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     POINT = np.array([0.0, 0.0, 0.0])
     RADIUS = 10
     s_g = extract_subgraph_from_point(G, POINT, RADIUS, filter_dataframe=True)
 
     # Check all nodes are within the sphere
     for n, d in s_g.nodes(data=True):
@@ -179,15 +179,15 @@
         if np.linalg.norm(d["coords"] - POINT) > RADIUS:
             assert n in s_g.nodes()
 
 
 def test_extract_subgraph_from_chains():
     """Tests subgraph extraction from chains."""
     file_path = Path(__file__).parent / "test_data/2jyf.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     CHAINS = ["A", "C"]
     s_g = extract_subgraph_from_chains(G, CHAINS, filter_dataframe=True)
 
     # Test we only selected the correct chains
     for n, d in s_g.nodes(data=True):
         assert d["chain_id"] in CHAINS
@@ -214,15 +214,15 @@
             assert n not in s_g.nodes()
 
 
 # @pytest.mark.skip(reason="TODO")
 def test_extract_subgraph_from_sequence_position():
     """Tests subgraph extraction from sequence position."""
     file_path = Path(__file__).parent / "test_data/2jyf.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     SEQ_POS = list(range(1, 50, 2))
 
     s_g = extract_subgraph_by_sequence_position(
         G,
         SEQ_POS,
         filter_dataframe=True,
@@ -251,15 +251,15 @@
         if d["residue_number"] in SEQ_POS:
             assert n not in s_g.nodes()
 
 
 def test_extract_subgraph_from_bond_type():
     """Tests subgraph extraction from bond type"""
     file_path = Path(__file__).parent / "test_data/2jyf.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     BOND_TYPES = ["covalent"]
 
     s_g = extract_subgraph_by_bond_type(G, BOND_TYPES, filter_dataframe=True)
 
     for u, v, d in G.edges(data=True):
         if d["kind"] in BOND_TYPES:
@@ -283,15 +283,15 @@
         for bond in list(d["kind"]):
             assert bond not in BOND_TYPES
 
 
 def test_extract_k_hop_subgraph():
     """Tests k-hop subgraph extraction."""
     file_path = Path(__file__).parent / "test_data/2jyf.pdb"
-    G = construct_graph(pdb_path=str(file_path))
+    G = construct_graph(path=str(file_path))
 
     CENTRAL_NODE = "A:A:6:181:N6"
     K = 1
     s_g = extract_k_hop_subgraph(G, CENTRAL_NODE, K, filter_dataframe=True)
 
     for n in s_g.nodes():
         if n != CENTRAL_NODE:
```

### Comparing `graphein-1.6.0/tests/testing/utils.py` & `graphein-1.7.0/tests/testing/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,25 @@
     nodes_equal,
 )
 
 
 def test_graph_isomorphism():
     """Test that the graph isomorphism is working."""
     file_path = Path(__file__).parent.parent / "protein" / "test_data/4hhb.pdb"
-    G_1 = construct_graph(pdb_path=str(file_path))
-    G_2 = construct_graph(pdb_path=str(file_path))
+    G_1 = construct_graph(path=str(file_path))
+    G_2 = construct_graph(path=str(file_path))
     assert graphs_isomorphic(G_1, G_2), "Graphs are not isomorphic."
     assert graphs_equal(G_1, G_2), "Graphs are not equal."
     assert nodes_equal(G_1, G_2), "Graphs do not contain the same nodes."
     assert node_data_equal(G_1, G_2), "Node features differ."
     assert edges_equal(G_1, G_2), "Graphs do not contain the same edges."
     assert edge_data_equal(G_1, G_2), "Edge features differ."
 
     file_path = Path(__file__).parent.parent / "protein" / "test_data/1lds.pdb"
-    G_2 = construct_graph(pdb_path=str(file_path))
+    G_2 = construct_graph(path=str(file_path))
     assert not graphs_isomorphic(G_1, G_2), "Graphs not isomorphic."
     assert not graphs_equal(G_1, G_2), "Graphs are equal."
     assert not nodes_equal(G_1, G_2), "Graphs contain the same nodes."
     assert not node_data_equal(G_1, G_2), "Node features do not differ."
     assert not edges_equal(G_1, G_2), "Graphs contain the same edges."
     assert not edge_data_equal(G_1, G_2), "Edge features do not differ."
```

### Comparing `graphein-1.6.0/tests/utils/test_cli.py` & `graphein-1.7.0/tests/utils/test_cli.py`

 * *Files identical despite different names*

### Comparing `graphein-1.6.0/tests/utils/test_yml_parser.py` & `graphein-1.7.0/tests/utils/test_yml_parser.py`

 * *Files identical despite different names*

