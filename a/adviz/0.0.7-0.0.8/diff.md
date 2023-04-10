# Comparing `tmp/adviz-0.0.7.tar.gz` & `tmp/adviz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adviz-0.0.7.tar", last modified: Mon Apr 10 10:52:55 2023, max compression
+gzip compressed data, was "adviz-0.0.8.tar", last modified: Mon Apr 10 19:21:08 2023, max compression
```

## Comparing `adviz-0.0.7.tar` & `adviz-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 10:52:55.067913 adviz-0.0.7/
--rw-rw-r--   0 me         (501) staff       (20)    11337 2023-01-20 02:50:04.000000 adviz-0.0.7/LICENSE
--rw-rw-r--   0 me         (501) staff       (20)      111 2023-01-20 02:50:04.000000 adviz-0.0.7/MANIFEST.in
--rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 10:52:55.066937 adviz-0.0.7/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)  3584472 2023-04-03 19:59:35.000000 adviz-0.0.7/README.md
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 10:52:55.047334 adviz-0.0.7/adviz/
--rw-r--r--   0 me         (501) staff       (20)      111 2023-04-10 10:51:03.000000 adviz-0.0.7/adviz/__init__.py
--rw-r--r--   0 me         (501) staff       (20)      738 2023-04-10 10:51:03.000000 adviz-0.0.7/adviz/_modidx.py
--rw-r--r--   0 me         (501) staff       (20)      142 2023-03-20 19:27:57.000000 adviz-0.0.7/adviz/core.py
--rw-r--r--   0 me         (501) staff       (20)     2498 2023-04-10 10:51:03.000000 adviz-0.0.7/adviz/status_codes.py
--rw-r--r--   0 me         (501) staff       (20)     3908 2023-04-10 10:51:03.000000 adviz-0.0.7/adviz/value_counts_plus.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 10:52:55.055494 adviz-0.0.7/adviz.egg-info/
--rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)      353 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/SOURCES.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/dependency_links.txt
--rw-r--r--   0 me         (501) staff       (20)       32 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/entry_points.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2023-03-19 21:23:32.000000 adviz-0.0.7/adviz.egg-info/not-zip-safe
--rw-r--r--   0 me         (501) staff       (20)       50 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/requires.txt
--rw-r--r--   0 me         (501) staff       (20)        6 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/top_level.txt
--rw-r--r--   0 me         (501) staff       (20)      832 2023-04-10 10:51:03.000000 adviz-0.0.7/settings.ini
--rw-r--r--   0 me         (501) staff       (20)       38 2023-04-10 10:52:55.068045 adviz-0.0.7/setup.cfg
--rw-rw-r--   0 me         (501) staff       (20)     2560 2023-01-20 02:50:04.000000 adviz-0.0.7/setup.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 19:21:08.534019 adviz-0.0.8/
+-rw-rw-r--   0 me         (501) staff       (20)    11337 2023-01-20 02:50:04.000000 adviz-0.0.8/LICENSE
+-rw-rw-r--   0 me         (501) staff       (20)      111 2023-01-20 02:50:04.000000 adviz-0.0.8/MANIFEST.in
+-rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 19:21:08.533073 adviz-0.0.8/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)  3584472 2023-04-03 19:59:35.000000 adviz-0.0.8/README.md
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 19:21:08.515397 adviz-0.0.8/adviz/
+-rw-r--r--   0 me         (501) staff       (20)      111 2023-04-10 19:17:02.000000 adviz-0.0.8/adviz/__init__.py
+-rw-r--r--   0 me         (501) staff       (20)      738 2023-04-10 19:17:02.000000 adviz-0.0.8/adviz/_modidx.py
+-rw-r--r--   0 me         (501) staff       (20)      142 2023-03-20 19:27:57.000000 adviz-0.0.8/adviz/core.py
+-rw-r--r--   0 me         (501) staff       (20)     2478 2023-04-10 19:17:02.000000 adviz-0.0.8/adviz/status_codes.py
+-rw-r--r--   0 me         (501) staff       (20)     3921 2023-04-10 19:17:02.000000 adviz-0.0.8/adviz/value_counts_plus.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 19:21:08.521638 adviz-0.0.8/adviz.egg-info/
+-rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)      353 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/SOURCES.txt
+-rw-r--r--   0 me         (501) staff       (20)        1 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/dependency_links.txt
+-rw-r--r--   0 me         (501) staff       (20)       32 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/entry_points.txt
+-rw-r--r--   0 me         (501) staff       (20)        1 2023-03-19 21:23:32.000000 adviz-0.0.8/adviz.egg-info/not-zip-safe
+-rw-r--r--   0 me         (501) staff       (20)       50 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/requires.txt
+-rw-r--r--   0 me         (501) staff       (20)        6 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/top_level.txt
+-rw-r--r--   0 me         (501) staff       (20)      832 2023-04-10 19:17:02.000000 adviz-0.0.8/settings.ini
+-rw-r--r--   0 me         (501) staff       (20)       38 2023-04-10 19:21:08.534142 adviz-0.0.8/setup.cfg
+-rw-rw-r--   0 me         (501) staff       (20)     2560 2023-01-20 02:50:04.000000 adviz-0.0.8/setup.py
```

### Comparing `adviz-0.0.7/LICENSE` & `adviz-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adviz-0.0.7/PKG-INFO` & `adviz-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adviz
-Version: 0.0.7
+Version: 0.0.8
 Summary: advertools visualizations
 Home-page: https://github.com/eliasdabbas/adviz
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adviz-0.0.7/README.md` & `adviz-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `adviz-0.0.7/adviz/_modidx.py` & `adviz-0.0.8/adviz/_modidx.py`

 * *Files identical despite different names*

