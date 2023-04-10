# Comparing `tmp/sneakpeek_py-0.1.0.tar.gz` & `tmp/sneakpeek_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneakpeek_py-0.1.0.tar", max compression
+gzip compressed data, was "sneakpeek_py-0.1.1.tar", max compression
```

## Comparing `sneakpeek_py-0.1.0.tar` & `sneakpeek_py-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0       85 2023-04-02 10:58:33.945002 sneakpeek_py-0.1.0/README.md
--rw-r--r--   0        0        0     1483 2023-04-10 14:15:27.936979 sneakpeek_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2469 2023-04-10 12:15:19.719088 sneakpeek_py-0.1.0/sneakpeek/api.py
--rw-r--r--   0        0        0     2044 2023-04-10 12:16:05.568698 sneakpeek_py-0.1.0/sneakpeek/cli.py
--rw-r--r--   0        0        0      283 2023-04-10 12:48:43.794471 sneakpeek_py-0.1.0/sneakpeek/config.py
--rw-r--r--   0        0        0     3926 2023-04-10 13:01:36.235348 sneakpeek_py-0.1.0/sneakpeek/context.py
--rw-r--r--   0        0        0      726 2023-04-10 11:41:30.863384 sneakpeek_py-0.1.0/sneakpeek/lib/errors.py
--rw-r--r--   0        0        0     1283 2023-04-10 13:20:11.729784 sneakpeek_py-0.1.0/sneakpeek/lib/models.py
--rw-r--r--   0        0        0     3821 2023-04-10 11:28:44.055807 sneakpeek_py-0.1.0/sneakpeek/lib/queue.py
--rw-r--r--   0        0        0     2005 2023-04-10 11:29:01.052309 sneakpeek_py-0.1.0/sneakpeek/lib/storage/base.py
--rw-r--r--   0        0        0     7544 2023-04-10 13:19:00.753044 sneakpeek_py-0.1.0/sneakpeek/lib/storage/in_memory_storage.py
--rw-r--r--   0        0        0     7015 2023-04-10 11:29:46.671675 sneakpeek_py-0.1.0/sneakpeek/lib/storage/redis_storage.py
--rw-r--r--   0        0        0     2275 2023-04-10 13:07:20.785205 sneakpeek_py-0.1.0/sneakpeek/runner.py
--rw-r--r--   0        0        0     5950 2023-04-10 13:24:57.422638 sneakpeek_py-0.1.0/sneakpeek/scheduler.py
--rw-r--r--   0        0        0      262 2023-04-10 12:49:48.973818 sneakpeek_py-0.1.0/sneakpeek/scraper.py
--rw-r--r--   0        0        0     2043 2023-04-10 12:42:32.866231 sneakpeek_py-0.1.0/sneakpeek/server.py
--rw-r--r--   0        0        0     2695 2023-04-10 13:08:17.784798 sneakpeek_py-0.1.0/sneakpeek/worker.py
--rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 sneakpeek_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       85 2023-04-02 10:58:33.945002 sneakpeek_py-0.1.1/README.md
+-rw-r--r--   0        0        0     1675 2023-04-10 15:19:46.404709 sneakpeek_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2469 2023-04-10 12:15:19.719088 sneakpeek_py-0.1.1/sneakpeek/api.py
+-rw-r--r--   0        0        0      283 2023-04-10 12:48:43.794471 sneakpeek_py-0.1.1/sneakpeek/config.py
+-rw-r--r--   0        0        0     3926 2023-04-10 13:01:36.235348 sneakpeek_py-0.1.1/sneakpeek/context.py
+-rw-r--r--   0        0        0      726 2023-04-10 11:41:30.863384 sneakpeek_py-0.1.1/sneakpeek/lib/errors.py
+-rw-r--r--   0        0        0     1317 2023-04-10 14:50:53.763609 sneakpeek_py-0.1.1/sneakpeek/lib/models.py
+-rw-r--r--   0        0        0     3821 2023-04-10 11:28:44.055807 sneakpeek_py-0.1.1/sneakpeek/lib/queue.py
+-rw-r--r--   0        0        0     2005 2023-04-10 11:29:01.052309 sneakpeek_py-0.1.1/sneakpeek/lib/storage/base.py
+-rw-r--r--   0        0        0     7544 2023-04-10 13:19:00.753044 sneakpeek_py-0.1.1/sneakpeek/lib/storage/in_memory_storage.py
+-rw-r--r--   0        0        0     7015 2023-04-10 11:29:46.671675 sneakpeek_py-0.1.1/sneakpeek/lib/storage/redis_storage.py
+-rw-r--r--   0        0        0     2349 2023-04-10 15:13:41.871987 sneakpeek_py-0.1.1/sneakpeek/runner.py
+-rw-r--r--   0        0        0     6233 2023-04-10 14:52:04.073105 sneakpeek_py-0.1.1/sneakpeek/scheduler.py
+-rw-r--r--   0        0        0      262 2023-04-10 12:49:48.973818 sneakpeek_py-0.1.1/sneakpeek/scraper.py
+-rw-r--r--   0        0        0     2614 2023-04-10 15:01:10.667971 sneakpeek_py-0.1.1/sneakpeek/server.py
+-rw-r--r--   0        0        0     2695 2023-04-10 13:08:17.784798 sneakpeek_py-0.1.1/sneakpeek/worker.py
+-rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 sneakpeek_py-0.1.1/PKG-INFO
```

### Comparing `sneakpeek_py-0.1.0/pyproject.toml` & `sneakpeek_py-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sneakpeek-py"
 packages = [{ include = "sneakpeek" }]
