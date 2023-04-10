# Comparing `tmp/laion_clap-1.1.2.tar.gz` & `tmp/laion_clap-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laion_clap-1.1.2.tar", last modified: Sat Apr  1 20:35:21 2023, max compression
+gzip compressed data, was "laion_clap-1.1.3.tar", last modified: Mon Apr 10 03:47:12 2023, max compression
```

## Comparing `laion_clap-1.1.2.tar` & `laion_clap-1.1.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-01 20:35:21.090839 laion_clap-1.1.2/
--rw-rw-r--   0 la        (1000) la        (1000)     7048 2023-02-28 19:23:25.000000 laion_clap-1.1.2/LICENSE
--rw-rw-r--   0 la        (1000) la        (1000)      203 2023-03-14 06:16:18.000000 laion_clap-1.1.2/MANIFEST.in
--rw-rw-r--   0 la        (1000) la        (1000)    21877 2023-04-01 20:35:21.090839 laion_clap-1.1.2/PKG-INFO
--rw-rw-r--   0 la        (1000) la        (1000)    13072 2023-04-01 20:34:38.000000 laion_clap-1.1.2/README.md
--rw-rw-r--   0 la        (1000) la        (1000)     1199 2023-04-01 20:15:22.000000 laion_clap-1.1.2/pyproject.toml
--rw-rw-r--   0 la        (1000) la        (1000)       38 2023-04-01 20:35:21.090839 laion_clap-1.1.2/setup.cfg
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-01 20:35:21.086839 laion_clap-1.1.2/src/
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-01 20:35:21.086839 laion_clap-1.1.2/src/laion_clap/
--rw-rw-r--   0 la        (1000) la        (1000)      129 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/__init__.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-01 20:35:21.086839 laion_clap-1.1.2/src/laion_clap/clap_module/
--rw-rw-r--   0 la        (1000) la        (1000)      568 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/__init__.py
--rw-rw-r--   0 la        (1000) la        (1000)     1215 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/bert.py
--rw-rw-r--   0 la        (1000) la        (1000)  1356917 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 la        (1000) la        (1000)    10593 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/factory.py
--rw-rw-r--   0 la        (1000) la        (1000)     7182 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/feature_fusion.py
--rw-rw-r--   0 la        (1000) la        (1000)    45110 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/htsat.py
--rw-rw-r--   0 la        (1000) la        (1000)     2204 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/linear_probe.py
--rw-rw-r--   0 la        (1000) la        (1000)    14405 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/loss.py
--rw-rw-r--   0 la        (1000) la        (1000)    32754 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-01 20:35:21.090839 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/HTSAT-base.json
--rw-rw-r--   0 la        (1000) la        (1000)      498 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/HTSAT-large.json
--rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/HTSAT-tiny-win-1536.json
--rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/HTSAT-tiny.json
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/PANN-10.json
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/PANN-14-fmax-18k.json
--rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/PANN-14-fmax-8k-20s.json
--rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/PANN-14-tiny-transformer.json
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/PANN-14-win-1536.json
--rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/PANN-14.json
--rw-rw-r--   0 la        (1000) la        (1000)      495 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/PANN-6.json
--rw-rw-r--   0 la        (1000) la        (1000)      388 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/RN101-quickgelu.json
--rw-rw-r--   0 la        (1000) la        (1000)      364 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/RN101.json
--rw-rw-r--   0 la        (1000) la        (1000)      389 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/RN50-quickgelu.json
--rw-rw-r--   0 la        (1000) la        (1000)      364 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/RN50.json
--rw-rw-r--   0 la        (1000) la        (1000)      365 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/RN50x16.json
--rw-rw-r--   0 la        (1000) la        (1000)      365 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/RN50x4.json
--rw-rw-r--   0 la        (1000) la        (1000)      294 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/ViT-B-16.json
--rw-rw-r--   0 la        (1000) la        (1000)      318 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/ViT-B-32-quickgelu.json
--rw-rw-r--   0 la        (1000) la        (1000)      294 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/ViT-B-32.json
--rw-rw-r--   0 la        (1000) la        (1000)      296 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/model_configs/ViT-L-14.json
--rw-rw-r--   0 la        (1000) la        (1000)     4724 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/openai.py
--rw-rw-r--   0 la        (1000) la        (1000)    21221 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/pann_model.py
--rw-rw-r--   0 la        (1000) la        (1000)     6212 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/pretrained.py
--rw-rw-r--   0 la        (1000) la        (1000)     4300 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/timm_model.py
--rw-rw-r--   0 la        (1000) la        (1000)     6204 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/tokenizer.py
--rw-rw-r--   0 la        (1000) la        (1000)      872 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/transform.py
--rw-rw-r--   0 la        (1000) la        (1000)    12988 2023-04-01 20:15:10.000000 laion_clap-1.1.2/src/laion_clap/clap_module/utils.py
--rw-rw-r--   0 la        (1000) la        (1000)       22 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/clap_module/version.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-01 20:35:21.090839 laion_clap-1.1.2/src/laion_clap/evaluate/
--rw-rw-r--   0 la        (1000) la        (1000)        0 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/evaluate/__init__.py
--rw-rw-r--   0 la        (1000) la        (1000)     5455 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/evaluate/eval_dcase.py
--rw-rw-r--   0 la        (1000) la        (1000)    20038 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/evaluate/eval_linear_probe.py
--rw-rw-r--   0 la        (1000) la        (1000)     6718 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/evaluate/eval_retrieval.py
--rw-rw-r--   0 la        (1000) la        (1000)     9557 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/evaluate/eval_retrieval_main.py
--rw-rw-r--   0 la        (1000) la        (1000)     9885 2023-04-01 20:15:10.000000 laion_clap-1.1.2/src/laion_clap/evaluate/eval_zeroshot_classification.py
--rw-rw-r--   0 la        (1000) la        (1000)     9154 2023-04-01 20:32:17.000000 laion_clap-1.1.2/src/laion_clap/hook.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-01 20:35:21.090839 laion_clap-1.1.2/src/laion_clap/training/
--rw-rw-r--   0 la        (1000) la        (1000)        0 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/__init__.py
--rw-rw-r--   0 la        (1000) la        (1000)    84448 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/audioset_textmap.npy
--rw-rw-r--   0 la        (1000) la        (1000)    32527 2023-04-01 20:15:10.000000 laion_clap-1.1.2/src/laion_clap/training/data.py
--rw-rw-r--   0 la        (1000) la        (1000)     5078 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/distributed.py
--rw-rw-r--   0 la        (1000) la        (1000)    22135 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/imagenet_zeroshot_data.py
--rw-rw-r--   0 la        (1000) la        (1000)     3265 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/infer_demo.py
--rw-rw-r--   0 la        (1000) la        (1000)      899 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/logger.py
--rw-rw-r--   0 la        (1000) la        (1000)    25047 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/lp_main.py
--rw-rw-r--   0 la        (1000) la        (1000)    10645 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/lp_train.py
--rw-rw-r--   0 la        (1000) la        (1000)    22608 2023-04-01 20:31:07.000000 laion_clap-1.1.2/src/laion_clap/training/main.py
--rw-rw-r--   0 la        (1000) la        (1000)    17401 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/params.py
--rw-rw-r--   0 la        (1000) la        (1000)      659 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/scheduler.py
--rw-rw-r--   0 la        (1000) la        (1000)    35672 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/train.py
--rw-rw-r--   0 la        (1000) la        (1000)     3395 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/laion_clap/training/zero_shot.py
--rw-rw-r--   0 la        (1000) la        (1000)     2596 2023-04-01 20:34:21.000000 laion_clap-1.1.2/src/laion_clap/unit_test.py
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-01 20:35:21.086839 laion_clap-1.1.2/src/laion_clap.egg-info/
--rw-rw-r--   0 la        (1000) la        (1000)    21877 2023-04-01 20:35:21.000000 laion_clap-1.1.2/src/laion_clap.egg-info/PKG-INFO
--rw-rw-r--   0 la        (1000) la        (1000)     3095 2023-04-01 20:35:21.000000 laion_clap-1.1.2/src/laion_clap.egg-info/SOURCES.txt
--rw-rw-r--   0 la        (1000) la        (1000)        1 2023-04-01 20:35:21.000000 laion_clap-1.1.2/src/laion_clap.egg-info/dependency_links.txt
--rw-rw-r--   0 la        (1000) la        (1000)      146 2023-04-01 20:35:21.000000 laion_clap-1.1.2/src/laion_clap.egg-info/requires.txt
--rw-rw-r--   0 la        (1000) la        (1000)       17 2023-04-01 20:35:21.000000 laion_clap-1.1.2/src/laion_clap.egg-info/top_level.txt
-drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-01 20:35:21.090839 laion_clap-1.1.2/src/tests/
--rw-rw-r--   0 la        (1000) la        (1000)        0 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/tests/__init__.py
--rw-rw-r--   0 la        (1000) la        (1000)    56326 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/tests/check_ckpt.py
--rw-rw-r--   0 la        (1000) la        (1000)     3295 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/tests/check_tars.py
--rw-rw-r--   0 la        (1000) la        (1000)     2174 2023-03-14 06:16:18.000000 laion_clap-1.1.2/src/tests/data_loader_test.py
+drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.618166 laion_clap-1.1.3/
+-rw-rw-r--   0 la        (1000) la        (1000)     7048 2023-02-28 19:23:25.000000 laion_clap-1.1.3/LICENSE
+-rw-rw-r--   0 la        (1000) la        (1000)      203 2023-03-14 06:16:18.000000 laion_clap-1.1.3/MANIFEST.in
+-rw-rw-r--   0 la        (1000) la        (1000)    23293 2023-04-10 03:47:12.618166 laion_clap-1.1.3/PKG-INFO
+-rw-rw-r--   0 la        (1000) la        (1000)    14488 2023-04-10 03:33:21.000000 laion_clap-1.1.3/README.md
+-rw-rw-r--   0 la        (1000) la        (1000)     1218 2023-04-10 03:46:52.000000 laion_clap-1.1.3/pyproject.toml
+-rw-rw-r--   0 la        (1000) la        (1000)       38 2023-04-10 03:47:12.618166 laion_clap-1.1.3/setup.cfg
+drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.610166 laion_clap-1.1.3/src/
+drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.610166 laion_clap-1.1.3/src/laion_clap/
+-rw-rw-r--   0 la        (1000) la        (1000)      129 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/__init__.py
+drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/laion_clap/clap_module/
+-rw-rw-r--   0 la        (1000) la        (1000)      568 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/__init__.py
+-rw-rw-r--   0 la        (1000) la        (1000)     1215 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/bert.py
+-rw-rw-r--   0 la        (1000) la        (1000)  1356917 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 la        (1000) la        (1000)    10593 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/factory.py
+-rw-rw-r--   0 la        (1000) la        (1000)     7182 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/feature_fusion.py
+-rw-rw-r--   0 la        (1000) la        (1000)    45110 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/htsat.py
+-rw-rw-r--   0 la        (1000) la        (1000)     2204 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/linear_probe.py
+-rw-rw-r--   0 la        (1000) la        (1000)    14405 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/loss.py
+-rw-rw-r--   0 la        (1000) la        (1000)    32754 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model.py
+drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/
+-rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/HTSAT-base.json
+-rw-rw-r--   0 la        (1000) la        (1000)      498 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/HTSAT-large.json
+-rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/HTSAT-tiny-win-1536.json
+-rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/HTSAT-tiny.json
+-rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-10.json
+-rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14-fmax-18k.json
+-rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14-fmax-8k-20s.json
+-rw-rw-r--   0 la        (1000) la        (1000)      496 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14-tiny-transformer.json
+-rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14-win-1536.json
+-rw-rw-r--   0 la        (1000) la        (1000)      497 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-14.json
+-rw-rw-r--   0 la        (1000) la        (1000)      495 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/PANN-6.json
+-rw-rw-r--   0 la        (1000) la        (1000)      388 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN101-quickgelu.json
+-rw-rw-r--   0 la        (1000) la        (1000)      364 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN101.json
+-rw-rw-r--   0 la        (1000) la        (1000)      389 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN50-quickgelu.json
+-rw-rw-r--   0 la        (1000) la        (1000)      364 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN50.json
+-rw-rw-r--   0 la        (1000) la        (1000)      365 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN50x16.json
+-rw-rw-r--   0 la        (1000) la        (1000)      365 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/RN50x4.json
+-rw-rw-r--   0 la        (1000) la        (1000)      294 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/ViT-B-16.json
+-rw-rw-r--   0 la        (1000) la        (1000)      318 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/ViT-B-32-quickgelu.json
+-rw-rw-r--   0 la        (1000) la        (1000)      294 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/ViT-B-32.json
+-rw-rw-r--   0 la        (1000) la        (1000)      296 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/model_configs/ViT-L-14.json
+-rw-rw-r--   0 la        (1000) la        (1000)     4724 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/openai.py
+-rw-rw-r--   0 la        (1000) la        (1000)    21221 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/pann_model.py
+-rw-rw-r--   0 la        (1000) la        (1000)     6212 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/pretrained.py
+-rw-rw-r--   0 la        (1000) la        (1000)     4300 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/timm_model.py
+-rw-rw-r--   0 la        (1000) la        (1000)     6204 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/tokenizer.py
+-rw-rw-r--   0 la        (1000) la        (1000)      872 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/transform.py
+-rw-rw-r--   0 la        (1000) la        (1000)    12988 2023-04-01 20:15:10.000000 laion_clap-1.1.3/src/laion_clap/clap_module/utils.py
+-rw-rw-r--   0 la        (1000) la        (1000)       22 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/clap_module/version.py
+drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/laion_clap/evaluate/
+-rw-rw-r--   0 la        (1000) la        (1000)        0 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/__init__.py
+-rw-rw-r--   0 la        (1000) la        (1000)     5455 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_dcase.py
+-rw-rw-r--   0 la        (1000) la        (1000)    20038 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_linear_probe.py
+-rw-rw-r--   0 la        (1000) la        (1000)     6718 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_retrieval.py
+-rw-rw-r--   0 la        (1000) la        (1000)     9557 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_retrieval_main.py
+-rw-rw-r--   0 la        (1000) la        (1000)     9769 2023-04-10 03:33:21.000000 laion_clap-1.1.3/src/laion_clap/evaluate/eval_zeroshot_classification.py
+-rw-rw-r--   0 la        (1000) la        (1000)     8767 2023-04-10 03:35:37.000000 laion_clap-1.1.3/src/laion_clap/hook.py
+drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/laion_clap/training/
+-rw-rw-r--   0 la        (1000) la        (1000)        0 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/__init__.py
+-rw-rw-r--   0 la        (1000) la        (1000)    84448 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/audioset_textmap.npy
+-rw-rw-r--   0 la        (1000) la        (1000)    32641 2023-04-10 03:33:21.000000 laion_clap-1.1.3/src/laion_clap/training/data.py
+-rw-rw-r--   0 la        (1000) la        (1000)     5078 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/distributed.py
+-rw-rw-r--   0 la        (1000) la        (1000)    22135 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/imagenet_zeroshot_data.py
+-rw-rw-r--   0 la        (1000) la        (1000)     3265 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/infer_demo.py
+-rw-rw-r--   0 la        (1000) la        (1000)      899 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/logger.py
+-rw-rw-r--   0 la        (1000) la        (1000)    25047 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/lp_main.py
+-rw-rw-r--   0 la        (1000) la        (1000)    10645 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/lp_train.py
+-rw-rw-r--   0 la        (1000) la        (1000)    22608 2023-04-01 20:31:07.000000 laion_clap-1.1.3/src/laion_clap/training/main.py
+-rw-rw-r--   0 la        (1000) la        (1000)    17401 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/params.py
+-rw-rw-r--   0 la        (1000) la        (1000)      659 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/scheduler.py
+-rw-rw-r--   0 la        (1000) la        (1000)    35672 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/train.py
+-rw-rw-r--   0 la        (1000) la        (1000)     3395 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/laion_clap/training/zero_shot.py
+-rw-rw-r--   0 la        (1000) la        (1000)     2596 2023-04-01 20:34:21.000000 laion_clap-1.1.3/src/laion_clap/unit_test.py
+drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.610166 laion_clap-1.1.3/src/laion_clap.egg-info/
+-rw-rw-r--   0 la        (1000) la        (1000)    23293 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/PKG-INFO
+-rw-rw-r--   0 la        (1000) la        (1000)     3095 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/SOURCES.txt
+-rw-rw-r--   0 la        (1000) la        (1000)        1 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/dependency_links.txt
+-rw-rw-r--   0 la        (1000) la        (1000)      160 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/requires.txt
+-rw-rw-r--   0 la        (1000) la        (1000)       17 2023-04-10 03:47:12.000000 laion_clap-1.1.3/src/laion_clap.egg-info/top_level.txt
+drwxrwxr-x   0 la        (1000) la        (1000)        0 2023-04-10 03:47:12.614166 laion_clap-1.1.3/src/tests/
+-rw-rw-r--   0 la        (1000) la        (1000)        0 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/tests/__init__.py
+-rw-rw-r--   0 la        (1000) la        (1000)    56326 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/tests/check_ckpt.py
+-rw-rw-r--   0 la        (1000) la        (1000)     3295 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/tests/check_tars.py
+-rw-rw-r--   0 la        (1000) la        (1000)     2174 2023-03-14 06:16:18.000000 laion_clap-1.1.3/src/tests/data_loader_test.py
```

### Comparing `laion_clap-1.1.2/LICENSE` & `laion_clap-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/PKG-INFO` & `laion_clap-1.1.3/src/laion_clap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: laion_clap
-Version: 1.1.2
+Name: laion-clap
+Version: 1.1.3
 Summary: Contrastive Language-Audio Pretraining Model from LAION
 Author: Yusong Wu, Tianyu Zhang, Yuchen Hui
 Author-email: Ke Chen <knutchen@ucsd.edu>
 Maintainer: Yusong Wu, Tianyu Zhang, Yuchen Hui
 Maintainer-email: Ke Chen <knutchen@ucsd.edu>
 License: Creative Commons Legal Code
         
