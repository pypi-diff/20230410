# Comparing `tmp/so_vits_svc_fork-3.1.6.tar.gz` & `tmp/so_vits_svc_fork-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.1.6.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.1.7.tar", max compression
```

## Comparing `so_vits_svc_fork-3.1.6.tar` & `so_vits_svc_fork-3.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-09 15:42:33.495442 so_vits_svc_fork-3.1.6/LICENSE
--rw-r--r--   0        0        0    17988 2023-04-09 15:42:33.495442 so_vits_svc_fork-3.1.6/README.md
--rw-r--r--   0        0        0     3113 2023-04-09 15:42:34.563462 so_vits_svc_fork-3.1.6/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-09 15:42:34.515461 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22637 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1275 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2712 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2826 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7259 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    24381 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    22944 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0      731 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1627 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1377 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1438 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2997 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4614 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4693 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    16186 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13081 2023-04-09 15:42:33.503442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    19957 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.1.6/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-09 22:37:18.171573 so_vits_svc_fork-3.1.7/LICENSE
+-rw-r--r--   0        0        0    17988 2023-04-09 22:37:18.171573 so_vits_svc_fork-3.1.7/README.md
+-rw-r--r--   0        0        0     3113 2023-04-09 22:37:19.227589 so_vits_svc_fork-3.1.7/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-09 22:37:19.175588 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22637 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1275 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2712 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2826 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7259 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    24381 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    22944 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0      731 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1627 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1377 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1438 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2997 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4614 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4693 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    16240 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13081 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    19957 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.1.7/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.1.6/LICENSE` & `so_vits_svc_fork-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/README.md` & `so_vits_svc_fork-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/pyproject.toml` & `so_vits_svc_fork-3.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.1.6"
+version = "3.1.7"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,48 @@
         else 32,
     )
     model = VitsLightning(reset_optimizer=reset_optimizer, **hparams)
     trainer.fit(model, datamodule=datamodule)
 
 
 class VitsLightning(pl.LightningModule):
+    def __init__(self, reset_optimizer: bool = False, **hparams: Any):
+        super().__init__()
+        self._temp_epoch = 0  # Add this line to initialize the _temp_epoch attribute
+        self.save_hyperparameters("reset_optimizer")
+        self.save_hyperparameters(*[k for k in hparams.keys()])
+        torch.manual_seed(self.hparams.train.seed)
+        self.net_g = SynthesizerTrn(
+            self.hparams.data.filter_length // 2 + 1,
+            self.hparams.train.segment_size // self.hparams.data.hop_length,
+            **self.hparams.model,
+        )
+        self.net_d = MultiPeriodDiscriminator(self.hparams.model.use_spectral_norm)
+        self.automatic_optimization = False
+        self.optim_g = torch.optim.AdamW(
+            self.net_g.parameters(),
+            self.hparams.train.learning_rate,
+            betas=self.hparams.train.betas,
+            eps=self.hparams.train.eps,
+        )
+        self.optim_d = torch.optim.AdamW(
+            self.net_d.parameters(),
+            self.hparams.train.learning_rate,
+            betas=self.hparams.train.betas,
+            eps=self.hparams.train.eps,
+        )
+        self.scheduler_g = torch.optim.lr_scheduler.ExponentialLR(
+            self.optim_g, gamma=self.hparams.train.lr_decay
+        )
+        self.scheduler_d = torch.optim.lr_scheduler.ExponentialLR(
+            self.optim_d, gamma=self.hparams.train.lr_decay
+        )
+        self.optimizers_count = 2
+        self.load(reset_optimizer)
+
     def on_train_start(self) -> None:
         self.set_current_epoch(self._temp_epoch)
         total_batch_idx = self._temp_epoch * len(self.trainer.train_dataloader)
         self.set_total_batch_idx(total_batch_idx)
         global_step = total_batch_idx * self.optimizers_count
         self.set_global_step(global_step)
 
@@ -177,47 +211,14 @@
                 self.scheduler_g.last_epoch = epoch - 1
                 self.scheduler_d.last_epoch = epoch - 1
             except Exception as e:
                 raise RuntimeError("Failed to load checkpoint") from e
         else:
             LOG.warning("No checkpoint found. Start from scratch.")
 
