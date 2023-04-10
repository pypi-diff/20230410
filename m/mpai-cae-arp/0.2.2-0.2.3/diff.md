# Comparing `tmp/mpai_cae_arp-0.2.2.tar.gz` & `tmp/mpai_cae_arp-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpai_cae_arp-0.2.2.tar", max compression
+gzip compressed data, was "mpai_cae_arp-0.2.3.tar", max compression
```

## Comparing `mpai_cae_arp-0.2.2.tar` & `mpai_cae_arp-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-03 21:35:54.975907 mpai_cae_arp-0.2.2/LICENSE
--rw-r--r--   0        0        0      491 2023-04-03 21:22:02.773309 mpai_cae_arp-0.2.2/README.md
--rw-r--r--   0        0        0      276 2023-04-04 08:31:02.533352 mpai_cae_arp-0.2.2/mpai_cae_arp/__init__.py
--rw-r--r--   0        0        0      176 2023-04-04 07:37:21.160932 mpai_cae_arp-0.2.2/mpai_cae_arp/audio/__init__.py
--rw-r--r--   0        0        0    17904 2023-04-06 15:03:52.274016 mpai_cae_arp-0.2.2/mpai_cae_arp/audio/_audio.py
--rw-r--r--   0        0        0     2516 2023-04-04 07:38:52.008419 mpai_cae_arp-0.2.2/mpai_cae_arp/audio/_noise.py
--rw-r--r--   0        0        0      219 2023-04-03 21:48:20.943719 mpai_cae_arp-0.2.2/mpai_cae_arp/audio/standards.py
--rw-r--r--   0        0        0     4211 2023-04-04 07:22:07.372604 mpai_cae_arp-0.2.2/mpai_cae_arp/audio/utils.py
--rw-r--r--   0        0        0     2045 2023-04-06 14:59:46.415794 mpai_cae_arp-0.2.2/mpai_cae_arp/files.py
--rw-r--r--   0        0        0     1304 2023-04-06 14:57:19.804922 mpai_cae_arp-0.2.2/mpai_cae_arp/io.py
--rw-r--r--   0        0        0     3100 2023-04-03 21:32:30.045143 mpai_cae_arp-0.2.2/mpai_cae_arp/time.py
--rw-r--r--   0        0        0        0 2023-04-03 21:25:06.272009 mpai_cae_arp-0.2.2/mpai_cae_arp/types/__init__.py
--rw-r--r--   0        0        0     6947 2023-04-09 09:39:26.907184 mpai_cae_arp-0.2.2/mpai_cae_arp/types/irregularity.py
--rw-r--r--   0        0        0     1668 2023-04-03 21:48:21.015718 mpai_cae_arp-0.2.2/mpai_cae_arp/types/schema.py
--rw-r--r--   0        0        0     1215 2023-04-09 09:39:33.927123 mpai_cae_arp-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 mpai_cae_arp-0.2.2/setup.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 mpai_cae_arp-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-03 21:35:54.975907 mpai_cae_arp-0.2.3/LICENSE
+-rw-r--r--   0        0        0      491 2023-04-03 21:22:02.773309 mpai_cae_arp-0.2.3/README.md
+-rw-r--r--   0        0        0      276 2023-04-04 08:31:02.533352 mpai_cae_arp-0.2.3/mpai_cae_arp/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-04 07:37:21.160932 mpai_cae_arp-0.2.3/mpai_cae_arp/audio/__init__.py
+-rw-r--r--   0        0        0    17904 2023-04-06 15:03:52.274016 mpai_cae_arp-0.2.3/mpai_cae_arp/audio/_audio.py
+-rw-r--r--   0        0        0     2516 2023-04-04 07:38:52.008419 mpai_cae_arp-0.2.3/mpai_cae_arp/audio/_noise.py
+-rw-r--r--   0        0        0      219 2023-04-03 21:48:20.943719 mpai_cae_arp-0.2.3/mpai_cae_arp/audio/standards.py
+-rw-r--r--   0        0        0     4211 2023-04-04 07:22:07.372604 mpai_cae_arp-0.2.3/mpai_cae_arp/audio/utils.py
+-rw-r--r--   0        0        0     2045 2023-04-06 14:59:46.415794 mpai_cae_arp-0.2.3/mpai_cae_arp/files.py
+-rw-r--r--   0        0        0     1304 2023-04-06 14:57:19.804922 mpai_cae_arp-0.2.3/mpai_cae_arp/io.py
+-rw-r--r--   0        0        0     3100 2023-04-03 21:32:30.045143 mpai_cae_arp-0.2.3/mpai_cae_arp/time.py
+-rw-r--r--   0        0        0        0 2023-04-03 21:25:06.272009 mpai_cae_arp-0.2.3/mpai_cae_arp/types/__init__.py
+-rw-r--r--   0        0        0     6939 2023-04-10 09:26:01.216220 mpai_cae_arp-0.2.3/mpai_cae_arp/types/irregularity.py
+-rw-r--r--   0        0        0     1668 2023-04-03 21:48:21.015718 mpai_cae_arp-0.2.3/mpai_cae_arp/types/schema.py
+-rw-r--r--   0        0        0     1215 2023-04-10 09:26:13.036153 mpai_cae_arp-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 mpai_cae_arp-0.2.3/setup.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 mpai_cae_arp-0.2.3/PKG-INFO
```

### Comparing `mpai_cae_arp-0.2.2/LICENSE` & `mpai_cae_arp-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.2/mpai_cae_arp/audio/_audio.py` & `mpai_cae_arp-0.2.3/mpai_cae_arp/audio/_audio.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.2/mpai_cae_arp/audio/_noise.py` & `mpai_cae_arp-0.2.3/mpai_cae_arp/audio/_noise.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.2/mpai_cae_arp/audio/utils.py` & `mpai_cae_arp-0.2.3/mpai_cae_arp/audio/utils.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.2/mpai_cae_arp/files.py` & `mpai_cae_arp-0.2.3/mpai_cae_arp/files.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.2/mpai_cae_arp/io.py` & `mpai_cae_arp-0.2.3/mpai_cae_arp/io.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.2/mpai_cae_arp/time.py` & `mpai_cae_arp-0.2.3/mpai_cae_arp/time.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.2/mpai_cae_arp/types/irregularity.py` & `mpai_cae_arp-0.2.3/mpai_cae_arp/types/irregularity.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         }
 
 
 class Irregularity(BaseModel):
     irregularity_ID: uuid.UUID
     source: Source
     time_label: str
