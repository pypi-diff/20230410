# Comparing `tmp/deepchem-2.7.2.dev20230406001048.tar.gz` & `tmp/deepchem-2.7.2.dev20230410162347.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230406001048.tar", last modified: Thu Apr  6 00:10:48 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230410162347.tar", last modified: Mon Apr 10 16:23:47 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230406001048.tar` & `deepchem-2.7.2.dev20230410162347.tar`

### file list

```diff
@@ -1,285 +1,285 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.536834 deepchem-2.7.2.dev20230406001048/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-06 00:10:48.536834 deepchem-2.7.2.dev20230406001048/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.508833 deepchem-2.7.2.dev20230406001048/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.508833 deepchem-2.7.2.dev20230406001048/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67590 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.508833 deepchem-2.7.2.dev20230406001048/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.512833 deepchem-2.7.2.dev20230406001048/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.512833 deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.512833 deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.516833 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.516833 deepchem-2.7.2.dev20230406001048/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.516833 deepchem-2.7.2.dev20230406001048/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.516833 deepchem-2.7.2.dev20230406001048/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.516833 deepchem-2.7.2.dev20230406001048/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.516833 deepchem-2.7.2.dev20230406001048/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.520834 deepchem-2.7.2.dev20230406001048/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.520834 deepchem-2.7.2.dev20230406001048/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.520834 deepchem-2.7.2.dev20230406001048/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.520834 deepchem-2.7.2.dev20230406001048/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.520834 deepchem-2.7.2.dev20230406001048/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    36117 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.520834 deepchem-2.7.2.dev20230406001048/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.524834 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38371 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   109518 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.524834 deepchem-2.7.2.dev20230406001048/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.532834 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.532834 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.532834 deepchem-2.7.2.dev20230406001048/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.532834 deepchem-2.7.2.dev20230406001048/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.532834 deepchem-2.7.2.dev20230406001048/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.532834 deepchem-2.7.2.dev20230406001048/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.536834 deepchem-2.7.2.dev20230406001048/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.536834 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-06 00:10:38.000000 deepchem-2.7.2.dev20230406001048/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:10:48.508833 deepchem-2.7.2.dev20230406001048/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-06 00:10:48.000000 deepchem-2.7.2.dev20230406001048/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-06 00:10:48.000000 deepchem-2.7.2.dev20230406001048/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 00:10:48.000000 deepchem-2.7.2.dev20230406001048/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-06 00:10:48.000000 deepchem-2.7.2.dev20230406001048/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 00:10:48.000000 deepchem-2.7.2.dev20230406001048/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-06 00:10:48.540835 deepchem-2.7.2.dev20230406001048/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-06 00:10:39.000000 deepchem-2.7.2.dev20230406001048/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.678206 deepchem-2.7.2.dev20230410162347/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-04-10 16:23:37.000000 deepchem-2.7.2.dev20230410162347/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 16:23:47.678206 deepchem-2.7.2.dev20230410162347/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-10 16:23:37.000000 deepchem-2.7.2.dev20230410162347/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.642206 deepchem-2.7.2.dev20230410162347/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.642206 deepchem-2.7.2.dev20230410162347/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67590 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.646206 deepchem-2.7.2.dev20230410162347/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.646206 deepchem-2.7.2.dev20230410162347/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.646206 deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.650206 deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.650206 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.650206 deepchem-2.7.2.dev20230410162347/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.650206 deepchem-2.7.2.dev20230410162347/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.654206 deepchem-2.7.2.dev20230410162347/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.654206 deepchem-2.7.2.dev20230410162347/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.654206 deepchem-2.7.2.dev20230410162347/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.658206 deepchem-2.7.2.dev20230410162347/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.658206 deepchem-2.7.2.dev20230410162347/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.658206 deepchem-2.7.2.dev20230410162347/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.658206 deepchem-2.7.2.dev20230410162347/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.658206 deepchem-2.7.2.dev20230410162347/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36276 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.658206 deepchem-2.7.2.dev20230410162347/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.662206 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109518 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.662206 deepchem-2.7.2.dev20230410162347/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.670206 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.670206 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.670206 deepchem-2.7.2.dev20230410162347/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.674206 deepchem-2.7.2.dev20230410162347/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.674206 deepchem-2.7.2.dev20230410162347/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.674206 deepchem-2.7.2.dev20230410162347/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.678206 deepchem-2.7.2.dev20230410162347/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.678206 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:47.642206 deepchem-2.7.2.dev20230410162347/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 16:23:47.000000 deepchem-2.7.2.dev20230410162347/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-10 16:23:47.000000 deepchem-2.7.2.dev20230410162347/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:23:47.000000 deepchem-2.7.2.dev20230410162347/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-10 16:23:47.000000 deepchem-2.7.2.dev20230410162347/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 16:23:47.000000 deepchem-2.7.2.dev20230410162347/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-10 16:23:47.682206 deepchem-2.7.2.dev20230410162347/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-10 16:23:38.000000 deepchem-2.7.2.dev20230410162347/setup.py
```

