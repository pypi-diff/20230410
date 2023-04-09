# Comparing `tmp/taskiq-0.3.5.tar.gz` & `tmp/taskiq-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.3.5.tar", max compression
+gzip compressed data, was "taskiq-0.4.0.tar", max compression
```

## Comparing `taskiq-0.3.5.tar` & `taskiq-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1075 2023-03-31 10:12:48.856502 taskiq-0.3.5/LICENSE
--rw-r--r--   0        0        0     1875 2023-03-31 10:12:48.856502 taskiq-0.3.5/README.md
--rw-r--r--   0        0        0     2626 2023-03-31 10:12:48.864503 taskiq-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1386 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/__init__.py
--rw-r--r--   0        0        0     2062 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/abc/__init__.py
--rw-r--r--   0        0        0     9490 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      637 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     2997 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1375 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1084 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0       34 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5741 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2162 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2489 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     1990 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3911 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2477 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1530 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     4265 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0     1688 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/worker/async_task_runner.py
--rw-r--r--   0        0        0      628 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     2795 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/worker/params_parser.py
--rw-r--r--   0        0        0     7305 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     7878 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/worker/receiver.py
--rw-r--r--   0        0        0     4682 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0      468 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/context.py
--rw-r--r--   0        0        0     2957 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/decor.py
--rw-r--r--   0        0        0      510 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/events.py
--rw-r--r--   0        0        0      778 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      851 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/funcs.py
--rw-r--r--   0        0        0     5594 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/kicker.py
--rw-r--r--   0        0        0      505 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     2005 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/py.typed
--rw-r--r--   0        0        0      476 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/result.py
--rw-r--r--   0        0        0       35 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1351 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     1519 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     1717 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0     1071 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/state.py
--rw-r--r--   0        0        0     4171 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/task.py
--rw-r--r--   0        0        0      582 2023-03-31 10:12:48.864503 taskiq-0.3.5/taskiq/utils.py
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 taskiq-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-09 23:15:51.392623 taskiq-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1875 2023-04-09 23:15:51.392623 taskiq-0.4.0/README.md
+-rw-r--r--   0        0        0     2888 2023-04-09 23:15:51.396623 taskiq-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1587 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/__init__.py
+-rw-r--r--   0        0        0     2077 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0     9488 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     2997 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1375 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1084 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0       34 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5874 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2154 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2514 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     1990 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3911 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1516 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     4286 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     7498 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     5192 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0      468 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/context.py
+-rw-r--r--   0        0        0     2929 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/decor.py
+-rw-r--r--   0        0        0      510 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/events.py
+-rw-r--r--   0        0        0      778 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      844 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4317 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2005 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2795 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0     9641 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0      476 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/result.py
+-rw-r--r--   0        0        0       35 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1351 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     1519 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     1717 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0     1071 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/state.py
+-rw-r--r--   0        0        0     4139 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/task.py
+-rw-r--r--   0        0        0      874 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/utils.py
+-rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 taskiq-0.4.0/PKG-INFO
```

### Comparing `taskiq-0.3.5/LICENSE` & `taskiq-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/README.md` & `taskiq-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/pyproject.toml` & `taskiq-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.3.5"
+version = "0.4.0"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
@@ -25,21 +25,26 @@
 ]
 keywords = ["taskiq", "tasks", "distributed", "async"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 typing-extensions = ">=3.10.0.0"
 pydantic = "^1.6.2"
-pyzmq = { version = "^23.2.0", optional = true }
-uvloop = { version = ">=0.16.0,<1", optional = true }
-watchdog = "^2.1.9"
-gitignore-parser = "^0"
 importlib-metadata = "*"
 pycron = "^3.0.0"
-taskiq_dependencies =  "^1"
+taskiq_dependencies = "^1"
+# For prometheus metrics
+prometheus_client = { version = "^0", optional = true }
+# For ZMQBroker
+pyzmq = { version = "^23.2.0", optional = true }
+# For speed
+uvloop = { version = ">=0.16.0,<1", optional = true }
+# For hot-reload.
+watchdog = { version = "^2.1.9", optional = true }
+gitignore-parser = { version = "^0", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = { version = "^22.6.0", allow-prereleases = true }
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 mypy = "^0.971"
@@ -53,14 +58,16 @@
 anyio = "^3.6.1"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 types-mock = "^4.0.15"
 
 [tool.poetry.extras]
 zmq = ["pyzmq"]
 uv = ["uvloop"]
+metrics = ["prometheus_client"]
+reload = ["watchdog", "gitignore-parser"]
 
 [tool.poetry.scripts]
 taskiq = "taskiq.__main__:main"
 
 [tool.poetry.plugins.taskiq_cli]
 worker = "taskiq.cli.worker.cmd:WorkerCMD"
 scheduler = "taskiq.cli.scheduler.cmd:SchedulerCMD"
```

### Comparing `taskiq-0.3.5/taskiq/__init__.py` & `taskiq-0.4.0/taskiq/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from taskiq.brokers.shared_broker import async_shared_broker
 from taskiq.brokers.zmq_broker import ZeroMQBroker
 from taskiq.context import Context
 from taskiq.events import TaskiqEvents
 from taskiq.exceptions import TaskiqError
 from taskiq.funcs import gather
 from taskiq.message import BrokerMessage, TaskiqMessage
+from taskiq.middlewares.prometheus_middleware import PrometheusMiddleware
+from taskiq.middlewares.retry_middleware import SimpleRetryMiddleware
 from taskiq.result import TaskiqResult
 from taskiq.scheduler import ScheduledTask, TaskiqScheduler
 from taskiq.state import TaskiqState
 from taskiq.task import AsyncTaskiqTask
 
 __all__ = [
     "gather",
@@ -37,8 +39,10 @@
     "TaskiqScheduler",
     "TaskiqFormatter",
     "AsyncTaskiqTask",
     "TaskiqMiddleware",
     "AsyncResultBackend",
     "async_shared_broker",
     "AsyncTaskiqDecoratedTask",
+    "SimpleRetryMiddleware",
+    "PrometheusMiddleware",
 ]
```

### Comparing `taskiq-0.3.5/taskiq/__main__.py` & `taskiq-0.4.0/taskiq/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 
 from importlib_metadata import entry_points, version
 
 from taskiq.abc.cmd import TaskiqCMD
 
 
-def main() -> None:  # noqa: C901, WPS210  # pragma: no cover
+def main() -> None:  # noqa: WPS210  # pragma: no cover
     """
     Main entrypoint of the taskiq.
 
     This function collects all python entrypoints
     and assembles a final argument parser.
 
     All found entrypoints are used as subcommands.
@@ -42,16 +42,16 @@
         title="Available subcommands",
         metavar="",
         dest="subcommand",
     )
     for entrypoint in entry_points().select(group="taskiq_cli"):
         try:
             cmd_class = entrypoint.load()
-        except ImportError:
-            print(f"Could not load {entrypoint.value}")  # noqa: WPS421
+        except ImportError as exc:
+            print(f"Could not load {entrypoint.value}. Cause: {exc}")  # noqa: WPS421
             continue
         if issubclass(cmd_class, TaskiqCMD):
             subparsers.add_parser(
                 entrypoint.name,
                 help=cmd_class.short_help,
                 add_help=False,
             )
```

### Comparing `taskiq-0.3.5/taskiq/abc/broker.py` & `taskiq-0.4.0/taskiq/abc/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from taskiq.abc.middleware import TaskiqMiddleware
 from taskiq.decor import AsyncTaskiqDecoratedTask
 from taskiq.events import TaskiqEvents
 from taskiq.formatters.json_formatter import JSONFormatter
 from taskiq.message import BrokerMessage
 from taskiq.result_backends.dummy import DummyResultBackend
 from taskiq.state import TaskiqState
-from taskiq.utils import maybe_awaitable
+from taskiq.utils import maybe_awaitable, remove_suffix
 
 if TYPE_CHECKING:  # pragma: no cover
     from taskiq.abc.formatter import TaskiqFormatter
     from taskiq.abc.result_backend import AsyncResultBackend
 
 _T = TypeVar("_T")  # noqa: WPS111
 _FuncParams = ParamSpec("_FuncParams")
@@ -53,15 +53,15 @@
     for tasks.
 
     :return: new task_id.
     """
     return uuid4().hex
 
 
-class AsyncBroker(ABC):  # noqa: WPS230
+class AsyncBroker(ABC):
     """
     Async broker.
 
     This abstract class must be implemented in order
     to get ability to send tasks to brokers
     in async mode.
     """
@@ -154,19 +154,22 @@
     ) -> None:
         """
         This method is used to kick tasks out from current program.
 
         Using this method tasks are sent to
         workers.
 
+        You don't need to send broker message. It's helper for brokers,
+        please send only bytes from message.message.
+
         :param message: name of a task.
         """
 
     @abstractmethod
-    def listen(self) -> AsyncGenerator[BrokerMessage, None]:
+    def listen(self) -> AsyncGenerator[bytes, None]:
         """
         This function listens to new messages and yields them.
 
         This it the main point for workers.
         This function is used to get new tasks from the network.
 
         :yield: incoming messages.
@@ -231,19 +234,15 @@
                 func: Callable[_FuncParams, _ReturnType],
             ) -> AsyncTaskiqDecoratedTask[_FuncParams, _ReturnType]:
                 nonlocal inner_task_name  # noqa: WPS420
                 if inner_task_name is None:
                     fmodule = func.__module__
                     if fmodule == "__main__":  # pragma: no cover
                         fmodule = ".".join(
-                            sys.argv[0]
-                            .removesuffix(
-                                ".py",
-                            )
-                            .split(
+                            remove_suffix(sys.argv[0], ".py").split(
                                 os.path.sep,
                             ),
                         )
                     inner_task_name = f"{fmodule}:{func.__name__}"  # noqa: WPS442
                 wrapper = wraps(func)
 
                 decorated_task = wrapper(
```

### Comparing `taskiq-0.3.5/taskiq/abc/formatter.py` & `taskiq-0.4.0/taskiq/abc/formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,14 @@
         Dump message to broker message instance.
 
         :param message: message to send.
         :return: message for brokers.
         """
 
     @abstractmethod
-    def loads(self, message: BrokerMessage) -> TaskiqMessage:
+    def loads(self, message: bytes) -> TaskiqMessage:
         """
         Parses broker message to TaskiqMessage.
 
         :param message: message to parse.
         :return: parsed taskiq message.
         """
```

### Comparing `taskiq-0.3.5/taskiq/abc/middleware.py` & `taskiq-0.4.0/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/abc/result_backend.py` & `taskiq-0.4.0/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/abc/schedule_source.py` & `taskiq-0.4.0/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/brokers/inmemory_broker.py` & `taskiq-0.4.0/taskiq/brokers/inmemory_broker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import asyncio
 import inspect
 from collections import OrderedDict
-from typing import Any, AsyncGenerator, Callable, Optional, TypeVar, get_type_hints
+from concurrent.futures import ThreadPoolExecutor
+from typing import Any, AsyncGenerator, Callable, Optional, Set, TypeVar, get_type_hints
 
 from taskiq_dependencies import DependencyGraph
 
 from taskiq.abc.broker import AsyncBroker
 from taskiq.abc.result_backend import AsyncResultBackend, TaskiqResult
-from taskiq.cli.worker.args import WorkerArgs
-from taskiq.cli.worker.receiver import Receiver
 from taskiq.events import TaskiqEvents
 from taskiq.exceptions import TaskiqError
 from taskiq.message import BrokerMessage
+from taskiq.receiver import Receiver
 from taskiq.utils import maybe_awaitable
 
 _ReturnType = TypeVar("_ReturnType")
 
 
 class InmemoryResultBackend(AsyncResultBackend[_ReturnType]):
     """
@@ -86,68 +87,69 @@
 
     It's useful for local development, if you don't want to setup real broker.
     """
 
     def __init__(  # noqa: WPS211
         self,
         sync_tasks_pool_size: int = 4,
-        logs_format: Optional[str] = None,
         max_stored_results: int = 100,
         cast_types: bool = True,
         result_backend: Optional[AsyncResultBackend[Any]] = None,
         task_id_generator: Optional[Callable[[], str]] = None,
+        max_async_tasks: int = 30,
     ) -> None:
         if result_backend is None:
             result_backend = InmemoryResultBackend(
                 max_stored_results=max_stored_results,
             )
         super().__init__(
             result_backend=result_backend,
             task_id_generator=task_id_generator,
         )
+        self.executor = ThreadPoolExecutor(sync_tasks_pool_size)
         self.receiver = Receiver(
-            self,
-            WorkerArgs(
-                broker="",
-                modules=[],
-                max_threadpool_threads=sync_tasks_pool_size,
-                no_parse=not cast_types,
-                log_collector_format=logs_format or WorkerArgs.log_collector_format,
-            ),
+            broker=self,
+            executor=self.executor,
+            validate_params=cast_types,
+            max_async_tasks=max_async_tasks,
         )
+        self._running_tasks: "Set[asyncio.Task[Any]]" = set()
 
     async def kick(self, message: BrokerMessage) -> None:
         """
         Kicking task.
 
         This method just executes given task.
 
         :param message: incomming message.
 
         :raises TaskiqError: if someone wants to kick unknown task.
         """
         target_task = self.available_tasks.get(message.task_name)
         if target_task is None:
             raise TaskiqError("Unknown task.")
+
         if not self.receiver.dependency_graphs.get(target_task.task_name):
             self.receiver.dependency_graphs[target_task.task_name] = DependencyGraph(
                 target_task.original_func,
             )
         if not self.receiver.task_signatures.get(target_task.task_name):
             self.receiver.task_signatures[target_task.task_name] = inspect.signature(
                 target_task.original_func,
             )
         if not self.receiver.task_hints.get(target_task.task_name):
             self.receiver.task_hints[target_task.task_name] = get_type_hints(
                 target_task.original_func,
             )
 
-        await self.receiver.callback(message=message)
+        task = asyncio.create_task(self.receiver.callback(message=message.message))
+        self._running_tasks.add(task)
+        task.add_done_callback(self._running_tasks.discard)
 
-    def listen(self) -> AsyncGenerator[BrokerMessage, None]:
+    def listen(self) -> AsyncGenerator[bytes, None]:
         """
         Inmemory broker cannot listen.
 
         This method throws RuntimeError if you call it.
         Because inmemory broker cannot really listen to any of tasks.
 
         :raises RuntimeError: if this method is called.
@@ -161,7 +163,8 @@
                 await maybe_awaitable(handler(self.state))
 
     async def shutdown(self) -> None:
         """Runs shutdown events for client and worker side."""
         for event in (TaskiqEvents.CLIENT_SHUTDOWN, TaskiqEvents.WORKER_SHUTDOWN):
             for handler in self.event_handlers.get(event, []):
                 await maybe_awaitable(handler(self.state))
+        self.executor.shutdown()
```

### Comparing `taskiq-0.3.5/taskiq/brokers/shared_broker.py` & `taskiq-0.4.0/taskiq/brokers/shared_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         :raises TaskiqError: if called.
         """
         raise TaskiqError(
             "You cannot use kiq directly on shared task "
             "without setting the default_broker.",
         )
 
-    async def listen(self) -> AsyncGenerator[BrokerMessage, None]:  # type: ignore
+    async def listen(self) -> AsyncGenerator[bytes, None]:  # type: ignore
         """
         Shared broker cannot listen to tasks.
 
         This method will throw an exception.
 
         :raises TaskiqError: if called.
         """
```

### Comparing `taskiq-0.3.5/taskiq/brokers/zmq_broker.py` & `taskiq-0.4.0/taskiq/brokers/zmq_broker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from logging import getLogger
 from typing import AsyncGenerator, Callable, Optional, TypeVar
 
 from taskiq.abc.broker import AsyncBroker
 from taskiq.abc.result_backend import AsyncResultBackend
 from taskiq.message import BrokerMessage
 
@@ -54,25 +55,27 @@
         Kicking message.
 
         This method is used to publish message
         via socket.
 
         :param message: message to publish.
         """
+        part_len = 100
+        parts = [
+            message.message[
+                idx * part_len : min(idx * part_len + part_len, len(message.message))
+            ]
+            for idx in range(math.ceil(len(message.message) / part_len))
+        ]
         with self.socket.connect(self.sub_host) as sock:
-            await sock.send_string(message.json())
+            await sock.send_multipart(parts)
 
-    async def listen(self) -> AsyncGenerator[BrokerMessage, None]:
+    async def listen(self) -> AsyncGenerator[bytes, None]:
         """
         Start accepting new messages.
 
         :yields: incoming messages.
         """
         with self.socket.connect(self.sub_host) as sock:
-            while True:
-                received_str = await sock.recv_string()
-                try:
-                    broker_msg = BrokerMessage.parse_raw(received_str)
-                except ValueError:
-                    logger.warning("Cannot parse received message %s", received_str)
-                    continue
-                yield broker_msg
+            while True:  # noqa: WPS457
+                data = await sock.recv_multipart()
+                yield b"".join(data)
```

### Comparing `taskiq-0.3.5/taskiq/cli/scheduler/args.py` & `taskiq-0.4.0/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/cli/scheduler/cmd.py` & `taskiq-0.4.0/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/cli/scheduler/run.py` & `taskiq-0.4.0/taskiq/cli/scheduler/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/cli/utils.py` & `taskiq-0.4.0/taskiq/cli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import sys
 from contextlib import contextmanager
 from importlib import import_module
 from logging import getLogger
 from pathlib import Path
 from typing import Any, Generator, List
 
+from taskiq.utils import remove_suffix
+
 logger = getLogger("taskiq.worker")
 
 
 @contextmanager
 def add_cwd_in_path() -> Generator[None, None, None]:
     """
     Adds current directory in python path.
@@ -77,10 +79,12 @@
     :param modules: list of modules to import.
     :param pattern: pattern of a file if fs_discover is True.
     :param fs_discover: If true it will try to import modules
         from filesystem.
     """
     if fs_discover:
         for path in Path(".").rglob(pattern):
-            modules.append(str(path).removesuffix(".py").replace(os.path.sep, "."))
+            modules.append(
+                remove_suffix(str(path), ".py").replace(os.path.sep, "."),
+            )
 
     import_from_modules(modules)
```

### Comparing `taskiq-0.3.5/taskiq/cli/watcher.py` & `taskiq-0.4.0/taskiq/cli/watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.callback = callback
         self.gitignore = None
         gpath = Path("./.gitignore")
         if use_gitignore and gpath.exists():
             self.gitignore = parse_gitignore(gpath)
         self.callback_kwargs = callback_kwargs
 
-    def dispatch(self, event: FileSystemEvent) -> None:  # noqa: C901
+    def dispatch(self, event: FileSystemEvent) -> None:
         """
         React to event.
 
         This function checks wether we need to
         react to event and calls callback if we do.
 
         :param event: incoming fs event.
```

### Comparing `taskiq-0.3.5/taskiq/cli/worker/args.py` & `taskiq-0.4.0/taskiq/cli/worker/args.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,26 +112,26 @@
             default=5,
             help="Maximum amount of time for graceful broker's shutdown is seconds.",
         )
         parser.add_argument(
             "--reload",
             "-r",
             action="store_true",
-            help="Reload workers if file is changed.",
+            help="Reload workers if file is changed. "
+            + "`reload` extra is required for this option.",
         )
         parser.add_argument(
             "--do-not-use-gitignore",
             action="store_true",
             dest="no_gitignore",
             help="Do not use gitignore to check for updated files.",
         )
         parser.add_argument(
             "--max-async-tasks",
             type=int,
             dest="max_async_tasks",
             default=100,
-            help="Maximum simultaneous async tasks per worker process. "
-            + "Infinite if less than 1",
+            help="Maximum simultaneous async tasks per worker process. ",
         )
 
         namespace = parser.parse_args(args)
         return WorkerArgs(**namespace.__dict__)
