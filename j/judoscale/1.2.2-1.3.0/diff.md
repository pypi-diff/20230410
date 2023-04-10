# Comparing `tmp/judoscale-1.2.2.tar.gz` & `tmp/judoscale-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "judoscale-1.2.2.tar", max compression
+gzip compressed data, was "judoscale-1.3.0.tar", max compression
```

## Comparing `judoscale-1.2.2.tar` & `judoscale-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1066 2023-04-03 12:08:54.785610 judoscale-1.2.2/LICENSE
--rw-r--r--   0        0        0    12620 2023-04-03 12:08:54.785610 judoscale-1.2.2/README.md
--rw-r--r--   0        0        0        0 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/__init__.py
--rw-r--r--   0        0        0      970 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/celery/__init__.py
--rw-r--r--   0        0        0     3987 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/celery/collector.py
--rw-r--r--   0        0        0        0 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/core/__init__.py
--rw-r--r--   0        0        0      642 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/core/adapter.py
--rw-r--r--   0        0        0     3396 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/core/config.py
--rw-r--r--   0        0        0       56 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/core/logger.py
--rw-r--r--   0        0        0     3641 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/core/metric.py
--rw-r--r--   0        0        0     2526 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/core/metrics_collectors.py
--rw-r--r--   0        0        0     1564 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/core/metrics_store.py
--rw-r--r--   0        0        0     3811 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/core/reporter.py
--rw-r--r--   0        0        0      192 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/django/__init__.py
--rw-r--r--   0        0        0     1329 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/django/apps.py
--rw-r--r--   0        0        0     1054 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/django/middleware.py
--rw-r--r--   0        0        0       73 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/flask/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/flask/judoscale.py
--rw-r--r--   0        0        0      708 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/rq/__init__.py
--rw-r--r--   0        0        0     1445 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/rq/apps.py
--rw-r--r--   0        0        0     2763 2023-04-03 12:08:54.785610 judoscale-1.2.2/judoscale/rq/collector.py
--rw-r--r--   0        0        0     1348 2023-04-03 12:08:54.785610 judoscale-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    14020 1970-01-01 00:00:00.000000 judoscale-1.2.2/setup.py
--rw-r--r--   0        0        0    13780 1970-01-01 00:00:00.000000 judoscale-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-10 09:42:06.457922 judoscale-1.3.0/LICENSE
+-rw-r--r--   0        0        0    14699 2023-04-10 09:42:06.457922 judoscale-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/asgi/__init__.py
+-rw-r--r--   0        0        0     1355 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/asgi/middleware.py
+-rw-r--r--   0        0        0      970 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/celery/__init__.py
+-rw-r--r--   0        0        0     4641 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/celery/collector.py
+-rw-r--r--   0        0        0        0 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/core/__init__.py
+-rw-r--r--   0        0        0      642 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/core/adapter.py
+-rw-r--r--   0        0        0     3422 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/core/config.py
+-rw-r--r--   0        0        0       56 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/core/logger.py
+-rw-r--r--   0        0        0     4271 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/core/metric.py
+-rw-r--r--   0        0        0     2526 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/core/metrics_collectors.py
+-rw-r--r--   0        0        0     1564 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/core/metrics_store.py
+-rw-r--r--   0        0        0     3811 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/core/reporter.py
+-rw-r--r--   0        0        0      192 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/django/__init__.py
+-rw-r--r--   0        0        0     1329 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/django/apps.py
+-rw-r--r--   0        0        0     1054 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/django/middleware.py
+-rw-r--r--   0        0        0       73 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/flask/__init__.py
+-rw-r--r--   0        0        0     1288 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/flask/judoscale.py
+-rw-r--r--   0        0        0      708 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/rq/__init__.py
+-rw-r--r--   0        0        0     1445 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/rq/apps.py
+-rw-r--r--   0        0        0     3080 2023-04-10 09:42:06.457922 judoscale-1.3.0/judoscale/rq/collector.py
+-rw-r--r--   0        0        0     1421 2023-04-10 09:42:06.457922 judoscale-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    16205 1970-01-01 00:00:00.000000 judoscale-1.3.0/setup.py
+-rw-r--r--   0        0        0    15935 1970-01-01 00:00:00.000000 judoscale-1.3.0/PKG-INFO
```

### Comparing `judoscale-1.2.2/LICENSE` & `judoscale-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/README.md` & `judoscale-1.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 It is recommended to install the specific web framework and/or background job library support as "extras" to the `judoscale` PyPI package. This ensures that checking if the installed web framework and/or background task processing library is supported happens at dependency resolution time.
 
 ## Supported web frameworks
 
 - [x] [Django](#using-judoscale-with-django)
 - [x] [Flask](#using-judoscale-with-flask)
-- [ ] FastAPI
+- [x] [FastAPI](#using-judoscale-with-fastapi)
 
 ## Supported job processors
 
 - [x] [Celery](#using-judoscale-with-celery-and-redis) (with Redis 6.0+ as the broker)
 - [x] [RQ](#using-judoscale-with-rq)
 
 # Using Judoscale with Django
@@ -87,14 +87,51 @@
     # Log level defaults to ENV["LOG_LEVEL"] or "INFO".
     "LOG_LEVEL": "DEBUG",
 }
 ```
 
 Note the [official recommendations for configuring Flask](https://flask.palletsprojects.com/en/2.2.x/config/#configuration-best-practices).
 
+# Using Judoscale with FastAPI
+
+Install Judoscale for FastAPI with:
+
+```sh
+$ pip install 'judoscale[fastapi]'
+```
+
+Since FastAPI uses [Starlette](https://www.starlette.io/), an ASGI framework, the integration is packaged into [ASGI middleware](https://asgi.readthedocs.io/en/latest/specs/main.html#middleware). Import the middleare class and register it with your FastAPI app:
+
+```py
+# app.py
+
+from judoscale.asgi.middleware import RequestQueueTimeMiddleware
+
+# If your app is a top-level global
+
+app = FastAPI()
+app.add_middleware(RequestQueueTimeMiddleware)
+
+
+# If your app uses the application factory pattern
+
+def create_app():
+    app = FastAPI()
+    app.add_middleware(RequestQueueTimeMiddleware)
+    return app
+```
+
+This sets up the Judoscale extension to capture request queue times.
+
+Optionally, you can override Judoscale's configuration by passing in extra configuration to the `add_middleware` method:
+
+```py
+app.add_middleware(RequestQueueTimeMiddleware, extra_config={"LOG_LEVEL": "DEBUG"})
+```
+
 # Using Judoscale with Celery and Redis
 
 Install Judoscale for Celery with:
 
 ```sh
 $ pip install 'judoscale[celery-redis]'
 ```
@@ -148,15 +185,25 @@
         # reported for the first MAX_QUEUES queues.
         # Defaults to 20.
         "MAX_QUEUES": 20,
 
         # Specify a list of known queues to report metrics for.
         # MAX_QUEUES is still honoured.
         # Defaults to empty list (report metrics for discovered queues).
-        "QUEUES": []
+        "QUEUES": [],
+
+        # Enable or disable (default) tracking how many jobs are currently being
+        # processed in each queue.
+        # This allows Judoscale to avoid downscaling workers that are executing jobs.
+        # See documentation: https://judoscale.com/docs/long-running-jobs-ruby#enable-long-running-job-support-in-the-dashboard
+        # NOTE: This option requires workers to have unique names. If you are running
+        # multiple Celery workers on the same machine, make sure to give each
+        # worker a distinct name.
+        # More information: https://docs.celeryq.dev/en/stable/userguide/workers.html#starting-the-worker
+        "TRACK_BUSY_JOBS": False,
     }
 }
 ```
 
 > :warning: **NOTE:** Calling `judoscale_celery` turns on sending [`task-sent`](https://docs.celeryq.dev/en/stable/userguide/configuration.html#task-send-sent-event) events. This is required for the Celery integration with Judoscale to work.
 
 ### Judoscale with Celery and Flask
@@ -238,15 +285,21 @@
         # reported for the first MAX_QUEUES queues.
         # Defaults to 20.
         "MAX_QUEUES": 20,
 
         # Specify a list of known queues to report metrics for.
         # MAX_QUEUES is still honoured.
         # Defaults to empty list (report metrics for discovered queues).
-        "QUEUES": []
+        "QUEUES": [],
+
+        # Enable or disable (default) tracking how many jobs are currently being
+        # processed in each queue.
+        # This allows Judoscale to avoid downscaling workers that are executing jobs.
+        # See documentation: https://judoscale.com/docs/long-running-jobs-ruby#enable-long-running-job-support-in-the-dashboard
+        "TRACK_BUSY_JOBS": False,
 }
 ```
 
 ### Judoscale with RQ and Flask
 
 The recommended way to initialise Judoscale for RQ is in the application factory:
```

### Comparing `judoscale-1.2.2/judoscale/celery/__init__.py` & `judoscale-1.3.0/judoscale/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/celery/collector.py` & `judoscale-1.3.0/judoscale/celery/collector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import time
+from collections import defaultdict
 from threading import Thread
 from typing import List, Optional, Set
 
 from celery import Celery
 from kombu import Connection
 from redis import Redis
 
@@ -12,14 +13,15 @@
 from judoscale.core.metric import Metric
 from judoscale.core.metrics_collectors import JobMetricsCollector
 
 DEFAULTS = {
     "ENABLED": True,
     "MAX_QUEUES": 20,
     "QUEUES": [],
+    "TRACK_BUSY_JOBS": False,
 }
 
 
 class TaskSentHandler(Thread):
     def __init__(
         self,
         collector: "CeleryMetricsCollector",
@@ -59,14 +61,17 @@
         self.redis: Redis = connection.channel().client
 
         if not self.is_supported_redis_version:
             raise RuntimeError(
                 "Unsupported Redis server version. Minimum Redis version is 6.0."
             )
 
+        if self.adapter_config["TRACK_BUSY_JOBS"]:
+            self.inspect = broker.control.inspect()
+
         self._celery_queues: Set[str] = set()
         self.task_sent_handler = TaskSentHandler(self, connection)
         logger.debug(f"Redis is at {self.redis.connection_pool}")
 
         system_queues = {"unacked", "unacked_index"}
         user_queues = {
             q.decode("utf-8") if type(q) is bytes else q
@@ -101,14 +106,25 @@
         return None
 
     def collect(self) -> List[Metric]:
         metrics = []
         if not self.should_collect:
             return metrics
 
+        if self.adapter_config["TRACK_BUSY_JOBS"] and (
+            workers_tasks := self.inspect.active()
+        ):
+            busy_counts = defaultdict(lambda: 0)
+            for active_tasks in workers_tasks.values():
+                for task in active_tasks:
+                    busy_counts[task["delivery_info"]["routing_key"]] += 1
+
+            for queue, count in busy_counts.items():
+                metrics.append(Metric.for_busy_queue(queue_name=queue, busy_jobs=count))
+
         logger.debug(f"Collecting metrics for queues {list(self.queues)}")
         for queue in self.queues:
             if task := self.oldest_task(queue):
                 if published_at := task.get("properties", {}).get("published_at"):
                     metrics.append(
                         Metric.for_queue(queue_name=queue, oldest_job_ts=published_at)
                     )
```

### Comparing `judoscale-1.2.2/judoscale/core/adapter.py` & `judoscale-1.3.0/judoscale/core/adapter.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/core/config.py` & `judoscale-1.3.0/judoscale/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 
         runtime_container = RuntimeContainer(service_id, instance, service_type)
         api_base_url = f"https://adapter.judoscale.com/api/{service_id}"
         return cls(runtime_container, api_base_url, env)
 
     def update(self, new_config: Mapping):
         for k, v in new_config.items():
+            k = k.upper()
             if k in self and isinstance(self[k], dict) and isinstance(v, dict):
                 self[k].update(v)
             else:
                 self[k] = v
         self._prepare_logging()
 
     def merge(self, new_config: Mapping):
```

### Comparing `judoscale-1.2.2/judoscale/core/metric.py` & `judoscale-1.3.0/judoscale/core/metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -103,7 +103,28 @@
 
         oldest_job_ts:
             The Unix timestamp of the oldest job in the queue.
         """
         metric = Metric.new(start_ms=int(oldest_job_ts * 1000), queue_name=queue_name)
         logger.debug(f"queue_name={queue_name}, queue_time={metric.value}ms")
         return metric
+
+    @classmethod
+    def for_busy_queue(cls, queue_name: str, busy_jobs: int) -> "Metric":
+        """
+        Log and return a Metric instance for the number of jobs being processed
+        for a given queue.
+
+        queue_name:
+            The name of the queue.
+
+        busy_jobs:
+            The number of jobs being processed for the given queue.
+        """
+        metric = Metric(
+            measurement="busy",
+            queue_name=queue_name,
+            value=busy_jobs,
+            timestamp=time.time(),
+        )
+        logger.debug(f"queue_name={queue_name}, busy_jobs={metric.value}")
+        return metric
```

### Comparing `judoscale-1.2.2/judoscale/core/metrics_collectors.py` & `judoscale-1.3.0/judoscale/core/metrics_collectors.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/core/metrics_store.py` & `judoscale-1.3.0/judoscale/core/metrics_store.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/core/reporter.py` & `judoscale-1.3.0/judoscale/core/reporter.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/django/apps.py` & `judoscale-1.3.0/judoscale/django/apps.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/django/middleware.py` & `judoscale-1.3.0/judoscale/django/middleware.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/flask/judoscale.py` & `judoscale-1.3.0/judoscale/flask/judoscale.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/rq/__init__.py` & `judoscale-1.3.0/judoscale/rq/__init__.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/rq/apps.py` & `judoscale-1.3.0/judoscale/rq/apps.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.2.2/judoscale/rq/collector.py` & `judoscale-1.3.0/judoscale/rq/collector.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from judoscale.core.metric import Metric
 from judoscale.core.metrics_collectors import JobMetricsCollector
 
 DEFAULTS = {
     "ENABLED": True,
     "MAX_QUEUES": 20,
     "QUEUES": [],
+    "TRACK_BUSY_JOBS": False,
 }
 
 
 class RQMetricsCollector(JobMetricsCollector):
     def __init__(self, config: Config, redis: Redis):
         super().__init__(config=config)
 
@@ -49,15 +50,24 @@
     def collect(self) -> List[Metric]:
         metrics = []
         if not self.should_collect:
             return metrics
 
         logger.debug(f"Collecting metrics for queues {list(self.queues)}")
         queues = [Queue(name=q, connection=self.redis) for q in self.queues]
+
         for queue in queues:
+            if self.adapter_config["TRACK_BUSY_JOBS"]:
+                metrics.append(
+                    Metric.for_busy_queue(
+                        queue_name=queue.name,
+                        busy_jobs=queue.started_job_registry.count,
+                    )
+                )
+
             if job := self.oldest_job(queue):
                 if job.enqueued_at is not None:
                     # RQ stores `enqueued_at` as a naive datetime object, which
                     # means it doesn't have any timezone information associated
                     # with it.
                     # But since the time is, in fact, in UTC, we can just replace
                     # the timezone with UTC and then convert it to a timestamp.
```

### Comparing `judoscale-1.2.2/pyproject.toml` & `judoscale-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "judoscale"
-version = "1.2.2"
+version = "1.3.0"
 description = "Official Python adapter for Judoscale — the advanced autoscaler for Heroku"
 authors = [
     "Adam McCrea <adam@adamlogic.com>",
     "Mara <mara@multiplace.org>",
     "Karl Sutt <karl@sutt.ee>"
 ]
 license = "MIT"
@@ -19,26 +19,28 @@
 packages = [{include = "judoscale"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "<3.0.0"
 django = { version = ">=2.1.0,<5.0.0", optional = true }
 flask = { version = ">=1.1.0,<3.0.0", optional = true }
+fastapi = { version = "< 1.0.0", optional = true }
 celery = { version = ">=4.4.0,<6.0.0", extras = ["redis"], optional = true }
 rq = { version = ">=1.0.0,<2.0.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.2"
 flake8 = { version = "^6.0.0", python = ">=3.8.1,<4.0.0" }
 pytest = "^7.2.2"
 
 [tool.poetry.extras]
 django = ["django"]
 flask = ["flask"]
+fastapi = ["fastapi"]
 celery-redis = ["celery"]
 rq = ["rq"]
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
```

### Comparing `judoscale-1.2.2/setup.py` & `judoscale-1.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['judoscale',
+ 'judoscale.asgi',
  'judoscale.celery',
  'judoscale.core',
  'judoscale.django',
  'judoscale.flask',
  'judoscale.rq']
 
 package_data = \
@@ -14,22 +15,23 @@
 
 install_requires = \
 ['requests<3.0.0']
 
 extras_require = \
 {'celery-redis': ['celery[redis]>=4.4.0,<6.0.0'],
  'django': ['django>=2.1.0,<5.0.0'],
+ 'fastapi': ['fastapi<1.0.0'],
  'flask': ['flask>=1.1.0,<3.0.0'],
  'rq': ['rq>=1.0.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'judoscale',
-    'version': '1.2.2',
+    'version': '1.3.0',
     'description': 'Official Python adapter for Judoscale — the advanced autoscaler for Heroku',
-    'long_description': '# Judoscale\n\nThis is the official Python adapter for [Judoscale](https://elements.heroku.com/addons/judoscale). You can use Judoscale without it, but this gives you request queue time metrics and job queue time (for supported job processors).\n\nIt is recommended to install the specific web framework and/or background job library support as "extras" to the `judoscale` PyPI package. This ensures that checking if the installed web framework and/or background task processing library is supported happens at dependency resolution time.\n\n## Supported web frameworks\n\n- [x] [Django](#using-judoscale-with-django)\n- [x] [Flask](#using-judoscale-with-flask)\n- [ ] FastAPI\n\n## Supported job processors\n\n- [x] [Celery](#using-judoscale-with-celery-and-redis) (with Redis 6.0+ as the broker)\n- [x] [RQ](#using-judoscale-with-rq)\n\n# Using Judoscale with Django\n\nInstall Judoscale for Django with:\n\n```sh\n$ pip install \'judoscale[django]\'\n```\n\nAdd Judoscale app to `settings.py`:\n\n```python\nINSTALLED_APPS = [\n    "judoscale.django",\n    # ... other apps\n]\n```\n\nThis sets up the Judoscale middleware to capture request queue times.\n\nOptionally, you can customize Judoscale in `settings.py`:\n\n```python\nJUDOSCALE = {\n    # Log level defaults to ENV["LOG_LEVEL"] or "INFO".\n    "LOG_LEVEL": "DEBUG",\n}\n```\n\nOnce deployed, you will see your request queue time metrics available in the Judoscale UI.\n\n# Using Judoscale with Flask\n\nInstall Judoscale for Flask with:\n\n```sh\n$ pip install \'judoscale[flask]\'\n```\n\nThe Flask support for Judoscale is packaged into a Flask extension. Import the extension class and use like you normally would in a Flask application:\n\n```py\n# app.py\n\nfrom judoscale.flask import Judoscale\n\n# If your app is a top-level global\n\napp = Flask("MyFlaskApp")\napp.config.from_object(\'...\')  # or however you configure your app\njudoscale = Judoscale(app)\n\n\n# If your app uses the application factory pattern\n\njudoscale = Judoscale()\n\ndef create_app():\n    app = Flask("MyFlaskApp")\n    app.config.from_object(\'...\')  # or however you configure your app\n    judoscale.init_app(app)\n    return app\n```\n\nThis sets up the Judoscale extension to capture request queue times.\n\nOptionally, you can override Judoscale\'s own configuration via your application\'s [configuration dictionary](https://flask.palletsprojects.com/en/2.2.x/api/#flask.Flask.config). The Judoscale Flask extension looks for a top-level `"JUDOSCALE"` key in `app.config`, which should be a dictionary, and which the extension uses to configure itself as soon as `judoscale.init_app()` is called.\n\n```python\nJUDOSCALE = {\n    # Log level defaults to ENV["LOG_LEVEL"] or "INFO".\n    "LOG_LEVEL": "DEBUG",\n}\n```\n\nNote the [official recommendations for configuring Flask](https://flask.palletsprojects.com/en/2.2.x/config/#configuration-best-practices).\n\n# Using Judoscale with Celery and Redis\n\nInstall Judoscale for Celery with:\n\n```sh\n$ pip install \'judoscale[celery-redis]\'\n```\n\n> :warning: **NOTE 1:** The Judoscale Celery integration currently only works with the [Redis broker](https://docs.celeryq.dev/en/stable/getting-started/backends-and-brokers/index.html#redis). The minimum supported Redis server version is 6.0.\n\n> :warning: **NOTE 2:** Using [task priorities](https://docs.celeryq.dev/en/latest/userguide/calling.html#advanced-options) is currently not supported by `judoscale`. You can still use task priorities, but `judoscale` won\'t see and report metrics on any queues other than the default, unprioritised queue.\n\nJudoscale can automatically scale the number of Celery workers based on the queue latency (the age of the oldest pending task in the queue).\n\n## Setting up the integration\n\nTo use the Celery integration, import `judoscale_celery` and call it with the Celery app instance. `judoscale_celery` should be called after you have set up and configured the Celery instance.\n\n```py\nfrom celery import Celery\nfrom judoscale.celery import judoscale_celery\n\ncelery_app = Celery(broker="redis://localhost:6379/0")\n# Further setup\n# celery_app.conf.update(...)\n# ...\n\njudoscale_celery(celery_app)\n```\n\nThis sets up Judoscale to periodically calculate and report queue latency for each Celery queue.\n\nIf you need to change the Judoscale integration configuration, you can pass a dictionary of Judoscale configuration options to `judoscale_celery` to override the default Judoscale config variables:\n\n```py\njudoscale_celery(celery_app, extra_config={"LOG_LEVEL": "DEBUG"})\n```\n\nAn example configuration dictionary accepted by `extra_config`:\n\n```py\n{\n    "LOG_LEVEL": "INFO",\n\n    # In addition to global configuration options for the Judoscale\n    # integration above, you can also specify the following configuration\n    # options for the Celery integration.\n    "CELERY": {\n        # Enable (default) or disable the Celery integration\n        "ENABLED": True,\n\n        # Report metrics on up to MAX_QUEUES queues.\n        # The list of discovered queues are sorted by the length\n        # of the queue name (shortest first) and metrics are\n        # reported for the first MAX_QUEUES queues.\n        # Defaults to 20.\n        "MAX_QUEUES": 20,\n\n        # Specify a list of known queues to report metrics for.\n        # MAX_QUEUES is still honoured.\n        # Defaults to empty list (report metrics for discovered queues).\n        "QUEUES": []\n    }\n}\n```\n\n> :warning: **NOTE:** Calling `judoscale_celery` turns on sending [`task-sent`](https://docs.celeryq.dev/en/stable/userguide/configuration.html#task-send-sent-event) events. This is required for the Celery integration with Judoscale to work.\n\n### Judoscale with Celery and Flask\n\nDepending on how you\'ve structured your Flask app, you should call `judoscale_celery` after your application has finished configuring the Celery app instance. If you have followed the [Flask guide](https://flask.palletsprojects.com/en/2.2.x/patterns/celery/) in the Flask documentation, the easiest place to initialise the Judoscale integration is in the application factory:\n\n```py\ndef create_app():\n    app = Flask(__name__)\n    app.config.from_object(...) # or however you configure your app\n    celery_app = celery_init_app(app)\n    # Initialise the Judoscale integration\n    judoscale_celery(celery_app, extra_config=app.config["JUDOSCALE"])\n    return app\n```\n\n### Judoscale with Celery and Django\n\nIf you have followed the [Django guide](https://docs.celeryq.dev/en/stable/django/first-steps-with-django.html) in the Celery documentation, you should have a module where you initialise the Celery app instance, auto-discover tasks, etc. You should call `judoscale_celery` after you have configured the Celery app instance:\n\n```py\nfrom celery import Celery\nfrom django.conf import settings\nfrom judoscale.celery import judoscale_celery\n\napp = Celery()\napp.config_from_object("django.conf:settings", namespace="CELERY")\napp.autodiscover_tasks()\n# Initialise the Judoscale integration\njudoscale_celery(app, extra_config=settings.JUDOSCALE)\n```\n\n# Using Judoscale with RQ\n\nInstall Judoscale for RQ with:\n\n```sh\n$ pip install \'judoscale[rq]\'\n```\n\nJudoscale can automatically scale the number of RQ workers based on the queue latency (the age of the oldest pending task in the queue).\n\n## Setting up the integration\n\nTo use the RQ integration, import `judoscale_rq` and call it with an instance of `Redis` pointing to the same Redis database that RQ uses.\n\n```py\nfrom redis import Redis\nfrom judoscale.rq import judoscale_rq\n\nredis = Redis(...)\njudoscale_rq(redis)\n```\n\nThis sets up Judoscale to periodically calculate and report queue latency for each RQ queue.\n\nIf you need to change the Judoscale integration configuration, you can pass a dictionary of Judoscale configuration options to `judoscale_rq` to override the default Judoscale config variables:\n\n```py\njudoscale_rq(redis, extra_config={"LOG_LEVEL": "DEBUG"})\n```\n\nAn example configuration dictionary accepted by `extra_config`:\n\n```py\n {\n    "LOG_LEVEL": "INFO",\n\n    # In addition to global configuration options for the Judoscale\n    # integration above, you can also specify the following configuration\n    # options for the RQ integration.\n    "RQ": {\n        # Enable (default) or disable the RQ integration\n        "ENABLED": True,\n\n        # Report metrics on up to MAX_QUEUES queues.\n        # The list of discovered queues are sorted by the length\n        # of the queue name (shortest first) and metrics are\n        # reported for the first MAX_QUEUES queues.\n        # Defaults to 20.\n        "MAX_QUEUES": 20,\n\n        # Specify a list of known queues to report metrics for.\n        # MAX_QUEUES is still honoured.\n        # Defaults to empty list (report metrics for discovered queues).\n        "QUEUES": []\n}\n```\n\n### Judoscale with RQ and Flask\n\nThe recommended way to initialise Judoscale for RQ is in the application factory:\n\n```py\njudoscale = Judoscale()\n\ndef create_app():\n    app = Flask(__name__)\n    app.config.from_object("...") # or however you configure your application\n    app.redis = Redis()\n\n    # Initialise the Judoscale integration for Flask\n    judoscale.init_app(app)\n\n    # Initialise the Judoscale integration for RQ\n    judoscale_rq(app.redis)\n\n    return app\n```\n\nThen, in your worker script, make sure that you create an app, which will initialise the Judoscale integration with RQ. Although not required, it\'s useful to run the worker within the Flask app context. If you have followed the [RQ on Heroku pattern](https://python-rq.org/patterns/) for setting up your RQ workers on Heroku, your worker script should look something like this:\n\n```py\nfrom rq.worker import HerokuWorker as Worker\n\napp = create_app()\n\nworker = Worker(..., connection=app.redis)\nwith app.app_context():\n    worker.work()\n```\n\nSee the [run-worker.py script](./sample-apps/flask_rq_sample/run-worker.py) for reference.\n\n### Judoscale with RQ and Django\n\nThe Judoscale integration for RQ is packaged into a separate Django app.\n\nYou should already have `judoscale.django` in your `INSTALLED_APPS`. Next, add the RQ integration app `judoscale.rq`:\n\n```python\nINSTALLED_APPS = [\n    "judoscale.django",\n    "judoscale.rq",\n    # ... other apps\n]\n```\n\nBy default, `judoscale.rq` will connect to the Redis instance as specified by the `REDIS_URL` environment variable. If that is not suitable, you can supply Redis connection information in the `JUDOSCALE` configuration dictionary under the `"REDIS"` key.\n\nAccepted formats are:\n\n- a dictionary containing a single key `"URL"` pointing to a Redis server URL, or;\n- a dictionary of configuration options corresponding to the keyword arguments of the [`Redis` constructor](https://github.com/redis/redis-py/blob/6c708c2e0511364c2c3f21fa1259de05e590632d/redis/client.py#L905).\n\n```py\nJUDOSCALE = {\n    # Configuring with a Redis server URL\n    "REDIS": {\n        "URL": os.getenv("REDISTOGO_URL")\n    }\n\n    # Configuring as kwargs to Redis(...)\n    "REDIS": {\n        "HOST": "localhost",\n        "PORT": 6379,\n        "DB": 0\n    }\n}\n```\n\nIf you are using [Django-RQ](https://github.com/rq/django-rq/tree/master), you can also pull configuration from `RQ_QUEUES` directly:\n\n```py\nRQ_QUEUES = {\n    "high_priority": {\n        "HOST": "...",\n        "PORT": 6379,\n        "DB": 0\n    },\n}\n\nJUDOSCALE = {\n    # ... other configuration options\n    "REDIS": RQ_QUEUES["high_priority"]\n}\n```\n\n> :warning: **NOTE:** Django-RQ enables configuring RQ such that different queues and workers use _different_ Redis instances. Judoscale currently only supports connecting to and monitoring queue latency on a single Redis instance.\n\n## Development\n\nThis repo includes a `sample-apps` directory containing apps you can run locally. These apps use the `judoscale` adapter, but they override `API_BASE_URL` so they\'re not connected to the real Judoscale API. Instead, they post API requests to https://requestinspector.com so you can observe the API behavior.\n\nSee the `README` in a sample app for details on how to set it up and run locally.\n\n### Contributing\n\n`judoscale` uses [Poetry](https://python-poetry.org/) for managing dependencies and packaging the project. Head over to the [installations instructions](https://python-poetry.org/docs/#installing-with-the-official-installer) and install Poetry, if needed.\n\nClone the repo with\n\n```sh\n$ git clone git@github.com:judoscale/judoscale-python.git\n$ cd judoscale-python\n```\n\nVerify that you are on a recent version of Poetry:\n\n```sh\n$ poetry --version\nPoetry (version 1.3.1)\n```\n\nInstall dependencies with Poetry and activate the virtualenv\n\n```sh\n$ poetry install --all-extras\n$ poetry shell\n```\n\nRun tests with\n\n```sh\n$ pytest\n```\n',
+    'long_description': '# Judoscale\n\nThis is the official Python adapter for [Judoscale](https://elements.heroku.com/addons/judoscale). You can use Judoscale without it, but this gives you request queue time metrics and job queue time (for supported job processors).\n\nIt is recommended to install the specific web framework and/or background job library support as "extras" to the `judoscale` PyPI package. This ensures that checking if the installed web framework and/or background task processing library is supported happens at dependency resolution time.\n\n## Supported web frameworks\n\n- [x] [Django](#using-judoscale-with-django)\n- [x] [Flask](#using-judoscale-with-flask)\n- [x] [FastAPI](#using-judoscale-with-fastapi)\n\n## Supported job processors\n\n- [x] [Celery](#using-judoscale-with-celery-and-redis) (with Redis 6.0+ as the broker)\n- [x] [RQ](#using-judoscale-with-rq)\n\n# Using Judoscale with Django\n\nInstall Judoscale for Django with:\n\n```sh\n$ pip install \'judoscale[django]\'\n```\n\nAdd Judoscale app to `settings.py`:\n\n```python\nINSTALLED_APPS = [\n    "judoscale.django",\n    # ... other apps\n]\n```\n\nThis sets up the Judoscale middleware to capture request queue times.\n\nOptionally, you can customize Judoscale in `settings.py`:\n\n```python\nJUDOSCALE = {\n    # Log level defaults to ENV["LOG_LEVEL"] or "INFO".\n    "LOG_LEVEL": "DEBUG",\n}\n```\n\nOnce deployed, you will see your request queue time metrics available in the Judoscale UI.\n\n# Using Judoscale with Flask\n\nInstall Judoscale for Flask with:\n\n```sh\n$ pip install \'judoscale[flask]\'\n```\n\nThe Flask support for Judoscale is packaged into a Flask extension. Import the extension class and use like you normally would in a Flask application:\n\n```py\n# app.py\n\nfrom judoscale.flask import Judoscale\n\n# If your app is a top-level global\n\napp = Flask("MyFlaskApp")\napp.config.from_object(\'...\')  # or however you configure your app\njudoscale = Judoscale(app)\n\n\n# If your app uses the application factory pattern\n\njudoscale = Judoscale()\n\ndef create_app():\n    app = Flask("MyFlaskApp")\n    app.config.from_object(\'...\')  # or however you configure your app\n    judoscale.init_app(app)\n    return app\n```\n\nThis sets up the Judoscale extension to capture request queue times.\n\nOptionally, you can override Judoscale\'s own configuration via your application\'s [configuration dictionary](https://flask.palletsprojects.com/en/2.2.x/api/#flask.Flask.config). The Judoscale Flask extension looks for a top-level `"JUDOSCALE"` key in `app.config`, which should be a dictionary, and which the extension uses to configure itself as soon as `judoscale.init_app()` is called.\n\n```python\nJUDOSCALE = {\n    # Log level defaults to ENV["LOG_LEVEL"] or "INFO".\n    "LOG_LEVEL": "DEBUG",\n}\n```\n\nNote the [official recommendations for configuring Flask](https://flask.palletsprojects.com/en/2.2.x/config/#configuration-best-practices).\n\n# Using Judoscale with FastAPI\n\nInstall Judoscale for FastAPI with:\n\n```sh\n$ pip install \'judoscale[fastapi]\'\n```\n\nSince FastAPI uses [Starlette](https://www.starlette.io/), an ASGI framework, the integration is packaged into [ASGI middleware](https://asgi.readthedocs.io/en/latest/specs/main.html#middleware). Import the middleare class and register it with your FastAPI app:\n\n```py\n# app.py\n\nfrom judoscale.asgi.middleware import RequestQueueTimeMiddleware\n\n# If your app is a top-level global\n\napp = FastAPI()\napp.add_middleware(RequestQueueTimeMiddleware)\n\n\n# If your app uses the application factory pattern\n\ndef create_app():\n    app = FastAPI()\n    app.add_middleware(RequestQueueTimeMiddleware)\n    return app\n```\n\nThis sets up the Judoscale extension to capture request queue times.\n\nOptionally, you can override Judoscale\'s configuration by passing in extra configuration to the `add_middleware` method:\n\n```py\napp.add_middleware(RequestQueueTimeMiddleware, extra_config={"LOG_LEVEL": "DEBUG"})\n```\n\n# Using Judoscale with Celery and Redis\n\nInstall Judoscale for Celery with:\n\n```sh\n$ pip install \'judoscale[celery-redis]\'\n```\n\n> :warning: **NOTE 1:** The Judoscale Celery integration currently only works with the [Redis broker](https://docs.celeryq.dev/en/stable/getting-started/backends-and-brokers/index.html#redis). The minimum supported Redis server version is 6.0.\n\n> :warning: **NOTE 2:** Using [task priorities](https://docs.celeryq.dev/en/latest/userguide/calling.html#advanced-options) is currently not supported by `judoscale`. You can still use task priorities, but `judoscale` won\'t see and report metrics on any queues other than the default, unprioritised queue.\n\nJudoscale can automatically scale the number of Celery workers based on the queue latency (the age of the oldest pending task in the queue).\n\n## Setting up the integration\n\nTo use the Celery integration, import `judoscale_celery` and call it with the Celery app instance. `judoscale_celery` should be called after you have set up and configured the Celery instance.\n\n```py\nfrom celery import Celery\nfrom judoscale.celery import judoscale_celery\n\ncelery_app = Celery(broker="redis://localhost:6379/0")\n# Further setup\n# celery_app.conf.update(...)\n# ...\n\njudoscale_celery(celery_app)\n```\n\nThis sets up Judoscale to periodically calculate and report queue latency for each Celery queue.\n\nIf you need to change the Judoscale integration configuration, you can pass a dictionary of Judoscale configuration options to `judoscale_celery` to override the default Judoscale config variables:\n\n```py\njudoscale_celery(celery_app, extra_config={"LOG_LEVEL": "DEBUG"})\n```\n\nAn example configuration dictionary accepted by `extra_config`:\n\n```py\n{\n    "LOG_LEVEL": "INFO",\n\n    # In addition to global configuration options for the Judoscale\n    # integration above, you can also specify the following configuration\n    # options for the Celery integration.\n    "CELERY": {\n        # Enable (default) or disable the Celery integration\n        "ENABLED": True,\n\n        # Report metrics on up to MAX_QUEUES queues.\n        # The list of discovered queues are sorted by the length\n        # of the queue name (shortest first) and metrics are\n        # reported for the first MAX_QUEUES queues.\n        # Defaults to 20.\n        "MAX_QUEUES": 20,\n\n        # Specify a list of known queues to report metrics for.\n        # MAX_QUEUES is still honoured.\n        # Defaults to empty list (report metrics for discovered queues).\n        "QUEUES": [],\n\n        # Enable or disable (default) tracking how many jobs are currently being\n        # processed in each queue.\n        # This allows Judoscale to avoid downscaling workers that are executing jobs.\n        # See documentation: https://judoscale.com/docs/long-running-jobs-ruby#enable-long-running-job-support-in-the-dashboard\n        # NOTE: This option requires workers to have unique names. If you are running\n        # multiple Celery workers on the same machine, make sure to give each\n        # worker a distinct name.\n        # More information: https://docs.celeryq.dev/en/stable/userguide/workers.html#starting-the-worker\n        "TRACK_BUSY_JOBS": False,\n    }\n}\n```\n\n> :warning: **NOTE:** Calling `judoscale_celery` turns on sending [`task-sent`](https://docs.celeryq.dev/en/stable/userguide/configuration.html#task-send-sent-event) events. This is required for the Celery integration with Judoscale to work.\n\n### Judoscale with Celery and Flask\n\nDepending on how you\'ve structured your Flask app, you should call `judoscale_celery` after your application has finished configuring the Celery app instance. If you have followed the [Flask guide](https://flask.palletsprojects.com/en/2.2.x/patterns/celery/) in the Flask documentation, the easiest place to initialise the Judoscale integration is in the application factory:\n\n```py\ndef create_app():\n    app = Flask(__name__)\n    app.config.from_object(...) # or however you configure your app\n    celery_app = celery_init_app(app)\n    # Initialise the Judoscale integration\n    judoscale_celery(celery_app, extra_config=app.config["JUDOSCALE"])\n    return app\n```\n\n### Judoscale with Celery and Django\n\nIf you have followed the [Django guide](https://docs.celeryq.dev/en/stable/django/first-steps-with-django.html) in the Celery documentation, you should have a module where you initialise the Celery app instance, auto-discover tasks, etc. You should call `judoscale_celery` after you have configured the Celery app instance:\n\n```py\nfrom celery import Celery\nfrom django.conf import settings\nfrom judoscale.celery import judoscale_celery\n\napp = Celery()\napp.config_from_object("django.conf:settings", namespace="CELERY")\napp.autodiscover_tasks()\n# Initialise the Judoscale integration\njudoscale_celery(app, extra_config=settings.JUDOSCALE)\n```\n\n# Using Judoscale with RQ\n\nInstall Judoscale for RQ with:\n\n```sh\n$ pip install \'judoscale[rq]\'\n```\n\nJudoscale can automatically scale the number of RQ workers based on the queue latency (the age of the oldest pending task in the queue).\n\n## Setting up the integration\n\nTo use the RQ integration, import `judoscale_rq` and call it with an instance of `Redis` pointing to the same Redis database that RQ uses.\n\n```py\nfrom redis import Redis\nfrom judoscale.rq import judoscale_rq\n\nredis = Redis(...)\njudoscale_rq(redis)\n```\n\nThis sets up Judoscale to periodically calculate and report queue latency for each RQ queue.\n\nIf you need to change the Judoscale integration configuration, you can pass a dictionary of Judoscale configuration options to `judoscale_rq` to override the default Judoscale config variables:\n\n```py\njudoscale_rq(redis, extra_config={"LOG_LEVEL": "DEBUG"})\n```\n\nAn example configuration dictionary accepted by `extra_config`:\n\n```py\n {\n    "LOG_LEVEL": "INFO",\n\n    # In addition to global configuration options for the Judoscale\n    # integration above, you can also specify the following configuration\n    # options for the RQ integration.\n    "RQ": {\n        # Enable (default) or disable the RQ integration\n        "ENABLED": True,\n\n        # Report metrics on up to MAX_QUEUES queues.\n        # The list of discovered queues are sorted by the length\n        # of the queue name (shortest first) and metrics are\n        # reported for the first MAX_QUEUES queues.\n        # Defaults to 20.\n        "MAX_QUEUES": 20,\n\n        # Specify a list of known queues to report metrics for.\n        # MAX_QUEUES is still honoured.\n        # Defaults to empty list (report metrics for discovered queues).\n        "QUEUES": [],\n\n        # Enable or disable (default) tracking how many jobs are currently being\n        # processed in each queue.\n        # This allows Judoscale to avoid downscaling workers that are executing jobs.\n        # See documentation: https://judoscale.com/docs/long-running-jobs-ruby#enable-long-running-job-support-in-the-dashboard\n        "TRACK_BUSY_JOBS": False,\n}\n```\n\n### Judoscale with RQ and Flask\n\nThe recommended way to initialise Judoscale for RQ is in the application factory:\n\n```py\njudoscale = Judoscale()\n\ndef create_app():\n    app = Flask(__name__)\n    app.config.from_object("...") # or however you configure your application\n    app.redis = Redis()\n\n    # Initialise the Judoscale integration for Flask\n    judoscale.init_app(app)\n\n    # Initialise the Judoscale integration for RQ\n    judoscale_rq(app.redis)\n\n    return app\n```\n\nThen, in your worker script, make sure that you create an app, which will initialise the Judoscale integration with RQ. Although not required, it\'s useful to run the worker within the Flask app context. If you have followed the [RQ on Heroku pattern](https://python-rq.org/patterns/) for setting up your RQ workers on Heroku, your worker script should look something like this:\n\n```py\nfrom rq.worker import HerokuWorker as Worker\n\napp = create_app()\n\nworker = Worker(..., connection=app.redis)\nwith app.app_context():\n    worker.work()\n```\n\nSee the [run-worker.py script](./sample-apps/flask_rq_sample/run-worker.py) for reference.\n\n### Judoscale with RQ and Django\n\nThe Judoscale integration for RQ is packaged into a separate Django app.\n\nYou should already have `judoscale.django` in your `INSTALLED_APPS`. Next, add the RQ integration app `judoscale.rq`:\n\n```python\nINSTALLED_APPS = [\n    "judoscale.django",\n    "judoscale.rq",\n    # ... other apps\n]\n```\n\nBy default, `judoscale.rq` will connect to the Redis instance as specified by the `REDIS_URL` environment variable. If that is not suitable, you can supply Redis connection information in the `JUDOSCALE` configuration dictionary under the `"REDIS"` key.\n\nAccepted formats are:\n\n- a dictionary containing a single key `"URL"` pointing to a Redis server URL, or;\n- a dictionary of configuration options corresponding to the keyword arguments of the [`Redis` constructor](https://github.com/redis/redis-py/blob/6c708c2e0511364c2c3f21fa1259de05e590632d/redis/client.py#L905).\n\n```py\nJUDOSCALE = {\n    # Configuring with a Redis server URL\n    "REDIS": {\n        "URL": os.getenv("REDISTOGO_URL")\n    }\n\n    # Configuring as kwargs to Redis(...)\n    "REDIS": {\n        "HOST": "localhost",\n        "PORT": 6379,\n        "DB": 0\n    }\n}\n```\n\nIf you are using [Django-RQ](https://github.com/rq/django-rq/tree/master), you can also pull configuration from `RQ_QUEUES` directly:\n\n```py\nRQ_QUEUES = {\n    "high_priority": {\n        "HOST": "...",\n        "PORT": 6379,\n        "DB": 0\n    },\n}\n\nJUDOSCALE = {\n    # ... other configuration options\n    "REDIS": RQ_QUEUES["high_priority"]\n}\n```\n\n> :warning: **NOTE:** Django-RQ enables configuring RQ such that different queues and workers use _different_ Redis instances. Judoscale currently only supports connecting to and monitoring queue latency on a single Redis instance.\n\n## Development\n\nThis repo includes a `sample-apps` directory containing apps you can run locally. These apps use the `judoscale` adapter, but they override `API_BASE_URL` so they\'re not connected to the real Judoscale API. Instead, they post API requests to https://requestinspector.com so you can observe the API behavior.\n\nSee the `README` in a sample app for details on how to set it up and run locally.\n\n### Contributing\n\n`judoscale` uses [Poetry](https://python-poetry.org/) for managing dependencies and packaging the project. Head over to the [installations instructions](https://python-poetry.org/docs/#installing-with-the-official-installer) and install Poetry, if needed.\n\nClone the repo with\n\n```sh\n$ git clone git@github.com:judoscale/judoscale-python.git\n$ cd judoscale-python\n```\n\nVerify that you are on a recent version of Poetry:\n\n```sh\n$ poetry --version\nPoetry (version 1.3.1)\n```\n\nInstall dependencies with Poetry and activate the virtualenv\n\n```sh\n$ poetry install --all-extras\n$ poetry shell\n```\n\nRun tests with\n\n```sh\n$ pytest\n```\n',
     'author': 'Adam McCrea',
     'author_email': 'adam@adamlogic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/judoscale/judoscale-python',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `judoscale-1.2.2/PKG-INFO` & `judoscale-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: judoscale
-Version: 1.2.2
+Version: 1.3.0
 Summary: Official Python adapter for Judoscale — the advanced autoscaler for Heroku
 Home-page: https://github.com/judoscale/judoscale-python
 License: MIT
 Author: Adam McCrea
 Author-email: adam@adamlogic.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,18 +13,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: celery-redis
 Provides-Extra: django
+Provides-Extra: fastapi
 Provides-Extra: flask
 Provides-Extra: rq
 Requires-Dist: celery[redis] (>=4.4.0,<6.0.0); extra == "celery-redis"
 Requires-Dist: django (>=2.1.0,<5.0.0); extra == "django"
+Requires-Dist: fastapi (<1.0.0); extra == "fastapi"
 Requires-Dist: flask (>=1.1.0,<3.0.0); extra == "flask"
 Requires-Dist: requests (<3.0.0)
 Requires-Dist: rq (>=1.0.0,<2.0.0); extra == "rq"
 Project-URL: Repository, https://github.com/judoscale/judoscale-python
 Description-Content-Type: text/markdown
 
 # Judoscale
@@ -33,15 +35,15 @@
 
 It is recommended to install the specific web framework and/or background job library support as "extras" to the `judoscale` PyPI package. This ensures that checking if the installed web framework and/or background task processing library is supported happens at dependency resolution time.
 
 ## Supported web frameworks
 
 - [x] [Django](#using-judoscale-with-django)
 - [x] [Flask](#using-judoscale-with-flask)
-- [ ] FastAPI
+- [x] [FastAPI](#using-judoscale-with-fastapi)
 
 ## Supported job processors
 
 - [x] [Celery](#using-judoscale-with-celery-and-redis) (with Redis 6.0+ as the broker)
 - [x] [RQ](#using-judoscale-with-rq)
 
 # Using Judoscale with Django
@@ -116,14 +118,51 @@
     # Log level defaults to ENV["LOG_LEVEL"] or "INFO".
     "LOG_LEVEL": "DEBUG",
 }
 ```
 
 Note the [official recommendations for configuring Flask](https://flask.palletsprojects.com/en/2.2.x/config/#configuration-best-practices).
 
+# Using Judoscale with FastAPI
+
+Install Judoscale for FastAPI with:
+
+```sh
+$ pip install 'judoscale[fastapi]'
+```
+
+Since FastAPI uses [Starlette](https://www.starlette.io/), an ASGI framework, the integration is packaged into [ASGI middleware](https://asgi.readthedocs.io/en/latest/specs/main.html#middleware). Import the middleare class and register it with your FastAPI app:
+
+```py
+# app.py
+
+from judoscale.asgi.middleware import RequestQueueTimeMiddleware
+
+# If your app is a top-level global
+
+app = FastAPI()
+app.add_middleware(RequestQueueTimeMiddleware)
+
+
+# If your app uses the application factory pattern
+
+def create_app():
+    app = FastAPI()
+    app.add_middleware(RequestQueueTimeMiddleware)
+    return app
+```
+
+This sets up the Judoscale extension to capture request queue times.
+
+Optionally, you can override Judoscale's configuration by passing in extra configuration to the `add_middleware` method:
+
+```py
+app.add_middleware(RequestQueueTimeMiddleware, extra_config={"LOG_LEVEL": "DEBUG"})
+```
+
 # Using Judoscale with Celery and Redis
 
 Install Judoscale for Celery with:
 
 ```sh
 $ pip install 'judoscale[celery-redis]'
 ```
@@ -177,15 +216,25 @@
         # reported for the first MAX_QUEUES queues.
         # Defaults to 20.
         "MAX_QUEUES": 20,
 
         # Specify a list of known queues to report metrics for.
         # MAX_QUEUES is still honoured.
         # Defaults to empty list (report metrics for discovered queues).
-        "QUEUES": []
+        "QUEUES": [],
+
+        # Enable or disable (default) tracking how many jobs are currently being
+        # processed in each queue.
+        # This allows Judoscale to avoid downscaling workers that are executing jobs.
+        # See documentation: https://judoscale.com/docs/long-running-jobs-ruby#enable-long-running-job-support-in-the-dashboard
+        # NOTE: This option requires workers to have unique names. If you are running
+        # multiple Celery workers on the same machine, make sure to give each
+        # worker a distinct name.
+        # More information: https://docs.celeryq.dev/en/stable/userguide/workers.html#starting-the-worker
+        "TRACK_BUSY_JOBS": False,
     }
 }
 ```
 
 > :warning: **NOTE:** Calling `judoscale_celery` turns on sending [`task-sent`](https://docs.celeryq.dev/en/stable/userguide/configuration.html#task-send-sent-event) events. This is required for the Celery integration with Judoscale to work.
 
 ### Judoscale with Celery and Flask
@@ -267,15 +316,21 @@
         # reported for the first MAX_QUEUES queues.
         # Defaults to 20.
         "MAX_QUEUES": 20,
 
         # Specify a list of known queues to report metrics for.
         # MAX_QUEUES is still honoured.
         # Defaults to empty list (report metrics for discovered queues).
-        "QUEUES": []
+        "QUEUES": [],
+
+        # Enable or disable (default) tracking how many jobs are currently being
+        # processed in each queue.
+        # This allows Judoscale to avoid downscaling workers that are executing jobs.
+        # See documentation: https://judoscale.com/docs/long-running-jobs-ruby#enable-long-running-job-support-in-the-dashboard
+        "TRACK_BUSY_JOBS": False,
 }
 ```
 
 ### Judoscale with RQ and Flask
 
 The recommended way to initialise Judoscale for RQ is in the application factory:
```

