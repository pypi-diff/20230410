# Comparing `tmp/sj_tool-1.0.4-py3-none-any.whl.zip` & `tmp/sj_tool-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,27 @@
-Zip file size: 10265 bytes, number of entries: 24
+Zip file size: 11291 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:37 sj_tool/__init__.py
 -rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email_sender.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Mar-14 09:42 sj_tool/file.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-04 05:43 sj_tool/json.py
--rw-rw-rw-  2.0 fat     1710 b- defN 23-Mar-31 04:11 sj_tool/scheduler.py
+-rw-rw-rw-  2.0 fat     2302 b- defN 23-Apr-10 09:23 sj_tool/scheduler.py
 -rw-rw-rw-  2.0 fat      245 b- defN 23-Apr-04 05:43 sj_tool/system.py
 -rw-rw-rw-  2.0 fat      597 b- defN 23-Apr-04 05:43 sj_tool/util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:40 sj_tool/db/__init__.py
 -rw-rw-rw-  2.0 fat     5626 b- defN 23-Apr-08 09:02 sj_tool/db/mongo.py
 -rw-rw-rw-  2.0 fat     1237 b- defN 23-Apr-08 08:39 sj_tool/db/mysql.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-27 08:29 sj_tool/fjsp/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-27 08:30 sj_tool/fjsp/entity/__init__.py
--rw-rw-rw-  2.0 fat      463 b- defN 23-Apr-08 16:59 sj_tool/fjsp/entity/changeover.py
--rw-rw-rw-  2.0 fat      663 b- defN 23-Apr-08 16:47 sj_tool/fjsp/entity/job.py
--rw-rw-rw-  2.0 fat      374 b- defN 23-Mar-27 11:20 sj_tool/fjsp/entity/machine.py
--rw-rw-rw-  2.0 fat      617 b- defN 23-Mar-27 11:02 sj_tool/fjsp/entity/operation.py
--rw-rw-rw-  2.0 fat      109 b- defN 23-Apr-08 16:59 sj_tool/fjsp/entity/product.py
+-rw-rw-rw-  2.0 fat      565 b- defN 23-Apr-09 06:28 sj_tool/fjsp/entity/changeover.py
+-rw-rw-rw-  2.0 fat      897 b- defN 23-Apr-10 09:07 sj_tool/fjsp/entity/global_pool.py
+-rw-rw-rw-  2.0 fat      703 b- defN 23-Apr-09 09:06 sj_tool/fjsp/entity/job.py
+-rw-rw-rw-  2.0 fat      411 b- defN 23-Apr-09 05:22 sj_tool/fjsp/entity/machine.py
+-rw-rw-rw-  2.0 fat      718 b- defN 23-Apr-09 03:28 sj_tool/fjsp/entity/operation.py
+-rw-rw-rw-  2.0 fat      113 b- defN 23-Apr-09 09:02 sj_tool/fjsp/entity/product.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-30 02:45 sj_tool/logger/__init__.py
 -rw-rw-rw-  2.0 fat     1866 b- defN 23-Apr-08 12:57 sj_tool/logger/text_logger.py
--rw-rw-rw-  2.0 fat     2062 b- defN 23-Apr-08 11:50 sj_tool/logger/visual_logger.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-08 17:05 sj_tool-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-08 17:05 sj_tool-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-08 17:05 sj_tool-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1887 b- defN 23-Apr-08 17:05 sj_tool-1.0.4.dist-info/RECORD
-24 files, 18992 bytes uncompressed, 7211 bytes compressed:  62.0%
+-rw-rw-rw-  2.0 fat     2718 b- defN 23-Apr-09 03:19 sj_tool/logger/visual_logger.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-10 09:36 sj_tool-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 09:36 sj_tool-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-10 09:36 sj_tool-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1977 b- defN 23-Apr-10 09:36 sj_tool-1.0.5.dist-info/RECORD
+25 files, 21511 bytes uncompressed, 8093 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -33,14 +33,17 @@
 
 Filename: sj_tool/fjsp/entity/__init__.py
 Comment: 
 
 Filename: sj_tool/fjsp/entity/changeover.py
 Comment: 
 
+Filename: sj_tool/fjsp/entity/global_pool.py
+Comment: 
+
 Filename: sj_tool/fjsp/entity/job.py
 Comment: 
 
 Filename: sj_tool/fjsp/entity/machine.py
 Comment: 
 
 Filename: sj_tool/fjsp/entity/operation.py
@@ -54,20 +57,20 @@
 
 Filename: sj_tool/logger/text_logger.py
 Comment: 
 
 Filename: sj_tool/logger/visual_logger.py
 Comment: 
 
