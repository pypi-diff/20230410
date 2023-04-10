# Comparing `tmp/sj_tool-1.0.5-py3-none-any.whl.zip` & `tmp/sj_tool-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,29 @@
-Zip file size: 11291 bytes, number of entries: 25
+Zip file size: 12105 bytes, number of entries: 27
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:37 sj_tool/__init__.py
+-rw-rw-rw-  2.0 fat      226 b- defN 23-Apr-10 10:09 sj_tool/decorator.py
+-rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email.py
 -rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email_sender.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Mar-14 09:42 sj_tool/file.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-04 05:43 sj_tool/json.py
--rw-rw-rw-  2.0 fat     2302 b- defN 23-Apr-10 09:23 sj_tool/scheduler.py
+-rw-rw-rw-  2.0 fat     2180 b- defN 23-Apr-10 10:28 sj_tool/scheduler.py
 -rw-rw-rw-  2.0 fat      245 b- defN 23-Apr-04 05:43 sj_tool/system.py
--rw-rw-rw-  2.0 fat      597 b- defN 23-Apr-04 05:43 sj_tool/util.py
+-rw-rw-rw-  2.0 fat     1002 b- defN 23-Apr-10 10:05 sj_tool/util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:40 sj_tool/db/__init__.py
 -rw-rw-rw-  2.0 fat     5626 b- defN 23-Apr-08 09:02 sj_tool/db/mongo.py
 -rw-rw-rw-  2.0 fat     1237 b- defN 23-Apr-08 08:39 sj_tool/db/mysql.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-27 08:29 sj_tool/fjsp/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-27 08:30 sj_tool/fjsp/entity/__init__.py
 -rw-rw-rw-  2.0 fat      565 b- defN 23-Apr-09 06:28 sj_tool/fjsp/entity/changeover.py
 -rw-rw-rw-  2.0 fat      897 b- defN 23-Apr-10 09:07 sj_tool/fjsp/entity/global_pool.py
 -rw-rw-rw-  2.0 fat      703 b- defN 23-Apr-09 09:06 sj_tool/fjsp/entity/job.py
 -rw-rw-rw-  2.0 fat      411 b- defN 23-Apr-09 05:22 sj_tool/fjsp/entity/machine.py
 -rw-rw-rw-  2.0 fat      718 b- defN 23-Apr-09 03:28 sj_tool/fjsp/entity/operation.py
 -rw-rw-rw-  2.0 fat      113 b- defN 23-Apr-09 09:02 sj_tool/fjsp/entity/product.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-30 02:45 sj_tool/logger/__init__.py
 -rw-rw-rw-  2.0 fat     1866 b- defN 23-Apr-08 12:57 sj_tool/logger/text_logger.py
 -rw-rw-rw-  2.0 fat     2718 b- defN 23-Apr-09 03:19 sj_tool/logger/visual_logger.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-10 09:36 sj_tool-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 09:36 sj_tool-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-10 09:36 sj_tool-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1977 b- defN 23-Apr-10 09:36 sj_tool-1.0.5.dist-info/RECORD
-25 files, 21511 bytes uncompressed, 8093 bytes compressed:  62.4%
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-10 10:28 sj_tool-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 10:28 sj_tool-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-10 10:28 sj_tool-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2126 b- defN 23-Apr-10 10:28 sj_tool-1.0.6.dist-info/RECORD
+27 files, 22645 bytes uncompressed, 8683 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -1,10 +1,16 @@
 Filename: sj_tool/__init__.py
 Comment: 
 
+Filename: sj_tool/decorator.py
+Comment: 
+
+Filename: sj_tool/email.py
+Comment: 
+
 Filename: sj_tool/email_sender.py
 Comment: 
 
 Filename: sj_tool/file.py
 Comment: 
 
 Filename: sj_tool/json.py
@@ -57,20 +63,20 @@
 
 Filename: sj_tool/logger/text_logger.py
 Comment: 
 
 Filename: sj_tool/logger/visual_logger.py
 Comment: 
 
-Filename: sj_tool-1.0.5.dist-info/METADATA
+Filename: sj_tool-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: sj_tool-1.0.5.dist-info/WHEEL
+Filename: sj_tool-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: sj_tool-1.0.5.dist-info/top_level.txt
+Filename: sj_tool-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: sj_tool-1.0.5.dist-info/RECORD
+Filename: sj_tool-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sj_tool/scheduler.py

```diff
@@ -1,17 +1,17 @@
 from apscheduler.schedulers.blocking import BlockingScheduler
 from apscheduler.schedulers.background import BackgroundScheduler
 
+from sj_tool.decorator import singleton
 
+
+@singleton
 class Scheduler(object):
-    def __init__(self, background=True):
-        """
-        :param background: 是否使用后台线程运行任务。若为True，则不会阻塞主线程
-        """
-        self.scheduler = BackgroundScheduler() if background else BlockingScheduler()
+    def __init__(self):
+        self.scheduler = BackgroundScheduler()
 
     def add_interval_job(self, job_fn, seconds, job_store="default", args=None) -> str:
         """
         添加定期执行的任务
         :param job_fn: 要运行的函数
         :param seconds: 间隔时间，单位：秒
         :param job_store: 用户可自定义的job空间，借助这个用户可以将job分类，加入到不同的jobstore，方便管理
@@ -44,12 +44,12 @@
     def start(self):
         # 开始调度任务
         self.scheduler.start()
 
     def shutdown(self):
         self.scheduler.shutdown()
 
-    def remove_jobs(self, job_store, job_id=None):
+    def remove_jobs(self, job_store="default", job_id=None):
         if job_id is None:
             self.scheduler.remove_all_jobs(job_store)
         else:
             self.scheduler.remove_job(job_id, job_store)
```

