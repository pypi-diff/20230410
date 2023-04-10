# Comparing `tmp/pytest-sugar-0.9.6.tar.gz` & `tmp/pytest-sugar-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-sugar-0.9.6.tar", last modified: Sat Nov  5 08:03:13 2022, max compression
+gzip compressed data, was "pytest-sugar-0.9.7.tar", last modified: Mon Apr 10 11:05:54 2023, max compression
```

## Comparing `pytest-sugar-0.9.6.tar` & `pytest-sugar-0.9.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 bansku     (501) staff       (20)        0 2022-11-05 08:03:13.918934 pytest-sugar-0.9.6/
--rw-r--r--   0 bansku     (501) staff       (20)     3531 2022-11-05 08:00:09.000000 pytest-sugar-0.9.6/CHANGES.rst
--rw-r--r--   0 bansku     (501) staff       (20)      191 2022-04-02 17:00:48.000000 pytest-sugar-0.9.6/CONTRIBUTORS.rst
--rw-r--r--   0 bansku     (501) staff       (20)     1490 2022-04-02 17:00:48.000000 pytest-sugar-0.9.6/LICENSE
--rw-r--r--   0 bansku     (501) staff       (20)       92 2022-04-02 17:00:48.000000 pytest-sugar-0.9.6/MANIFEST.in
--rw-r--r--   0 bansku     (501) staff       (20)     2783 2022-11-05 08:03:13.919092 pytest-sugar-0.9.6/PKG-INFO
--rw-r--r--   0 bansku     (501) staff       (20)     1330 2022-11-05 07:57:08.000000 pytest-sugar-0.9.6/README.md
-drwxr-xr-x   0 bansku     (501) staff       (20)        0 2022-11-05 08:03:13.918717 pytest-sugar-0.9.6/pytest_sugar.egg-info/
--rw-r--r--   0 bansku     (501) staff       (20)     2783 2022-11-05 08:03:13.000000 pytest-sugar-0.9.6/pytest_sugar.egg-info/PKG-INFO
--rw-r--r--   0 bansku     (501) staff       (20)      368 2022-11-05 08:03:13.000000 pytest-sugar-0.9.6/pytest_sugar.egg-info/SOURCES.txt
--rw-r--r--   0 bansku     (501) staff       (20)        1 2022-11-05 08:03:13.000000 pytest-sugar-0.9.6/pytest_sugar.egg-info/dependency_links.txt
--rw-r--r--   0 bansku     (501) staff       (20)       32 2022-11-05 08:03:13.000000 pytest-sugar-0.9.6/pytest_sugar.egg-info/entry_points.txt
--rw-r--r--   0 bansku     (501) staff       (20)        1 2022-04-02 17:01:33.000000 pytest-sugar-0.9.6/pytest_sugar.egg-info/not-zip-safe
--rw-r--r--   0 bansku     (501) staff       (20)       45 2022-11-05 08:03:13.000000 pytest-sugar-0.9.6/pytest_sugar.egg-info/requires.txt
--rw-r--r--   0 bansku     (501) staff       (20)       13 2022-11-05 08:03:13.000000 pytest-sugar-0.9.6/pytest_sugar.egg-info/top_level.txt
--rw-r--r--   0 bansku     (501) staff       (20)    22204 2022-11-05 08:02:13.000000 pytest-sugar-0.9.6/pytest_sugar.py
--rw-r--r--   0 bansku     (501) staff       (20)       67 2022-11-05 08:03:13.919517 pytest-sugar-0.9.6/setup.cfg
--rw-r--r--   0 bansku     (501) staff       (20)     2452 2022-04-02 17:00:48.000000 pytest-sugar-0.9.6/setup.py
--rw-r--r--   0 bansku     (501) staff       (20)    15229 2022-04-02 17:00:48.000000 pytest-sugar-0.9.6/test_sugar.py
--rw-r--r--   0 bansku     (501) staff       (20)     1988 2022-04-02 17:00:48.000000 pytest-sugar-0.9.6/tox.ini
+drwxr-xr-x   0 jm         (501) staff       (20)        0 2023-04-10 11:05:54.007958 pytest-sugar-0.9.7/
+-rw-r--r--   0 jm         (501) staff       (20)     3683 2023-04-10 11:05:52.000000 pytest-sugar-0.9.7/CHANGES.rst
+-rw-r--r--   0 jm         (501) staff       (20)      191 2022-11-08 15:15:38.000000 pytest-sugar-0.9.7/CONTRIBUTORS.rst
+-rw-r--r--   0 jm         (501) staff       (20)     1490 2022-11-08 15:15:38.000000 pytest-sugar-0.9.7/LICENSE
+-rw-r--r--   0 jm         (501) staff       (20)       93 2022-11-10 16:12:09.000000 pytest-sugar-0.9.7/MANIFEST.in
+-rw-r--r--   0 jm         (501) staff       (20)     3858 2023-04-10 11:05:54.008039 pytest-sugar-0.9.7/PKG-INFO
+-rw-r--r--   0 jm         (501) staff       (20)     2533 2023-04-10 09:38:24.000000 pytest-sugar-0.9.7/README.md
+-rw-r--r--   0 jm         (501) staff       (20)     1392 2023-04-10 11:05:52.000000 pytest-sugar-0.9.7/pyproject.toml
+drwxr-xr-x   0 jm         (501) staff       (20)        0 2023-04-10 11:05:54.007815 pytest-sugar-0.9.7/pytest_sugar.egg-info/
+-rw-r--r--   0 jm         (501) staff       (20)     3858 2023-04-10 11:05:53.000000 pytest-sugar-0.9.7/pytest_sugar.egg-info/PKG-INFO
+-rw-r--r--   0 jm         (501) staff       (20)      383 2023-04-10 11:05:53.000000 pytest-sugar-0.9.7/pytest_sugar.egg-info/SOURCES.txt
+-rw-r--r--   0 jm         (501) staff       (20)        1 2023-04-10 11:05:53.000000 pytest-sugar-0.9.7/pytest_sugar.egg-info/dependency_links.txt
+-rw-r--r--   0 jm         (501) staff       (20)       32 2023-04-10 11:05:53.000000 pytest-sugar-0.9.7/pytest_sugar.egg-info/entry_points.txt
+-rw-r--r--   0 jm         (501) staff       (20)        1 2023-04-03 04:12:59.000000 pytest-sugar-0.9.7/pytest_sugar.egg-info/not-zip-safe
+-rw-r--r--   0 jm         (501) staff       (20)       78 2023-04-10 11:05:53.000000 pytest-sugar-0.9.7/pytest_sugar.egg-info/requires.txt
+-rw-r--r--   0 jm         (501) staff       (20)       13 2023-04-10 11:05:53.000000 pytest-sugar-0.9.7/pytest_sugar.egg-info/top_level.txt
+-rw-r--r--   0 jm         (501) staff       (20)    23043 2023-04-10 11:05:52.000000 pytest-sugar-0.9.7/pytest_sugar.py
+-rw-r--r--   0 jm         (501) staff       (20)      144 2023-04-10 11:05:54.008278 pytest-sugar-0.9.7/setup.cfg
+-rw-r--r--   0 jm         (501) staff       (20)     2405 2023-03-29 11:10:14.000000 pytest-sugar-0.9.7/setup.py
+-rw-r--r--   0 jm         (501) staff       (20)    15526 2023-03-29 11:10:14.000000 pytest-sugar-0.9.7/test_sugar.py
+-rw-r--r--   0 jm         (501) staff       (20)      664 2022-11-10 16:12:09.000000 pytest-sugar-0.9.7/tox.ini
```

### Comparing `pytest-sugar-0.9.6/CHANGES.rst` & `pytest-sugar-0.9.7/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Changelog
 ---------
 