-Filename: sj_tool-1.0.4.dist-info/METADATA
+Filename: sj_tool-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: sj_tool-1.0.4.dist-info/WHEEL
+Filename: sj_tool-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: sj_tool-1.0.4.dist-info/top_level.txt
+Filename: sj_tool-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: sj_tool-1.0.4.dist-info/RECORD
+Filename: sj_tool-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sj_tool/scheduler.py

```diff
@@ -1,40 +1,55 @@
 from apscheduler.schedulers.blocking import BlockingScheduler
 from apscheduler.schedulers.background import BackgroundScheduler
 
 
-def add_interval_job(job_fn, seconds, use_background_scheduler=True, args=None):
-    """
-    添加定期执行的任务
-    :param job_fn: 要运行的函数
-    :param seconds: 间隔时间，单位：秒
-    :param use_background_scheduler: 是否使用后台线程运行任务。若为True，则不会阻塞主线程
-    :param args: 要运行函数的参数
-    :return:
-    """
-    # 注意：BlockingScheduler会阻塞当前线程，直到调度器被关闭。
-    # 创建一个调度器实例
-    scheduler = BackgroundScheduler() if use_background_scheduler else BlockingScheduler()
-    # 添加一个定时任务
-    scheduler.add_job(job_fn, "interval", seconds=seconds, args=args)
-    # 开始调度任务
-    scheduler.start()
-
-
-def add_fix_time_job(job_fn, hour, minute=0, second=0, use_background_scheduler=True, args=None):
-    """
-    添加定期执行的任务
-    :param job_fn: 要运行的函数
-    :param hour: 时
-    :param minute: 分
-    :param second: 秒
-    :param use_background_scheduler: 是否使用后台线程运行任务。若为True，则不会阻塞主线程
-    :param args: 要运行函数的参数
-    :return:
-    """
-    # 注意：BlockingScheduler会阻塞当前线程，直到调度器被关闭。
-    # 创建一个调度器实例
-    scheduler = BackgroundScheduler() if use_background_scheduler else BlockingScheduler()
-    # 添加一个定时任务
-    scheduler.add_job(job_fn, "cron", hour=hour, minute=minute, second=second, args=args)
-    # 开始调度任务
-    scheduler.start()
+class Scheduler(object):
+    def __init__(self, background=True):
+        """
+        :param background: 是否使用后台线程运行任务。若为True，则不会阻塞主线程
+        """
+        self.scheduler = BackgroundScheduler() if background else BlockingScheduler()
+
+    def add_interval_job(self, job_fn, seconds, job_store="default", args=None) -> str:
+        """
+        添加定期执行的任务
+        :param job_fn: 要运行的函数
+        :param seconds: 间隔时间，单位：秒
+        :param job_store: 用户可自定义的job空间，借助这个用户可以将job分类，加入到不同的jobstore，方便管理
+        :param args: 要运行函数的参数
+        :return:
+        """
+        # 注意：BlockingScheduler会阻塞当前线程，直到调度器被关闭。
+        # 添加一个定时任务
+        job = self.scheduler.add_job(job_fn, "interval", seconds=seconds, jobstore=job_store, args=args)
+        return job.id
+
+    def add_fix_time_job(self, job_fn, hour, minute=0, second=0, job_store="default", args=None) -> str:
+        """
+        添加定期执行的任务
+        :param job_fn: 要运行的函数
+        :param hour: 时
+        :param minute: 分
+        :param second: 秒
+        :param job_store: 用户可自定义的job空间，借助这个用户可以将job分类，加入到不同的jobstore，方便管理
+        :param args: 要运行函数的参数
+        :return: str, job的id
+        """
+        # 注意：BlockingScheduler会阻塞当前线程，直到调度器被关闭。
+        # 添加一个定时任务
+        job = self.scheduler.add_job(
+            job_fn, "cron", hour=hour, minute=minute, second=second, jobstore=job_store, args=args
+        )
+        return job.id
+
+    def start(self):
+        # 开始调度任务
+        self.scheduler.start()
+
+    def shutdown(self):
+        self.scheduler.shutdown()
+
+    def remove_jobs(self, job_store, job_id=None):
+        if job_id is None:
+            self.scheduler.remove_all_jobs(job_store)
+        else:
+            self.scheduler.remove_job(job_id, job_store)
```

## sj_tool/fjsp/entity/changeover.py

```diff
@@ -1,11 +1,15 @@
-class OperationType(object):
-    def __init__(self, idx, name):
-        self.id = idx
+from typing import Dict
+
+
+class BasicOpInfo(object):
+    def __init__(self, op_type, name, machine_dict: Dict):
+        self.op_type = op_type
         self.name = name
+        self.machine_dict = machine_dict
 
 
 class Changeover(object):
     def __init__(self):
         self.info = {}
 
     def add(self, pre_mtm, pre_op_type, cur_mtm, cur_op_type, processing_time):
```

