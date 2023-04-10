# Comparing `tmp/drclient-0.0.3.tar.gz` & `tmp/drclient-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drclient-0.0.3.tar", last modified: Thu Apr  6 21:58:03 2023, max compression
+gzip compressed data, was "drclient-0.0.4.tar", last modified: Mon Apr 10 07:14:01 2023, max compression
```

## Comparing `drclient-0.0.3.tar` & `drclient-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.692306 drclient-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.688306 drclient-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.692306 drclient-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-06 21:57:57.000000 drclient-0.0.3/.github/workflows/multi-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-06 21:57:57.000000 drclient-0.0.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-06 21:57:57.000000 drclient-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-06 21:57:57.000000 drclient-0.0.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.692306 drclient-0.0.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-06 21:57:57.000000 drclient-0.0.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-06 21:57:57.000000 drclient-0.0.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-06 21:57:57.000000 drclient-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-06 21:57:57.000000 drclient-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-06 21:58:03.692306 drclient-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-06 21:57:57.000000 drclient-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.692306 drclient-0.0.3/drclient/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.692306 drclient-0.0.3/drclient/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/cli/cmd_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/cli/cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/cli/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.692306 drclient-0.0.3/drclient/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/registry/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/registry/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/threaded_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-06 21:58:03.000000 drclient-0.0.3/drclient/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.692306 drclient-0.0.3/drclient/view/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/view/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/view/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-06 21:57:57.000000 drclient-0.0.3/drclient/view/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.692306 drclient-0.0.3/drclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-06 21:58:03.000000 drclient-0.0.3/drclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-06 21:58:03.000000 drclient-0.0.3/drclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 21:58:03.000000 drclient-0.0.3/drclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-06 21:58:03.000000 drclient-0.0.3/drclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-06 21:58:03.000000 drclient-0.0.3/drclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-06 21:58:03.000000 drclient-0.0.3/drclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-06 21:57:57.000000 drclient-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-06 21:57:57.000000 drclient-0.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-06 21:57:57.000000 drclient-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-06 21:58:03.692306 drclient-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-06 21:57:57.000000 drclient-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:58:03.692306 drclient-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-06 21:57:57.000000 drclient-0.0.3/tests/test_image_url.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-06 21:57:57.000000 drclient-0.0.3/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-06 21:57:57.000000 drclient-0.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.318467 drclient-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 07:13:51.000000 drclient-0.0.4/.github/workflows/multi-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-10 07:13:51.000000 drclient-0.0.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-10 07:13:51.000000 drclient-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 07:13:51.000000 drclient-0.0.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-10 07:13:51.000000 drclient-0.0.4/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-10 07:13:51.000000 drclient-0.0.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 07:13:51.000000 drclient-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 07:13:51.000000 drclient-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-10 07:14:01.322467 drclient-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-10 07:13:51.000000 drclient-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/cli/cmd_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/cli/cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/cli/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/registry/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/registry/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/threaded_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/view/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/view/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/view/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-10 07:13:51.000000 drclient-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 07:13:51.000000 drclient-0.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 07:13:51.000000 drclient-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-10 07:14:01.326467 drclient-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-10 07:13:51.000000 drclient-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 07:13:51.000000 drclient-0.0.4/tests/test_image_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-10 07:13:51.000000 drclient-0.0.4/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-10 07:13:51.000000 drclient-0.0.4/tox.ini
```

### Comparing `drclient-0.0.3/.github/workflows/multi-test.yaml` & `drclient-0.0.4/.github/workflows/multi-test.yaml`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/.github/workflows/release.yaml` & `drclient-0.0.4/.github/workflows/release.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -25,7 +25,17 @@
         run: python setup.py sdist bdist_wheel
 
       - name: Publish distribution 📦 to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@master
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
+  create-release:
+    runs-on: ubuntu-latest
+    permissions:
+      contents: write
+    steps:
+    - uses: actions/checkout@v3
+    - uses: ncipollo/release-action@v1
+      with:
+        artifacts: "release.tar.gz,foo/*.txt"
+        bodyFile: "body.md"
```

### Comparing `drclient-0.0.3/.gitignore` & `drclient-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/.pre-commit-config.yaml` & `drclient-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/LICENSE` & `drclient-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/PKG-INFO` & `drclient-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drclient
-Version: 0.0.3
+Version: 0.0.4
 Summary: A docker registry client command line utility and Python library
 Home-page: https://github.com/joaompinto/drclient
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drclient-0.0.3/README.md` & `drclient-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/drclient/cli/cmd_info.py` & `drclient-0.0.4/drclient/cli/cmd_info.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/drclient/cli/cmd_pull.py` & `drclient-0.0.4/drclient/cli/cmd_pull.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import atexit
 import os
 import shutil
 import tarfile
 from pathlib import Path