```

### Comparing `taskiq-0.3.5/taskiq/cli/worker/cmd.py` & `taskiq-0.4.0/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/cli/worker/log_collector.py` & `taskiq-0.4.0/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/cli/worker/params_parser.py` & `taskiq-0.4.0/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/cli/worker/process_manager.py` & `taskiq-0.4.0/taskiq/cli/worker/process_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import logging
 import signal
 from dataclasses import dataclass
 from multiprocessing import Process, Queue
 from time import sleep
-from typing import Any, Callable, List
+from typing import Any, Callable, List, Optional
 
-from watchdog.observers import Observer
+try:
+    from watchdog.observers import Observer  # noqa: WPS433
+
+    from taskiq.cli.watcher import FileWatcher  # noqa: WPS433
+except ImportError:
+    Observer = None  # type: ignore
+    FileWatcher = None  # type: ignore
 
-from taskiq.cli.watcher import FileWatcher
 from taskiq.cli.worker.args import WorkerArgs
 
 logger = logging.getLogger("taskiq.process-manager")
 
 
 class ProcessActionBase:
     """Base for all process actions. Used for types."""
@@ -128,21 +133,21 @@
     and maintains their states. If process
     is down, it tries to restart it.
     """
 
     def __init__(
         self,
         args: WorkerArgs,
-        observer: Observer,
         worker_function: Callable[[WorkerArgs], None],
+        observer: Optional[Observer] = None,
     ) -> None:
         self.worker_function = worker_function
         self.action_queue: "Queue[ProcessActionBase]" = Queue(-1)
         self.args = args
-        if args.reload:
+        if args.reload and observer is not None:
             observer.schedule(
                 FileWatcher(
                     callback=schedule_workers_reload,
                     use_gitignore=not args.no_gitignore,
                     action_queue=self.action_queue,
                 ),
                 path=".",
```

### Comparing `taskiq-0.3.5/taskiq/cli/worker/receiver.py` & `taskiq-0.4.0/taskiq/receiver/receiver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import asyncio
 import inspect
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import Executor
 from logging import getLogger
 from time import time
-from typing import Any, Callable, Dict, get_type_hints
+from typing import Any, Callable, Dict, Optional, get_type_hints
 
 from taskiq_dependencies import DependencyGraph
 
 from taskiq.abc.broker import AsyncBroker
 from taskiq.abc.middleware import TaskiqMiddleware
-from taskiq.cli.worker.args import WorkerArgs
-from taskiq.cli.worker.params_parser import parse_params
 from taskiq.context import Context
-from taskiq.message import BrokerMessage, TaskiqMessage
+from taskiq.message import TaskiqMessage
+from taskiq.receiver.params_parser import parse_params
 from taskiq.result import TaskiqResult
 from taskiq.state import TaskiqState
 from taskiq.utils import maybe_awaitable
 
 logger = getLogger(__name__)
 
 
@@ -33,101 +32,112 @@
     """
     return target(*message.args, **message.kwargs)
 
 
 class Receiver:
     """Class that uses as a callback handler."""
 
