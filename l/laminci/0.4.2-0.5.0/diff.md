# Comparing `tmp/laminci-0.4.2.tar.gz` & `tmp/laminci-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.4.2.tar", last modified: Wed Mar 29 20:03:51 2023, max compression
+gzip compressed data, was "laminci-0.5.0.tar", last modified: Mon Apr 10 13:29:47 2023, max compression
```

## Comparing `laminci-0.4.2.tar` & `laminci-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.4.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.4.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.4.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.4.2/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.4.2/README.md
--rw-r--r--   0        0        0     2229 2023-03-29 20:03:32.064730 laminci-0.4.2/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.4.2/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-02-23 20:46:33.157438 laminci-0.4.2/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.4.2/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.4.2/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.4.2/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.4.2/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-03-29 20:03:25.012545 laminci-0.4.2/laminci/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-26 17:43:55.264065 laminci-0.4.2/laminci/_artifacts.py
--rw-r--r--   0        0        0     1794 2023-03-25 16:54:29.619400 laminci-0.4.2/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.4.2/laminci/_docs.py
--rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.4.2/laminci/_env.py
--rw-r--r--   0        0        0     2258 2023-03-29 20:02:50.066680 laminci-0.4.2/laminci/_nox.py
--rw-r--r--   0        0        0      134 2023-02-23 21:55:02.625676 laminci-0.4.2/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.4.2/laminci/nox.py
--rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.4.2/noxfile.py
--rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.4.2/pyproject.toml
--rw-r--r--   0        0        0       27 2023-02-23 21:02:08.742721 laminci-0.4.2/tests/test_base.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.5.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.5.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.5.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.5.0/README.md
+-rw-r--r--   0        0        0     2381 2023-04-10 13:29:15.652653 laminci-0.5.0/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.5.0/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-02-23 20:46:33.157438 laminci-0.5.0/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.5.0/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.5.0/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.5.0/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.5.0/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-04-10 13:29:05.870814 laminci-0.5.0/laminci/__init__.py
+-rw-r--r--   0        0        0     1254 2023-04-10 13:28:24.635403 laminci-0.5.0/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1794 2023-03-25 16:54:29.619400 laminci-0.5.0/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.5.0/laminci/_docs.py
+-rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.5.0/laminci/_env.py
+-rw-r--r--   0        0        0     2258 2023-03-29 20:02:50.066680 laminci-0.5.0/laminci/_nox.py
+-rw-r--r--   0        0        0      134 2023-02-23 21:55:02.625676 laminci-0.5.0/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.5.0/laminci/nox.py
+-rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.5.0/noxfile.py
+-rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-02-23 21:02:08.742721 laminci-0.5.0/tests/test_base.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.5.0/PKG-INFO
```

### Comparing `laminci-0.4.2/.github/workflows/build.yml` & `laminci-0.5.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.4.2/.github/workflows/latest-changes.yml` & `laminci-0.5.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.4.2/.gitignore` & `laminci-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.4.2/.pre-commit-config.yaml` & `laminci-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.4.2/docs/changelog.md` & `laminci-0.5.0/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+⬆️ Upgrade to new replace API | [15](https://github.com/laminlabs/laminci/pull/15) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.0
 ♻️ Replace `lndb` with `lamin` | [14](https://github.com/laminlabs/laminci/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-03-29 | 0.4.2
 🚸 Replace git checkout with git switch | [13](https://github.com/laminlabs/laminci/pull/13) | [falexwolf](https://github.com/falexwolf) | 2023-03-27 | 0.4.1
 ⬆️ Upgrade to LaminDB v0.35 | [12](https://github.com/laminlabs/laminci/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-03-26 | 0.4.0
 🚚 Rename `upload_docs_dir` to `upload_docs_artifact` |  | 2023-03-21 | 0.3.4
 🍱 Track images in docs | [11](https://github.com/laminlabs/laminci/pull/11) | [falexwolf](https://github.com/falexwolf) | 2023-03-12 | 0.3.2
 ➖ Remove dependency on lamindb in laminci | [10](https://github.com/laminlabs/laminci/pull/10) | [falexwolf](https://github.com/falexwolf) | 2023-03-09 | 0.3.0 / 0.3.1
 🍱 Track readme in docs upload | [9](https://github.com/laminlabs/laminci/pull/9) | [falexwolf](https://github.com/falexwolf) | 2023-03-06 | 0.2.5
```

### Comparing `laminci-0.4.2/docs/guide/quickstart.ipynb` & `laminci-0.5.0/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.4.2/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.5.0/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.4.2/laminci/_artifacts.py` & `laminci-0.5.0/laminci/_artifacts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import os
 from pathlib import Path
 from zipfile import ZipFile
 
-from ._env import get_package_name
-
+from lamin_logger import logger
 
-def upload_docs_artifact():
-    import lamindb as ln
+from ._env import get_package_name
 
-    if os.environ["GITHUB_EVENT_NAME"] != "push":
-        return
-    package_name = get_package_name()
-    filestem = f"{package_name}_docs"
-    filename = f"{filestem}.zip"
 
-    with ZipFile(filename, "w") as zf:
+def zip_docs_dir(zip_filename: str) -> None:
+    with ZipFile(zip_filename, "w") as zf:
         zf.write("README.md")
         for f in Path("./docs").glob("**/*"):
             if ".ipynb_checkpoints" in str(f):
                 continue
             if f.suffix in {".md", ".ipynb", ".png", ".jpg", ".svg"}:
                 zf.write(f, f.relative_to("./docs"))  # add at root level
 
+
+def upload_docs_artifact() -> None:
+    import lamindb as ln
+
+    if "GITHUB_EVENT_NAME" in os.environ and os.environ["GITHUB_EVENT_NAME"] != "push":
+        logger.info("Only upload docs artifact for push event.")
+        return None
+    package_name = get_package_name()
+    zip_filename = f"{package_name}_docs.zip"
+    zip_docs_dir(zip_filename)
+
     ln.setup.load("testuser1/lamin-site-assets", migrate=True)
 
-    with ln.Session() as ss:
-        transform = ln.add(ln.Transform, name=f"CI {package_name}")
-        run = ln.Run(transform=transform)
-
-        dobject = ss.select(ln.File, name=filestem).one_or_none()
-        if dobject is not None:
-            dobject._cloud_filepath = None
-            dobject._local_filepath = Path(filename)
-            dobject.source = run
-        else:
-            dobject = ln.File(filename, source=run)
-        ss.add(dobject)
+    transform = ln.add(ln.Transform, name=f"CI {package_name}")
+    ln.track(transform=transform)
+
+    file = ln.select(ln.File, key=f"docs/{zip_filename}").one_or_none()
+    if file is not None:
+        file.replace(zip_filename)
+    else:
+        file = ln.File(zip_filename, key=f"docs/{zip_filename}")
+    ln.add(file)
```

### Comparing `laminci-0.4.2/laminci/_db.py` & `laminci-0.5.0/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.4.2/laminci/_env.py` & `laminci-0.5.0/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.4.2/laminci/_nox.py` & `laminci-0.5.0/laminci/_nox.py`

 * *Files identical despite different names*

### Comparing `laminci-0.4.2/pyproject.toml` & `laminci-0.5.0/pyproject.toml`

 * *Files identical despite different names*

