# Comparing `tmp/audioldm-0.0.9.tar.gz` & `tmp/audioldm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioldm-0.0.9.tar", last modified: Fri Feb 17 21:35:36 2023, max compression
+gzip compressed data, was "audioldm-0.1.0.tar", last modified: Mon Apr 10 13:47:09 2023, max compression
```

## Comparing `audioldm-0.0.9.tar` & `audioldm-0.1.0.tar`

### file list

```diff
@@ -1,104 +1,103 @@
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.492013 audioldm-0.0.9/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    15035 2023-02-03 10:13:09.000000 audioldm-0.0.9/LICENSE
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       86 2023-02-04 20:47:44.000000 audioldm-0.0.9/MANIFEST.in
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     7463 2023-02-17 21:35:36.487522 audioldm-0.0.9/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6814 2023-02-17 21:34:03.000000 audioldm-0.0.9/README.md
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    12321 2023-02-17 21:32:26.000000 audioldm-0.0.9/app.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.375569 audioldm-0.0.9/audioldm/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      834 2023-02-15 12:05:10.000000 audioldm-0.0.9/audioldm/__init__.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3986 2023-02-17 21:34:51.000000 audioldm-0.0.9/audioldm/__main__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.388964 audioldm-0.0.9/audioldm/audio/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       63 2023-02-15 12:05:10.000000 audioldm-0.0.9/audioldm/audio/__init__.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     2642 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/audio/audio_processing.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6374 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/audio/stft.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     2642 2023-02-15 12:05:10.000000 audioldm-0.0.9/audioldm/audio/tools.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.393919 audioldm-0.0.9/audioldm/clap/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/__init__.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6293 2023-02-05 13:14:28.000000 audioldm-0.0.9/audioldm/clap/encoders.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.418280 audioldm-0.0.9/audioldm/clap/open_clip/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      639 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/__init__.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     1220 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/bert.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    11000 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/factory.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     7177 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/feature_fusion.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    48104 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/htsat.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     2243 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/linear_probe.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    16143 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/loss.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    33147 2023-02-02 20:01:51.000000 audioldm-0.0.9/audioldm/clap/open_clip/model.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.443720 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/HTSAT-base.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      498 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/HTSAT-large.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/HTSAT-tiny.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/PANN-10.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/PANN-14-win-1536.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/PANN-14.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      495 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/PANN-6.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      388 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/RN101-quickgelu.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/RN101.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      389 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/RN50-quickgelu.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/RN50.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/RN50x16.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/RN50x4.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/ViT-B-16.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      318 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/ViT-B-32.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      296 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/model_configs/ViT-L-14.json
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     5023 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/openai.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    23398 2023-02-02 20:01:50.000000 audioldm-0.0.9/audioldm/clap/open_clip/pann_model.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6440 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/pretrained.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4337 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/timm_model.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6400 2023-02-15 12:05:10.000000 audioldm-0.0.9/audioldm/clap/open_clip/tokenizer.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     1051 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/transform.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    12103 2023-02-02 20:01:50.000000 audioldm-0.0.9/audioldm/clap/open_clip/utils.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       22 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/open_clip/version.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.465464 audioldm-0.0.9/audioldm/clap/training/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/__init__.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    84448 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/audioset_textmap.npy
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    34417 2023-02-02 20:01:50.000000 audioldm-0.0.9/audioldm/clap/training/data.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     5165 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/distributed.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    22199 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/imagenet_zeroshot_data.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3208 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/infer_demo.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      943 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/logger.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    25459 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/lp_main.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    10607 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/lp_train.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    22551 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/main.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    17202 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/params.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      661 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/scheduler.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    36331 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/train.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3429 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/clap/training/zero_shot.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.470616 audioldm-0.0.9/audioldm/hifigan/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      180 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/hifigan/__init__.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     5524 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/hifigan/models.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     2110 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/hifigan/utilities.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.482797 audioldm-0.0.9/audioldm/latent_diffusion/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/latent_diffusion/__init__.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    15343 2023-02-02 20:01:50.000000 audioldm-0.0.9/audioldm/latent_diffusion/attention.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    13593 2023-02-02 20:01:50.000000 audioldm-0.0.9/audioldm/latent_diffusion/ddim.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    16399 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/latent_diffusion/ddpm.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3066 2023-02-02 20:01:50.000000 audioldm-0.0.9/audioldm/latent_diffusion/ema.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    39155 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/latent_diffusion/openaimodel.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     9863 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/latent_diffusion/util.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    24044 2023-02-04 20:50:49.000000 audioldm-0.0.9/audioldm/ldm.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     5489 2023-02-15 12:05:10.000000 audioldm-0.0.9/audioldm/pipeline.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     5844 2023-02-15 12:05:10.000000 audioldm-0.0.9/audioldm/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.484506 audioldm-0.0.9/audioldm/variational_autoencoder/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/variational_autoencoder/__init__.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3132 2023-02-02 20:01:50.000000 audioldm-0.0.9/audioldm/variational_autoencoder/autoencoder.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3097 2023-02-02 18:45:00.000000 audioldm-0.0.9/audioldm/variational_autoencoder/distributions.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    34390 2023-02-02 20:01:51.000000 audioldm-0.0.9/audioldm/variational_autoencoder/modules.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.381788 audioldm-0.0.9/audioldm.egg-info/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     7463 2023-02-17 21:35:36.000000 audioldm-0.0.9/audioldm.egg-info/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3319 2023-02-17 21:35:36.000000 audioldm-0.0.9/audioldm.egg-info/SOURCES.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        1 2023-02-17 21:35:36.000000 audioldm-0.0.9/audioldm.egg-info/dependency_links.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      155 2023-02-17 21:35:36.000000 audioldm-0.0.9/audioldm.egg-info/requires.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        9 2023-02-17 21:35:36.000000 audioldm-0.0.9/audioldm.egg-info/top_level.txt
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-02-17 21:35:36.490342 audioldm-0.0.9/bin/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3986 2023-02-15 12:20:06.000000 audioldm-0.0.9/bin/audioldm
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       31 2023-02-04 20:09:26.000000 audioldm-0.0.9/bin/audioldm.cmd
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      470 2023-02-06 20:56:29.000000 audioldm-0.0.9/check.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       38 2023-02-17 21:35:36.488465 audioldm-0.0.9/setup.cfg
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4462 2023-02-17 21:35:24.000000 audioldm-0.0.9/setup.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.317385 audioldm-0.1.0/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    15035 2023-04-10 06:44:17.000000 audioldm-0.1.0/LICENSE
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)       86 2023-04-10 06:44:17.000000 audioldm-0.1.0/MANIFEST.in
+-rw-r--r--   0 tiger     (1000) tiger     (1000)    10920 2023-04-10 13:47:09.314005 audioldm-0.1.0/PKG-INFO
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    10271 2023-04-10 08:05:27.000000 audioldm-0.1.0/README.md
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    13173 2023-04-10 07:11:35.000000 audioldm-0.1.0/app.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.636739 audioldm-0.1.0/audioldm/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      132 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/__init__.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     4751 2023-04-10 07:14:59.000000 audioldm-0.1.0/audioldm/__main__.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.707851 audioldm-0.1.0/audioldm/audio/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)       78 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/audio/__init__.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     2642 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/audio/audio_processing.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     6374 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/audio/stft.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     2759 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/audio/tools.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.718051 audioldm-0.1.0/audioldm/clap/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)        0 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/__init__.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     6318 2023-04-10 07:02:06.000000 audioldm-0.1.0/audioldm/clap/encoders.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.925058 audioldm-0.1.0/audioldm/clap/open_clip/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      639 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/__init__.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     1220 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/bert.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)  1356917 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    11070 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/factory.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     7177 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/feature_fusion.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    48104 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/htsat.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     2243 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/linear_probe.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    16143 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/loss.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    33147 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.100740 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/HTSAT-base.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      498 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/HTSAT-large.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      496 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      496 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/HTSAT-tiny.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-10.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      496 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      496 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      495 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-6.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      388 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN101-quickgelu.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      364 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN101.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      389 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN50-quickgelu.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      364 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN50.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      365 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN50x16.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      365 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN50x4.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      294 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/ViT-B-16.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      318 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      294 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/ViT-B-32.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      296 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/ViT-L-14.json
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     5085 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/openai.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    23398 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/pann_model.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     6501 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/pretrained.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     4337 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/timm_model.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     6400 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/tokenizer.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     1051 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/transform.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    12103 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/utils.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)       22 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/version.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.206260 audioldm-0.1.0/audioldm/clap/training/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)        0 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/__init__.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    84448 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/audioset_textmap.npy
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    34417 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/data.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     5165 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/distributed.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    22199 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/imagenet_zeroshot_data.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3208 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/infer_demo.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      943 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/logger.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    25459 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/lp_main.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    10607 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/lp_train.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    22551 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/main.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    17283 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/params.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      661 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/scheduler.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    36331 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/train.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3429 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/zero_shot.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.229407 audioldm-0.1.0/audioldm/hifigan/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)      180 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/hifigan/__init__.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     5524 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/hifigan/models.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     2110 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/hifigan/utilities.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.272894 audioldm-0.1.0/audioldm/latent_diffusion/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)        0 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/__init__.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    15343 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/attention.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    13593 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/ddim.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    16399 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/ddpm.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3066 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/ema.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    39155 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/openaimodel.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     9863 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/util.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    28164 2023-04-10 06:45:17.000000 audioldm-0.1.0/audioldm/ldm.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    10650 2023-04-10 06:58:19.000000 audioldm-0.1.0/audioldm/pipeline.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     9803 2023-04-10 13:43:23.000000 audioldm-0.1.0/audioldm/utils.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.297363 audioldm-0.1.0/audioldm/variational_autoencoder/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)        0 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/variational_autoencoder/__init__.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3132 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/variational_autoencoder/autoencoder.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3097 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/variational_autoencoder/distributions.py
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)    34390 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/variational_autoencoder/modules.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.663418 audioldm-0.1.0/audioldm.egg-info/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)    10920 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3310 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      189 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/requires.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        9 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/top_level.txt
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.310793 audioldm-0.1.0/bin/
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     4751 2023-04-10 07:23:00.000000 audioldm-0.1.0/bin/audioldm
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)       31 2023-04-10 06:44:17.000000 audioldm-0.1.0/bin/audioldm.cmd
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-04-10 13:47:09.317005 audioldm-0.1.0/setup.cfg
+-rwxrwxrwx   0 tiger     (1000) tiger     (1000)     4510 2023-04-10 08:01:38.000000 audioldm-0.1.0/setup.py
```

### Comparing `audioldm-0.0.9/LICENSE` & `audioldm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/PKG-INFO` & `audioldm-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,163 @@
-Metadata-Version: 2.1
-Name: audioldm
-Version: 0.0.9
-Summary: This package is written for text-to-audio generation.
-Home-page: https://github.com/haoheliu/audioldm
-Author: Haohe Liu
-Author-email: haoheliu@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# :sound: Audio Generation with AudioLDM
 
