# Comparing `tmp/pt-datasets-0.9.8.tar.gz` & `tmp/pt-datasets-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pt-datasets-0.9.8.tar", last modified: Wed Jan 27 06:16:11 2021, max compression
+gzip compressed data, was "dist/pt-datasets-0.9.9.tar", last modified: Wed Jan 27 06:52:38 2021, max compression
```

## Comparing `pt-datasets-0.9.8.tar` & `pt-datasets-0.9.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 darth     (1000) darth     (1000)        0 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/
--rw-rw-r--   0 darth     (1000) darth     (1000)     6743 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/PKG-INFO
--rw-rw-r--   0 darth     (1000) darth     (1000)     5064 2021-01-22 09:58:36.000000 pt-datasets-0.9.8/README.md
-drwxrwxr-x   0 darth     (1000) darth     (1000)        0 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/pt_datasets/
--rw-rw-r--   0 darth     (1000) darth     (1000)     6324 2021-01-27 06:14:18.000000 pt-datasets-0.9.8/pt_datasets/COVID19Dataset.py
--rw-rw-r--   0 darth     (1000) darth     (1000)     1329 2021-01-21 15:52:25.000000 pt-datasets-0.9.8/pt_datasets/__init__.py
--rw-rw-r--   0 darth     (1000) darth     (1000)     1729 2020-11-01 10:33:17.000000 pt-datasets-0.9.8/pt_datasets/create_dataloader.py
--rw-rw-r--   0 darth     (1000) darth     (1000)     1513 2021-01-02 15:17:54.000000 pt-datasets-0.9.8/pt_datasets/create_dataset.py
--rw-rw-r--   0 darth     (1000) darth     (1000)     1722 2021-01-21 15:52:25.000000 pt-datasets-0.9.8/pt_datasets/download_covid_dataset.py
--rw-rw-r--   0 darth     (1000) darth     (1000)     2469 2020-11-26 15:01:42.000000 pt-datasets-0.9.8/pt_datasets/encode_features.py
--rw-rw-r--   0 darth     (1000) darth     (1000)    17915 2021-01-27 06:14:18.000000 pt-datasets-0.9.8/pt_datasets/load_dataset.py
--rw-rw-r--   0 darth     (1000) darth     (1000)     8005 2021-01-21 12:08:15.000000 pt-datasets-0.9.8/pt_datasets/utils.py
-drwxrwxr-x   0 darth     (1000) darth     (1000)        0 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/pt_datasets.egg-info/
--rw-rw-r--   0 darth     (1000) darth     (1000)     6743 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/pt_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 darth     (1000) darth     (1000)      437 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/pt_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 darth     (1000) darth     (1000)        1 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/pt_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 darth     (1000) darth     (1000)      128 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/pt_datasets.egg-info/requires.txt
--rw-rw-r--   0 darth     (1000) darth     (1000)       12 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/pt_datasets.egg-info/top_level.txt
--rw-rw-r--   0 darth     (1000) darth     (1000)       79 2021-01-27 06:16:11.000000 pt-datasets-0.9.8/setup.cfg
--rw-rw-r--   0 darth     (1000) darth     (1000)     1474 2021-01-27 06:15:08.000000 pt-datasets-0.9.8/setup.py
+drwxrwxr-x   0 darth     (1000) darth     (1000)        0 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/
+-rw-rw-r--   0 darth     (1000) darth     (1000)     6743 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/PKG-INFO
+-rw-rw-r--   0 darth     (1000) darth     (1000)     5064 2021-01-22 09:58:36.000000 pt-datasets-0.9.9/README.md
+drwxrwxr-x   0 darth     (1000) darth     (1000)        0 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/pt_datasets/
+-rw-rw-r--   0 darth     (1000) darth     (1000)     6340 2021-01-27 06:40:23.000000 pt-datasets-0.9.9/pt_datasets/COVID19Dataset.py
+-rw-rw-r--   0 darth     (1000) darth     (1000)     1329 2021-01-21 15:52:25.000000 pt-datasets-0.9.9/pt_datasets/__init__.py
+-rw-rw-r--   0 darth     (1000) darth     (1000)     1729 2020-11-01 10:33:17.000000 pt-datasets-0.9.9/pt_datasets/create_dataloader.py
+-rw-rw-r--   0 darth     (1000) darth     (1000)     1513 2021-01-02 15:17:54.000000 pt-datasets-0.9.9/pt_datasets/create_dataset.py
+-rw-rw-r--   0 darth     (1000) darth     (1000)     1722 2021-01-21 15:52:25.000000 pt-datasets-0.9.9/pt_datasets/download_covid_dataset.py
+-rw-rw-r--   0 darth     (1000) darth     (1000)     2469 2020-11-26 15:01:42.000000 pt-datasets-0.9.9/pt_datasets/encode_features.py
+-rw-rw-r--   0 darth     (1000) darth     (1000)    17915 2021-01-27 06:14:18.000000 pt-datasets-0.9.9/pt_datasets/load_dataset.py
+-rw-rw-r--   0 darth     (1000) darth     (1000)     8005 2021-01-21 12:08:15.000000 pt-datasets-0.9.9/pt_datasets/utils.py
+drwxrwxr-x   0 darth     (1000) darth     (1000)        0 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/pt_datasets.egg-info/
+-rw-rw-r--   0 darth     (1000) darth     (1000)     6743 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/pt_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 darth     (1000) darth     (1000)      437 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/pt_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 darth     (1000) darth     (1000)        1 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/pt_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 darth     (1000) darth     (1000)      128 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/pt_datasets.egg-info/requires.txt
+-rw-rw-r--   0 darth     (1000) darth     (1000)       12 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/pt_datasets.egg-info/top_level.txt
+-rw-rw-r--   0 darth     (1000) darth     (1000)       79 2021-01-27 06:52:38.000000 pt-datasets-0.9.9/setup.cfg
+-rw-rw-r--   0 darth     (1000) darth     (1000)     1474 2021-01-27 06:51:58.000000 pt-datasets-0.9.9/setup.py
```

### Comparing `pt-datasets-0.9.8/PKG-INFO` & `pt-datasets-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-datasets
-Version: 0.9.8
+Version: 0.9.9
 Summary: Library for loading PyTorch datasets and data loaders.
 Home-page: https://github.com/AFAgarap/pt-datasets
 Author: Abien Fred Agarap
 Author-email: abienfred.agarap@gmail.com
 License: AGPL-3.0 License
 Description: # PyTorch Datasets