-    irregularity_type: IrregularityType = None
+    irregularity_type: IrregularityType | None = None
     irregularity_properties: IrregularityProperties | None = None
     image_URI: str | None = None
     audio_block_URI: str | None = None
 
     @staticmethod
     def from_json(json_irreg: dict):
 
@@ -116,15 +116,15 @@
 
         return dictionary
 
 
 class IrregularityFile(BaseModel):
     # TODO: the offset calculation is not implemented yet, so it is set to None
     irregularities: list[Irregularity]
-    offset: Annotated[int, Field(default=0)]
+    offset: int | None = None
 
     class Config:
         schema_extra = {
             "example": {
                 "offset":
                 0,
                 "irregularities": [{
```

### Comparing `mpai_cae_arp-0.2.2/mpai_cae_arp/types/schema.py` & `mpai_cae_arp-0.2.3/mpai_cae_arp/types/schema.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.2/pyproject.toml` & `mpai_cae_arp-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpai-cae-arp"
-version = "0.2.2"
+version = "0.2.3"
 description = "The MPAI CAE-ARP software API"
 authors = ["Matteo Spanio <dev2@audioinnova.com>"]
 readme = "README.md"
 packages = [{include = "mpai_cae_arp"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `mpai_cae_arp-0.2.2/setup.py` & `mpai_cae_arp-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'llvmlite>=0.39.1,<0.40.0',
  'numpy==1.23.3',
  'pydantic>=1.10.7,<2.0.0',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'mpai-cae-arp',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'The MPAI CAE-ARP software API',
     'long_description': '# MPAI CAE-ARP API\n\n[![LICENSE](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://img.shields.io/badge/license-GPLv3-blue.svg)\n\n## Description\n\nThis package provides a set of tools for common task in MPAI CAE-ARP standard. It is usend in the official implementation of the standard and can be used as well to develop your own.\n\n## License\n\nThis software is licensed under the GPLv3 license. See the [official site](http://www.gnu.org/licenses/gpl-3.0.html) for more information.\n',
     'author': 'Matteo Spanio',
     'author_email': 'dev2@audioinnova.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mpai_cae_arp-0.2.2/PKG-INFO` & `mpai_cae_arp-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpai-cae-arp
-Version: 0.2.2
+Version: 0.2.3
 Summary: The MPAI CAE-ARP software API
 Author: Matteo Spanio
 Author-email: dev2@audioinnova.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

