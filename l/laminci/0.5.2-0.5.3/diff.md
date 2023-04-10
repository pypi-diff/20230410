# Comparing `tmp/laminci-0.5.2.tar.gz` & `tmp/laminci-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.5.2.tar", last modified: Mon Apr 10 14:12:28 2023, max compression
+gzip compressed data, was "laminci-0.5.3.tar", last modified: Mon Apr 10 14:59:34 2023, max compression
```

## Comparing `laminci-0.5.2.tar` & `laminci-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.5.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.5.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.5.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.5.2/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.5.2/README.md
--rw-r--r--   0        0        0     2711 2023-04-10 14:12:08.068757 laminci-0.5.2/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.5.2/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-02-23 20:46:33.157438 laminci-0.5.2/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.5.2/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.5.2/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.5.2/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.5.2/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-04-10 14:12:03.248788 laminci-0.5.2/laminci/__init__.py
--rw-r--r--   0        0        0     1283 2023-04-10 14:11:31.171863 laminci-0.5.2/laminci/_artifacts.py
--rw-r--r--   0        0        0     1794 2023-03-25 16:54:29.619400 laminci-0.5.2/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.5.2/laminci/_docs.py
--rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.5.2/laminci/_env.py
--rw-r--r--   0        0        0     2423 2023-04-10 13:41:42.840205 laminci-0.5.2/laminci/_nox.py
--rw-r--r--   0        0        0      134 2023-02-23 21:55:02.625676 laminci-0.5.2/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.5.2/laminci/nox.py
--rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.5.2/noxfile.py
--rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       27 2023-02-23 21:02:08.742721 laminci-0.5.2/tests/test_base.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.5.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.5.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.5.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.5.3/README.md
+-rw-r--r--   0        0        0     2711 2023-04-10 14:59:15.965346 laminci-0.5.3/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.5.3/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-02-23 20:46:33.157438 laminci-0.5.3/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.5.3/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.5.3/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.5.3/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.5.3/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-04-10 14:59:01.991275 laminci-0.5.3/laminci/__init__.py
+-rw-r--r--   0        0        0     1413 2023-04-10 14:58:46.731399 laminci-0.5.3/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1794 2023-03-25 16:54:29.619400 laminci-0.5.3/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.5.3/laminci/_docs.py
+-rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.5.3/laminci/_env.py
+-rw-r--r--   0        0        0     2423 2023-04-10 13:41:42.840205 laminci-0.5.3/laminci/_nox.py
+-rw-r--r--   0        0        0      134 2023-02-23 21:55:02.625676 laminci-0.5.3/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.5.3/laminci/nox.py
+-rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.5.3/noxfile.py
+-rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-02-23 21:02:08.742721 laminci-0.5.3/tests/test_base.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.5.3/PKG-INFO
```

### Comparing `laminci-0.5.2/.github/workflows/build.yml` & `laminci-0.5.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.5.2/.github/workflows/latest-changes.yml` & `laminci-0.5.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.5.2/.gitignore` & `laminci-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.5.2/.pre-commit-config.yaml` & `laminci-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.5.2/docs/changelog.md` & `laminci-0.5.3/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🚸 Close current instance before uploading docs artifacts | [17](https://github.com/laminlabs/laminci/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.2
+🚸 Close current instance before uploading docs artifacts | [17](https://github.com/laminlabs/laminci/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.3
 🚸 Add support for environments | [16](https://github.com/laminlabs/laminci/pull/16) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.1
 ⬆️ Upgrade to new replace API | [15](https://github.com/laminlabs/laminci/pull/15) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.0
 ♻️ Replace `lndb` with `lamin` | [14](https://github.com/laminlabs/laminci/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-03-29 | 0.4.2
 🚸 Replace git checkout with git switch | [13](https://github.com/laminlabs/laminci/pull/13) | [falexwolf](https://github.com/falexwolf) | 2023-03-27 | 0.4.1
 ⬆️ Upgrade to LaminDB v0.35 | [12](https://github.com/laminlabs/laminci/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-03-26 | 0.4.0
 🚚 Rename `upload_docs_dir` to `upload_docs_artifact` |  | 2023-03-21 | 0.3.4
 🍱 Track images in docs | [11](https://github.com/laminlabs/laminci/pull/11) | [falexwolf](https://github.com/falexwolf) | 2023-03-12 | 0.3.2
```

### Comparing `laminci-0.5.2/docs/guide/quickstart.ipynb` & `laminci-0.5.3/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.5.2/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.5.3/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.5.2/laminci/_artifacts.py` & `laminci-0.5.3/laminci/_artifacts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 from pathlib import Path
 from zipfile import ZipFile
 
-import lndb
 from lamin_logger import logger
 
 from ._env import get_package_name
 
 
 def zip_docs_dir(zip_filename: str) -> None:
     with ZipFile(zip_filename, "w") as zf:
@@ -15,15 +14,20 @@
             if ".ipynb_checkpoints" in str(f):
                 continue
             if f.suffix in {".md", ".ipynb", ".png", ".jpg", ".svg"}:
                 zf.write(f, f.relative_to("./docs"))  # add at root level
 
 
 def upload_docs_artifact() -> None:
+    # this is super ugly but necessary right now
+    # we might need to close the current instance as it might be corrupted
+    import lndb
+
     lndb.close()
+
     import lamindb as ln
 
     if "GITHUB_EVENT_NAME" in os.environ and os.environ["GITHUB_EVENT_NAME"] != "push":
         logger.info("Only upload docs artifact for push event.")
         return None
     package_name = get_package_name()
     zip_filename = f"{package_name}_docs.zip"
```

### Comparing `laminci-0.5.2/laminci/_db.py` & `laminci-0.5.3/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.5.2/laminci/_env.py` & `laminci-0.5.3/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.5.2/laminci/_nox.py` & `laminci-0.5.3/laminci/_nox.py`

 * *Files identical despite different names*

### Comparing `laminci-0.5.2/pyproject.toml` & `laminci-0.5.3/pyproject.toml`

 * *Files identical despite different names*