### Comparing `deepchem-2.7.2.dev20230406001048/LICENSE` & `deepchem-2.7.2.dev20230410162347/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/PKG-INFO` & `deepchem-2.7.2.dev20230410162347/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230406001048
+Version: 2.7.2.dev20230410162347
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230406001048/README.md` & `deepchem-2.7.2.dev20230410162347/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230410162347/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230410162347/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230410162347/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230410162347/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230410162347/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230410162347/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Dict
+from typing import Dict, Optional
 from collections import Counter
 from rdkit import Chem
 from deepchem.data import Dataset
 from deepchem.feat.base_classes import Featurizer
 from deepchem.utils.typing import RDKitMol, RDKitAtom, RDKitBond
 from deepchem.feat.vocabulary_builders.vocabulary_builder import VocabularyBuilder
 
@@ -21,14 +21,23 @@
     it is connected to two carbon atoms by a single bond and 1 O atom by a double bond.
     The vocabulary of an atom is then computed as the `atom-symbol_contexts` where the contexts
     are sorted in alphabetical order when there are multiple contexts. For example, the
     vocabulary of second C is `C_C-SINGLE2_O-DOUBLE1`. The algorithm enumerates vocabulary of all atoms
     in the dataset and makes a vocabulary to index mapping by sorting the vocabulary
     by frequency and then alphabetically.
 
+    The algorithm enumerates vocabulary of all atoms in the dataset and makes a vocabulary to
+    index mapping by sorting the vocabulary by frequency and then alphabetically. The `max_size`
+    parameter can be used for setting the size of the vocabulary. When this parameter is set,
+    the algorithm stops adding new words to the index when the vocabulary size reaches `max_size`.
+
+    Parameters
+    ----------
+    max_size: int (optional)
+        Maximum size of vocabulary
 
     Example
     -------
     >>> import tempfile
     >>> import deepchem as dc
     >>> from rdkit import Chem
     >>> file = tempfile.NamedTemporaryFile()
@@ -44,18 +53,18 @@
     4
 
     Reference
     ---------
     .. Rong, Yu, et al. "Self-supervised graph transformer on large-scale molecular data." Advances in Neural Information Processing Systems 33 (2020): 12559-12571.
     """
 
-    def __init__(self):
+    def __init__(self, max_size: Optional[int] = None):
         self.specials = ('<pad>', '<other>')
         self.min_freq = 1
-        self.max_size = None
+        self.size = max_size
         self.itos = list(self.specials)
         self.stoi = self._make_reverse_mapping(self.itos)
         self.pad_index = 0
         self.other_index = 1
 
     def build(self, dataset: Dataset) -> None:
         """Builds vocabulary
@@ -73,26 +82,30 @@
                 v = self.atom_to_vocab(mol, atom)
                 counter[v] += 1
 
         # sort first by frequency, then alphabetically
         words_and_frequencies = sorted(counter.items(), key=lambda tup: tup[0])
         words_and_frequencies.sort(key=lambda tup: tup[1], reverse=True)
         for word, freq in words_and_frequencies:
+            if len(self.itos) == self.size:
+                break
             self.itos.append(word)
+        if self.size is None:
+            self.size = len(self.itos)
         self.stoi = self._make_reverse_mapping(self.itos)
 
     def save(self, fname: str) -> None:
         """Saves a vocabulary in json format
 
         Parameter
         ---------
         fname: str
             Filename to save vocabulary
         """
-        vocab = {'stoi': self.stoi, 'itos': self.itos}
+        vocab = {'stoi': self.stoi, 'itos': self.itos, 'size': self.size}
         with open(fname, 'w') as f:
             json.dump(vocab, f)
 
     @classmethod
     def load(cls, fname: str) -> 'GroverAtomVocabularyBuilder':
         """Loads vocabulary from the specified json file
 
@@ -105,15 +118,16 @@
         -------
         vocab: GroverAtomVocabularyBuilder
             A grover atom vocabulary builder which can be used for encoding
         """
         with open(fname, 'r') as f:
             data = json.load(f)
         vocab = cls()
-        vocab.stoi, vocab.itos = data['stoi'], data['itos']
+        vocab.stoi, vocab.itos, vocab.size = data['stoi'], data['itos'], data[
+            'size']
         return vocab
 
     @staticmethod
     def atom_to_vocab(mol: RDKitMol, atom: RDKitAtom) -> str:
         """Convert atom to vocabulary.
 
         Parameters
@@ -196,15 +210,23 @@
     has one bond with an O atom and one bond with a C atom. Consider the C=O double bond.
     The bond feature is DOUBLE-STEREONONE-NONE. The corresponding context is
     atomSymbol-bondFeature-Count. This gives us C-(DOUBLE-STEREONONE-NONE)1.
     Similary, it also has another bond with a C atom which gives the
     context C-(SINGLE-STEREONONE-NONE)1. Hence, the vocabulary of
     the bond is '(SINGLE-STEREONONE-NONE)_C-(DOUBLE-STEREONONE-NONE)1_C-(SINGLE-STEREONONE-NONE)1'
 
-    The algorithm enumerates vocabulary of all bonds in the dataset and makes a vocabulary to index mapping by sorting the vocabulary by frequency and then alphabetically.
+    The algorithm enumerates vocabulary of all bonds in the dataset and makes a vocabulary to
+    index mapping by sorting the vocabulary by frequency and then alphabetically. The `max_size`
+    parameter can be used for setting the size of the vocabulary. When this parameter is set,
+    the algorithm stops adding new words to the index when the vocabulary size reaches `max_size`.
+
+    Parameters
+    ----------
+    max_size: int (optional)
+        Maximum size of vocabulary
 
     Example
     -------
     >>> import tempfile
     >>> import deepchem as dc
     >>> from rdkit import Chem
     >>> file = tempfile.NamedTemporaryFile()
@@ -221,18 +243,18 @@
 
     Reference
     ---------
     .. Rong, Yu, et al. "Self-supervised graph transformer on large-scale molecular data." Advances in Neural Information Processing Systems 33 (2020): 12559-12571.
     """
     BOND_FEATURES = ['BondType', 'Stereo', 'BondDir']
 
-    def __init__(self):
+    def __init__(self, max_size: Optional[int] = None):
         self.specials = ('<pad>', '<other>')
         self.min_freq = 1
-        self.max_size = None
+        self.size = max_size
         self.itos = list(self.specials)
         self.stoi = self._make_reverse_mapping(self.itos)
         self.pad_index = 0
         self.other_index = 1
 
     def build(self, dataset: Dataset) -> None:
         """Builds vocabulary
@@ -250,26 +272,30 @@
                 v = self.bond_to_vocab(mol, bond)
                 counter[v] += 1
 
         # sort first by frequency, then alphabetically
         words_and_frequencies = sorted(counter.items(), key=lambda tup: tup[0])
         words_and_frequencies.sort(key=lambda tup: tup[1], reverse=True)
         for word, freq in words_and_frequencies:
+            if len(self.itos) == self.size:
+                break
             self.itos.append(word)
+        if self.size is None:
+            self.size = len(self.itos)
         self.stoi = self._make_reverse_mapping(self.itos)
 
     def save(self, fname: str) -> None:
         """Saves a vocabulary in json format
 
         Parameter
         ---------
         fname: str
             Filename to save vocabulary
         """
-        vocab = {'stoi': self.stoi, 'itos': self.itos}
+        vocab = {'stoi': self.stoi, 'itos': self.itos, 'size': self.size}
         with open(fname, 'w') as f:
             json.dump(vocab, f)
 
     @classmethod
     def load(cls, fname: str) -> 'GroverBondVocabularyBuilder':
         """Loads vocabulary from the specified json file
 
