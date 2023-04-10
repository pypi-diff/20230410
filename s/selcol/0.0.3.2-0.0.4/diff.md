# Comparing `tmp/selcol-0.0.3.2.tar.gz` & `tmp/selcol-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selcol-0.0.3.2.tar", last modified: Wed Jan 11 08:38:00 2023, max compression
+gzip compressed data, was "selcol-0.0.4.tar", last modified: Mon Apr 10 21:15:23 2023, max compression
```

## Comparing `selcol-0.0.3.2.tar` & `selcol-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,54 @@
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-01-11 08:38:00.808346 selcol-0.0.3.2/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       38 2023-01-11 08:30:47.000000 selcol-0.0.3.2/MANIFEST.in
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      257 2023-01-11 08:38:00.808346 selcol-0.0.3.2/PKG-INFO
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      550 2023-01-01 17:29:44.000000 selcol-0.0.3.2/README.md
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       63 2022-12-28 18:19:34.000000 selcol-0.0.3.2/pyproject.toml
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-01-11 08:38:00.804346 selcol-0.0.3.2/selcol/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        0 2022-12-29 18:57:10.000000 selcol-0.0.3.2/selcol/__init__.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      824 2023-01-11 08:31:57.000000 selcol-0.0.3.2/selcol/file.py
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-01-11 08:38:00.804346 selcol-0.0.3.2/selcol/pretrained/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       13 2023-01-11 08:28:54.000000 selcol-0.0.3.2/selcol/pretrained/.gitignore
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-01-11 08:38:00.804346 selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      529 2023-01-01 19:38:20.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332605 2023-01-01 19:38:20.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   331764 2023-01-01 19:38:20.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/numpy_layers.pkl
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-01-11 08:38:00.808346 selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      726 2023-01-01 15:51:31.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/metadata.json
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-1.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338205 2023-01-01 15:51:31.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-128.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-16.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-32.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-64.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-8.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   337364 2023-01-01 15:51:31.000000 selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/numpy_layers.pkl
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-01-11 08:38:00.808346 selcol-0.0.3.2/selcol/runtime/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      168 2023-01-01 18:50:35.000000 selcol-0.0.3.2/selcol/runtime/__init__.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3327 2023-01-11 07:41:04.000000 selcol-0.0.3.2/selcol/runtime/interface.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3658 2023-01-11 07:41:04.000000 selcol-0.0.3.2/selcol/runtime/jax_model.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     4128 2023-01-11 07:41:04.000000 selcol-0.0.3.2/selcol/runtime/ort_model.py
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-01-11 08:38:00.808346 selcol-0.0.3.2/selcol/traintime/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        0 2022-12-29 16:59:41.000000 selcol-0.0.3.2/selcol/traintime/__init__.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     8348 2022-12-31 22:50:53.000000 selcol-0.0.3.2/selcol/traintime/dataset.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     9012 2023-01-01 18:49:50.000000 selcol-0.0.3.2/selcol/traintime/neural.py
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-01-11 08:38:00.804346 selcol-0.0.3.2/selcol.egg-info/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      257 2023-01-11 08:38:00.000000 selcol-0.0.3.2/selcol.egg-info/PKG-INFO
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     2344 2023-01-11 08:38:00.000000 selcol-0.0.3.2/selcol.egg-info/SOURCES.txt
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        1 2023-01-11 08:38:00.000000 selcol-0.0.3.2/selcol.egg-info/dependency_links.txt
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       49 2023-01-11 08:38:00.000000 selcol-0.0.3.2/selcol.egg-info/requires.txt
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        7 2023-01-11 08:38:00.000000 selcol-0.0.3.2/selcol.egg-info/top_level.txt
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       38 2023-01-11 08:38:00.808346 selcol-0.0.3.2/setup.cfg
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      554 2023-01-11 08:37:37.000000 selcol-0.0.3.2/setup.py
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.696110 selcol-0.0.4/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       38 2023-01-11 08:30:47.000000 selcol-0.0.4/MANIFEST.in
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      197 2023-04-10 21:15:23.696110 selcol-0.0.4/PKG-INFO
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      550 2023-01-01 17:29:44.000000 selcol-0.0.4/README.md
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       63 2022-12-28 18:19:34.000000 selcol-0.0.4/pyproject.toml
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.680110 selcol-0.0.4/selcol/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        0 2022-12-29 18:57:10.000000 selcol-0.0.4/selcol/__init__.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      824 2023-01-15 03:02:13.000000 selcol-0.0.4/selcol/file.py
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.680110 selcol-0.0.4/selcol/pretrained/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       13 2023-01-11 08:28:54.000000 selcol-0.0.4/selcol/pretrained/.gitignore
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.680110 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)     1020 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/metadata.json
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-1.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355007 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-128.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-16.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-32.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-64.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-8.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   354164 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/numpy_layers.pkl
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.692110 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      529 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332605 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   331764 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/numpy_layers.pkl
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.692110 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      726 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/metadata.json
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-1.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338205 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-128.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-16.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-32.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-64.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-8.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   337364 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/numpy_layers.pkl
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.696110 selcol-0.0.4/selcol/runtime/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      168 2023-01-01 18:50:35.000000 selcol-0.0.4/selcol/runtime/__init__.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3327 2023-04-09 19:21:17.000000 selcol-0.0.4/selcol/runtime/interface.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3658 2023-01-11 07:41:04.000000 selcol-0.0.4/selcol/runtime/jax_model.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     4128 2023-01-11 07:41:04.000000 selcol-0.0.4/selcol/runtime/ort_model.py
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.696110 selcol-0.0.4/selcol/traintime/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        0 2022-12-29 16:59:41.000000 selcol-0.0.4/selcol/traintime/__init__.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     8395 2023-04-09 14:41:30.000000 selcol-0.0.4/selcol/traintime/dataset.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     9915 2023-04-09 15:36:33.000000 selcol-0.0.4/selcol/traintime/neural.py
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.680110 selcol-0.0.4/selcol.egg-info/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      197 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/PKG-INFO
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3338 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/SOURCES.txt
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        1 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/dependency_links.txt
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       49 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/requires.txt
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        7 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/top_level.txt
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       38 2023-04-10 21:15:23.696110 selcol-0.0.4/setup.cfg
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      553 2023-04-10 21:14:53.000000 selcol-0.0.4/setup.py
```

### Comparing `selcol-0.0.3.2/README.md` & `selcol-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/file.py` & `selcol-0.0.4/selcol/file.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json` & `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/numpy_layers.pkl` & `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/numpy_layers.pkl`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/metadata.json` & `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/metadata.json`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-1.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-1.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-128.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-128.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-16.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-16.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-32.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-32.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-64.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-64.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-8.onnx` & `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-8.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/numpy_layers.pkl` & `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/numpy_layers.pkl`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/runtime/interface.py` & `selcol-0.0.4/selcol/runtime/interface.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/runtime/jax_model.py` & `selcol-0.0.4/selcol/runtime/jax_model.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/runtime/ort_model.py` & `selcol-0.0.4/selcol/runtime/ort_model.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.3.2/selcol/traintime/dataset.py` & `selcol-0.0.4/selcol/traintime/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,26 +45,25 @@
         check_link_names = []
         for link in robot_model.link_list:
             if has_ignore_name(link.name):
                 continue
 
             transform = link.worldcoords().T()
 
-            if use_visual_mesh:
-                mesh = link.visual_mesh
-                if len(mesh) == 0:
-                    continue
-                assert len(mesh) == 1
-                mesh = mesh[0]
-            else:
-                # I didn't test this feature well.
-                mesh = link.collision_mesh
-                if mesh is None:
-                    continue
-            col_manager.add_object(link.name, mesh, transform=transform)
+            assert use_visual_mesh
+
+            mesh = link.visual_mesh
+            if len(mesh) == 0:
+                continue
+
+            union_mesh = mesh[0]
+            for i in range(1, len(mesh)):
+                union_mesh = trimesh.util.concatenate(union_mesh, mesh[i])
+
+            col_manager.add_object(link.name, union_mesh, transform=transform)
             check_link_names.append(link.name)
 
         _, ignore_set = col_manager.in_collision_internal(return_names=True)
         return cls(col_manager, check_link_names, robot_model, ignore_set)
 
     def update(self, robot_model: RobotModel) -> None:
         for link_name in self._check_link_names:
@@ -224,28 +223,33 @@
     else:
         robot_config_list = []
         for _ in range(task_arg.n_sample):
             vec = get_random_robot_state(robot_model, task_arg.joint_names)
             robot_config_list.append(vec)
 
     samples: List[Tuple[np.ndarray, bool]] = []
+    total_count = 0
     positive_count = 0
     for robot_config in tqdm.tqdm(robot_config_list, disable=task_arg.disable_tqdm):
 
         # update config
         for angle, jn in zip(robot_config, task_arg.joint_names):
             robot_model.__dict__[jn].joint_angle(angle)
         manager.update(robot_model)
 
         # check
         pairs = manager.check_collision()
         colliding = len(pairs) > 0
+
         samples.append((robot_config, colliding))
+
+        total_count += 1
         if colliding:
             positive_count += 1
+        logger.debug("positive ratio {}".format(float(positive_count) / float(total_count)))
 
     file_path = task_arg.cache_path / (
         "dataset-{}-{}dof".format(header.robot_name, len(header.joint_names))
         + str(uuid.uuid4())
         + ".pkl"
     )
```