-version = "0.1.0"
+version = "0.1.1"
 description = "Tool box for creating scrapers, so that you only focus on scraping logic"
 authors = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 maintainers = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 repository = "https://github.com/flulemon/sneakpeek"
 documentation = "https://github.com/flulemon/sneakpeek"
 homepage = "https://github.com/flulemon/sneakpeek"
 license = "BSD-3-Clause"
@@ -41,7 +41,13 @@
 black = "^23.3.0"
 pytest-lazy-fixture = "^0.6.3"
 pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+log_cli = true
+log_cli_level = "INFO"
+log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+log_cli_date_format = "%Y-%m-%d %H:%M:%S"
```

### Comparing `sneakpeek_py-0.1.0/sneakpeek/api.py` & `sneakpeek_py-0.1.1/sneakpeek/api.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.0/sneakpeek/context.py` & `sneakpeek_py-0.1.1/sneakpeek/context.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.0/sneakpeek/lib/errors.py` & `sneakpeek_py-0.1.1/sneakpeek/lib/errors.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.0/sneakpeek/lib/models.py` & `sneakpeek_py-0.1.1/sneakpeek/lib/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from sneakpeek.config import ScraperConfig
 
 UNSET_ID: int = -1
 
 
 class ScraperSchedule(str, Enum):
     INACTIVE = "inactive"
+    EVERY_SECOND = "every_second"
     EVERY_MINUTE = "every_minute"
     EVERY_HOUR = "every_hour"
     EVERY_DAY = "every_day"
     EVERY_WEEK = "every_week"
     EVERY_MONTH = "every_month"
     CRONTAB = "crontab"
```

### Comparing `sneakpeek_py-0.1.0/sneakpeek/lib/queue.py` & `sneakpeek_py-0.1.1/sneakpeek/lib/queue.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.0/sneakpeek/lib/storage/base.py` & `sneakpeek_py-0.1.1/sneakpeek/lib/storage/base.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.0/sneakpeek/lib/storage/in_memory_storage.py` & `sneakpeek_py-0.1.1/sneakpeek/lib/storage/in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.0/sneakpeek/lib/storage/redis_storage.py` & `sneakpeek_py-0.1.1/sneakpeek/lib/storage/redis_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.0/sneakpeek/runner.py` & `sneakpeek_py-0.1.1/sneakpeek/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from abc import ABC
+from datetime import datetime
 from traceback import format_exc
 from typing import List
 
 from sneakpeek.context import ScraperContext
 from sneakpeek.lib.errors import UnknownScraperHandlerError
 from sneakpeek.lib.models import Scraper, ScraperRun, ScraperRunStatus
 from sneakpeek.lib.queue import QueueABC
