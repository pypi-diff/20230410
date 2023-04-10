# Comparing `tmp/so_vits_svc_fork-3.1.7.tar.gz` & `tmp/so_vits_svc_fork-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.1.7.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.1.8.tar", max compression
```

## Comparing `so_vits_svc_fork-3.1.7.tar` & `so_vits_svc_fork-3.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-09 22:37:18.171573 so_vits_svc_fork-3.1.7/LICENSE
--rw-r--r--   0        0        0    17988 2023-04-09 22:37:18.171573 so_vits_svc_fork-3.1.7/README.md
--rw-r--r--   0        0        0     3113 2023-04-09 22:37:19.227589 so_vits_svc_fork-3.1.7/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-09 22:37:19.175588 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22637 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1275 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2712 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2826 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7259 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    24381 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    22944 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0      731 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-09 22:37:18.175573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1627 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1377 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1438 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2997 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4614 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4693 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    16240 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13081 2023-04-09 22:37:18.179573 so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    19957 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.1.7/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-10 10:50:42.816867 so_vits_svc_fork-3.1.8/LICENSE
+-rw-r--r--   0        0        0    17996 2023-04-10 10:50:42.816867 so_vits_svc_fork-3.1.8/README.md
+-rw-r--r--   0        0        0     3113 2023-04-10 10:50:43.808863 so_vits_svc_fork-3.1.8/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-10 10:50:43.760863 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22637 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1275 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2712 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2826 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7259 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    24381 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    22944 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0      731 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1627 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1377 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1438 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2997 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4614 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4693 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    16240 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13081 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.1.8/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.1.7/LICENSE` & `so_vits_svc_fork-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/README.md` & `so_vits_svc_fork-3.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -148,16 +148,16 @@
 - In real-time inference, if there is noise on the inputs, the HuBERT model will react to those as well. Consider using realtime noise reduction applications such as [RTX Voice](https://www.nvidia.com/en-us/geforce/guides/nvidia-rtx-voice-setup-guide/) in this case.
 
 ### Training
 
 #### Before training
 
 - If your dataset has BGM, please remove the BGM using software such as [Ultimate Vocal Remover](https://ultimatevocalremover.com/). `3_HP-Vocal-UVR.pth` or `UVR-MDX-NET Main` is recommended. [^1]
-- If your dataset is a long audio file with a single speaker, use `svc split` to split the dataset into multiple files (using `librosa`).
-- If your dataset is a long audio file with multiple speakers, use `svc sd` to split the dataset into multiple files (using `pyannote.audio`). Further manual classification may be necessary due to accuracy issues. If speakers speak with a variety of speech styles, set --min-speakers larger than the actual number of speakers. Due to unresolved dependencies, please install `pyannote.audio` manually: `pip install pyannote-audio`.
+- If your dataset is a long audio file with a single speaker, use `svc pre-split` to split the dataset into multiple files (using `librosa`).
+- If your dataset is a long audio file with multiple speakers, use `svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`). Further manual classification may be necessary due to accuracy issues. If speakers speak with a variety of speech styles, set --min-speakers larger than the actual number of speakers. Due to unresolved dependencies, please install `pyannote.audio` manually: `pip install pyannote-audio`.
 
 [^1]: https://ytpmv.info/how-to-use-uvr/
 
 #### Cloud
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-vits-svc-fork-4.0.ipynb)
 [![Open In Paperspace](https://img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://console.paperspace.com/github/34j/so-vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb)
```

#### html2text {}

```diff
@@ -43,17 +43,17 @@
 inference, if there is noise on the inputs, the HuBERT model will react to
 those as well. Consider using realtime noise reduction applications such as
 [RTX Voice](https://www.nvidia.com/en-us/geforce/guides/nvidia-rtx-voice-setup-
 guide/) in this case. ### Training #### Before training - If your dataset has
 BGM, please remove the BGM using software such as [Ultimate Vocal Remover]
 (https://ultimatevocalremover.com/). `3_HP-Vocal-UVR.pth` or `UVR-MDX-NET Main`
 is recommended. [^1] - If your dataset is a long audio file with a single
-speaker, use `svc split` to split the dataset into multiple files (using
+speaker, use `svc pre-split` to split the dataset into multiple files (using
 `librosa`). - If your dataset is a long audio file with multiple speakers, use
-`svc sd` to split the dataset into multiple files (using `pyannote.audio`).
+`svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`).
 Further manual classification may be necessary due to accuracy issues. If
 speakers speak with a variety of speech styles, set --min-speakers larger than
 the actual number of speakers. Due to unresolved dependencies, please install
 `pyannote.audio` manually: `pip install pyannote-audio`. [^1]: https://
 ytpmv.info/how-to-use-uvr/ #### Cloud [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-
```

### Comparing `so_vits_svc_fork-3.1.7/pyproject.toml` & `so_vits_svc_fork-3.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.1.7"
+version = "3.1.8"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.7/PKG-INFO` & `so_vits_svc_fork-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.1.7
+Version: 3.1.8
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -206,16 +206,16 @@
 - In real-time inference, if there is noise on the inputs, the HuBERT model will react to those as well. Consider using realtime noise reduction applications such as [RTX Voice](https://www.nvidia.com/en-us/geforce/guides/nvidia-rtx-voice-setup-guide/) in this case.
 
 ### Training
 
 #### Before training
 
 - If your dataset has BGM, please remove the BGM using software such as [Ultimate Vocal Remover](https://ultimatevocalremover.com/). `3_HP-Vocal-UVR.pth` or `UVR-MDX-NET Main` is recommended. [^1]
-- If your dataset is a long audio file with a single speaker, use `svc split` to split the dataset into multiple files (using `librosa`).
-- If your dataset is a long audio file with multiple speakers, use `svc sd` to split the dataset into multiple files (using `pyannote.audio`). Further manual classification may be necessary due to accuracy issues. If speakers speak with a variety of speech styles, set --min-speakers larger than the actual number of speakers. Due to unresolved dependencies, please install `pyannote.audio` manually: `pip install pyannote-audio`.
+- If your dataset is a long audio file with a single speaker, use `svc pre-split` to split the dataset into multiple files (using `librosa`).
+- If your dataset is a long audio file with multiple speakers, use `svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`). Further manual classification may be necessary due to accuracy issues. If speakers speak with a variety of speech styles, set --min-speakers larger than the actual number of speakers. Due to unresolved dependencies, please install `pyannote.audio` manually: `pip install pyannote-audio`.
 
 [^1]: https://ytpmv.info/how-to-use-uvr/
 
 #### Cloud
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-vits-svc-fork-4.0.ipynb)
 [![Open In Paperspace](https://img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://console.paperspace.com/github/34j/so-vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.1.7 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.1.8 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -69,17 +69,17 @@
 inference, if there is noise on the inputs, the HuBERT model will react to
 those as well. Consider using realtime noise reduction applications such as
 [RTX Voice](https://www.nvidia.com/en-us/geforce/guides/nvidia-rtx-voice-setup-
 guide/) in this case. ### Training #### Before training - If your dataset has
 BGM, please remove the BGM using software such as [Ultimate Vocal Remover]
 (https://ultimatevocalremover.com/). `3_HP-Vocal-UVR.pth` or `UVR-MDX-NET Main`
 is recommended. [^1] - If your dataset is a long audio file with a single
-speaker, use `svc split` to split the dataset into multiple files (using
+speaker, use `svc pre-split` to split the dataset into multiple files (using
 `librosa`). - If your dataset is a long audio file with multiple speakers, use
-`svc sd` to split the dataset into multiple files (using `pyannote.audio`).
+`svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`).
 Further manual classification may be necessary due to accuracy issues. If
 speakers speak with a variety of speech styles, set --min-speakers larger than
 the actual number of speakers. Due to unresolved dependencies, please install
 `pyannote.audio` manually: `pip install pyannote-audio`. [^1]: https://
 ytpmv.info/how-to-use-uvr/ #### Cloud [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-
```