-    def __init__(self, reset_optimizer: bool = False, **hparams: Any):
-        super().__init__()
-        self.save_hyperparameters("reset_optimizer")
-        self.save_hyperparameters(*[k for k in hparams.keys()])
-        torch.manual_seed(self.hparams.train.seed)
-        self.net_g = SynthesizerTrn(
-            self.hparams.data.filter_length // 2 + 1,
-            self.hparams.train.segment_size // self.hparams.data.hop_length,
-            **self.hparams.model,
-        )
-        self.net_d = MultiPeriodDiscriminator(self.hparams.model.use_spectral_norm)
-        self.automatic_optimization = False
-        self.optim_g = torch.optim.AdamW(
-            self.net_g.parameters(),
-            self.hparams.train.learning_rate,
-            betas=self.hparams.train.betas,
-            eps=self.hparams.train.eps,
-        )
-        self.optim_d = torch.optim.AdamW(
-            self.net_d.parameters(),
-            self.hparams.train.learning_rate,
-            betas=self.hparams.train.betas,
-            eps=self.hparams.train.eps,
-        )
-        self.scheduler_g = torch.optim.lr_scheduler.ExponentialLR(
-            self.optim_g, gamma=self.hparams.train.lr_decay
-        )
-        self.scheduler_d = torch.optim.lr_scheduler.ExponentialLR(
-            self.optim_d, gamma=self.hparams.train.lr_decay
-        )
-        self.optimizers_count = 2
-        self.load(reset_optimizer)
-
     def configure_optimizers(self):
         return [self.optim_g, self.optim_d], [self.scheduler_g, self.scheduler_d]
 
     def log_image_dict(
         self, image_dict: dict[str, Any], dataformats: str = "HWC"
     ) -> None:
         if not isinstance(self.logger, TensorBoardLogger):
@@ -235,15 +236,15 @@
             warnings.warn("Audio logging is only supported with TensorBoardLogger.")
             return
         writer: SummaryWriter = self.logger.experiment
         for k, v in audio_dict.items():
             writer.add_audio(
                 k,
                 v,
-                self.trainer.fit_loop.total_batch_idx,
+                self.total_batch_idx,
                 sample_rate=self.hparams.data.sampling_rate,
             )
 
     def log_dict_(self, log_dict: dict[str, Any], **kwargs) -> None:
         if not isinstance(self.logger, TensorBoardLogger):
             warnings.warn("Logging is only supported with TensorBoardLogger.")
             return
@@ -287,16 +288,16 @@
             y,
             ids_slice * self.hparams.data.hop_length,
             self.hparams.train.segment_size,
         )
 
         # generator loss
         LOG.debug("Calculating generator loss")
-        with torch.no_grad():
-            y_d_hat_r, y_d_hat_g, fmap_r, fmap_g = self.net_d(y, y_hat)
+        y_d_hat_r, y_d_hat_g, fmap_r, fmap_g = self.net_d(y, y_hat)
+
         with autocast(enabled=False):
             loss_mel = F.l1_loss(y_mel, y_hat_mel) * self.hparams.train.c_mel
             loss_kl = (
                 kl_loss(z_p, logs_q, m_p, logs_p, z_mask) * self.hparams.train.c_kl
             )
             loss_fm = feature_loss(fmap_r, fmap_g)
             loss_gen, losses_gen = generator_loss(y_d_hat_g)
@@ -349,17 +350,17 @@
                         lf0[0, 0, :].cpu().numpy(),
                         norm_lf0[0, 0, :].detach().cpu().numpy(),
                     ),
                 }
             )
 
         # optimizer
+        optim_g.zero_grad()
         self.manual_backward(loss_gen_all)
         optim_g.step()
-        optim_g.zero_grad()
         self.untoggle_optimizer(optim_g)
 
         # Discriminator
         # train
         self.toggle_optimizer(optim_d)
         y_d_hat_r, y_d_hat_g, _, _ = self.net_d(y, y_hat.detach())
 
@@ -373,17 +374,17 @@
         # log loss
         self.log_("loss/d/total", loss_disc_all, prog_bar=True)
         self.log_(
             "grad_norm_d", commons.clip_grad_value_(self.net_d.parameters(), None)
         )
 
         # optimizer
+        optim_d.zero_grad()
         self.manual_backward(loss_disc_all)
         optim_d.step()
-        optim_d.zero_grad()
         self.untoggle_optimizer(optim_d)
 
     def validation_step(self, batch, batch_idx):
         with torch.no_grad():
             self.net_g.eval()
             c, f0, _, mel, y, g, _, uv = batch
             y_hat = self.net_g.infer(c, f0, uv, g=g)
@@ -395,15 +396,15 @@
                 {
                     "gen/mel": utils.plot_spectrogram_to_numpy(
                         y_hat_mel[0].cpu().numpy()
                     ),
                     "gt/mel": utils.plot_spectrogram_to_numpy(mel[0].cpu().numpy()),
                 }
             )
-            if self.current_epoch == 0:
+            if self.current_epoch == 0 or batch_idx != 0:
                 return
             utils.save_checkpoint(
                 self.net_g,
                 self.optim_g,
                 self.hparams.train.learning_rate,
                 self.current_epoch + 1,  # prioritize prevention of undervaluation
                 Path(self.hparams.model_dir) / f"G_{self.total_batch_idx}.pth",
```

### Comparing `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.6/PKG-INFO` & `so_vits_svc_fork-3.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.1.6
+Version: 3.1.7
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.1.6 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.1.7 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