+[![arXiv](https://img.shields.io/badge/arXiv-2301.12503-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2301.12503)  [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://audioldm.github.io/)  [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/haoheliu/audioldm-text-to-audio-generation)  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/olaviinha/NeuralTextToAudio/blob/main/AudioLDM_pub.ipynb?force_theme=dark)  [![Replicate](https://replicate.com/jagilley/audio-ldm/badge)](https://replicate.com/jagilley/audio-ldm)
 
-# Text-to-Audio Generation
+<!-- # [![PyPI version](https://badge.fury.io/py/voicefixer.svg)](https://badge.fury.io/py/voicefixer) -->
 
-[![arXiv](https://img.shields.io/badge/arXiv-2109.13731-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2301.12503)  [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://audioldm.github.io/)  [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/haoheliu/audioldm-text-to-audio-generation)  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/olaviinha/NeuralTextToAudio/blob/main/AudioLDM_pub.ipynb?force_theme=dark)  [![Replicate](https://replicate.com/jagilley/audio-ldm/badge)](https://replicate.com/jagilley/audio-ldm)
+**Generate speech, sound effects, music and beyond.**
 
-<!-- # [![PyPI version](https://badge.fury.io/py/voicefixer.svg)](https://badge.fury.io/py/voicefixer) -->
+This repo currently support: 
 
-Generate speech, sound effects, music and beyond.
+- **Text-to-Audio Generation**: Generate audio given text input.
+- **Audio-to-Audio Generation**: Given an audio, generate another audio that contain the same type of sound. 
+- **Text-guided Audio-to-Audio Style Transfer**: Transfer the sound of an audio into another one using the text description.
 
 <hr>
 
 ## Important tricks to make your generated audio sound better
-1. Try to use more adjectives to describe your sound. For example: "A man is speaking clearly and slowly in a professional studio" is better than "A man is speaking". This can make sure AudioLDM understand what you want.
+1. Try to provide more hints to AudioLDM, such as using more adjectives to describe your sound (e.g., clearly, high quality) or make your target more specific (e.g., "water stream in a forest" instead of "stream"). This can make sure AudioLDM understand what you want. 
 2. Try to use different random seeds, which can affect the generation quality significantly sometimes.
-3. It's best to use general terms like 'man' or 'woman' instead of specific names for individuals or abstract objects that humans may not be familiar with, such as 'mummy'.
+3. It's best to use general terms like 'man' or 'woman' instead of specific names for individuals or abstract objects that humans may not be familiar with.
 
 # Change Log
 
+**2023-04-10**: Try to finetune AudioLDM with MusicCaps and AudioCaps datasets. Add three more checkpoints, including audioldm-m-text-ft, audioldm-s-text-ft, and audioldm-m-full.
+
+**2023-03-04**: Add two more checkpoints, one is small model with more training steps, another is a large model. Add model selection in the Gradio APP.
+
+**2023-02-24**: Add audio-to-audio generation. Add test cases. Add a pipeline (python function) for audio super-resolution and inpainting.
+
 **2023-02-15**: Add audio style transfer. Add more options on generation.
 
 ## Web APP
+
+The web APP currently only support Text-to-Audio generation. For full functionality please refer to the [Commandline Usage](https://github.com/haoheliu/AudioLDM#commandline-usage).
+
 1. Prepare running environment
 ```shell
 conda create -n audioldm python=3.8; conda activate audioldm
-pip3 install audioldm==0.0.8
+pip3 install audioldm
 git clone https://github.com/haoheliu/AudioLDM; cd AudioLDM
 ```
 2. Start the web application (powered by Gradio)
 ```shell
 python3 app.py
 ```
 3. A link will be printed out. Click the link to open the browser and play.
 
 ## Commandline Usage
-1. Prepare running environment
+Prepare running environment
 ```shell
 # Optional
 conda create -n audioldm python=3.8; conda activate audioldm
 # Install AudioLDM
-pip3 install audioldm==0.0.8
+pip3 install audioldm
 ```
 
-2. text-to-audio generation
-```python
-# Test run
-audioldm -t "A hammer is hitting a wooden surface" # The default --mode is "generation"
+:star2: **Text-to-Audio Generation**: generate an audio guided by a text
+```shell
+# The default --mode is "generation"
+audioldm -t "A hammer is hitting a wooden surface" 
+# Result will be saved in "./output/generation"
+```
+
+:star2: **Audio-to-Audio Generation**: generate an audio guided by an audio (output will have similar audio events as the input audio file).
+```shell
+audioldm --file_path trumpet.wav
+# Result will be saved in "./output/generation_audio_to_audio/trumpet"
 ```
 
-3. audio-to-audio style transfer
-```python
+:star2: **Text-guided Audio-to-Audio Style Transfer**
+```shell
 # Test run
 # --file_path is the original audio file for transfer
 # -t is the text AudioLDM uses for transfer. 
 # Please make sure that --file_path exist
 audioldm --mode "transfer" --file_path trumpet.wav -t "Children Singing" 
+# Result will be saved in "./output/transfer/trumpet"
 
 # Tune the value of --transfer_strength is important!
 # --transfer_strength: A value between 0 and 1. 0 means original audio without transfer, 1 means completely transfer to the audio indicated by text
 audioldm --mode "transfer" --file_path trumpet.wav -t "Children Singing" --transfer_strength 0.25
 ```
 
-For more options on guidance scale, batchsize, seed, ddim steps, etc., please run
+:gear: How to choose between different model checkpoints?
+```
+# Add the --model_name parameter, choice={audioldm-m-text-ft, audioldm-s-text-ft, audioldm-m-full, audioldm-s-full,audioldm-l-full,audioldm-s-full-v2}
+audioldm --model_name audioldm-s-full
+```
+- :star: audioldm-m-text-ft (**recommand**, default): the medium large AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
+- :star: audioldm-s-text-ft (**recommand**): the small AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
+- audioldm-m-full: the medium AudioLDM without finetuning and trained with audio embeddings as condition *(added 2023-04-10)*.
+- audioldm-s-full-v2: more training steps comparing with audioldm-s-full *(added 2023-03-04)*.
+- audioldm-l-full: larger model comparing with audioldm-s-full *(added 2023-03-04)*.
+- audioldm-s-full: the original open-sourced version *(added 2023-02-01)*.
+
+:grey_question: For more options on guidance scale, batchsize, seed, ddim steps, etc., please run
 ```shell
 audioldm -h
 ```
-```shell
-usage: audioldm [-h] [--mode {generation,transfer}] [-t TEXT] [-f FILE_PATH] [--transfer_strength TRANSFER_STRENGTH] [-s SAVE_PATH] [-ckpt CKPT_PATH] [-b BATCHSIZE] [--ddim_steps DDIM_STEPS] [-gs GUIDANCE_SCALE]
-                [-dur DURATION] [-n N_CANDIDATE_GEN_PER_TEXT] [--seed SEED]
+```console
+usage: audioldm [-h] [--mode {generation,transfer}] [-t TEXT] [-f FILE_PATH] [--transfer_strength TRANSFER_STRENGTH] [-s SAVE_PATH] [--model_name {audioldm-s-full,audioldm-l-full,audioldm-s-full-v2}] [-ckpt CKPT_PATH]
+                [-b BATCHSIZE] [--ddim_steps DDIM_STEPS] [-gs GUIDANCE_SCALE] [-dur DURATION] [-n N_CANDIDATE_GEN_PER_TEXT] [--seed SEED]
 
 optional arguments:
   -h, --help            show this help message and exit
   --mode {generation,transfer}
                         generation: text-to-audio generation; transfer: style transfer
-  -t TEXT, --text TEXT  Text prompt to the model for audio generation
+  -t TEXT, --text TEXT  Text prompt to the model for audio generation, DEFAULT ""
   -f FILE_PATH, --file_path FILE_PATH
-                        Original audio file for style transfer
+                        (--mode transfer): Original audio file for style transfer; Or (--mode generation): the guidance audio file for generating simialr audio, DEFAULT None
   --transfer_strength TRANSFER_STRENGTH
-                        A value between 0 and 1. 0 means original audio without transfer, 1 means completely transfer to the audio indicated by text
+                        A value between 0 and 1. 0 means original audio without transfer, 1 means completely transfer to the audio indicated by text, DEFAULT 0.5
   -s SAVE_PATH, --save_path SAVE_PATH
-                        The path to save model output
+                        The path to save model output, DEFAULT "./output"
+  --model_name {audioldm-s-full,audioldm-l-full,audioldm-s-full-v2}
+                        The checkpoint you gonna use, DEFAULT "audioldm-s-full"
   -ckpt CKPT_PATH, --ckpt_path CKPT_PATH
-                        The path to the pretrained .ckpt model
+                        (deprecated) The path to the pretrained .ckpt model, DEFAULT None
   -b BATCHSIZE, --batchsize BATCHSIZE
-                        Generate how many samples at the same time
+                        Generate how many samples at the same time, DEFAULT 1
   --ddim_steps DDIM_STEPS
-                        The sampling step for DDIM
+                        The sampling step for DDIM, DEFAULT 200
   -gs GUIDANCE_SCALE, --guidance_scale GUIDANCE_SCALE
-                        Guidance scale (Large => better quality and relavancy to text; Small => better diversity)
+                        Guidance scale (Large => better quality and relavancy to text; Small => better diversity), DEFAULT 2.5
   -dur DURATION, --duration DURATION
-                        The duration of the samples
+                        The duration of the samples, DEFAULT 10
   -n N_CANDIDATE_GEN_PER_TEXT, --n_candidate_gen_per_text N_CANDIDATE_GEN_PER_TEXT
-                        Automatic quality control. This number control the number of candidates (e.g., generate three audios and choose the best to show you). A Larger value usually lead to better quality with heavier
-                        computation
-  --seed SEED           Change this value (any integer number) will lead to a different generation result.
+                        Automatic quality control. This number control the number of candidates (e.g., generate three audios and choose the best to show you). A Larger value usually lead to better quality with heavier computation, DEFAULT 3
+  --seed SEED           Change this value (any integer number) will lead to a different generation result. DEFAULT 42
 ```
 
-
-
 For the evaluation of audio generative model, please refer to [audioldm_eval](https://github.com/haoheliu/audioldm_eval).
 
 # Web Demo
 
 Integrated into [Hugging Face Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/haoheliu/audioldm-text-to-audio-generation)
 
+# TuneFlow Demo
+
+Try out AudioLDM as a [TuneFlow](https://tuneflow.com) plugin [![TuneFlow x AudioLDM](https://img.shields.io/badge/TuneFlow-AudioLDM-%23C563E6%20)](https://github.com/tuneflow/AudioLDM). See how it can work in a real DAW (Digital Audio Workstation). 
 
 # TODO
 
-- [ ] Update the checkpoint with more training steps.
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/haoheliuP)
+
+- [x] Update the checkpoint with more training steps.
+- [x] Update the checkpoint with more parameters (audioldm-l).
 - [ ] Add AudioCaps finetuned AudioLDM-S model
 - [x] Build pip installable package for commandline use
 - [x] Build Gradio web application
+- [ ] Add super-resolution, inpainting into Gradio web application
+- [ ] Add style-transfer into Gradio web application
 - [x] Add text-guided style transfer
-- [ ] Add audio super-resolution
-- [ ] Add audio inpainting
+- [x] Add audio-to-audio generation
+- [x] Add audio super-resolution
+- [x] Add audio inpainting
 
 ## Cite this work
 
 If you found this tool useful, please consider citing
 ```bibtex
 @article{liu2023audioldm,
   title={AudioLDM: Text-to-Audio Generation with Latent Diffusion Models},
```

### Comparing `audioldm-0.0.9/app.py` & `audioldm-0.1.0/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import numpy as np
 from audioldm import text_to_audio, build_model
 
 # from share_btn import community_icon_html, loading_icon_html, share_js
 
 model_id = "haoheliu/AudioLDM-S-Full"
 
-audioldm = build_model()
+audioldm = None
+current_model_name = None
 # audioldm=None
 
 # def predict(input, history=[]):
 #     # tokenize the new input sentence
 #     new_user_input_ids = tokenizer.encode(input + tokenizer.eos_token, return_tensors='pt')
 
 #     # append the new user input tokens to the chat history
@@ -20,21 +21,26 @@
 #     history = model.generate(bot_input_ids, max_length=1000, pad_token_id=tokenizer.eos_token_id).tolist()
 
 #     # convert the tokens to text, and then split the responses into lines
 #     response = tokenizer.decode(history[0]).split("<|endoftext|>")
 #     response = [(response[i], response[i+1]) for i in range(0, len(response)-1, 2)]  # convert to tuples of list
 #     return response, history
 
-
-def text2audio(text, duration, guidance_scale, random_seed, n_candidates):
+def text2audio(text, duration, guidance_scale, random_seed, n_candidates, model_name):
+    global audioldm, current_model_name
+    
+    if audioldm is None or model_name != current_model_name:
+        audioldm=build_model(model_name=model_name)
+        current_model_name = model_name
+        
     # print(text, length, guidance_scale)
     waveform = text_to_audio(
-        audioldm,
-        text,
-        random_seed,
+        latent_diffusion=audioldm,
+        text=text,
+        seed=random_seed,
         duration=duration,
         guidance_scale=guidance_scale,
         n_candidate_gen_per_text=int(n_candidates),
     )  # [bs, 1, samples]
     waveform = [
         gr.make_waveform((16000, wave[0]), bg_image="bg.png") for wave in waveform
     ]
@@ -243,14 +249,17 @@
                 n_candidates = gr.Slider(
                     1,
                     5,
                     value=3,
                     step=1,
                     label="Automatic quality control. This number control the number of candidates (e.g., generate three audios and choose the best to show you). A Larger value usually lead to better quality with heavier computation",
                 )
+                model_name = gr.Dropdown(
+                    ["audioldm-s-full", "audioldm-l-full", "audioldm-s-full-v2","audioldm-m-text-ft", "audioldm-s-text-ft", "audioldm-m-full"], value="audioldm-m-text-ft", label="Choose the model to use. audioldm-m-text-ft and audioldm-s-text-ft are recommanded. -s- means small, -m- means medium and -l- means large",
+                )
             ############# Output
             # outputs=gr.Audio(label="Output", type="numpy")
             outputs = gr.Video(label="Output", elem_id="output-video")
 
             # with gr.Group(elem_id="container-advanced-btns"):
             #   # advanced_button = gr.Button("Advanced options", elem_id="advanced-btn")
             #   with gr.Group(elem_id="share-btn-container"):
@@ -263,15 +272,15 @@
         # with gr.Group(elem_id="share-btn-container", visible=False):
         #     community_icon = gr.HTML(community_icon_html)
         #     loading_icon = gr.HTML(loading_icon_html)
         #     share_button = gr.Button("Share to community", elem_id="share-btn")
 
         btn.click(
             text2audio,
-            inputs=[textbox, duration, guidance_scale, seed, n_candidates],
+            inputs=[textbox, duration, guidance_scale, seed, n_candidates, model_name],
             outputs=[outputs],
         )
 
         # share_button.click(None, [], [], _js=share_js)
         gr.HTML(
             """
         <div class="footer" style="text-align: center; max-width: 700px; margin: 0 auto;">
@@ -279,39 +288,41 @@
                     </p>
                     <br>
                     <p>Model by <a href="https://twitter.com/LiuHaohe" style="text-decoration: underline;" target="_blank">Haohe Liu</a></p>
                     <br>
         </div>
         """
         )
-        gr.Examples(
-            [
-                ["A hammer is hitting a wooden surface", 5, 2.5, 45, 3],
-                [
-                    "Peaceful and calming ambient music with singing bowl and other instruments.",
-                    5,
-                    2.5,
-                    45,
-                    3,
-                ],
-                ["A man is speaking in a small room.", 5, 2.5, 45, 3],
-                ["A female is speaking followed by footstep sound", 5, 2.5, 45, 3],
-                [
-                    "Wooden table tapping sound followed by water pouring sound.",
-                    5,
-                    2.5,
-                    45,
-                    3,
-                ],
-            ],
-            fn=text2audio,
-            inputs=[textbox, duration, guidance_scale, seed, n_candidates],
-            outputs=[outputs],
-            cache_examples=True,
-        )
+        # gr.Examples(
+        #     [
+        #         ["A hammer is hitting a wooden surface", 5, 2.5, 45, 3, "audioldm-s-full"],
+        #         [
+        #             "Peaceful and calming ambient music with singing bowl and other instruments.",
+        #             5,
+        #             2.5,
+        #             45,
+        #             3,
+        #             "audioldm-s-full"
+        #         ],
+        #         ["A man is speaking in a small room.", 5, 2.5, 45, 3, "audioldm-s-full"],
+        #         ["A female is speaking followed by footstep sound", 5, 2.5, 45, 3, "audioldm-s-full"],
+        #         [
+        #             "Wooden table tapping sound followed by water pouring sound.",
+        #             5,
+        #             2.5,
+        #             45,
+        #             3,
+        #             "audioldm-s-full"
+        #         ],
+        #     ],
+        #     fn=text2audio,
+        #     inputs=[textbox, duration, guidance_scale, seed, n_candidates, model_name],
+        #     outputs=[outputs],
+        #     cache_examples=True,
+        # )
         with gr.Accordion("Additional information", open=False):
             gr.HTML(
                 """
                 <div class="acknowledgments">
                     <p> We build the model with data from <a href="http://research.google.com/audioset/">AudioSet</a>, <a href="https://freesound.org/">Freesound</a> and <a href="https://sound-effects.bbcrewind.co.uk/">BBC Sound Effect library</a>. We share this demo based on the <a href="https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/375954/Research.pdf">UK copyright exception</a> of data for academic research. </p>
                             </div>
                         """
```

### Comparing `audioldm-0.0.9/audioldm/__main__.py` & `audioldm-0.1.0/audioldm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/usr/bin/python3
 import os
-from audioldm import text_to_audio, style_transfer, build_model, save_wave, get_time
+from audioldm import text_to_audio, style_transfer, build_model, save_wave, get_time, round_up_duration, get_duration
 import argparse
 
+CACHE_DIR = os.getenv(
+    "AUDIOLDM_CACHE_DIR",
+    os.path.join(os.path.expanduser("~"), ".cache/audioldm"))
+
 parser = argparse.ArgumentParser()
 
 parser.add_argument(
     "--mode",
     type=str,
     required=False,
     default="generation",
@@ -15,25 +19,25 @@
 )
 
 parser.add_argument(
     "-t",
     "--text",
     type=str,
     required=False,
-    default="A hammer is hitting a wooden surface",
+    default="",
     help="Text prompt to the model for audio generation",
 )
 
 parser.add_argument(
     "-f",
     "--file_path",
     type=str,
     required=False,
     default=None,
-    help="Original audio file for style transfer",
+    help="(--mode transfer): Original audio file for style transfer; Or (--mode generation): the guidance audio file for generating simialr audio",
 )
 
 parser.add_argument(
     "--transfer_strength",
     type=float,
     required=False,
     default=0.5,
@@ -46,23 +50,29 @@
     type=str,
     required=False,
     help="The path to save model output",
     default="./output",
 )
 
 parser.add_argument(
+    "--model_name",
+    type=str,
+    required=False,
+    help="The checkpoint you gonna use",
+    default="audioldm-m-text-ft",
+    choices=["audioldm-s-full", "audioldm-l-full", "audioldm-s-full-v2","audioldm-m-text-ft", "audioldm-s-text-ft", "audioldm-m-full"]
+)
+
+parser.add_argument(
     "-ckpt",
     "--ckpt_path",
     type=str,
     required=False,
     help="The path to the pretrained .ckpt model",
-    default=os.path.join(
-                os.path.expanduser("~"),
-                ".cache/audioldm/audioldm-s-full.ckpt",
-            ),
+    default=None,
 )
 
 parser.add_argument(
     "-b",
     "--batchsize",
     type=int,
     required=False,
@@ -74,15 +84,14 @@
     "--ddim_steps",
     type=int,
     required=False,
     default=200,
     help="The sampling step for DDIM",
 )
 
-
 parser.add_argument(
     "-gs",
     "--guidance_scale",
     type=float,
     required=False,
     default=2.5,
     help="Guidance scale (Large => better quality and relavancy to text; Small => better diversity)",
@@ -111,39 +120,54 @@
     type=int,
     required=False,
     default=42,
     help="Change this value (any integer number) will lead to a different generation result.",
 )
 
 args = parser.parse_args()
+
+if(args.ckpt_path is not None):
+    print("Warning: ckpt_path has no effect after version 0.0.20.")
+    
 assert args.duration % 2.5 == 0, "Duration must be a multiple of 2.5"
-save_path = os.path.join(args.save_path, args.mode)
+
+mode = args.mode
+if(mode == "generation" and args.file_path is not None):
+    mode = "generation_audio_to_audio"
+    if(len(args.text) > 0):
+        print("Warning: You have specified the --file_path. --text will be ignored")
+        args.text = ""
+        
+save_path = os.path.join(args.save_path, mode)
+
 if(args.file_path is not None):
     save_path = os.path.join(save_path, os.path.basename(args.file_path.split(".")[0]))
 
 text = args.text
 random_seed = args.seed
 duration = args.duration
 guidance_scale = args.guidance_scale
 n_candidate_gen_per_text = args.n_candidate_gen_per_text
 
 os.makedirs(save_path, exist_ok=True)
-audioldm = build_model(ckpt_path=args.ckpt_path)
+audioldm = build_model(model_name=args.model_name)
 
 if(args.mode == "generation"):
     waveform = text_to_audio(
         audioldm,
         text,
+        args.file_path,
         random_seed,
         duration=duration,
         guidance_scale=guidance_scale,
         ddim_steps=args.ddim_steps,
         n_candidate_gen_per_text=n_candidate_gen_per_text,
         batchsize=args.batchsize,
     )
+    
 elif(args.mode == "transfer"):
     assert args.file_path is not None
     assert os.path.exists(args.file_path), "The original audio file \'%s\' for style transfer does not exist." % args.file_path
     waveform = style_transfer(
         audioldm,
         text,
         args.file_path,
```

### Comparing `audioldm-0.0.9/audioldm/audio/audio_processing.py` & `audioldm-0.1.0/audioldm/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/audio/stft.py` & `audioldm-0.1.0/audioldm/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/audio/tools.py` & `audioldm-0.1.0/audioldm/audio/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,46 +30,50 @@
 
     return fbank
 
 
 def pad_wav(waveform, segment_length):
     waveform_length = waveform.shape[-1]
     assert waveform_length > 100, "Waveform is too short, %s" % waveform_length
-    if waveform_length == segment_length:
+    if segment_length is None or waveform_length == segment_length:
         return waveform
     elif waveform_length > segment_length:
         return waveform[:segment_length]
     elif waveform_length < segment_length:
         temp_wav = np.zeros((1, segment_length))
         temp_wav[:, :waveform_length] = waveform
     return temp_wav
 
-
 def normalize_wav(waveform):
     waveform = waveform - np.mean(waveform)
     waveform = waveform / (np.max(np.abs(waveform)) + 1e-8)
     return waveform * 0.5
 
 
 def read_wav_file(filename, segment_length):
     # waveform, sr = librosa.load(filename, sr=None, mono=True) # 4 times slower
     waveform, sr = torchaudio.load(filename)  # Faster!!!
     waveform = torchaudio.functional.resample(waveform, orig_freq=sr, new_freq=16000)
     waveform = waveform.numpy()[0, ...]
     waveform = normalize_wav(waveform)
     waveform = waveform[None, ...]
     waveform = pad_wav(waveform, segment_length)
+    
+    waveform = waveform / np.max(np.abs(waveform))
+    waveform = 0.5 * waveform
+    
     return waveform
 
 
 def wav_to_fbank(filename, target_length=1024, fn_STFT=None):
     assert fn_STFT is not None
 
     # mixup
     waveform = read_wav_file(filename, target_length * 160)  # hop size is 160
+
     waveform = waveform[0, ...]
     waveform = torch.FloatTensor(waveform)
 
     fbank, log_magnitudes_stft, energy = get_mel_from_wav(waveform, fn_STFT)
 
     fbank = torch.FloatTensor(fbank.T)
     log_magnitudes_stft = torch.FloatTensor(log_magnitudes_stft.T)
```

### Comparing `audioldm-0.0.9/audioldm/clap/encoders.py` & `audioldm-0.1.0/audioldm/clap/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 class CLAPAudioEmbeddingClassifierFreev2(nn.Module):
     def __init__(
         self,
         pretrained_path="",
         key="class",
         sampling_rate=16000,
         embed_mode="audio",
+        amodel = "HTSAT-tiny",
         unconditional_prob=0.1,
         random_mute=False,
         max_random_mute_portion=0.5,
         training_mode=True,
     ):
         super().__init__()
 
         self.key = key
         self.device = "cpu"
         self.precision = "fp32"
-        self.amodel = "HTSAT-tiny"  # or 'PANN-14'
+        self.amodel = amodel  # or 'PANN-14'
         self.tmodel = "roberta"  # the best text encoder in our training
         self.enable_fusion = False  # False if you do not want to use the fusion model
         self.fusion_type = "aff_2d"
         self.pretrained = pretrained_path
         self.embed_mode = embed_mode
         self.embed_mode_orig = embed_mode
         self.sampling_rate = sampling_rate
```

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/__init__.py` & `audioldm-0.1.0/audioldm/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/bert.py` & `audioldm-0.1.0/audioldm/clap/open_clip/bert.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audioldm-0.1.0/audioldm/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/factory.py` & `audioldm-0.1.0/audioldm/clap/open_clip/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from .model import CLAP, convert_weights_to_fp16
 from .openai import load_openai_model
 from .pretrained import get_pretrained_url, download_pretrained
 from .transform import image_transform
 
 _MODEL_CONFIG_PATHS = [Path(__file__).parent / f"model_configs/"]
 _MODEL_CONFIGS = {}  # directory (model_name: config) of model architecture configs
+CACHE_DIR = os.getenv("AUDIOLDM_CACHE_DIR", "~/.cache/audioldm")
+
 
 
 def _natural_key(string_):
     return [int(s) if s.isdigit() else s for s in re.split(r"(\d+)", string_.lower())]
 
 
 def _rescan_model_configs():
@@ -71,15 +73,15 @@
     amodel_name: str,
     tmodel_name: str,
     pretrained: str = "",
     precision: str = "fp32",
     device: torch.device = torch.device("cpu"),
     jit: bool = False,
     force_quick_gelu: bool = False,
-    openai_model_cache_dir: str = os.path.expanduser("~/.cache/clip"),
+    openai_model_cache_dir: str = os.path.expanduser(f"{CACHE_DIR}/clip"),
     skip_params=True,
     pretrained_audio: str = "",
     pretrained_text: str = "",
     enable_fusion: bool = False,
     fusion_type: str = "None"
     # pretrained_image: bool = False,
 ):
```

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/feature_fusion.py` & `audioldm-0.1.0/audioldm/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/htsat.py` & `audioldm-0.1.0/audioldm/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/linear_probe.py` & `audioldm-0.1.0/audioldm/clap/open_clip/linear_probe.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/loss.py` & `audioldm-0.1.0/audioldm/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/model.py` & `audioldm-0.1.0/audioldm/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/openai.py` & `audioldm-0.1.0/audioldm/clap/open_clip/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,29 @@
     get_pretrained_url,
     list_pretrained_tag_models,
     download_pretrained,
 )
 
 __all__ = ["list_openai_models", "load_openai_model"]
 
+CACHE_DIR = os.getenv("AUDIOLDM_CACHE_DIR", "~/.cache")
+
+
 
 def list_openai_models() -> List[str]:
     """Returns the names of available CLIP models"""
     return list_pretrained_tag_models("openai")
 
 
 def load_openai_model(
     name: str,
     model_cfg,
     device: Union[str, torch.device] = "cuda" if torch.cuda.is_available() else "cpu",
     jit=True,
-    cache_dir=os.path.expanduser("~/.cache/clip"),
+    cache_dir=os.path.expanduser(f"{CACHE_DIR}/clip"),
     enable_fusion: bool = False,
     fusion_type: str = "None",
 ):
     """Load a CLIP model, preserve its text pretrained part, and set in the CLAP model
 
     Parameters
     ----------
```

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/pann_model.py` & `audioldm-0.1.0/audioldm/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/pretrained.py` & `audioldm-0.1.0/audioldm/clap/open_clip/pretrained.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import hashlib
 import os
 import urllib
 import warnings
 
 from tqdm import tqdm
 
+CACHE_DIR = os.getenv("AUDIOLDM_CACHE_DIR", "~/.cache")
+
 _RN50 = dict(
     openai="https://openaipublic.azureedge.net/clip/models/afeb0e10f9e5a86da6080e35cf09123aca3b358a0c3e3b6c78a7b63bc04b6762/RN50.pt",
     yfcc15m="https://github.com/mlfoundations/open_clip/releases/download/v0.2-weights/rn50-quickgelu-yfcc15m-455df137.pt",
     cc12m="https://github.com/mlfoundations/open_clip/releases/download/v0.2-weights/rn50-quickgelu-cc12m-f000538c.pt",
 )
 
 _RN50_quickgelu = dict(
@@ -108,15 +110,15 @@
         return ""
     model_pretrained = _PRETRAINED[model]
     if tag not in model_pretrained:
         return ""
     return model_pretrained[tag]
 
 
-def download_pretrained(url: str, root: str = os.path.expanduser("~/.cache/clip")):
+def download_pretrained(url: str, root: str = os.path.expanduser(f"{CACHE_DIR}/clip")):
     os.makedirs(root, exist_ok=True)
     filename = os.path.basename(url)
 
     if "openaipublic" in url:
         expected_sha256 = url.split("/")[-2]
     else:
         expected_sha256 = ""
```

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/timm_model.py` & `audioldm-0.1.0/audioldm/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/tokenizer.py` & `audioldm-0.1.0/audioldm/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/transform.py` & `audioldm-0.1.0/audioldm/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/open_clip/utils.py` & `audioldm-0.1.0/audioldm/clap/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/audioset_textmap.npy` & `audioldm-0.1.0/audioldm/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/data.py` & `audioldm-0.1.0/audioldm/clap/training/data.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/distributed.py` & `audioldm-0.1.0/audioldm/clap/training/distributed.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/imagenet_zeroshot_data.py` & `audioldm-0.1.0/audioldm/clap/training/imagenet_zeroshot_data.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/infer_demo.py` & `audioldm-0.1.0/audioldm/clap/training/infer_demo.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/logger.py` & `audioldm-0.1.0/audioldm/clap/training/logger.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/lp_main.py` & `audioldm-0.1.0/audioldm/clap/training/lp_main.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/lp_train.py` & `audioldm-0.1.0/audioldm/clap/training/lp_train.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/main.py` & `audioldm-0.1.0/audioldm/clap/training/main.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/params.py` & `audioldm-0.1.0/audioldm/clap/training/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 import argparse
+import os
+
+CACHE_DIR = os.getenv(
+    "AUDIOLDM_CACHE_DIR",
+    "~/.cache")
+
 
 
 def get_default_params(model_name):
     # Params from paper (https://arxiv.org/pdf/2103.00020.pdf)
     model_name = model_name.lower()
     if "vit" in model_name:
         return {"lr": 5.0e-4, "beta1": 0.9, "beta2": 0.98, "eps": 1.0e-6}
@@ -422,15 +428,15 @@
         type=str,
         default="_R@10",
         help="The metric for selecting top-k checkpoint.",
     )
     parser.add_argument(
         "--openai-model-cache-dir",
         type=str,
-        default="~/.cache/clip",
+        default=f"{CACHE_DIR}/clip",
         help="Directory to download OpenAI models.",
     )
     parser.add_argument(
         "--optimizer",
         type=str,
         default="adamw",
         help="can be AdamW or SGD",
```

### Comparing `audioldm-0.0.9/audioldm/clap/training/scheduler.py` & `audioldm-0.1.0/audioldm/clap/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/train.py` & `audioldm-0.1.0/audioldm/clap/training/train.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/clap/training/zero_shot.py` & `audioldm-0.1.0/audioldm/clap/training/zero_shot.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/hifigan/models.py` & `audioldm-0.1.0/audioldm/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/hifigan/utilities.py` & `audioldm-0.1.0/audioldm/hifigan/utilities.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/latent_diffusion/attention.py` & `audioldm-0.1.0/audioldm/latent_diffusion/attention.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/latent_diffusion/ddim.py` & `audioldm-0.1.0/audioldm/latent_diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/latent_diffusion/ddpm.py` & `audioldm-0.1.0/audioldm/latent_diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/latent_diffusion/ema.py` & `audioldm-0.1.0/audioldm/latent_diffusion/ema.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/latent_diffusion/openaimodel.py` & `audioldm-0.1.0/audioldm/latent_diffusion/openaimodel.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/latent_diffusion/util.py` & `audioldm-0.1.0/audioldm/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/ldm.py` & `audioldm-0.1.0/audioldm/ldm.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,15 +142,16 @@
             if hasattr(self.cond_stage_model, "encode") and callable(
                 self.cond_stage_model.encode
             ):
                 c = self.cond_stage_model.encode(c)
                 if isinstance(c, DiagonalGaussianDistribution):
                     c = c.mode()
             else:
-                if len(c) == 1:
+                # Text input is list
+                if type(c) == list and len(c) == 1:
                     c = self.cond_stage_model([c[0], c[0]])
                     c = c[0:1]
                 else:
                     c = self.cond_stage_model(c)
         else:
             assert hasattr(self.cond_stage_model, self.cond_stage_forward)
             c = getattr(self.cond_stage_model, self.cond_stage_forward)(c)
@@ -661,14 +662,15 @@
         # print("Waveform save path: ", waveform_save_path)
 
         with self.ema_scope("Generate"):
             for batch in batchs:
                 z, c = self.get_input(
                     batch,
                     self.first_stage_key,
+                    cond_key=self.cond_stage_key,
                     return_first_stage_outputs=False,
                     force_c_encode=True,
                     return_original_cond=False,
                     bs=None,
                 )
                 text = super().get_input(batch, "text")
 
@@ -689,15 +691,18 @@
                     ddim=use_ddim,
                     ddim_steps=ddim_steps,
                     eta=ddim_eta,
                     unconditional_guidance_scale=unconditional_guidance_scale,
                     unconditional_conditioning=unconditional_conditioning,
                     use_plms=use_plms,
                 )
-
+                
+                if(torch.max(torch.abs(samples)) > 1e2):
+                    samples = torch.clip(samples, min=-10, max=10)
+                    
                 mel = self.decode_first_stage(samples)
 
                 waveform = self.mel_spectrogram_to_waveform(mel)
 
                 if waveform.shape[0] > 1:
                     similarity = self.cond_stage_model.cos_similarity(
                         torch.FloatTensor(waveform).squeeze(1), text
@@ -710,7 +715,104 @@
                         best_index.append(i + max_index * z.shape[0])
 
                     waveform = waveform[best_index]
                     # print("Similarity between generated audio and text", similarity)
                     # print("Choose the following indexes:", best_index)
 
         return waveform
+
+    @torch.no_grad()
+    def generate_sample_masked(
+        self,
+        batchs,
+        ddim_steps=200,
+        ddim_eta=1.0,
+        x_T=None,
+        n_candidate_gen_per_text=1,
+        unconditional_guidance_scale=1.0,
+        unconditional_conditioning=None,
+        name="waveform",
+        use_plms=False,
+        time_mask_ratio_start_and_end=(0.25, 0.75),
+        freq_mask_ratio_start_and_end=(0.75, 1.0),
+        save=False,
+        **kwargs,
+    ):
+        # Generate n_candidate_gen_per_text times and select the best
+        # Batch: audio, text, fnames
+        assert x_T is None
+        try:
+            batchs = iter(batchs)
+        except TypeError:
+            raise ValueError("The first input argument should be an iterable object")
+
+        if use_plms:
+            assert ddim_steps is not None
+        use_ddim = ddim_steps is not None
+        # waveform_save_path = os.path.join(self.get_log_dir(), name)
+        # os.makedirs(waveform_save_path, exist_ok=True)
+        # print("Waveform save path: ", waveform_save_path)
+
+        with self.ema_scope("Generate"):
+            for batch in batchs:
+                z, c = self.get_input(
+                    batch,
+                    self.first_stage_key,
+                    cond_key=self.cond_stage_key,
+                    return_first_stage_outputs=False,
+                    force_c_encode=True,
+                    return_original_cond=False,
+                    bs=None,
+                )
+                text = super().get_input(batch, "text")
+                
+                # Generate multiple samples
+                batch_size = z.shape[0] * n_candidate_gen_per_text
+                
+                _, h, w = z.shape[0], z.shape[2], z.shape[3]
+                
+                mask = torch.ones(batch_size, h, w).to(self.device)
+                
+                mask[:, int(h * time_mask_ratio_start_and_end[0]) : int(h * time_mask_ratio_start_and_end[1]), :] = 0 
+                mask[:, :, int(w * freq_mask_ratio_start_and_end[0]) : int(w * freq_mask_ratio_start_and_end[1])] = 0 
+                mask = mask[:, None, ...]
+                
+                c = torch.cat([c] * n_candidate_gen_per_text, dim=0)
+                text = text * n_candidate_gen_per_text
+
+                if unconditional_guidance_scale != 1.0:
+                    unconditional_conditioning = (
+                        self.cond_stage_model.get_unconditional_condition(batch_size)
+                    )
+
+                samples, _ = self.sample_log(
+                    cond=c,
+                    batch_size=batch_size,
+                    x_T=x_T,
+                    ddim=use_ddim,
+                    ddim_steps=ddim_steps,
+                    eta=ddim_eta,
+                    unconditional_guidance_scale=unconditional_guidance_scale,
+                    unconditional_conditioning=unconditional_conditioning,
+                    use_plms=use_plms, mask=mask, x0=torch.cat([z] * n_candidate_gen_per_text)
+                )
+
+                mel = self.decode_first_stage(samples)
+
+                waveform = self.mel_spectrogram_to_waveform(mel)
+
+                if waveform.shape[0] > 1:
+                    similarity = self.cond_stage_model.cos_similarity(
+                        torch.FloatTensor(waveform).squeeze(1), text
+                    )
+
+                    best_index = []
+                    for i in range(z.shape[0]):
+                        candidates = similarity[i :: z.shape[0]]
+                        max_index = torch.argmax(candidates).item()
+                        best_index.append(i + max_index * z.shape[0])
+
+                    waveform = waveform[best_index]
+                    # print("Similarity between generated audio and text", similarity)
+                    # print("Choose the following indexes:", best_index)
+
+        return waveform
```

### Comparing `audioldm-0.0.9/audioldm/variational_autoencoder/autoencoder.py` & `audioldm-0.1.0/audioldm/variational_autoencoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/variational_autoencoder/distributions.py` & `audioldm-0.1.0/audioldm/variational_autoencoder/distributions.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm/variational_autoencoder/modules.py` & `audioldm-0.1.0/audioldm/variational_autoencoder/modules.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.0.9/audioldm.egg-info/SOURCES.txt` & `audioldm-0.1.0/audioldm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 app.py
-check.py
 setup.py
 audioldm/__init__.py
 audioldm/__main__.py
 audioldm/ldm.py
 audioldm/pipeline.py
 audioldm/utils.py
 audioldm.egg-info/PKG-INFO
```

### Comparing `audioldm-0.0.9/bin/audioldm` & `audioldm-0.1.0/bin/audioldm`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/usr/bin/python3
 import os
-from audioldm import text_to_audio, style_transfer, build_model, save_wave, get_time
+from audioldm import text_to_audio, style_transfer, build_model, save_wave, get_time, round_up_duration, get_duration
 import argparse
 
+CACHE_DIR = os.getenv(
+    "AUDIOLDM_CACHE_DIR",
+    os.path.join(os.path.expanduser("~"), ".cache/audioldm"))
+
 parser = argparse.ArgumentParser()
 
 parser.add_argument(
     "--mode",
     type=str,
     required=False,
     default="generation",
@@ -15,25 +19,25 @@
 )
 
 parser.add_argument(
     "-t",
     "--text",
     type=str,
     required=False,
-    default="A hammer is hitting a wooden surface",
+    default="",
     help="Text prompt to the model for audio generation",
 )
 
 parser.add_argument(
     "-f",
     "--file_path",
     type=str,
     required=False,
     default=None,
-    help="Original audio file for style transfer",
+    help="(--mode transfer): Original audio file for style transfer; Or (--mode generation): the guidance audio file for generating simialr audio",
 )
 
 parser.add_argument(
     "--transfer_strength",
     type=float,
     required=False,
     default=0.5,
@@ -46,23 +50,29 @@
     type=str,
     required=False,
     help="The path to save model output",
     default="./output",
 )
 
 parser.add_argument(
+    "--model_name",
+    type=str,
+    required=False,
+    help="The checkpoint you gonna use",
+    default="audioldm-m-text-ft",
+    choices=["audioldm-s-full", "audioldm-l-full", "audioldm-s-full-v2","audioldm-m-text-ft", "audioldm-s-text-ft", "audioldm-m-full"]
+)
+
+parser.add_argument(
     "-ckpt",
     "--ckpt_path",
     type=str,
     required=False,
     help="The path to the pretrained .ckpt model",
-    default=os.path.join(
-                os.path.expanduser("~"),
-                ".cache/audioldm/audioldm-s-full.ckpt",
-            ),
+    default=None,
 )
 
 parser.add_argument(
     "-b",
     "--batchsize",
     type=int,
     required=False,
@@ -74,15 +84,14 @@
     "--ddim_steps",
     type=int,
     required=False,
     default=200,
     help="The sampling step for DDIM",
 )
 
-
 parser.add_argument(
     "-gs",
     "--guidance_scale",
     type=float,
     required=False,
     default=2.5,
     help="Guidance scale (Large => better quality and relavancy to text; Small => better diversity)",
@@ -111,39 +120,54 @@
     type=int,
     required=False,
     default=42,
     help="Change this value (any integer number) will lead to a different generation result.",
 )
 
 args = parser.parse_args()
+
+if(args.ckpt_path is not None):
+    print("Warning: ckpt_path has no effect after version 0.0.20.")
+    
 assert args.duration % 2.5 == 0, "Duration must be a multiple of 2.5"
-save_path = os.path.join(args.save_path, args.mode)
+
+mode = args.mode
+if(mode == "generation" and args.file_path is not None):
+    mode = "generation_audio_to_audio"
+    if(len(args.text) > 0):
+        print("Warning: You have specified the --file_path. --text will be ignored")
+        args.text = ""
+        
+save_path = os.path.join(args.save_path, mode)
+
 if(args.file_path is not None):
     save_path = os.path.join(save_path, os.path.basename(args.file_path.split(".")[0]))
 
 text = args.text
 random_seed = args.seed
 duration = args.duration
 guidance_scale = args.guidance_scale
 n_candidate_gen_per_text = args.n_candidate_gen_per_text
 
 os.makedirs(save_path, exist_ok=True)
-audioldm = build_model(ckpt_path=args.ckpt_path)
+audioldm = build_model(model_name=args.model_name)
 
 if(args.mode == "generation"):
     waveform = text_to_audio(
         audioldm,
         text,
+        args.file_path,
         random_seed,
         duration=duration,
         guidance_scale=guidance_scale,
         ddim_steps=args.ddim_steps,
         n_candidate_gen_per_text=n_candidate_gen_per_text,
         batchsize=args.batchsize,
     )
+    
 elif(args.mode == "transfer"):
     assert args.file_path is not None
     assert os.path.exists(args.file_path), "The original audio file \'%s\' for style transfer does not exist." % args.file_path
     waveform = style_transfer(
         audioldm,
         text,
         args.file_path,
```

### Comparing `audioldm-0.0.9/setup.py` & `audioldm-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,32 +27,34 @@
 # Package meta-data.
 NAME = "audioldm"
 DESCRIPTION = "This package is written for text-to-audio generation."
 URL = "https://github.com/haoheliu/audioldm"
 EMAIL = "haoheliu@gmail.com"
 AUTHOR = "Haohe Liu"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.0.9"
+VERSION = "0.1.0"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
     "gradio",
     "pyyaml",
     "einops",
+    "chardet",
     "numpy<=1.23.5",
     "soundfile",
-    "librosa",
+    "librosa==0.9.2",
     "scipy",
     "pandas",
-    "torchlibrosa",
+    "torchlibrosa==0.0.9",
     "transformers",
+    "progressbar",
     "ftfy",
 ]
 
 # What packages are optional?
 EXTRAS = {}
 
 # The rest you shouldn't have to touch too much :)
```