-A list of changes between each release.
+0.9.7 - 2023-04-10
+^^^^^^^^^^^^^^^^^^
+
+- For long-running tests, display minutes and not only seconds (thanks @last-partizan)
+- Add support for Pytest’s ``--header`` option (thanks @wiresv)
 
 0.9.6 (2022-11-5)
 ^^^^^^^^^^^^^^^^^^^
 
 - Remove py.std calls (thanks @alexcjohnson)
 
 0.9.5 (2022-07-10)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-sugar-0.9.6/LICENSE` & `pytest-sugar-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sugar-0.9.6/pytest_sugar.py` & `pytest-sugar-0.9.7/pytest_sugar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,218 +1,245 @@
-# -*- coding: utf-8 -*-
 """
 pytest_sugar
 ~~~~~~~~~~~~
 
 pytest-sugar is a plugin for pytest that changes the default look
 and feel of pytest (e.g. progressbar, show tests that fail instantly).
 
 :copyright: see LICENSE for details
 :license: BSD, see LICENSE for more details.
 """
-from __future__ import unicode_literals
+
+import dataclasses
 import locale
 import os
 import re
 import sys
 import time
-from packaging.version import parse
-
-try:
-    from configparser import ConfigParser
-except ImportError:
-    from ConfigParser import ConfigParser
-
-from termcolor import colored
+from configparser import ConfigParser  # type: ignore
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import pytest
-from _pytest.terminal import TerminalReporter
-
+from _pytest.config.argparsing import Parser
+from _pytest.main import Session
+from _pytest.nodes import Item
+from _pytest.reports import BaseReport, CollectReport, TestReport
+from _pytest.terminal import TerminalReporter, format_session_duration
+from termcolor import colored
 
-__version__ = '0.9.6'
+__version__ = "0.9.7"
 
 LEN_RIGHT_MARGIN = 0
 LEN_PROGRESS_PERCENTAGE = 5
-LEN_PROGRESS_BAR_SETTING = '10'
-LEN_PROGRESS_BAR = None
-THEME = {
-    'header': 'magenta',
-    'skipped': 'blue',
-    'success': 'green',
-    'warning': 'yellow',
-    'fail': 'red',
-    'error': 'red',
-    'xfailed': 'green',
-    'xpassed': 'red',
-    'progressbar': 'green',
-    'progressbar_fail': 'red',
-    'progressbar_background': 'grey',
-    'path': 'cyan',
-    'name': None,
-    'symbol_passed': '✓',
-    'symbol_skipped': 's',
-    'symbol_failed': '⨯',
-    'symbol_failed_not_call': 'ₓ',
-    'symbol_xfailed_skipped': 'x',
-    'symbol_xfailed_failed': 'X',
-    'symbol_unknown': '?',
-    'unknown': 'blue',
-    'symbol_rerun': 'R',
-    'rerun': 'blue',
-}
-PROGRESS_BAR_BLOCKS = [
-    ' ', '▏', '▎', '▎', '▍', '▍', '▌', '▌', '▋', '▋', '▊', '▊', '▉', '▉', '█',
+LEN_PROGRESS_BAR_SETTING = "10"
+LEN_PROGRESS_BAR: Optional[int] = None
+
+
+@dataclasses.dataclass
+class Theme:
+    header: Optional[str] = "magenta"
+    skipped: Optional[str] = "blue"
+    success: Optional[str] = "green"
+    warning: Optional[str] = "yellow"
+    fail: Optional[str] = "red"
+    error: Optional[str] = "red"
+    xfailed: Optional[str] = "green"
+    xpassed: Optional[str] = "red"
+    progressbar: Optional[str] = "green"
+    progressbar_fail: Optional[str] = "red"
+    progressbar_background: Optional[str] = "grey"
+    path: Optional[str] = "cyan"
+    name = None
+    symbol_passed: str = "✓"
+    symbol_skipped: str = "s"
+    symbol_failed: str = "⨯"
+    symbol_failed_not_call: str = "ₓ"
+    symbol_xfailed_skipped: str = "x"
+    symbol_xfailed_failed: str = "X"
+    symbol_unknown: str = "?"
+    unknown: Optional[str] = "blue"
+    symbol_rerun: Optional[str] = "R"
+    rerun: Optional[str] = "blue"
+
+    def __getitem__(self, x):
+        return getattr(self, x)
+
+
+THEME: Theme = Theme()
+PROGRESS_BAR_BLOCKS: List[str] = [
+    " ",
+    "▏",
+    "▎",
+    "▎",
+    "▍",
+    "▍",
+    "▌",
+    "▌",
+    "▋",
+    "▋",
+    "▊",
+    "▊",
+    "▉",
+    "▉",
+    "█",
 ]
 
 
 def flatten(seq):
     for x in seq:
         if isinstance(x, (list, tuple)):
-            for y in flatten(x):
-                yield y
+            yield from flatten(x)
         else:
             yield x
 
 
-def pytest_runtestloop(session):
-    reporter = session.config.pluginmanager.getplugin('terminalreporter')
+def pytest_collection_finish(session: Session) -> None:
+    reporter = session.config.pluginmanager.getplugin("terminalreporter")
     if reporter:
         reporter.tests_count = len(session.items)
 
 
-class DeferredXdistPlugin(object):
+class DeferredXdistPlugin:
     def pytest_xdist_node_collection_finished(self, node, ids):
-        terminal_reporter = node.config.pluginmanager.getplugin(
-            'terminalreporter'
-        )
+        terminal_reporter = node.config.pluginmanager.getplugin("terminalreporter")
         if terminal_reporter:
             terminal_reporter.tests_count = len(ids)
 
 
-def pytest_deselected(items):
-    """ Update tests_count to not include deselected tests """
+def pytest_deselected(items: Sequence[Item]) -> None:
+    """Update tests_count to not include deselected tests"""
     if len(items) > 0:
         pluginmanager = items[0].config.pluginmanager
-        terminal_reporter = pluginmanager.getplugin('terminalreporter')
-        if (hasattr(terminal_reporter, 'tests_count')
-                and terminal_reporter.tests_count > 0):
+        terminal_reporter = pluginmanager.getplugin("terminalreporter")
+        if (
+            hasattr(terminal_reporter, "tests_count")
+            and terminal_reporter.tests_count > 0
+        ):
             terminal_reporter.tests_count -= len(items)
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser: Parser) -> None:
     group = parser.getgroup("terminal reporting", "reporting", after="general")
     group._addoption(
-        '--old-summary', action="store_true",
-        dest="tb_summary", default=False,
-        help=(
-            "Show tests that failed instead of one-line tracebacks"
-        )
+        "--old-summary",
+        action="store_true",
+        dest="tb_summary",
+        default=False,
+        help=("Show tests that failed instead of one-line tracebacks"),
     )
     group._addoption(
-        '--force-sugar', action="store_true",
-        dest="force_sugar", default=False,
-        help=(
-            "Force pytest-sugar output even when not in real terminal"
-        )
+        "--force-sugar",
+        action="store_true",
+        dest="force_sugar",
+        default=False,
+        help=("Force pytest-sugar output even when not in real terminal"),
     )
 
 
-def pytest_sessionstart(session):
-    global LEN_PROGRESS_BAR_SETTING
+def pytest_sessionstart(session: Session) -> None:
+    global THEME, LEN_PROGRESS_BAR_SETTING
     config = ConfigParser()