```

### Comparing `pt-datasets-0.9.8/README.md` & `pt-datasets-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pt-datasets-0.9.8/pt_datasets/COVID19Dataset.py` & `pt-datasets-0.9.9/pt_datasets/COVID19Dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def __getitem__(self, idx) -> Tuple:
         if torch.is_tensor(idx):
             idx = idx.tolist()
         image = self.data[idx]
         if self.transform:
             image = self.transform(image)
-        label = self.labels[idx]
+        label = self.labels[idx].astype("int64")
         return (image, label)
 
 
 class BinaryCOVID19Dataset(torch.utils.data.Dataset):
     """
     Dataset class for the COVID19 binary classification dataset.
     """
```

### Comparing `pt-datasets-0.9.8/pt_datasets/__init__.py` & `pt-datasets-0.9.9/pt_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pt-datasets-0.9.8/pt_datasets/create_dataloader.py` & `pt-datasets-0.9.9/pt_datasets/create_dataloader.py`

 * *Files identical despite different names*

### Comparing `pt-datasets-0.9.8/pt_datasets/create_dataset.py` & `pt-datasets-0.9.9/pt_datasets/create_dataset.py`

 * *Files identical despite different names*

### Comparing `pt-datasets-0.9.8/pt_datasets/download_covid_dataset.py` & `pt-datasets-0.9.9/pt_datasets/download_covid_dataset.py`

 * *Files identical despite different names*

### Comparing `pt-datasets-0.9.8/pt_datasets/encode_features.py` & `pt-datasets-0.9.9/pt_datasets/encode_features.py`

 * *Files identical despite different names*

### Comparing `pt-datasets-0.9.8/pt_datasets/load_dataset.py` & `pt-datasets-0.9.9/pt_datasets/load_dataset.py`

 * *Files identical despite different names*

### Comparing `pt-datasets-0.9.8/pt_datasets/utils.py` & `pt-datasets-0.9.9/pt_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `pt-datasets-0.9.8/pt_datasets.egg-info/PKG-INFO` & `pt-datasets-0.9.9/pt_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-datasets
-Version: 0.9.8
+Version: 0.9.9
 Summary: Library for loading PyTorch datasets and data loaders.
 Home-page: https://github.com/AFAgarap/pt-datasets
 Author: Abien Fred Agarap
 Author-email: abienfred.agarap@gmail.com
 License: AGPL-3.0 License
 Description: # PyTorch Datasets
```

### Comparing `pt-datasets-0.9.8/setup.py` & `pt-datasets-0.9.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         echo "[SUCCESS] Done downloading AG News Dataset."
         """
     os.system(ag_news_setup)
 
 
 setup(
     name="pt-datasets",
-    version="0.9.8",
+    version="0.9.9",
     packages=["pt_datasets"],
     url="https://github.com/AFAgarap/pt-datasets",
     license="AGPL-3.0 License",
     author="Abien Fred Agarap",
     author_email="abienfred.agarap@gmail.com",
     description="Library for loading PyTorch datasets and data loaders.",
     long_description=long_description,
```