@@ -282,15 +308,16 @@
         -------
         vocab: GroverAtomVocabularyBuilder
             A grover atom vocabulary builder which can be used for encoding
         """
         with open(fname, 'r') as f:
             data = json.load(f)
         vocab = cls()
-        vocab.stoi, vocab.itos = data['stoi'], data['itos']
+        vocab.stoi, vocab.itos, vocab.size = data['stoi'], data['itos'], data[
+            'size']
         return vocab
 
     @staticmethod
     def bond_to_vocab(mol: RDKitMol, bond: RDKitBond):
         """Convert bond to vocabulary.
 
         The algorithm considers only one-hop neighbor atoms.
```

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230410162347/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230410162347/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230410162347/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230410162347/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230410162347/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230410162347/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230410162347/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230410162347/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230410162347/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -844,15 +844,15 @@
             atom_vocab_task_target: torch.Tensor
                 Targets for atom vocabulary prediction
             bond_vocab_task_target: torch.Tensor
                 Targets for bond vocabulary prediction
             fg_task_target: torch.Tensor
                 Targets for functional groups
             dist_coff: float, default 0.1
-                loss metric
+                Loss term weight for weighting closeness between embedding generated from atom hidden state and bond hidden state in atom vocabulary and bond vocabulary prediction tasks.
 
             Returns
             -------
             loss: torch.Tensor
                 loss value
             """
             av_task_loss = nn.NLLLoss(reduction="mean")  # same for av and bv
@@ -860,17 +860,17 @@
             av_task_dist_loss = nn.MSELoss(reduction="mean")
             fg_task_dist_loss = nn.MSELoss(reduction="mean")
 
             sigmoid = nn.Sigmoid()
 
             av_atom_loss = av_task_loss(atom_vocab_task_atom_pred,
                                         atom_vocab_task_target)
-            av_bond_loss = av_task_loss(bond_vocab_task_atom_pred,
+            av_bond_loss = av_task_loss(atom_vocab_task_bond_pred,
                                         atom_vocab_task_target)
-            bv_atom_loss = av_task_loss(atom_vocab_task_bond_pred,
+            bv_atom_loss = av_task_loss(bond_vocab_task_atom_pred,
                                         bond_vocab_task_target)
             bv_bond_loss = av_task_loss(bond_vocab_task_bond_pred,
                                         bond_vocab_task_target)
 
             fg_atom_from_atom_loss = fg_task_loss(fg_task_atom_from_atom,
                                                   fg_task_target)
             fg_atom_from_bond_loss = fg_task_loss(fg_task_atom_from_bond,
```

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/models.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from deepchem.models.torch_models.pagtn import Pagtn, PagtnModel
 from deepchem.models.torch_models.mat import MAT, MATModel
 from deepchem.models.torch_models.megnet import MEGNetModel
 from deepchem.models.torch_models.normalizing_flows_pytorch import NormalizingFlow
 from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList
 from deepchem.models.torch_models.cnn import CNN
 from deepchem.models.torch_models.attention import ScaledDotProductAttention, SelfAttention
+from deepchem.models.torch_models.grover import GroverModel, GroverPretrain, GroverFinetune
 from deepchem.models.torch_models.readout import GroverReadout
 try:
     from deepchem.models.torch_models.dmpnn import DMPNN, DMPNNModel
 except ModuleNotFoundError as e:
     logger.warning(
         f'Skipped loading modules with pytorch-geometric dependency, missing a dependency. {e}'
     )
