# Comparing `tmp/molfeat-0.8.5.tar.gz` & `tmp/molfeat-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molfeat-0.8.5.tar", last modified: Fri Apr  7 16:48:05 2023, max compression
+gzip compressed data, was "molfeat-0.8.6.tar", last modified: Mon Apr 10 17:36:02 2023, max compression
```

## Comparing `molfeat-0.8.5.tar` & `molfeat-0.8.6.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.993735 molfeat-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-07 16:46:34.000000 molfeat-0.8.5/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.973734 molfeat-0.8.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.977734 molfeat-0.8.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/ISSUE_TEMPLATE/1_bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/ISSUE_TEMPLATE/2_refactor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/ISSUE_TEMPLATE/3_documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.977734 molfeat-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-07 16:46:34.000000 molfeat-0.8.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-07 16:46:34.000000 molfeat-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-07 16:46:34.000000 molfeat-0.8.5/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-07 16:46:34.000000 molfeat-0.8.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-07 16:46:34.000000 molfeat-0.8.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-07 16:46:34.000000 molfeat-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-07 16:48:05.993735 molfeat-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-07 16:46:34.000000 molfeat-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.977734 molfeat-0.8.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.977734 molfeat-0.8.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.calc.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.store.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.trans.base.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.trans.concat.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.trans.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.trans.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.trans.pretrained.fcd.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.trans.pretrained.graphormer.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.trans.pretrained.hf_transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.trans.struct.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/api/molfeat.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.969734 molfeat-0.8.5/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.977734 molfeat-0.8.5/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/assets/css/custom-molfeat.css
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.977734 molfeat-0.8.5/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/benchmark.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.981735 molfeat-0.8.5/docs/developers/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/developers/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/developers/create-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/developers/register-plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.981735 molfeat-0.8.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.981735 molfeat-0.8.5/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/tutorials/add_your_own.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/tutorials/datacache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/tutorials/graphs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/tutorials/integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/tutorials/pyg_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/tutorials/save_and_load.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/tutorials/transformer_finetuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/tutorials/types_of_featurizers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-07 16:46:34.000000 molfeat-0.8.5/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-07 16:46:34.000000 molfeat-0.8.5/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-07 16:46:34.000000 molfeat-0.8.5/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.981735 molfeat-0.8.5/molfeat/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.985735 molfeat-0.8.5/molfeat/calc/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/_atom_bond_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/_map4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/_mhfp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/cats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    22488 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/skeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/calc/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.985735 molfeat-0.8.5/molfeat/data/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/data/cats_features.fdef
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/data/elements.xz
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/data/elements_completed.xz
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/data/origin.xz
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/data/skey_parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.985735 molfeat-0.8.5/molfeat/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/plugins/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/plugins/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/plugins/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.985735 molfeat-0.8.5/molfeat/store/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/store/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/store/modelcard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/store/modelstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.985735 molfeat-0.8.5/molfeat/trans/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33035 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.985735 molfeat-0.8.5/molfeat/trans/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27395 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/graph/adj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.989735 molfeat-0.8.5/molfeat/trans/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/pretrained/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/pretrained/dgl_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/pretrained/fcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/pretrained/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/pretrained/hf_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.989735 molfeat-0.8.5/molfeat/trans/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/struct/esm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/trans/struct/prot1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.989735 molfeat-0.8.5/molfeat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25556 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/utils/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-07 16:46:34.000000 molfeat-0.8.5/molfeat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.981735 molfeat-0.8.5/molfeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-07 16:48:05.000000 molfeat-0.8.5/molfeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-07 16:48:05.000000 molfeat-0.8.5/molfeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:48:05.000000 molfeat-0.8.5/molfeat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:47:54.000000 molfeat-0.8.5/molfeat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-07 16:48:05.000000 molfeat-0.8.5/molfeat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 16:48:05.000000 molfeat-0.8.5/molfeat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.989735 molfeat-0.8.5/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-07 16:46:34.000000 molfeat-0.8.5/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-07 16:46:34.000000 molfeat-0.8.5/plugin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-07 16:46:34.000000 molfeat-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-07 16:46:34.000000 molfeat-0.8.5/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:48:05.993735 molfeat-0.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:48:05.993735 molfeat-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_atom_bond_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_prot_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-07 16:46:34.000000 molfeat-0.8.5/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-10 17:34:46.000000 molfeat-0.8.6/.authors.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/1_bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/2_refactor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/3_documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-10 17:34:46.000000 molfeat-0.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-10 17:34:46.000000 molfeat-0.8.6/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-10 17:34:46.000000 molfeat-0.8.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-10 17:34:46.000000 molfeat-0.8.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-10 17:34:46.000000 molfeat-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-10 17:36:02.965476 molfeat-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-10 17:34:46.000000 molfeat-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.calc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.store.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.concat.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.pretrained.fcd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.pretrained.graphormer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.pretrained.hf_transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.struct.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.949476 molfeat-0.8.6/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/assets/css/custom-molfeat.css
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/benchmark.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/developers/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/developers/create-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/developers/register-plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/add_your_own.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/datacache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/graphs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/pyg_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/save_and_load.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/transformer_finetuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/types_of_featurizers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-10 17:34:46.000000 molfeat-0.8.6/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-10 17:34:46.000000 molfeat-0.8.6/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/molfeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/_atom_bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/_map4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/_mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/cats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22488 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/skeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/cats_features.fdef
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/elements.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/elements_completed.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/origin.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/skey_parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/plugins/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/plugins/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/plugins/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/store/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/store/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/store/modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/store/modelstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33689 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/trans/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27395 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/graph/adj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/trans/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/dgl_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/fcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/hf_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/molfeat/trans/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/struct/esm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/struct/prot1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/molfeat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25556 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/molfeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:35:52.000000 molfeat-0.8.6/molfeat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-10 17:34:46.000000 molfeat-0.8.6/news/TEMPLATE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-10 17:34:46.000000 molfeat-0.8.6/plugin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-10 17:34:46.000000 molfeat-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-10 17:34:46.000000 molfeat-0.8.6/rever.xsh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:36:02.965476 molfeat-0.8.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_atom_bond_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_prot_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_viz.py
```

### Comparing `molfeat-0.8.5/.authors.yml` & `molfeat-0.8.6/.authors.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 - name: maclandrol
   email: emmanuel.noutahi@hotmail.ca