-    def __init__(self, broker: AsyncBroker, cli_args: WorkerArgs) -> None:
+    def __init__(
+        self,
+        broker: AsyncBroker,
+        executor: Optional[Executor] = None,
+        validate_params: bool = True,
+        max_async_tasks: "Optional[int]" = None,
+    ) -> None:
         self.broker = broker
-        self.cli_args = cli_args
+        self.executor = executor
+        self.validate_params = validate_params
         self.task_signatures: Dict[str, inspect.Signature] = {}
         self.task_hints: Dict[str, Dict[str, Any]] = {}
         self.dependency_graphs: Dict[str, DependencyGraph] = {}
         for task in self.broker.available_tasks.values():
             self.task_signatures[task.task_name] = inspect.signature(task.original_func)
             self.task_hints[task.task_name] = get_type_hints(task.original_func)
             self.dependency_graphs[task.task_name] = DependencyGraph(task.original_func)
-        self.executor = ThreadPoolExecutor(
-            max_workers=cli_args.max_threadpool_threads,
-        )
+        self.sem: "Optional[asyncio.Semaphore]" = None
+        if max_async_tasks is not None and max_async_tasks > 0:
+            self.sem = asyncio.Semaphore(max_async_tasks)
+        else:
+            logger.warning(
+                "Setting unlimited number of async tasks "
+                + "can result in undefined behavior",
+            )
 
     async def callback(  # noqa: C901, WPS213
         self,
-        message: BrokerMessage,
+        message: bytes,
         raise_err: bool = False,
     ) -> None:
         """
         Receive new message and execute tasks.
 
         This method is used to process message,
         that came from brokers.
 
         :raises Exception: if raise_err is true,
             and excpetion were found while saving result.
         :param message: received message.
         :param raise_err: raise an error if cannot save result in
             result_backend.
         """