### Comparing `selcol-0.0.3.2/selcol/traintime/neural.py` & `selcol-0.0.4/selcol/traintime/neural.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __len__(self) -> int:
         return len(self.Y)
 
     def __getitem__(self, idx) -> Tuple[torch.Tensor, torch.Tensor]:
         return self.X[idx], self.Y[idx]
 
     @classmethod
-    def load(cls, base_path: Path) -> "SelfColDataset":
+    def load(cls, base_path: Path, balance: bool = True) -> "SelfColDataset":
         hash_values = set()
 
         x_list = []
         y_list = []
 
         n_dof: Optional[int] = None
         header: Optional[Metadata] = None
@@ -63,14 +63,34 @@
             n_dof = len(chunk.header.joint_names)
 
         all_hashvalue_same = len(hash_values) == 1
         assert all_hashvalue_same
 
         X = torch.stack(x_list)
         Y = torch.stack(y_list)
+
+        if balance:
+            positive_indices = torch.where(Y > 0.5)[0]
+            negative_indices = torch.where(Y <= 0.5)[0]
+            n_positive = len(positive_indices)
+            n_negative = len(negative_indices)
+            logger.info("balancing data... posi: {}. nega: {}".format(n_positive, n_negative))
+
+            if n_positive > n_negative:
+                positive_indices = positive_indices[torch.randperm(n_positive)][:n_negative]
+            else:
+                negative_indices = negative_indices[torch.randperm(n_negative)][:n_positive]
+
+            n_positive = len(positive_indices)
+            n_negative = len(negative_indices)
+            logger.info("modified to => posi: {}. nega: {}".format(n_positive, n_negative))
+            indices = torch.concat([positive_indices, negative_indices])
+            X = X[indices]
+            Y = Y[indices]
+
         assert n_dof is not None
         assert header is not None
         return cls(n_dof, X, Y.float(), header)
 
 
 @dataclass
 class SelcolNetConfig:
```

### Comparing `selcol-0.0.3.2/selcol.egg-info/SOURCES.txt` & `selcol-0.0.4/selcol.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 selcol/file.py
 selcol.egg-info/PKG-INFO
 selcol.egg-info/SOURCES.txt
 selcol.egg-info/dependency_links.txt
 selcol.egg-info/requires.txt
 selcol.egg-info/top_level.txt
 selcol/pretrained/.gitignore
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/metadata.json
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-1.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-128.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-16.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-32.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-64.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-8.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/numpy_layers.pkl
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx
```

### Comparing `selcol-0.0.3.2/setup.py` & `selcol-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 install_requires = ["numpy", "onnxruntime"]
 dev_requires = ["torch", "scikit-robot", "tqdm"]
 
 setup(
     name="selcol",
-    version="0.0.3.2",
+    version="0.0.4",
     description="yet another percol implementation",
     author="Hirokazu Ishida",
     author_email="h-ishida@jsk.imi.i.u-tokyo.ac.jp",
     license="MIT",
     install_requires=install_requires,
     extras_require={"dev": dev_requires},
     packages=find_packages(exclude=("tests", "docs")),
     package_data={"selcol": ["py.typed"]},
-    include_package_data=True
+    include_package_data=True,
 )
```

