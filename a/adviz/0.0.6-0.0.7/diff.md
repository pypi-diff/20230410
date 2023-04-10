# Comparing `tmp/adviz-0.0.6.tar.gz` & `tmp/adviz-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adviz-0.0.6.tar", last modified: Wed Apr  5 20:22:39 2023, max compression
+gzip compressed data, was "adviz-0.0.7.tar", last modified: Mon Apr 10 10:52:55 2023, max compression
```

## Comparing `adviz-0.0.6.tar` & `adviz-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-05 20:22:39.038346 adviz-0.0.6/
--rw-rw-r--   0 me         (501) staff       (20)    11337 2023-01-20 02:50:04.000000 adviz-0.0.6/LICENSE
--rw-rw-r--   0 me         (501) staff       (20)      111 2023-01-20 02:50:04.000000 adviz-0.0.6/MANIFEST.in
--rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-05 20:22:39.037348 adviz-0.0.6/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)  3584472 2023-04-03 19:59:35.000000 adviz-0.0.6/README.md
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-05 20:22:39.015843 adviz-0.0.6/adviz/
--rw-r--r--   0 me         (501) staff       (20)      111 2023-04-05 20:22:06.000000 adviz-0.0.6/adviz/__init__.py
--rw-r--r--   0 me         (501) staff       (20)      738 2023-04-05 20:22:06.000000 adviz-0.0.6/adviz/_modidx.py
--rw-r--r--   0 me         (501) staff       (20)      142 2023-03-20 19:27:57.000000 adviz-0.0.6/adviz/core.py
--rw-r--r--   0 me         (501) staff       (20)     2498 2023-04-05 20:22:06.000000 adviz-0.0.6/adviz/status_codes.py
--rw-r--r--   0 me         (501) staff       (20)     2878 2023-04-05 20:22:06.000000 adviz-0.0.6/adviz/value_counts_plus.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-05 20:22:39.026767 adviz-0.0.6/adviz.egg-info/
--rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)      353 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/SOURCES.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/dependency_links.txt
--rw-r--r--   0 me         (501) staff       (20)       32 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/entry_points.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2023-03-19 21:23:32.000000 adviz-0.0.6/adviz.egg-info/not-zip-safe
--rw-r--r--   0 me         (501) staff       (20)       50 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/requires.txt
--rw-r--r--   0 me         (501) staff       (20)        6 2023-04-05 20:22:38.000000 adviz-0.0.6/adviz.egg-info/top_level.txt
--rw-r--r--   0 me         (501) staff       (20)      832 2023-04-05 20:22:05.000000 adviz-0.0.6/settings.ini
--rw-r--r--   0 me         (501) staff       (20)       38 2023-04-05 20:22:39.038441 adviz-0.0.6/setup.cfg
--rw-rw-r--   0 me         (501) staff       (20)     2560 2023-01-20 02:50:04.000000 adviz-0.0.6/setup.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 10:52:55.067913 adviz-0.0.7/
+-rw-rw-r--   0 me         (501) staff       (20)    11337 2023-01-20 02:50:04.000000 adviz-0.0.7/LICENSE
+-rw-rw-r--   0 me         (501) staff       (20)      111 2023-01-20 02:50:04.000000 adviz-0.0.7/MANIFEST.in
+-rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 10:52:55.066937 adviz-0.0.7/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)  3584472 2023-04-03 19:59:35.000000 adviz-0.0.7/README.md
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 10:52:55.047334 adviz-0.0.7/adviz/
+-rw-r--r--   0 me         (501) staff       (20)      111 2023-04-10 10:51:03.000000 adviz-0.0.7/adviz/__init__.py
+-rw-r--r--   0 me         (501) staff       (20)      738 2023-04-10 10:51:03.000000 adviz-0.0.7/adviz/_modidx.py
+-rw-r--r--   0 me         (501) staff       (20)      142 2023-03-20 19:27:57.000000 adviz-0.0.7/adviz/core.py
+-rw-r--r--   0 me         (501) staff       (20)     2498 2023-04-10 10:51:03.000000 adviz-0.0.7/adviz/status_codes.py
+-rw-r--r--   0 me         (501) staff       (20)     3908 2023-04-10 10:51:03.000000 adviz-0.0.7/adviz/value_counts_plus.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 10:52:55.055494 adviz-0.0.7/adviz.egg-info/
+-rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)      353 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/SOURCES.txt
+-rw-r--r--   0 me         (501) staff       (20)        1 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/dependency_links.txt
+-rw-r--r--   0 me         (501) staff       (20)       32 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/entry_points.txt
+-rw-r--r--   0 me         (501) staff       (20)        1 2023-03-19 21:23:32.000000 adviz-0.0.7/adviz.egg-info/not-zip-safe
+-rw-r--r--   0 me         (501) staff       (20)       50 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/requires.txt
+-rw-r--r--   0 me         (501) staff       (20)        6 2023-04-10 10:52:54.000000 adviz-0.0.7/adviz.egg-info/top_level.txt
+-rw-r--r--   0 me         (501) staff       (20)      832 2023-04-10 10:51:03.000000 adviz-0.0.7/settings.ini
+-rw-r--r--   0 me         (501) staff       (20)       38 2023-04-10 10:52:55.068045 adviz-0.0.7/setup.cfg
+-rw-rw-r--   0 me         (501) staff       (20)     2560 2023-01-20 02:50:04.000000 adviz-0.0.7/setup.py
```

### Comparing `adviz-0.0.6/LICENSE` & `adviz-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adviz-0.0.6/PKG-INFO` & `adviz-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adviz
-Version: 0.0.6
+Version: 0.0.7
 Summary: advertools visualizations
 Home-page: https://github.com/eliasdabbas/adviz
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adviz-0.0.6/README.md` & `adviz-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `adviz-0.0.6/adviz/_modidx.py` & `adviz-0.0.7/adviz/_modidx.py`

 * *Files identical despite different names*

