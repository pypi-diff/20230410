# Comparing `tmp/rootbox-0.0.5.tar.gz` & `tmp/rootbox-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootbox-0.0.5.tar", last modified: Mon Apr 10 07:48:01 2023, max compression
+gzip compressed data, was "rootbox-0.0.6.tar", last modified: Mon Apr 10 19:38:28 2023, max compression
```

## Comparing `rootbox-0.0.5.tar` & `rootbox-0.0.6.tar`

### file list

```diff
@@ -1,55 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.240427 rootbox-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.232427 rootbox-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.236427 rootbox-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-10 07:47:55.000000 rootbox-0.0.5/.github/workflows/multi-test.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-10 07:47:55.000000 rootbox-0.0.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-04-10 07:47:55.000000 rootbox-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-04-10 07:47:55.000000 rootbox-0.0.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.236427 rootbox-0.0.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-10 07:47:55.000000 rootbox-0.0.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-04-10 07:47:55.000000 rootbox-0.0.5/CREDITS.md
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-10 07:47:55.000000 rootbox-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-10 07:47:55.000000 rootbox-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-10 07:48:01.240427 rootbox-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-04-10 07:47:55.000000 rootbox-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.236427 rootbox-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-10 07:47:55.000000 rootbox-0.0.5/docs/LXC.md
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-10 07:47:55.000000 rootbox-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-04-10 07:47:55.000000 rootbox-0.0.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-10 07:47:55.000000 rootbox-0.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.236427 rootbox-0.0.5/rootbox/
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.240427 rootbox-0.0.5/rootbox/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/cli/cmd_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/cli/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/cli/cmd_lxc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/cli/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/cli/verbose.py
--rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/colorhelper.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/download.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/enter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/lxc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/mount.py
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/process.py
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/rootfs.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/size.py
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/tar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/unshare.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-10 07:47:55.000000 rootbox-0.0.5/rootbox/verbose.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-10 07:48:01.000000 rootbox-0.0.5/rootbox/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.240427 rootbox-0.0.5/rootbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-10 07:48:01.000000 rootbox-0.0.5/rootbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-04-10 07:48:01.000000 rootbox-0.0.5/rootbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 07:48:01.000000 rootbox-0.0.5/rootbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-10 07:48:01.000000 rootbox-0.0.5/rootbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-10 07:48:01.000000 rootbox-0.0.5/rootbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-10 07:48:01.000000 rootbox-0.0.5/rootbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.240427 rootbox-0.0.5/samples/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-04-10 07:47:55.000000 rootbox-0.0.5/samples/test.py
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-10 07:48:01.240427 rootbox-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-10 07:47:55.000000 rootbox-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 07:48:01.240427 rootbox-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-10 07:47:55.000000 rootbox-0.0.5/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-10 07:47:55.000000 rootbox-0.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.030635 rootbox-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.034635 rootbox-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-10 19:38:20.000000 rootbox-0.0.6/.github/workflows/multi-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-10 19:38:20.000000 rootbox-0.0.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-04-10 19:38:20.000000 rootbox-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-04-10 19:38:20.000000 rootbox-0.0.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.034635 rootbox-0.0.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-10 19:38:20.000000 rootbox-0.0.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-04-10 19:38:20.000000 rootbox-0.0.6/CREDITS.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-10 19:38:20.000000 rootbox-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-10 19:38:20.000000 rootbox-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-04-10 19:38:28.042636 rootbox-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-10 19:38:20.000000 rootbox-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.034635 rootbox-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-10 19:38:20.000000 rootbox-0.0.6/docs/LXC.md
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-10 19:38:20.000000 rootbox-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-04-10 19:38:20.000000 rootbox-0.0.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-10 19:38:20.000000 rootbox-0.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.038636 rootbox-0.0.6/rootbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/rootbox/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_lxc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/colorhelper.py
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/enter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/rootbox/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/images/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/images/lxc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/images_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/mount.py
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/size.py
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/socket.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/tar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/unshare.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/rootbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-04-10 19:38:28.000000 rootbox-0.0.6/rootbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/samples/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-04-10 19:38:20.000000 rootbox-0.0.6/samples/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-10 19:38:28.046635 rootbox-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-10 19:38:20.000000 rootbox-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-04-10 19:38:20.000000 rootbox-0.0.6/tests/test_cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-10 19:38:20.000000 rootbox-0.0.6/tests/test_image_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-10 19:38:20.000000 rootbox-0.0.6/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-10 19:38:20.000000 rootbox-0.0.6/tox.ini
```

### Comparing `rootbox-0.0.5/.github/workflows/multi-test.yaml` & `rootbox-0.0.6/.github/workflows/multi-test.yaml`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/.github/workflows/release.yaml` & `rootbox-0.0.6/.github/workflows/release.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
       - name: Publish distribution 📦 to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@master
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
 
+  # https://github.com/marketplace/actions/create-release
   create-release:
     runs-on: ubuntu-latest
     permissions:
       contents: write
     steps:
     - uses: actions/checkout@v3
     - uses: ncipollo/release-action@v1
```