-        logger.debug(f"Received message: {message}")
-        if message.task_name not in self.broker.available_tasks:
-            logger.warning(
-                'task "%s" is not found. Maybe you forgot to import it?',
-                message.task_name,
-            )
-            return
-        logger.debug(
-            "Function for task %s is resolved. Executing...",
-            message.task_name,
-        )
         try:
             taskiq_msg = self.broker.formatter.loads(message=message)
         except Exception as exc:
             logger.warning(
                 "Cannot parse message: %s. Skipping execution.\n %s",
                 message,
                 exc,
                 exc_info=True,
             )
             return
+        logger.debug(f"Received message: {taskiq_msg}")
+        if taskiq_msg.task_name not in self.broker.available_tasks:
+            logger.warning(
+                'task "%s" is not found. Maybe you forgot to import it?',
+                taskiq_msg.task_name,
+            )
+            return
+        logger.debug(
+            "Function for task %s is resolved. Executing...",
+            taskiq_msg.task_name,
+        )
         for middleware in self.broker.middlewares:
             if middleware.__class__.pre_execute != TaskiqMiddleware.pre_execute:
                 taskiq_msg = await maybe_awaitable(
                     middleware.pre_execute(
                         taskiq_msg,
                     ),
                 )
 
         logger.info(
             "Executing task %s with ID: %s",
             taskiq_msg.task_name,
             taskiq_msg.task_id,
         )
         result = await self.run_task(
-            target=self.broker.available_tasks[message.task_name].original_func,
+            target=self.broker.available_tasks[taskiq_msg.task_name].original_func,
             message=taskiq_msg,
         )
         for middleware in self.broker.middlewares:
             if middleware.__class__.post_execute != TaskiqMiddleware.post_execute:
                 await maybe_awaitable(middleware.post_execute(taskiq_msg, result))
         try:
-            await self.broker.result_backend.set_result(message.task_id, result)
+            await self.broker.result_backend.set_result(taskiq_msg.task_id, result)
+            for middleware in self.broker.middlewares:
+                if middleware.__class__.post_save != TaskiqMiddleware.post_save:
+                    await maybe_awaitable(middleware.post_save(taskiq_msg, result))
         except Exception as exc:
             logger.exception(
                 "Can't set result in result backend. Cause: %s",
                 exc,
                 exc_info=True,
             )
             if raise_err:
                 raise exc
 
-        for middleware in self.broker.middlewares:
-            if middleware.__class__.post_save != TaskiqMiddleware.post_save:
-                await maybe_awaitable(middleware.post_save(taskiq_msg, result))
-
     async def run_task(  # noqa: C901, WPS210
         self,
         target: Callable[..., Any],
         message: TaskiqMessage,
     ) -> TaskiqResult[Any]:
         """
         This function actually executes functions.
@@ -146,18 +156,18 @@
         :param target: function to execute.
         :param message: received message.
         :return: result of execution.
         """
         loop = asyncio.get_running_loop()
         returned = None
         found_exception = None
-        signature = self.task_signatures.get(message.task_name)
+        signature = None
+        if self.validate_params:
+            signature = self.task_signatures.get(message.task_name)
         dependency_graph = self.dependency_graphs.get(message.task_name)
