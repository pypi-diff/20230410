# Comparing `tmp/pdstools-3.0.1.tar.gz` & `tmp/pdstools-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.0.1.tar", last modified: Fri Mar 31 11:55:15 2023, max compression
+gzip compressed data, was "pdstools-3.0.2.tar", last modified: Mon Apr 10 12:52:27 2023, max compression
```

## Comparing `pdstools-3.0.1.tar` & `pdstools-3.0.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.328621 pdstools-3.0.1/
--rw-r--r--   0 kass1    (1567227574) staff       (20)    11357 2023-03-25 12:28:07.000000 pdstools-3.0.1/LICENSE
--rw-r--r--   0 kass1    (1567227574) staff       (20)     4414 2023-03-31 11:55:15.327035 pdstools-3.0.1/PKG-INFO
--rw-r--r--   0 kass1    (1567227574) staff       (20)     3469 2023-03-25 12:28:07.000000 pdstools-3.0.1/README.md
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.206241 pdstools-3.0.1/pdstools.egg-info/
--rw-r--r--   0 kass1    (1567227574) staff       (20)     4414 2023-03-31 11:55:15.000000 pdstools-3.0.1/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 kass1    (1567227574) staff       (20)     1332 2023-03-31 11:55:15.000000 pdstools-3.0.1/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 kass1    (1567227574) staff       (20)        1 2023-03-31 11:55:15.000000 pdstools-3.0.1/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 kass1    (1567227574) staff       (20)       51 2023-03-31 11:55:15.000000 pdstools-3.0.1/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 kass1    (1567227574) staff       (20)      227 2023-03-31 11:55:15.000000 pdstools-3.0.1/pdstools.egg-info/requires.txt
--rw-r--r--   0 kass1    (1567227574) staff       (20)        9 2023-03-31 11:55:15.000000 pdstools-3.0.1/pdstools.egg-info/top_level.txt
--rw-r--r--   0 kass1    (1567227574) staff       (20)     1750 2023-03-28 14:58:57.000000 pdstools-3.0.1/pyproject.toml
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.168178 pdstools-3.0.1/python/
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.209828 pdstools-3.0.1/python/pdstools/
--rw-r--r--   0 kass1    (1567227574) staff       (20)      766 2023-03-28 14:39:34.000000 pdstools-3.0.1/python/pdstools/__init__.py
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.223580 pdstools-3.0.1/python/pdstools/adm/
--rw-r--r--   0 kass1    (1567227574) staff       (20)    56845 2023-03-31 11:43:44.000000 pdstools-3.0.1/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)    39891 2023-03-31 11:43:44.000000 pdstools-3.0.1/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)     4598 2023-03-31 11:43:44.000000 pdstools-3.0.1/python/pdstools/adm/Tables.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)        0 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.233050 pdstools-3.0.1/python/pdstools/app/
--rw-r--r--   0 kass1    (1567227574) staff       (20)      446 2023-03-26 12:55:56.000000 pdstools-3.0.1/python/pdstools/app/Home.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)        0 2023-03-26 13:58:53.000000 pdstools-3.0.1/python/pdstools/app/__init__.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)      961 2023-03-31 11:43:44.000000 pdstools-3.0.1/python/pdstools/app/cli.py
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.240830 pdstools-3.0.1/python/pdstools/app/pages/
--rw-r--r--   0 kass1    (1567227574) staff       (20)     1220 2023-03-26 11:17:23.000000 pdstools-3.0.1/python/pdstools/app/pages/CategorizationTest.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)     7620 2023-03-31 11:43:44.000000 pdstools-3.0.1/python/pdstools/app/pages/Health Check.py
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.251450 pdstools-3.0.1/python/pdstools/ih/
--rw-r--r--   0 kass1    (1567227574) staff       (20)     3558 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)        0 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/ih/__init__.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)    15127 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.268932 pdstools-3.0.1/python/pdstools/pega_io/
--rw-r--r--   0 kass1    (1567227574) staff       (20)      736 2023-03-31 07:34:19.000000 pdstools-3.0.1/python/pdstools/pega_io/API.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)    13543 2023-03-30 09:58:35.000000 pdstools-3.0.1/python/pdstools/pega_io/File.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)     6261 2023-03-30 11:27:29.000000 pdstools-3.0.1/python/pdstools/pega_io/S3.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)       57 2023-03-28 13:58:05.000000 pdstools-3.0.1/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.279469 pdstools-3.0.1/python/pdstools/plots/
--rw-r--r--   0 kass1    (1567227574) staff       (20)        0 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/plots/__init__.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)    51016 2023-03-26 09:16:53.000000 pdstools-3.0.1/python/pdstools/plots/plot_base.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)    29608 2023-03-26 13:31:12.000000 pdstools-3.0.1/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.287966 pdstools-3.0.1/python/pdstools/reports/
--rw-r--r--   0 kass1    (1567227574) staff       (20)    39141 2023-03-31 11:43:44.000000 pdstools-3.0.1/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 kass1    (1567227574) staff       (20)        0 2023-03-26 13:05:55.000000 pdstools-3.0.1/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.318212 pdstools-3.0.1/python/pdstools/utils/
--rw-r--r--   0 kass1    (1567227574) staff       (20)        0 2023-03-26 13:57:18.000000 pdstools-3.0.1/python/pdstools/utils/__init__.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)    17891 2023-03-31 11:43:44.000000 pdstools-3.0.1/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)     1138 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/utils/datasets.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)      445 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/utils/errors.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)    15921 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)     2026 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/utils/pega_template.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)     9169 2023-03-31 11:43:44.000000 pdstools-3.0.1/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)       92 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/utils/types.py
-drwxr-xr-x   0 kass1    (1567227574) staff       (20)        0 2023-03-31 11:55:15.325161 pdstools-3.0.1/python/pdstools/valuefinder/
--rw-r--r--   0 kass1    (1567227574) staff       (20)    21893 2023-03-28 14:42:07.000000 pdstools-3.0.1/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)        0 2023-03-25 12:28:08.000000 pdstools-3.0.1/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 kass1    (1567227574) staff       (20)       38 2023-03-31 11:55:15.328900 pdstools-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.508414 pdstools-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 12:52:17.000000 pdstools-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 12:52:27.504413 pdstools-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-10 12:52:17.000000 pdstools-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-10 12:52:17.000000 pdstools-3.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.496413 pdstools-3.0.2/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)    57635 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40057 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/app/pages/Health Check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    39142 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/reports/HealthCheckModel.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (123)    24211 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:52:27.508414 pdstools-3.0.2/setup.cfg
```

### Comparing `pdstools-3.0.1/LICENSE` & `pdstools-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/PKG-INFO` & `pdstools-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.0.1
+Version: 3.0.2
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.0.1 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.0.2 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.0.1/README.md` & `pdstools-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/pdstools.egg-info/PKG-INFO` & `pdstools-3.0.2/pdstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.0.1
+Version: 3.0.2
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.0.1 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.0.2 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.0.1/pdstools.egg-info/SOURCES.txt` & `pdstools-3.0.2/pdstools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,32 @@
 python/pdstools/adm/ADMDatamart.py
 python/pdstools/adm/ADMTrees.py
 python/pdstools/adm/Tables.py
 python/pdstools/adm/__init__.py
 python/pdstools/app/Home.py
 python/pdstools/app/__init__.py
 python/pdstools/app/cli.py