-    config.read([
-        'pytest-sugar.conf',
-        os.path.expanduser('~/.pytest-sugar.conf')
-    ])
+    config.read(["pytest-sugar.conf", os.path.expanduser("~/.pytest-sugar.conf")])
+
+    theme_attributes: Dict[str, Optional[str]] = {}
+    fields: Tuple[dataclasses.Field, ...] = dataclasses.fields(Theme)
 
-    for key in THEME:
-        if not config.has_option('theme', key):
+    for field in fields:
+        key = field.name
+        if not config.has_option("theme", key):
             continue
 
-        value = config.get("theme", key)
-        value = value.lower()
-        if value in ('', 'none'):
+        value_str: str = config.get("theme", key).lower()
+        value: Optional[str] = value_str
+        if value in ("", "none"):
             value = None
 
-        THEME[key] = value
+        theme_attributes[key] = value
+
+    if config.has_option("sugar", "progressbar_length"):
+        LEN_PROGRESS_BAR_SETTING = config.get("sugar", "progressbar_length")
 
-    if config.has_option('sugar', 'progressbar_length'):
-        LEN_PROGRESS_BAR_SETTING = config.get('sugar', 'progressbar_length')
+    THEME = Theme(**theme_attributes)  # type: ignore
 
 
-def strip_colors(text):
-    ansi_escape = re.compile(r'\x1b[^m]*m')
-    stripped = ansi_escape.sub('', text)
+def strip_colors(text: str) -> str:
+    ansi_escape = re.compile(r"\x1b[^m]*m")
+    stripped = ansi_escape.sub("", text)
     return stripped
 
 
-def real_string_length(string):
+def real_string_length(string: str) -> int:
     return len(strip_colors(string))
 
 
 IS_SUGAR_ENABLED = False
 
 
-@pytest.mark.trylast
+@pytest.hookimpl(trylast=True)
 def pytest_configure(config):
     global IS_SUGAR_ENABLED
 
-    if sys.stdout.isatty() or config.getvalue('force_sugar'):
+    if sys.stdout.isatty() or config.getvalue("force_sugar"):
         IS_SUGAR_ENABLED = True
 
-    if config.pluginmanager.hasplugin('xdist'):
+    if config.pluginmanager.hasplugin("xdist"):
         try:
-            import xdist
+            import xdist  # type: ignore
         except ImportError:
             pass
         else:
             from packaging import version
+
             xdist_version = version.Version(xdist.__version__)
-            if xdist_version >= version.Version('1.14'):
+            if xdist_version >= version.Version("1.14"):
                 config.pluginmanager.register(DeferredXdistPlugin())
 
-    if IS_SUGAR_ENABLED and not getattr(config, 'slaveinput', None):
+    if IS_SUGAR_ENABLED and not getattr(config, "slaveinput", None):
         # Get the standard terminal reporter plugin and replace it with our
-        standard_reporter = config.pluginmanager.getplugin('terminalreporter')
+        standard_reporter = config.pluginmanager.getplugin("terminalreporter")
         sugar_reporter = SugarTerminalReporter(standard_reporter)
         config.pluginmanager.unregister(standard_reporter)
-        config.pluginmanager.register(sugar_reporter, 'terminalreporter')
+        config.pluginmanager.register(sugar_reporter, "terminalreporter")
 
 
-def pytest_report_teststatus(report):
+def pytest_report_teststatus(report: BaseReport) -> Optional[Tuple[str, str, str]]:
     if not IS_SUGAR_ENABLED:
-        return
+        return None
 
     if report.passed:
-        letter = colored(THEME['symbol_passed'], THEME['success'])
+        letter = colored(THEME.symbol_passed, THEME.success)
     elif report.skipped:
-        letter = colored(THEME['symbol_skipped'], THEME['skipped'])
+        letter = colored(THEME.symbol_skipped, THEME.skipped)
     elif report.failed:
-        letter = colored(THEME['symbol_failed'], THEME['fail'])
+        letter = colored(THEME.symbol_failed, THEME.fail)
         if report.when != "call":
-            letter = colored(THEME['symbol_failed_not_call'], THEME['fail'])
-    elif report.outcome == 'rerun':
-        letter = colored(THEME['symbol_rerun'], THEME['rerun'])
+            letter = colored(THEME.symbol_failed_not_call, THEME.fail)
+    elif report.outcome == "rerun":
+        letter = colored(THEME.symbol_rerun, THEME.rerun)
     else:
-        letter = colored(THEME['symbol_unknown'], THEME['unknown'])
+        letter = colored(THEME.symbol_unknown, THEME.unknown)
 
     if hasattr(report, "wasxfail"):
         if report.skipped:
-            return "xfailed", colored(
-                THEME['symbol_xfailed_skipped'], THEME['xfailed']
-            ), "xfail"
-        elif report.passed:
-            return "xpassed", colored(
-                THEME['symbol_xfailed_failed'], THEME['xpassed']
-            ), "XPASS"
+            return (
+                "xfailed",
+                colored(THEME.symbol_xfailed_skipped, THEME.xfailed),
+                "xfail",
+            )
+        if report.passed:
+            return (
+                "xpassed",
+                colored(THEME.symbol_xfailed_failed, THEME.xpassed),
+                "XPASS",
+            )
 
     return report.outcome, letter, report.outcome.upper()
 
 
-class SugarTerminalReporter(TerminalReporter):
+class SugarTerminalReporter(TerminalReporter):  # type: ignore
     def __init__(self, reporter):
         TerminalReporter.__init__(self, reporter.config)
         self.paths_left = []
         self.tests_count = 0
         self.tests_taken = 0
         self.reports = []
         self.unreported_errors = []
@@ -220,410 +247,399 @@
         self.reset_tracked_lines()
 
     def reset_tracked_lines(self):
         self.current_lines = {}
         self.current_line_nums = {}
         self.current_line_num = 0
 
-    def report_collect(self, final=False):
-        pass
-
-    def pytest_collectreport(self, report):
+    def pytest_collectreport(self, report: CollectReport) -> None:
         TerminalReporter.pytest_collectreport(self, report)
         if report.location[0]:
-            self.paths_left.append(
-                os.path.join(os.getcwd(), report.location[0])
-            )
+            self.paths_left.append(os.path.join(os.getcwd(), report.location[0]))
         if report.failed:
             self.rewrite("")
             self.print_failure(report)
 
-    def pytest_sessionstart(self, session):
+    def pytest_sessionstart(self, session: Session) -> None:
         self._session = session
         self._sessionstarttime = time.time()
+        if self.no_header:
+            return
         verinfo = ".".join(map(str, sys.version_info[:3]))
         self.write_line(
             "Test session starts "
-            "(platform: %s, Python %s, pytest %s, pytest-sugar %s)" % (
-                sys.platform, verinfo, pytest.__version__, __version__,
-            ), bold=True
+            "(platform: %s, Python %s, pytest %s, pytest-sugar %s)"
+            % (
+                sys.platform,
+                verinfo,
+                pytest.__version__,
+                __version__,
+            ),
+            bold=True,
         )
         lines = self.config.hook.pytest_report_header(
-            config=self.config, startdir=self.startdir)
+            config=self.config, startdir=self.startpath
+        )
         lines.reverse()
         for line in flatten(lines):
             self.write_line(line)
 
-    def write_fspath_result(self, fspath, res):
+    def write_fspath_result(self, nodeid: str, res, **markup: bool) -> None:
         return
 
