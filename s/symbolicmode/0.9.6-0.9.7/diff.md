# Comparing `tmp/symbolicmode-0.9.6.tar.gz` & `tmp/symbolicmode-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolicmode-0.9.6.tar", last modified: Mon Apr 10 01:34:34 2023, max compression
+gzip compressed data, was "symbolicmode-0.9.7.tar", last modified: Mon Apr 10 04:11:21 2023, max compression
```

## Comparing `symbolicmode-0.9.6.tar` & `symbolicmode-0.9.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:34:34.919566 symbolicmode-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-10 01:34:22.000000 symbolicmode-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-10 01:34:34.919566 symbolicmode-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-10 01:34:22.000000 symbolicmode-0.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-10 01:34:25.000000 symbolicmode-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 01:34:34.919566 symbolicmode-0.9.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:34:34.915566 symbolicmode-0.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:34:34.915566 symbolicmode-0.9.6/src/symbolicmode/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9017 2023-04-10 01:34:22.000000 symbolicmode-0.9.6/src/symbolicmode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:34:34.915566 symbolicmode-0.9.6/src/symbolicmode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-10 01:34:34.000000 symbolicmode-0.9.6/src/symbolicmode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-10 01:34:34.000000 symbolicmode-0.9.6/src/symbolicmode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 01:34:34.000000 symbolicmode-0.9.6/src/symbolicmode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 01:34:34.000000 symbolicmode-0.9.6/src/symbolicmode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:34:34.919566 symbolicmode-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-10 01:34:22.000000 symbolicmode-0.9.6/tests/test_chmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-10 01:34:22.000000 symbolicmode-0.9.6/tests/test_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-10 04:11:14.000000 symbolicmode-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.536718 symbolicmode-0.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.536718 symbolicmode-0.9.7/src/symbolicmode/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9621 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/src/symbolicmode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/src/symbolicmode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-10 04:11:21.000000 symbolicmode-0.9.7/src/symbolicmode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-10 04:11:21.000000 symbolicmode-0.9.7/src/symbolicmode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 04:11:21.000000 symbolicmode-0.9.7/src/symbolicmode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 04:11:21.000000 symbolicmode-0.9.7/src/symbolicmode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/tests/test_chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/tests/test_modes.py
```

### Comparing `symbolicmode-0.9.6/LICENSE` & `symbolicmode-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.6/PKG-INFO` & `symbolicmode-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 0.9.6
+Version: 0.9.7
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-0.9.6/README.md` & `symbolicmode-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.6/pyproject.toml` & `symbolicmode-0.9.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [project]
 name = "symbolicmode"
-version = "0.9.6"
+version = "0.9.7"
 authors = [
   { name="Sean Reifschneider", email="jafo00@gmail.com" },
 ]
 description = "Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `symbolicmode-0.9.6/src/symbolicmode/__init__.py` & `symbolicmode-0.9.7/src/symbolicmode/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """
 This module implements code for handling symbolic permissions in the way that GNU
 chmod from coreutils does.  For example: "a=rx,u+w" for 755
 
-Written by Sean Reifschneider and ChatGPT, 2023-03
+Written by Sean Reifschneider and ChatGPT, 2023-04
 """
 
 import os
 import re
 from typing import Union, Iterator, Tuple
 from pathlib import Path
 import stat
@@ -20,19 +20,27 @@
     is_directory: bool = False,
     umask: Union[int, None] = None,
 ) -> int:
     """
     Convert a symbolic file permission string to its numeric equivalent.
 
     The function takes a symbolic permission description string in the format of
-    `user[=,+,-]permissions,group[=,+,-]permissions,other[=,+,-]permissions`.
+    `[ugoa][=,+,-][PERMS][,...]`.
+
+    `ugoa` means "user", "group", "other", or "all" (short for "ugo"), representing
+    the permissions to be set.  If none of "ugoa" are listed, it acts as if "a" was
+    given, but applies the umask to the permission bits that are set.
+
     The available permission characters are `r` (read), `w` (write), `x` (execute),
     `X` (execute if a directory), `s` (setuid/setgid), and `t` (sticky bit), or a single
     character from: 'u', 'g', 'o'.
 
