# Comparing `tmp/secimport-0.7.0.tar.gz` & `tmp/secimport-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secimport-0.7.0.tar", max compression
+gzip compressed data, was "secimport-0.7.3.tar", max compression
```

## Comparing `secimport-0.7.0.tar` & `secimport-0.7.3.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0     1069 2022-07-09 18:11:47.562704 secimport-0.7.0/LICENSE
--rw-r--r--   0        0        0     4389 2023-04-09 18:52:50.816277 secimport-0.7.0/README.md
--rw-r--r--   0        0        0     1715 2023-04-09 18:52:50.838075 secimport-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      437 2023-04-09 18:52:50.838697 secimport-0.7.0/secimport/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:52:50.838812 secimport-0.7.0/secimport/backends/bpftrace_backend/__init__.py
--rw-r--r--   0        0        0      362 2023-04-09 18:52:50.839406 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
--rw-r--r--   0        0        0      373 2023-04-09 18:52:50.839675 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/kill_process.bt
--rw-r--r--   0        0        0      125 2023-04-09 18:52:50.840067 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_file_system.bt
--rw-r--r--   0        0        0      110 2023-04-09 18:52:50.840472 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_network.bt
--rw-r--r--   0        0        0       72 2023-04-09 18:52:50.840884 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
--rw-r--r--   0        0        0       71 2023-04-09 18:52:50.841620 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
--rw-r--r--   0        0        0      183 2023-04-09 18:52:50.841872 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_syscall.bt
--rw-r--r--   0        0        0     8797 2023-04-09 18:52:50.842186 secimport-0.7.0/secimport/backends/bpftrace_backend/bpftrace_backend.py
--rw-r--r--   0        0        0    22157 2023-04-09 18:52:50.843083 secimport-0.7.0/secimport/backends/bpftrace_backend/default.template.bt
--rw-r--r--   0        0        0    23175 2023-04-09 18:52:50.844075 secimport-0.7.0/secimport/backends/bpftrace_backend/default.yaml.template.bt
--rw-r--r--   0        0        0       67 2023-04-09 18:52:50.844594 secimport-0.7.0/secimport/backends/bpftrace_backend/filters/file_system.bt
--rw-r--r--   0        0        0      176 2023-04-09 18:52:50.845002 secimport-0.7.0/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
--rw-r--r--   0        0        0       40 2023-04-09 18:52:50.845662 secimport-0.7.0/secimport/backends/bpftrace_backend/filters/networking.bt
--rw-r--r--   0        0        0      553 2023-04-09 18:52:50.846141 secimport-0.7.0/secimport/backends/bpftrace_backend/filters/processes.bt
--rwxr-xr-x   0        0        0    22668 2023-04-09 18:52:50.846870 secimport-0.7.0/secimport/backends/bpftrace_backend/generate_profile.bt
--rw-r--r--   0        0        0     1203 2023-04-09 18:52:50.847215 secimport-0.7.0/secimport/backends/bpftrace_backend/new_template.bt
--rw-r--r--   0        0        0      502 2023-04-09 18:52:50.847539 secimport-0.7.0/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
--rw-r--r--   0        0        0        0 2023-04-09 18:52:50.847638 secimport-0.7.0/secimport/backends/common/__init__.py
--rw-r--r--   0        0        0      112 2023-04-09 18:52:50.847941 secimport-0.7.0/secimport/backends/common/instrumentation_backend.py
--rw-r--r--   0        0        0     7102 2023-04-09 18:52:50.848401 secimport-0.7.0/secimport/backends/common/utils.py
--rw-r--r--   0        0        0        0 2023-04-09 18:52:50.848529 secimport-0.7.0/secimport/backends/dtrace_backend/__init__.py
--rw-r--r--   0        0        0      415 2023-04-09 18:52:50.849122 secimport-0.7.0/secimport/backends/dtrace_backend/actions/kill_on_processing.d
--rw-r--r--   0        0        0      662 2023-04-09 18:52:50.850407 secimport-0.7.0/secimport/backends/dtrace_backend/actions/kill_process.d
--rw-r--r--   0        0        0      134 2023-04-09 18:52:50.850975 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_file_system.d
--rw-r--r--   0        0        0      124 2023-04-09 18:52:50.851498 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_network.d
--rw-r--r--   0        0        0      187 2023-04-09 18:52:50.852004 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
--rw-r--r--   0        0        0      188 2023-04-09 18:52:50.852531 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
--rw-r--r--   0        0        0       64 2023-04-09 18:52:50.853048 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_syscall.d
--rwxr-xr-x   0        0        0     1606 2023-04-09 18:52:50.853621 secimport-0.7.0/secimport/backends/dtrace_backend/default.allowlist.template.d
--rwxr-xr-x   0        0        0     1081 2023-04-09 18:52:50.854185 secimport-0.7.0/secimport/backends/dtrace_backend/default.blocklist.template.d
--rwxr-xr-x   0        0        0     1753 2023-04-09 18:52:50.854734 secimport-0.7.0/secimport/backends/dtrace_backend/default.template.d
--rwxr-xr-x   0        0        0     2587 2023-04-09 18:52:50.855314 secimport-0.7.0/secimport/backends/dtrace_backend/default.yaml.template.d
--rw-r--r--   0        0        0     8813 2023-04-09 18:52:50.856136 secimport-0.7.0/secimport/backends/dtrace_backend/dtrace_backend.py
--rw-r--r--   0        0        0      172 2023-04-09 18:52:50.857008 secimport-0.7.0/secimport/backends/dtrace_backend/filters/file_system.d
--rw-r--r--   0        0        0      177 2023-04-09 18:52:50.857464 secimport-0.7.0/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
--rw-r--r--   0        0        0       31 2023-04-09 18:52:50.857889 secimport-0.7.0/secimport/backends/dtrace_backend/filters/networking.d
--rw-r--r--   0        0        0      436 2023-04-09 18:52:50.858379 secimport-0.7.0/secimport/backends/dtrace_backend/filters/processes.d
--rw-r--r--   0        0        0      969 2023-04-09 18:52:50.858858 secimport-0.7.0/secimport/backends/dtrace_backend/generate_profile.d
--rw-r--r--   0        0        0       30 2023-04-09 18:52:50.859176 secimport-0.7.0/secimport/backends/dtrace_backend/headers/destructive.d
--rw-r--r--   0        0        0     1238 2023-04-09 18:52:50.859698 secimport-0.7.0/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
--rwxr-xr-x   0        0        0     4389 2023-04-09 18:52:50.860203 secimport-0.7.0/secimport/backends/dtrace_backend/py_sandbox.d
--rw-r--r--   0        0        0    13365 2023-04-09 18:52:50.860554 secimport-0.7.0/secimport/cli.py
--rwxr-xr-x   0        0        0    22294 2023-04-09 18:52:50.860987 secimport-0.7.0/secimport/profiles/trace.bt
--rw-r--r--   0        0        0     3048 2023-04-09 18:52:50.861289 secimport-0.7.0/secimport/sandbox_helper.py
--rw-r--r--   0        0        0     5705 2023-04-09 18:53:17.178027 secimport-0.7.0/setup.py
--rw-r--r--   0        0        0     5065 2023-04-09 18:53:17.178415 secimport-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-09 23:14:32.882650 secimport-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4590 2023-04-09 23:14:32.882650 secimport-0.7.3/README.md
+-rw-r--r--   0        0        0     1715 2023-04-09 23:14:32.882650 secimport-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      437 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
+-rw-r--r--   0        0        0      373 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/kill_process.bt
+-rw-r--r--   0        0        0      125 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_file_system.bt
+-rw-r--r--   0        0        0      110 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_network.bt
+-rw-r--r--   0        0        0       72 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
+-rw-r--r--   0        0        0       71 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
+-rw-r--r--   0        0        0      183 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_syscall.bt
+-rw-r--r--   0        0        0     8757 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/bpftrace_backend.py
+-rw-r--r--   0        0        0    22157 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/default.template.bt
+-rw-r--r--   0        0        0     1653 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/default.yaml.template.bt
+-rw-r--r--   0        0        0       67 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/filters/file_system.bt
+-rw-r--r--   0        0        0      176 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
+-rw-r--r--   0        0        0       40 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/filters/networking.bt
+-rw-r--r--   0        0        0      553 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/filters/processes.bt
+-rwxr-xr-x   0        0        0    22668 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/generate_profile.bt
+-rw-r--r--   0        0        0     1203 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/new_template.bt
+-rw-r--r--   0        0        0      502 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
+-rw-r--r--   0        0        0        0 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/common/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/common/instrumentation_backend.py
+-rw-r--r--   0        0        0    14433 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/common/utils.py
+-rw-r--r--   0        0        0        0 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/kill_on_processing.d
+-rw-r--r--   0        0        0      662 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/kill_process.d
+-rw-r--r--   0        0        0      134 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_file_system.d
+-rw-r--r--   0        0        0      124 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_network.d
+-rw-r--r--   0        0        0      187 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
+-rw-r--r--   0        0        0      188 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
+-rw-r--r--   0        0        0       64 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_syscall.d
+-rwxr-xr-x   0        0        0     1606 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/default.allowlist.template.d
+-rwxr-xr-x   0        0        0     1081 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/default.blocklist.template.d
+-rwxr-xr-x   0        0        0     1753 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/default.template.d
+-rwxr-xr-x   0        0        0     2587 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/default.yaml.template.d
+-rw-r--r--   0        0        0     8813 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/dtrace_backend.py
+-rw-r--r--   0        0        0      172 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/filters/file_system.d
+-rw-r--r--   0        0        0      177 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
+-rw-r--r--   0        0        0       31 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/filters/networking.d
+-rw-r--r--   0        0        0      436 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/filters/processes.d
+-rw-r--r--   0        0        0      969 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/generate_profile.d
+-rw-r--r--   0        0        0       30 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/headers/destructive.d
+-rw-r--r--   0        0        0     1238 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
+-rwxr-xr-x   0        0        0     4389 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/py_sandbox.d
+-rw-r--r--   0        0        0    13365 2023-04-09 23:14:32.886650 secimport-0.7.3/secimport/cli.py
+-rwxr-xr-x   0        0        0    22294 2023-04-09 23:14:32.886650 secimport-0.7.3/secimport/profiles/trace.bt
+-rw-r--r--   0        0        0     3048 2023-04-09 23:14:32.886650 secimport-0.7.3/secimport/sandbox_helper.py
+-rw-r--r--   0        0        0     5317 1970-01-01 00:00:00.000000 secimport-0.7.3/PKG-INFO
```

### Comparing `secimport-0.7.0/LICENSE` & `secimport-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/README.md` & `secimport-0.7.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # secimport
 
 `secimport` is a cross-platform sandbox toolkit that traces your Python application and enforces privileges per module in your code in runtime. It uses backends like bpftrace (eBPF) and dtrace under the hood.
 