-        if self.cli_args.no_parse:
-            signature = None
         parse_params(signature, self.task_hints.get(message.task_name) or {}, message)
 
         dep_ctx = None
         if dependency_graph:
             # Create a context for dependency resolving.
             broker_ctx = self.broker.custom_dependency_context
             broker_ctx.update(
@@ -215,7 +225,46 @@
                             message,
                             result,
                             found_exception,
                         ),
                     )
 
         return result
+
+    async def listen(self) -> None:  # pragma: no cover
+        """
+        This function iterates over tasks asynchronously.
+
+        It uses listen() method of an AsyncBroker
+        to get new messages from queues.
+        """
+        await self.broker.startup()
+        logger.info("Listening started.")
+        tasks = set()
+
+        def task_cb(task: "asyncio.Task[Any]") -> None:
+            """
+            Callback for tasks.
+
+            This function used to remove task
+            from the list of active tasks and release
+            the semaphore, so other tasks can use it.
+
+            :param task: finished task
+            """
+            tasks.discard(task)
+            if self.sem is not None:
+                self.sem.release()
+
+        async for message in self.broker.listen():
+            # Waits for semaphore to be released.
+            if self.sem is not None:
+                await self.sem.acquire()
+            task = asyncio.create_task(self.callback(message=message, raise_err=False))
+            tasks.add(task)
+
+            # We want the task to remove itself from the set when it's done.
+            #
+            # Because python's GC can silently cancel task
+            # and it considered to be Hisenbug.
+            # https://textual.textualize.io/blog/2023/02/11/the-heisenbug-lurking-in-your-async-code/
+            task.add_done_callback(task_cb)
```

### Comparing `taskiq-0.3.5/taskiq/cli/worker/run.py` & `taskiq-0.4.0/taskiq/cli/worker/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import asyncio
 import logging
 import signal
+from concurrent.futures import ThreadPoolExecutor
 from typing import Any
 
-from watchdog.observers import Observer
-
 from taskiq.abc.broker import AsyncBroker
 from taskiq.cli.utils import import_object, import_tasks
 from taskiq.cli.worker.args import WorkerArgs
-from taskiq.cli.worker.async_task_runner import async_listen_messages
 from taskiq.cli.worker.process_manager import ProcessManager
+from taskiq.receiver import Receiver
 
 try:
     import uvloop  # noqa: WPS433
 except ImportError:
     uvloop = None  # type: ignore
 
 
+try:
+    from watchdog.observers import Observer  # noqa: WPS433
+except ImportError:
+    Observer = None  # type: ignore
+
 logger = logging.getLogger("taskiq.worker")
 
 
 async def shutdown_broker(broker: AsyncBroker, timeout: float) -> None:
     """
     This function used to shutdown broker.
 
@@ -43,15 +47,15 @@
         logger.warning(
             "Exception found while terminating: %s",
             exc,
             exc_info=True,
         )
 
 
-def start_listen(args: WorkerArgs) -> None:  # noqa: C901, WPS213
+def start_listen(args: WorkerArgs) -> None:  # noqa: WPS213
     """
     This function starts actual listening process.
 
     It imports broker and all tasks.
     Since tasks registers themselfs in a global set,
     it's easy to just import module where you have decorated
     function and they will be available in broker's `available_tasks`
