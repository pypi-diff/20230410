# Comparing `tmp/censoredsummarystats-0.1.6.tar.gz` & `tmp/censoredsummarystats-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-0.1.6.tar", max compression
+gzip compressed data, was "censoredsummarystats-0.1.7.tar", max compression
```

## Comparing `censoredsummarystats-0.1.6.tar` & `censoredsummarystats-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      572 2023-03-27 09:16:02.152983 censoredsummarystats-0.1.6/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0    49439 2023-03-19 21:57:43.609414 censoredsummarystats-0.1.6/censoredsummarystats/censoredsummarystats.py
--rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-0.1.6/LICENSE
--rw-r--r--   0        0        0      534 2023-03-27 09:16:10.476106 censoredsummarystats-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-0.1.6/README.md
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 censoredsummarystats-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      572 2023-03-27 09:16:02.152983 censoredsummarystats-0.1.7/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0    52645 2023-04-09 06:25:41.657236 censoredsummarystats-0.1.7/censoredsummarystats/censoredsummarystats.py
+-rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-0.1.7/LICENSE
+-rw-r--r--   0        0        0      534 2023-04-10 04:00:09.056947 censoredsummarystats-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-0.1.7/README.md
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 censoredsummarystats-0.1.7/PKG-INFO
```

### Comparing `censoredsummarystats-0.1.6/censoredsummarystats/__init__.py` & `censoredsummarystats-0.1.7/censoredsummarystats/__init__.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.1.6/censoredsummarystats/censoredsummarystats.py` & `censoredsummarystats-0.1.7/censoredsummarystats/censoredsummarystats.py`

 * *Files 2% similar despite different names*

```diff
@@ -510,15 +510,15 @@
         will be found within each group. Multiple lists can be supplied to
         perform sequential maxima before converting intervals to a result.
         The default is [[]].
     values : list of strings, optional
         The column name(s) for the column(s) that contain the results. If a 
         single column name is given, it is assumed that the column contains
         combined censor and numeric components. If two column names are
-        provided, then the first should only contain one of five censors (<,≤,≥,>)
+        provided, then the first should only contain one of five censors (<,≤,,≥,>)
         and the second should contain only numeric data.
         The default is ['CensorComponent','NumericComponent'].
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
         e.g., <0.5 would be converted to (-np.inf,5).
         If False, then only non-negative values are considered
         e.g., <0.5 would be converted to [0,5).
@@ -664,15 +664,15 @@
         will be found within each group. Multiple lists can be supplied to
         perform sequential minima before converting intervals to a result.
         The default is [[]].
     values : list of strings, optional
         The column name(s) for the column(s) that contain the results. If a 
         single column name is given, it is assumed that the column contains
         combined censor and numeric components. If two column names are
-        provided, then the first should only contain one of five censors (<,≤,≥,>)
+        provided, then the first should only contain one of five censors (<,≤,,≥,>)
         and the second should contain only numeric data.
         The default is ['CensorComponent','NumericComponent'].
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
         e.g., <0.5 would be converted to (-np.inf,5).
         If False, then only non-negative values are considered
         e.g., <0.5 would be converted to [0,5).
@@ -806,15 +806,15 @@
         will be found within each group. Multiple lists can be supplied to
         perform sequential averaging before converting intervals to a result.
         The default is [[]].
     values : list of strings, optional
         The column name(s) for the column(s) that contain the results. If a 
         single column name is given, it is assumed that the column contains
         combined censor and numeric components. If two column names are
-        provided, then the first should only contain one of five censors (<,≤,≥,>)
+        provided, then the first should only contain one of five censors (<,≤,,≥,>)
         and the second should contain only numeric data.
         The default is ['CensorComponent','NumericComponent'].
     focus_high_potential : boolean, optional
         If True, then information on the highest potential result will be
         focused over the lowest potential result.
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
@@ -931,15 +931,16 @@
     df['Size'] = df.groupby(groupby_columns)['SiteID'].transform('size')
     
     # Set values for percentile methods
     method_dict = {'weiball':0.0, 'tukey':1/3, 'blom':3/8, 'hazen':1/2, 'excel':1.0}
     # https://en.wikipedia.org/wiki/Percentile
     C = method_dict[method]
     