### Comparing `adviz-0.0.6/adviz/status_codes.py` & `adviz-0.0.7/adviz/status_codes.py`

 * *Files identical despite different names*

### Comparing `adviz-0.0.6/adviz/value_counts_plus.py` & `adviz-0.0.7/adviz/value_counts_plus.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 # %% ../nbs/00_value_counts_plus.ipynb 4
 def value_counts_plus(
     series,
     dropna=False,
     show_top=10,
     sort_others=False,
     style=True,
+    size=10,
+    thousands=',',
+    decimal='.',
     name='data',
     background_gradient='cividis'):
     """
     Provide a few ways of showing counts of values of items in ``series``.
 
     Parameters
     ----------
@@ -29,47 +32,71 @@
     sort_others : bool
         Whether or not to place "Others" in the bottom (default) or in its
         sorted order position.
     style : bool
         Whether or not to style values for easier reading. If set to ``True``
         the result would not be a DataFrame, and cannot be further manipulated.
         Set the value to ``False`` to get aDataFrame as the return value.
+    size : int
+        The size in points of the font of the table. This results in the whole
+        table being resized.
+    thousands : str
+        The character to use to separate thousands if `style=True`. Defaults to
+        `,` but you can change to `.` or space, or any oher character you want.
+    decimal : str
+        The character to use to display decimal number if `style=True`. Defaults to
+        `.` but you can change to `,`or any oher character you want.
+
     name : str
         The name of the column that you want displayed in the final table. It
         appears in the caption and defaults to "data".
     background_gradient: str
         The name of the color map to be used as the gradient. Many color maps
         are available: cividis, viridis, copper, cool, magma, and more. You can
         reverse the color by appending _r to the end of the colormap name
         cividis_r for example. Enter a random string to get an error message
         with all available colormaps.
 
     Returns
     -------
-    value_counts_df : a pandas.DataFrame showing counts based on the provided arguments
+    value_counts_df : pandas.DataFrame
+        A DataFrame showing counts based on the provided arguments
     """
-    val_counts = pd.Series(series).value_counts(dropna=dropna).rename(name)
+    final_col_names = ['count', 'cum_count', 'perc', 'cum_perc']
+    if name in final_col_names:
+        raise ValueError(f"Please make sure you use a name other than {final_col_names}")
+    val_counts = pd.Series(series).rename(name).value_counts(dropna=dropna).reset_index()
     if len(val_counts) > show_top:
+        others_df = pd.DataFrame({
+            name: ['Others:'],
+            'count': val_counts[show_top:]['count'].sum()
+            }, index=[show_top])
         val_counts = pd.concat([
-            val_counts.iloc[:show_top],
-            pd.Series(val_counts.iloc[show_top:].sum(), index=['Others:'])]).rename(name)
+            val_counts[:show_top],
+            others_df
+        ])
         if sort_others:
-            val_counts = val_counts.sort_values(ascending=False)
-        show_top += 1
+            val_counts = val_counts.sort_values(by=['count'], ascending=False)
+
     count_df = (val_counts
-                .reset_index()
-                .assign(cum_count=lambda df: df[name].cumsum(),
-                        perc=lambda df: df[name].div(df[name].sum()),
-                        cum_perc=lambda df: df['perc'].cumsum())
-                .rename(columns={'index': name, name: 'count'}))
+                .assign(
+                    cum_count=lambda df: df['count'].cumsum(),
+                    perc=lambda df: df['count'].div(df['count'].sum()),
+                    cum_perc=lambda df: df['perc'].cumsum())
+                )
     if not style:
-        return count_df.head(show_top)
-    return (count_df.
-            head(show_top).style
+        return count_df
+    return (count_df
+            .style
             .format({'count': '{:,}', 'cumsum': '{:,}', 
                      'perc': '{:.1%}',
                      'cum_count': '{:,}',
-                     'cum_perc': '{:.1%}'})
+                     'cum_perc': '{:.1%}'},
+                    thousands=thousands,
+                    decimal=decimal)
             .background_gradient(background_gradient)
+            .relabel_index(range(1, len(count_df)+1), axis=0)
+            .relabel_index([name, 'count', 'cum. count', '%', 'cum. %'], axis=1)
             .highlight_null()
-            .set_caption(f'<h2>Counts of <b>{name}</b></h2>'))
+            .set_caption(f'<h2>Counts of <b>{name}</b></h2>')
+            .set_table_attributes(f'style=font-size:{size}pt;'))
```

### Comparing `adviz-0.0.6/adviz.egg-info/PKG-INFO` & `adviz-0.0.7/adviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adviz
-Version: 0.0.6
+Version: 0.0.7
 Summary: advertools visualizations
 Home-page: https://github.com/eliasdabbas/adviz
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adviz-0.0.6/settings.ini` & `adviz-0.0.7/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = adviz
 lib_name = adviz
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = adviz
 nbs_path = nbs
 recursive = True
```

### Comparing `adviz-0.0.6/setup.py` & `adviz-0.0.7/setup.py`

 * *Files identical despite different names*