## sj_tool/fjsp/entity/job.py

```diff
@@ -1,12 +1,14 @@
+from typing import Union
+
 import pandas as pd
 
 
 class BaseJob(object):
-    def __init__(self, job_id: str, product_code, arrival_time: str, ots_time: str, demand: float):
+    def __init__(self, job_id: Union[int, str], product_code, arrival_time: str, ots_time: str, demand: float):
         """
 
         :param job_id:
         :param product_code: 产品编码
         :param arrival_time: job到达时间，即最早可开始时间
         :param ots_time: 截止时间
         :param demand: 需求量
```

## sj_tool/fjsp/entity/machine.py

```diff
@@ -1,13 +1,14 @@
 from typing import List
 
 
-class Machine(object):
-    def __init__(self, machine_id, available_ops: List[str], unit_times):
+class BaseMachine(object):
+    def __init__(self, idx, name, available_ops: List[str] = [], unit_times={}):
         """
 
         :param machine_id:
         :param available_ops:
         """
-        self.id = machine_id
+        self.id = idx
+        self.name = name
         self.available_ops = available_ops
-        self.unit_times = unit_times  # {('product_id','process'):单个的节拍 }
+        self.unit_times = unit_times  # {('product_id','operation_type'):单个的节拍 }
```

## sj_tool/fjsp/entity/operation.py

```diff
@@ -1,17 +1,20 @@
-from typing import List, Tuple
+from typing import List, Tuple, Dict
 
 
-class Operation:
-    def __init__(self, job_id, op_id, machine_times: List[Tuple[int, float]] = None):
+class BaseOperation:
+    def __init__(self, idx, job_id, op_type, machine_times: Dict[int, float] = None):
         """
 
-        :param op_id:操作的id
-        :param machine_times: 操作在不同机器上的所需时间列表，例：[(0,2),(1,3),(2,4)],
+        :param idx: 工序id
+        :param job_id: 工单id
+        :param op_type: 工序类型
+        :param machine_times: 操作在不同机器上的所需时间列表，例：{1:2,2:2,3:4},
                 其中每个tuple的第一个元素表示机器id，第二个元素表示工序在对应机器上的单个所需时间
         """
+        self.id = idx
         self.job_id = job_id
-        self.id = op_id
+        self.op_type = op_type
         # op ids
         self.pre_ops = []
         self.next_ops = []
         self.machine_times = machine_times
```

## sj_tool/fjsp/entity/product.py

```diff
@@ -1,4 +1,4 @@
-class Product(object):
+class BaseProduct(object):
     def __init__(self, idx, name):
         self.id = idx
         self.name = name
```

## sj_tool/logger/visual_logger.py

```diff
@@ -1,18 +1,21 @@
 import wave
+
+import loguru
 import numpy as np
 
 from typing import List, Union
 from visualdl import LogWriter
 from tensorboardX import SummaryWriter
 
 
 class VisualLogger(object):
-    def __init__(self, logdir, use_visualdl=True):
+    def __init__(self, logdir, use_visualdl=True, text_logger: loguru.Logger = None):
         self.writer = LogWriter(logdir) if use_visualdl else SummaryWriter(logdir)
+        self.text_logger = text_logger
 
     def add_scalar(self, tag: str, value: Union[str, int, float], step: int):
         self.writer.add_scalar(tag, value, step)
 
     def add_image(self, tag: str, img: np.ndarray, step: int):
         self.writer.add_image(tag=tag, img=img, step=step)
 
@@ -32,17 +35,29 @@
         num_thresholds,
     ):
         self.writer.add_pr_curve(
             tag=tag, labels=labels, predictions=predictions, step=step, num_thresholds=num_thresholds
         )
 
     def add_hyper_params(self, hparams_dict, metrics_list):
+        if not isinstance(self.writer, LogWriter):
+            if self.text_logger is not None:
+                self.text_logger.error(
+                    "Func add_hyper_params is not available when you are not using visualdl.LogWriter"
+                )
+            return
         self.writer.add_hparams(hparams_dict=hparams_dict, metrics_list=metrics_list)
 
     def add_hyper_param_value(self, metric, value, step):
+        if not isinstance(self.writer, LogWriter):
+            if self.text_logger is not None:
+                self.text_logger.error(
+                    "Func add_hyper_params is not available when you are not using visualdl.LogWriter"
+                )
+            return
         self.writer.add_scalar(metric, value, step)
 
     @staticmethod
     def _read_audio_data(audio_path):
         """
         Get audio data.
         """
```

