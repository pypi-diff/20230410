# Comparing `tmp/raydl-0.0.7.tar.gz` & `tmp/raydl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raydl-0.0.7.tar", last modified: Sun Apr  9 16:03:55 2023, max compression
+gzip compressed data, was "raydl-0.0.8.tar", last modified: Mon Apr 10 17:16:36 2023, max compression
```

## Comparing `raydl-0.0.7.tar` & `raydl-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-09 16:03:55.585296 raydl-0.0.7/
--rw-r--r--   0 rayw       (501) staff       (20)     1069 2023-01-24 10:36:02.000000 raydl-0.0.7/LICENSE
--rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-09 16:03:55.585139 raydl-0.0.7/PKG-INFO
--rw-r--r--   0 rayw       (501) staff       (20)      227 2023-01-24 12:20:22.000000 raydl-0.0.7/README.md
--rw-r--r--   0 rayw       (501) staff       (20)     1736 2023-04-09 16:03:34.000000 raydl-0.0.7/pyproject.toml
--rw-r--r--   0 rayw       (501) staff       (20)       38 2023-04-09 16:03:55.585345 raydl-0.0.7/setup.cfg
--rw-r--r--   0 rayw       (501) staff       (20)       38 2023-01-24 12:50:45.000000 raydl-0.0.7/setup.py
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-09 16:03:55.580953 raydl-0.0.7/src/
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-09 16:03:55.584117 raydl-0.0.7/src/raydl/
--rw-r--r--   0 rayw       (501) staff       (20)      441 2023-04-09 16:03:34.000000 raydl-0.0.7/src/raydl/__init__.py
--rw-r--r--   0 rayw       (501) staff       (20)     3242 2023-03-29 17:49:47.000000 raydl-0.0.7/src/raydl/__main__.py
--rw-r--r--   0 rayw       (501) staff       (20)     1466 2023-01-31 03:35:05.000000 raydl-0.0.7/src/raydl/collect_env.py
--rw-r--r--   0 rayw       (501) staff       (20)    12896 2023-04-09 16:01:01.000000 raydl-0.0.7/src/raydl/image.py
--rw-r--r--   0 rayw       (501) staff       (20)     4339 2023-04-01 02:56:34.000000 raydl-0.0.7/src/raydl/initialization.py
--rw-r--r--   0 rayw       (501) staff       (20)    13850 2023-04-01 02:57:11.000000 raydl-0.0.7/src/raydl/sfdb.py
--rw-r--r--   0 rayw       (501) staff       (20)     5021 2023-03-29 15:02:33.000000 raydl-0.0.7/src/raydl/tensor.py
--rw-r--r--   0 rayw       (501) staff       (20)     2229 2023-02-25 16:45:04.000000 raydl-0.0.7/src/raydl/time.py
--rw-r--r--   0 rayw       (501) staff       (20)      705 2023-03-18 18:27:59.000000 raydl-0.0.7/src/raydl/utils.py
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-09 16:03:55.584923 raydl-0.0.7/src/raydl.egg-info/
--rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/PKG-INFO
--rw-r--r--   0 rayw       (501) staff       (20)      396 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/SOURCES.txt
--rw-r--r--   0 rayw       (501) staff       (20)        1 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/dependency_links.txt
--rw-r--r--   0 rayw       (501) staff       (20)       37 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/requires.txt
--rw-r--r--   0 rayw       (501) staff       (20)        6 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/top_level.txt
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-10 17:16:36.692127 raydl-0.0.8/
+-rw-r--r--   0 rayw       (501) staff       (20)     1069 2023-01-24 10:36:02.000000 raydl-0.0.8/LICENSE
+-rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-10 17:16:36.691822 raydl-0.0.8/PKG-INFO
+-rw-r--r--   0 rayw       (501) staff       (20)      227 2023-01-24 12:20:22.000000 raydl-0.0.8/README.md
+-rw-r--r--   0 rayw       (501) staff       (20)     1736 2023-04-10 17:16:01.000000 raydl-0.0.8/pyproject.toml
+-rw-r--r--   0 rayw       (501) staff       (20)       38 2023-04-10 17:16:36.692227 raydl-0.0.8/setup.cfg
+-rw-r--r--   0 rayw       (501) staff       (20)       38 2023-01-24 12:50:45.000000 raydl-0.0.8/setup.py
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-10 17:16:36.683941 raydl-0.0.8/src/
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-10 17:16:36.690100 raydl-0.0.8/src/raydl/
+-rw-r--r--   0 rayw       (501) staff       (20)      461 2023-04-10 17:16:01.000000 raydl-0.0.8/src/raydl/__init__.py
+-rw-r--r--   0 rayw       (501) staff       (20)     5063 2023-04-10 17:14:21.000000 raydl-0.0.8/src/raydl/__main__.py
+-rw-r--r--   0 rayw       (501) staff       (20)     1466 2023-01-31 03:35:05.000000 raydl-0.0.8/src/raydl/collect_env.py
+-rw-r--r--   0 rayw       (501) staff       (20)    12896 2023-04-09 16:01:01.000000 raydl-0.0.8/src/raydl/image.py
+-rw-r--r--   0 rayw       (501) staff       (20)     4339 2023-04-01 02:56:34.000000 raydl-0.0.8/src/raydl/initialization.py
+-rw-r--r--   0 rayw       (501) staff       (20)    13883 2023-04-10 15:30:58.000000 raydl-0.0.8/src/raydl/sfdb.py
+-rw-r--r--   0 rayw       (501) staff       (20)     5021 2023-03-29 15:02:33.000000 raydl-0.0.8/src/raydl/tensor.py
+-rw-r--r--   0 rayw       (501) staff       (20)     2229 2023-02-25 16:45:04.000000 raydl-0.0.8/src/raydl/time.py
+-rw-r--r--   0 rayw       (501) staff       (20)      705 2023-03-18 18:27:59.000000 raydl-0.0.8/src/raydl/utils.py
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-10 17:16:36.691449 raydl-0.0.8/src/raydl.egg-info/
+-rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/PKG-INFO
+-rw-r--r--   0 rayw       (501) staff       (20)      396 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/SOURCES.txt
+-rw-r--r--   0 rayw       (501) staff       (20)        1 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/dependency_links.txt
+-rw-r--r--   0 rayw       (501) staff       (20)       37 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/requires.txt
+-rw-r--r--   0 rayw       (501) staff       (20)        6 2023-04-10 17:16:36.000000 raydl-0.0.8/src/raydl.egg-info/top_level.txt
```

### Comparing `raydl-0.0.7/LICENSE` & `raydl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `raydl-0.0.7/PKG-INFO` & `raydl-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raydl
-Version: 0.0.7
+Version: 0.0.8
 Summary: The library of utilities to help you deal with the deep learning in PyTorch.
 Author: Ray Wang
 License: MIT License
         
         Copyright (c) [2023] [Ray Wang]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `raydl-0.0.7/pyproject.toml` & `raydl-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "raydl"