-python/pdstools/app/pages/CategorizationTest.py
 python/pdstools/app/pages/Health Check.py
 python/pdstools/ih/IHAnalysis.py
 python/pdstools/ih/__init__.py
 python/pdstools/ih/legacy_IH.py
 python/pdstools/pega_io/API.py
 python/pdstools/pega_io/File.py
 python/pdstools/pega_io/S3.py
 python/pdstools/pega_io/__init__.py
 python/pdstools/plots/__init__.py
 python/pdstools/plots/plot_base.py
 python/pdstools/plots/plots_plotly.py
 python/pdstools/reports/HealthCheck.qmd
+python/pdstools/reports/HealthCheckModel.qmd
 python/pdstools/reports/__init__.py
 python/pdstools/utils/__init__.py
 python/pdstools/utils/cdh_utils.py
 python/pdstools/utils/datasets.py
 python/pdstools/utils/errors.py
 python/pdstools/utils/hds_utils.py
 python/pdstools/utils/pega_template.py
+python/pdstools/utils/polars_ext.py
 python/pdstools/utils/streamlit_utils.py
 python/pdstools/utils/types.py
 python/pdstools/valuefinder/ValueFinder.py
 python/pdstools/valuefinder/__init__.py
```

### Comparing `pdstools-3.0.1/pyproject.toml` & `pdstools-3.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "datascientist",
     "tools",
 ]
 dependencies = [
         "plotly>=5.5.0",
         "requests",
         "pydot",
-        "polars>=0.16.8",
+        "polars>=0.17.0",
         "pyarrow",
         "tqdm",
         "pyyaml",
         "aioboto3>=11.0"
     ]
 requires-python = ">=3.8"
```

### Comparing `pdstools-3.0.1/python/pdstools/__init__.py` & `pdstools-3.0.2/python/pdstools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Python pdstools"""
 
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 
-from polars.polars import toggle_string_cache
-
-toggle_string_cache(True)
+from polars import enable_string_cache
+enable_string_cache(True)
 
 import sys
 from pathlib import Path
 
 from .adm.ADMDatamart import ADMDatamart
 from .adm.ADMTrees import ADMTrees, MultiTrees
 from .pega_io import getToken, readClientCredentialFile, readDSExport
 from .pega_io import File, API, S3
 from .utils import cdh_utils, datasets, errors, hds_utils
 from .utils.cdh_utils import defaultPredictorCategorization
 from .utils.datasets import CDHSample, SampleTrees, SampleValueFinder
 from .utils.hds_utils import Config, DataAnonymization
 from .valuefinder.ValueFinder import ValueFinder
+from .utils.polars_ext import *
 
 if "streamlit" in sys.modules:
     from .utils import streamlit_utils
 
 __reports__ = Path(__file__).parents[0] / "reports"
```

### Comparing `pdstools-3.0.1/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.0.2/python/pdstools/adm/ADMDatamart.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,16 +366,16 @@
             self.import_strategy = "eager"
 
         elif isinstance(name, pl.LazyFrame):
             df = name.lazy()
 
         else:
             return None, None, None
-
-        self.model_snapshots = True
+        if df is None:
+            return None, None, None
 
         df = cdh_utils._polarsCapitalize(df)
         cols, missing = self._available_columns(
             df, include_cols=include_cols, drop_cols=drop_cols
         )
         if subset:
             df = df.select(cols)
@@ -671,14 +671,16 @@
             modeldata_cache = pega_io.cache_to_file(
                 self.modelData, path, name=f"cached_modelData_{time}"
             )
         if self.predictorData is not None:
             predictordata_cache = pega_io.cache_to_file(
                 self.predictorData, path, name=f"cached_predictorData_{time}"
             )
+        else:
+            predictordata_cache = None
         return modeldata_cache, predictordata_cache
 
     def _apply_query(
         self,
         df: any_frame,
         query: Optional[Union[pl.Expr, List[pl.Expr], str, Dict[str, list]]] = None,
     ) -> pl.LazyFrame:
@@ -1311,14 +1313,16 @@
         name: Optional[str] = None,
         output_location: Path = Path("."),
         working_dir: Path = Path("."),
         delete_temp_files=True,
         output_type="html",
         include_tables=True,
         allow_collect=True,
+        *,
+        modelData_only: bool = False,
         **kwargs,
     ):
         """Manually generates a Health Check
 
         The recommended way to run the Health Check is through the Streamlit app,
         which you get to by running `pdstools run` in your terminal/command line.
         However, it's also possible to directly run the Health Check from the
@@ -1354,42 +1358,60 @@
             If false, you can always get the tables directly by calling
             :meth:`.exportTables`
         allow_collect : bool, default = True
             An override for the `lazy` memory_strategy. If set to True, still allows
             for collecting of data. Naturally, we need to collect the data in order
             to cache it to disk for the health check, so if set to False
             with a `lazy` memory_strategy, you won't be able to generate.
