# Comparing `tmp/pdstools-3.0.2.tar.gz` & `tmp/pdstools-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.0.2.tar", last modified: Mon Apr 10 12:52:27 2023, max compression
+gzip compressed data, was "pdstools-3.1.0.tar", last modified: Mon Apr 10 15:05:14 2023, max compression
```

## Comparing `pdstools-3.0.2.tar` & `pdstools-3.1.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.508414 pdstools-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 12:52:17.000000 pdstools-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 12:52:27.504413 pdstools-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-10 12:52:17.000000 pdstools-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/pdstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 12:52:27.000000 pdstools-3.0.2/pdstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-10 12:52:17.000000 pdstools-3.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.496413 pdstools-3.0.2/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/python/pdstools/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/python/pdstools/adm/
--rw-r--r--   0 runner    (1001) docker     (123)    57635 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 runner    (1001) docker     (123)    40057 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/adm/Tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/python/pdstools/app/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/app/Home.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.500413 pdstools-3.0.2/python/pdstools/app/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/app/pages/Health Check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/ih/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/ih/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/pega_io/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/pega_io/API.py
--rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/pega_io/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/pega_io/S3.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/plots/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/reports/
--rw-r--r--   0 runner    (1001) docker     (123)    39142 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/reports/HealthCheckModel.qmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/pega_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/polars_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:27.504413 pdstools-3.0.2/python/pdstools/valuefinder/
--rw-r--r--   0 runner    (1001) docker     (123)    24211 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:52:17.000000 pdstools-3.0.2/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:52:27.508414 pdstools-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 15:05:04.000000 pdstools-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 15:05:14.071000 pdstools-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-10 15:05:04.000000 pdstools-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-10 15:05:04.000000 pdstools-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)    57635 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40057 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/app/pages/Health Check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    39142 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/reports/HealthCheckModel.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (123)    24211 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:05:14.071000 pdstools-3.1.0/setup.cfg
```

### Comparing `pdstools-3.0.2/LICENSE` & `pdstools-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/PKG-INFO` & `pdstools-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.0.2
+Version: 3.1.0
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
-Metadata-Version: 2.1 Name: pdstools Version: 3.0.2 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.0 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.0.2/README.md` & `pdstools-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/pdstools.egg-info/PKG-INFO` & `pdstools-3.1.0/pdstools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.0.2
+Version: 3.1.0
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
-Metadata-Version: 2.1 Name: pdstools Version: 3.0.2 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.0 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.0.2/pdstools.egg-info/SOURCES.txt` & `pdstools-3.1.0/pdstools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,11 +32,12 @@
 python/pdstools/utils/__init__.py
 python/pdstools/utils/cdh_utils.py
 python/pdstools/utils/datasets.py
 python/pdstools/utils/errors.py
 python/pdstools/utils/hds_utils.py
 python/pdstools/utils/pega_template.py
 python/pdstools/utils/polars_ext.py
+python/pdstools/utils/show_versions.py
 python/pdstools/utils/streamlit_utils.py
 python/pdstools/utils/types.py
 python/pdstools/valuefinder/ValueFinder.py
 python/pdstools/valuefinder/__init__.py
```

### Comparing `pdstools-3.0.2/pyproject.toml` & `pdstools-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/__init__.py` & `pdstools-3.1.0/python/pdstools/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Python pdstools"""
 
-__version__ = "3.0.2"
+__version__ = "3.1.0"
 
 from polars import enable_string_cache
+
 enable_string_cache(True)
 
 import sys
 from pathlib import Path
 
 from .adm.ADMDatamart import ADMDatamart
 from .adm.ADMTrees import ADMTrees, MultiTrees
 from .pega_io import getToken, readClientCredentialFile, readDSExport
 from .pega_io import File, API, S3
 from .utils import cdh_utils, datasets, errors, hds_utils
 from .utils.cdh_utils import defaultPredictorCategorization
+from .utils.show_versions import show_versions
 from .utils.datasets import CDHSample, SampleTrees, SampleValueFinder
 from .utils.hds_utils import Config, DataAnonymization
 from .valuefinder.ValueFinder import ValueFinder
 from .utils.polars_ext import *
 
 if "streamlit" in sys.modules:
     from .utils import streamlit_utils
```

### Comparing `pdstools-3.0.2/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.1.0/python/pdstools/adm/ADMDatamart.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/adm/ADMTrees.py` & `pdstools-3.1.0/python/pdstools/adm/ADMTrees.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/adm/Tables.py` & `pdstools-3.1.0/python/pdstools/adm/Tables.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/app/cli.py` & `pdstools-3.1.0/python/pdstools/app/cli.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/app/pages/Health Check.py` & `pdstools-3.1.0/python/pdstools/app/pages/Health Check.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.1.0/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/ih/legacy_IH.py` & `pdstools-3.1.0/python/pdstools/ih/legacy_IH.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/pega_io/API.py` & `pdstools-3.1.0/python/pdstools/pega_io/API.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/pega_io/File.py` & `pdstools-3.1.0/python/pdstools/pega_io/File.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/pega_io/S3.py` & `pdstools-3.1.0/python/pdstools/pega_io/S3.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/plots/plot_base.py` & `pdstools-3.1.0/python/pdstools/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/plots/plots_plotly.py` & `pdstools-3.1.0/python/pdstools/plots/plots_plotly.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.1.0/python/pdstools/reports/HealthCheck.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/reports/HealthCheckModel.qmd` & `pdstools-3.1.0/python/pdstools/reports/HealthCheckModel.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/utils/cdh_utils.py` & `pdstools-3.1.0/python/pdstools/utils/cdh_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/utils/datasets.py` & `pdstools-3.1.0/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/utils/hds_utils.py` & `pdstools-3.1.0/python/pdstools/utils/hds_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/utils/pega_template.py` & `pdstools-3.1.0/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/utils/polars_ext.py` & `pdstools-3.1.0/python/pdstools/utils/polars_ext.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.1.0/python/pdstools/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.0.2/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.1.0/python/pdstools/valuefinder/ValueFinder.py`

 * *Files identical despite different names*