## sj_tool/util.py

```diff
@@ -1,18 +1,41 @@
+import os
+import random
+import importlib
+
+import numpy as np
+
+
+def package_exists(package_name):
+    """
+    检查是否存在某个包
+    :param package_name: 包名
+    :return:
+    """
+    try:
+        importlib.import_module(package_name)
+        return True
+    except ImportError:
+        return False
+
+
 def set_random_seed(seed: int):
     """
     Setup all possible random seeds so results can be reproduced
     """
-    import torch
-
     os.environ["PYTHONHASHSEED"] = str(seed)
-    torch.manual_seed(seed)
-    torch.cuda.manual_seed_all(seed)
-    torch.backends.cudnn.deterministic = True
-    torch.backends.cudnn.benchmark = False
-    torch.manual_seed(seed)
     # tf.set_random_seed(random_seed) # if you use tensorflow
     random.seed(seed)
     np.random.seed(seed)
-    if torch.cuda.is_available():
+
+    if package_exists("torch"):
+        import torch
+
+        torch.manual_seed(seed)
         torch.cuda.manual_seed_all(seed)
-        torch.cuda.manual_seed(seed)
+        torch.backends.cudnn.deterministic = True
+        torch.backends.cudnn.benchmark = False
+        torch.manual_seed(seed)
+
+        if torch.cuda.is_available():
+            torch.cuda.manual_seed_all(seed)
+            torch.cuda.manual_seed(seed)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `sj_tool-1.0.5.dist-info/RECORD` & `sj_tool-1.0.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 sj_tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+sj_tool/decorator.py,sha256=nUTxQpiRjmV37SqojRz46vbYmV6N8-wbhF1tejJVeco,226
+sj_tool/email.py,sha256=qxNj5bQ31yzF1bi2XLIxJq5akw-vksZLOS9L5HdM5p8,476
 sj_tool/email_sender.py,sha256=qxNj5bQ31yzF1bi2XLIxJq5akw-vksZLOS9L5HdM5p8,476
 sj_tool/file.py,sha256=NsbZm_9UGni8CKoZEL9mMFwX7u2R2DXA-HtuUS1iaPw,155
 sj_tool/json.py,sha256=yG7paERY6nUtF51kz5ZXp396TKT-UgIyb0teAXeKD5Q,313
-sj_tool/scheduler.py,sha256=3NLG6IhyKXMHIkJgovyndwd0qYmWWxWrLjDHVY5OG2c,2302
+sj_tool/scheduler.py,sha256=nSQm7feMCZ8SMeaOqQQ6KkFkwytWXHlMW1fVX7xHYU4,2180
 sj_tool/system.py,sha256=xQxxnAKZ8yW8LJZlw0MhpRyQ_p1LnqwlKnuwgiFdqgI,245
-sj_tool/util.py,sha256=cFqbYbJ_NzqG2OeEF8IFrV7wjsDcULZmOa7UgatZF84,597
+sj_tool/util.py,sha256=oqnYmmzOa3dPRCNWSHDU_NziY7hODzi73A7xHQ6gcVw,1002
 sj_tool/db/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/db/mongo.py,sha256=oUDrhYV_sOq8M9KNFK_QDExCWQ070T1nksp8XzGtDs4,5626
 sj_tool/db/mysql.py,sha256=o9tidq_q9TkDbJXUb6KTMf9O9cJMZeL3rCsADCmroBQ,1237
 sj_tool/fjsp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/fjsp/entity/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/fjsp/entity/changeover.py,sha256=ORGpGQ41ac0ztSqjf48k8Zm3mUl2LXSiupLeBL4rRXY,565
 sj_tool/fjsp/entity/global_pool.py,sha256=9-pE3_NIZqVWDM0TrGosycMfzaE1iQov8mSZ3-LZEPo,897
 sj_tool/fjsp/entity/job.py,sha256=Jj5OGh1-X1LhIfy4WnkffeGL7S0StTUxOnNj0nqCbWA,703
 sj_tool/fjsp/entity/machine.py,sha256=zBjVt5VYEuJlqA4yHzzEw9wlbVSAaJHlgj0lweSNaSw,411
 sj_tool/fjsp/entity/operation.py,sha256=_wI52FmRa80I_SvMm5fB0ZX4cQUAmhY3jtbUuN8dgsY,718
 sj_tool/fjsp/entity/product.py,sha256=IzErQu-Hm0d8rSdWA3Z-HYaYBDmNUbyOMBumYc1dwuU,113
 sj_tool/logger/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/logger/text_logger.py,sha256=hNPAxGVOsL46q-9cd-o-S7WV3CL52vlhD7HWKRAeh2Y,1866
 sj_tool/logger/visual_logger.py,sha256=AfKNWJpTb-Odm4gWUyVRXIykiXyvfrdAjukwugCD6os,2718
-sj_tool-1.0.5.dist-info/METADATA,sha256=dbzMNVqp7rxan2b2dfyLVUai-d8eWwmEEE9Q-7C7dIY,492
-sj_tool-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sj_tool-1.0.5.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
-sj_tool-1.0.5.dist-info/RECORD,,
+sj_tool-1.0.6.dist-info/METADATA,sha256=fqz--AZEPyxo6ebGv7tTlXLOmAZIIIOi3O312CzyLxE,492
+sj_tool-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sj_tool-1.0.6.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
+sj_tool-1.0.6.dist-info/RECORD,,
```