+[![Upload Python Package](https://github.com/avilum/secimport/actions/workflows/python-publish.yml/badge.svg?branch=master)](https://github.com/avilum/secimport/actions/workflows/python-publish.yml)
+
+
 ## Why It's Awesome
 
 - Trace which syscalls are called by each module in your code.
   - `secimport` uses USDT (Userland Statically Defined Tracing) probes in the runtime (Python interpreter for example) using eBPF and dtrace instrumentation scripts.
   - Audit the flow of your application at user-space/os/kernel level
 - Reduce supply chain attack and RCE vectors by restricting modules/packages inside your production environment.
 - No performance impact (see [Performance](https://github.com/avilum/secimport/wiki/Performance-Benchmarks)).
```

#### html2text {}

```diff
@@ -1,20 +1,23 @@
 # secimport `secimport` is a cross-platform sandbox toolkit that traces your
 Python application and enforces privileges per module in your code in runtime.
-It uses backends like bpftrace (eBPF) and dtrace under the hood. ## Why It's
-Awesome - Trace which syscalls are called by each module in your code. -
-`secimport` uses USDT (Userland Statically Defined Tracing) probes in the
-runtime (Python interpreter for example) using eBPF and dtrace instrumentation
-scripts. - Audit the flow of your application at user-space/os/kernel level -
-Reduce supply chain attack and RCE vectors by restricting modules/packages
-inside your production environment. - No performance impact (see [Performance]
-(https://github.com/avilum/secimport/wiki/Performance-Benchmarks)). - Don't
-change the way you code! - Supports `Python` at the moment - `Go` is under
-development ## Installation For evaluation, we highly recommend the QuickStart
-with Docker instead of self-installing.
+It uses backends like bpftrace (eBPF) and dtrace under the hood. [![Upload
+Python Package](https://github.com/avilum/secimport/actions/workflows/python-
+publish.yml/badge.svg?branch=master)](https://github.com/avilum/secimport/
+actions/workflows/python-publish.yml) ## Why It's Awesome - Trace which
+syscalls are called by each module in your code. - `secimport` uses USDT
+(Userland Statically Defined Tracing) probes in the runtime (Python interpreter
+for example) using eBPF and dtrace instrumentation scripts. - Audit the flow of
+your application at user-space/os/kernel level - Reduce supply chain attack and
+RCE vectors by restricting modules/packages inside your production environment.
+- No performance impact (see [Performance](https://github.com/avilum/secimport/
+wiki/Performance-Benchmarks)). - Don't change the way you code! - Supports
+`Python` at the moment - `Go` is under development ## Installation For
+evaluation, we highly recommend the QuickStart with Docker instead of self-
+installing.
 If you are not using Docker, follow Installation to install eBPF or DTrace. -
 To install secimport from git clone: `python3 -m pip install -e .` - To install
 secimport from pypi (latest stable release): `python3 -m pip install secimport`
 ## Docker The quickest way to evaluate `secimport` is to use our [Docker
 container](docker/README.md), which includes `bpftrace` (`ebpf`) and other
 plug-and-play examples. ## Quick Start - Using the CLI To run an end-to-end
 interactive example: 1. Build a docker with custom kernel that matches your
```

### Comparing `secimport-0.7.0/pyproject.toml` & `secimport-0.7.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secimport"
-version = "0.7.0"
+version = "0.7.3"
 description = "A sandbox/supervisor for python modules."
 authors = ["Avi Lumelsky"]
 license = "MIT"
 homepage = "https://github.com/avilum/secimport"
 readme = "README.md"
 packages = [
     { include = "secimport" },
```

### Comparing `secimport-0.7.0/secimport/backends/bpftrace_backend/bpftrace_backend.py` & `secimport-0.7.3/secimport/backends/bpftrace_backend/bpftrace_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import importlib
 import os
 import subprocess
 from sys import executable as PYTHON_EXECUTABLE
 import stat
 from pathlib import Path
-from time import sleep
 
 from secimport.backends.common.utils import (
     BASE_DIR_NAME,
     SECIMPORT_ROOT,
 )
 
 TEMPLATES_DIR_NAME = SECIMPORT_ROOT / "backends" / "bpftrace_backend"
@@ -103,15 +102,14 @@
     st = os.stat(module_file_path)
     os.chmod(module_file_path, st.st_mode | stat.S_IEXEC)
     print("(sandbox command): ", bpftrace_command)
     print()
     print("Waiting for bpftrace.... ")
     if not dry_run:
         os.system(bpftrace_command)
-        sleep(5)
     return True
 
 
 def render_bpftrace_template(
     module_traced_name: str,
     allow_shells: bool,
     allow_networking: bool,
```

### Comparing `secimport-0.7.0/secimport/backends/bpftrace_backend/default.template.bt` & `secimport-0.7.3/secimport/backends/bpftrace_backend/default.template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/bpftrace_backend/default.yaml.template.bt` & `secimport-0.7.3/secimport/backends/bpftrace_backend/generate_profile.bt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env bpftrace
 
+// Usage:
+// ./trace.bt -c Python-3.10.0/python
+
 BEGIN {
     // Mapping all syscalls both ways, based on https://github.com/iovisor/bpftrace/blob/2c7a7a598dbe1aa790db2dfe2db242aa69137d5b/tools/syscount.bt
     // Generates using bash:
     //   $ apt-get install auditd
     //   $ ausyscall --dump | awk 'NR > 1 { printf("\t@sysname[%d] = \"%s\";\n", $1, $2); }';
     printf("REGISTERING SYSCALLS...\n");
     @sysname[0] = "read";
@@ -675,75 +678,61 @@
 	@sysnum["pwritev2"] = 328;
 	@sysnum["pkey_mprotect"] = 329;
 	@sysnum["pkey_alloc"] = 330;
 	@sysnum["pkey_free"] = 331;
 	@sysnum["statx"] = 332;
 	@sysnum["io_pgetevents"] = 333;
 	@sysnum["rseq"] = 334;
-
-    ###SYSCALL_FILTER###
-    printf("STARTED\n");
+    printf("Tracing Modules - Exit gracefully with Ctrl+D\n")
 }
 
-
-usdt:###INTERPRETER_PATH###:function__entry {
+// function__entry(str filename, str funcname, int lineno)
+usdt:/workspace/Python-3.10.0/python:function__entry {
         @["depth"]++;
         @entrypoints[str(arg0)] = @["depth"];
         @globals["previous_module"] = @globals["current_module"];
         @globals["current_module"] = str(arg0);
-        @latest_supervised_module =  str(arg0);
-        // printf("%s, %s, depth=%d\n", str(arg0), str(arg1), @["depth"]);
+
+        // To trace python calls in the console, uncomment:
+        // printf("%s, %s, depth=%d\n", str(arg0), str(arg1), @["depth"]) ;
 }
 
-usdt:###INTERPRETER_PATH###:function__return {
-    @["depth"]--;
+// function__return(str filename, str funcname, int lineno)
+usdt:/workspace/Python-3.10.0/python:function__return {
+        @["depth"]--;
 }
 
 tracepoint:raw_syscalls:sys_enter /comm == "python"/ {
-    // Allowing global requirements ("general requirements") to be used by all syscalls.
-    if (@syscalls_filters["general_requirements", @sysname[args->id]] != 1){
-        // Logging every syscall that was not confirmed by the user at compile time.
-        if (@syscalls_filters[@latest_supervised_module, @sysname[args->id]] != 1){
-            printf("\033[91m[SECURITY PROFILE VIOLATED]: %s called syscall %s at depth %d\033[0m\r\n", @latest_supervised_module, @sysname[args->id], @["depth"]);
-
-            if (str($1) == "STOP") {
-                printf("\n^^^ STOPPING PROCESS %d DUE TO SYSCALL VIOLATION ^^^\n", pid);
-                signal("SIGSTOP");
-                printf("\t\tPROCESS %d STOPPED.\r\n", pid);
-            }
-
-            if (str($1) == "KILL") {
-                printf("\n^^^ KILLING PROCESS %d DUE TO SYSCALL VIOLATION ^^^\n", pid);
-                signal("SIGKILL");
-                // system("pkill -9 python"); // optional. Please use "bpftrace --unsafe" or remove this line.
-                printf("\t\tKILLED.\r\n");
-                exit(); // optional
-            }
-        }
-    }
+    // @modules_syscalls[@globals["current_module"], @sysname[args->id], @["depth"]] = count();
+    @modules_syscalls[@globals["current_module"], @sysname[args->id]] = count();
+    @syscalls[@sysname[args->id]] = count();
 }
 
 
 // Invoked before importlib imports a module
 // import__find__load__start(str modulename)
-// usdt:###INTERPRETER_PATH###:import__find__load__start {
-    // TODO: verify that the module is allowed in the syscall filter.
+usdt:###INTERPRETER_PATH###:import__find__load__start {
     // @imports[arg0] = count();
-    // printf("importing %d", arg0);
-// }
+    // printf('importing %s', arg0);
+}
 
 // Invoked after importlib imports a module
 // import__find__load__done(str modulename, int found)
-// usdt:###INTERPRETER_PATH###:import__find__load__done{
-    // printf("imported %d", arg0);
-// }
-
+usdt:###INTERPRETER_PATH###:import__find__load__done{
+    // printf('imported %s with result %d', arg0, arg1);
+}
 
 END {
+    printf("Summary:");
+	printf(" %-32s %-10s %-22s %8s\r\n", "FILE", "TYPE", "NAME", "COUNT");
+	printf("\r\nAll syscalls (count):\r\n");
+	print(@syscalls);
+    printf("\r\nSyscalls Per Python Module:\r\n");
+    print(@modules_syscalls);
+	printf("\r\nDone.\r\n");
     clear(@sysname);
     clear(@sysnum);
+    clear(@syscalls);
+    clear(@modules_syscalls);
     clear(@entrypoints);
-    clear(@syscalls_filters);
     clear(@globals);
-    clear(@latest_supervised_module);
-    clear(@);
 }
```

### Comparing `secimport-0.7.0/secimport/backends/bpftrace_backend/filters/processes.bt` & `secimport-0.7.3/secimport/backends/bpftrace_backend/filters/processes.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/bpftrace_backend/generate_profile.bt` & `secimport-0.7.3/secimport/profiles/trace.bt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env bpftrace
 
+// A profiling script that logs all the syscalls, per python module.
+// It can be attached to a running process using -p or can be used to trace a python shell interactively.
+//
 // Usage:
 // ./trace.bt -c Python-3.10.0/python
 
 BEGIN {
     // Mapping all syscalls both ways, based on https://github.com/iovisor/bpftrace/blob/2c7a7a598dbe1aa790db2dfe2db242aa69137d5b/tools/syscount.bt
     // Generates using bash:
     //   $ apt-get install auditd
@@ -681,58 +684,43 @@
 	@sysnum["pkey_free"] = 331;
 	@sysnum["statx"] = 332;
 	@sysnum["io_pgetevents"] = 333;
 	@sysnum["rseq"] = 334;
     printf("Tracing Modules - Exit gracefully with Ctrl+D\n")
 }
 
-// function__entry(str filename, str funcname, int lineno)
 usdt:/workspace/Python-3.10.0/python:function__entry {
         @["depth"]++;
         @entrypoints[str(arg0)] = @["depth"];
         @globals["previous_module"] = @globals["current_module"];
         @globals["current_module"] = str(arg0);
 
         // To trace python calls in the console, uncomment:
         // printf("%s, %s, depth=%d\n", str(arg0), str(arg1), @["depth"]) ;
 }
 
-// function__return(str filename, str funcname, int lineno)
 usdt:/workspace/Python-3.10.0/python:function__return {
         @["depth"]--;
 }
 
 tracepoint:raw_syscalls:sys_enter /comm == "python"/ {
     // @modules_syscalls[@globals["current_module"], @sysname[args->id], @["depth"]] = count();
     @modules_syscalls[@globals["current_module"], @sysname[args->id]] = count();
     @syscalls[@sysname[args->id]] = count();
 }
 
 
-// Invoked before importlib imports a module
-// import__find__load__start(str modulename)
-usdt:###INTERPRETER_PATH###:import__find__load__start {
-    // @imports[arg0] = count();
-    // printf('importing %s', arg0);
-}
-
-// Invoked after importlib imports a module
-// import__find__load__done(str modulename, int found)
-usdt:###INTERPRETER_PATH###:import__find__load__done{
-    // printf('imported %s with result %d', arg0, arg1);
-}
-
 END {
     printf("Summary:");
 	printf(" %-32s %-10s %-22s %8s\r\n", "FILE", "TYPE", "NAME", "COUNT");
 	printf("\r\nAll syscalls (count):\r\n");
 	print(@syscalls);
     printf("\r\nSyscalls Per Python Module:\r\n");
     print(@modules_syscalls);
 	printf("\r\nDone.\r\n");
     clear(@sysname);
     clear(@sysnum);
     clear(@syscalls);
     clear(@modules_syscalls);
     clear(@entrypoints);
-    clear(@globals);
+    clear(@globals)
 }
```

### Comparing `secimport-0.7.0/secimport/backends/bpftrace_backend/new_template.bt` & `secimport-0.7.3/secimport/backends/bpftrace_backend/new_template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/dtrace_backend/actions/kill_process.d` & `secimport-0.7.3/secimport/backends/dtrace_backend/actions/kill_process.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/dtrace_backend/default.allowlist.template.d` & `secimport-0.7.3/secimport/backends/dtrace_backend/default.allowlist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/dtrace_backend/default.blocklist.template.d` & `secimport-0.7.3/secimport/backends/dtrace_backend/default.blocklist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/dtrace_backend/default.template.d` & `secimport-0.7.3/secimport/backends/dtrace_backend/default.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/dtrace_backend/default.yaml.template.d` & `secimport-0.7.3/secimport/backends/dtrace_backend/default.yaml.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/dtrace_backend/dtrace_backend.py` & `secimport-0.7.3/secimport/backends/dtrace_backend/dtrace_backend.py`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/dtrace_backend/generate_profile.d` & `secimport-0.7.3/secimport/backends/dtrace_backend/generate_profile.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d` & `secimport-0.7.3/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/backends/dtrace_backend/py_sandbox.d` & `secimport-0.7.3/secimport/backends/dtrace_backend/py_sandbox.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/cli.py` & `secimport-0.7.3/secimport/cli.py`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/secimport/sandbox_helper.py` & `secimport-0.7.3/secimport/sandbox_helper.py`

 * *Files identical despite different names*

### Comparing `secimport-0.7.0/setup.py` & `secimport-0.7.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,133 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: secimport
+Version: 0.7.3
+Summary: A sandbox/supervisor for python modules.
+Home-page: https://github.com/avilum/secimport
+License: MIT
+Author: Avi Lumelsky
+Requires-Python: >=3.6,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: fire (>=0.4.0,<0.5.0)
+Description-Content-Type: text/markdown
+
+# secimport
+
+`secimport` is a cross-platform sandbox toolkit that traces your Python application and enforces privileges per module in your code in runtime. It uses backends like bpftrace (eBPF) and dtrace under the hood.
+
+[![Upload Python Package](https://github.com/avilum/secimport/actions/workflows/python-publish.yml/badge.svg?branch=master)](https://github.com/avilum/secimport/actions/workflows/python-publish.yml)
+
+
+## Why It's Awesome
+
+- Trace which syscalls are called by each module in your code.
+  - `secimport` uses USDT (Userland Statically Defined Tracing) probes in the runtime (Python interpreter for example) using eBPF and dtrace instrumentation scripts.
+  - Audit the flow of your application at user-space/os/kernel level
+- Reduce supply chain attack and RCE vectors by restricting modules/packages inside your production environment.
+- No performance impact (see [Performance](https://github.com/avilum/secimport/wiki/Performance-Benchmarks)).
+- Don't change the way you code!
+- Supports `Python` at the moment
+  -  `Go` is under development
+
+
+## Installation
+For evaluation, we highly recommend the QuickStart with <a href="#Docker">Docker</a> instead of self-installing.<br>
+If you are not using Docker, follow <a href="https://github.com/avilum/secimport/wiki/Installation">Installation</a> to install eBPF or DTrace.
+- To install secimport from git clone: `python3 -m pip install -e .`
+- To install secimport from pypi (latest stable release): `python3 -m pip install secimport`
+
+
+## Docker
+The quickest way to evaluate `secimport` is to use our [Docker container](docker/README.md), which includes `bpftrace` (`ebpf`) and other plug-and-play examples.
+
+## Quick Start - Using the CLI
+To run an end-to-end interactive example:
+1. Build a docker with custom kernel that matches your existing OS kernel version
+    ```
+    ➜  secimport ✗ cd docker/
+    ➜  docker ✗ ./build.sh
+    ```
+2. Run the container
+    ```
+    ➜  docker ✗ ./run.sh
+    Running temporary container...
+
+    root@f05d2c33b0b3:/workspace#
+    ```
+3. Use the CLI
+    ```
+    root@f05d2c33b0b3:/workspace# secimport interactive
+
+    Let's create our first tailor-made sandbox with secimport!
+    - A python shell will be opened
+    - The behavior will be recorded.
+
+    OK? (y): y
+    >>> secimport trace
+
+    TRACING: ['/workspace/secimport/profiles/trace.bt', '-c', '/workspace/Python-3.10.0/python', '-o', 'trace.log']
+
+                            Press CTRL+D/CTRL+C to stop the trace;
+
+    Python 3.10.0 (default, Apr  9 2023, 17:19:17) [GCC 9.4.0] on linux
+    Type "help", "copyright", "credits" or "license" for more information.
+    >>> import ...
+
+
+    ```
+## Sandbox Your Program (Using the CLI)
+`secimport trace` will start a bpftrace program that will log all the syscalls for all the modules in your application into a file.<br>
+Once you covered the logic you would like to or sandbox and you're satisfied, hit `CTRL+C` or `CTRL+D` or wait for the program to finish.
+```
+$ secimport trace
+$ secimport trace -h
+$ secimport trace_pid 123
+$ secimport trace_pid -h
+```
+
+Then, build a sandbox from the trace using the `build` command:
+```
+# secimport build
+$ secimport build -h
+```
+
+Finally, run the sandbox with the `run` command:
+```
+$ secimport run
+$ secimport run --entrypoint my_custom_main.py
+$ secimport run --entrypoint my_custom_main.py --stop_on_violation=true
+$ secimport run --entrypoint my_custom_main.py --kill_on_violation=true
+$ secimport run --sandbox_executable /path/to/my_sandbox.bt --pid 2884
+$ secimport run --sandbox_executable /path/to/my_sandbox.bt --sandbox_logfile my_log.log
+$ secimport run -h
+```
+
+For more detailed usage instructions, see the [Command-Line Usage](https://github.com/avilum/secimport/wiki/Command-Line-Usage) page.
+
+## Python API
+
+You can also use `secimport` by replacing `import` with `secimport.secure_import` for selected modules. See the [Python Imports](examples/python_imports/) example for more details.
+
+## Examples
+
+The [Sandbox Examples](https://github.com/avilum/secimport/wiki/Sandbox-Examples) page contains basic and advanced real-world examples.
+
+## Contributing
+
+For information on how to contribute to `secimport`, see the [Contributing](https://github.com/avilum/secimport/blob/master/docs/CONTRIBUTING.md) guide.
 
-packages = \
-['secimport',
- 'secimport.backends.bpftrace_backend',
- 'secimport.backends.common',
- 'secimport.backends.dtrace_backend']
-
-package_data = \
-{'': ['*'],
- 'secimport': ['profiles/*'],
- 'secimport.backends.bpftrace_backend': ['actions/*', 'filters/*', 'probes/*'],
- 'secimport.backends.dtrace_backend': ['actions/*',
-                                       'filters/*',
-                                       'headers/*',
-                                       'probes/*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0', 'fire>=0.4.0,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['secimport = secimport.cli:main']}
-
-setup_kwargs = {
-    'name': 'secimport',
-    'version': '0.7.0',
-    'description': 'A sandbox/supervisor for python modules.',
-    'long_description': '# secimport\n\n`secimport` is a cross-platform sandbox toolkit that traces your Python application and enforces privileges per module in your code in runtime. It uses backends like bpftrace (eBPF) and dtrace under the hood.\n\n## Why It\'s Awesome\n\n- Trace which syscalls are called by each module in your code.\n  - `secimport` uses USDT (Userland Statically Defined Tracing) probes in the runtime (Python interpreter for example) using eBPF and dtrace instrumentation scripts.\n  - Audit the flow of your application at user-space/os/kernel level\n- Reduce supply chain attack and RCE vectors by restricting modules/packages inside your production environment.\n- No performance impact (see [Performance](https://github.com/avilum/secimport/wiki/Performance-Benchmarks)).\n- Don\'t change the way you code!\n- Supports `Python` at the moment\n  -  `Go` is under development\n\n\n## Installation\nFor evaluation, we highly recommend the QuickStart with <a href="#Docker">Docker</a> instead of self-installing.<br>\nIf you are not using Docker, follow <a href="https://github.com/avilum/secimport/wiki/Installation">Installation</a> to install eBPF or DTrace.\n- To install secimport from git clone: `python3 -m pip install -e .`\n- To install secimport from pypi (latest stable release): `python3 -m pip install secimport`\n\n\n## Docker\nThe quickest way to evaluate `secimport` is to use our [Docker container](docker/README.md), which includes `bpftrace` (`ebpf`) and other plug-and-play examples.\n\n## Quick Start - Using the CLI\nTo run an end-to-end interactive example:\n1. Build a docker with custom kernel that matches your existing OS kernel version\n    ```\n    ➜  secimport ✗ cd docker/\n    ➜  docker ✗ ./build.sh\n    ```\n2. Run the container\n    ```\n    ➜  docker ✗ ./run.sh\n    Running temporary container...\n\n    root@f05d2c33b0b3:/workspace#\n    ```\n3. Use the CLI\n    ```\n    root@f05d2c33b0b3:/workspace# secimport interactive\n\n    Let\'s create our first tailor-made sandbox with secimport!\n    - A python shell will be opened\n    - The behavior will be recorded.\n\n    OK? (y): y\n    >>> secimport trace\n\n    TRACING: [\'/workspace/secimport/profiles/trace.bt\', \'-c\', \'/workspace/Python-3.10.0/python\', \'-o\', \'trace.log\']\n\n                            Press CTRL+D/CTRL+C to stop the trace;\n\n    Python 3.10.0 (default, Apr  9 2023, 17:19:17) [GCC 9.4.0] on linux\n    Type "help", "copyright", "credits" or "license" for more information.\n    >>> import ...\n\n\n    ```\n## Sandbox Your Program (Using the CLI)\n`secimport trace` will start a bpftrace program that will log all the syscalls for all the modules in your application into a file.<br>\nOnce you covered the logic you would like to or sandbox and you\'re satisfied, hit `CTRL+C` or `CTRL+D` or wait for the program to finish.\n```\n$ secimport trace\n$ secimport trace -h\n$ secimport trace_pid 123\n$ secimport trace_pid -h\n```\n\nThen, build a sandbox from the trace using the `build` command:\n```\n# secimport build\n$ secimport build -h\n```\n\nFinally, run the sandbox with the `run` command:\n```\n$ secimport run\n$ secimport run --entrypoint my_custom_main.py\n$ secimport run --entrypoint my_custom_main.py --stop_on_violation=true\n$ secimport run --entrypoint my_custom_main.py --kill_on_violation=true\n$ secimport run --sandbox_executable /path/to/my_sandbox.bt --pid 2884\n$ secimport run --sandbox_executable /path/to/my_sandbox.bt --sandbox_logfile my_log.log\n$ secimport run -h\n```\n\nFor more detailed usage instructions, see the [Command-Line Usage](https://github.com/avilum/secimport/wiki/Command-Line-Usage) page.\n\n## Python API\n\nYou can also use `secimport` by replacing `import` with `secimport.secure_import` for selected modules. See the [Python Imports](examples/python_imports/) example for more details.\n\n## Examples\n\nThe [Sandbox Examples](https://github.com/avilum/secimport/wiki/Sandbox-Examples) page contains basic and advanced real-world examples.\n\n## Contributing\n\nFor information on how to contribute to `secimport`, see the [Contributing](https://github.com/avilum/secimport/blob/master/docs/CONTRIBUTING.md) guide.\n\n## Roadmap\n\nSee the [Roadmap](https://github.com/avilum/secimport/blob/master/docs/ROADMAP.md) for the planned features and development milestones.\n\n## Changelog\n\nSee the [Changelog](https://github.com/avilum/secimport/blob/master/docs/CHANGELOG.md) for development progress and existing features.\n',
-    'author': 'Avi Lumelsky',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/avilum/secimport',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
+## Roadmap
 
+See the [Roadmap](https://github.com/avilum/secimport/blob/master/docs/ROADMAP.md) for the planned features and development milestones.
+
+## Changelog
+
+See the [Changelog](https://github.com/avilum/secimport/blob/master/docs/CHANGELOG.md) for development progress and existing features.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,71 +1,70 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['secimport',
-'secimport.backends.bpftrace_backend', 'secimport.backends.common',
-'secimport.backends.dtrace_backend'] package_data = \ {'': ['*'], 'secimport':
-['profiles/*'], 'secimport.backends.bpftrace_backend': ['actions/*', 'filters/
-*', 'probes/*'], 'secimport.backends.dtrace_backend': ['actions/*', 'filters/
-*', 'headers/*', 'probes/*']} install_requires = \ ['PyYAML>=6.0,<7.0',
-'fire>=0.4.0,<0.5.0'] entry_points = \ {'console_scripts': ['secimport =
-secimport.cli:main']} setup_kwargs = { 'name': 'secimport', 'version': '0.7.0',
-'description': 'A sandbox/supervisor for python modules.', 'long_description':
-'# secimport\n\n`secimport` is a cross-platform sandbox toolkit that traces
-your Python application and enforces privileges per module in your code in
-runtime. It uses backends like bpftrace (eBPF) and dtrace under the hood.\n\n##
-Why It\'s Awesome\n\n- Trace which syscalls are called by each module in your
-code.\n - `secimport` uses USDT (Userland Statically Defined Tracing) probes in
-the runtime (Python interpreter for example) using eBPF and dtrace
-instrumentation scripts.\n - Audit the flow of your application at user-space/
-os/kernel level\n- Reduce supply chain attack and RCE vectors by restricting
-modules/packages inside your production environment.\n- No performance impact
-(see [Performance](https://github.com/avilum/secimport/wiki/Performance-
-Benchmarks)).\n- Don\'t change the way you code!\n- Supports `Python` at the
-moment\n - `Go` is under development\n\n\n## Installation\nFor evaluation, we
-highly recommend the QuickStart with Docker instead of self-installing.
-\nIf you are not using Docker, follow Installation to install eBPF or
-DTrace.\n- To install secimport from git clone: `python3 -m pip install -
-e .`\n- To install secimport from pypi (latest stable release): `python3 -m pip
-install secimport`\n\n\n## Docker\nThe quickest way to evaluate `secimport` is
-to use our [Docker container](docker/README.md), which includes `bpftrace`
-(`ebpf`) and other plug-and-play examples.\n\n## Quick Start - Using the
-CLI\nTo run an end-to-end interactive example:\n1. Build a docker with custom
-kernel that matches your existing OS kernel version\n ```\n â secimport â
-cd docker/\n â docker â ./build.sh\n ```\n2. Run the container\n ```\n â
-docker â ./run.sh\n Running temporary container...\n\n root@f05d2c33b0b3:/
-workspace#\n ```\n3. Use the CLI\n ```\n root@f05d2c33b0b3:/workspace#
-secimport interactive\n\n Let\'s create our first tailor-made sandbox with
-secimport!\n - A python shell will be opened\n - The behavior will be
-recorded.\n\n OK? (y): y\n >>> secimport trace\n\n TRACING: [\'/workspace/
-secimport/profiles/trace.bt\', \'-c\', \'/workspace/Python-3.10.0/python\', \'-
-o\', \'trace.log\']\n\n Press CTRL+D/CTRL+C to stop the trace;\n\n Python
-3.10.0 (default, Apr 9 2023, 17:19:17) [GCC 9.4.0] on linux\n Type "help",
-"copyright", "credits" or "license" for more information.\n >>> import
-...\n\n\n ```\n## Sandbox Your Program (Using the CLI)\n`secimport trace` will
-start a bpftrace program that will log all the syscalls for all the modules in
-your application into a file.
-\nOnce you covered the logic you would like to or sandbox and you\'re
-satisfied, hit `CTRL+C` or `CTRL+D` or wait for the program to finish.\n```\n$
-secimport trace\n$ secimport trace -h\n$ secimport trace_pid 123\n$ secimport
-trace_pid -h\n```\n\nThen, build a sandbox from the trace using the `build`
-command:\n```\n# secimport build\n$ secimport build -h\n```\n\nFinally, run the
-sandbox with the `run` command:\n```\n$ secimport run\n$ secimport run --
-entrypoint my_custom_main.py\n$ secimport run --entrypoint my_custom_main.py --
-stop_on_violation=true\n$ secimport run --entrypoint my_custom_main.py --
-kill_on_violation=true\n$ secimport run --sandbox_executable /path/to/
-my_sandbox.bt --pid 2884\n$ secimport run --sandbox_executable /path/to/
-my_sandbox.bt --sandbox_logfile my_log.log\n$ secimport run -h\n```\n\nFor more
+Metadata-Version: 2.1 Name: secimport Version: 0.7.3 Summary: A sandbox/
+supervisor for python modules. Home-page: https://github.com/avilum/secimport
+License: MIT Author: Avi Lumelsky Requires-Python: >=3.6,<4.0 Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: fire
+(>=0.4.0,<0.5.0) Description-Content-Type: text/markdown # secimport
+`secimport` is a cross-platform sandbox toolkit that traces your Python
+application and enforces privileges per module in your code in runtime. It uses
+backends like bpftrace (eBPF) and dtrace under the hood. [![Upload Python
+Package](https://github.com/avilum/secimport/actions/workflows/python-
+publish.yml/badge.svg?branch=master)](https://github.com/avilum/secimport/
+actions/workflows/python-publish.yml) ## Why It's Awesome - Trace which
+syscalls are called by each module in your code. - `secimport` uses USDT
+(Userland Statically Defined Tracing) probes in the runtime (Python interpreter
+for example) using eBPF and dtrace instrumentation scripts. - Audit the flow of
+your application at user-space/os/kernel level - Reduce supply chain attack and
+RCE vectors by restricting modules/packages inside your production environment.
+- No performance impact (see [Performance](https://github.com/avilum/secimport/
+wiki/Performance-Benchmarks)). - Don't change the way you code! - Supports
+`Python` at the moment - `Go` is under development ## Installation For
+evaluation, we highly recommend the QuickStart with Docker instead of self-
+installing.
+If you are not using Docker, follow Installation to install eBPF or DTrace. -
+To install secimport from git clone: `python3 -m pip install -e .` - To install
+secimport from pypi (latest stable release): `python3 -m pip install secimport`
+## Docker The quickest way to evaluate `secimport` is to use our [Docker
+container](docker/README.md), which includes `bpftrace` (`ebpf`) and other
+plug-and-play examples. ## Quick Start - Using the CLI To run an end-to-end
+interactive example: 1. Build a docker with custom kernel that matches your
+existing OS kernel version ``` â secimport â cd docker/ â docker â ./
+build.sh ``` 2. Run the container ``` â docker â ./run.sh Running temporary
+container... root@f05d2c33b0b3:/workspace# ``` 3. Use the CLI ```
+root@f05d2c33b0b3:/workspace# secimport interactive Let's create our first
+tailor-made sandbox with secimport! - A python shell will be opened - The
+behavior will be recorded. OK? (y): y >>> secimport trace TRACING: ['/
+workspace/secimport/profiles/trace.bt', '-c', '/workspace/Python-3.10.0/
+python', '-o', 'trace.log'] Press CTRL+D/CTRL+C to stop the trace; Python
+3.10.0 (default, Apr 9 2023, 17:19:17) [GCC 9.4.0] on linux Type "help",
+"copyright", "credits" or "license" for more information. >>> import ... ``` ##
+Sandbox Your Program (Using the CLI) `secimport trace` will start a bpftrace
+program that will log all the syscalls for all the modules in your application
+into a file.
+Once you covered the logic you would like to or sandbox and you're satisfied,
+hit `CTRL+C` or `CTRL+D` or wait for the program to finish. ``` $ secimport
+trace $ secimport trace -h $ secimport trace_pid 123 $ secimport trace_pid -
+h ``` Then, build a sandbox from the trace using the `build` command: ``` #
+secimport build $ secimport build -h ``` Finally, run the sandbox with the
+`run` command: ``` $ secimport run $ secimport run --entrypoint
+my_custom_main.py $ secimport run --entrypoint my_custom_main.py --
+stop_on_violation=true $ secimport run --entrypoint my_custom_main.py --
+kill_on_violation=true $ secimport run --sandbox_executable /path/to/
+my_sandbox.bt --pid 2884 $ secimport run --sandbox_executable /path/to/
+my_sandbox.bt --sandbox_logfile my_log.log $ secimport run -h ``` For more
 detailed usage instructions, see the [Command-Line Usage](https://github.com/
-avilum/secimport/wiki/Command-Line-Usage) page.\n\n## Python API\n\nYou can
-also use `secimport` by replacing `import` with `secimport.secure_import` for
-selected modules. See the [Python Imports](examples/python_imports/) example
-for more details.\n\n## Examples\n\nThe [Sandbox Examples](https://github.com/
-avilum/secimport/wiki/Sandbox-Examples) page contains basic and advanced real-
-world examples.\n\n## Contributing\n\nFor information on how to contribute to
-`secimport`, see the [Contributing](https://github.com/avilum/secimport/blob/
-master/docs/CONTRIBUTING.md) guide.\n\n## Roadmap\n\nSee the [Roadmap](https://
-github.com/avilum/secimport/blob/master/docs/ROADMAP.md) for the planned
-features and development milestones.\n\n## Changelog\n\nSee the [Changelog]
-(https://github.com/avilum/secimport/blob/master/docs/CHANGELOG.md) for
-development progress and existing features.\n', 'author': 'Avi Lumelsky',
-'author_email': None, 'maintainer': None, 'maintainer_email': None, 'url':
-'https://github.com/avilum/secimport', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.6,<4.0', } setup(**setup_kwargs)
+avilum/secimport/wiki/Command-Line-Usage) page. ## Python API You can also use
+`secimport` by replacing `import` with `secimport.secure_import` for selected
+modules. See the [Python Imports](examples/python_imports/) example for more
+details. ## Examples The [Sandbox Examples](https://github.com/avilum/
+secimport/wiki/Sandbox-Examples) page contains basic and advanced real-world
+examples. ## Contributing For information on how to contribute to `secimport`,
+see the [Contributing](https://github.com/avilum/secimport/blob/master/docs/
+CONTRIBUTING.md) guide. ## Roadmap See the [Roadmap](https://github.com/avilum/
+secimport/blob/master/docs/ROADMAP.md) for the planned features and development
+milestones. ## Changelog See the [Changelog](https://github.com/avilum/
+secimport/blob/master/docs/CHANGELOG.md) for development progress and existing
+features.
```