+    Multiple operators+permissions may be specified after the "ugoa", as with the "chown"
+    tool: "u=r+w-x".
+
     Args:
         symbolic_perm (str): The symbolic permission description string.
         initial_mode (int, optional): The mode to start off with.  If changing mode of an
                 existing file, this is it's current mode, and can also impact 'X'.
         is_directory (bool, optional): A boolean indicating whether the file is a directory.
                 This affects the behavior of the `X` permission. Defaults to False.
         umask (int, optional): Umask to use for "=[modes]" operation.  If not specified, the
@@ -51,105 +59,123 @@
         0o700
         >>> symbolic_to_numeric_permissions("u=rws,g=rx,o=r")
         0o4754
         >>> symbolic_to_numeric_permissions("=rw", initial_mode=0o4777, is_directory=False, umask=0o027)
         0o640
     """
 
+    #  Helpers
     def update_perm(operation: str, instruction_perms: int, current_perm: int) -> int:
-        "Helper function to apply `operation` to the current perms and the instruction_perms"
+        "Apply `operation` to the current perms and the instruction_perms"
         if operation == "=":
             return instruction_perms
         if operation == "+":
             return current_perm | instruction_perms
         return current_perm & ~instruction_perms
 
     def parse_instructions(permstr: str) -> Iterator[Tuple[str, str, str]]:
-        """Helper to parse the instruction into (lhs, op, rhs).  This also expands
+        """Parse the instruction into (lhs, op, rhs).  This also expands
         multi-operation expressions into multiple u/op/perm tuples."""
         rx = re.compile(r"([=+-][rwxXstugo]*)")
         for instruction in permstr.split(","):
             m = rx.split(instruction)
             if not m:
                 raise ValueError(f"Invalid instruction: {instruction}")
             user = m[0]
             for op, perm in [(op_perm[0], op_perm[1:]) for op_perm in m[1::2]]:
                 yield ((user, op, perm))
 
+    def sum_premissions(perms_str: str) -> int:
+        "Turn the permissions part of the statement into the numeric bits set"
+        unique_perms = set(perms_str)
+        if "x" in unique_perms and "X" in unique_perms:
+            unique_perms.remove("X")  # prevent doubling "x" bit
+        perms_sum = sum(
+            perm_values.get(p, perm_values.get(p.upper(), 0)) for p in unique_perms
+        )
+
+        #  handle u/g/o in PERMS
+        if ("u" in perms_str or "g" in perms_str or "o" in perms_str) and len(
+            perms_str
+        ) != 1:
+            raise ValueError(
+                "If u/g/o specified on RHS, only a single letter of u/g/o can be specified"
+            )
+        perms_sum = perms["u"] if perms_str == "u" else perms_sum
+        perms_sum = perms["g"] if perms_str == "g" else perms_sum
+        perms_sum = perms["o"] if perms_str == "o" else perms_sum
+
+        return perms_sum
+
+    def calc_special_bit(
+        value: int,
+        perms_str: str,
+        operation: str,
+        mode_char: str,
+        bit_value: int,
+        override: bool,
+    ) -> int:
+        "Calculate the special bits (suid/sgid/sticky)"
+        if mode_char in perms_str:
+            value = bit_value if operation in "+=" else 0
+        value = (
+            0
+            if mode_char not in perms_str and operation == "=" and not override
+            else value
+        )
+        return value
+
     # Define a mapping of symbolic permission characters to their corresponding numeric values
     perm_values = {"r": 4, "w": 2, "x": 1, "X": 1 if is_directory else 0, "-": 0}
 
     #  bits to shift based on u/g/o
     shift_by_user = {"u": 6, "g": 3, "o": 0}
 
     # Extract initial permissions and special bits