-  num_commits: 29
+  num_commits: 34
   first_commit: 2021-04-06 11:53:10
 - name: Cas Wognum
   email: caswognum@outlook.com
   aliases:
   - cwognum
-  num_commits: 28
+  num_commits: 30
   first_commit: 2023-03-20 13:05:13
 - name: Hadrien Mary
   email: hadrien.mary@gmail.com
   alternate_emails:
   - hadim@users.noreply.github.com
   num_commits: 23
   first_commit: 2023-03-21 12:50:42
```

### Comparing `molfeat-0.8.5/.github/CODE_OF_CONDUCT.md` & `molfeat-0.8.6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.github/ISSUE_TEMPLATE/1_bug_report.yaml` & `molfeat-0.8.6/.github/ISSUE_TEMPLATE/1_bug_report.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.github/ISSUE_TEMPLATE/2_refactor.yaml` & `molfeat-0.8.6/.github/ISSUE_TEMPLATE/2_refactor.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.github/ISSUE_TEMPLATE/3_documentation.yaml` & `molfeat-0.8.6/.github/ISSUE_TEMPLATE/3_documentation.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml` & `molfeat-0.8.6/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.github/ISSUE_TEMPLATE/config.yml` & `molfeat-0.8.6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.github/workflows/doc.yml` & `molfeat-0.8.6/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.github/workflows/release.yml` & `molfeat-0.8.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.github/workflows/test.yml` & `molfeat-0.8.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.gitignore` & `molfeat-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/.mailmap` & `molfeat-0.8.6/.mailmap`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/CHANGELOG.rst` & `molfeat-0.8.6/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 ==================
 molfeat Change Log
 ==================
 
 .. current developments
 
+v0.8.6
+====================
+
+**Added:**
+
+* Support for batch transformation in `MoleculeTransformer` for calculators that implements `batch_compute`
+
+**Changed:**
+
+* Pull request template for better directive.
+
+**Authors:**
+
+* maclandrol
+
+
+
 v0.8.5
 ====================
 
 **Authors:**
```