### Comparing `adviz-0.0.7/adviz/status_codes.py` & `adviz-0.0.8/adviz/status_codes.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,20 +41,17 @@
     export_to_html: str, optional
         The path to the HTML file if you want to save it as a shareable file
 
     Returns
     -------
     status_codes_figure : plotly.graph_objects.Figure
     """
-    status_counts = (
-        pd.Series(status_list)
-        .value_counts()
-        .rename_axis('index')
-        .reset_index()
-        .rename(columns={'index': 'status'})
+    status_counts = pd.Series(status_list).value_counts().reset_index()
+    status_counts.columns = ['status', 'count']
+    status_counts = (status_counts
         .assign(status_cat=lambda df: df['status'].astype(int).round(-2))
         .assign(status_desc=lambda df: [responses[int(code)] for code in df['status']])
     )
     status_fig = px.treemap(
         status_counts,
         maxdepth = 2,
         path=[px.Constant('Status codes'), 'status_cat', 'status'],
```

### Comparing `adviz-0.0.7/adviz/value_counts_plus.py` & `adviz-0.0.8/adviz/value_counts_plus.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     value_counts_df : pandas.DataFrame
         A DataFrame showing counts based on the provided arguments
     """
     final_col_names = ['count', 'cum_count', 'perc', 'cum_perc']
     if name in final_col_names:
         raise ValueError(f"Please make sure you use a name other than {final_col_names}")
     val_counts = pd.Series(series).rename(name).value_counts(dropna=dropna).reset_index()
+    val_counts.columns = [name, 'count']
     if len(val_counts) > show_top:
         others_df = pd.DataFrame({
             name: ['Others:'],
             'count': val_counts[show_top:]['count'].sum()
             }, index=[show_top])
         val_counts = pd.concat([
             val_counts[:show_top],
@@ -81,22 +82,22 @@
                 .assign(
                     cum_count=lambda df: df['count'].cumsum(),
                     perc=lambda df: df['count'].div(df['count'].sum()),
                     cum_perc=lambda df: df['perc'].cumsum())
                 )
     if not style:
         return count_df
+    count_df.index = range(1, len(count_df)+1)
+    count_df.columns = [name, 'count', 'cum. count', '%', 'cum. %']
     return (count_df
             .style
             .format({'count': '{:,}', 'cumsum': '{:,}', 
                      'perc': '{:.1%}',
                      'cum_count': '{:,}',
                      'cum_perc': '{:.1%}'},
                     thousands=thousands,
                     decimal=decimal)
             .background_gradient(background_gradient)
-            .relabel_index(range(1, len(count_df)+1), axis=0)
-            .relabel_index([name, 'count', 'cum. count', '%', 'cum. %'], axis=1)
             .highlight_null()
             .set_caption(f'<h2>Counts of <b>{name}</b></h2>')
             .set_table_attributes(f'style=font-size:{size}pt;'))
```

### Comparing `adviz-0.0.7/adviz.egg-info/PKG-INFO` & `adviz-0.0.8/adviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adviz
-Version: 0.0.7
+Version: 0.0.8
 Summary: advertools visualizations
 Home-page: https://github.com/eliasdabbas/adviz
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adviz-0.0.7/settings.ini` & `adviz-0.0.8/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = adviz
 lib_name = adviz
-version = 0.0.7
+version = 0.0.8
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = adviz
 nbs_path = nbs
 recursive = True
```

### Comparing `adviz-0.0.7/setup.py` & `adviz-0.0.8/setup.py`

 * *Files identical despite different names*