-    user_perms = (initial_mode >> 6) & 0o7
-    group_perms = (initial_mode >> 3) & 0o7
-    other_perms = (initial_mode >> 0) & 0o7
-    perms = {"u": user_perms, "g": group_perms, "o": other_perms}
+    perms = {
+        "u": (initial_mode >> 6) & 0o7,
+        "g": (initial_mode >> 3) & 0o7,
+        "o": initial_mode & 0o7,
+    }
     setuid_bit = 4 if initial_mode & 0o4000 else 0
     setgid_bit = 2 if initial_mode & 0o2000 else 0
     sticky_bit = 1 if initial_mode & 0o1000 else 0
 
+    #  get umask from system if not specified
     if umask is None:
         umask = os.umask(0)
         os.umask(umask)
 
     for users, operation, perms_str in parse_instructions(symbolic_perm):
-        #  set X value for executable based on current perms
+        #  if file: set X value if current perms have any 'x' bit set
         if not is_directory:
             perm_values["X"] = (
                 1 if perms["u"] & 1 or perms["g"] & 1 or perms["o"] & 1 else 0
             )
 
-        # calculate PERMS value
-        perm_set = set(perms_str)
-        if "x" in perm_set and "X" in perm_set:
-            perm_set.remove("X")  # prevent doubling "x" bit
-        perm_sum = sum(
-            perm_values.get(p, perm_values.get(p.upper(), 0)) for p in perm_set
-        )
-
-        #  handle u/g/o in PERMS
-        if ("u" in perms_str or "g" in perms_str or "o" in perms_str) and len(
-            perms_str
-        ) != 1:
-            raise ValueError(
-                "If u/g/o specified on RHS, only a single letter of u/g/o can be specified"
-            )
-        perm_sum = perms["u"] if perms_str == "u" else perm_sum
-        perm_sum = perms["g"] if perms_str == "g" else perm_sum
-        perm_sum = perms["o"] if perms_str == "o" else perm_sum
+        perm_sum = sum_premissions(perms_str)
 
         # Update the numeric file mode variables based on the users and operation
         effective_users = ("u", "g", "o") if users == "" or "a" in users else users
         for user in effective_users:
             apply_mask = (~umask if users == "" else 0o7777) >> shift_by_user[user]
             perms[user] = update_perm(operation, perm_sum & apply_mask, perms[user])
+
+            #  set special bits
             if user == "u":
-                if "s" in perms_str:
-                    setuid_bit = 4 if operation in "+=" else 0
-                setuid_bit = (
-                    0
-                    if "s" not in perms_str and operation == "=" and not is_directory
-                    else setuid_bit
+                setuid_bit = calc_special_bit(
+                    setuid_bit, perms_str, operation, "s", 4, is_directory
                 )
             if user == "g":
-                if "s" in perms_str:
-                    setgid_bit = 2 if operation in "+=" else 0
-                setgid_bit = (
-                    0
-                    if "s" not in perms_str and operation == "=" and not is_directory
-                    else setgid_bit
+                setgid_bit = calc_special_bit(
+                    setgid_bit, perms_str, operation, "s", 2, is_directory
                 )
             if user == "o":
-                if "t" in perms_str:
-                    sticky_bit = 1 if operation in "+=" else 0
-                sticky_bit = (
-                    0 if "t" not in perms_str and operation == "=" else sticky_bit
+                sticky_bit = calc_special_bit(
+                    sticky_bit, perms_str, operation, "t", 1, False
                 )
 
     # Combine the numeric file modes for the owner, group, and others into a single numeric file mode
     return (
         ((setuid_bit + setgid_bit + sticky_bit) << 9)
         | (perms["u"] << 6)
         | (perms["g"] << 3)
```

### Comparing `symbolicmode-0.9.6/src/symbolicmode.egg-info/PKG-INFO` & `symbolicmode-0.9.7/src/symbolicmode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 0.9.6
+Version: 0.9.7
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-0.9.6/tests/test_chmod.py` & `symbolicmode-0.9.7/tests/test_chmod.py`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.6/tests/test_modes.py` & `symbolicmode-0.9.7/tests/test_modes.py`

 * *Files identical despite different names*

