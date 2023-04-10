# Comparing `tmp/nextgpt-0.0.2.tar.gz` & `tmp/nextgpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextgpt-0.0.2.tar", last modified: Mon Apr 10 19:58:40 2023, max compression
+gzip compressed data, was "nextgpt-0.0.3.tar", last modified: Mon Apr 10 20:56:49 2023, max compression
```

## Comparing `nextgpt-0.0.2.tar` & `nextgpt-0.0.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.158031 nextgpt-0.0.2/
--rw-r--r--   0 ybae2      (502) staff       (20)    11396 2023-04-10 16:51:37.000000 nextgpt-0.0.2/LICENSE
--rw-r--r--   0 ybae2      (502) staff       (20)       60 2023-04-10 19:51:51.000000 nextgpt-0.0.2/MANIFEST.in
--rw-r--r--   0 ybae2      (502) staff       (20)     1584 2023-04-10 19:58:40.158342 nextgpt-0.0.2/PKG-INFO
--rw-r--r--   0 ybae2      (502) staff       (20)     1359 2023-04-10 18:26:51.000000 nextgpt-0.0.2/README.md
--rw-r--r--   0 ybae2      (502) staff       (20)      254 2023-04-10 16:58:44.000000 nextgpt-0.0.2/requirements.txt
--rw-r--r--   0 ybae2      (502) staff       (20)      103 2023-04-10 19:58:40.161108 nextgpt-0.0.2/setup.cfg
--rw-r--r--   0 ybae2      (502) staff       (20)      888 2023-04-10 19:58:23.000000 nextgpt-0.0.2/setup.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:39.976555 nextgpt-0.0.2/src/
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:39.986398 nextgpt-0.0.2/src/nextgpt/
--rw-r--r--   0 ybae2      (502) staff       (20)        0 2023-04-02 22:26:04.000000 nextgpt-0.0.2/src/nextgpt/__init__.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:39.997412 nextgpt-0.0.2/src/nextgpt/dataset/
--rw-rw-r--   0 ybae2      (502) staff       (20)      384 2023-04-09 23:18:51.000000 nextgpt-0.0.2/src/nextgpt/dataset/__init__.py
--rw-r--r--   0 ybae2      (502) staff       (20)     1557 2023-04-09 23:42:09.000000 nextgpt-0.0.2/src/nextgpt/dataset/prompt_dataset.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2077 2023-04-08 05:42:58.000000 nextgpt-0.0.2/src/nextgpt/dataset/reward_dataset.py
--rw-r--r--   0 ybae2      (502) staff       (20)     5903 2023-04-08 23:30:05.000000 nextgpt-0.0.2/src/nextgpt/dataset/sft_dataset.py
--rw-rw-r--   0 ybae2      (502) staff       (20)      121 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/dataset/utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.001613 nextgpt-0.0.2/src/nextgpt/experience_maker/
--rw-rw-r--   0 ybae2      (502) staff       (20)      155 2023-04-07 03:39:09.000000 nextgpt-0.0.2/src/nextgpt/experience_maker/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2455 2023-04-08 19:18:09.000000 nextgpt-0.0.2/src/nextgpt/experience_maker/base.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1421 2023-04-08 19:18:19.000000 nextgpt-0.0.2/src/nextgpt/experience_maker/naive.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.005834 nextgpt-0.0.2/src/nextgpt/finetuning/
--rw-r--r--   0 ybae2      (502) staff       (20)      130 2023-04-10 17:22:26.000000 nextgpt-0.0.2/src/nextgpt/finetuning/__init__.py
--rw-r--r--   0 ybae2      (502) staff       (20)     1872 2023-04-01 19:32:10.000000 nextgpt-0.0.2/src/nextgpt/finetuning/callbacks.py
--rw-r--r--   0 ybae2      (502) staff       (20)     1038 2023-04-01 19:32:10.000000 nextgpt-0.0.2/src/nextgpt/finetuning/trainer.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.016041 nextgpt-0.0.2/src/nextgpt/models/
--rw-rw-r--   0 ybae2      (502) staff       (20)      245 2023-04-04 17:08:15.000000 nextgpt-0.0.2/src/nextgpt/models/__init__.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.026901 nextgpt-0.0.2/src/nextgpt/models/base/
--rw-rw-r--   0 ybae2      (502) staff       (20)      161 2023-04-08 06:54:54.000000 nextgpt-0.0.2/src/nextgpt/models/base/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2480 2023-04-09 23:51:32.000000 nextgpt-0.0.2/src/nextgpt/models/base/actor.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1624 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/base/critic.py
--rw-rw-r--   0 ybae2      (502) staff       (20)      919 2023-04-08 06:34:00.000000 nextgpt-0.0.2/src/nextgpt/models/base/lm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1419 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/base/reward_model.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.044173 nextgpt-0.0.2/src/nextgpt/models/bloom/
--rw-rw-r--   0 ybae2      (502) staff       (20)      197 2023-04-08 06:56:20.000000 nextgpt-0.0.2/src/nextgpt/models/bloom/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1097 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/bloom/bloom_actor.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1214 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/bloom/bloom_critic.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1091 2023-04-03 09:12:22.000000 nextgpt-0.0.2/src/nextgpt/models/bloom/bloom_lm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1170 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/bloom/bloom_rm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     6951 2023-04-08 19:12:37.000000 nextgpt-0.0.2/src/nextgpt/models/generation.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     3552 2023-04-08 19:13:03.000000 nextgpt-0.0.2/src/nextgpt/models/generation_utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.055013 nextgpt-0.0.2/src/nextgpt/models/gpt/
--rw-rw-r--   0 ybae2      (502) staff       (20)      173 2023-04-08 06:56:00.000000 nextgpt-0.0.2/src/nextgpt/models/gpt/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1182 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/gpt/gpt_actor.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1242 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/gpt/gpt_critic.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1347 2023-04-08 20:49:49.000000 nextgpt-0.0.2/src/nextgpt/models/gpt/gpt_lm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1456 2023-04-06 18:56:26.000000 nextgpt-0.0.2/src/nextgpt/models/gpt/gpt_rm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     4792 2023-04-08 19:13:30.000000 nextgpt-0.0.2/src/nextgpt/models/lora.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     3633 2023-04-10 16:48:50.000000 nextgpt-0.0.2/src/nextgpt/models/loss.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.066673 nextgpt-0.0.2/src/nextgpt/models/opt/
--rw-rw-r--   0 ybae2      (502) staff       (20)      173 2023-04-08 06:56:42.000000 nextgpt-0.0.2/src/nextgpt/models/opt/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1164 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/opt/opt_actor.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1283 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/opt/opt_critic.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1158 2023-04-03 09:12:22.000000 nextgpt-0.0.2/src/nextgpt/models/opt/opt_lm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1176 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/models/opt/opt_rm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     3483 2023-04-08 19:14:21.000000 nextgpt-0.0.2/src/nextgpt/models/utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.106800 nextgpt-0.0.2/src/nextgpt/replay_buffer/
--rw-rw-r--   0 ybae2      (502) staff       (20)      117 2023-04-07 03:39:09.000000 nextgpt-0.0.2/src/nextgpt/replay_buffer/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1050 2023-04-08 19:18:33.000000 nextgpt-0.0.2/src/nextgpt/replay_buffer/base.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1997 2023-04-08 19:18:40.000000 nextgpt-0.0.2/src/nextgpt/replay_buffer/naive.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2376 2023-04-08 19:18:49.000000 nextgpt-0.0.2/src/nextgpt/replay_buffer/utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.142342 nextgpt-0.0.2/src/nextgpt/trainer/
--rw-rw-r--   0 ybae2      (502) staff       (20)      190 2023-04-08 06:57:54.000000 nextgpt-0.0.2/src/nextgpt/trainer/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     8730 2023-04-08 19:32:33.000000 nextgpt-0.0.2/src/nextgpt/trainer/base.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.148657 nextgpt-0.0.2/src/nextgpt/trainer/callbacks/
--rw-rw-r--   0 ybae2      (502) staff       (20)      193 2023-04-07 03:39:09.000000 nextgpt-0.0.2/src/nextgpt/trainer/callbacks/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)      841 2023-04-08 19:20:17.000000 nextgpt-0.0.2/src/nextgpt/trainer/callbacks/base.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     5402 2023-04-08 19:20:52.000000 nextgpt-0.0.2/src/nextgpt/trainer/callbacks/performance_evaluator.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2840 2023-04-08 19:20:48.000000 nextgpt-0.0.2/src/nextgpt/trainer/callbacks/save_checkpoint.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     6980 2023-04-10 01:27:30.000000 nextgpt-0.0.2/src/nextgpt/trainer/ppo.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     6121 2023-04-08 19:08:44.000000 nextgpt-0.0.2/src/nextgpt/trainer/rm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     6991 2023-04-08 22:42:31.000000 nextgpt-0.0.2/src/nextgpt/trainer/sft.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:40.156832 nextgpt-0.0.2/src/nextgpt/trainer/strategies/
--rw-rw-r--   0 ybae2      (502) staff       (20)      145 2023-04-03 20:19:30.000000 nextgpt-0.0.2/src/nextgpt/trainer/strategies/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     4758 2023-04-08 18:37:38.000000 nextgpt-0.0.2/src/nextgpt/trainer/strategies/base.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     4537 2023-04-08 18:42:20.000000 nextgpt-0.0.2/src/nextgpt/trainer/strategies/ddp.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     3077 2023-04-08 18:45:13.000000 nextgpt-0.0.2/src/nextgpt/trainer/strategies/naive.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1108 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/trainer/strategies/sampler.py
--rw-rw-r--   0 ybae2      (502) staff       (20)      121 2023-03-28 02:52:31.000000 nextgpt-0.0.2/src/nextgpt/trainer/utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 19:58:39.991624 nextgpt-0.0.2/src/nextgpt.egg-info/
--rw-r--r--   0 ybae2      (502) staff       (20)     1584 2023-04-10 19:58:39.000000 nextgpt-0.0.2/src/nextgpt.egg-info/PKG-INFO
--rw-r--r--   0 ybae2      (502) staff       (20)     2251 2023-04-10 19:58:39.000000 nextgpt-0.0.2/src/nextgpt.egg-info/SOURCES.txt
--rw-r--r--   0 ybae2      (502) staff       (20)        1 2023-04-10 19:58:39.000000 nextgpt-0.0.2/src/nextgpt.egg-info/dependency_links.txt
--rw-r--r--   0 ybae2      (502) staff       (20)       54 2023-04-10 19:58:39.000000 nextgpt-0.0.2/src/nextgpt.egg-info/requires.txt
--rw-r--r--   0 ybae2      (502) staff       (20)        8 2023-04-10 19:58:39.000000 nextgpt-0.0.2/src/nextgpt.egg-info/top_level.txt
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.928187 nextgpt-0.0.3/
+-rw-r--r--   0 ybae2      (502) staff       (20)    11396 2023-04-10 16:51:37.000000 nextgpt-0.0.3/LICENSE
+-rw-r--r--   0 ybae2      (502) staff       (20)       60 2023-04-10 19:51:51.000000 nextgpt-0.0.3/MANIFEST.in
+-rw-r--r--   0 ybae2      (502) staff       (20)     1584 2023-04-10 20:56:49.928496 nextgpt-0.0.3/PKG-INFO
+-rw-r--r--   0 ybae2      (502) staff       (20)     1359 2023-04-10 18:26:51.000000 nextgpt-0.0.3/README.md
+-rw-r--r--   0 ybae2      (502) staff       (20)      254 2023-04-10 16:58:44.000000 nextgpt-0.0.3/requirements.txt
+-rw-r--r--   0 ybae2      (502) staff       (20)      103 2023-04-10 20:56:49.931403 nextgpt-0.0.3/setup.cfg
+-rw-r--r--   0 ybae2      (502) staff       (20)      888 2023-04-10 20:56:43.000000 nextgpt-0.0.3/setup.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.733049 nextgpt-0.0.3/src/
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.747668 nextgpt-0.0.3/src/nextgpt/
+-rw-r--r--   0 ybae2      (502) staff       (20)        0 2023-04-02 22:26:04.000000 nextgpt-0.0.3/src/nextgpt/__init__.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.765299 nextgpt-0.0.3/src/nextgpt/dataset/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      384 2023-04-09 23:18:51.000000 nextgpt-0.0.3/src/nextgpt/dataset/__init__.py
+-rw-r--r--   0 ybae2      (502) staff       (20)     1557 2023-04-09 23:42:09.000000 nextgpt-0.0.3/src/nextgpt/dataset/prompt_dataset.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2077 2023-04-08 05:42:58.000000 nextgpt-0.0.3/src/nextgpt/dataset/reward_dataset.py
+-rw-r--r--   0 ybae2      (502) staff       (20)     5903 2023-04-08 23:30:05.000000 nextgpt-0.0.3/src/nextgpt/dataset/sft_dataset.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)      121 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/dataset/utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.770291 nextgpt-0.0.3/src/nextgpt/experience_maker/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      155 2023-04-07 03:39:09.000000 nextgpt-0.0.3/src/nextgpt/experience_maker/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2455 2023-04-08 19:18:09.000000 nextgpt-0.0.3/src/nextgpt/experience_maker/base.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1421 2023-04-08 19:18:19.000000 nextgpt-0.0.3/src/nextgpt/experience_maker/naive.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.776202 nextgpt-0.0.3/src/nextgpt/finetuning/
+-rw-r--r--   0 ybae2      (502) staff       (20)      130 2023-04-10 17:22:26.000000 nextgpt-0.0.3/src/nextgpt/finetuning/__init__.py
+-rw-r--r--   0 ybae2      (502) staff       (20)     1872 2023-04-01 19:32:10.000000 nextgpt-0.0.3/src/nextgpt/finetuning/callbacks.py
+-rw-r--r--   0 ybae2      (502) staff       (20)     1038 2023-04-01 19:32:10.000000 nextgpt-0.0.3/src/nextgpt/finetuning/trainer.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.787798 nextgpt-0.0.3/src/nextgpt/models/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      245 2023-04-04 17:08:15.000000 nextgpt-0.0.3/src/nextgpt/models/__init__.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.802292 nextgpt-0.0.3/src/nextgpt/models/base/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      161 2023-04-08 06:54:54.000000 nextgpt-0.0.3/src/nextgpt/models/base/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2480 2023-04-09 23:51:32.000000 nextgpt-0.0.3/src/nextgpt/models/base/actor.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1624 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/base/critic.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)      919 2023-04-08 06:34:00.000000 nextgpt-0.0.3/src/nextgpt/models/base/lm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1419 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/base/reward_model.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.814100 nextgpt-0.0.3/src/nextgpt/models/bloom/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      197 2023-04-08 06:56:20.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1097 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_actor.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1214 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_critic.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1091 2023-04-03 09:12:22.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_lm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1170 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_rm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     6951 2023-04-08 19:12:37.000000 nextgpt-0.0.3/src/nextgpt/models/generation.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     3552 2023-04-08 19:13:03.000000 nextgpt-0.0.3/src/nextgpt/models/generation_utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.834428 nextgpt-0.0.3/src/nextgpt/models/gpt/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      173 2023-04-08 06:56:00.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1182 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_actor.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1242 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_critic.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1347 2023-04-08 20:49:49.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_lm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1456 2023-04-06 18:56:26.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_rm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     4792 2023-04-08 19:13:30.000000 nextgpt-0.0.3/src/nextgpt/models/lora.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     3633 2023-04-10 16:48:50.000000 nextgpt-0.0.3/src/nextgpt/models/loss.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.848555 nextgpt-0.0.3/src/nextgpt/models/opt/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      173 2023-04-08 06:56:42.000000 nextgpt-0.0.3/src/nextgpt/models/opt/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1164 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/opt/opt_actor.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1283 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/opt/opt_critic.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1158 2023-04-03 09:12:22.000000 nextgpt-0.0.3/src/nextgpt/models/opt/opt_lm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1176 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/opt/opt_rm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     3483 2023-04-08 19:14:21.000000 nextgpt-0.0.3/src/nextgpt/models/utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.861828 nextgpt-0.0.3/src/nextgpt/replay_buffer/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      117 2023-04-07 03:39:09.000000 nextgpt-0.0.3/src/nextgpt/replay_buffer/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1050 2023-04-08 19:18:33.000000 nextgpt-0.0.3/src/nextgpt/replay_buffer/base.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1997 2023-04-08 19:18:40.000000 nextgpt-0.0.3/src/nextgpt/replay_buffer/naive.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2376 2023-04-08 19:18:49.000000 nextgpt-0.0.3/src/nextgpt/replay_buffer/utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.881883 nextgpt-0.0.3/src/nextgpt/trainer/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      190 2023-04-08 06:57:54.000000 nextgpt-0.0.3/src/nextgpt/trainer/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     8730 2023-04-08 19:32:33.000000 nextgpt-0.0.3/src/nextgpt/trainer/base.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.907237 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      193 2023-04-07 03:39:09.000000 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)      841 2023-04-08 19:20:17.000000 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/base.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     5402 2023-04-08 19:20:52.000000 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/performance_evaluator.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2840 2023-04-08 19:20:48.000000 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/save_checkpoint.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     6980 2023-04-10 01:27:30.000000 nextgpt-0.0.3/src/nextgpt/trainer/ppo.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     6121 2023-04-08 19:08:44.000000 nextgpt-0.0.3/src/nextgpt/trainer/rm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     7045 2023-04-10 20:54:20.000000 nextgpt-0.0.3/src/nextgpt/trainer/sft.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.926174 nextgpt-0.0.3/src/nextgpt/trainer/strategies/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      145 2023-04-03 20:19:30.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     4758 2023-04-08 18:37:38.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/base.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     4537 2023-04-08 18:42:20.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/ddp.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     3077 2023-04-08 18:45:13.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/naive.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1108 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/sampler.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)      121 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/trainer/utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.755478 nextgpt-0.0.3/src/nextgpt.egg-info/
+-rw-r--r--   0 ybae2      (502) staff       (20)     1584 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/PKG-INFO
+-rw-r--r--   0 ybae2      (502) staff       (20)     2251 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 ybae2      (502) staff       (20)        1 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 ybae2      (502) staff       (20)       54 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/requires.txt
+-rw-r--r--   0 ybae2      (502) staff       (20)        8 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/top_level.txt
```

### Comparing `nextgpt-0.0.2/LICENSE` & `nextgpt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/PKG-INFO` & `nextgpt-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextgpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: nextGPT
 Home-page: https://github.com/louiezzang/next-gpt
 Author: Younggue Bae
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nextgpt-0.0.2/README.md` & `nextgpt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/setup.py` & `nextgpt-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import os
 import sys
 import pkg_resources
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "nextGPT"
 
 setup(
     name="nextgpt",
     version=VERSION,
     description=DESCRIPTION,
     long_description=open("README.md", "r", encoding="utf-8").read(),
```

### Comparing `nextgpt-0.0.2/src/nextgpt/dataset/prompt_dataset.py` & `nextgpt-0.0.3/src/nextgpt/dataset/prompt_dataset.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/dataset/reward_dataset.py` & `nextgpt-0.0.3/src/nextgpt/dataset/reward_dataset.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/dataset/sft_dataset.py` & `nextgpt-0.0.3/src/nextgpt/dataset/sft_dataset.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/experience_maker/base.py` & `nextgpt-0.0.3/src/nextgpt/experience_maker/base.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/experience_maker/naive.py` & `nextgpt-0.0.3/src/nextgpt/experience_maker/naive.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/finetuning/callbacks.py` & `nextgpt-0.0.3/src/nextgpt/finetuning/callbacks.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/finetuning/trainer.py` & `nextgpt-0.0.3/src/nextgpt/finetuning/trainer.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/base/actor.py` & `nextgpt-0.0.3/src/nextgpt/models/base/actor.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/base/critic.py` & `nextgpt-0.0.3/src/nextgpt/models/base/critic.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/base/lm.py` & `nextgpt-0.0.3/src/nextgpt/models/base/lm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/base/reward_model.py` & `nextgpt-0.0.3/src/nextgpt/models/base/reward_model.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/bloom/bloom_actor.py` & `nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_actor.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/bloom/bloom_critic.py` & `nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_critic.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/bloom/bloom_lm.py` & `nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_lm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/bloom/bloom_rm.py` & `nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_rm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/generation.py` & `nextgpt-0.0.3/src/nextgpt/models/generation.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/generation_utils.py` & `nextgpt-0.0.3/src/nextgpt/models/generation_utils.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/gpt/gpt_actor.py` & `nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_actor.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/gpt/gpt_critic.py` & `nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_critic.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/gpt/gpt_lm.py` & `nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_lm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/gpt/gpt_rm.py` & `nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_rm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/lora.py` & `nextgpt-0.0.3/src/nextgpt/models/lora.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/loss.py` & `nextgpt-0.0.3/src/nextgpt/models/loss.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/opt/opt_actor.py` & `nextgpt-0.0.3/src/nextgpt/models/opt/opt_actor.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/opt/opt_critic.py` & `nextgpt-0.0.3/src/nextgpt/models/opt/opt_critic.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/opt/opt_lm.py` & `nextgpt-0.0.3/src/nextgpt/models/opt/opt_lm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/opt/opt_rm.py` & `nextgpt-0.0.3/src/nextgpt/models/opt/opt_rm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/models/utils.py` & `nextgpt-0.0.3/src/nextgpt/models/utils.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/replay_buffer/base.py` & `nextgpt-0.0.3/src/nextgpt/replay_buffer/base.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/replay_buffer/naive.py` & `nextgpt-0.0.3/src/nextgpt/replay_buffer/naive.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/replay_buffer/utils.py` & `nextgpt-0.0.3/src/nextgpt/replay_buffer/utils.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/base.py` & `nextgpt-0.0.3/src/nextgpt/trainer/base.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/callbacks/base.py` & `nextgpt-0.0.3/src/nextgpt/trainer/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/callbacks/performance_evaluator.py` & `nextgpt-0.0.3/src/nextgpt/trainer/callbacks/performance_evaluator.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/callbacks/save_checkpoint.py` & `nextgpt-0.0.3/src/nextgpt/trainer/callbacks/save_checkpoint.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/ppo.py` & `nextgpt-0.0.3/src/nextgpt/trainer/ppo.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/rm.py` & `nextgpt-0.0.3/src/nextgpt/trainer/rm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/sft.py` & `nextgpt-0.0.3/src/nextgpt/trainer/sft.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from torch import nn
 from torch.optim import Adam, Optimizer
 from torch.optim.lr_scheduler import LambdaLR
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 from tqdm import tqdm
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
-from transformers.trainer import get_scheduler
+# from transformers.trainer import get_scheduler
+from transformers.optimization import get_scheduler
 
 from .strategies import Strategy
 from .utils import is_rank_0
 
 
 class SFTTrainer(ABC):
     """
```

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/strategies/base.py` & `nextgpt-0.0.3/src/nextgpt/trainer/strategies/base.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/strategies/ddp.py` & `nextgpt-0.0.3/src/nextgpt/trainer/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/strategies/naive.py` & `nextgpt-0.0.3/src/nextgpt/trainer/strategies/naive.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt/trainer/strategies/sampler.py` & `nextgpt-0.0.3/src/nextgpt/trainer/strategies/sampler.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.2/src/nextgpt.egg-info/PKG-INFO` & `nextgpt-0.0.3/src/nextgpt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextgpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: nextGPT
 Home-page: https://github.com/louiezzang/next-gpt
 Author: Younggue Bae
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nextgpt-0.0.2/src/nextgpt.egg-info/SOURCES.txt` & `nextgpt-0.0.3/src/nextgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

