# Comparing `tmp/drclient-0.0.4.tar.gz` & `tmp/drclient-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drclient-0.0.4.tar", last modified: Mon Apr 10 07:14:01 2023, max compression
+gzip compressed data, was "drclient-0.0.5.tar", last modified: Mon Apr 10 15:01:24 2023, max compression
```

## Comparing `drclient-0.0.4.tar` & `drclient-0.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.318467 drclient-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 07:13:51.000000 drclient-0.0.4/.github/workflows/multi-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-10 07:13:51.000000 drclient-0.0.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-10 07:13:51.000000 drclient-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 07:13:51.000000 drclient-0.0.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-10 07:13:51.000000 drclient-0.0.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-10 07:13:51.000000 drclient-0.0.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 07:13:51.000000 drclient-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 07:13:51.000000 drclient-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-10 07:14:01.322467 drclient-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-10 07:13:51.000000 drclient-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/cli/cmd_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/cli/cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/cli/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/registry/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/registry/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/threaded_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient/view/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/view/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/view/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-10 07:13:51.000000 drclient-0.0.4/drclient/view/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/drclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 07:14:01.000000 drclient-0.0.4/drclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-10 07:13:51.000000 drclient-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 07:13:51.000000 drclient-0.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 07:13:51.000000 drclient-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-10 07:14:01.326467 drclient-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-10 07:13:51.000000 drclient-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:14:01.322467 drclient-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 07:13:51.000000 drclient-0.0.4/tests/test_image_url.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-10 07:13:51.000000 drclient-0.0.4/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-10 07:13:51.000000 drclient-0.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.530635 drclient-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.538635 drclient-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 15:01:16.000000 drclient-0.0.5/.github/workflows/multi-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 15:01:16.000000 drclient-0.0.5/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-10 15:01:16.000000 drclient-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 15:01:16.000000 drclient-0.0.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.538635 drclient-0.0.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-10 15:01:16.000000 drclient-0.0.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-10 15:01:16.000000 drclient-0.0.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 15:01:16.000000 drclient-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 15:01:16.000000 drclient-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-10 15:01:24.542635 drclient-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-10 15:01:16.000000 drclient-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.538635 drclient-0.0.5/drclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/drclient/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/cli/cmd_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/cli/cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/cli/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/drclient/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/registry/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/registry/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/threaded_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/drclient/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/view/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/view/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/view/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.538635 drclient-0.0.5/drclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-10 15:01:16.000000 drclient-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 15:01:16.000000 drclient-0.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 15:01:16.000000 drclient-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-10 15:01:24.542635 drclient-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-10 15:01:16.000000 drclient-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 15:01:16.000000 drclient-0.0.5/tests/test_image_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-10 15:01:16.000000 drclient-0.0.5/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-10 15:01:16.000000 drclient-0.0.5/tox.ini
```

### Comparing `drclient-0.0.4/.github/workflows/multi-test.yaml` & `drclient-0.0.5/.github/workflows/multi-test.yaml`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/.github/workflows/release.yaml` & `drclient-0.0.5/.github/workflows/release.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,17 @@
         run: python setup.py sdist bdist_wheel
 
       - name: Publish distribution 📦 to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@master
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
+
   create-release:
     runs-on: ubuntu-latest
     permissions:
       contents: write
     steps:
     - uses: actions/checkout@v3
     - uses: ncipollo/release-action@v1
       with:
-        artifacts: "release.tar.gz,foo/*.txt"
-        bodyFile: "body.md"
+        generateReleaseNotes: true
```

### Comparing `drclient-0.0.4/.gitignore` & `drclient-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/.pre-commit-config.yaml` & `drclient-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/LICENSE` & `drclient-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/PKG-INFO` & `drclient-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drclient
-Version: 0.0.4
+Version: 0.0.5
 Summary: A docker registry client command line utility and Python library
 Home-page: https://github.com/joaompinto/drclient
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drclient-0.0.4/README.md` & `drclient-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/drclient/cli/cmd_info.py` & `drclient-0.0.5/drclient/cli/cmd_info.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/drclient/cli/cmd_pull.py` & `drclient-0.0.5/drclient/cli/cmd_pull.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     output_directory: Path = typer.Option(
         None, "-d", "--output-directory", help="Output to a directory"
     ),
 ):
     """
     Pull image from a docker registry
     """
+    is_tmp_output_directory = False
     registry, repository, tag = DockerRegistryClient.parse_image_url(image_name)
     source_reference = f"{registry}/{repository}:{tag}"
 
     drc = DockerRegistryClient(registry)
     drc.authenticate()
     manifest = drc.get_manifest(repository, tag)
     layers = manifest["layers"]
@@ -40,20 +41,19 @@
     total_size = sum([layer["size"] for layer in layers])
     print(
         f"Pulling {len(layers)} layer(s) [{sizeof_fmt(total_size)}] "
         f"for image {source_reference} to local image {local_image_name}"
     )
 
     if output_directory is None:
-        is_tmp_output_directory = True
         output_directory = mkdtemp()
-        if tar_file:
+        if tar_file or squafshfs_file:
+            is_tmp_output_directory = True
             atexit.register(shutil.rmtree, output_directory)
     else:
-        is_tmp_output_directory = False
         if not output_directory.exists():
             output_directory.mkdir(parents=True)
         else:
             if not output_directory.is_dir():
                 raise typer.BadParameter(
                     f"Output directory {output_directory} is not a directory"
                 )
@@ -64,17 +64,19 @@
                 )
 
     pull_layers_in_threads(drc, layers, output_directory)
     print("Extracting layers...", end="", flush=True)
     extract_layers(layers, Path(output_directory))
     print("Done")
     if tar_file:
+        cwd = os.getcwd()
         os.chdir(output_directory)
         with tarfile.open(tar_file, "w:gz") as tar:
-            tar.add(".", recursive=True)
+            tar.add(".", arcname="", recursive=True)
+        os.chdir(cwd)
 
     if squafshfs_file:
         if squafshfs_file.exists():
             squafshfs_file.unlink()
         print("Creating squashfs file...", end="", flush=True)
         exit_code, output = getstatusoutput(
             f"mksquashfs {output_directory} {squafshfs_file}"
```

### Comparing `drclient-0.0.4/drclient/extract.py` & `drclient-0.0.5/drclient/extract.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/drclient/registry/registry.py` & `drclient-0.0.5/drclient/registry/registry.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/drclient/threaded_pull.py` & `drclient-0.0.5/drclient/threaded_pull.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/drclient/view/history.py` & `drclient-0.0.5/drclient/view/history.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/drclient/view/info.py` & `drclient-0.0.5/drclient/view/info.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/drclient.egg-info/PKG-INFO` & `drclient-0.0.5/drclient.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drclient
-Version: 0.0.4
+Version: 0.0.5
 Summary: A docker registry client command line utility and Python library
 Home-page: https://github.com/joaompinto/drclient
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drclient-0.0.4/drclient.egg-info/SOURCES.txt` & `drclient-0.0.5/drclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drclient-0.0.4/setup.py` & `drclient-0.0.5/setup.py`

 * *Files identical despite different names*