-    # Ensure rank is at least 1 and no more than len(data)
+    # Calculate minimum data size for percentile method to 
+    # ensure rank is at least 1 and no more than len(data)
     minimum_size = round(C + (1-C)*max((1-percentile)/percentile,
                                        percentile/(1-percentile)),10)
     
     # Only consider groups that meet the minimum size requirement
     df = df[df['Size'] >= minimum_size]
     
     # Determine left bound and boundary for each group
@@ -1097,15 +1098,15 @@
         perform sequential median percentiles before calculating a percentile
         over the final grouping.
         The default is [[]].
     values : list of strings, optional
         The column name(s) for the column(s) that contain the results. If a 
         single column name is given, it is assumed that the column contains
         combined censor and numeric components. If two column names are
-        provided, then the first should only contain one of five censors (<,≤,≥,>)
+        provided, then the first should only contain one of five censors (<,≤,,≥,>)
         and the second should contain only numeric data.
         The default is ['CensorComponent','NumericComponent'].
     focus_high_potential : boolean, optional
         If True, then information on the highest potential result will be
         focused over the lowest potential result.
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
@@ -1166,7 +1167,74 @@
                                 precision_tolerance_to_drop_censor = precision_tolerance_to_drop_censor)
     
     # Combine the censor and numeric components into a result
     df = components_to_result(df, censor_column, numeric_column, precision_rounding)
     
     return df
 
+def median(df,
+           groupby_columns = [[]],
+           values = ['CensorComponent','NumericComponent'],
+           focus_high_potential = True,
+           include_negative_interval = False,
+           precision_tolerance_to_drop_censor = 0.25,
+           precision_rounding = True):
+    '''
+    A function that generates median results for groups within a DataFrame.
+
+    Parameters
+    ----------
+    df : DataFrame
+        DataFrame that contains censored or uncensored results
+    groupby_columns : list of lists of strings, optional
+        List of column names that should be used to create groups. A percentile
+        will be found within each group. Multiple lists can be supplied to
+        perform sequential median percentiles before calculating a percentile
+        over the final grouping.
+        The default is [[]].
+    values : list of strings, optional
+        The column name(s) for the column(s) that contain the results. If a 
+        single column name is given, it is assumed that the column contains
+        combined censor and numeric components. If two column names are
+        provided, then the first should only contain one of five censors (<,≤,,≥,>)
+        and the second should contain only numeric data.
+        The default is ['CensorComponent','NumericComponent'].
+    focus_high_potential : boolean, optional
+        If True, then information on the highest potential result will be
+        focused over the lowest potential result.
+    include_negative_interval : boolean, optional
+        If True, then all positive and negative values are considered
+        e.g., <0.5 would be converted to (-np.inf,5).
+        If False, then only non-negative values are considered
+        e.g., <0.5 would be converted to [0,5).
+        This setting only affects results if focus_high_potential is False.
+        The default is False.
+    precision_tolerance_to_drop_censor : float, optional
+        Threshold for reporting censored vs non-censored results.
+        Using the default, a result that is known to be in the interval (0.3, 0.5)
+        would be returned as 0.4, whereas a tolerance of 0 would yield a
+        result of <0.5 or >0.3 depending on the value of focus_highest_potential.
+        The default is 0.25.
+    precision_rounding : boolean, optional
+        If True, a rounding method is applied to round results to have no more
+        decimals than what can be measured.
+        The default is True.
+
+    Returns
+    -------
+    df : DataFrame
+        DataFrame that contains calculated percentiles
+
+    '''
+    
+    # Call percentile function with percentile = 50
+    df = percentile(df,
+                    50,
+                    groupby_columns = groupby_columns,
+                    values = values,
+                    focus_high_potential = focus_high_potential,
+                    include_negative_interval = include_negative_interval,
+                    precision_tolerance_to_drop_censor = precision_tolerance_to_drop_censor,
+                    precision_rounding = precision_rounding)
+    
+    return df
+
```

### Comparing `censoredsummarystats-0.1.6/LICENSE` & `censoredsummarystats-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.1.6/pyproject.toml` & `censoredsummarystats-0.1.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "0.1.6"
+version = "0.1.7"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
 packages = [{include = "censoredsummarystats"}]
 
 [tool.poetry.dependencies]
```

### Comparing `censoredsummarystats-0.1.6/PKG-INFO` & `censoredsummarystats-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