+        Keyword arguments
+        -----------------
+        modelData_only: bool, default = False
+            If set to True, calls model-based Health Check files. Can be used if 
+            predictor binning data is missing
 
         Returns
         -------
         str:
             The full path to the generated Health Check file.
         """
 
         def delete_temp_files(working_dir, files):
-            for f in ["params.yaml", "HealthCheck.qmd", "HealthCheck.ipynb", "log.txt"]:
+            temp_files = files + (
+                "params.yaml",
+                "HealthCheck.qmd",
+                "HealthCheck.ipynb",
+                "HealthCheckModel.qmd",
+                "HealthCheckModel.ipynb",
+                "log.txt",
+            )
+            for f in temp_files:
                 try:
                     os.remove(f"{working_dir}/{f}")
                 except:
                     pass
-            for f in files:
-                os.remove(f)
+
+        working_dir, output_location = Path(working_dir), Path(output_location)
 
         from pdstools import __reports__
 
         verbose = kwargs.get("verbose", self.verbose)
-
-        if self.modelData is None or self.predictorData is None:
-            raise AssertionError("Needs both model and predictor data.")
+        if modelData_only:
+            healthcheck_file = "HealthCheckModel.qmd"
+            if self.modelData is None:
+                raise AssertionError("Needs model data.")
+        else:
+            healthcheck_file = "HealthCheck.qmd"
+            if self.modelData is None or self.predictorData is None:
+                raise AssertionError("Needs both model and predictor data.")
         if self.import_strategy == "lazy" and not allow_collect:
             raise NotEagerError("Generating healthcheck")
         if not os.path.exists(working_dir):
             os.mkdir(working_dir)
 
-        shutil.copy(__reports__ / "HealthCheck.qmd", working_dir)
+        shutil.copy(__reports__ / healthcheck_file, working_dir)
         if name is not None:
             output_filename = f"HealthCheck_{name.replace(' ', '_')}.{output_type}"
         else:
             output_filename = f"ADM_HealthCheck.{output_type}"
 
         files = self.save_data(working_dir)
 
@@ -1397,15 +1419,15 @@
             "kwargs": {"subset": False, "predictorCategorization": None},
             "include_tables": include_tables,
         }
 
         with open(f"{working_dir}/params.yaml", "w") as f:
             yaml.dump(params, f)
 
-        bashCommand = f"quarto render HealthCheck.qmd --to {output_type} --output {output_filename} --execute-params params.yaml"
+        bashCommand = f"quarto render {healthcheck_file} --to {output_type} --output {output_filename} --execute-params params.yaml"
         if not verbose:
             stdout, stderr = subprocess.DEVNULL, subprocess.STDOUT
         else:
             print("Set verbose=False to hide output.")
             print("Running:", bashCommand)
             stdout, stderr = subprocess.PIPE, None
         if kwargs.get("output_to_file", False):
@@ -1451,17 +1473,15 @@
         ----------
         file: Path, default = 'Tables.xlsx'
             The file name of the exported Excel file
 
         """
         from xlsxwriter import Workbook
 
-        tabs = {
-            tab: getattr(self, tab) for tab in dir(Tables) if not tab.startswith("_")
-        }
+        tabs = {tab: getattr(self, tab) for tab in self.ApplicableTables}
         with Workbook(file) as wb:
             for tab, data in tabs.items():
                 data = data.with_columns(
                     pl.col(pl.List(pl.Categorical), pl.List(pl.Utf8))
                     .arr.eval(pl.element().cast(pl.Utf8))
                     .arr.join(", ")
                 )
```

### Comparing `pdstools-3.0.1/python/pdstools/adm/ADMTrees.py` & `pdstools-3.0.2/python/pdstools/adm/ADMTrees.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,17 +283,20 @@
             try:
                 self.model = self.trees["model"]["boosters"][0]["trees"]
             except Exception as e1:
                 try:
                     self.model = self.trees["model"]["model"]["boosters"][0]["trees"]
                 except Exception as e2:
                     try:
-                        self.model = self.trees["model"]["model"]["booster"]["trees"]
+                        self.model = self.trees["model"]["booster"]["trees"]
                     except Exception as e3:
-                        raise (e1, e2, e3)
+                        try:
+                            self.model = self.trees["model"]["model"]["booster"]["trees"]
+                        except Exception as e4:
+                            raise (e1, e2, e3, e4)
 
         if decode:
             logging.info("Decoding the tree splits.")
             self._decodeTrees()
 
         try:
             self.properties = {
```

### Comparing `pdstools-3.0.1/python/pdstools/adm/Tables.py` & `pdstools-3.0.2/python/pdstools/adm/Tables.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,17 +32,43 @@
             "Direction",
             "Treatment",
         ]
 
         return [
             col
             for col in columns
-            if col in self.combinedData.columns
+            if col in self.modelData.columns
             and self.modelData.schema[col] != pl.Null
         ]