@@ -98,15 +102,23 @@
         raise KeyboardInterrupt
 
     signal.signal(signal.SIGINT, interrupt_handler)
     signal.signal(signal.SIGTERM, interrupt_handler)
 
     loop = asyncio.get_event_loop()
     try:
-        loop.run_until_complete(async_listen_messages(broker, args))
+        logger.debug("Initialize receiver.")
+        with ThreadPoolExecutor(args.max_threadpool_threads) as pool:
+            receiver = Receiver(
+                broker=broker,
+                executor=pool,
+                validate_params=not args.no_parse,
+                max_async_tasks=args.max_async_tasks,
+            )
+            loop.run_until_complete(receiver.listen())
     except KeyboardInterrupt:
         logger.warning("Worker process interrupted.")
         loop.run_until_complete(shutdown_broker(broker, args.shutdown_timeout))
 
 
 def run_worker(args: WorkerArgs) -> None:  # noqa: WPS213
     """
@@ -120,25 +132,27 @@
     logging.basicConfig(
         level=logging.getLevelName(args.log_level),
         format="[%(asctime)s][%(name)s][%(levelname)-7s][%(processName)s] %(message)s",
     )
     logging.getLogger("watchdog.observers.inotify_buffer").setLevel(level=logging.INFO)
     logger.info("Starting %s worker processes.", args.workers)
 
-    observer = Observer()
+    observer = None
+    if Observer is not None:
+        observer = Observer()
 
-    if args.reload:
+    if observer is not None and args.reload:
         observer.start()
         args.workers = 1
         logging.warning(
             "Reload on chage enabled. Number of worker processes set to 1.",
         )
 
     manager = ProcessManager(args=args, observer=observer, worker_function=start_listen)
 
     manager.start()
 
-    if observer.is_alive():
+    if observer is not None and observer.is_alive():
         if args.reload:
             logger.info("Stopping watching files.")
         observer.stop()
     logger.info("Stopping logging thread.")
```

### Comparing `taskiq-0.3.5/taskiq/decor.py` & `taskiq-0.4.0/taskiq/decor.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,23 +56,23 @@
         self,
         *args: _FuncParams.args,
         **kwargs: _FuncParams.kwargs,
     ) -> _ReturnType:
         return self.original_func(*args, **kwargs)
 
     @overload
-    async def kiq(  # noqa: D102
+    async def kiq(
         self: "AsyncTaskiqDecoratedTask[_FuncParams, Coroutine[Any, Any, _T]]",
         *args: _FuncParams.args,
         **kwargs: _FuncParams.kwargs,
     ) -> AsyncTaskiqTask[_T]:
         ...
 
     @overload
-    async def kiq(  # noqa: D102
+    async def kiq(
         self: "AsyncTaskiqDecoratedTask[_FuncParams, _ReturnType]",
         *args: _FuncParams.args,
         **kwargs: _FuncParams.kwargs,
     ) -> AsyncTaskiqTask[_ReturnType]:
         ...
 
     async def kiq(
```

### Comparing `taskiq-0.3.5/taskiq/exceptions.py` & `taskiq-0.4.0/taskiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/formatters/json_formatter.py` & `taskiq-0.4.0/taskiq/formatters/json_formatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
         :param message: message to send.
         :return: Dumped message.
         """
         return BrokerMessage(
             task_id=message.task_id,
             task_name=message.task_name,
-            message=message.json(),
+            message=message.json().encode(),
             labels=message.labels,
         )
 
-    def loads(self, message: BrokerMessage) -> TaskiqMessage:
+    def loads(self, message: bytes) -> TaskiqMessage:
         """
         Loads json from message.
 
         :param message: broker's message.
         :return: parsed taskiq message.
         """
-        return TaskiqMessage.parse_raw(message.message)
+        return TaskiqMessage.parse_raw(message)
```

### Comparing `taskiq-0.3.5/taskiq/funcs.py` & `taskiq-0.4.0/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/kicker.py` & `taskiq-0.4.0/taskiq/kicker.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,30 +84,30 @@
         :param broker: new broker instance.
         :return: Kicker with new broker.
         """
         self.broker = broker
         return self
 
     @overload
-    async def kiq(  # noqa: D102
+    async def kiq(
         self: "AsyncKicker[_FuncParams, Coroutine[Any, Any, _T]]",
         *args: _FuncParams.args,
         **kwargs: _FuncParams.kwargs,
     ) -> AsyncTaskiqTask[_T]:  # pragma: no cover
         ...
 
     @overload
-    async def kiq(  # noqa: D102
+    async def kiq(
         self: "AsyncKicker[_FuncParams, _ReturnType]",
         *args: _FuncParams.args,
         **kwargs: _FuncParams.kwargs,
     ) -> AsyncTaskiqTask[_ReturnType]:  # pragma: no cover
         ...
 
-    async def kiq(  # noqa: C901
+    async def kiq(
         self,
         *args: _FuncParams.args,
         **kwargs: _FuncParams.kwargs,
     ) -> Any:
         """
         This method sends function call over the network.