## Comparing `sj_tool-1.0.4.dist-info/RECORD` & `sj_tool-1.0.5.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 sj_tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/email_sender.py,sha256=qxNj5bQ31yzF1bi2XLIxJq5akw-vksZLOS9L5HdM5p8,476
 sj_tool/file.py,sha256=NsbZm_9UGni8CKoZEL9mMFwX7u2R2DXA-HtuUS1iaPw,155
 sj_tool/json.py,sha256=yG7paERY6nUtF51kz5ZXp396TKT-UgIyb0teAXeKD5Q,313
-sj_tool/scheduler.py,sha256=dZJdlvgWuDurNro3ZZ1dgA6qqoqCLSGFzPekS0Tkkx0,1710
+sj_tool/scheduler.py,sha256=3NLG6IhyKXMHIkJgovyndwd0qYmWWxWrLjDHVY5OG2c,2302
 sj_tool/system.py,sha256=xQxxnAKZ8yW8LJZlw0MhpRyQ_p1LnqwlKnuwgiFdqgI,245
 sj_tool/util.py,sha256=cFqbYbJ_NzqG2OeEF8IFrV7wjsDcULZmOa7UgatZF84,597
 sj_tool/db/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/db/mongo.py,sha256=oUDrhYV_sOq8M9KNFK_QDExCWQ070T1nksp8XzGtDs4,5626
 sj_tool/db/mysql.py,sha256=o9tidq_q9TkDbJXUb6KTMf9O9cJMZeL3rCsADCmroBQ,1237
 sj_tool/fjsp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/fjsp/entity/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sj_tool/fjsp/entity/changeover.py,sha256=LKGrTW1pppF8zEP6fOXBYYmUa2hjtkpoN73OkGI65p0,463
-sj_tool/fjsp/entity/job.py,sha256=v3Co8jowTkjtDihATSsScKFjl9vwXxqKxuMIzm9M6-g,663
-sj_tool/fjsp/entity/machine.py,sha256=F0IDbnE-Jp5h6EaTmZ19PIOxLDtZIvtPyUgC3-nFDK0,374
-sj_tool/fjsp/entity/operation.py,sha256=JL3pza2IeJIvGwru5ieWSdwvN8DWHGR7XIr1TW2gPdQ,617
-sj_tool/fjsp/entity/product.py,sha256=YTYKXvDH0D6AkOhyONP47POeOidHzSLgLmiXWNXnR6k,109
+sj_tool/fjsp/entity/changeover.py,sha256=ORGpGQ41ac0ztSqjf48k8Zm3mUl2LXSiupLeBL4rRXY,565
+sj_tool/fjsp/entity/global_pool.py,sha256=9-pE3_NIZqVWDM0TrGosycMfzaE1iQov8mSZ3-LZEPo,897
+sj_tool/fjsp/entity/job.py,sha256=Jj5OGh1-X1LhIfy4WnkffeGL7S0StTUxOnNj0nqCbWA,703
+sj_tool/fjsp/entity/machine.py,sha256=zBjVt5VYEuJlqA4yHzzEw9wlbVSAaJHlgj0lweSNaSw,411
+sj_tool/fjsp/entity/operation.py,sha256=_wI52FmRa80I_SvMm5fB0ZX4cQUAmhY3jtbUuN8dgsY,718
+sj_tool/fjsp/entity/product.py,sha256=IzErQu-Hm0d8rSdWA3Z-HYaYBDmNUbyOMBumYc1dwuU,113
 sj_tool/logger/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/logger/text_logger.py,sha256=hNPAxGVOsL46q-9cd-o-S7WV3CL52vlhD7HWKRAeh2Y,1866
-sj_tool/logger/visual_logger.py,sha256=7X73d7-xHmG2JDiUtFWRVBiNXb8mp91T4nX_sBB1wbc,2062
-sj_tool-1.0.4.dist-info/METADATA,sha256=WP9CsV4Q-NFUlq-1MsUMjqIbGM31MP0yCoF4Ff-E7Bk,492
-sj_tool-1.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sj_tool-1.0.4.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
-sj_tool-1.0.4.dist-info/RECORD,,
+sj_tool/logger/visual_logger.py,sha256=AfKNWJpTb-Odm4gWUyVRXIykiXyvfrdAjukwugCD6os,2718
+sj_tool-1.0.5.dist-info/METADATA,sha256=dbzMNVqp7rxan2b2dfyLVUai-d8eWwmEEE9Q-7C7dIY,492
+sj_tool-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sj_tool-1.0.5.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
+sj_tool-1.0.5.dist-info/RECORD,,
```

