# Comparing `tmp/failprint-0.8.0.tar.gz` & `tmp/failprint-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "failprint-0.8.0.tar", last modified: Sat Jul 31 18:18:28 2021, max compression
+gzip compressed data, was "failprint-0.9.0.tar", last modified: Fri Feb 10 13:35:51 2023, max compression
```

## Comparing `failprint-0.8.0.tar` & `failprint-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,20 @@
--rw-r--r--   0 pawamoy   (1000) users      (985)      754 2021-05-22 15:53:22.127240 failprint-0.8.0/LICENSE
--rw-r--r--   0 pawamoy   (1000) users      (985)     4714 2021-06-06 17:35:11.089927 failprint-0.8.0/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)     2417 2021-07-31 10:36:47.600135 failprint-0.8.0/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) users      (985)      257 2021-06-06 17:35:11.089927 failprint-0.8.0/src/failprint/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      344 2021-06-18 19:27:34.167378 failprint-0.8.0/src/failprint/__main__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      990 2020-10-10 22:45:09.303442 failprint-0.8.0/src/failprint/capture.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     6020 2021-07-31 18:18:24.521907 failprint-0.8.0/src/failprint/cli.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     4191 2020-10-11 18:41:07.718091 failprint-0.8.0/src/failprint/formats.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2864 2021-07-31 10:36:47.600135 failprint-0.8.0/src/failprint/process.py
--rw-r--r--   0 pawamoy   (1000) users      (985)        0 2021-05-22 15:56:28.697574 failprint-0.8.0/src/failprint/py.typed
--rw-r--r--   0 pawamoy   (1000) users      (985)     8227 2021-07-31 11:58:40.385609 failprint-0.8.0/src/failprint/runners.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      302 2021-01-17 16:51:33.020552 failprint-0.8.0/src/failprint/types.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       37 2021-07-29 19:04:38.340509 failprint-0.8.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0 pawamoy   (1000) users      (985)      194 2021-07-29 19:04:38.340509 failprint-0.8.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 pawamoy   (1000) users      (985)      295 2021-07-29 19:04:38.340509 failprint-0.8.0/tests/.pytest_cache/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)       29 2021-07-29 20:46:31.551335 failprint-0.8.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 pawamoy   (1000) users      (985)      110 2021-07-31 18:08:34.363674 failprint-0.8.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 pawamoy   (1000) users      (985)        2 2021-07-31 18:08:34.420340 failprint-0.8.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 pawamoy   (1000) users      (985)        9 2021-07-31 18:08:22.673844 failprint-0.8.0/tests/.pytest_cache/v/randomly_seed
--rw-r--r--   0 pawamoy   (1000) users      (985)      162 2020-04-30 11:03:32.049542 failprint-0.8.0/tests/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       47 2020-09-04 16:33:33.639978 failprint-0.8.0/tests/conftest.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      817 2020-10-11 17:22:45.809295 failprint-0.8.0/tests/test_capture.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      895 2021-06-06 17:35:11.089927 failprint-0.8.0/tests/test_cli.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     3358 2020-10-10 23:14:46.307266 failprint-0.8.0/tests/test_formats.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2159 2021-07-31 10:36:47.600135 failprint-0.8.0/tests/test_process.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     9094 2021-07-31 10:36:47.600135 failprint-0.8.0/tests/test_runners.py
--rw-------   0 pawamoy   (1000) users      (985)     6861 2021-07-31 18:18:29.008510 failprint-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-02-10 13:22:27.696958 failprint-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4818 2023-02-10 13:22:27.850288 failprint-0.9.0/README.md
+-rw-r--r--   0        0        0     3230 2023-02-10 13:22:27.850288 failprint-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-02-10 13:22:27.850288 failprint-0.9.0/src/failprint/__init__.py
+-rw-r--r--   0        0        0      344 2023-02-10 13:22:27.540294 failprint-0.9.0/src/failprint/__main__.py
+-rw-r--r--   0        0        0     2926 2023-02-10 13:10:24.550141 failprint-0.9.0/src/failprint/capture.py
+-rw-r--r--   0        0        0     6197 2023-02-10 13:29:32.616214 failprint-0.9.0/src/failprint/cli.py
+-rw-r--r--   0        0        0     4880 2023-02-10 13:10:24.560140 failprint-0.9.0/src/failprint/formats.py
+-rw-r--r--   0        0        0     2875 2023-02-10 13:10:24.563474 failprint-0.9.0/src/failprint/process.py
+-rw-r--r--   0        0        0        0 2023-02-10 13:22:27.533627 failprint-0.9.0/src/failprint/py.typed
+-rw-r--r--   0        0        0     7449 2023-02-10 13:10:24.563474 failprint-0.9.0/src/failprint/runners.py
+-rw-r--r--   0        0        0      338 2023-02-10 13:10:24.566807 failprint-0.9.0/src/failprint/types.py
+-rw-r--r--   0        0        0      162 2023-02-10 13:22:27.533627 failprint-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-02-10 13:22:27.530294 failprint-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      817 2020-10-11 17:22:45.809295 failprint-0.9.0/tests/test_capture.py
+-rw-r--r--   0        0        0      891 2023-02-10 13:22:27.850288 failprint-0.9.0/tests/test_cli.py
+-rw-r--r--   0        0        0     3358 2020-10-10 23:14:46.307266 failprint-0.9.0/tests/test_formats.py
+-rw-r--r--   0        0        0     2159 2021-07-31 10:36:47.600135 failprint-0.9.0/tests/test_process.py
+-rw-r--r--   0        0        0     9094 2021-07-31 10:36:47.600135 failprint-0.9.0/tests/test_runners.py
+-rw-r--r--   0        0        0     6290 1970-01-01 00:00:00.000000 failprint-0.9.0/PKG-INFO
```

### Comparing `failprint-0.8.0/LICENSE` & `failprint-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `failprint-0.8.0/README.md` & `failprint-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # failprint
 
 [![ci](https://github.com/pawamoy/failprint/workflows/ci/badge.svg)](https://github.com/pawamoy/failprint/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/failprint/)
 [![pypi version](https://img.shields.io/pypi/v/failprint.svg)](https://pypi.org/project/failprint/)
+[![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/pawamoy/failprint)
 [![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/failprint/community)
 
 Run a command, print its output only if it fails.
 
 Tired of searching the `quiet` options of your programs
 to lighten up the output of your `make check` or `make lint` commands?
 
@@ -52,22 +53,21 @@
 ```
 </details>
 
 ## Installation
 
 With `pip`:
 ```bash
-python3.6 -m pip install failprint
+pip install failprint
 ```
 
 With [`pipx`](https://github.com/pipxproject/pipx):
 ```bash
-python3.6 -m pip install --user pipx
-
-pipx install --python python3.6 failprint
+python3.7 -m pip install --user pipx
+pipx install failprint
 ```
 
 ## Usage
 
 ```console
 % poetry run failprint -h
 usage: failprint [-h] [-c {stdout,stderr,both,none}] [-f {pretty,tap}] [-y | -Y] [-p | -P] [-q | -Q] [-s | -S] [-z | -Z] [-n NUMBER]
@@ -119,8 +119,8 @@
     fmt=None,       # pretty, tap, or custom="MY_CUSTOM_FORMAT"
     pty=False,      # use a PTY
     progress=True,  # print the "progress" template before running the command
     nofail=False,   # always return zero
     quiet=False,    # don't print output when the command fails
     silent=False,   # don't print anything
 )
-```
+```
```

#### html2text {}

```diff
@@ -1,55 +1,56 @@
 # failprint [![ci](https://github.com/pawamoy/failprint/workflows/ci/
 badge.svg)](https://github.com/pawamoy/failprint/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-
 blue.svg?style=flat)](https://pawamoy.github.io/failprint/) [![pypi version]
 (https://img.shields.io/pypi/v/failprint.svg)](https://pypi.org/project/
-failprint/) [![gitter](https://badges.gitter.im/join%20chat.svg)](https://
-gitter.im/failprint/community) Run a command, print its output only if it
-fails. Tired of searching the `quiet` options of your programs to lighten up
-the output of your `make check` or `make lint` commands? Tired of finding out
-that standard output and error are mixed up in some of them? Simply run your
-command through `failprint`. If it succeeds, nothing is printed. If it fails,
-standard error is printed. Plus other configuration goodies :wink: ## Example
-You don't want to see output when the command succeeds. ![demo](demo.svg) The
-task runner [`duty`](https://github.com/pawamoy/duty) uses `failprint`,
-allowing you to define tasks in Python and run them with minimalist and
-beautiful output: ![demo_duty](demo_duty.svg) ## Requirements failprint
-requires Python 3.6 or above.  To install Python 3.6, I recommend using pyenv.
-```bash # install pyenv git clone https://github.com/pyenv/pyenv ~/.pyenv #
-setup pyenv (you should also put these three lines in .bashrc or similar)
-export PATH="${HOME}/.pyenv/bin:${PATH}" export PYENV_ROOT="${HOME}/.pyenv"
-eval "$(pyenv init -)" # install Python 3.6 pyenv install 3.6.12 # make it
-available globally pyenv global system 3.6.12 ```  ## Installation With `pip`:
-```bash python3.6 -m pip install failprint ``` With [`pipx`](https://
-github.com/pipxproject/pipx): ```bash python3.6 -m pip install --user pipx pipx
-install --python python3.6 failprint ``` ## Usage ```console % poetry run
-failprint -h usage: failprint [-h] [-c {stdout,stderr,both,none}] [-f
-{pretty,tap}] [-y | -Y] [-p | -P] [-q | -Q] [-s | -S] [-z | -Z] [-n NUMBER] [-
-t TITLE] COMMAND [COMMAND ...] positional arguments: COMMAND optional
-arguments: -h, --help show this help message and exit -c
-{stdout,stderr,both,none}, --capture {stdout,stderr,both,none} Which output to
-capture. Colors are supported with 'both' only, unless the command has a 'force
-color' option. -f {pretty,tap}, --format {pretty,tap} Output format. Pass your
-own Jinja2 template as a string with '-f custom=TEMPLATE'. Available variables:
-command, title (command or title passed with -t), code (exit status), success
-(boolean), failure (boolean), number (command number passed with -n), output
-(command output), nofail (boolean), quiet (boolean), silent (boolean).
-Available filters: indent (textwrap.indent). -y, --pty Enable the use of a
-pseudo-terminal. PTY doesn't allow programs to use standard input. -Y, --no-pty
-Disable the use of a pseudo-terminal. PTY doesn't allow programs to use
-standard input. -p, --progress Print progress while running a command. -P, --
-no-progress Don't print progress while running a command. -q, --quiet Don't
-print the command output, even if it failed. -Q, --no-quiet Print the command
-output when it fails. -s, --silent Don't print anything. -S, --no-silent Print
-output as usual. -z, --zero, --nofail Don't fail. Always return a success (0)
-exit code. -Z, --no-zero, --strict Return the original exit code. -n NUMBER, --
-number NUMBER Command number. Useful for the 'tap' format. -t TITLE, --title
-TITLE Command title. Default is the command itself. ``` ```python from
-failprint.runners import run cmd = "echo hello" exit_code = run( cmd, # str,
-list of str, or Python callable args=None, # args for callable kwargs=None, #
-kwargs for callable number=1, # command number, useful for tap format
-capture=None, # stdout, stderr, both, none, True or False title=None, # command
-title fmt=None, # pretty, tap, or custom="MY_CUSTOM_FORMAT" pty=False, # use a
-PTY progress=True, # print the "progress" template before running the command
-nofail=False, # always return zero quiet=False, # don't print output when the
-command fails silent=False, # don't print anything ) ```
+failprint/) [![gitpod](https://img.shields.io/badge/gitpod-workspace-
+blue.svg?style=flat)](https://gitpod.io/#https://github.com/pawamoy/failprint)
+[![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/
+failprint/community) Run a command, print its output only if it fails. Tired of
+searching the `quiet` options of your programs to lighten up the output of your
+`make check` or `make lint` commands? Tired of finding out that standard output
+and error are mixed up in some of them? Simply run your command through
+`failprint`. If it succeeds, nothing is printed. If it fails, standard error is
+printed. Plus other configuration goodies :wink: ## Example You don't want to
+see output when the command succeeds. ![demo](demo.svg) The task runner
+[`duty`](https://github.com/pawamoy/duty) uses `failprint`, allowing you to
+define tasks in Python and run them with minimalist and beautiful output: !
+[demo_duty](demo_duty.svg) ## Requirements failprint requires Python 3.6 or
+above.  To install Python 3.6, I recommend using pyenv. ```bash # install pyenv
+git clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should
+also put these three lines in .bashrc or similar) export PATH="${HOME}/.pyenv/
+bin:${PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" #
+install Python 3.6 pyenv install 3.6.12 # make it available globally pyenv
+global system 3.6.12 ```  ## Installation With `pip`: ```bash pip install
+failprint ``` With [`pipx`](https://github.com/pipxproject/pipx): ```bash
+python3.7 -m pip install --user pipx pipx install failprint ``` ## Usage
+```console % poetry run failprint -h usage: failprint [-h] [-c
+{stdout,stderr,both,none}] [-f {pretty,tap}] [-y | -Y] [-p | -P] [-q | -Q] [-
+s | -S] [-z | -Z] [-n NUMBER] [-t TITLE] COMMAND [COMMAND ...] positional
+arguments: COMMAND optional arguments: -h, --help show this help message and
+exit -c {stdout,stderr,both,none}, --capture {stdout,stderr,both,none} Which
+output to capture. Colors are supported with 'both' only, unless the command
+has a 'force color' option. -f {pretty,tap}, --format {pretty,tap} Output
+format. Pass your own Jinja2 template as a string with '-f custom=TEMPLATE'.
+Available variables: command, title (command or title passed with -t), code
+(exit status), success (boolean), failure (boolean), number (command number
+passed with -n), output (command output), nofail (boolean), quiet (boolean),
+silent (boolean). Available filters: indent (textwrap.indent). -y, --pty Enable
+the use of a pseudo-terminal. PTY doesn't allow programs to use standard input.
+-Y, --no-pty Disable the use of a pseudo-terminal. PTY doesn't allow programs
+to use standard input. -p, --progress Print progress while running a command. -
+P, --no-progress Don't print progress while running a command. -q, --quiet
+Don't print the command output, even if it failed. -Q, --no-quiet Print the
+command output when it fails. -s, --silent Don't print anything. -S, --no-
+silent Print output as usual. -z, --zero, --nofail Don't fail. Always return a
+success (0) exit code. -Z, --no-zero, --strict Return the original exit code. -
+n NUMBER, --number NUMBER Command number. Useful for the 'tap' format. -
+t TITLE, --title TITLE Command title. Default is the command itself. ```
+```python from failprint.runners import run cmd = "echo hello" exit_code = run
+( cmd, # str, list of str, or Python callable args=None, # args for callable
+kwargs=None, # kwargs for callable number=1, # command number, useful for tap
+format capture=None, # stdout, stderr, both, none, True or False title=None, #
+command title fmt=None, # pretty, tap, or custom="MY_CUSTOM_FORMAT" pty=False,
+# use a PTY progress=True, # print the "progress" template before running the
+command nofail=False, # always return zero quiet=False, # don't print output
+when the command fails silent=False, # don't print anything ) ```
```

### Comparing `failprint-0.8.0/src/failprint/cli.py` & `failprint-0.9.0/src/failprint/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 #   `__main__.py` as a script. That means there won't be any
 #   `failprint.__main__` in `sys.modules`.
 # - When you import `__main__` it will get executed again (as a module) because
 #   there's no `failprint.__main__` in `sys.modules`.
 
 """Module that contains the command line application."""
 
+from __future__ import annotations
+
 import argparse
-from typing import List, Optional, Sequence
+from typing import Any, Sequence
 
 from failprint.capture import Capture
 from failprint.formats import accept_custom_format, formats
 from failprint.runners import run
 
 
 class ArgParser(argparse.ArgumentParser):
@@ -24,15 +26,15 @@
 
     def add_bool_argument(
         self,
         truthy: Sequence[str],
         falsy: Sequence[str],
         truthy_help: str = "",
         falsy_help: str = "",
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         """
         Add a boolean flag/argument to the parser.
 
         Arguments:
             truthy: Values that will store true in the destination.
             falsy: Values that will store false in the destination.
@@ -44,15 +46,15 @@
         falsy_kwargs = {**kwargs, "help": falsy_help, "action": "store_false"}
 
         mxg = self.add_mutually_exclusive_group()
         mxg.add_argument(*truthy, **truthy_kwargs)  # type: ignore  # mypy is confused by arguments position
         mxg.add_argument(*falsy, **falsy_kwargs)  # type: ignore
 
 
-def add_flags(parser, set_defaults=True) -> ArgParser:
+def add_flags(parser: ArgParser, set_defaults: bool = True) -> ArgParser:
     """
     Add some boolean flags to the parser.
 
     We made this method separate and public
     for its use in [duty](https://github.com/pawamoy/duty).
 
     Arguments:
@@ -101,22 +103,24 @@
         ["-p", "--progress"],
         ["-P", "--no-progress"],
         dest="progress",
         default=True if set_defaults else None,
         truthy_help="Print progress while running a command.",
         falsy_help="Don't print progress while running a command.",
     )
+    # TODO: specific to the format
     parser.add_bool_argument(
         ["-q", "--quiet"],
         ["-Q", "--no-quiet"],
         dest="quiet",
         default=False if set_defaults else None,
         truthy_help="Don't print the command output, even if it failed.",
         falsy_help="Print the command output when it fails.",
     )
+    # TODO: specific to the format
     parser.add_bool_argument(
         ["-s", "--silent"],
         ["-S", "--no-silent"],
         dest="silent",
         default=False if set_defaults else None,
         truthy_help="Don't print anything.",
         falsy_help="Print output as usual.",
@@ -129,34 +133,34 @@
         truthy_help="Don't fail. Always return a success (0) exit code.",
         falsy_help="Return the original exit code.",
     )
     return parser
 
 
 def get_parser() -> ArgParser:
-    """
-    Return the CLI argument parser.
+    """Return the CLI argument parser.
 
     Returns:
         An argparse parser.
     """
     parser = add_flags(ArgParser(prog="failprint"))
+    # TODO: specific to the format
     parser.add_argument("-n", "--number", type=int, default=1, help="Command number. Useful for the 'tap' format.")
+    # TODO: specific to the format
     parser.add_argument("-t", "--title", help="Command title. Default is the command itself.")
     parser.add_argument("cmd", metavar="COMMAND", nargs="+")
     return parser
 
 
-def main(args: Optional[List[str]] = None) -> int:
-    """
-    Run the main program.
+def main(args: list[str] | None = None) -> int:
+    """Run the main program.
 
     This function is executed when you type `failprint` or `python -m failprint`.
 
-    Arguments:
+    Parameters:
         args: Arguments passed from the command line.
 
     Returns:
         An exit code.
     """
     parser = get_parser()
     opts = parser.parse_args(args).__dict__.items()  # noqa: WPS609
```

### Comparing `failprint-0.8.0/src/failprint/process.py` & `failprint-0.9.0/src/failprint/process.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Functions related to subprocesses."""
 
+from __future__ import annotations
+
 import contextlib
 import subprocess  # noqa: S404 (we don't mind the security implication)
-from typing import List, Optional, Tuple
 
 from failprint import WINDOWS
 from failprint.capture import Capture
 from failprint.formats import printable_command
 from failprint.types import CmdType
 
 if not WINDOWS:
     from ptyprocess import PtyProcessUnicode
 
 
 def run_subprocess(
     cmd: CmdType,
     capture: Capture = Capture.BOTH,
     shell: bool = False,
-    stdin: Optional[str] = None,
-) -> Tuple[int, str]:
+    stdin: str | None = None,
+) -> tuple[int, str]:
     """
     Run a command in a subprocess.
 
     Arguments:
         cmd: The command to run.
         capture: The output to capture.
         shell: Whether to run the command in a shell.
@@ -61,28 +62,32 @@
         output = process.stderr
     else:
         output = process.stdout
 
     return process.returncode, output
 
 
-def run_pty_subprocess(cmd: List[str], capture: Capture = Capture.BOTH, stdin: Optional[str] = None) -> Tuple[int, str]:
+def run_pty_subprocess(
+    cmd: list[str],
+    capture: Capture = Capture.BOTH,
+    stdin: str | None = None,
+) -> tuple[int, str] | None:
     """
     Run a command in a PTY subprocess.
 
     Arguments:
         cmd: The command to run.
         capture: The output to capture.
         stdin: String to use as standard input.
 
     Returns:
         The exit code and the command output.
     """
     process = PtyProcessUnicode.spawn(cmd)
-    pty_output: List[str] = []
+    pty_output: list[str] = []
 
     if stdin is not None:
         process.setecho(False)
         process.waitnoecho()
         process.write(stdin)
         process.sendeof()
         # not sure why but sending only one eof is not always enough,
```

### Comparing `failprint-0.8.0/src/failprint/runners.py` & `failprint-0.9.0/src/failprint/runners.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,32 @@
 """Functions to run commands and capture output."""
 
+from __future__ import annotations
+
 import os
 import shutil
 import sys
 import textwrap
 import traceback
-from contextlib import contextmanager
-from io import StringIO
-from typing import Callable, Optional, Tuple, Union
+from typing import Callable, Sequence, TextIO
 
 import colorama
 from ansimarkup import ansiprint
 from jinja2 import Environment
 
 from failprint import WINDOWS
-from failprint.capture import Capture, cast_capture
+from failprint.capture import Capture, cast_capture, stdbuffer
 from failprint.formats import DEFAULT_FORMAT, accept_custom_format, formats, printable_command
 from failprint.process import run_pty_subprocess, run_subprocess
 from failprint.types import CmdFuncType, CmdType
 
 if WINDOWS:
     colorama.init()
 
 
-class StdBuffer:
-    """A simple placeholder for three memory buffers."""
-
-    def __init__(self, stdinput=None, stdout=None, stderr=None):
-        """
-        Initialize the object.
-
-        Arguments:
-            stdinput: String to use as standard input.
-            stdout: A buffer for standard output.
-            stderr: A buffer for standard error.
-        """
-        self.stdin = StringIO(stdinput) if stdinput is not None else sys.stdin
-        self.stdout = stdout or StringIO()
-        self.stderr = stderr or StringIO()
-
-
-@contextmanager
-def stdbuffer(stdinput=None):
-    """
-    Capture output in a `with` statement.
-
-    Arguments:
-        stdinput: String to use as standard input.
-
-    Yields:
-        An instance of `StdBuffer`.
-    """
-    old_stdin = sys.stdin
-    old_stdout = sys.stdout
-    old_stderr = sys.stderr
-
-    buffer = StdBuffer(stdinput)
-
-    sys.stdin = buffer.stdin
-    sys.stdout = buffer.stdout
-    sys.stderr = buffer.stderr
-
-    yield buffer
-
-    sys.stdin = old_stdin
-    sys.stdout = old_stdout
-    sys.stderr = old_stderr
-
-    buffer.stdin.close()
-    buffer.stdout.close()
-    buffer.stderr.close()
-
-
 class RunResult:
     """Placeholder for a run result."""
 
     def __init__(self, code: int, output: str) -> None:
         """
         Initialize the object.
 
@@ -85,26 +36,27 @@
         """
         self.code = code
         self.output = output
 
 
 def run(  # noqa: WPS231 (high complexity)
     cmd: CmdFuncType,
-    args=None,
-    kwargs=None,
+    args: Sequence | None = None,
+    kwargs: dict | None = None,
     number: int = 1,
-    capture: Optional[Union[str, bool, Capture]] = None,
-    title: Optional[str] = None,
-    fmt: Optional[str] = None,
+    capture: str | bool | Capture | None = None,
+    title: str | None = None,
+    fmt: str | None = None,
     pty: bool = False,
     progress: bool = True,
     nofail: bool = False,
     quiet: bool = False,
     silent: bool = False,
-    stdin: Optional[str] = None,
+    stdin: str | None = None,
+    command: str | None = None,
 ) -> RunResult:
     """
     Run a command in a subprocess or a Python function, and print its output if it fails.
 
     Arguments:
         cmd: The command to run.
         args: Arguments to pass to the callable.
@@ -115,26 +67,27 @@
         fmt: The output format.
         pty: Whether to run in a PTY.
         progress: Whether to show progress.
         nofail: Whether to always succeed.
         quiet: Whether to not print the command output.
         silent: Don't print anything.
         stdin: String to use as standard input.
+        command: The command to display.
 
     Returns:
         The command exit code, or 0 if `nofail` is True.
     """
     format_name: str = fmt or os.environ.get("FAILPRINT_FORMAT", DEFAULT_FORMAT)  # type: ignore
     format_name = accept_custom_format(format_name)
     format_obj = formats.get(format_name, formats[DEFAULT_FORMAT])
 
     env = Environment(autoescape=False)  # noqa: S701 (no HTML: no need to escape)
     env.filters["indent"] = textwrap.indent
 
-    command = printable_command(cmd, args, kwargs)
+    command = command if command is not None else printable_command(cmd, args, kwargs)
 
     if not silent and progress and format_obj.progress_template:
         progress_template = env.from_string(format_obj.progress_template)
         ansiprint(progress_template.render({"title": title, "command": command}), end="\r")
 
     capture = cast_capture(capture)
 
@@ -166,16 +119,16 @@
 
 
 def run_command(
     cmd: CmdType,
     capture: Capture = Capture.BOTH,
     ansi: bool = False,
     pty: bool = False,
-    stdin: Optional[str] = None,
-) -> Tuple[int, str]:
+    stdin: str | None = None,
+) -> tuple[int, str]:
     """
     Run a command.
 
     Arguments:
         cmd: The command to run.
         capture: The output to capture.
         ansi: Whether to accept ANSI sequences.
@@ -204,20 +157,20 @@
             cmd[0] = shutil.which(cmd[0]) or cmd[0]  # type: ignore  # we know cmd is a list
         return run_subprocess(cmd, capture, shell=shell, stdin=stdin)  # noqa: S604 (shell=True)
 
     return run_subprocess(cmd, capture, shell=shell, stdin=stdin)  # noqa: S604 (shell=True)
 
 
 def run_function(
-    func,
-    args=None,
-    kwargs=None,
+    func: Callable,
+    args: Sequence | None = None,
+    kwargs: dict | None = None,
     capture: Capture = Capture.BOTH,
-    stdin: Optional[str] = None,
-) -> Tuple[int, str]:
+    stdin: str | None = None,
+) -> tuple[int, str]:
     """
     Run a function.
 
     Arguments:
         func: The function to run.
         args: Positional arguments passed to the function.
         kwargs: Keyword arguments passed to the function.
@@ -246,29 +199,41 @@
             output = buffer.stderr.getvalue()
         else:
             output = buffer.stdout.getvalue()
 
     return code, output
 
 
-def run_function_get_code(func: Callable, stderr, args=None, kwargs=None) -> int:  # noqa: WPS212 (return statements)
+def run_function_get_code(  # noqa: WPS212,WPS231
+    func: Callable,
+    stderr: TextIO,
+    args: Sequence,
+    kwargs: dict,
+) -> int:
     """
     Run a function and return a exit code.
 
     Arguments:
         func: The function to run.
         stderr: A file descriptor to write potential tracebacks.
         args: Positional arguments passed to the function.
         kwargs: Keyword arguments passed to the function.
 
     Returns:
         An exit code.
     """
     try:
         result = func(*args, **kwargs)
+    except SystemExit as exit:
+        if exit.code is None:
+            return 0
+        if isinstance(exit.code, int):
+            return exit.code
+        stderr.write(str(exit.code))
+        return 1
     except Exception:  # noqa: W0703 (catching Exception on purpose)
         stderr.write(traceback.format_exc() + "\n")
         return 1
 
     # first check True and False
     # because int(True) == 1 and int(False) == 0
     if result is True:
```

### Comparing `failprint-0.8.0/tests/test_capture.py` & `failprint-0.9.0/tests/test_capture.py`

 * *Files identical despite different names*

### Comparing `failprint-0.8.0/tests/test_cli.py` & `failprint-0.9.0/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 def test_fail_without_arguments():
     """Fails without arguments."""
     with pytest.raises(SystemExit):
         cli.main([])
 
 
 def test_show_help(capsys):
-    """
-    Show help.
+    """Show help.
 
-    Arguments:
+    Parameters:
         capsys: Pytest fixture to capture output.
     """
     with pytest.raises(SystemExit):
         cli.main(["-h"])
     captured = capsys.readouterr()
     assert "failprint" in captured.out
```

### Comparing `failprint-0.8.0/tests/test_formats.py` & `failprint-0.9.0/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `failprint-0.8.0/tests/test_process.py` & `failprint-0.9.0/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `failprint-0.8.0/tests/test_runners.py` & `failprint-0.9.0/tests/test_runners.py`

 * *Files identical despite different names*

### Comparing `failprint-0.8.0/PKG-INFO` & `failprint-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,150 +1,160 @@
 Metadata-Version: 2.1
 Name: failprint
-Version: 0.8.0
+Version: 0.9.0
 Summary: Run a command, print its output only if it fails.
-License: UNKNOWN
+License: ISC
 Keywords: cli,failure,output,runner
 Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
-Classifier: License :: Other/Proprietary License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Project-URL: Changelog, https://pawamoy.github.io/failprint/changelog
 Project-URL: Discussions, https://github.com/pawamoy/failprint/discussions
 Project-URL: Documentation, https://pawamoy.github.io/failprint
 Project-URL: Funding, https://github.com/sponsors/pawamoy
 Project-URL: Gitter, https://gitter.im/failprint/community
 Project-URL: Homepage, https://pawamoy.github.io/failprint
 Project-URL: Issues, https://github.com/pawamoy/failprint/issues
 Project-URL: Repository, https://github.com/pawamoy/failprint
 Description-Content-Type: text/markdown
-Description: # failprint
-        
-        [![ci](https://github.com/pawamoy/failprint/workflows/ci/badge.svg)](https://github.com/pawamoy/failprint/actions?query=workflow%3Aci)
-        [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/failprint/)
-        [![pypi version](https://img.shields.io/pypi/v/failprint.svg)](https://pypi.org/project/failprint/)
-        [![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/failprint/community)
-        
-        Run a command, print its output only if it fails.
-        
-        Tired of searching the `quiet` options of your programs
-        to lighten up the output of your `make check` or `make lint` commands?
-        
-        Tired of finding out that standard output and error are mixed up in some of them?
-        
-        Simply run your command through `failprint`.
-        If it succeeds, nothing is printed.
-        If it fails, standard error is printed.
-        Plus other configuration goodies :wink:
-        
-        ## Example
-        
-        You don't want to see output when the command succeeds.
-        
-        ![demo](demo.svg)
-        
-        The task runner [`duty`](https://github.com/pawamoy/duty) uses `failprint`,
-        allowing you to define tasks in Python and run them with minimalist and beautiful output:
-        
-        ![demo_duty](demo_duty.svg)
-        
-        ## Requirements
-        
-        failprint requires Python 3.6 or above.
-        
-        <details>
-        <summary>To install Python 3.6, I recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
-        
-        ```bash
-        # install pyenv
-        git clone https://github.com/pyenv/pyenv ~/.pyenv
-        
-        # setup pyenv (you should also put these three lines in .bashrc or similar)
-        export PATH="${HOME}/.pyenv/bin:${PATH}"
-        export PYENV_ROOT="${HOME}/.pyenv"
-        eval "$(pyenv init -)"
-        
-        # install Python 3.6
-        pyenv install 3.6.12
-        
-        # make it available globally
-        pyenv global system 3.6.12
-        ```
-        </details>
-        
-        ## Installation
-        
-        With `pip`:
-        ```bash
-        python3.6 -m pip install failprint
-        ```
-        
-        With [`pipx`](https://github.com/pipxproject/pipx):
-        ```bash
-        python3.6 -m pip install --user pipx
-        
-        pipx install --python python3.6 failprint
-        ```
-        
-        ## Usage
-        
-        ```console
-        % poetry run failprint -h
-        usage: failprint [-h] [-c {stdout,stderr,both,none}] [-f {pretty,tap}] [-y | -Y] [-p | -P] [-q | -Q] [-s | -S] [-z | -Z] [-n NUMBER]
-                         [-t TITLE]
-                         COMMAND [COMMAND ...]
-        
-        positional arguments:
-          COMMAND
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -c {stdout,stderr,both,none}, --capture {stdout,stderr,both,none}
-                                Which output to capture. Colors are supported with 'both' only, unless the command has a 'force color'
-                                option.
-          -f {pretty,tap}, --format {pretty,tap}
-                                Output format. Pass your own Jinja2 template as a string with '-f custom=TEMPLATE'. Available variables:
-                                command, title (command or title passed with -t), code (exit status), success (boolean), failure (boolean),
-                                number (command number passed with -n), output (command output), nofail (boolean), quiet (boolean), silent
-                                (boolean). Available filters: indent (textwrap.indent).
-          -y, --pty             Enable the use of a pseudo-terminal. PTY doesn't allow programs to use standard input.
-          -Y, --no-pty          Disable the use of a pseudo-terminal. PTY doesn't allow programs to use standard input.
-          -p, --progress        Print progress while running a command.
-          -P, --no-progress     Don't print progress while running a command.
-          -q, --quiet           Don't print the command output, even if it failed.
-          -Q, --no-quiet        Print the command output when it fails.
-          -s, --silent          Don't print anything.
-          -S, --no-silent       Print output as usual.
-          -z, --zero, --nofail  Don't fail. Always return a success (0) exit code.
-          -Z, --no-zero, --strict
-                                Return the original exit code.
-          -n NUMBER, --number NUMBER
-                                Command number. Useful for the 'tap' format.
-          -t TITLE, --title TITLE
-                                Command title. Default is the command itself.
-        ```
-        
-        ```python
-        from failprint.runners import run
-        
-        cmd = "echo hello"
-        
-        exit_code = run(
-            cmd,            # str, list of str, or Python callable
-            args=None,      # args for callable
-            kwargs=None,    # kwargs for callable
-            number=1,       # command number, useful for tap format
-            capture=None,   # stdout, stderr, both, none, True or False
-            title=None,     # command title
-            fmt=None,       # pretty, tap, or custom="MY_CUSTOM_FORMAT"
-            pty=False,      # use a PTY
-            progress=True,  # print the "progress" template before running the command
-            nofail=False,   # always return zero
-            quiet=False,    # don't print output when the command fails
-            silent=False,   # don't print anything
-        )
-        ```
+
+# failprint
+
+[![ci](https://github.com/pawamoy/failprint/workflows/ci/badge.svg)](https://github.com/pawamoy/failprint/actions?query=workflow%3Aci)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/failprint/)
+[![pypi version](https://img.shields.io/pypi/v/failprint.svg)](https://pypi.org/project/failprint/)
+[![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/pawamoy/failprint)
+[![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/failprint/community)
+
+Run a command, print its output only if it fails.
+
+Tired of searching the `quiet` options of your programs
+to lighten up the output of your `make check` or `make lint` commands?
+
+Tired of finding out that standard output and error are mixed up in some of them?
+
+Simply run your command through `failprint`.
+If it succeeds, nothing is printed.
+If it fails, standard error is printed.
+Plus other configuration goodies :wink:
+
+## Example
+
+You don't want to see output when the command succeeds.
+
+![demo](demo.svg)
+
+The task runner [`duty`](https://github.com/pawamoy/duty) uses `failprint`,
+allowing you to define tasks in Python and run them with minimalist and beautiful output:
+
+![demo_duty](demo_duty.svg)
+
+## Requirements
+
+failprint requires Python 3.6 or above.
+
+<details>
+<summary>To install Python 3.6, I recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
+
+```bash
+# install pyenv
+git clone https://github.com/pyenv/pyenv ~/.pyenv
+
+# setup pyenv (you should also put these three lines in .bashrc or similar)
+export PATH="${HOME}/.pyenv/bin:${PATH}"
+export PYENV_ROOT="${HOME}/.pyenv"
+eval "$(pyenv init -)"
+
+# install Python 3.6
+pyenv install 3.6.12
+
+# make it available globally
+pyenv global system 3.6.12
+```
+</details>
+
+## Installation
+
+With `pip`:
+```bash
+pip install failprint
+```
+
+With [`pipx`](https://github.com/pipxproject/pipx):
+```bash
+python3.7 -m pip install --user pipx
+pipx install failprint
+```
+
+## Usage
+
+```console
+% poetry run failprint -h
+usage: failprint [-h] [-c {stdout,stderr,both,none}] [-f {pretty,tap}] [-y | -Y] [-p | -P] [-q | -Q] [-s | -S] [-z | -Z] [-n NUMBER]
+                 [-t TITLE]
+                 COMMAND [COMMAND ...]
+
+positional arguments:
+  COMMAND
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c {stdout,stderr,both,none}, --capture {stdout,stderr,both,none}
+                        Which output to capture. Colors are supported with 'both' only, unless the command has a 'force color'
+                        option.
+  -f {pretty,tap}, --format {pretty,tap}
+                        Output format. Pass your own Jinja2 template as a string with '-f custom=TEMPLATE'. Available variables:
+                        command, title (command or title passed with -t), code (exit status), success (boolean), failure (boolean),
+                        number (command number passed with -n), output (command output), nofail (boolean), quiet (boolean), silent
+                        (boolean). Available filters: indent (textwrap.indent).
+  -y, --pty             Enable the use of a pseudo-terminal. PTY doesn't allow programs to use standard input.
+  -Y, --no-pty          Disable the use of a pseudo-terminal. PTY doesn't allow programs to use standard input.
+  -p, --progress        Print progress while running a command.
+  -P, --no-progress     Don't print progress while running a command.
+  -q, --quiet           Don't print the command output, even if it failed.
+  -Q, --no-quiet        Print the command output when it fails.
+  -s, --silent          Don't print anything.
+  -S, --no-silent       Print output as usual.
+  -z, --zero, --nofail  Don't fail. Always return a success (0) exit code.
+  -Z, --no-zero, --strict
+                        Return the original exit code.
+  -n NUMBER, --number NUMBER
+                        Command number. Useful for the 'tap' format.
+  -t TITLE, --title TITLE
+                        Command title. Default is the command itself.
+```
+
+```python
+from failprint.runners import run
+
+cmd = "echo hello"
+
+exit_code = run(
+    cmd,            # str, list of str, or Python callable
+    args=None,      # args for callable
+    kwargs=None,    # kwargs for callable
+    number=1,       # command number, useful for tap format
+    capture=None,   # stdout, stderr, both, none, True or False
+    title=None,     # command title
+    fmt=None,       # pretty, tap, or custom="MY_CUSTOM_FORMAT"
+    pty=False,      # use a PTY
+    progress=True,  # print the "progress" template before running the command
+    nofail=False,   # always return zero
+    quiet=False,    # don't print output when the command fails
+    silent=False,   # don't print anything
+)
+```
+
```

#### html2text {}

```diff
@@ -1,28 +1,34 @@
-Metadata-Version: 2.1 Name: failprint Version: 0.8.0 Summary: Run a command,
-print its output only if it fails. License: UNKNOWN Keywords:
+Metadata-Version: 2.1 Name: failprint Version: 0.9.0 Summary: Run a command,
+print its output only if it fails. License: ISC Keywords:
 cli,failure,output,runner Author-email: TimothÃ©e Mazzucotelli
-pm.me> Requires-Python: >=3.6 Classifier: Development Status :: 4 - Beta
-Classifier: License :: Other/Proprietary License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Project-URL: Changelog, https://pawamoy.github.io/failprint/changelog Project-
-URL: Discussions, https://github.com/pawamoy/failprint/discussions Project-URL:
-Documentation, https://pawamoy.github.io/failprint Project-URL: Funding, https:
-//github.com/sponsors/pawamoy Project-URL: Gitter, https://gitter.im/failprint/
-community Project-URL: Homepage, https://pawamoy.github.io/failprint Project-
-URL: Issues, https://github.com/pawamoy/failprint/issues Project-URL:
-Repository, https://github.com/pawamoy/failprint Description-Content-Type:
-text/markdown Description: # failprint [![ci](https://github.com/pawamoy/
-failprint/workflows/ci/badge.svg)](https://github.com/pawamoy/failprint/
-actions?query=workflow%3Aci) [![documentation](https://img.shields.io/badge/
-docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/
-failprint/) [![pypi version](https://img.shields.io/pypi/v/failprint.svg)]
-(https://pypi.org/project/failprint/) [![gitter](https://badges.gitter.im/
+pm.me> Requires-Python: >=3.7 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
+Documentation Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Documentation Classifier: Topic :: Utilities
+Classifier: Typing :: Typed Project-URL: Changelog, https://pawamoy.github.io/
+failprint/changelog Project-URL: Discussions, https://github.com/pawamoy/
+failprint/discussions Project-URL: Documentation, https://pawamoy.github.io/
+failprint Project-URL: Funding, https://github.com/sponsors/pawamoy Project-
+URL: Gitter, https://gitter.im/failprint/community Project-URL: Homepage,
+https://pawamoy.github.io/failprint Project-URL: Issues, https://github.com/
+pawamoy/failprint/issues Project-URL: Repository, https://github.com/pawamoy/
+failprint Description-Content-Type: text/markdown # failprint [![ci](https://
+github.com/pawamoy/failprint/workflows/ci/badge.svg)](https://github.com/
+pawamoy/failprint/actions?query=workflow%3Aci) [![documentation](https://
+img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://
+pawamoy.github.io/failprint/) [![pypi version](https://img.shields.io/pypi/v/
+failprint.svg)](https://pypi.org/project/failprint/) [![gitpod](https://
+img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/
+#https://github.com/pawamoy/failprint) [![gitter](https://badges.gitter.im/
 join%20chat.svg)](https://gitter.im/failprint/community) Run a command, print
 its output only if it fails. Tired of searching the `quiet` options of your
 programs to lighten up the output of your `make check` or `make lint` commands?
 Tired of finding out that standard output and error are mixed up in some of
 them? Simply run your command through `failprint`. If it succeeds, nothing is
 printed. If it fails, standard error is printed. Plus other configuration
 goodies :wink: ## Example You don't want to see output when the command
@@ -31,40 +37,40 @@
 them with minimalist and beautiful output: ![demo_duty](demo_duty.svg) ##
 Requirements failprint requires Python 3.6 or above.  To install Python 3.6, I
 recommend using pyenv. ```bash # install pyenv git clone https://github.com/
 pyenv/pyenv ~/.pyenv # setup pyenv (you should also put these three lines in
 .bashrc or similar) export PATH="${HOME}/.pyenv/bin:${PATH}" export
 PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install Python 3.6 pyenv
 install 3.6.12 # make it available globally pyenv global system 3.6.12 ```  ##
-Installation With `pip`: ```bash python3.6 -m pip install failprint ``` With
-[`pipx`](https://github.com/pipxproject/pipx): ```bash python3.6 -m pip install
---user pipx pipx install --python python3.6 failprint ``` ## Usage ```console %
-poetry run failprint -h usage: failprint [-h] [-c {stdout,stderr,both,none}] [-
-f {pretty,tap}] [-y | -Y] [-p | -P] [-q | -Q] [-s | -S] [-z | -Z] [-n NUMBER]
-[-t TITLE] COMMAND [COMMAND ...] positional arguments: COMMAND optional
-arguments: -h, --help show this help message and exit -c
-{stdout,stderr,both,none}, --capture {stdout,stderr,both,none} Which output to
-capture. Colors are supported with 'both' only, unless the command has a 'force
-color' option. -f {pretty,tap}, --format {pretty,tap} Output format. Pass your
-own Jinja2 template as a string with '-f custom=TEMPLATE'. Available variables:
-command, title (command or title passed with -t), code (exit status), success
-(boolean), failure (boolean), number (command number passed with -n), output
-(command output), nofail (boolean), quiet (boolean), silent (boolean).
-Available filters: indent (textwrap.indent). -y, --pty Enable the use of a
-pseudo-terminal. PTY doesn't allow programs to use standard input. -Y, --no-pty
-Disable the use of a pseudo-terminal. PTY doesn't allow programs to use
-standard input. -p, --progress Print progress while running a command. -P, --
-no-progress Don't print progress while running a command. -q, --quiet Don't
-print the command output, even if it failed. -Q, --no-quiet Print the command
-output when it fails. -s, --silent Don't print anything. -S, --no-silent Print
-output as usual. -z, --zero, --nofail Don't fail. Always return a success (0)
-exit code. -Z, --no-zero, --strict Return the original exit code. -n NUMBER, --
-number NUMBER Command number. Useful for the 'tap' format. -t TITLE, --title
-TITLE Command title. Default is the command itself. ``` ```python from
-failprint.runners import run cmd = "echo hello" exit_code = run( cmd, # str,
-list of str, or Python callable args=None, # args for callable kwargs=None, #
-kwargs for callable number=1, # command number, useful for tap format
-capture=None, # stdout, stderr, both, none, True or False title=None, # command
-title fmt=None, # pretty, tap, or custom="MY_CUSTOM_FORMAT" pty=False, # use a
-PTY progress=True, # print the "progress" template before running the command
-nofail=False, # always return zero quiet=False, # don't print output when the
-command fails silent=False, # don't print anything ) ```
+Installation With `pip`: ```bash pip install failprint ``` With [`pipx`](https:
+//github.com/pipxproject/pipx): ```bash python3.7 -m pip install --user pipx
+pipx install failprint ``` ## Usage ```console % poetry run failprint -h usage:
+failprint [-h] [-c {stdout,stderr,both,none}] [-f {pretty,tap}] [-y | -Y] [-p |
+-P] [-q | -Q] [-s | -S] [-z | -Z] [-n NUMBER] [-t TITLE] COMMAND [COMMAND ...]
+positional arguments: COMMAND optional arguments: -h, --help show this help
+message and exit -c {stdout,stderr,both,none}, --capture
+{stdout,stderr,both,none} Which output to capture. Colors are supported with
+'both' only, unless the command has a 'force color' option. -f {pretty,tap}, --
+format {pretty,tap} Output format. Pass your own Jinja2 template as a string
+with '-f custom=TEMPLATE'. Available variables: command, title (command or
+title passed with -t), code (exit status), success (boolean), failure
+(boolean), number (command number passed with -n), output (command output),
+nofail (boolean), quiet (boolean), silent (boolean). Available filters: indent
+(textwrap.indent). -y, --pty Enable the use of a pseudo-terminal. PTY doesn't
+allow programs to use standard input. -Y, --no-pty Disable the use of a pseudo-
+terminal. PTY doesn't allow programs to use standard input. -p, --progress
+Print progress while running a command. -P, --no-progress Don't print progress
+while running a command. -q, --quiet Don't print the command output, even if it
+failed. -Q, --no-quiet Print the command output when it fails. -s, --silent
+Don't print anything. -S, --no-silent Print output as usual. -z, --zero, --
+nofail Don't fail. Always return a success (0) exit code. -Z, --no-zero, --
+strict Return the original exit code. -n NUMBER, --number NUMBER Command
+number. Useful for the 'tap' format. -t TITLE, --title TITLE Command title.
+Default is the command itself. ``` ```python from failprint.runners import run
+cmd = "echo hello" exit_code = run( cmd, # str, list of str, or Python callable
+args=None, # args for callable kwargs=None, # kwargs for callable number=1, #
+command number, useful for tap format capture=None, # stdout, stderr, both,
+none, True or False title=None, # command title fmt=None, # pretty, tap, or
+custom="MY_CUSTOM_FORMAT" pty=False, # use a PTY progress=True, # print the
+"progress" template before running the command nofail=False, # always return
+zero quiet=False, # don't print output when the command fails silent=False, #
+don't print anything ) ```
```

