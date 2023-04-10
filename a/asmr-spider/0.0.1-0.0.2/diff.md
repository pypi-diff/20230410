# Comparing `tmp/asmr_spider-0.0.1.tar.gz` & `tmp/asmr_spider-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmr_spider-0.0.1.tar", max compression
+gzip compressed data, was "asmr_spider-0.0.2.tar", max compression
```

## Comparing `asmr_spider-0.0.1.tar` & `asmr_spider-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-04-10 03:54:17.066181 asmr_spider-0.0.1/LICENSE
--rw-r--r--   0        0        0      552 2023-04-10 03:54:17.066181 asmr_spider-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-10 03:54:17.066181 asmr_spider-0.0.1/asmr_spider/__init__.py
--rw-r--r--   0        0        0      554 2023-04-10 03:54:17.066181 asmr_spider-0.0.1/asmr_spider/__main__.py
--rw-r--r--   0        0        0     1759 2023-04-10 03:54:17.066181 asmr_spider-0.0.1/asmr_spider/config.py
--rw-r--r--   0        0        0     5102 2023-04-10 03:54:17.066181 asmr_spider-0.0.1/asmr_spider/spider.py
--rw-r--r--   0        0        0      942 2023-04-10 03:54:17.066181 asmr_spider-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 asmr_spider-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/LICENSE
+-rw-r--r--   0        0        0      552 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/asmr_spider/__init__.py
+-rw-r--r--   0        0        0      601 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/asmr_spider/__main__.py
+-rw-r--r--   0        0        0     1767 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/asmr_spider/config.py
+-rw-r--r--   0        0        0     5102 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/asmr_spider/spider.py
+-rw-r--r--   0        0        0      942 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 asmr_spider-0.0.2/PKG-INFO
```

### Comparing `asmr_spider-0.0.1/LICENSE` & `asmr_spider-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.1/README.md` & `asmr_spider-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.1/asmr_spider/config.py` & `asmr_spider-0.0.2/asmr_spider/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from pydantic import BaseModel, Extra
 from pathlib import Path
-import yaml
+import sys, yaml
+from pydantic import BaseModel, Extra
 from loguru import logger
 from rich.progress import (
     BarColumn,
     DownloadColumn,
     Progress,
     TextColumn,
     TransferSpeedColumn,
@@ -52,15 +52,15 @@
     try:
         confpath.write_text(default_config, encoding='utf-8')
         logger.info(f := f'{confpath}: 配置文件已生成.')
         progress.console.log(f)
     except Exception as e:
         logger.error(f := f"{confpath}: 创建配置文件失败!\n"+repr(e))
         progress.console.log(f, style='bold yellow on black')
-        exit(-1)
+        sys.exit(1)
 
 
 _config = yaml.safe_load(confpath.read_text('utf-8'))
 
 
 class Config(BaseModel, extra=Extra.ignore):
     username: str = 'guest'
```

### Comparing `asmr_spider-0.0.1/asmr_spider/spider.py` & `asmr_spider-0.0.2/asmr_spider/spider.py`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.1/pyproject.toml` & `asmr_spider-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asmr-spider"
-version = "0.0.1"
+version = "0.0.2"
 description = "asmr.one 音声下载器"
 authors = ["月ヶ瀬"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [
     { include = "asmr_spider" },
 ]
```

### Comparing `asmr_spider-0.0.1/PKG-INFO` & `asmr_spider-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmr-spider
-Version: 0.0.1
+Version: 0.0.2
 Summary: asmr.one 音声下载器
 Home-page: https://github.com/tkgs0/asmr-spider
 License: GPL-3.0
 Keywords: ASMR,ASMR Downloader
 Author: 月ヶ瀬
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