```

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/grover_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         embedding: Dict[str, torch.Tensor]
             Returns a dictionary of embeddings. The embeddings are:
          - atom_from_atom: node messages aggregated from node hidden states
          - bond_from_atom: bond messages aggregated from bond hidden states
          - atom_from_bond: node message aggregated from bond hidden states
          - bond_from_bond: bond messages aggregated from bond hidden states.
         """
+        # TODO Explain in detail what the four outcompes are
         output = self.encoders(graph_batch)
         return {
             "atom_from_atom": output[0][0],
             "bond_from_atom": output[0][1],
             "atom_from_bond": output[1][0],
             "bond_from_bond": output[1][1]
         }
@@ -132,17 +133,17 @@
 
         Returns
         -------
         logits: torch.Tensor
             the prediction for each bond, (num_bond, vocab_size)
         """
         nm_bonds = embeddings.shape[0]
-        # The bond and rev bond have odd and even ids respectively.
-        ids1 = list(range(1, nm_bonds, 2))
-        ids2 = list(range(0, nm_bonds, 2))
+        # The bond and rev bond have even and odd ids respectively.
+        ids1 = list(range(0, nm_bonds, 2))
+        ids2 = list(range(1, nm_bonds, 2))
         logits = self.linear(embeddings[ids1]) + self.linear_rev(
             embeddings[ids2])
         return self.logsoftmax(logits)
 
 
 class GroverAtomVocabPredictor(nn.Module):
     """Grover Atom Vocabulary Prediction Module.
```

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/modular.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         components: dict
             A dictionary of the components of the model. The keys are the names of the
             components and the values are the components themselves.
         """
 
         self.model = model
         self.components = components
+        # FIXME self.loss_func is an incorrect argument for TorchModel.loss because
+        # it performs more than computing loss
         super().__init__(self.model, self.loss_func, **kwargs)
         self.model.to(self.device)
         self.components = {
             k: v.to(self.device) for k, v in self.components.items()
         }
 
     def build_model(self) -> nn.Module:
@@ -182,14 +184,15 @@
         if not isinstance(callbacks, SequenceCollection):
             callbacks = [callbacks]
         self._ensure_built()
         self.model.train()
         avg_loss = 0.0
         last_avg_loss = 0.0
         averaged_batches = 0
+        # FIXME This line is not needed as loss is computed inside the call to loss_func
         if loss is None:
             loss = self._loss_fn
         if variables is None:
             optimizer = self._pytorch_optimizer
             lr_schedule = self._lr_schedule
         else:
             var_key = tuple(variables)
@@ -306,15 +309,15 @@
             self.model(inputs)
 
         self._ensure_built()
 
         if source_model is not None:
             for name, module in source_model.components.items():
                 if components is None or name in components:
-                    self.components[name] = module
+                    self.components[name].load_state_dict(module.state_dict())
             self.build_model()
 
         elif source_model is None:
             self.restore(components=components,
                          checkpoint=checkpoint,
                          model_dir=model_dir)
```

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/readout.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     embeddings. The generate embedding can be used in downstream tasks like graph
     classification or graph prediction problems.
 
     Parameters
     ----------
     rtype: str
         Readout type, can be 'mean' or 'self-attention'
-    hidden_size: int
-        Input layer hidden size
+    in_features: int
+        Size fof input features
     attn_hidden_size: int
         If readout type is attention, size of hidden layer in attention network.
     attn_out_size: int
         If readout type is attention, size of attention out layer.
 
     Example
     -------
```

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230410162347/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230410162347/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230410162347/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230410162347/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230410162347/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230410162347/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230410162347/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230410162347/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230410162347/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230410162347/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230410162347/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230410162347/deepchem.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230406001048
+Version: 2.7.2.dev20230410162347
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230406001048/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230410162347/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/setup.cfg` & `deepchem-2.7.2.dev20230410162347/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230406001048/setup.py` & `deepchem-2.7.2.dev20230410162347/setup.py`

 * *Files identical despite different names*

