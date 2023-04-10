# Comparing `tmp/adviz-0.0.5.tar.gz` & `tmp/adviz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adviz-0.0.5.tar", last modified: Wed Apr  5 14:36:58 2023, max compression
+gzip compressed data, was "adviz-0.0.6.tar", last modified: Wed Apr  5 20:22:39 2023, max compression
```

## Comparing `adviz-0.0.5.tar` & `adviz-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-05 14:36:58.580702 adviz-0.0.5/
--rw-rw-r--   0 me         (501) staff       (20)    11337 2023-01-20 02:50:04.000000 adviz-0.0.5/LICENSE
--rw-rw-r--   0 me         (501) staff       (20)      111 2023-01-20 02:50:04.000000 adviz-0.0.5/MANIFEST.in
--rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-05 14:36:58.579140 adviz-0.0.5/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)  3584472 2023-04-03 19:59:35.000000 adviz-0.0.5/README.md
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-05 14:36:58.561846 adviz-0.0.5/adviz/
--rw-r--r--   0 me         (501) staff       (20)      111 2023-04-05 14:36:52.000000 adviz-0.0.5/adviz/__init__.py
--rw-r--r--   0 me         (501) staff       (20)      738 2023-04-05 14:36:52.000000 adviz-0.0.5/adviz/_modidx.py
--rw-r--r--   0 me         (501) staff       (20)      142 2023-03-20 19:27:57.000000 adviz-0.0.5/adviz/core.py
--rw-r--r--   0 me         (501) staff       (20)     2498 2023-04-05 14:36:52.000000 adviz-0.0.5/adviz/status_codes.py
--rw-r--r--   0 me         (501) staff       (20)     2923 2023-04-05 14:36:52.000000 adviz-0.0.5/adviz/value_counts_plus.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-05 14:36:58.570923 adviz-0.0.5/adviz.egg-info/
--rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-05 14:36:58.000000 adviz-0.0.5/adviz.egg-info/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)      353 2023-04-05 14:36:58.000000 adviz-0.0.5/adviz.egg-info/SOURCES.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2023-04-05 14:36:58.000000 adviz-0.0.5/adviz.egg-info/dependency_links.txt
--rw-r--r--   0 me         (501) staff       (20)       32 2023-04-05 14:36:58.000000 adviz-0.0.5/adviz.egg-info/entry_points.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2023-03-19 21:23:32.000000 adviz-0.0.5/adviz.egg-info/not-zip-safe
--rw-r--r--   0 me         (501) staff       (20)       50 2023-04-05 14:36:58.000000 adviz-0.0.5/adviz.egg-info/requires.txt
--rw-r--r--   0 me         (501) staff       (20)        6 2023-04-05 14:36:58.000000 adviz-0.0.5/adviz.egg-info/top_level.txt
--rw-r--r--   0 me         (501) staff       (20)      832 2023-04-05 14:36:52.000000 adviz-0.0.5/settings.ini
--rw-r--r--   0 me         (501) staff       (20)       38 2023-04-05 14:36:58.580821 adviz-0.0.5/setup.cfg
--rw-rw-r--   0 me         (501) staff       (20)     2560 2023-01-20 02:50:04.000000 adviz-0.0.5/setup.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-05 20:22:39.038346 adviz-0.0.6/
+-rw-rw-r--   0 me         (501) staff       (20)    11337 2023-01-20 02:50:04.000000 adviz-0.0.6/LICENSE
+-rw-rw-r--   0 me         (501) staff       (20)      111 2023-01-20 02:50:04.000000 adviz-0.0.6/MANIFEST.in
+-rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-05 20:22:39.037348 adviz-0.0.6/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)  3584472 2023-04-03 19:59:35.000000 adviz-0.0.6/README.md
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-05 20:22:39.015843 adviz-0.0.6/adviz/
+-rw-r--r--   0 me         (501) staff       (20)      111 2023-04-05 20:22:06.000000 adviz-0.0.6/adviz/__init__.py
+-rw-r--r--   0 me         (501) staff       (20)      738 2023-04-05 20:22:06.000000 adviz-0.0.6/adviz/_modidx.py
+-rw-r--r--   0 me         (501) staff       (20)      142 2023-03-20 19:27:57.000000 adviz-0.0.6/adviz/core.py
+-rw-r--r--   0 me         (501) staff       (20)     2498 2023-04-05 20:22:06.000000 adviz-0.0.6/adviz/status_codes.py
+-rw-r--r--   0 me         (501) staff       (20)     2878 2023-04-05 20:22:06.000000 adviz-0.0.6/adviz/value_counts_plus.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-05 20:22:39.026767 adviz-0.0.6/adviz.egg-info/
+-rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)      353 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/SOURCES.txt
+-rw-r--r--   0 me         (501) staff       (20)        1 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/dependency_links.txt
+-rw-r--r--   0 me         (501) staff       (20)       32 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/entry_points.txt
+-rw-r--r--   0 me         (501) staff       (20)        1 2023-03-19 21:23:32.000000 adviz-0.0.6/adviz.egg-info/not-zip-safe
+-rw-r--r--   0 me         (501) staff       (20)       50 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/requires.txt
+-rw-r--r--   0 me         (501) staff       (20)        6 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/top_level.txt
+-rw-r--r--   0 me         (501) staff       (20)      832 2023-04-05 20:22:05.000000 adviz-0.0.6/settings.ini
+-rw-r--r--   0 me         (501) staff       (20)       38 2023-04-05 20:22:39.038441 adviz-0.0.6/setup.cfg
+-rw-rw-r--   0 me         (501) staff       (20)     2560 2023-01-20 02:50:04.000000 adviz-0.0.6/setup.py
```

### Comparing `adviz-0.0.5/LICENSE` & `adviz-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adviz-0.0.5/PKG-INFO` & `adviz-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adviz
-Version: 0.0.5
+Version: 0.0.6
 Summary: advertools visualizations
 Home-page: https://github.com/eliasdabbas/adviz
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adviz-0.0.5/README.md` & `adviz-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `adviz-0.0.5/adviz/_modidx.py` & `adviz-0.0.6/adviz/_modidx.py`

 * *Files identical despite different names*