```

### Comparing `taskiq-0.3.5/taskiq/middlewares/retry_middleware.py` & `taskiq-0.4.0/taskiq/middlewares/retry_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/result_backends/dummy.py` & `taskiq-0.4.0/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/schedule_sources/label_based.py` & `taskiq-0.4.0/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/scheduler/merge_functions.py` & `taskiq-0.4.0/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/scheduler/scheduler.py` & `taskiq-0.4.0/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/state.py` & `taskiq-0.4.0/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.3.5/taskiq/task.py` & `taskiq-0.4.0/taskiq/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,30 @@
         """
         Method to check wether result is ready.
 
         :return: True if result is ready.
         """
 
     @abstractmethod
-    def get_result(  # noqa: WPS234
+    def get_result(
         self,
         with_logs: bool = False,
     ) -> Union[
         "TaskiqResult[_ReturnType]",
         Coroutine[Any, Any, "TaskiqResult[_ReturnType]"],
     ]:
         """
         Get actual execution result.
 
         :param with_logs: wether you want to fetch logs.
         :return: TaskiqResult.
         """
 
     @abstractmethod
-    def wait_result(  # noqa: WPS234
+    def wait_result(
         self,
         check_interval: float = 0.2,
         timeout: float = -1.0,
         with_logs: bool = False,
     ) -> Union[
         "TaskiqResult[_ReturnType]",
         Coroutine[Any, Any, "TaskiqResult[_ReturnType]"],
```

### Comparing `taskiq-0.3.5/PKG-INFO` & `taskiq-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.3.5
+Version: 0.4.0
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
@@ -25,25 +25,28 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
+Provides-Extra: metrics
+Provides-Extra: reload
 Provides-Extra: uv
 Provides-Extra: zmq
-Requires-Dist: gitignore-parser (>=0,<1)
+Requires-Dist: gitignore-parser (>=0,<1) ; extra == "reload"
 Requires-Dist: importlib-metadata
+Requires-Dist: prometheus_client (>=0,<1) ; extra == "metrics"
 Requires-Dist: pycron (>=3.0.0,<4.0.0)
 Requires-Dist: pydantic (>=1.6.2,<2.0.0)
 Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq"
 Requires-Dist: taskiq_dependencies (>=1,<2)
 Requires-Dist: typing-extensions (>=3.10.0.0)
 Requires-Dist: uvloop (>=0.16.0,<1) ; extra == "uv"
-Requires-Dist: watchdog (>=2.1.9,<3.0.0)
+Requires-Dist: watchdog (>=2.1.9,<3.0.0) ; extra == "reload"
 Project-URL: Documentation, https://taskiq-python.github.io/
 Project-URL: Repository, https://github.com/taskiq-python/taskiq
 Description-Content-Type: text/markdown
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/)
 [![PyPI](https://img.shields.io/pypi/v/taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/taskiq?style=for-the-badge)](https://pypistats.org/packages/taskiq)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.3.5 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.4.0 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -10,23 +10,25 @@
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: System :: Networking Classifier:
-Typing :: Typed Provides-Extra: uv Provides-Extra: zmq Requires-Dist:
-gitignore-parser (>=0,<1) Requires-Dist: importlib-metadata Requires-Dist:
-pycron (>=3.0.0,<4.0.0) Requires-Dist: pydantic (>=1.6.2,<2.0.0) Requires-Dist:
-pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq" Requires-Dist: taskiq_dependencies
-(>=1,<2) Requires-Dist: typing-extensions (>=3.10.0.0) Requires-Dist: uvloop
-(>=0.16.0,<1) ; extra == "uv" Requires-Dist: watchdog (>=2.1.9,<3.0.0) Project-
-URL: Documentation, https://taskiq-python.github.io/ Project-URL: Repository,
-https://github.com/taskiq-python/taskiq Description-Content-Type: text/markdown
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
+Typing :: Typed Provides-Extra: metrics Provides-Extra: reload Provides-Extra:
+uv Provides-Extra: zmq Requires-Dist: gitignore-parser (>=0,<1) ; extra ==
+"reload" Requires-Dist: importlib-metadata Requires-Dist: prometheus_client
+(>=0,<1) ; extra == "metrics" Requires-Dist: pycron (>=3.0.0,<4.0.0) Requires-
+Dist: pydantic (>=1.6.2,<2.0.0) Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra
+== "zmq" Requires-Dist: taskiq_dependencies (>=1,<2) Requires-Dist: typing-
+extensions (>=3.10.0.0) Requires-Dist: uvloop (>=0.16.0,<1) ; extra == "uv"
+Requires-Dist: watchdog (>=2.1.9,<3.0.0) ; extra == "reload" Project-URL:
+Documentation, https://taskiq-python.github.io/ Project-URL: Repository, https:
+//github.com/taskiq-python/taskiq Description-Content-Type: text/markdown [!
+[PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/) [![PyPI](https:/
 /img.shields.io/pypi/v/taskiq?style=for-the-badge)](https://pypi.org/project/
 taskiq/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/taskiq?style=for-
 the-badge)](https://pypistats.org/packages/taskiq)
 [https://raw.githubusercontent.com/taskiq-python/taskiq/master/imgs/logo.svg]
 ===============================================================================
 Taskiq is an asynchronous distributed task queue for python. This project takes
```