+from subprocess import getstatusoutput
 from tempfile import mkdtemp
 
 import typer
 
 from ..extract import extract_layers
 from ..registry import DockerRegistryClient
 from ..threaded_pull import pull_layers_in_threads
@@ -14,24 +15,24 @@
 
 
 def pull(
     image_name: str = typer.Argument(..., help="The name of the image"),
     tar_file: Path = typer.Option(
         None, "-t", "--tar-file", help="Output to a tar.gz file"
     ),
+    squafshfs_file: Path = typer.Option(
+        None, "-s", "--squashfs-file", help="Output to a .sqfs file"
+    ),
     output_directory: Path = typer.Option(
         None, "-d", "--output-directory", help="Output to a directory"
     ),
 ):
     """
     Pull image from a docker registry
     """
-    if tar_file and output_directory:
-        raise typer.BadParameter("Cannot specify both output file and output directory")
-
     registry, repository, tag = DockerRegistryClient.parse_image_url(image_name)
     source_reference = f"{registry}/{repository}:{tag}"
 
     drc = DockerRegistryClient(registry)
     drc.authenticate()
     manifest = drc.get_manifest(repository, tag)
     layers = manifest["layers"]
@@ -39,33 +40,48 @@
     total_size = sum([layer["size"] for layer in layers])
     print(
         f"Pulling {len(layers)} layer(s) [{sizeof_fmt(total_size)}] "
         f"for image {source_reference} to local image {local_image_name}"
     )
 
     if output_directory is None:
+        is_tmp_output_directory = True
         output_directory = mkdtemp()
         if tar_file:
             atexit.register(shutil.rmtree, output_directory)
     else:
+        is_tmp_output_directory = False
         if not output_directory.exists():
             output_directory.mkdir(parents=True)
         else:
             if not output_directory.is_dir():
                 raise typer.BadParameter(
                     f"Output directory {output_directory} is not a directory"
                 )
             os.scandir(output_directory)
             if any(os.scandir(output_directory)):
                 raise typer.BadParameter(
                     f"Output directory {output_directory} is not empty"
                 )
 
     pull_layers_in_threads(drc, layers, output_directory)
+    print("Extracting layers...", end="", flush=True)
     extract_layers(layers, Path(output_directory))
+    print("Done")
     if tar_file:
         os.chdir(output_directory)
         with tarfile.open(tar_file, "w:gz") as tar:
             tar.add(".", recursive=True)
-        os.chdir("/")
-    else:
+
+    if squafshfs_file:
+        if squafshfs_file.exists():
+            squafshfs_file.unlink()
+        print("Creating squashfs file...", end="", flush=True)
+        exit_code, output = getstatusoutput(
+            f"mksquashfs {output_directory} {squafshfs_file}"
+        )
+        if exit_code != 0:
+            raise typer.Exit(f"Failed to create squashfs file: {output}")
+        print("Done")
+
+    if not is_tmp_output_directory:
         print(f"Contents of {source_reference} extracted to {output_directory}")
```

### Comparing `drclient-0.0.3/drclient/extract.py` & `drclient-0.0.4/drclient/extract.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """ This module provides functions to extract contents from docker images """
 import tarfile
 from pathlib import Path
 
+tarfile.os.chown = (
+    lambda x, y, z: 0
+)  # Monkey patch chown because we don't care about ownership
+
 tarfile.os.mknod = (
     lambda x, y, z: 0
 )  # Monkey patch mknod because some layers include devices
 
 
 def extract_layers(layers: dict, directory: Path):
     """Extract the contents of the layers in the given directory to a tar.gz file"""
```

### Comparing `drclient-0.0.3/drclient/registry/registry.py` & `drclient-0.0.4/drclient/registry/registry.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/drclient/threaded_pull.py` & `drclient-0.0.4/drclient/threaded_pull.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/drclient/view/history.py` & `drclient-0.0.4/drclient/view/history.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/drclient/view/info.py` & `drclient-0.0.4/drclient/view/info.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/drclient.egg-info/PKG-INFO` & `drclient-0.0.4/drclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drclient
-Version: 0.0.3
+Version: 0.0.4
 Summary: A docker registry client command line utility and Python library
 Home-page: https://github.com/joaompinto/drclient
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drclient-0.0.3/drclient.egg-info/SOURCES.txt` & `drclient-0.0.4/drclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drclient-0.0.3/setup.py` & `drclient-0.0.4/setup.py`

 * *Files identical despite different names*

