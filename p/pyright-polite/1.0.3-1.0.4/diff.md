# Comparing `tmp/pyright_polite-1.0.3.tar.gz` & `tmp/pyright_polite-1.0.4.tar.gz`

## Comparing `pyright_polite-1.0.3.tar` & `pyright_polite-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/.justfile
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/.pylintrc
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/setup.cfg
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/__about__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/__init__.py
--rw-r--r--   0        0        0     8846 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/cli.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/main.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/platform.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/polite.py
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/pyright.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/LICENSE
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/README.md
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/hatch.toml
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/.justfile
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/.pylintrc
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/setup.cfg
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/__about__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/__init__.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/cli.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/main.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/platform.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/polite.py
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/pyright.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/README.md
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/hatch.toml
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/PKG-INFO
```

### Comparing `pyright_polite-1.0.3/.justfile` & `pyright_polite-1.0.4/.justfile`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/.pre-commit-config.yaml` & `pyright_polite-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/src/pyright_polite/cli.py` & `pyright_polite-1.0.4/src/pyright_polite/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     def error(self, message: str):
         """Custom `error` method to exit with a returncode of 4 instead of 2.
 
         Pyright exits with a returncode of 4 when launched with invalid command-line
         arguments, so we should do the same.
 
         The `exit_on_error` parameter for `argparse.ArgumentParser` was only introduced
-        in Python 3.9, so we can't make us of that.
+        in Python 3.9, so we can't make use of that.
         """
         self.print_usage(sys.stderr)
         args = {"prog": self.prog, "message": message}
         self.exit(4, ("%(prog)s: error: %(message)s\n") % args)
 
 
 class CustomHelpFormatter(argparse.HelpFormatter):
@@ -134,16 +134,16 @@
 
 def prepare_argv(parsed_args: argparse.Namespace) -> List[str]:
     """Prepare argv for `asyncio.create_subprocess_exec()`.
 
     This includes the pyright executable (ie, argv[0]).
 
     pyright has args that are incompatible with each other, but instead of recreating
-    pyright's compatibility logic we'll just let pyright complain if it receives a set
-    of incompatible args.
+    pyright's compatibility logic we'll just let pyright complain if it receives
+    incompatible args.
 
     Args:
         parsed_args (argparse.Namespace): The parsed arguments.
 
     Returns:
         List[str]: The argv list to pass to `asyncio.create_subprocess_exec()`.
     """
@@ -211,15 +211,15 @@
     if any(arg in UNFILTERED_ARGS for arg in args):
         mode = Mode.UNFILTERED
 
     return mode
 
 
 def parse_cli() -> CommandLine:
-    """Handle command line arguments.
+    """Handle command-line arguments.
 
     Returns:
         CommandLine: The argv list and the deduced mode of operation.
     """
     parser: argparse.ArgumentParser = ArgumentParser(
         formatter_class=CustomHelpFormatter,
         allow_abbrev=False,
```

### Comparing `pyright_polite-1.0.3/src/pyright_polite/main.py` & `pyright_polite-1.0.4/src/pyright_polite/main.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/src/pyright_polite/platform.py` & `pyright_polite-1.0.4/src/pyright_polite/platform.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/src/pyright_polite/polite.py` & `pyright_polite-1.0.4/src/pyright_polite/polite.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,24 @@
     STDERR = auto()
     STDOUT = auto()
 
 
 class Polite:
     """Launch pyright, handle its output and react to signals."""
 
+    __slots__ = (
+        "subproc",
+        "_returncode",
+        "cli",
+        "stdout_lines",
+        "lock",
+        "signalled",
+        "signal_returncodes",
+    )
+
     def __init__(self, cli: CommandLine) -> None:
         """Prepare the instance."""
         self.subproc: asyncio.subprocess.Process
         self._returncode: int = 0
 
         self.cli: CommandLine = cli
         self.stdout_lines: List[str] = []
```

### Comparing `pyright_polite-1.0.3/src/pyright_polite/pyright.py` & `pyright_polite-1.0.4/src/pyright_polite/pyright.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/.gitignore` & `pyright_polite-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/LICENSE` & `pyright_polite-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/README.md` & `pyright_polite-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/hatch.toml` & `pyright_polite-1.0.4/hatch.toml`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/pyproject.toml` & `pyright_polite-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.3/PKG-INFO` & `pyright_polite-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright-polite
-Version: 1.0.3
+Version: 1.0.4
 Summary: An intelligent cross-platform wrapper for pyright that makes it less noisy.
 Project-URL: Homepage, https://github.com/jamielinux/pyright-polite
 Project-URL: Issues, https://github.com/jamielinux/pyright-polite/issues
 Project-URL: Source, https://github.com/jamielinux/pyright-polite
 Author-email: Jamie Nguyen <j@jamielinux.com>
 License-Expression: MIT
 License-File: LICENSE
```