+    @property
+    def AvailableTables(self):
+        df = pl.DataFrame(
+            {
+                "model_overview": [1, 0],
+                "predictors_per_configuration": [1, 1],
+                "bad_predictors": [1, 1],
+                "zero_response": [1, 0],
+                "zero_positives": [1, 0],
+                "reach": [1, 0],
+                "minimum_performance": [1, 1],
+                "appendix": [1, 0],
+            }
+        )
+        df = df.transpose().with_columns(pl.Series(df.columns))
+        df.columns = ["modelData", "predictorData", "Tables"]
+        return df.select(["Tables", "modelData", "predictorData"])
+    
+    @property
+    def ApplicableTables(self):
+        df = self.AvailableTables
+        if not self.hasModels:
+            df = df.filter(pl.col("modelData") == 0)
+        if not self.hasPredictorBinning:
+            df = df.filter(pl.col("predictorData") == 0)
+        return df.get_column("Tables").to_list()
 
     @cached_property
     def model_overview(self):
         return (
             self.last(strategy="lazy")
             .groupby(["Configuration", "Channel", "Direction"])
             .agg(
```

### Comparing `pdstools-3.0.1/python/pdstools/app/cli.py` & `pdstools-3.0.2/python/pdstools/app/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
     print("Running app.")
     print(args)
     filename = Home.__file__
     sys.argv = ["streamlit", "run", filename]
     if len(args) > 1:
         sys.argv.extend(args[1:])
+    if "--server.maxUploadSize" not in sys.argv:
+        sys.argv.extend(["--server.maxUploadSize", "2000"])
     sys.exit(stcli.main())
 
 
 def help(*args):
     msg = (
         "Command line utility to run pdstools apps. ",
         "Currently, only the health check is provided, ",
```

### Comparing `pdstools-3.0.1/python/pdstools/app/pages/Health Check.py` & `pdstools-3.0.2/python/pdstools/app/pages/Health Check.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,18 +82,24 @@
     what values you want to keep in the Health Check.
     """
 
     if "dm" in st.session_state:
         st.session_state["filters"] = streamlit_utils.filter_dataframe(
             st.session_state["dm"].modelData
         )
+    else:
+        st.warning("Please configure your files in the `data import` tab.")
 
 
 with report:
     "# Generating the Health Check"
+    if "dm" not in st.session_state:
+        st.warning("Please configure your files in the `data import` tab.")
+        st.stop()
+
     """Time to start the Health Check. """
     with st.expander("Health Check options"):
         name = st.text_input("Customer name")
         if name == "":
             name = None
         output_type = st.selectbox("Select output type", ["html"], index=0)
         working_dir = Path(st.text_input("Change working directory", "healthCheckDir"))
@@ -123,14 +129,15 @@
                         name=name,
                         output_type=output_type,
                         working_dir=working_dir,
                         output_location=working_dir,
                         delete_temp_files=delete_temp_files,
                         include_tables=include_tables,
                         output_to_file=True,
+                        modelData_only=st.session_state["modelhc"],
                     )
                 )
                 if os.path.isfile(outfile):
                     file = open(outfile, "rb")
             except Exception as e:
                 st.error(f"""Error occured when generating healthcheck: {e}""")
                 with open(working_dir / "log.txt", "rb") as f:
```

### Comparing `pdstools-3.0.1/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.0.2/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/ih/legacy_IH.py` & `pdstools-3.0.2/python/pdstools/ih/legacy_IH.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/pega_io/API.py` & `pdstools-3.0.2/python/pdstools/pega_io/API.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/pega_io/File.py` & `pdstools-3.0.2/python/pdstools/pega_io/File.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/pega_io/S3.py` & `pdstools-3.0.2/python/pdstools/pega_io/S3.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/plots/plot_base.py` & `pdstools-3.0.2/python/pdstools/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/plots/plots_plotly.py` & `pdstools-3.0.2/python/pdstools/plots/plots_plotly.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.0.2/python/pdstools/reports/HealthCheck.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -552,14 +552,15 @@
 ## Empty and Immature Models
 All below lists are guidance. There should be just a small percentage of immature or empty models overall. Having no or just 1 active predictor is very suspicious
 
 ### Models that have never been used
 These models have no responses at all: no positives but also no negatives. The models for these actions/treatments exist, so they must have been created in the evaluation of the actions/treatments, but they were never selected to show to the customer, so never received any responses.
 
 Often these represent actions that never made it into production and were only used to test out logic. But it could also be that the response mechanism is broken. It could for example be caused by outcome labels that are returned by the channel application not matching the configuration of the adaptive models.
+
 ```{python}
 if include_tables:
     zero_response = datamart.zero_response.to_pandas(use_pyarrow_extension_array=True)
 
     if zero_response.shape[0] >0:
         print(f"There are {zero_response.shape[0]} models with zero response")
         show(zero_response, scrollX = True)
```

### Comparing `pdstools-3.0.1/python/pdstools/utils/cdh_utils.py` & `pdstools-3.0.2/python/pdstools/utils/cdh_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/utils/datasets.py` & `pdstools-3.0.2/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/utils/hds_utils.py` & `pdstools-3.0.2/python/pdstools/utils/hds_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/utils/pega_template.py` & `pdstools-3.0.2/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.1/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.0.2/python/pdstools/utils/streamlit_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 def cachedDatamart(*args, **kwargs):
     print("Importing datamart.")
     return ADMDatamart(*args, **kwargs)
 
 
 def import_datamart(**opts):
     st.session_state["params"] = {}
+    st.session_state["modelhc"] = False
     st.write("### Data import")
 
     source = st.selectbox(
         "Select data source",
         options=[
             "Direct file path",
             "Direct file upload",
@@ -47,21 +48,36 @@
     model_file = st.file_uploader(
         "Upload Model Snapshot", type=["json", "zip", "parquet", "csv", "arrow"]
     )
     predictor_file = st.file_uploader(
         "Upload Predictor Binning snapshot",
         type=["json", "zip", "parquet", "csv", "arrow"],
     )
-    if model_file is not None and predictor_file is not None:
+    if model_file and predictor_file:
         try:
             st.session_state["dm"] = cachedDatamart(
                 model_df=model_file, predictor_df=predictor_file, **opts
             )
         except Exception as e:
             st.write("Oh oh.", e)
+    elif model_file is not None and predictor_file is None:
+        st.warning("""Please also upload the Predictor Binning file. 
+                If you don't have access to a predictor binning file
+                and want to run the Health Check only on the model snapshot, check the
+                checkbox below.
+                """)
+        model_analysis = st.checkbox("Only run model-based Health Check")
+        if model_analysis:
+            try:
+                st.session_state["dm"] = cachedDatamart(
+                    model_df=model_file, predictor_filename=None, **opts
+                )
+                st.session_state["modelhc"] = True
+            except Exception as e:
+                st.write("Oh oh.", e)
 
 
 def fromFilePath(**opts):
     st.write(
         """If you've followed the instructions on how to get the ADMDatamart data,
     you can import the data simply by pointing the app to the directory
     where the original files are located, and we can find it automatically."""
@@ -99,28 +115,49 @@
             data.write(f"Predictor binning found: {predictor_matches}")
         else:
             box.write("## X")
             data.write(
                 "Could not find the predicting binning snapshot in the given folder."
             )
 
-        if model_matches is None and predictor_matches is None:
+        if model_matches is None:
             st.write(
                 """If you can't get the files to automatically be detected, 
     try uploading the files manually using a different data source."""
             )
+
+        elif predictor_matches is None:
+            st.warning(
+                """No predictor binning file found, please also upload the Predictor
+                Binning file. If you have a predictor binning snapshot but we can't
+                detect it, use the **Direct file upload** option in the dropdown above.
+                If you don't have access to a predictor binning file
+                and want to run the Health Check only on the model snapshot, check the
+                checkbox below.
+                """
+            )
+            model_analysis = st.checkbox("Only run model-based Health Check")
+            if model_analysis:
+                st.session_state["dm"] = cachedDatamart(
+                    path=dir,
+                    model_filename=Path(model_matches).name,
+                    predictor_filename=None,
+                    import_strategy="lazy",
+                    **opts,
+                )
+                st.session_state["modelhc"] = True
+
         else:
             st.session_state["dm"] = cachedDatamart(
                 path=dir,
                 model_filename=Path(model_matches).name,
                 predictor_filename=Path(predictor_matches).name,
                 import_strategy="lazy",
                 **opts,
             )
-            # st.write(st.session_state["params"])
 
 
 def filter_dataframe(df: pl.LazyFrame, schema: Optional[dict] = None) -> pl.LazyFrame:
     """
     Adds a UI on top of a dataframe to let viewers filter columns
 
     Parameters
```

### Comparing `pdstools-3.0.1/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.0.2/python/pdstools/valuefinder/ValueFinder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from tqdm.auto import tqdm
-import time
+import functools
+import operator
+from os import PathLike
+from typing import Literal, Optional, Union
+
 import numpy as np
 import pandas as pd
-import polars as pl
-import math
 import plotly.express as px
 import plotly.figure_factory as ff
 import plotly.graph_objects as go
+import polars as pl
 from plotly.subplots import make_subplots
-from typing import Optional, Union
+
 from .. import pega_io
 from ..utils import cdh_utils
-from os import PathLike
 
 
 class ValueFinder:
     """Class to analyze Value Finder datasets.
 
     Relies heavily on polars for faster reading and transformations.
     See https://pola-rs.github.io/polars/py-polars/html/index.html
@@ -27,84 +28,101 @@
     Parameters
     ----------
     path : Optional[str]
         Path to the ValueFinder data files
     df : Optional[DataFrame]
         Override to supply a dataframe instead of a file.
         Supports pandas or polars dataframes
+    import_strategy: Literal['eager', 'lazy'], default = 'eager'
+        Whether to import the file fully to memory, or scan the file
+        When data fits into memory, 'eager' is typically more efficient
+        However, when data does not fit, the lazy methods typically allow
+        you to still use the data.
     verbose : bool
         Whether to print out information during importing
 
     Keyword arguments
     -----------------
+    th: float
+        An optional keyword argument to override the propensity threshold
     filename : Optional[str]
         The name, or extended filepath, towards the file
     subset : bool
         Whether to select only a subset of columns.
         Will speed up analysis and reduce unused information
     """
 
     def __init__(
         self,
         path: Optional[str] = None,
         df: Optional[Union[pd.DataFrame, pl.DataFrame, pl.LazyFrame]] = None,
         verbose: bool = True,
+        import_strategy: Literal["eager", "lazy"] = "eager",
         **kwargs,
     ):
         if path is None and df is None:
             raise ValueError(
                 "Please supply a path to the data files or the df directly."
             )
 
+        self.import_strategy = import_strategy
+
         keep_cols = [
             "pyStage",
             "pyIssue",
             "pyGroup",
             "pyChannel",
             "pyDirection",
             "CustomerID",
             "pyName",
             "pyWorkID",
             "pyModelPropensity",
             "pyPropensity",
             "FinalPropensity",
         ]
-        self.df = kwargs.pop("df", df)
-        if self.df is None:
-            start = time.time()
+
+        if df is not None:
+            self.df = pega_io.readDSExport(df, verbose=verbose)
+        else:
             filename = kwargs.pop("filename", "ValueFinder")
-            self.df = pega_io.readDSExport(filename, path, return_pl=True, verbose=verbose)
-            if verbose:
-                print(f"Data import took {round(time.time() - start,2)} seconds")
-
-        if verbose:
-            print("Transforming to polars...", end=" ")
-        start = time.time()
-        if isinstance(self.df, pl.LazyFrame):
-            self.df = self.df.collect()
-        elif not isinstance(self.df, pl.DataFrame):
-            self.df = pl.DataFrame(self.df)
+            self.df = pega_io.readDSExport(filename, path, verbose=verbose)
+
         if kwargs.get("subset", True):
             self.df = self.df.select(keep_cols)
-        if verbose:
-            print(f"Took: {round(time.time() - start,2)} seconds")
 
-        self.th = self.df.filter(pl.col("pyStage") == "Eligibility")[
-            "pyModelPropensity"
-        ].quantile(0.05)
-
-        self.ncust = 10 ** math.ceil(math.log10(pl.n_unique(self.df["CustomerID"])))
-        self.customersummary = self.getCustomerSummary(self.th, verbose)
-        self.countsPerStage = self.getCountsPerStage(self.customersummary, verbose)
-        self.countsPerThreshold = dict()
+        if "th" not in kwargs:
+            self.th = self.df.filter(pl.col("pyStage") == "Eligibility").select(
+                pl.quantile("pyModelPropensity", 0.05).alias("th")
+            )
+        else:
+            self.th = pl.LazyFrame({"th": kwargs.pop("th")})
+
+        self.ncust = self.df.select(
+            (pl.lit(10) ** pl.col("CustomerID").n_unique().log10().ceil())
+            .cast(pl.UInt32)
+            .alias("ncust")
+        )
+
         self.NBADStages = ["Eligibility", "Applicability", "Suitability", "Arbitration"]
         self.maxPropPerCustomer = self.df.groupby(["CustomerID", "pyStage"]).agg(
             pl.max("pyModelPropensity").alias("MaxModelPropensity")
         )
 
+        if import_strategy == "eager":
+            self.df = self.df.collect().lazy()
+            self.th = self.th.collect().lazy()
+            self.ncust = self.ncust.collect().lazy()
+            self.maxPropPerCustomer = self.maxPropPerCustomer.collect().lazy()
+
+        self.customersummary = self.getCustomerSummary(self.th)
+        self.countsPerStage = self.getCountsPerStage(self.customersummary)
+
+        self._thMap = dict()
+        self.countsPerThreshold = dict()
+
     def save_data(self, path: str = ".") -> PathLike:
         """Cache the ValueFinder dataset to a file
 
         Parameters
         ----------
         path : str
             Where to place the file
@@ -117,158 +135,181 @@
         from datetime import datetime
 
         time = cdh_utils.toPRPCDateTime(datetime.now())
         out = pega_io.cache_to_file(self.df, path, name=f"cached_ValueFinder_{time}")
         return out
 
     def getCustomerSummary(
-        self, th: Optional[float] = None, verbose: bool = True
+        self,
+        th: Optional[float] = None,
     ) -> pl.DataFrame:
         """Computes the summary of propensities for all customers
 
         Parameters
         ----------
         th: Optional[float]
             The threshold to consider an action 'good'.
             If a customer has actions with propensity above this,
             the customer has at least one relevant action.
             If not given, will default to 5th quantile.
-        verbose: bool, default = True
-            Whether to print out the execution times
         """
-        th = th or self.th
-        if verbose:
-            print("Generating: Customer Summary...", end=" ")
-        start = time.time()
+        if th is None:
+            th = self.th
+        if isinstance(th, float):
+            th = pl.LazyFrame({"th": th})
 
         df = (
-            self.df.groupby(["CustomerID", "pyStage"])
+            self.df.with_context(th)
+            .groupby(["CustomerID", "pyStage"])
             .agg(
                 [
                     pl.max("pyPropensity").alias("MaxPropensity"),
                     pl.max("FinalPropensity").alias("MaxFinalPropensity"),
                     pl.max("pyModelPropensity").alias("MaxModelPropensity"),
                     pl.count("pyPropensity").alias("NOffers"),
                 ]
             )
             .with_columns(
                 [
-                    (pl.col("MaxModelPropensity") >= th).alias("relevantActions"),
-                    (pl.col("MaxModelPropensity") < th).alias("irrelevantActions"),
+                    (pl.col("MaxModelPropensity") >= pl.col("th")).alias(
+                        "relevantActions"
+                    ),
+                    (pl.col("MaxModelPropensity") < pl.col("th")).alias(
+                        "irrelevantActions"
+                    ),
                 ]
             )
         )
-        if verbose:
-            print(f"Took: {round(time.time() - start,2)} seconds")
 
-        return df
+        if self.import_strategy == "eager":
+            return df.collect().lazy()
+        else:
+            return df
 
     def getCountsPerStage(
-        self, customersummary: Optional[pl.DataFrame] = None, verbose: bool = True
+        self,
+        customersummary: Optional[pl.DataFrame] = None,
     ) -> pl.DataFrame:
         """Generates an aggregated view per stage.
 
         Parameters
         ----------
         customersummary : Optional[pl.DataFrame]
             Optional override of the customer summary,
             which can be generated by getCustomerSummary().
-        verbose : bool, default = True
-            Whether to print execution times.
         """
         if customersummary is None:
             customersummary = self.customersummary
-        if verbose:
-            print("Generating: Counts per stage...", end=" ")
-        start = time.time()
 
         df = (
             customersummary.groupby("pyStage")
             .agg(
                 [
                     pl.sum("relevantActions"),
                     pl.sum("irrelevantActions"),
                     pl.count("relevantActions").alias("NoActions"),
                 ]
             )
-            .with_column((self.ncust - pl.col("NoActions")).alias("NoActions"))
+            .with_context(self.ncust)
+            .with_columns((pl.col("ncust") - pl.col("NoActions")).alias("NoActions"))
         )
-        if verbose:
-            print(f"Took: {round(time.time() - start,2)} seconds")
-        return df
+        if self.import_strategy == "eager":
+            return df.collect().lazy()
+        else:
+            return df
 
-    def addCountsPerThresholdRange(
-        self, start: float, stop: float, step: float, verbose: bool = True
-    ):
-        """Adds the counts per stage for a range of quantiles.
+    def getThFromQuantile(self, quantile: float) -> float:
+        """Return the propensity threshold corresponding to a given quantile
+
+        If the threshold is already in `self._thMap`, simply gets it from there
+        Otherwise, computes the threshold and then adds it to the map.
+
+        Parameters
+        ----------
+        quantile: float
+            The quantile to get the threshold for
+
+        """
+        import functools
+        import operator
+
+        if quantile not in functools.reduce(operator.iconcat, self._thMap.values(), []):
+            th = (
+                self.df.filter(pl.col("pyStage") == "Eligibility")
+                .select(pl.col("pyModelPropensity").quantile(quantile))
+                .collect()
+                .item()
+            )
+            if th in self._thMap.keys():
+                self._thMap[th].append(quantile)
+            else:
+                self._thMap[th] = [quantile]
+        return [th for th, quantiles in self._thMap.items() if quantile in quantiles][0]
+
+    def getCountsPerThreshold(self, th, return_df=False) -> Optional[pl.LazyFrame]:
+        if th not in self.countsPerThreshold.keys():
+            df = (
+                (
+                    self.maxPropPerCustomer.with_columns(
+                        [
+                            (pl.col("MaxModelPropensity") >= th).alias(
+                                "relevantActions"
+                            ),
+                            (pl.col("MaxModelPropensity") < th).alias(
+                                "irrelevantActions"
+                            ),
+                        ]
+                    )
+                )
+                .groupby("pyStage")
+                .agg(
+                    [
+                        pl.sum("relevantActions"),
+                        pl.sum("irrelevantActions"),
+                        pl.count("relevantActions").alias("NoActions"),
+                    ]
+                )
+                .with_context(self.ncust)
+                .with_columns(
+                    (pl.col("ncust") - pl.col("NoActions")).alias("NoActions")
+                )
+            )
+            if self.import_strategy == "eager":
+                self.countsPerThreshold[th] = df.collect().lazy()
+            else:
+                self.countsPerThreshold[th] = df
+        if return_df:
+            return self.countsPerThreshold[th]
+
+    def addCountsForThresholdRange(
+        self, start, stop, step, method=Literal["threshold, quantile"]
+    ) -> None:
+        """Adds the counts per stage for a range of quantiles or thresholds.
 
-        In the background, uses numpy's arange function
-        to generate the range of quantiles.
-        Then, for each quantile the counts per stage are computed,
-        and added to the 'countsPerThreshold' dictionary.
-        As optimization, if a quantile produces a threshold that is
-        already previously computed, it simply adds that computed dataframe.
+        Once computed, the values are added to `.countsPerThreshold` so we
+        only need to compute each value once.
 
         Parameters
         ----------
         start : float
-            The starting quantile
+            The starting of the range
         stop : float
-            The ending quantile
+            The end of the range
         step : float
             The steps to compute between start and stop
-        verbose : bool, default = True
-            Whether to print out the progress of computation
+        method: Literal["threshold", "quantile"]:
+            Whether to get a range of thresholds directly or compute
+            the thresholds from their quantiles
         """
-        to_add = set(np.arange(start, stop, step)) - self.countsPerThreshold.keys()
-        if len(to_add) > 0:
-            self.skippedquantiles = []
-            for quantile in tqdm(to_add, disable=not verbose):
-                th = self.df.filter(pl.col("pyStage") == "Eligibility")[
-                    "pyModelPropensity"
-                ].quantile(quantile)
-
-                skipped = False
-                for quantile2, data in self.countsPerThreshold.items():
-                    if data[0] == th:
-                        self.countsPerThreshold[quantile] = (th, data[1])
-                        skipped = True
-                        self.skippedquantiles.append((quantile2, th))
-                        break
-
-                if not skipped:
-                    self.countsPerThreshold[quantile] = (
-                        th,
-                        (
-                            self.maxPropPerCustomer.with_columns(
-                                [
-                                    (pl.col("MaxModelPropensity") >= th).alias(
-                                        "relevantActions"
-                                    ),
-                                    (pl.col("MaxModelPropensity") < th).alias(
-                                        "irrelevantActions"
-                                    ),
-                                ]
-                            )
-                        )
-                        .groupby("pyStage")
-                        .agg(
-                            [
-                                pl.sum("relevantActions"),
-                                pl.sum("irrelevantActions"),
-                                pl.count("relevantActions").alias("NoActions"),
-                            ]
-                        )
-                        .with_column(
-                            (self.ncust - pl.col("NoActions")).alias("NoActions")
-                        ),
-                    )
-        else:
-            if verbose:
-                print("All thresholds already computed.")
+        import numpy as np
+
+        to_add = np.arange(start, stop, step)
+        if method == "quantile":
+            to_add = list(map(self.getThFromQuantile, to_add))
+        list(map(self.getCountsPerThreshold, to_add))
 
     def plotPropensityDistribution(self, sampledN: int = 10_000) -> go.Figure:
         """Plots the distribution of the different propensities.
 
         For optimization reasons (storage for all points in a boxplot and
         time complexity for computing the distribution plot),
         we have to sample to a reasonable amount of data points.
@@ -281,16 +322,15 @@
         """
         i = 0
         figs = make_subplots(
             rows=len(self.NBADStages), cols=1, shared_xaxes=True, vertical_spacing=0.005
         )
         for stage in self.NBADStages:
             data = self.df.filter(pl.col("pyStage") == stage)
-            if len(data) > sampledN:
-                data = data.sample(sampledN)
+            data = data.pdstools.sample(sampledN).collect()
             temp = ff.create_distplot(
                 [data["pyModelPropensity"].to_list()],
                 ["pyModelPropensity"],
                 show_rug=False,
                 show_hist=False,
             )
             tempdf = pd.DataFrame(
@@ -330,17 +370,21 @@
         """
         colors = ["#001F5F", "#10A5AC", "#F76923"]
         propensities = ["FinalPropensity", "pyPropensity", "pyModelPropensity"]
 
         i = 0
         figs = make_subplots(rows=len(propensities), cols=1, shared_xaxes=True)
         yrange = [0, 15]
-        data = self.df.filter(pl.col("pyStage") == stage).select(propensities)
-        if len(data) > sampledN:
-            data = data.sample(sampledN)
+        th = self.th.pdstools.item()
+        data = (
+            self.df.filter(pl.col("pyStage") == stage)
+            .select(propensities)
+            .pdstools.sample(sampledN)
+            .collect()
+        )
         for ptype in propensities:
             plotdf = data[ptype].to_list()
             temp = ff.create_distplot(
                 [plotdf], ["value"], show_rug=False, show_hist=False
             )
             tempdf = pd.DataFrame(
                 {"x": temp["data"][0]["x"], "y": temp["data"][0]["y"]}
@@ -366,16 +410,16 @@
                 ),
                 row=i + 1,
                 col=1,
             )
             figs.update_yaxes(range=yrange, col=1, row=i + 1)
             figs.add_shape(
                 type="line",
-                x0=self.th,
-                x1=self.th,
+                x0=th,
+                x1=th,
                 y0=yrange[0],
                 y1=yrange[1],
                 line=dict(dash="dot"),
                 col=1,
                 row=i + 1,
             )
             i += 1
@@ -389,211 +433,256 @@
             legend_title="Type",
             height=800,
         )
         return figs
 
     def plotPieCharts(
         self,
-        start: Optional[float] = None,
-        stop: Optional[float] = None,
-        step: Optional[float] = None,
-        verbose: bool = True,
-    ):
-        """Plots the pie chart, split per stage.
-
-        If start, stop and step are supplied,
-        it will generate a slider to set the threshold
-        dynamically throughout the given range of quantiles.
-        If any of the is None, it will simply use the default
-        threshold based on the 5th quantile.
+        start: float = None,
+        stop: float = None,
+        step: float = None,
+        *,
+        method: Literal["threshold", "quantile"] = "threshold",
+        rounding: int = 3,
+        th: Optional[float] = None,
+    ) -> go.FigureWidget:
+        """Plots pie charts showing the distribution of customers
+
+        The pie charts each represent the fraction of customers with
+        the color indicating whether they have sufficient relevant actions
+        in that stage of the NBAD arbitration.
+
+        If no values are provided for start, stop or step, the pie charts are
+        shown using the default propensity threshold, as part of the Value Finder
+        class.
 
         Parameters
         ----------
         start : float
-            The starting quantile
+            The starting of the range
         stop : float
-            The ending quantile
+            The end of the range
         step : float
             The steps to compute between start and stop
-        verbose : bool, default = True
-            Whether to print out the progress of computation
+
+        Keyword arguments
+        -----------------
+        method : Literal['threshold', 'quantile'], default='threshold'
+            Whether the range is computed based on the threshold directly
+            or based on the quantile of the propensity
+        rounding : int
+            The number of digits to round the values by
+        th : Optional[float]
+            Choose a specific propensity threshold to plot
         """
+        default = th or self.th.pdstools.item()
         if None in (start, stop, step):
             if start is not None:
                 start, stop = start, start + 1
             else:
-                start, stop = self.th, self.th + 1
+                start, stop = default, default + 1
             step = 10000
-
+        iter = np.arange(start, stop, step)
         fig = make_subplots(
             rows=1,
             cols=len(self.NBADStages),
             specs=[[{"type": "domain"}] * len(self.NBADStages)],
             subplot_titles=self.NBADStages,
         )
-        self.addCountsPerThresholdRange(start, stop, step, verbose=verbose)
-        founddefault = False
-        rounding = 3
-        arange = np.arange(start, stop, step)
-        for i, quantile in enumerate(arange):
-            if self.countsPerThreshold[quantile][0] == self.th:
-                visible, founddefault = True, True
+
+        found_default = None
+        default_n = 0
+        steps = []
+        for n, iter_val in enumerate(iter):
+            if method == "quantile":
+                threshold = self.getThFromQuantile(iter_val)
+            else:
+                threshold = iter_val
+            if threshold == default:
+                visible, found_default, default_n = True, True, n
             else:
                 visible = False
+            df = (
+                self.getCountsPerThreshold(threshold, True)
+                .collect()
+                .partition_by("pyStage", as_dict=True)
+            )
             for i, stage in enumerate(self.NBADStages):
-                data = (
-                    self.countsPerThreshold[quantile][1]
-                    .filter(pl.col("pyStage") == stage)
-                    .drop("pyStage")
-                )
+                plotdf = df[stage].drop("pyStage")
                 fig.add_trace(
                     go.Pie(
-                        values=list(data.to_numpy())[0],
+                        values=list(plotdf.to_numpy())[0],
                         labels=list(
-                            data.rename(
+                            plotdf.rename(
                                 {
                                     "relevantActions": "At least one relevant action",
                                     "irrelevantActions": "Only irrelevant actions",
                                     "NoActions": "Without actions",
                                 }
                             ).columns
                         ),
                         name=stage,
                         visible=visible,
                         sort=False,
                     ),
                     1,
                     i + 1,
                 )
-        steps = []
-        for i, quantile in enumerate(arange):
+
+            visibleStages = [False] * len(iter) * 4
+            for x in range(n * 4, n * 4 + 4):
+                visibleStages[x] = True
+            title = "Distribution of customers per stage "
+            if method == "threshold":
+                title += f"at propensity threshold: {round(threshold,rounding):.1%}"
+            else:
+                title += f"at quantile: {round(iter_val,rounding)} (threshold: {round(threshold,rounding):.1%})"
             step = dict(
                 method="update",
-                label=str(round(quantile, rounding)),
+                label=str(round(iter_val, rounding)),
                 args=[
-                    {"visible": [False] * len(fig.data)},
-                    {
-                        "title": f"Propensity percentile: {str(round(quantile,rounding))}, propensity: {self.countsPerThreshold[quantile][0]}"
-                    },
+                    {"visible": visibleStages},
+                    {"title": title},
                 ],
             )
-            for x in range(i * 4, i * 4 + 4):
-                step["args"][0]["visible"][x] = True
             steps.append(step)
         sliders = [
             dict(
-                active=list(arange)[0],
-                currentvalue={"prefix": "Propensity percentile: "},
+                active=default_n,
+                currentvalue={"prefix": f"Propensity {method}: "},
                 pad={"t": 50},
                 steps=steps,
             )
         ]
-
-        fig.update_layout(sliders=sliders)
+        fig.update_layout(
+            sliders=sliders,
+            title_text=f"Distribution of customers per stage at propensity threshold {round(float(default), rounding):.1%}",
+        )
         fig.update_traces(marker=dict(colors=["#219e3f", "#fca52e", "#cd001f"]))
-        if not founddefault:
+
+        if not found_default:
             for i in range(0, 4):
                 fig.data[i].visible = True
+        for i in range(len(fig.layout.sliders[0].steps)):
+            fig.layout.sliders[0].steps[
+                i
+            ].label = f"{float(fig.layout.sliders[0].steps[i].label):.1%}"
         return fig
 
-    def plotDistributionPerThreshold(self, target: str = "Quantile", **kwargs):
+    def plotDistributionPerThreshold(
+        self,
+        start: float = None,
+        stop: float = None,
+        step: float = None,
+        *,
+        method: Literal["threshold", "quantile"] = "threshold",
+        rounding=3,
+    ) -> go.FigureWidget:
         """Plots the distribution of customers per threshold, per stage.
 
         Based on the precomputed data in self.countsPerThreshold,
         this function will plot the distribution per stage.
 
         To add more data points between a given range,
         simply pass all three arguments to this function:
-        start, stop and step. Alternatively, you may
-        call the self.addCountsPerThresholdRange() function,
-        with the start, stop and step arguments outside of this call.
+        start, stop and step.
 
         Parameters
         ----------
-        target : str, default = Quantile
-            Determines which threshold to plot:
-            based on the quantiles or the raw propensities.
-            One of: {'Quantile', 'Propensity'}
-
-        Keyword arguments
-        -----------------
         start : float
-            The starting quantile
+            The starting of the range
         stop : float
-            The ending quantile
+            The end of the range
         step : float
             The steps to compute between start and stop
-        verbose : bool, default = True
-            Whether to print out the progress of computation
+
+        Keyword arguments
+        -----------------
+        method : Literal['threshold', 'quantile'], default='threshold'
+            Whether the range is computed based on the threshold directly
+            or based on the quantile of the propensity
+        rounding : int
+            The number of digits to round the values by
         """
-        if {"start", "stop", "step"}.issubset(kwargs):
-            self.addCountsPerThresholdRange(
-                kwargs.get("start"), kwargs.get("stop"), kwargs.get("step")
-            )
-        self.addCountsPerThresholdRange(0.01, 1, 0.1)
-
-        df = list()
-        for quantile, data in self.countsPerThreshold.items():
-            target2 = data[0] if target.casefold() == "propensity" else quantile
-            df.append(data[1].with_column(pl.lit(target2).alias(target)))
-        df = pl.concat(df).to_pandas().set_index(target)
+
+        if None not in (start, stop, step):
+            self.addCountsForThresholdRange(start, stop, step, method)
+        self.addCountsForThresholdRange(0.01, 1, 0.1, "quantile")
+        if method == "threshold":
+            df = [
+                df.with_columns(threshold=pl.lit(th).round(rounding))
+                for th, df in self.countsPerThreshold.items()
+            ]
+        else:
+            df = []
+            for quantile in functools.reduce(
+                operator.iconcat, self._thMap.values(), []
+            ):
+                th = self.getThFromQuantile(quantile)
+                df.append(
+                    self.getCountsPerThreshold(th, True).with_columns(
+                        quantile=pl.lit(quantile).round(rounding)
+                    )
+                )
+        df = pl.concat(df).collect().to_pandas().set_index(method)
         fig = px.area(
             df.rename(
                 columns={
                     "relevantActions": "At least one relevant action",
                     "irrelevantActions": "Only irrelevant actions",
                     "NoActions": "Without actions",
                 }
             ),
             color_discrete_sequence=["#219e3f", "#fca52e", "#cd001f"],
             facet_col="pyStage",
-            title=f"Distribution of offers per stage",
-            labels={"value": "Number of people"},
+            title="Distribution of offers per stage",
+            labels={"value": "Number of people", method: method.title()},
             category_orders={"pyStage": self.NBADStages},
             template="none",
         )
         fig.update_layout(legend_title_text="Status")
+        if method == "threshold":
+            fig.update_xaxes(tickformat=",.1%")
         return fig
 
-    def plotFunnelChart(self, level: str = "Action", query=None):
+    def plotFunnelChart(self, level: str = "Action", query=None, return_df=False):
         """Plots the funnel of actions or issues per stage.
 
         Parameters
         ----------
         level : str, default = 'Actions'
             Which element to plot:
             - If 'Actions', plots the distribution of actions.
             - If 'Issues', plots the distribution of issues
         """
-        funneldf = pd.DataFrame()
         if level.casefold() in {"action", "name", "pyname"}:
             level, cat = "pyName", "Actions"
         elif level.casefold() in {"issue", "pyissue"}:
             level, cat = "pyIssue", "Issues"
         elif level.casefold() in {"group", "pygroup"}:
             level, cat = "pyGroup", "Groups"
-        ncat = "all"
-        for stage in self.NBADStages:
-            temp = self.df if query is None else self.df.filter(query)
-            temp = (
-                temp.filter(pl.col("pyStage") == stage)[level]
-                .value_counts()
-                .rename({level: "Name", "counts": "Count"})
-                .to_pandas()
-            )
-            temp["Stage"] = stage
-
-            if ncat != "all":
-                funneldf = pd.concat([funneldf, temp[0:ncat]], axis=0).sort_values(
-                    ["Name"]
-                )
-            else:
-                funneldf = pd.concat([funneldf, temp], axis=0).sort_values(["Name"])
+
+        df = self.df if query is None else self.df.filter(query)
+        df = (
+            pl.LazyFrame({"pyStage": self.NBADStages})
+            .join(
+                df.groupby("pyStage")
+                .agg(pl.col(level).value_counts().sort())
+                .explode(level)
+                .unnest(level),
+                on="pyStage",
+            )
+            .rename({level: "Name", "counts": "Count", "pyStage": "Stage"})
+            .collect()
+        )
+        if return_df:
+            return df
+
         fig = px.funnel(
-            funneldf,
+            df.to_pandas(),
             y="Count",
             x="Stage",
             color="Name",
             text="Name",
             title=f"Distribution of {cat.casefold()} over the stages",
             template="none",
         )
```