-version = "0.0.7"
+version = "0.0.8"
 description = "The library of utilities to help you deal with the deep learning in PyTorch."
 readme = "README.md"
 authors = [{ name = "Ray Wang" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -51,15 +51,15 @@
 ignore = ["UP007", "C408", "B905"]
 line-length=119
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.bumpver]
-current_version = "0.0.7"
+current_version = "0.0.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `raydl-0.0.7/src/raydl/__main__.py` & `raydl-0.0.8/src/raydl/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,48 @@
 import fire
 import torch
 from torchvision.datasets.folder import is_image_file
 
 import raydl
 
 
+def diff(path1, path2, save_path=None, adaptive=False):
+    path1 = Path(path1)
+    path2 = Path(path2)
+    if path1.is_file() and path2.is_file():
+        save_path = Path(save_path) if save_path is not None else path1.parent
+        images_iterator = [(path1, path2, save_path / f"{path1.stem}_diff_{path2.stem}{path1.suffix}")]
+    elif path1.is_dir() and path2.is_dir():
+        save_path = Path(save_path) if save_path is not None else path1.parent / f"{path1.name}_diff_{path2.name}"
+        if not save_path.exists():
+            print(f"mkdir {save_path}")
+            save_path.mkdir()
+        files1 = [f for f in Path(path1).glob("*") if is_image_file(f.name) and (path2 / f.name).exists()]
+        files2 = [path2 / f.name for f in files1]
+        images_iterator = zip(files1, files2, [save_path / f.name for f in files1])
+    else:
+        raise ValueError(f"{path1} and {path2} are not both files or both folders")
+    for image_path1, image_path2, path in images_iterator:
+        image1 = raydl.load_images(image_path1, value_range=(0, 1))
+        image2 = raydl.load_images(image_path2, value_range=(0, 1))
+        assert image1.size() == image2.size()
+        range_max = (1**1 * 3) ** 0.5 if not adaptive else None
+        image_diff = torch.norm(image1 - image2, p=2, dim=1)
+        print(
+            f"{image_path1} and {image_path2} "
+            f"max difference is {image_diff.max():.4f} ({100 * image_diff.max() / ((1 ** 1 * 3) ** 0.5):.2f}%)"
+        )
+        diff_heatmap = raydl.create_heatmap(image_diff, scale_each=False, range_min=0, range_max=range_max)
+        if path.exists():
+            _path = path.parent / f"{path.stem}_diff{path.suffix}"
+            print(f"{path} existed! rename save path to {_path}")
+            path = _path
+        raydl.save_images(diff_heatmap, path)
+
+
 def _infer_save_path(save_path, images_to_compare, batch_id, batch_size):
     if batch_size == 1:
         if is_image_file(save_path.name):
             save_path.parent.mkdir(exist_ok=True)
             return save_path.parent / images_to_compare[batch_id]
         save_path.mkdir(exist_ok=True)
         return save_path / images_to_compare[batch_id]
```

### Comparing `raydl-0.0.7/src/raydl/collect_env.py` & `raydl-0.0.8/src/raydl/collect_env.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.7/src/raydl/image.py` & `raydl-0.0.8/src/raydl/image.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.7/src/raydl/initialization.py` & `raydl-0.0.8/src/raydl/initialization.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.7/src/raydl/sfdb.py` & `raydl-0.0.8/src/raydl/sfdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 class PILImageTypeMapper(TypeMapper):
     def __init__(self) -> None:
         super().__init__("BLOB", PIL.Image.Image)
 
     @staticmethod
     def serialize(obj: PIL.Image.Image):
         buff = BytesIO()
-        obj.save(buff, format="webp")
+        obj.save(buff, format="webp", lossless=True)
         return buff.getvalue()
 
     @staticmethod
     def unserialize(val):
         return PIL.Image.open(BytesIO(val))
 
 
@@ -169,15 +169,15 @@
             self._sqlite.commit()
 
             self._commit_timer = time.time()
             self._commit_counter = 0
         return
 
     def close(self):
-        if self._sqlite is None:
+        if self._sqlite is None or self._is_close:
             return
         self._sanity_check()
         self.commit()
         with self._lock:
             self._sqlite.close()
             self._is_close = True
         return
```

### Comparing `raydl-0.0.7/src/raydl/tensor.py` & `raydl-0.0.8/src/raydl/tensor.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.7/src/raydl/time.py` & `raydl-0.0.8/src/raydl/time.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.7/src/raydl/utils.py` & `raydl-0.0.8/src/raydl/utils.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.7/src/raydl.egg-info/PKG-INFO` & `raydl-0.0.8/src/raydl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raydl
-Version: 0.0.7
+Version: 0.0.8
 Summary: The library of utilities to help you deal with the deep learning in PyTorch.
 Author: Ray Wang
 License: MIT License
         
         Copyright (c) [2023] [Ray Wang]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