@@ -55,9 +56,10 @@
         except Exception as e:
             self._logger.error(f"Failed to execute: {human_run_id}: {e}")
             self._logger.debug(
                 f"Failed to execute: {human_run_id}. Traceback: {format_exc()}"
             )
             run.status = ScraperRunStatus.FAILED
             run.result = str(e)
+        run.finished_at = datetime.utcnow()
         await self._storage.update_scraper_run(run)
         self._logger.info(f"Successfully executed {human_run_id}")
```

### Comparing `sneakpeek_py-0.1.0/sneakpeek/scheduler.py` & `sneakpeek_py-0.1.1/sneakpeek/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from apscheduler.triggers.interval import IntervalTrigger
 
 from sneakpeek.lib.models import Lease, Scraper, ScraperSchedule
 from sneakpeek.lib.queue import QueueABC
 from sneakpeek.lib.storage.base import Storage
 
 DEFAULT_LEASE_DURATION = timedelta(minutes=1)
+DEFAULT_STORAGE_POLL_DELAY = timedelta(seconds=5)
 
 
 class SchedulerABC(ABC):
     async def start(self) -> None:
         raise NotImplementedError()
 
     async def stop(self) -> None:
@@ -27,14 +28,15 @@
 
 
 class Scheduler(SchedulerABC):
     def __init__(
         self,
         storage: Storage,
         queue: QueueABC,
+        storage_poll_frequency: timedelta = DEFAULT_STORAGE_POLL_DELAY,
         lease_duration: timedelta = DEFAULT_LEASE_DURATION,
     ) -> None:
         self._lease_name = "sneakpeek:scheduler"
         self._owner_id = str(uuid4())
         self._lease_duration = lease_duration
         self._storage = storage
         self._queue = queue
@@ -42,15 +44,15 @@
         self._lease: Lease | None = None
         self._lock = Lock()
         self._scrapers: Dict[int, Scraper] = {}
         self._logger = logging.getLogger(__name__)
         self._scheduler.add_job(
             self._on_tick,
             trigger="interval",
-            seconds=10,
+            seconds=int(storage_poll_frequency.total_seconds()),
             id="scheduler:internal:on_tick",
             max_instances=1,
         )
 
     async def _enqueue_scraper(self, scraper_id: int) -> None:
         scraper = self._scrapers.get(scraper_id)
         if not scraper:
@@ -93,14 +95,16 @@
                 return IntervalTrigger(days=1, start_date=start_date)
             case ScraperSchedule.EVERY_WEEK:
                 return IntervalTrigger(weeks=1, start_date=start_date)
             case ScraperSchedule.EVERY_MONTH:
                 return IntervalTrigger(days=30, start_date=start_date)
             case ScraperSchedule.EVERY_MINUTE:
                 return IntervalTrigger(minutes=1, start_date=start_date)