-    def insert_progress(self, report):
+    def insert_progress(self, report: Union[CollectReport, TestReport]) -> None:
         def get_progress_bar():
             length = LEN_PROGRESS_BAR
             if not length:
-                return ''
+                return ""
 
-            p = (
-                float(self.tests_taken) / self.tests_count
-                if self.tests_count else 0
-            )
+            p = float(self.tests_taken) / self.tests_count if self.tests_count else 0
             floored = int(p * length)
-            rem = int(round(
-                (p * length - floored) * (len(PROGRESS_BAR_BLOCKS) - 1)
-            ))
+            rem = int(round((p * length - floored) * (len(PROGRESS_BAR_BLOCKS) - 1)))
             progressbar = "%i%% " % round(p * 100)
             # make sure we only report 100% at the last test
             if progressbar == "100% " and self.tests_taken < self.tests_count:
                 progressbar = "99% "
 
             # if at least one block indicates failure,
             # then the percentage should reflect that
             if [1 for block, success in self.progress_blocks if not success]:
-                progressbar = colored(progressbar, THEME['fail'])
+                progressbar = colored(progressbar, THEME.fail)
             else:
-                progressbar = colored(progressbar, THEME['success'])
+                progressbar = colored(progressbar, THEME.success)
 
             bar = PROGRESS_BAR_BLOCKS[-1] * floored
             if rem > 0:
                 bar += PROGRESS_BAR_BLOCKS[rem]
-            bar += ' ' * (LEN_PROGRESS_BAR - len(bar))
+            bar += " " * (LEN_PROGRESS_BAR - len(bar))
 
             last = 0
             last_theme = None
 
-            progressbar_background = THEME['progressbar_background']
+            progressbar_background = THEME.progressbar_background
             if progressbar_background is None:
                 on_color = None
             else:
-                on_color = 'on_' + progressbar_background
+                on_color = "on_" + progressbar_background
 
             for block, success in self.progress_blocks:
                 if success:
-                    theme = THEME['progressbar']
+                    theme = THEME.progressbar
                 else:
-                    theme = THEME['progressbar_fail']
+                    theme = THEME.progressbar_fail
 
                 if last < block:
-                    progressbar += colored(bar[last:block],
-                                           last_theme,
-                                           on_color)
-
-                progressbar += colored(bar[block],
-                                       theme,
-                                       on_color)
+                    progressbar += colored(bar[last:block], last_theme, on_color)
+
+                progressbar += colored(bar[block], theme, on_color)
                 last = block + 1
                 last_theme = theme
 
             if last < len(bar):
-                progressbar += colored(bar[last:len(bar)],
-                                       last_theme,
-                                       on_color)
+                progressbar += colored(bar[last : len(bar)], last_theme, on_color)
 
             return progressbar
 
         append_string = get_progress_bar()
 
         path = self.report_key(report)
         current_line = self.current_lines.get(path, "")
         line_num = self.current_line_nums.get(path, self.current_line_num)
 
         console_width = self._tw.fullwidth
         num_spaces = (
-            console_width - real_string_length(current_line) -
-            real_string_length(append_string) - LEN_RIGHT_MARGIN
+            console_width
+            - real_string_length(current_line)
+            - real_string_length(append_string)
+            - LEN_RIGHT_MARGIN
         )
         full_line = current_line + " " * num_spaces
         full_line += append_string
 
         self.overwrite(full_line, self.current_line_num - line_num)
 
-    def overwrite(self, line, rel_line_num):
+    def overwrite(self, line: str, rel_line_num: int) -> None:
         # Move cursor up rel_line_num lines
         if rel_line_num > 0:
             self.write("\033[%dA" % rel_line_num)
 
         # Overwrite the line
-        self.write("\r%s" % line)
+        self.write(f"\r{line}")
 
         # Return cursor to original line
         if rel_line_num > 0:
             self.write("\033[%dB" % rel_line_num)
 
-    def get_max_column_for_test_status(self):
+    def get_max_column_for_test_status(self) -> int:
+        assert LEN_PROGRESS_BAR
+
         return (
             self._tw.fullwidth
             - LEN_PROGRESS_PERCENTAGE
             - LEN_PROGRESS_BAR
             - LEN_RIGHT_MARGIN
         )
 
-    def begin_new_line(self, report, print_filename):
+    def begin_new_line(
+        self, report: Union[CollectReport, TestReport], print_filename: bool
+    ) -> None:
         path = self.report_key(report)
         self.current_line_num += 1
         if len(report.fspath) > self.get_max_column_for_test_status() - 5:
-            fspath = '...' + report.fspath[
-                -(self.get_max_column_for_test_status() - 5 - 5):
-            ]
+            fspath = (
+                "..."
+                + report.fspath[-(self.get_max_column_for_test_status() - 5 - 5) :]
+            )
         else:
             fspath = report.fspath
         basename = os.path.basename(fspath)
         if print_filename:
             if self.showlongtestinfo:
                 test_location = report.location[0]
                 test_name = report.location[2]
             else:
-                test_location = fspath[0:-len(basename)]
-                test_name = fspath[-len(basename):]
+                test_location = fspath[0 : -len(basename)]
+                test_name = fspath[-len(basename) :]
             if test_location:
                 pass
                 # only replace if test_location is not empty, if it is,
                 # test_name contains the filename
                 # FIXME: This doesn't work.
                 # test_name = test_name.replace('.', '::')
             self.current_lines[path] = (
-                " " +
-                colored(test_location, THEME['path']) +
-                ("::" if self.verbosity > 0 else "") +
-                colored(test_name, THEME['name']) +
                 " "
+                + colored(test_location, THEME.path)
+                + ("::" if self.verbosity > 0 else "")
+                + colored(test_name, THEME.name)
+                + " "
             )
         else:
             self.current_lines[path] = " " * (2 + len(fspath))
         self.current_line_nums[path] = self.current_line_num
         self.write("\r\n")
 
-    def reached_last_column_for_test_status(self, report):
-        len_line = real_string_length(
-            self.current_lines[self.report_key(report)])
+    def reached_last_column_for_test_status(
+        self, report: Union[CollectReport, TestReport]
+    ) -> bool:
+        len_line = real_string_length(self.current_lines[self.report_key(report)])
         return len_line >= self.get_max_column_for_test_status()
 
-    def pytest_runtest_logstart(self, nodeid, location):
+    def pytest_runtest_logstart(self, nodeid, location) -> None:
         # Prevent locationline from being printed since we already
         # show the module_name & in verbose mode the test name.
         pass
 
-    def pytest_runtest_logfinish(self):
+    def pytest_runtest_logfinish(self, nodeid: str) -> None:
         # prevent the default implementation to try to show
         # pytest's default progress
         pass
 
-    def report_key(self, report):
+    def report_key(self, report: Union[CollectReport, TestReport]) -> Any:
         """Returns a key to identify which line the report should write to."""
-        return report.location if self.showlongtestinfo else report.fspath
+        return (
+            (report.location or "") if self.showlongtestinfo else (report.fspath or "")
+        )
 
-    def pytest_runtest_logreport(self, report):
+    def pytest_runtest_logreport(self, report: TestReport) -> None:
         global LEN_PROGRESS_BAR_SETTING, LEN_PROGRESS_BAR
 
         res = pytest_report_teststatus(report=report)
+        assert res
         cat, letter, word = res
         self.stats.setdefault(cat, []).append(report)
 
         if not LEN_PROGRESS_BAR:
-            if LEN_PROGRESS_BAR_SETTING.endswith('%'):
+            if LEN_PROGRESS_BAR_SETTING.endswith("%"):
                 LEN_PROGRESS_BAR = (
-                    self._tw.fullwidth *
-                    int(LEN_PROGRESS_BAR_SETTING[:-1]) // 100
+                    self._tw.fullwidth * int(LEN_PROGRESS_BAR_SETTING[:-1]) // 100
                 )
             else:
                 LEN_PROGRESS_BAR = int(LEN_PROGRESS_BAR_SETTING)
 
         self.reports.append(report)
-        if report.outcome == 'failed':
+        if report.outcome == "failed":
             print("")
             self.print_failure(report)
             # Ignore other reports or it will cause duplicated letters
-        if report.when == 'teardown':
+        if report.when == "teardown":
             self.tests_taken += 1
             self.insert_progress(report)
             path = os.path.join(os.getcwd(), report.location[0])
 
-        if report.when == 'call' or report.skipped:
+        if report.when == "call" or report.skipped:
             path = self.report_key(report)
             if path not in self.current_line_nums:
                 self.begin_new_line(report, print_filename=True)
             elif self.reached_last_column_for_test_status(report):
                 # Print filename if another line was inserted in-between
                 print_filename = (
-                    self.current_line_nums[self.report_key(report)] !=
-                    self.current_line_num)
+                    self.current_line_nums[self.report_key(report)]
+                    != self.current_line_num
+                )
                 self.begin_new_line(report, print_filename)
 
             self.current_lines[path] = self.current_lines[path] + letter
 
             block = int(
                 float(self.tests_taken) * LEN_PROGRESS_BAR / self.tests_count
-                if self.tests_count else 0
+                if self.tests_count
+                else 0
             )
             if report.failed:
-                if (
-                    not self.progress_blocks or
-                    self.progress_blocks[-1][0] != block
-                ):
+                if not self.progress_blocks or self.progress_blocks[-1][0] != block:
                     self.progress_blocks.append([block, False])
-                elif (
-                    self.progress_blocks and
-                    self.progress_blocks[-1][0] == block
-                ):
+                elif self.progress_blocks and self.progress_blocks[-1][0] == block:
                     self.progress_blocks[-1][1] = False
             else:
-                if (
-                    not self.progress_blocks or
-                    self.progress_blocks[-1][0] != block
-                ):
+                if not self.progress_blocks or self.progress_blocks[-1][0] != block:
                     self.progress_blocks.append([block, True])
 
             if not letter and not word:
                 return
             if self.verbosity > 0:
-                markup = {'red': True}
+                markup = {"red": True}
                 if isinstance(word, tuple):
                     word, markup = word
                 else:
                     if report.passed:
-                        markup = {'green': True}
+                        markup = {"green": True}
                     elif report.skipped:
-                        markup = {'yellow': True}
+                        markup = {"yellow": True}
                     elif hasattr(report, "rerun") and isinstance(report.rerun, int):
-                        markup = {'blue': True}
+                        markup = {"blue": True}
                 line = self._locationline(str(report.fspath), *report.location)
-                if hasattr(report, 'node'):
+                if hasattr(report, "node"):
                     self._tw.write("\r\n")
                     self.current_line_num += 1
-                    if hasattr(report, 'node'):
-                        self._tw.write("[%s] " % report.node.gateway.id)
+                    if hasattr(report, "node"):
+                        self._tw.write(f"[{report.node.gateway.id}] ")
                     self._tw.write(word, **markup)
                     self._tw.write(" " + line)
                     self.currentfspath = -2
 
-    def count(self, key, when=('call',)):
-        if self.stats.get(key):
-            return len([
-                x for x in self.stats.get(key)
-                if not hasattr(x, 'when') or x.when in when
-            ])
-        else:
-            return 0
+    def count(self, key: str, when: tuple = ("call",)) -> int:
+        value = self.stats.get(key)
+        if value:
+            return len([x for x in value if not hasattr(x, "when") or x.when in when])
+        return 0
 
-    def summary_stats(self):
+    def summary_stats(self) -> None:
         session_duration = time.time() - self._sessionstarttime
 
-        print("\nResults (%.2fs):" % round(session_duration, 2))
-        if self.count('passed') > 0:
-            self.write_line(colored(
-                "   % 5d passed" % self.count('passed'),
-                THEME['success']
-            ))
-
-        if self.count('xpassed') > 0:
-            self.write_line(colored(
-                "   % 5d xpassed" % self.count('xpassed'),
-                THEME['xpassed']
-            ))
-
-        if self.count('failed', when=['call']) > 0:
-            self.write_line(colored(
-                "   % 5d failed" % self.count('failed', when=['call']),
-                THEME['fail']
-            ))
-            for report in self.stats['failed']:
-                if report.when != 'call':
+        print(f"\nResults ({format_session_duration(session_duration)}):")
+        if self.count("passed") > 0:
+            self.write_line(
+                colored("   % 5d passed" % self.count("passed"), THEME.success)
+            )
+
+        if self.count("xpassed") > 0:
+            self.write_line(
+                colored("   % 5d xpassed" % self.count("xpassed"), THEME.xpassed)
+            )
+
+        if self.count("failed", when=("call",)) > 0:
+            self.write_line(
+                colored(
+                    "   % 5d failed" % self.count("failed", when=("call",)),
+                    THEME.fail,
+                )
+            )
+            for report in self.stats["failed"]:
+                if report.when != "call":
                     continue
                 if self.config.option.tb_summary:
                     crashline = self._get_decoded_crashline(report)
                 else:
                     path = os.path.dirname(report.location[0])
                     name = os.path.basename(report.location[0])
                     lineno = self._get_lineno_from_report(report)
