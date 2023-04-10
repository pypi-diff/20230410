# Comparing `tmp/stlog-0.0.5.tar.gz` & `tmp/stlog-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlog-0.0.5.tar", max compression
+gzip compressed data, was "stlog-0.0.7.tar", max compression
```

## Comparing `stlog-0.0.5.tar` & `stlog-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-04-09 08:00:18.688375 stlog-0.0.5/LICENSE
--rw-r--r--   0        0        0     8010 2023-04-09 08:00:18.688375 stlog-0.0.5/README.md
--rw-r--r--   0        0        0     1240 2023-04-09 08:00:58.407341 stlog-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-09 08:00:57.979309 stlog-0.0.5/stlog/__init__.py
--rw-r--r--   0        0        0      301 2023-04-09 08:00:57.979309 stlog-0.0.5/stlog/__init__.py.restore_version
--rw-r--r--   0        0        0     2463 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/adapter.py
--rw-r--r--   0        0        0     7277 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/base.py
--rw-r--r--   0        0        0     2638 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/context.py
--rw-r--r--   0        0        0    12835 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/formatter.py
--rw-r--r--   0        0        0     2499 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/handler.py
--rw-r--r--   0        0        0     4580 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/output.py
--rw-r--r--   0        0        0     4793 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/setup.py
--rw-r--r--   0        0        0     8562 1970-01-01 00:00:00.000000 stlog-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-10 12:45:31.855016 stlog-0.0.7/LICENSE
+-rw-r--r--   0        0        0     8010 2023-04-10 12:45:31.855016 stlog-0.0.7/README.md
+-rw-r--r--   0        0        0     1240 2023-04-10 12:45:54.319048 stlog-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-10 12:45:53.971048 stlog-0.0.7/stlog/__init__.py
+-rw-r--r--   0        0        0      301 2023-04-10 12:45:53.971048 stlog-0.0.7/stlog/__init__.py.restore_version
+-rw-r--r--   0        0        0     2641 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/adapter.py
+-rw-r--r--   0        0        0     7277 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/base.py
+-rw-r--r--   0        0        0     2638 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/context.py
+-rw-r--r--   0        0        0    12794 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/formatter.py
+-rw-r--r--   0        0        0     2499 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/handler.py
+-rw-r--r--   0        0        0     4920 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/output.py
+-rw-r--r--   0        0        0     4793 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/setup.py
+-rw-r--r--   0        0        0     8562 1970-01-01 00:00:00.000000 stlog-0.0.7/PKG-INFO
```

### Comparing `stlog-0.0.5/LICENSE` & `stlog-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stlog-0.0.5/README.md` & `stlog-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `stlog-0.0.5/pyproject.toml` & `stlog-0.0.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stlog"
-version = "0.0.5"
+version = "0.0.7"
 description = ""
 authors = ["Fabien MARTY <fabien.marty@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "stlog"}]
 
 [tool.poetry.dependencies]
```

### Comparing `stlog-0.0.5/stlog/adapter.py` & `stlog-0.0.7/stlog/adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,20 @@
 
     def process(
         self, msg: typing.Any, kwargs: collections.abc.MutableMapping[str, typing.Any]
     ) -> tuple[typing.Any, collections.abc.MutableMapping[str, typing.Any]]:
         new_kwargs = {**LogContext._get(), **kwargs}
         return super().process(msg, new_kwargs)
 
+    def addFilter(self, filter):  # noqa: N802
+        self.logger.addFilter(filter)
+
+    def removeFilter(self, filter):  # noqa: N802
+        self.logger.removeFilter(filter)
+
 
 def getLogger(name: str | None = None, **kwargs) -> StLogLoggerAdapter:  # noqa: N802
     """Return a standard logger (adapted for `stlog` and `stlog.LogContext` support).
 
     You can pass some context key/values in `**kwargs` which will be specific to this logger.
 
     If you want to set more globally available context, use `stlog.LogContext` class.
```

### Comparing `stlog-0.0.5/stlog/base.py` & `stlog-0.0.7/stlog/base.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.5/stlog/context.py` & `stlog-0.0.7/stlog/context.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.5/stlog/formatter.py` & `stlog-0.0.7/stlog/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import fnmatch
 import json
 import logging
 import re
 import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from typing import Any, Callable, Literal, Sequence
+from typing import Any, Callable, Sequence
 
 from stlog.base import (
     GLOBAL_LOGGING_CONFIG,
     STLOG_EXTRA_KEY,
     check_env_true,
     logfmt_format,
     rich_logfmt_format,
@@ -50,38 +50,38 @@
 @dataclass
 class Formatter(logging.Formatter):
     """Abstract base class for `stlog` formatters.
 
     Attributes:
         fmt: the default format for the formatter.
         datefmt: the format to use for `{asctime}` placeholder.