+            case ScraperSchedule.EVERY_SECOND:
+                return IntervalTrigger(seconds=1, start_date=start_date)
 
     def _remove_scraper_job(self, scraper) -> None:
         logging.info(f"Removing scraper enqueue job: {scraper}")
         self._scheduler.remove_job(f"scheduler:scraper:{scraper.id}")
         del self._scrapers[scraper.id]
 
     async def _update_scraper_job(
```

### Comparing `sneakpeek_py-0.1.0/sneakpeek/server.py` & `sneakpeek_py-0.1.1/sneakpeek/worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,79 @@
-import asyncio
 import logging
-from typing import List
+from abc import ABC
+from asyncio import AbstractEventLoop, Lock, get_running_loop, sleep
+from datetime import timedelta
+from traceback import format_exc
+from typing import Dict
+
+from sneakpeek.lib.models import ScraperRun
+from sneakpeek.lib.queue import QueueABC
+from sneakpeek.runner import RunnerABC
 
-import uvicorn
 
-from sneakpeek.api import create_api
-from sneakpeek.lib.queue import Queue
-from sneakpeek.lib.storage.base import Storage
-from sneakpeek.runner import Runner
-from sneakpeek.scheduler import Scheduler
-from sneakpeek.scraper import ScraperABC
-from sneakpeek.worker import Worker
+class WorkerABC(ABC):
+    async def start(self) -> None:
+        raise NotImplementedError()
 
-DEFAULT_API_PORT = 8080
-WORKER_DEFAULT_CONCURRENCY = 50
+    async def stop(self) -> None:
+        raise NotImplementedError()
 
 
-class SneakpeekServer:
+class Worker(WorkerABC):
     def __init__(
         self,
-        handlers: List[ScraperABC],
-        storage: Storage,
-        run_api: bool = True,
-        run_worker: bool = True,
-        run_scheduler: bool = True,
-        worker_max_concurrency: int = WORKER_DEFAULT_CONCURRENCY,
-        api_port: int = DEFAULT_API_PORT,
+        runner: RunnerABC,
+        queue: QueueABC,
+        loop: AbstractEventLoop | None = None,
+        max_concurrency: int = 50,
     ) -> None:
-        self._storage = storage
-        self._queue = Queue(self._storage)
-        self._scheduler = Scheduler(self._storage, self._queue)
-        self._runner = Runner(handlers, self._queue, self._storage)
-        self._worker = Worker(
-            self._runner,
-            self._queue,
-            max_concurrency=worker_max_concurrency,
-        )
-        self._api_config = uvicorn.Config(
-            create_api(self._storage, self._queue, handlers),
-            port=api_port,
-        )
-        self._api_server = uvicorn.Server(self._api_config)
+        self._running = False
+        self._loop = loop
         self._logger = logging.getLogger(__name__)
-        self._run_api = run_api
-        self._run_worker = run_worker
-        self._run_scheduler = run_scheduler
+        self._lock = Lock()
+        self._runner = runner
+        self._queue = queue
+        self._active: Dict[int, ScraperRun] = {}
+        self._max_concurrency = max_concurrency
+
+    async def _execute_scraper(self, scraper_run: ScraperRun) -> None:
+        self._logger.info(f"Executing scraper run id={scraper_run.id}")
+        try:
+            await self._runner.run(scraper_run)
+        except Exception as e:
+            self._logger.error(f"Failed to execute {scraper_run.id}: {e}")
+            self._logger.debug(f"Failed to execute {scraper_run.id}: {format_exc()}")
+        del self._active[scraper_run.id]
+
+    async def _on_tick(self) -> None:
+        async with self._lock:
+            if len(self._active) >= self._max_concurrency:
+                self._logger.debug(
+                    f"Not dequeuing any tasks because worker has reached max concurrency,"
+                    f" there are {len(self._active)} of active tasks"
+                )
+                return
+
+            dequeued = await self._queue.dequeue()
+            if not dequeued:
+                self._logger.debug("No pending tasks in the queue")
+                return
+
+            self._logger.info(f"Dequeued a job with id={dequeued.id}")
+            self._active[dequeued.id] = dequeued
+            self._loop.create_task(self._execute_scraper(dequeued))
+
+    async def _worker_loop(self) -> None:
+        while self._running:
+            await self._on_tick()
+            await sleep(timedelta(seconds=1).total_seconds())
 
     async def start(self) -> None:
-        loop = asyncio.get_running_loop()
-        self._logger.info("Starting sneakpeek server")
-        if self._run_scheduler:
-            loop.create_task(self._scheduler.start())
-        if self._run_worker:
-            loop.create_task(self._worker.start())
-        if self._run_api:
-            loop.create_task(self._api_server.serve())
+        self._logger.info("Starting worker")
+        self._running = True
+        if not self._loop:
+            self._loop = get_running_loop()
+        self._loop.create_task(self._worker_loop())
 
     async def stop(self) -> None:
-        self._logger.info("Stopping sneakpeek server")
-        await self._scheduler.stop()
-        await self._worker.stop()
-        await self._api_server.stop()
+        self._logger.info(f"Stopping worker. There are {len(self._active)} jobs")
+        self._running = False
```

### Comparing `sneakpeek_py-0.1.0/PKG-INFO` & `sneakpeek_py-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sneakpeek-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool box for creating scrapers, so that you only focus on scraping logic
 Home-page: https://github.com/flulemon/sneakpeek
 License: BSD-3-Clause
 Author: Dan Yazovsky
 Author-email: daniil.yazovsky@gmail.com
 Maintainer: Dan Yazovsky
 Maintainer-email: daniil.yazovsky@gmail.com
```