-                    crashline = '%s%s%s:%s %s' % (
-                        colored(path, THEME['path']),
-                        '/' if path else '',
-                        colored(name, THEME['name']),
-                        lineno if lineno else '?',
-                        colored(report.location[2], THEME['fail'])
+                    crashline = "{}{}{}:{} {}".format(
+                        colored(path, THEME.path),
+                        "/" if path else "",
+                        colored(name, THEME.name),
+                        lineno if lineno else "?",
+                        colored(report.location[2], THEME.fail),
                     )
-                self.write_line("         - %s" % crashline)
+                self.write_line(f"         - {crashline}")
 
-        if self.count('failed', when=['setup', 'teardown']) > 0:
-            self.write_line(colored(
-                "   % 5d error" % (
-                    self.count('failed', when=['setup', 'teardown'])
-                ),
-                THEME['error']
-            ))
-
-        if self.count('xfailed') > 0:
-            self.write_line(colored(
-                "   % 5d xfailed" % self.count('xfailed'),
-                THEME['xfailed']
-            ))
-
-        if self.count('skipped', when=['call', 'setup', 'teardown']) > 0:
-            self.write_line(colored(
-                "   % 5d skipped" % (
-                    self.count('skipped', when=['call', 'setup', 'teardown'])
-                ),
-                THEME['skipped']
-            ))
-
-        if self.count('rerun') > 0:
-            self.write_line(colored(
-                "   % 5d rerun" % self.count('rerun'),
-                THEME['rerun']
-            ))
-
-        if self.count('deselected') > 0:
-            self.write_line(colored(
-                "   % 5d deselected" % self.count('deselected'),
-                THEME['warning']
-            ))
+        if self.count("failed", when=("setup", "teardown")) > 0:
+            self.write_line(
+                colored(
+                    "   % 5d error"
+                    % (self.count("failed", when=("setup", "teardown"))),
+                    THEME.error,
+                )
+            )
+
+        if self.count("xfailed") > 0:
+            self.write_line(
+                colored("   % 5d xfailed" % self.count("xfailed"), THEME.xfailed)
+            )
+
+        if self.count("skipped", when=("call", "setup", "teardown")) > 0:
+            self.write_line(
+                colored(
+                    "   % 5d skipped"
+                    % (self.count("skipped", when=("call", "setup", "teardown"))),
+                    THEME.skipped,
+                )
+            )
+
+        if self.count("rerun") > 0:
+            self.write_line(colored("   % 5d rerun" % self.count("rerun"), THEME.rerun))
+
+        if self.count("deselected") > 0:
+            self.write_line(
+                colored("   % 5d deselected" % self.count("deselected"), THEME.warning)
+            )
 
-    def _get_decoded_crashline(self, report):
+    def _get_decoded_crashline(self, report: CollectReport) -> str:
         crashline = self._getcrashline(report)
 
-        if hasattr(crashline, 'decode'):
+        if hasattr(crashline, "decode"):
             encoding = locale.getpreferredencoding()
             try:
                 crashline = crashline.decode(encoding)
             except UnicodeDecodeError:
-                encoding = 'utf-8'
-                crashline = crashline.decode(encoding, errors='replace')
+                encoding = "utf-8"
+                crashline = crashline.decode(encoding, errors="replace")
 
         return crashline
 
-    def _get_lineno_from_report(self, report):
+    def _get_lineno_from_report(self, report: CollectReport) -> int:
         # Doctest failures in pytest>3.10 are stored in
         # reprlocation_lines, a list of (ReprFileLocation, lines)
         try:
-            location, lines = report.longrepr.reprlocation_lines[0]
+            location, lines = report.longrepr.reprlocation_lines[0]  # type: ignore
             return location.lineno
         except AttributeError:
             pass
         # Doctest failure reports have lineno=None at least up to
         # pytest==3.0.7, but it is available via longrepr object.
         try:
-            return report.longrepr.reprlocation.lineno
+            return report.longrepr.reprlocation.lineno  # type: ignore
         except AttributeError:
             lineno = report.location[1]
             if lineno is not None:
                 lineno += 1
             return lineno
 
-    def summary_failures(self):
+    def summary_failures(self) -> None:
         # Prevent failure summary from being shown since we already
         # show the failure instantly after failure has occurred.
         pass
 
-    def summary_errors(self):
+    def summary_errors(self) -> None:
         # Prevent error summary from being shown since we already
         # show the error instantly after error has occurred.
         pass
 
-    def print_failure(self, report):
+    def print_failure(self, report: Union[CollectReport, TestReport]) -> None:
         # https://github.com/Frozenball/pytest-sugar/issues/34
-        if hasattr(report, 'wasxfail'):
+        if hasattr(report, "wasxfail"):
             return
 
         if self.config.option.tbstyle != "no":
             if self.config.option.tbstyle == "line":
                 line = self._getcrashline(report)
                 self.write_line(line)
             else:
@@ -632,16 +648,11 @@
                 when = getattr(report, "when", "collect")
                 if when == "collect":
                     msg = "ERROR collecting " + msg
                 elif when == "setup":
                     msg = "ERROR at setup of " + msg
                 elif when == "teardown":
                     msg = "ERROR at teardown of " + msg
-                self.write_line('')
+                self.write_line("")
                 self.write_sep("―", msg)
                 self._outrep_summary(report)
         self.reset_tracked_lines()
-
-
-# On older version of Pytest, allow default progress
-if parse(pytest.__version__) <= parse('3.4'):  # pragma: no cover
-    del SugarTerminalReporter.pytest_runtest_logfinish
```

### Comparing `pytest-sugar-0.9.6/setup.py` & `pytest-sugar-0.9.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,70 @@
-from setuptools import setup
 import codecs
 
+from setuptools import setup
+
 
 # Copied from (and hacked):
 # https://github.com/pypa/virtualenv/blob/develop/setup.py#L42
 def get_version(filename):
     import os
     import re
 
     here = os.path.dirname(os.path.abspath(__file__))
-    f = codecs.open(os.path.join(here, filename), encoding='utf-8')
+    f = codecs.open(os.path.join(here, filename), encoding="utf-8")
     version_file = f.read()
     f.close()
-    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]",
-                              version_file, re.M)
+    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
     if version_match:
         return version_match.group(1)
     raise RuntimeError("Unable to find version string.")
 
 
 setup(
-    name='pytest-sugar',
+    name="pytest-sugar",
     description=(
-        'pytest-sugar is a plugin for pytest that changes the default'
-        ' look and feel of pytest (e.g. progressbar, show tests that'
-        ' fail instantly).'
+        "pytest-sugar is a plugin for pytest that changes the default"
+        " look and feel of pytest (e.g. progressbar, show tests that"
+        " fail instantly)."
     ),
-    long_description=codecs.open("README.md", encoding='utf-8').read(),
-    long_description_content_type='text/markdown',
-    version=get_version('pytest_sugar.py'),
-    url='https://pivotfinland.com/pytest-sugar/',
+    long_description=codecs.open("README.md", encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
+    version=get_version("pytest_sugar.py"),
+    url="https://pivotfinland.com/pytest-sugar/",
     project_urls={
-        'Source': 'https://github.com/Teemu/pytest-sugar/',
-        'Tracker': 'https://github.com/Teemu/pytest-sugar/issues',
+        "Source": "https://github.com/Teemu/pytest-sugar/",
+        "Tracker": "https://github.com/Teemu/pytest-sugar/issues",
     },
-    license='BSD',
-    author='Teemu, Janne Vanhala and others',
-    author_email='orkkiolento@gmail.com, janne.vanhala@gmail.com',
-    py_modules=['pytest_sugar'],
-    entry_points={'pytest11': ['sugar = pytest_sugar']},
+    license="BSD",
+    author="Teemu, Janne Vanhala and others",
+    author_email="orkkiolento@gmail.com, janne.vanhala@gmail.com",
+    py_modules=["pytest_sugar"],
+    entry_points={"pytest11": ["sugar = pytest_sugar"]},
     zip_safe=False,
     include_package_data=True,
-    platforms='any',
-    install_requires=['pytest>=2.9', 'termcolor>=1.1.0', 'packaging>=14.1'],
+    platforms="any",
+    install_requires=["pytest>=6.2.0", "termcolor>=2.1.0", "packaging>=21.3"],
+    extras_require={
+        "dev": [
+            "black",
+            "flake8",
+            "pre-commit",
+        ]
+    },
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: POSIX',
-        'Operating System :: Microsoft :: Windows',
-        'Operating System :: MacOS :: MacOS X',
-        'Topic :: Software Development :: Testing',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Utilities',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: Implementation :: PyPy',
-    ]
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: POSIX",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: MacOS :: MacOS X",
+        "Topic :: Software Development :: Testing",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Utilities",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: Implementation :: PyPy",
+    ],
 )
```

### Comparing `pytest-sugar-0.9.6/test_sugar.py` & `pytest-sugar-0.9.7/test_sugar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,84 @@
-# -*- coding: utf-8 -*-
-import pytest
 import re
+
+import pytest
+
 from pytest_sugar import strip_colors
 
 pytest_plugins = "pytester"
 
 
 def get_counts(stdout):
     output = strip_colors(stdout)
 
     def _get(x):
-        m = re.search(r'\d %s' % x, output)
+        m = re.search(r"\d %s" % x, output)
         if m:
             return m.group()[0]