@@ -268,14 +268,33 @@
 ## Pretrained Models
 The pretrained checkpoints can be found in [here](https://huggingface.co/lukewys/laion_clap/tree/main).
 Please refer to the previous section for how to load and run the checkpoints.
 
 The checkpoints list here for each model setting is the one with the highest average mAP score in training.
 The average mAP score is calculated by averaging 4 scores: A-->T mAP@10 on AudioCaps, and T-->A mAP@10 on AudioCaps, A-->T mAP@10 on Clotho, and T-->A mAP@10 on Clotho.
 
+Update 2023.4.7: we have released 3 larger CLAP models trained on music, speech dataset in addition to LAION-Audio-630k. Here are descriptions of the model and their performance:
+
+ - `music_speech_audioset_epoch_15_esc_89.98.pt`: trained on music + speech + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 89.98%, the GTZAN performance is 73%.
+ - `music_audioset_epoch_15_esc_90.14.pt`: trained on music + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 90.14%, the GTZAN performance is 64%.
+ - `music_speech_epoch_15_esc_89.25.pt`: trained on music + speech + LAION-Audio-630k. The zeroshot ESC50 performance is 89.25%, the GTZAN performance is 73%.
+
+The model uses a larger audio encoder. To load the model using the pip API:
+```python
+import laion_clap
+model = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
+model.load_ckpt('checkpoint_path/checkpoint_name.pt')
+```
+
+Please note that this is a temporary release for people who are working on larger-scale down-stream task. 
+We will release a more comprehensive version of the model with detailed experiments in the future.
+Please take your own risk when using this model.
+
+* All the new checkpoints did not trained with fusion. The training dataset size for `music_speech_audioset_epoch_15_esc_89.98.pt` is around 4M samples. The zeroshot GTZAN score is evaluated using the prompt `This audio is a <genre> song.`
+
 ## Reproducibility
 An example of the preprocessed Clotho dataset in webdataset format can be download [here](https://drive.google.com/drive/folders/1mU9mBOe11jTFCrQRJQsUa4S-3TlNuYoI?usp=sharing) (by downloading, you will be agreeing the license described in the [Clotho dataset](https://zenodo.org/record/3490684#.Y9ALPeyZP1w)). The audio encoder pretrained with 48kHz AudioSet can be found [here](https://drive.google.com/drive/folders/1SMQyzJvc6DwJNuhQ_WI8tlCFL5HG2vk6?usp=sharing), where `HTSAT-fullset-imagenet-map=0.467.ckpt` is the checkpoint used to initalize our HTSAT audio encoder. You should get similar result by loading from the audio encoder checkpoint and training on same dataset.
 
 The script to train the model on Clotho dataset is included [here](experiment_scripts/train-only-clotho.sh). You need to replace the `datasetpath` and `pretrained-audio` to pointing to your own directory. You could check the [report](https://stability.wandb.io/clap/clap/reports/CLAP-trained-on-Clotho-dataset--VmlldzoyNzY?accessToken=c0erq9hhp7h880jclihd9j9if679s6bylwto33vo14yo5jg40ppe38qeoafoonpz) of the training script on a single A100 GPU for reference.
 
 Because most of the dataset has copyright restriction, unfortunatly we cannot directly share other preprocessed datasets. The caption generated by keyword-to-caption model for Audioset can be found [here](https://github.com/LAION-AI/audio-dataset/tree/main/laion-audio-630k#keyword-to-caption-augmentation)
```

### Comparing `laion_clap-1.1.2/README.md` & `laion_clap-1.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -127,14 +127,33 @@
 ## Pretrained Models
 The pretrained checkpoints can be found in [here](https://huggingface.co/lukewys/laion_clap/tree/main).
 Please refer to the previous section for how to load and run the checkpoints.
 
 The checkpoints list here for each model setting is the one with the highest average mAP score in training.
 The average mAP score is calculated by averaging 4 scores: A-->T mAP@10 on AudioCaps, and T-->A mAP@10 on AudioCaps, A-->T mAP@10 on Clotho, and T-->A mAP@10 on Clotho.
 
+Update 2023.4.7: we have released 3 larger CLAP models trained on music, speech dataset in addition to LAION-Audio-630k. Here are descriptions of the model and their performance:
+
+ - `music_speech_audioset_epoch_15_esc_89.98.pt`: trained on music + speech + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 89.98%, the GTZAN performance is 73%.
+ - `music_audioset_epoch_15_esc_90.14.pt`: trained on music + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 90.14%, the GTZAN performance is 64%.
+ - `music_speech_epoch_15_esc_89.25.pt`: trained on music + speech + LAION-Audio-630k. The zeroshot ESC50 performance is 89.25%, the GTZAN performance is 73%.
+
+The model uses a larger audio encoder. To load the model using the pip API:
+```python
+import laion_clap
+model = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
+model.load_ckpt('checkpoint_path/checkpoint_name.pt')
+```
+
+Please note that this is a temporary release for people who are working on larger-scale down-stream task. 
+We will release a more comprehensive version of the model with detailed experiments in the future.
+Please take your own risk when using this model.
+
+* All the new checkpoints did not trained with fusion. The training dataset size for `music_speech_audioset_epoch_15_esc_89.98.pt` is around 4M samples. The zeroshot GTZAN score is evaluated using the prompt `This audio is a <genre> song.`
+
 ## Reproducibility
 An example of the preprocessed Clotho dataset in webdataset format can be download [here](https://drive.google.com/drive/folders/1mU9mBOe11jTFCrQRJQsUa4S-3TlNuYoI?usp=sharing) (by downloading, you will be agreeing the license described in the [Clotho dataset](https://zenodo.org/record/3490684#.Y9ALPeyZP1w)). The audio encoder pretrained with 48kHz AudioSet can be found [here](https://drive.google.com/drive/folders/1SMQyzJvc6DwJNuhQ_WI8tlCFL5HG2vk6?usp=sharing), where `HTSAT-fullset-imagenet-map=0.467.ckpt` is the checkpoint used to initalize our HTSAT audio encoder. You should get similar result by loading from the audio encoder checkpoint and training on same dataset.
 
 The script to train the model on Clotho dataset is included [here](experiment_scripts/train-only-clotho.sh). You need to replace the `datasetpath` and `pretrained-audio` to pointing to your own directory. You could check the [report](https://stability.wandb.io/clap/clap/reports/CLAP-trained-on-Clotho-dataset--VmlldzoyNzY?accessToken=c0erq9hhp7h880jclihd9j9if679s6bylwto33vo14yo5jg40ppe38qeoafoonpz) of the training script on a single A100 GPU for reference.
 
 Because most of the dataset has copyright restriction, unfortunatly we cannot directly share other preprocessed datasets. The caption generated by keyword-to-caption model for Audioset can be found [here](https://github.com/LAION-AI/audio-dataset/tree/main/laion-audio-630k#keyword-to-caption-augmentation)
```

### Comparing `laion_clap-1.1.2/pyproject.toml` & `laion_clap-1.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "laion_clap"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Ke Chen", email="knutchen@ucsd.edu" },
   { name="Yusong Wu" },
   { name="Tianyu Zhang" },
   { name="Yuchen Hui" }
 ]
 maintainers = [
@@ -17,14 +17,15 @@
   { name="Yuchen Hui" }
 ]
 description = "Contrastive Language-Audio Pretraining Model from LAION"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
+  "numpy==1.23.5",
   "soundfile",
   "librosa",
   "torchlibrosa",
   "ftfy",
   "braceexpand",
   "webdataset",
   "wget",
```

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/__init__.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/__init__.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/bert.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/bert.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/bpe_simple_vocab_16e6.txt.gz` & `laion_clap-1.1.3/src/laion_clap/clap_module/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/factory.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/factory.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/feature_fusion.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/htsat.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/htsat.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/linear_probe.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/linear_probe.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/loss.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/loss.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/model.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/model.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/openai.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/openai.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/pann_model.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/pann_model.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/pretrained.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/pretrained.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/timm_model.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/timm_model.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/tokenizer.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/tokenizer.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/transform.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/transform.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/clap_module/utils.py` & `laion_clap-1.1.3/src/laion_clap/clap_module/utils.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/evaluate/eval_dcase.py` & `laion_clap-1.1.3/src/laion_clap/evaluate/eval_dcase.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/evaluate/eval_linear_probe.py` & `laion_clap-1.1.3/src/laion_clap/evaluate/eval_linear_probe.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/evaluate/eval_retrieval.py` & `laion_clap-1.1.3/src/laion_clap/evaluate/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/evaluate/eval_retrieval_main.py` & `laion_clap-1.1.3/src/laion_clap/evaluate/eval_retrieval_main.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/evaluate/eval_zeroshot_classification.py` & `laion_clap-1.1.3/src/laion_clap/evaluate/eval_zeroshot_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,18 @@
             all_audio_features.append(audio_features.detach().cpu())
             all_class_labels.append(torch.argmax(batch["class_label"], 1).long())
         all_audio_features = torch.cat(all_audio_features, dim=0)
         all_class_labels = torch.cat(all_class_labels, dim=0)
         metrics["num_samples"] = all_audio_features.shape[0]
 
         # get text features
-        all_texts = [f"This audio clip belongs to the genre of {t}." for t in args.class_index_dict.keys()]
-        # if args.val_dataset_names == ['GTZAN']:
-        #     all_texts = [f"This is a {t} song." for t in args.class_index_dict.keys()]
-        # else:
-        #     all_texts = [f"This is a sound of {t}." for t in args.class_index_dict.keys()]
+        if args.val_dataset_names == ['GTZAN']:
+            all_texts = [f"This is a {t} song." for t in args.class_index_dict.keys()]
+        else:
+            all_texts = [f"This is a sound of {t}." for t in args.class_index_dict.keys()]
         logging.info(f'class label prompts: {all_texts}')
         # (yusong): a hack, can make it better
         if args.tmodel == "transformer":
             from clap_module.tokenizer import tokenize
             all_texts = tokenize(all_texts)
         else:
             from training.data import tokenizer
```

### Comparing `laion_clap-1.1.2/src/laion_clap/hook.py` & `laion_clap-1.1.3/src/laion_clap/hook.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,25 @@
 """
 Contrastive Language-Audio Pretraining Model from LAION
 --------------------------------------------------------
 Paper: https://arxiv.org/abs/2211.06687
 Authors (equal contributions): Ke Chen, Yusong Wu, Tianyu Zhang, Yuchen Hui
 Support: LAION
 """
-import progressbar
 import os
 import torch
 import librosa
 from clap_module import create_model
 from training.data import get_audio_features
 from training.data import int16_to_float32, float32_to_int16
 
 from transformers import RobertaTokenizer
 import wget
 from clap_module.factory import load_state_dict
 
-pbar = None
-
-
-def show_progress(block_num, block_size, total_size):
-    global pbar
-    if pbar is None:
-        pbar = progressbar.ProgressBar(maxval=total_size)
-        pbar.start()
-    downloaded = block_num * block_size
-    print(downloaded, total_size)
-    if downloaded < total_size:
-        pbar.update(downloaded)
-    else:
-        pbar.finish()
-        pbar = None
-
 
 class CLAP_Module(torch.nn.Module):
     def __init__(self, enable_fusion=False, device=None, amodel= 'HTSAT-tiny', tmodel='roberta') -> None:
         """Initialize CLAP Model
 
         Parameters
         ----------
@@ -48,14 +31,15 @@
             audio encoder architecture, default: HTSAT-tiny
         tmodel: str
             text encoder architecture, default: roberta
         """
         super(CLAP_Module, self).__init__()
         if device is None:
             device = 'cuda:0' if torch.cuda.is_available() else 'cpu'
+
         precision = 'fp32'
 
         if enable_fusion:
             fusion_type = 'aff_2d'
             model, model_cfg = create_model(
                 amodel,
                 tmodel,
@@ -68,15 +52,15 @@
             model, model_cfg = create_model(
                 amodel,
                 tmodel,
                 precision=precision,
                 device=device,
                 enable_fusion=enable_fusion
             )
-        self.enbale_fusion = enable_fusion
+        self.enable_fusion = enable_fusion
         self.model = model
         self.model_cfg = model_cfg
         self.tokenize = RobertaTokenizer.from_pretrained('roberta-base')
 
     def tokenizer(self, text):
         result = self.tokenize(
             text,
@@ -111,15 +95,15 @@
             '630k-audioset-fusion-best.pt'
         ]
         if ckpt is not None:
             print(f'Load the specified checkpoint {ckpt} from users.')
         else:
             print(f'Load our best checkpoint in the paper.')
             if model_id == -1:
-                model_id = 3 if self.enbale_fusion else 1
+                model_id = 3 if self.enable_fusion else 1
             package_dir = os.path.dirname(os.path.realpath(__file__))
             weight_file_name = download_names[model_id]
             ckpt = os.path.join(package_dir, weight_file_name)
             if os.path.exists(ckpt):
                 print(f'The checkpoint is already downloaded')
             else:
                 print('Downloading laion_clap weight files...')
@@ -151,20 +135,20 @@
         for f in x:
             # load the waveform of the shape (T,), should resample to 48000
             audio_waveform, _ = librosa.load(f, sr=48000)           
             # quantize
             audio_waveform = int16_to_float32(float32_to_int16(audio_waveform))
             audio_waveform = torch.from_numpy(audio_waveform).float()
             temp_dict = {}
-            # the 'fusion' truncate mode can be changed to 'rand_trunc' if run in unfusion mode
             temp_dict = get_audio_features(
                 temp_dict, audio_waveform, 480000, 
-                data_truncating='fusion', 
+                data_truncating='fusion' if self.enable_fusion else 'rand_trunc', 
                 data_filling='repeatpad',
-                audio_cfg=self.model_cfg['audio_cfg']
+                audio_cfg=self.model_cfg['audio_cfg'],
+                require_grad=audio_waveform.requires_grad
             )
             audio_input.append(temp_dict)
         audio_embed = self.model.get_audio_embedding(audio_input)
         if not use_tensor:
             audio_embed = audio_embed.detach().cpu().numpy()
         return audio_embed
 
@@ -188,20 +172,20 @@
         audio_input = []
         for audio_waveform in x:          
             # quantize
             if not use_tensor:
                 audio_waveform = int16_to_float32(float32_to_int16(audio_waveform))
                 audio_waveform = torch.from_numpy(audio_waveform).float()
             temp_dict = {}
-            # the 'fusion' truncate mode can be changed to 'rand_trunc' if run in unfusion mode
             temp_dict = get_audio_features(
                 temp_dict, audio_waveform, 480000, 
-                data_truncating='fusion', 
+                data_truncating='fusion' if self.enable_fusion else 'rand_trunc', 
                 data_filling='repeatpad',
-                audio_cfg=self.model_cfg['audio_cfg']
+                audio_cfg=self.model_cfg['audio_cfg'],
+                require_grad=audio_waveform.requires_grad
             )
             audio_input.append(temp_dict)
         audio_embed = self.model.get_audio_embedding(audio_input)
         if not use_tensor:
             audio_embed = audio_embed.detach().cpu().numpy()
         return audio_embed
```

### Comparing `laion_clap-1.1.2/src/laion_clap/training/audioset_textmap.npy` & `laion_clap-1.1.3/src/laion_clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/data.py` & `laion_clap-1.1.3/src/laion_clap/training/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,15 @@
                     [int(sizes[os.path.basename(shard)]) for shard in shards_list]
                 )
             elif os.path.exists(len_filename):
                 # FIXME this used to be eval(open(...)) but that seemed rather unsafe
                 total_size = ast.literal_eval(open(len_filename, "r").read())
             else:
                 raise Exception(
-                    "Cannot find sizes file for dataset. Please specify the path to the file."
+                    f"Cannot find sizes file for dataset {shards}. Please specify the path to the file."
                 )
                 # total_size = None  # num samples undefined
                 # some common dataset sizes (at time of authors last download)
                 # cc3m-train: 2905954
                 # cc12m: 10968539
                 # LAION-400m: 407332084
         num_shards = len(shards_list)
@@ -358,39 +358,41 @@
         [os.path.join(v, k) for k, v in sampled_filepath_dict.items()],
         sampled_size_dict,
     )
 
 
 def get_mel(audio_data, audio_cfg):
     # mel shape: (n_mels, T)
-    mel = torchaudio.transforms.MelSpectrogram(
+    mel_tf = torchaudio.transforms.MelSpectrogram(
         sample_rate=audio_cfg['sample_rate'],
         n_fft=audio_cfg['window_size'],
         win_length=audio_cfg['window_size'],
         hop_length=audio_cfg['hop_size'],
         center=True,
         pad_mode="reflect",
         power=2.0,
         norm=None,
         onesided=True,
-        n_mels=64,
+        n_mels=audio_cfg['mel_bins'],
         f_min=audio_cfg['fmin'],
         f_max=audio_cfg['fmax']
-    )(audio_data)
+    ).to(audio_data.device)
+    
+    mel = mel_tf(audio_data)
     # Align to librosa:
     # librosa_melspec = librosa.feature.melspectrogram(
     #     waveform,
     #     sr=audio_cfg['sample_rate'],
     #     n_fft=audio_cfg['window_size'],
     #     hop_length=audio_cfg['hop_size'],
     #     win_length=audio_cfg['window_size'],
     #     center=True,
     #     pad_mode="reflect",
     #     power=2.0,
-    #     n_mels=64,
+    #     n_mels=audio_cfg['mel_bins'],
     #     norm=None,
     #     htk=True,
     #     f_min=audio_cfg['fmin'],
     #     f_max=audio_cfg['fmax']
     # )
     # we use log mel spectrogram as input
     mel = torchaudio.transforms.AmplitudeToDB(top_db=None)(mel)
@@ -445,15 +447,15 @@
                     idx_back = np.random.choice(ranges[2])
                     # select mel
                     mel_chunk_front = mel[idx_front:idx_front + chunk_frames, :]
                     mel_chunk_middle = mel[idx_middle:idx_middle + chunk_frames, :]
                     mel_chunk_back = mel[idx_back:idx_back + chunk_frames, :]
 
                     # shrink the mel
-                    mel_shrink = torchvision.transforms.Resize(size=[chunk_frames, 64])(mel[None])[0]
+                    mel_shrink = torchvision.transforms.Resize(size=[chunk_frames, audio_cfg['mel_bins']])(mel[None])[0]
                     # logging.info(f"mel_shrink.shape: {mel_shrink.shape}")
 
                     # stack
                     mel_fusion = torch.stack([mel_shrink, mel_chunk_front, mel_chunk_middle, mel_chunk_back], dim=0)
                     sample["mel_fusion"] = mel_fusion
                     longer = torch.tensor([True])
             else:
```

### Comparing `laion_clap-1.1.2/src/laion_clap/training/distributed.py` & `laion_clap-1.1.3/src/laion_clap/training/distributed.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/imagenet_zeroshot_data.py` & `laion_clap-1.1.3/src/laion_clap/training/imagenet_zeroshot_data.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/infer_demo.py` & `laion_clap-1.1.3/src/laion_clap/training/infer_demo.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/logger.py` & `laion_clap-1.1.3/src/laion_clap/training/logger.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/lp_main.py` & `laion_clap-1.1.3/src/laion_clap/training/lp_main.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/lp_train.py` & `laion_clap-1.1.3/src/laion_clap/training/lp_train.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/main.py` & `laion_clap-1.1.3/src/laion_clap/training/main.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/params.py` & `laion_clap-1.1.3/src/laion_clap/training/params.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/scheduler.py` & `laion_clap-1.1.3/src/laion_clap/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/train.py` & `laion_clap-1.1.3/src/laion_clap/training/train.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/training/zero_shot.py` & `laion_clap-1.1.3/src/laion_clap/training/zero_shot.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap/unit_test.py` & `laion_clap-1.1.3/src/laion_clap/unit_test.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/laion_clap.egg-info/PKG-INFO` & `laion_clap-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: laion-clap
-Version: 1.1.2
+Name: laion_clap
+Version: 1.1.3
 Summary: Contrastive Language-Audio Pretraining Model from LAION
 Author: Yusong Wu, Tianyu Zhang, Yuchen Hui
 Author-email: Ke Chen <knutchen@ucsd.edu>
 Maintainer: Yusong Wu, Tianyu Zhang, Yuchen Hui
 Maintainer-email: Ke Chen <knutchen@ucsd.edu>
 License: Creative Commons Legal Code
         
@@ -268,14 +268,33 @@
 ## Pretrained Models
 The pretrained checkpoints can be found in [here](https://huggingface.co/lukewys/laion_clap/tree/main).
 Please refer to the previous section for how to load and run the checkpoints.
 
 The checkpoints list here for each model setting is the one with the highest average mAP score in training.
 The average mAP score is calculated by averaging 4 scores: A-->T mAP@10 on AudioCaps, and T-->A mAP@10 on AudioCaps, A-->T mAP@10 on Clotho, and T-->A mAP@10 on Clotho.
 
+Update 2023.4.7: we have released 3 larger CLAP models trained on music, speech dataset in addition to LAION-Audio-630k. Here are descriptions of the model and their performance:
+
+ - `music_speech_audioset_epoch_15_esc_89.98.pt`: trained on music + speech + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 89.98%, the GTZAN performance is 73%.
+ - `music_audioset_epoch_15_esc_90.14.pt`: trained on music + Audioset + LAION-Audio-630k. The zeroshot ESC50 performance is 90.14%, the GTZAN performance is 64%.
+ - `music_speech_epoch_15_esc_89.25.pt`: trained on music + speech + LAION-Audio-630k. The zeroshot ESC50 performance is 89.25%, the GTZAN performance is 73%.
+
+The model uses a larger audio encoder. To load the model using the pip API:
+```python
+import laion_clap
+model = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
+model.load_ckpt('checkpoint_path/checkpoint_name.pt')
+```
+
+Please note that this is a temporary release for people who are working on larger-scale down-stream task. 
+We will release a more comprehensive version of the model with detailed experiments in the future.
+Please take your own risk when using this model.
+
+* All the new checkpoints did not trained with fusion. The training dataset size for `music_speech_audioset_epoch_15_esc_89.98.pt` is around 4M samples. The zeroshot GTZAN score is evaluated using the prompt `This audio is a <genre> song.`
+
 ## Reproducibility
 An example of the preprocessed Clotho dataset in webdataset format can be download [here](https://drive.google.com/drive/folders/1mU9mBOe11jTFCrQRJQsUa4S-3TlNuYoI?usp=sharing) (by downloading, you will be agreeing the license described in the [Clotho dataset](https://zenodo.org/record/3490684#.Y9ALPeyZP1w)). The audio encoder pretrained with 48kHz AudioSet can be found [here](https://drive.google.com/drive/folders/1SMQyzJvc6DwJNuhQ_WI8tlCFL5HG2vk6?usp=sharing), where `HTSAT-fullset-imagenet-map=0.467.ckpt` is the checkpoint used to initalize our HTSAT audio encoder. You should get similar result by loading from the audio encoder checkpoint and training on same dataset.
 
 The script to train the model on Clotho dataset is included [here](experiment_scripts/train-only-clotho.sh). You need to replace the `datasetpath` and `pretrained-audio` to pointing to your own directory. You could check the [report](https://stability.wandb.io/clap/clap/reports/CLAP-trained-on-Clotho-dataset--VmlldzoyNzY?accessToken=c0erq9hhp7h880jclihd9j9if679s6bylwto33vo14yo5jg40ppe38qeoafoonpz) of the training script on a single A100 GPU for reference.
 
 Because most of the dataset has copyright restriction, unfortunatly we cannot directly share other preprocessed datasets. The caption generated by keyword-to-caption model for Audioset can be found [here](https://github.com/LAION-AI/audio-dataset/tree/main/laion-audio-630k#keyword-to-caption-augmentation)
```

### Comparing `laion_clap-1.1.2/src/laion_clap.egg-info/SOURCES.txt` & `laion_clap-1.1.3/src/laion_clap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/tests/check_ckpt.py` & `laion_clap-1.1.3/src/tests/check_ckpt.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/tests/check_tars.py` & `laion_clap-1.1.3/src/tests/check_tars.py`

 * *Files identical despite different names*

### Comparing `laion_clap-1.1.2/src/tests/data_loader_test.py` & `laion_clap-1.1.3/src/tests/data_loader_test.py`

 * *Files identical despite different names*