+        style: FIXME
         include_extras_keys_fnmatchs: fnmatch patterns list for including keys in `{extra}` placeholder.
         exclude_extras_keys_fnmatchs: fnmatch patterns list for excluding keys in `{extra}` placeholder.
         extra_key_rename_fn: callable which takes a key name and return a renamed key to use
             (or None to ignore the key/value).
         extra_key_max_length: maximum size of extra keys to be included in `{extra}` placeholder
             (after this limit, the value will be truncated and ... will be added at the end, 0 means "no limit").
         converter: time converter function (use `time.gmtime` (default) for UTC date/times, use `time.time`
             for local date/times), if you change the default, please change also `datefmt` keyword.
 
     """
 
     fmt: str | None = DEFAULT_STLOG_HUMAN_FORMAT
     datefmt: str | None = DEFAULT_STLOG_DATE_FORMAT
-    style: Literal["%", "{", "$"] = "{"
-    validate: bool = True
+    style: str = "{"
     include_extras_keys_fnmatchs: Sequence[str] = ("*",)
     exclude_extras_keys_fnmatchs: Sequence[str] = ("_*",)
     extra_key_rename_fn: Callable[[str], str | None] | None = None
     extra_key_max_length: int = 32
     converter: Callable[[float | None], time.struct_time] = time.gmtime
 
     def __post_init__(self):
         super().__init__(  # explicit call because logging.Formatter is not a dataclass
-            fmt=self.fmt, datefmt=self.datefmt, validate=self.validate, style=self.style
+            fmt=self.fmt, datefmt=self.datefmt, style=self.style  # type: ignore
         )
         self.include_extra_keys_patterns: list[re.Pattern] = [
             re.compile(fnmatch.translate(x)) for x in self.include_extras_keys_fnmatchs
         ]
         self.exclude_extra_keys_patterns: list[re.Pattern] = [
             re.compile(fnmatch.translate(x)) for x in self.exclude_extras_keys_fnmatchs
         ]
```

### Comparing `stlog-0.0.5/stlog/handler.py` & `stlog-0.0.7/stlog/handler.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.5/stlog/output.py` & `stlog-0.0.7/stlog/output.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,30 +39,37 @@
 class Output:
     """Abstract output base class.
 
     Attributes:
         formatter: the Python logging Formatter to use.
         level: python logging level specific to this output
             (None means "use the global logging level").
+        filters: list of logging Filters (or simple callables) to filter some LogRecord
+            for this specific output.
 
     """
 
     _handler: logging.Handler = field(init=False, default_factory=logging.NullHandler)
     formatter: logging.Formatter | None = None
     level: int | str | None = None
+    filters: typing.Iterable[
+        typing.Callable[[logging.LogRecord], bool] | logging.Filter
+    ] = field(default_factory=list)
 
     def set_handler(
         self,
         handler: logging.Handler,
     ):
         """Configure the Python logging Handler to use."""
         self._handler = handler
         self._handler.setFormatter(self.get_formatter_or_raise())
         if self.level is not None:
             self._handler.setLevel(self.level)
+        for filter in self.filters:
+            self._handler.addFilter(filter)
 
     def get_handler(self) -> logging.Handler:
         """Get the configured Python logging Handler."""
         return self._handler
 
     def get_formatter_or_raise(self) -> logging.Formatter:
         if self.formatter is None:
```

### Comparing `stlog-0.0.5/stlog/setup.py` & `stlog-0.0.7/stlog/setup.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.5/PKG-INFO` & `stlog-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlog
-Version: 0.0.5
+Version: 0.0.7
 Summary: 
 License: MIT
 Author: Fabien MARTY
 Author-email: fabien.marty@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