-        else:
-            return 'n/a'
+        return "n/a"
 
     return {
         x: _get(x)
         for x in (
-            'passed',
-            'xpassed',
-            'failed',
-            'xfailed',
-            'deselected',
-            'error',
-            'rerun',
-            'skipped'
+            "passed",
+            "xpassed",
+            "failed",
+            "xfailed",
+            "deselected",
+            "error",
+            "rerun",
+            "skipped",
         )
     }
 
 
 def assert_count(testdir, *args):
     """Assert that n passed, n failed, ... matches"""
-    without_plugin = testdir.runpytest('-p', 'no:sugar', *args).stdout.str()
-    with_plugin = testdir.runpytest('--force-sugar', *args).stdout.str()
+    without_plugin = testdir.runpytest("-p", "no:sugar", *args).stdout.str()
+    with_plugin = testdir.runpytest("--force-sugar", *args).stdout.str()
 
     count_without = get_counts(without_plugin)
     count_with = get_counts(with_plugin)
 
     assert count_without == count_with, (
         "When running test with and without plugin, "
         "the resulting output differs.\n\n"
         "Without plugin: %s\n"
-        "With plugin: %s\n" % (
-            ", ".join('%s %s' % (v, k) for k, v in count_without.items()),
-            ", ".join('%s %s' % (v, k) for k, v in count_with.items()),
+        "With plugin: %s\n"
+        % (
+            ", ".join("{} {}".format(v, k) for k, v in count_without.items()),
+            ", ".join("{} {}".format(v, k) for k, v in count_with.items()),
         )
     )
 
 
-class TestTerminalReporter(object):
+class TestTerminalReporter:
     def test_new_summary(self, testdir):
         testdir.makepyfile(
             """
             import pytest
 
             def test_sample():
                 assert False
             """
         )
-        output = testdir.runpytest(
-            '--force-sugar'
-        ).stdout.str()
-        assert 'test_new_summary.py:3 test_sample' in strip_colors(output)
+        output = testdir.runpytest("--force-sugar").stdout.str()
+        assert "test_new_summary.py:3 test_sample" in strip_colors(output)
 
     def test_old_summary(self, testdir):
         testdir.makepyfile(
             """
             import pytest
 
             def test_sample():
                 assert False
             """
         )
-        output = testdir.runpytest(
-            '--force-sugar', '--old-summary'
-        ).stdout.str()
-        assert 'test_old_summary.py:4: assert False' in strip_colors(output)
+        output = testdir.runpytest("--force-sugar", "--old-summary").stdout.str()
+        assert "test_old_summary.py:4: assert False" in strip_colors(output)
 
     def test_xfail_true(self, testdir):
         testdir.makepyfile(
             """
             import pytest
 
             @pytest.mark.xfail
@@ -112,15 +109,15 @@
         )
         testdir.makepyfile(
             """
             def test():
                 pass
             """
         )
-        result = testdir.runpytest('--force-sugar')
+        result = testdir.runpytest("--force-sugar")
         assert result.ret == 0, result.stderr.str()
 
     def test_xfail_strict_true(self, testdir):
         testdir.makepyfile(
             """
             import pytest
 
@@ -164,15 +161,15 @@
             def test_sample():
                 assert False
             """
         )
         assert_count(testdir)
 
     def test_flaky_test(self, testdir):
-        pytest.importorskip('pytest_rerunfailures')
+        pytest.importorskip("pytest_rerunfailures")
         testdir.makepyfile(
             """
             import pytest
 
             COUNT = 0
 
             @pytest.mark.flaky(reruns=10)
@@ -190,20 +187,22 @@
             import pytest
 
             @pytest.mark.xfail(strict=True)
             def test_xpass():
                 assert True
             """
         )
-        result = testdir.runpytest('--force-sugar')
-        result.stdout.fnmatch_lines([
-            '*test_xpass*',
-            '*XPASS(strict)*',
-            '*1 failed*',
-        ])
+        result = testdir.runpytest("--force-sugar")
+        result.stdout.fnmatch_lines(
+            [
+                "*test_xpass*",
+                "*XPASS(strict)*",
+                "*1 failed*",
+            ]
+        )
 
     def test_teardown_errors(self, testdir):
         testdir.makepyfile(
             """
             import pytest
             @pytest.yield_fixture
             def fixt():
@@ -212,20 +211,18 @@
 
             def test_foo(fixt):
                 pass
             """
         )
         assert_count(testdir)
 
-        result = testdir.runpytest('--force-sugar')
-        result.stdout.fnmatch_lines([
-            '*ERROR at teardown of test_foo*',
-            '*1 passed*',
-            '*1 error*'
-        ])
+        result = testdir.runpytest("--force-sugar")
+        result.stdout.fnmatch_lines(
+            ["*ERROR at teardown of test_foo*", "*1 passed*", "*1 error*"]
+        )
 
     def test_skipping_tests(self, testdir):
         testdir.makepyfile(
             """
             import pytest
             @pytest.mark.skipif(True, reason='This must be skipped.')
             def test_skip_this_if():
@@ -264,53 +261,59 @@
             def test_one():
                 print('test_one_passed')
 
             def test_ignored():
                 assert 0
             """
         )
-        result = testdir.runpytest('-s')
-        result.stdout.fnmatch_lines([
-            '*test_one_passed*',
-            '*100%*',
-        ])
+        result = testdir.runpytest("-s")
+        result.stdout.fnmatch_lines(
+            [
+                "*test_one_passed*",
+                "*100%*",
+            ]
+        )
         assert result.ret == 0
 
     def test_fail(self, testdir):
         testdir.makepyfile(
             """
             import pytest
             def test_func():
                 assert 0
             """
         )
-        result = testdir.runpytest('--force-sugar')
-        result.stdout.fnmatch_lines([
-            "* test_func *",
-            "    def test_func():",
-            ">       assert 0",
-            "E       assert 0",
-        ])
+        result = testdir.runpytest("--force-sugar")
+        result.stdout.fnmatch_lines(
+            [
+                "* test_func *",
+                "    def test_func():",
+                ">       assert 0",
+                "E       assert 0",
+            ]
+        )
 
     def test_fail_unicode_crashline(self, testdir):
         testdir.makepyfile(
             """
             # -*- coding: utf-8 -*-
             import pytest
             def test_func():
                 assert b'hello' == b'Bj\\xc3\\xb6rk Gu\\xc3\\xb0mundsd'
             """
         )
-        result = testdir.runpytest('--force-sugar')
-        result.stdout.fnmatch_lines([
-            "* test_func *",
-            "    def test_func():",
-            ">       assert * == *",
-            "E       AssertionError: assert * == *",
-        ])
+        result = testdir.runpytest("--force-sugar")
+        result.stdout.fnmatch_lines(
+            [
+                "* test_func *",
+                "    def test_func():",
+                ">       assert * == *",
+                "E       AssertionError: assert * == *",
+            ]
+        )
 
     def test_fail_in_fixture_and_test(self, testdir):
         testdir.makepyfile(
             """
             import pytest
             def test_func():
                 assert False
@@ -323,39 +326,41 @@
                 return 3/0
 
             def test_lol(failure):
                 assert True
             """
         )
         assert_count(testdir)
-        output = strip_colors(testdir.runpytest('--force-sugar').stdout.str())
-        assert output.count('         -') == 2
+        output = strip_colors(testdir.runpytest("--force-sugar").stdout.str())
+        assert output.count("         -") == 2
 
     def test_fail_fail(self, testdir):
         testdir.makepyfile(
             """
             import pytest
             def test_func():
                 assert 0
             def test_func2():
                 assert 0
             """
         )
         assert_count(testdir)
-        result = testdir.runpytest('--force-sugar')
-        result.stdout.fnmatch_lines([
-            "* test_func *",
-            "    def test_func():",
-            ">       assert 0",
-            "E       assert 0",
-            "* test_func2 *",
-            "    def test_func2():",
-            ">       assert 0",
-            "E       assert 0",
-        ])
+        result = testdir.runpytest("--force-sugar")
+        result.stdout.fnmatch_lines(
+            [
+                "* test_func *",
+                "    def test_func():",
+                ">       assert 0",
+                "E       assert 0",
+                "* test_func2 *",
+                "    def test_func2():",
+                ">       assert 0",
+                "E       assert 0",
+            ]
+        )
 
     def test_error_in_setup_then_pass(self, testdir):
         testdir.makepyfile(
             """
             def setup_function(function):
                 print ("setup func")
                 if function is test_nada:
@@ -363,30 +368,32 @@
             def test_nada():
                 pass
             def test_zip():
                 pass
             """
         )
         assert_count(testdir)
-        result = testdir.runpytest('--force-sugar')
+        result = testdir.runpytest("--force-sugar")
 
-        result.stdout.fnmatch_lines([
-            "*ERROR at setup of test_nada*",
-            "",
-            "function = <function test_nada at *",
-            "",
-            "*setup_function(function):*",
-            "*setup func*",
-            "*if function is test_nada:*",
-            "*assert 0*",
-            "test_error_in_setup_then_pass.py:4: AssertionError",
-            "*Captured stdout setup*",
-            "*setup func*",
-            "*1 passed*",
-        ])
+        result.stdout.fnmatch_lines(
+            [
+                "*ERROR at setup of test_nada*",
+                "",
+                "function = <function test_nada at *",
+                "",
+                "*setup_function(function):*",
+                "*setup func*",
+                "*if function is test_nada:*",
+                "*assert 0*",
+                "test_error_in_setup_then_pass.py:4: AssertionError",
+                "*Captured stdout setup*",
+                "*setup func*",
+                "*1 passed*",
+            ]
+        )
         assert result.ret != 0
 
     def test_error_in_teardown_then_pass(self, testdir):
         testdir.makepyfile(
             """
             def teardown_function(function):
                 print ("teardown func")
@@ -395,43 +402,47 @@
             def test_nada():
                 pass
             def test_zip():
                 pass
             """
         )
         assert_count(testdir)
-        result = testdir.runpytest('--force-sugar')
+        result = testdir.runpytest("--force-sugar")
 
-        result.stdout.fnmatch_lines([
-            "*ERROR at teardown of test_nada*",
-            "",
-            "function = <function test_nada at*",
-            "",
-            "*def teardown_function(function):*",
-            "*teardown func*",
-            "*if function is test_nada*",
-            ">*assert 0*",
-            "E*assert 0*",
-            "test_error_in_teardown_then_pass.py:4: AssertionError",
-            "*Captured stdout teardown*",
-            "teardown func",
-            "*2 passed*",
-        ])
+        result.stdout.fnmatch_lines(
+            [
+                "*ERROR at teardown of test_nada*",
+                "",
+                "function = <function test_nada at*",
+                "",
+                "*def teardown_function(function):*",
+                "*teardown func*",
+                "*if function is test_nada*",
+                ">*assert 0*",
+                "E*assert 0*",
+                "test_error_in_teardown_then_pass.py:4: AssertionError",
+                "*Captured stdout teardown*",
+                "teardown func",
+                "*2 passed*",
+            ]
+        )
         assert result.ret != 0
 
     def test_collect_error(self, testdir):
         testdir.makepyfile("""raise ValueError(0)""")
         assert_count(testdir)
-        result = testdir.runpytest('--force-sugar')
-        result.stdout.fnmatch_lines([
-            "*ERROR collecting test_collect_error.py*",
-            "test_collect_error.py:1: in <module>",
-            "    raise ValueError(0)",
-            "E   ValueError: 0",
-        ])
+        result = testdir.runpytest("--force-sugar")
+        result.stdout.fnmatch_lines(
+            [
+                "*ERROR collecting test_collect_error.py*",
+                "test_collect_error.py:1: in <module>",
+                "    raise ValueError(0)",
+                "E   ValueError: 0",
+            ]
+        )
 
     def test_verbose(self, testdir):
         testdir.makepyfile(
             """
             import pytest
 
             def test_true():
@@ -452,29 +463,25 @@
                 assert True
 
             @pytest.mark.xfail
             def test_xfail():
                 assert True
             """
         )
-        assert_count(testdir, '--verbose')
+        assert_count(testdir, "--verbose")
 
     def test_verbose_has_double_colon(self, testdir):
         testdir.makepyfile(
             """
             def test_true():
                 assert True
             """
         )
-        output = testdir.runpytest(
-            '--force-sugar', '--verbose'
-        ).stdout.str()
-        assert 'test_verbose_has_double_colon.py::test_true' in strip_colors(
-            output
-        )
+        output = testdir.runpytest("--force-sugar", "--verbose").stdout.str()
+        assert "test_verbose_has_double_colon.py::test_true" in strip_colors(output)
 
     # def test_verbose_has_double_colon_with_class(self, testdir):
     #     testdir.makepyfile(
     #         """
     #         class TestTrue:
 
     #             def test_true(self):
@@ -511,63 +518,65 @@
             """
             def test_nada():
                 pass
             def test_zip():
                 pass
             """
         )
-        result = testdir.runpytest('--force-sugar', '-n2')
+        result = testdir.runpytest("--force-sugar", "-n2")
 
         assert result.ret == 0, result.stderr.str()
 
     def test_xdist_verbose(self, testdir):
         pytest.importorskip("xdist")
         testdir.makepyfile(
             """
             def test_nada():
                 pass
             def test_zip():
                 pass
             """
         )
-        result = testdir.runpytest('--force-sugar', '-n2', '-v')
+        result = testdir.runpytest("--force-sugar", "-n2", "-v")
 
         assert result.ret == 0, result.stderr.str()
 
     def test_doctest(self, testdir):
-        """ Test doctest-modules """
+        """Test doctest-modules"""
 
         testdir.makepyfile(
             """
-            class ToTest(object):
+            class ToTest():
                 @property
                 def doctest(self):
                     \"\"\"
                         >>> Invalid doctest
                     \"\"\"
             """
         )
-        result = testdir.runpytest('--force-sugar', '--doctest-modules')
+        result = testdir.runpytest("--force-sugar", "--doctest-modules")
 
         assert result.ret == 1, result.stderr.str()
 
     def test_doctest_lineno(self, testdir):
-        """ Test location reported for doctest-modules """
+        """Test location reported for doctest-modules"""
 
         testdir.makepyfile(
             """
             def foobar():
                 '''
                 >>> foobar()
                 '''
                 raise NotImplementedError
             """
         )
-        result = testdir.runpytest('--force-sugar', '--doctest-modules')
+        result = testdir.runpytest("--force-sugar", "--doctest-modules")
 
         assert result.ret == 1, result.stderr.str()
-        result.stdout.fnmatch_lines([
-            'UNEXPECTED EXCEPTION: NotImplementedError()',
-            '*test_doctest_lineno.py:3: UnexpectedException',
-            'Results*:',
-            '*-*test_doctest_lineno.py*:3*',
-        ])
+        result.stdout.fnmatch_lines(
+            [
+                "UNEXPECTED EXCEPTION: NotImplementedError()",
+                "*test_doctest_lineno.py:3: UnexpectedException",
+                "Results*:",
+                "*-*test_doctest_lineno.py*:3*",
+            ]
+        )
```