### Comparing `adviz-0.0.5/adviz/status_codes.py` & `adviz-0.0.6/adviz/status_codes.py`

 * *Files identical despite different names*

### Comparing `adviz-0.0.5/adviz/value_counts_plus.py` & `adviz-0.0.6/adviz/value_counts_plus.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,35 +43,33 @@
         cividis_r for example. Enter a random string to get an error message
         with all available colormaps.
 
     Returns
     -------
     value_counts_df : a pandas.DataFrame showing counts based on the provided arguments
     """
-    series = pd.Series(series).rename(name)
-    val_counts = series.value_counts(dropna=dropna)
+    val_counts = pd.Series(series).value_counts(dropna=dropna).rename(name)
     if len(val_counts) > show_top:
         val_counts = pd.concat([
-            val_counts[:show_top],
-            pd.Series(val_counts[show_top:].sum(), index=['Others:'])]).rename(name)
+            val_counts.iloc[:show_top],
+            pd.Series(val_counts.iloc[show_top:].sum(), index=['Others:'])]).rename(name)
         if sort_others:
             val_counts = val_counts.sort_values(ascending=False)
         show_top += 1
     count_df = (val_counts
-                .to_frame()
+                .reset_index()
                 .assign(cum_count=lambda df: df[name].cumsum(),
                         perc=lambda df: df[name].div(df[name].sum()),
                         cum_perc=lambda df: df['perc'].cumsum())
-                .reset_index()
                 .rename(columns={'index': name, name: 'count'}))
     if not style:
         return count_df.head(show_top)
     return (count_df.
             head(show_top).style
             .format({'count': '{:,}', 'cumsum': '{:,}', 
                      'perc': '{:.1%}',
                      'cum_count': '{:,}',
                      'cum_perc': '{:.1%}'})
             .background_gradient(background_gradient)
             .highlight_null()
-            .set_caption(f'<h2>Counts of <b>{series.name}</b></h2>'))
+            .set_caption(f'<h2>Counts of <b>{name}</b></h2>'))
```

### Comparing `adviz-0.0.5/adviz.egg-info/PKG-INFO` & `adviz-0.0.6/adviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adviz
-Version: 0.0.5
+Version: 0.0.6
 Summary: advertools visualizations
 Home-page: https://github.com/eliasdabbas/adviz
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adviz-0.0.5/settings.ini` & `adviz-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = adviz
 lib_name = adviz
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = adviz
 nbs_path = nbs
 recursive = True
```

### Comparing `adviz-0.0.5/setup.py` & `adviz-0.0.6/setup.py`

 * *Files identical despite different names*