### Comparing `molfeat-0.8.5/LICENSE` & `molfeat-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/PKG-INFO` & `molfeat-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.5
+Version: 0.8.6
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -53,15 +53,15 @@
 
 [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/latestdoi/613548667)
 [![PyPI](https://img.shields.io/pypi/v/molfeat)](https://pypi.org/project/molfeat/)
 [![Conda](https://img.shields.io/conda/v/conda-forge/molfeat?label=conda&color=success)](https://anaconda.org/conda-forge/molfeat)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/molfeat)](https://pypi.org/project/molfeat/)
 [![Conda](https://img.shields.io/conda/dn/conda-forge/molfeat)](https://anaconda.org/conda-forge/molfeat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/molfeat)](https://pypi.org/project/molfeat/)
-[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/datamol/blob/main/LICENSE)
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/molfeat/blob/main/LICENSE)
 [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/molfeat)](https://github.com/datamol-io/molfeat/stargazers)
 [![GitHub Repo stars](https://img.shields.io/github/forks/datamol-io/molfeat)](https://github.com/datamol-io/molfeat/network/members)
 [![test](https://github.com/datamol-io/molfeat/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/test.yml)
 [![code-check](https://github.com/datamol-io/molfeat/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/molfeat/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/doc.yml)
 [![release](https://github.com/datamol-io/molfeat/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/release.yml)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.5 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.6 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -26,15 +26,15 @@
 pypi.org/project/molfeat/) [![Conda](https://img.shields.io/conda/v/conda-
 forge/molfeat?label=conda&color=success)](https://anaconda.org/conda-forge/
 molfeat) [![PyPI - Downloads](https://img.shields.io/pypi/dm/molfeat)](https://
 pypi.org/project/molfeat/) [![Conda](https://img.shields.io/conda/dn/conda-
 forge/molfeat)](https://anaconda.org/conda-forge/molfeat) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/molfeat)](https://pypi.org/
 project/molfeat/) [![license](https://img.shields.io/badge/License-
-Apache%202.0-blue.svg)](https://github.com/datamol-io/datamol/blob/main/
+Apache%202.0-blue.svg)](https://github.com/datamol-io/molfeat/blob/main/
 LICENSE) [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/
 molfeat)](https://github.com/datamol-io/molfeat/stargazers) [![GitHub Repo
 stars](https://img.shields.io/github/forks/datamol-io/molfeat)](https://
 github.com/datamol-io/molfeat/network/members) [![test](https://github.com/
 datamol-io/molfeat/actions/workflows/test.yml/badge.svg)](https://github.com/
 datamol-io/molfeat/actions/workflows/test.yml) [![code-check](https://
 github.com/datamol-io/molfeat/actions/workflows/code-check.yml/badge.svg)]
```

### Comparing `molfeat-0.8.5/README.md` & `molfeat-0.8.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/latestdoi/613548667)
 [![PyPI](https://img.shields.io/pypi/v/molfeat)](https://pypi.org/project/molfeat/)
 [![Conda](https://img.shields.io/conda/v/conda-forge/molfeat?label=conda&color=success)](https://anaconda.org/conda-forge/molfeat)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/molfeat)](https://pypi.org/project/molfeat/)
 [![Conda](https://img.shields.io/conda/dn/conda-forge/molfeat)](https://anaconda.org/conda-forge/molfeat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/molfeat)](https://pypi.org/project/molfeat/)
-[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/datamol/blob/main/LICENSE)
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/molfeat/blob/main/LICENSE)
 [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/molfeat)](https://github.com/datamol-io/molfeat/stargazers)
 [![GitHub Repo stars](https://img.shields.io/github/forks/datamol-io/molfeat)](https://github.com/datamol-io/molfeat/network/members)
 [![test](https://github.com/datamol-io/molfeat/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/test.yml)
 [![code-check](https://github.com/datamol-io/molfeat/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/molfeat/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/doc.yml)
 [![release](https://github.com/datamol-io/molfeat/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/release.yml)
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 pypi.org/project/molfeat/) [![Conda](https://img.shields.io/conda/v/conda-
 forge/molfeat?label=conda&color=success)](https://anaconda.org/conda-forge/
 molfeat) [![PyPI - Downloads](https://img.shields.io/pypi/dm/molfeat)](https://
 pypi.org/project/molfeat/) [![Conda](https://img.shields.io/conda/dn/conda-
 forge/molfeat)](https://anaconda.org/conda-forge/molfeat) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/molfeat)](https://pypi.org/
 project/molfeat/) [![license](https://img.shields.io/badge/License-
-Apache%202.0-blue.svg)](https://github.com/datamol-io/datamol/blob/main/
+Apache%202.0-blue.svg)](https://github.com/datamol-io/molfeat/blob/main/
 LICENSE) [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/
 molfeat)](https://github.com/datamol-io/molfeat/stargazers) [![GitHub Repo
 stars](https://img.shields.io/github/forks/datamol-io/molfeat)](https://
 github.com/datamol-io/molfeat/network/members) [![test](https://github.com/
 datamol-io/molfeat/actions/workflows/test.yml/badge.svg)](https://github.com/
 datamol-io/molfeat/actions/workflows/test.yml) [![code-check](https://
 github.com/datamol-io/molfeat/actions/workflows/code-check.yml/badge.svg)]
```

### Comparing `molfeat-0.8.5/docs/assets/css/custom-molfeat.css` & `molfeat-0.8.6/docs/assets/css/custom-molfeat.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/assets/css/custom.css` & `molfeat-0.8.6/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/benchmark.ipynb` & `molfeat-0.8.6/docs/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/developers/contribute.md` & `molfeat-0.8.6/docs/developers/contribute.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/developers/create-plugin.md` & `molfeat-0.8.6/docs/developers/create-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/developers/register-plugin.md` & `molfeat-0.8.6/docs/developers/register-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/images/logo-black.png` & `molfeat-0.8.6/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/images/logo-black.svg` & `molfeat-0.8.6/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/images/logo-title.svg` & `molfeat-0.8.6/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/images/logo.png` & `molfeat-0.8.6/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/images/logo.svg` & `molfeat-0.8.6/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/index.md` & `molfeat-0.8.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/tutorials/add_your_own.ipynb` & `molfeat-0.8.6/docs/tutorials/add_your_own.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9774450547112541%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'data': {'text/plain': ['[array([13.        , 13.        ,  "*

 * *            "3.        ,  0.63696169]),\\n', ' array([5.        , 4.        , 4.        , "*

 * *            "0.63696169]),\\n', ' array([5.        , 4.        , 0.        , 0.63696169])]']}}}, "*

 * *            '\'source\': {insert: [(6, \'smiles = dm.freesolv()["smiles"].iloc[:3]\\n\'), (15, '*

 * *            "'mol_transf(smiles)')], delete: [14]}}, 4: {'outputs': {0: {'data': {'text/plain': "*

 * *            "['[array([13.     […]*

```diff
@@ -30,38 +30,41 @@
             "metadata": {
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[array([14.        , 15.        ,  6.        ,  0.63696169])]"
+                            "[array([13.        , 13.        ,  3.        ,  0.63696169]),\n",
+                            " array([5.        , 4.        , 4.        , 0.63696169]),\n",
+                            " array([5.        , 4.        , 0.        , 0.63696169])]"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "import datamol as dm\n",
                 "\n",
                 "from molfeat.trans import MoleculeTransformer\n",
                 "from rdkit.Chem.rdMolDescriptors import CalcNumHeteroatoms\n",
                 "\n",
+                "smiles = dm.freesolv()[\"smiles\"].iloc[:3]\n",
                 "def my_calculator(mol):\n",
                 "    \"\"\"My custom featurizer\"\"\"\n",
                 "    mol = dm.to_mol(mol)\n",
                 "    rng = np.random.default_rng(0)\n",
                 "    return [mol.GetNumAtoms(), mol.GetNumBonds(), CalcNumHeteroatoms(mol), rng.random()]\n",
                 "\n",
                 "# This directly works with the MoleculeTransformer\n",
                 "mol_transf = MoleculeTransformer(my_calculator)\n",
-                "mol_transf([\"CN1C=NC2=C1C(=O)N(C(=O)N2C)C\"])"
+                "mol_transf(smiles)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
@@ -77,15 +80,17 @@
             "metadata": {
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[array([14.        , 15.        ,  6.        ,  0.63696169])]"
+                            "[array([13.        , 13.        ,  3.        ,  0.63696169]),\n",
+                            " array([5.        , 4.        , 4.        , 0.63696169]),\n",
+                            " array([5.        , 4.        , 0.        , 0.63696169])]"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -97,15 +102,76 @@
                 "    def __call__(self, mol):\n",
                 "        mol = dm.to_mol(mol)\n",
                 "        rng = np.random.default_rng(0)\n",
                 "        return [mol.GetNumAtoms(), mol.GetNumBonds(), CalcNumHeteroatoms(mol), rng.random()]\n",
                 "\n",
                 "\n",
                 "mol_transf = MoleculeTransformer(MyCalculator())\n",
-                "mol_transf([\"CN1C=NC2=C1C(=O)N(C(=O)N2C)C\"])"
+                "mol_transf(smiles)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "If your calculator can perform featurization of a batch of molecules in an efficient way, then you should implement the optional `batch_compute` method which will then be used by `MoleculeTransformer` instead of the default sequential or parallelization process. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "We are in batch mode!\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([[0.77395605, 0.43887844, 0.85859792, 0.69736803, 0.09417735,\n",
+                            "        0.97562235, 0.7611397 , 0.78606431, 0.12811363, 0.45038594],\n",
+                            "       [0.37079802, 0.92676499, 0.64386512, 0.82276161, 0.4434142 ,\n",
+                            "        0.22723872, 0.55458479, 0.06381726, 0.82763117, 0.6316644 ],\n",
+                            "       [0.75808774, 0.35452597, 0.97069802, 0.89312112, 0.7783835 ,\n",
+                            "        0.19463871, 0.466721  , 0.04380377, 0.15428949, 0.68304895]])"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "from molfeat.calc import SerializableCalculator\n",
+                "\n",
+                "class MyBatchableCalculator(SerializableCalculator):\n",
+                "    def __init__(self, random_seed=42, length=10):\n",
+                "        self.random_seed = random_seed\n",
+                "        self.length = length\n",
+                "        self.rng = np.random.default_rng(self.random_seed)\n",
+                "\n",
+                "    def __call__(self, mol):\n",
+                "        print(\"We are in single compute mode!\")\n",
+                "        return self.rng.random(self.length)\n",
+                "    \n",
+                "    def __len__(self):\n",
+                "        return self.length\n",
+                "        \n",
+                "    def batch_compute(self, mols, **kwargs):\n",
+                "        # note that dm.parallelized information is passed along with the molecules list\n",
+                "        print(\"We are in batch mode!\")\n",
+                "        return self.rng.random((len(mols), self.length))\n",
+                "\n",
+                "mol_transf = MoleculeTransformer(MyBatchableCalculator())\n",
+                "mol_transf(smiles)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
@@ -114,15 +180,15 @@
                 "## Define your own transformer\n",
                 "The above example shows that in many cases, there's no direct need to create your own transformer class. You can simply use the `MoleculeTransformer` base class.\n",
                 "In more complex cases, such as with pretrained models where batching would be advantageous, it is instead preferable to create your own subclass. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from sklearn.ensemble import RandomForestRegressor\n",
                 "from molfeat.trans.pretrained import PretrainedMolTransformer\n",
@@ -160,26 +226,26 @@
                 "        In this dummy example, we simply multiply the features by the importance of the feature\n",
                 "        \"\"\"\n",
                 "        return [feats * self._model.feature_importances_ for feats in mols]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(1, 167)"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "mol_transf = MyFoundationModel()\n",
                 "mol_transf([\"CN1C=NC2=C1C(=O)N(C(=O)N2C)C\"]).shape"
@@ -195,24 +261,24 @@
                 "```bash\n",
                 "pip install astrochem_embedding\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "torch.Size([10, 32])"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import torch\n",
                 "import datamol as dm\n",
@@ -246,26 +312,26 @@
                 "## Add it to your Model Store\n",
                 "Molfeat has a Model Store to publish your models in a centralized location.\n",
                 "The default is a read-only GCP bucket but you can replace this with your own file storage. This can, for example, be useful to share private featurizers with your team."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "0"
+                            "1"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import platformdirs\n",
                 "from molfeat.store.modelstore import ModelStore\n",
@@ -274,47 +340,47 @@
                 "path = dm.fs.join(platformdirs.user_cache_dir(\"molfeat\"), \"custom_model_store\")\n",
                 "store = ModelStore(model_store_bucket=path)\n",
                 "len(store.available_models)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "b5568f0732774c3fa9955550c4365af8",
+                            "model_id": "805c88dfabe241bdb8d04325fca22448",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0.00/4.00 [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2023-04-01 15:10:14.556 | INFO     | molfeat.store.modelstore:register:124 - Successfuly registered model my_foundation_model !\n"
+                        "2023-04-07 18:59:03.363 | INFO     | molfeat.store.modelstore:register:124 - Successfuly registered model my_foundation_model !\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "[ModelInfo(name='my_foundation_model', inputs='smiles', type='pretrained', version=0, group='my_group', submitter='Datamol', description='Solves chemistry!', representation='vector', require_3D=False, tags=['foundation_model', 'random_forest'], authors=['Datamol'], reference='/fake/ref', created_at=datetime.datetime(2023, 4, 1, 15, 10, 14, 527157), sha256sum='9c298d589a2158eb513cb52191144518a2acab2cb0c04f1df14fca0f712fa4a1')]"
+                            "[ModelInfo(name='my_foundation_model', inputs='smiles', type='pretrained', version=0, group='my_group', submitter='Datamol', description='Solves chemistry!', representation='vector', require_3D=False, tags=['foundation_model', 'random_forest'], authors=['Datamol'], reference='/fake/ref', created_at=datetime.datetime(2023, 4, 7, 18, 59, 3, 312234), sha256sum='9c298d589a2158eb513cb52191144518a2acab2cb0c04f1df14fca0f712fa4a1')]"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Let's define our model's info\n",
                 "info = ModelInfo(\n",
@@ -361,13 +427,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 0
 }
```

### Comparing `molfeat-0.8.5/docs/tutorials/datacache.ipynb` & `molfeat-0.8.6/docs/tutorials/datacache.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/tutorials/graphs.ipynb` & `molfeat-0.8.6/docs/tutorials/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/tutorials/integrations.ipynb` & `molfeat-0.8.6/docs/tutorials/integrations.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/tutorials/pyg_integration.ipynb` & `molfeat-0.8.6/docs/tutorials/pyg_integration.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/tutorials/save_and_load.ipynb` & `molfeat-0.8.6/docs/tutorials/save_and_load.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/tutorials/transformer_finetuning.ipynb` & `molfeat-0.8.6/docs/tutorials/transformer_finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/tutorials/types_of_featurizers.ipynb` & `molfeat-0.8.6/docs/tutorials/types_of_featurizers.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/docs/usage.md` & `molfeat-0.8.6/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/env.yml` & `molfeat-0.8.6/env.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/mkdocs.yml` & `molfeat-0.8.6/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
   - markdown_include.include
   - pymdownx.emoji
   - pymdownx.highlight
   - pymdownx.magiclink
   - pymdownx.superfences
   - pymdownx.tabbed
   - pymdownx.tasklist
+  - pymdownx.details
   # For `tab_length=2` in the markdown extension
   # See https://github.com/mkdocs/mkdocs/issues/545
   - mdx_truly_sane_lists
   - toc:
       permalink: true
 
 plugins:
```

### Comparing `molfeat-0.8.5/molfeat/calc/__init__.py` & `molfeat-0.8.6/molfeat/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/_atom_bond_features.py` & `molfeat-0.8.6/molfeat/calc/_atom_bond_features.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/_map4.py` & `molfeat-0.8.6/molfeat/calc/_map4.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/_mhfp.py` & `molfeat-0.8.6/molfeat/calc/_mhfp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/atom.py` & `molfeat-0.8.6/molfeat/calc/atom.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/base.py` & `molfeat-0.8.6/molfeat/calc/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,15 +26,48 @@
             )
         if name != "SerializableCalculator":
             # do not register the base class
             _CALCULATORS[name] = cls
 
 
 class SerializableCalculator(abc.ABC, metaclass=_CalculatorMeta):
-    """Interface to define a serializable calculator"""
+    """Interface to define a serializable calculator
+
+    ???+ tip "Subclassing SerializableCalculator"
+        When subclassing a calculator, you must implement the __call__ method.
+        If your calculator also implements a `batch_compute` method, it will be used
+        by `MoleculeTransformer` to accelerate featurization.
+
+        ```python
+        from molfeat.calc import SerializableCalculator
+
+        class MyCalculator(SerializableCalculator):
+
+            def __call__(self, mol, **kwargs):
+                # you have to implement this
+                ...
+
+            def __len__(self):
+                # you don't have to implement this but are encouraged to do so
+                # this is used to determine the length of the output
+                ...
+
+            @property
+            def columns(self):
+                # you don't have to implement this
+                # use this to return the name of each entry returned by your featurizer
+                ...
+
+            def batch_compute(self, mols:list, **dm_parallelized_kwargs):
+                # you don't need to implement this
+                # but you should if there is an efficient batching process
+                # By default dm.parallelized arguments will also be passed as input
+                ...
+        ```
+    """
 
     @abc.abstractmethod
     def __call__(self, *args, **kwargs):
         pass
 
     @classmethod
     def from_state_dict(cls, state: dict, override_args: Optional[dict] = None):
```

### Comparing `molfeat-0.8.5/molfeat/calc/bond.py` & `molfeat-0.8.6/molfeat/calc/bond.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/cats.py` & `molfeat-0.8.6/molfeat/calc/cats.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/descriptors.py` & `molfeat-0.8.6/molfeat/calc/descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/fingerprints.py` & `molfeat-0.8.6/molfeat/calc/fingerprints.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/pharmacophore.py` & `molfeat-0.8.6/molfeat/calc/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/shape.py` & `molfeat-0.8.6/molfeat/calc/shape.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/skeys.py` & `molfeat-0.8.6/molfeat/calc/skeys.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/calc/tree.py` & `molfeat-0.8.6/molfeat/calc/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/data/cats_features.fdef` & `molfeat-0.8.6/molfeat/data/cats_features.fdef`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/data/elements.xz` & `molfeat-0.8.6/molfeat/data/elements.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/data/elements_completed.xz` & `molfeat-0.8.6/molfeat/data/elements_completed.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/data/origin.xz` & `molfeat-0.8.6/molfeat/data/origin.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/data/skey_parameters.csv` & `molfeat-0.8.6/molfeat/data/skey_parameters.csv`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/plugins/entry_point.py` & `molfeat-0.8.6/molfeat/plugins/entry_point.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/plugins/factories.py` & `molfeat-0.8.6/molfeat/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/store/loader.py` & `molfeat-0.8.6/molfeat/store/loader.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/store/modelcard.py` & `molfeat-0.8.6/molfeat/store/modelcard.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/store/modelstore.py` & `molfeat-0.8.6/molfeat/store/modelstore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/base.py` & `molfeat-0.8.6/molfeat/trans/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,18 @@
     Base class for molecular data transformer such as Fingerprinter etc.
     If you create a subclass of this featurizer, you will need to make sure that the
     input argument of the init are kept as is in the object attributes.
 
     !!! note
         The transformer supports a variety of datatype, they are only enforced when passing the
         `enforce_dtype=True` attributes in `__call__`. For pandas dataframes, use `'pandas'|'df'|'dataframe'|pd.DataFrame`
+
+    ???+ tip "Using a custom Calculator"
+        You can use your own calculator for featurization. It's recommended to subclass `molfeat.calc.base.SerializableCalculator`
+        If you calculator also implements a `batch_compute` method, it will be used for batch featurization and parallelization options will be passed to it.
     """
 
     def __init__(
         self,
         featurizer: Union[str, Callable],
         n_jobs: int = 1,
         verbose: bool = False,
@@ -292,27 +296,30 @@
             mols = [mols]
 
         def _to_mol(x):
             return dm.to_mol(x) if x else None
 
         parallel_kwargs = getattr(self, "parallel_kwargs", {})
 
-        mols = dm.parallelized(_to_mol, mols, n_jobs=self.n_jobs, **parallel_kwargs)
-
-        if self.n_jobs not in [0, 1]:
-            # use a proxy model to run in parallel
-            cpy = self.copy()
-            features = dm.parallelized(
-                cpy._transform,
-                mols,
-                n_jobs=self.n_jobs,
-                **cpy.parallel_kwargs,
-            )
+        if hasattr(self.featurizer, "batch_compute") and callable(self.featurizer.batch_compute):
+            # this calculator can be batched which will be faster
+            features = self.featurizer.batch_compute(mols, n_jobs=self.n_jobs, **parallel_kwargs)
         else:
-            features = [self._transform(mol) for mol in mols]
+            mols = dm.parallelized(_to_mol, mols, n_jobs=self.n_jobs, **parallel_kwargs)
+            if self.n_jobs not in [0, 1]:
+                # use a proxy model to run in parallel
+                cpy = self.copy()
+                features = dm.parallelized(
+                    cpy._transform,
+                    mols,
+                    n_jobs=self.n_jobs,
+                    **cpy.parallel_kwargs,
+                )
+            else:
+                features = [self._transform(mol) for mol in mols]
         if not ignore_errors:
             for ind, feat in enumerate(features):
                 if feat is None:
                     raise ValueError(f"Cannot transform molecule at index {ind}")
 
         return features
```

### Comparing `molfeat-0.8.5/molfeat/trans/concat.py` & `molfeat-0.8.6/molfeat/trans/concat.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/fp.py` & `molfeat-0.8.6/molfeat/trans/fp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/graph/adj.py` & `molfeat-0.8.6/molfeat/trans/graph/adj.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/graph/tree.py` & `molfeat-0.8.6/molfeat/trans/graph/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/pretrained/base.py` & `molfeat-0.8.6/molfeat/trans/pretrained/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/pretrained/dgl_pretrained.py` & `molfeat-0.8.6/molfeat/trans/pretrained/dgl_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/pretrained/fcd.py` & `molfeat-0.8.6/molfeat/trans/pretrained/fcd.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/pretrained/graphormer.py` & `molfeat-0.8.6/molfeat/trans/pretrained/graphormer.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/pretrained/hf_transformers.py` & `molfeat-0.8.6/molfeat/trans/pretrained/hf_transformers.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/struct/esm.py` & `molfeat-0.8.6/molfeat/trans/struct/esm.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/trans/struct/prot1D.py` & `molfeat-0.8.6/molfeat/trans/struct/prot1D.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/cache.py` & `molfeat-0.8.6/molfeat/utils/cache.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/commons.py` & `molfeat-0.8.6/molfeat/utils/commons.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/const.py` & `molfeat-0.8.6/molfeat/utils/const.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/converters.py` & `molfeat-0.8.6/molfeat/utils/converters.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/datatype.py` & `molfeat-0.8.6/molfeat/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/log.py` & `molfeat-0.8.6/molfeat/utils/log.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/parsing.py` & `molfeat-0.8.6/molfeat/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/pooler.py` & `molfeat-0.8.6/molfeat/utils/pooler.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/requires.py` & `molfeat-0.8.6/molfeat/utils/requires.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/utils/state.py` & `molfeat-0.8.6/molfeat/utils/state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat/viz.py` & `molfeat-0.8.6/molfeat/viz.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/molfeat.egg-info/PKG-INFO` & `molfeat-0.8.6/molfeat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.5
+Version: 0.8.6
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -53,15 +53,15 @@
 
 [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/latestdoi/613548667)
 [![PyPI](https://img.shields.io/pypi/v/molfeat)](https://pypi.org/project/molfeat/)
 [![Conda](https://img.shields.io/conda/v/conda-forge/molfeat?label=conda&color=success)](https://anaconda.org/conda-forge/molfeat)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/molfeat)](https://pypi.org/project/molfeat/)
 [![Conda](https://img.shields.io/conda/dn/conda-forge/molfeat)](https://anaconda.org/conda-forge/molfeat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/molfeat)](https://pypi.org/project/molfeat/)
-[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/datamol/blob/main/LICENSE)
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/molfeat/blob/main/LICENSE)
 [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/molfeat)](https://github.com/datamol-io/molfeat/stargazers)
 [![GitHub Repo stars](https://img.shields.io/github/forks/datamol-io/molfeat)](https://github.com/datamol-io/molfeat/network/members)
 [![test](https://github.com/datamol-io/molfeat/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/test.yml)
 [![code-check](https://github.com/datamol-io/molfeat/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/molfeat/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/doc.yml)
 [![release](https://github.com/datamol-io/molfeat/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/release.yml)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.5 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.6 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -26,15 +26,15 @@
 pypi.org/project/molfeat/) [![Conda](https://img.shields.io/conda/v/conda-
 forge/molfeat?label=conda&color=success)](https://anaconda.org/conda-forge/
 molfeat) [![PyPI - Downloads](https://img.shields.io/pypi/dm/molfeat)](https://
 pypi.org/project/molfeat/) [![Conda](https://img.shields.io/conda/dn/conda-
 forge/molfeat)](https://anaconda.org/conda-forge/molfeat) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/molfeat)](https://pypi.org/
 project/molfeat/) [![license](https://img.shields.io/badge/License-
-Apache%202.0-blue.svg)](https://github.com/datamol-io/datamol/blob/main/
+Apache%202.0-blue.svg)](https://github.com/datamol-io/molfeat/blob/main/
 LICENSE) [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/
 molfeat)](https://github.com/datamol-io/molfeat/stargazers) [![GitHub Repo
 stars](https://img.shields.io/github/forks/datamol-io/molfeat)](https://
 github.com/datamol-io/molfeat/network/members) [![test](https://github.com/
 datamol-io/molfeat/actions/workflows/test.yml/badge.svg)](https://github.com/
 datamol-io/molfeat/actions/workflows/test.yml) [![code-check](https://
 github.com/datamol-io/molfeat/actions/workflows/code-check.yml/badge.svg)]
```

### Comparing `molfeat-0.8.5/molfeat.egg-info/SOURCES.txt` & `molfeat-0.8.6/molfeat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/pyproject.toml` & `molfeat-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/tests/test_atom_bond_calculator.py` & `molfeat-0.8.6/tests/test_atom_bond_calculator.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/tests/test_descriptors.py` & `molfeat-0.8.6/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/tests/test_fp.py` & `molfeat-0.8.6/tests/test_fp.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,42 @@
 import datamol as dm
 import pandas as pd
 import numpy as np
 import tempfile
 import joblib
 
 from rdkit.DataStructs.cDataStructs import ExplicitBitVect
+from molfeat.calc import SerializableCalculator
 from molfeat.calc.descriptors import MordredDescriptors
 from molfeat.calc.fingerprints import FPCalculator
 from molfeat.calc.pharmacophore import Pharmacophore2D
 from molfeat.trans import MoleculeTransformer
 from molfeat.trans.base import PrecomputedMolTransformer
 from molfeat.trans.fp import FPVecTransformer
 from molfeat.trans.fp import FPVecFilteredTransformer
 from molfeat.trans.concat import FeatConcat
 from molfeat.utils.cache import DataCache, FileCache, MPDataCache
 
 
+class CustomBatchCalculator(SerializableCalculator):
+    def __init__(self, random_seed: int = 42, length: int = 10):
+        self.random_seed = random_seed
+        self.length = length
+        self.rng = np.random.RandomState(self.random_seed)
+
+    def __call__(self, mol, **kwargs):
+        return self.rng.randn(self.length)
+
+    def __len__(self):
+        return self.length
+
+    def batch_compute(self, mols, **kwargs):
+        return self.rng.randn(len(mols), self.length)
+
+
 class TestMolTransformer(ut.TestCase):
     r"""Test cases for FingerprintsTransformer"""
     smiles = [
         "CCOc1c(OC)cc(CCN)cc1OC",
         "COc1cc(CCN)cc(OC)c1OC",
         "C[C@@H]([NH3+])Cc1c2ccoc2c(Br)c2ccoc12",
     ]
@@ -55,14 +72,21 @@
                 precomp, smiles, n_jobs=-1, batch_size=100, concatenate=True
             )
             self.assertTrue(smiles[0] in cache)
             self.assertTrue(len(cache) == len(fps))
             np.testing.assert_array_equal(cache[smiles[0]], fps[0])
             np.testing.assert_allclose(fps, batched_fps)
 
+    def test_custom_calculator(self):
+        calc = CustomBatchCalculator()
+        transf = MoleculeTransformer(featurizer=calc)
+        fps = transf.transform(self.smiles)
+        self.assertEqual(len(fps), len(self.smiles))
+        self.assertEqual(len(fps[0]), len(calc))
+
     def test_transformer(self):
         for fpkind in self.fp_list:
             transf = MoleculeTransformer(featurizer=fpkind)
             fps = transf.transform(self.smiles)
             unique_len = set([len(x) for x in fps])
             self.assertEqual(len(unique_len), 1)
```

### Comparing `molfeat-0.8.5/tests/test_graphs.py` & `molfeat-0.8.6/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/tests/test_pharmacophore.py` & `molfeat-0.8.6/tests/test_pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/tests/test_pretrained.py` & `molfeat-0.8.6/tests/test_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/tests/test_prot_embed.py` & `molfeat-0.8.6/tests/test_prot_embed.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/tests/test_state.py` & `molfeat-0.8.6/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.5/tests/test_utils.py` & `molfeat-0.8.6/tests/test_utils.py`

 * *Files identical despite different names*