### Comparing `rootbox-0.0.5/.gitignore` & `rootbox-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/.pre-commit-config.yaml` & `rootbox-0.0.6/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -35,7 +35,17 @@
     - id: black
 
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
     rev: 'v0.0.259'
     hooks:
     - id: ruff
+
+# - repo: local
+#   hooks:
+#     -   id: tox-on-python3.8
+#         name: Run tox in Python 3.8 using rootbox
+#         entry:
+#             python -m rootbox run docker:python:3.8-alpine
+#              "apk add git && pip install tox && tox"
+#         language: system
+#         pass_filenames: false
```

### Comparing `rootbox-0.0.5/LICENSE` & `rootbox-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/PKG-INFO` & `rootbox-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 Metadata-Version: 2.1
 Name: rootbox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Portable reproducible environments for Linux applications
 Home-page: https://github.com/joaompinto/rootbox
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rootbox
 
 [![PyPi](https://img.shields.io/pypi/v/rootbox.svg?style=flat-square)](https://pypi.python.org/pypi/rootbox)
-![License](https://img.shields.io/github/license/0x0I/rootbox?style=flat-square)
+![License](https://img.shields.io/github/license/joaompinto/rootbox?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## What is rootbox?
 
 Rootbox is a tool for Linux and WSL that allows regular (unprivileged) users to deploy applications in a portable and reproducible way.
 
 ## How does it work
 Rootbox uses Linux kernel namespaces to create contained environments.
 
 ## What is the difference between rootbox and Docker?
-The focus of rootbox is to provide a tool that can be used to run applications without the need to install dependencies on the host system.
-
- > rootbox does **NOT** aim to provide full isolation between environemtns and the host, for such use cases please consider using Docker or Podman.
+The focus of rootbox is to provide a tool that can be used to run applications without the need to install dependencies on the host system. Rootbox does **NOT** aim to provide full isolation between environemtns and the host, for such use cases please consider using Docker or Podman.
 
 ## What is nedded to run rootbox?
-
 - A Linux distrubtion or Linux on Windows with WSL (Kernel version >=4.18)
 - Python 3.8, 3.9, 3.10 or 3.11
 - Only 64-bit architectures are supported
 
-
-
 ## What applications can I run with rootbox?
 
 - images from the Linux Containers project ([LXC](https://https://images.linuxcontainers.org/)).
 - images from the Docker Hub registry ([Docker Hub](https://hub.docker.com/))
 
 ## Supported package managers
 
 | Status | Tool | Distros |
 |:------:|------|---------|
 |✅|apk|Alpine|
 |✅|pacman|ArchLinux|
 |✅|dnf|Alma; CentOS; Fedora; Rocky|
-|✅|xpbs|VoidLinux|
+|✅|xbps|VoidLinux|
 |✅|zypper|openSUSE|
 |❌|apt|Debian/Ubuntu|
 
 ## How to install
 ```sh
 pip install rootbox
 ```
@@ -62,22 +57,22 @@
 # Check the list of supported distro names in the table above
 rootbox lxc list
 ```
 
 ### Run an in-memory single run container
 Run a shell in an Alpine Linux container
 ```sh
-rootbox run alpine:3.17
+rootbox run lxc:alpine:3.17
 ```
 Check the apk version:
 ```sh
-rootbox run alpine:3.17 "apk --version"
+rootbox run lxc:alpine:3.17 "apk --version"
 ```
 
 ### Create an in-memory multi run container
 ```sh
-rootbox create alpine:3.17
+rootbox create lxc:alpine:3.17
 ```
 ### Execute a command in a container
 ```sh
-rootbox execute alpine:3.17 "apk --version"
+rootbox execute lxc:alpine:3.17 "apk --version"
 ```
```

### Comparing `rootbox-0.0.5/README.md` & `rootbox-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 # rootbox
 
 [![PyPi](https://img.shields.io/pypi/v/rootbox.svg?style=flat-square)](https://pypi.python.org/pypi/rootbox)
-![License](https://img.shields.io/github/license/0x0I/rootbox?style=flat-square)
+![License](https://img.shields.io/github/license/joaompinto/rootbox?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## What is rootbox?
 
 Rootbox is a tool for Linux and WSL that allows regular (unprivileged) users to deploy applications in a portable and reproducible way.
 
 ## How does it work
 Rootbox uses Linux kernel namespaces to create contained environments.
 
 ## What is the difference between rootbox and Docker?
-The focus of rootbox is to provide a tool that can be used to run applications without the need to install dependencies on the host system.
-
- > rootbox does **NOT** aim to provide full isolation between environemtns and the host, for such use cases please consider using Docker or Podman.
+The focus of rootbox is to provide a tool that can be used to run applications without the need to install dependencies on the host system. Rootbox does **NOT** aim to provide full isolation between environemtns and the host, for such use cases please consider using Docker or Podman.
 
 ## What is nedded to run rootbox?
-
 - A Linux distrubtion or Linux on Windows with WSL (Kernel version >=4.18)
 - Python 3.8, 3.9, 3.10 or 3.11
 - Only 64-bit architectures are supported
 
-
-
 ## What applications can I run with rootbox?
 
 - images from the Linux Containers project ([LXC](https://https://images.linuxcontainers.org/)).
 - images from the Docker Hub registry ([Docker Hub](https://hub.docker.com/))
 
 ## Supported package managers
 
 | Status | Tool | Distros |
 |:------:|------|---------|
 |✅|apk|Alpine|
 |✅|pacman|ArchLinux|
 |✅|dnf|Alma; CentOS; Fedora; Rocky|
-|✅|xpbs|VoidLinux|
+|✅|xbps|VoidLinux|
 |✅|zypper|openSUSE|
 |❌|apt|Debian/Ubuntu|
 
 ## How to install
 ```sh
 pip install rootbox
 ```
@@ -51,22 +46,22 @@
 # Check the list of supported distro names in the table above
 rootbox lxc list
 ```
 
 ### Run an in-memory single run container
 Run a shell in an Alpine Linux container
 ```sh
-rootbox run alpine:3.17
+rootbox run lxc:alpine:3.17
 ```
 Check the apk version:
 ```sh
-rootbox run alpine:3.17 "apk --version"
+rootbox run lxc:alpine:3.17 "apk --version"
 ```
 
 ### Create an in-memory multi run container
 ```sh
-rootbox create alpine:3.17
+rootbox create lxc:alpine:3.17
 ```
 ### Execute a command in a container
 ```sh
-rootbox execute alpine:3.17 "apk --version"
+rootbox execute lxc:alpine:3.17 "apk --version"
 ```
```

### Comparing `rootbox-0.0.5/docs/LXC.md` & `rootbox-0.0.6/docs/LXC.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 The images are obtained from: https://images.linuxcontainers.org/images
 
 The url to download the images is const5ructed from the index using the following template:
 
 ```python
 # Python snippet
 LXC_URL_TEMPL = 'https://images.linuxcontainers.org/images/{}/{}/{}/{}/{}/rootfs.tar.xz'
-url = LXC_URL_TEMPL.format(distro_name, distro_version, distro_arch, distro_variant, distro_build)
+url = LXC_URL_TEMPL.format(image_name, distro_version, distro_arch, distro_variant, distro_build)
 ```
```

### Comparing `rootbox-0.0.5/rootbox/__main__.py` & `rootbox-0.0.6/rootbox/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import typer
 
-from .cli import cmd_create, cmd_exec, cmd_lxc, cmd_run, verbose
+from .cli import cmd_create, cmd_exec, cmd_lxc, cmd_pull, cmd_run, verbose
 
 
 def main():
     app = typer.Typer(short_help="Utility to manage a pypy.org metadata cache")
 
     app.command(help="Create a container instance")(cmd_create.create)
     app.command(help="Execute a command in an existing instance")(cmd_exec.exec)
+    app.command(help="Pull an image into the local cache")(cmd_pull.pull)
     app.command(help="Run a command in an ephemeral instance")(cmd_run.run)
     app.add_typer(
         cmd_lxc.app, name="lxc", help="Get information about available LCX images"
     )
 
     app.callback()(verbose.verbose)
     app()
```

### Comparing `rootbox-0.0.5/rootbox/colorhelper.py` & `rootbox-0.0.6/rootbox/colorhelper.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/rootbox/enter.py` & `rootbox-0.0.6/rootbox/enter.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/rootbox/mount.py` & `rootbox-0.0.6/rootbox/mount.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/rootbox/process.py` & `rootbox-0.0.6/rootbox/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     sock.listen(1)
     conn, _ = sock.accept()
 
     message = conn.recv(1024).decode("utf-8")
     if message != "setup":
         raise Exception(f"Unexpected message from parent process: {message}")
     verbose(f"Received message from parent process: {message}")
-    mount_dir = prepare_rootfs(tar_fname, in_memory=True)
+    mount_dir = prepare_rootfs(tar_fname, in_memory=True, perform_chroot=False)
     conn.sendall(b"ok")
     conn.close()
 
     while True:
         conn, _ = sock.accept()
         message = conn.recv(1024).decode("utf-8")
         if message == "info":
```

### Comparing `rootbox-0.0.5/rootbox/size.py` & `rootbox-0.0.6/rootbox/size.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/rootbox/socket.py` & `rootbox-0.0.6/rootbox/socket.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/rootbox/unshare.py` & `rootbox-0.0.6/rootbox/unshare.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/rootbox.egg-info/PKG-INFO` & `rootbox-0.0.6/rootbox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 Metadata-Version: 2.1
 Name: rootbox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Portable reproducible environments for Linux applications
 Home-page: https://github.com/joaompinto/rootbox
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rootbox
 
 [![PyPi](https://img.shields.io/pypi/v/rootbox.svg?style=flat-square)](https://pypi.python.org/pypi/rootbox)
-![License](https://img.shields.io/github/license/0x0I/rootbox?style=flat-square)
+![License](https://img.shields.io/github/license/joaompinto/rootbox?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## What is rootbox?
 
 Rootbox is a tool for Linux and WSL that allows regular (unprivileged) users to deploy applications in a portable and reproducible way.
 
 ## How does it work
 Rootbox uses Linux kernel namespaces to create contained environments.
 
 ## What is the difference between rootbox and Docker?
-The focus of rootbox is to provide a tool that can be used to run applications without the need to install dependencies on the host system.
-
- > rootbox does **NOT** aim to provide full isolation between environemtns and the host, for such use cases please consider using Docker or Podman.
+The focus of rootbox is to provide a tool that can be used to run applications without the need to install dependencies on the host system. Rootbox does **NOT** aim to provide full isolation between environemtns and the host, for such use cases please consider using Docker or Podman.
 
 ## What is nedded to run rootbox?
-
 - A Linux distrubtion or Linux on Windows with WSL (Kernel version >=4.18)
 - Python 3.8, 3.9, 3.10 or 3.11
 - Only 64-bit architectures are supported
 
-
-
 ## What applications can I run with rootbox?
 
 - images from the Linux Containers project ([LXC](https://https://images.linuxcontainers.org/)).
 - images from the Docker Hub registry ([Docker Hub](https://hub.docker.com/))
 
 ## Supported package managers
 
 | Status | Tool | Distros |
 |:------:|------|---------|
 |✅|apk|Alpine|
 |✅|pacman|ArchLinux|
 |✅|dnf|Alma; CentOS; Fedora; Rocky|
-|✅|xpbs|VoidLinux|
+|✅|xbps|VoidLinux|
 |✅|zypper|openSUSE|
 |❌|apt|Debian/Ubuntu|
 
 ## How to install
 ```sh
 pip install rootbox
 ```
@@ -62,22 +57,22 @@
 # Check the list of supported distro names in the table above
 rootbox lxc list
 ```
 
 ### Run an in-memory single run container
 Run a shell in an Alpine Linux container
 ```sh
-rootbox run alpine:3.17
+rootbox run lxc:alpine:3.17
 ```
 Check the apk version:
 ```sh
-rootbox run alpine:3.17 "apk --version"
+rootbox run lxc:alpine:3.17 "apk --version"
 ```
 
 ### Create an in-memory multi run container
 ```sh
-rootbox create alpine:3.17
+rootbox create lxc:alpine:3.17
 ```
 ### Execute a command in a container
 ```sh
-rootbox execute alpine:3.17 "apk --version"
+rootbox execute lxc:alpine:3.17 "apk --version"
 ```
```

### Comparing `rootbox-0.0.5/rootbox.egg-info/SOURCES.txt` & `rootbox-0.0.6/rootbox.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 tox.ini
 .github/workflows/multi-test.yaml
 .github/workflows/release.yaml
 .vscode/settings.json
 docs/LXC.md
 rootbox/__main__.py
 rootbox/colorhelper.py
-rootbox/docker.py
 rootbox/download.py
 rootbox/enter.py
-rootbox/lxc.py
+rootbox/http.py
+rootbox/images_cache.py
 rootbox/mount.py
+rootbox/path.py
 rootbox/process.py
 rootbox/rootfs.py
 rootbox/size.py
 rootbox/socket.py
 rootbox/tar.py
 rootbox/unshare.py
 rootbox/verbose.py
@@ -34,11 +35,17 @@
 rootbox.egg-info/dependency_links.txt
 rootbox.egg-info/entry_points.txt
 rootbox.egg-info/requires.txt
 rootbox.egg-info/top_level.txt
 rootbox/cli/cmd_create.py
 rootbox/cli/cmd_exec.py
 rootbox/cli/cmd_lxc.py
+rootbox/cli/cmd_pull.py
 rootbox/cli/cmd_run.py
 rootbox/cli/verbose.py
+rootbox/images/__init__.py
+rootbox/images/docker.py
+rootbox/images/lxc.py
 samples/test.py
+tests/test_cmd_pull.py
+tests/test_image_url.py
 tests/test_version.py
```

### Comparing `rootbox-0.0.5/samples/test.py` & `rootbox-0.0.6/samples/test.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.5/setup.py` & `rootbox-0.0.6/setup.py`

 * *Files identical despite different names*

