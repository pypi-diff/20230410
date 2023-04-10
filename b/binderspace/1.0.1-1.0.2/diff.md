# Comparing `tmp/binderspace-1.0.1.tar.gz` & `tmp/binderspace-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binderspace-1.0.1.tar", last modified: Wed Apr  5 19:11:47 2023, max compression
+gzip compressed data, was "binderspace-1.0.2.tar", last modified: Mon Apr 10 18:47:12 2023, max compression
```

## Comparing `binderspace-1.0.1.tar` & `binderspace-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 payam     (1000) payam     (1000)        0 2023-04-05 19:11:47.675478 binderspace-1.0.1/
--rw-rw-r--   0 payam     (1000) payam     (1000)      712 2023-04-05 19:11:47.675478 binderspace-1.0.1/PKG-INFO
-drwxrwxr-x   0 payam     (1000) payam     (1000)        0 2023-04-05 19:11:47.675478 binderspace-1.0.1/binderspace/
--rw-rw-r--   0 payam     (1000) payam     (1000)        0 2023-04-05 19:06:25.489137 binderspace-1.0.1/binderspace/__init__.py
--rw-rw-r--   0 payam     (1000) payam     (1000)     4396 2023-04-05 19:06:25.489137 binderspace-1.0.1/binderspace/binder_space.py
--rw-rw-r--   0 payam     (1000) payam     (1000)    20662 2023-04-05 19:06:25.489137 binderspace-1.0.1/binderspace/module.py
--rw-rw-r--   0 payam     (1000) payam     (1000)    10822 2023-04-05 19:06:25.489137 binderspace-1.0.1/binderspace/motif_search.py
--rw-rw-r--   0 payam     (1000) payam     (1000)       40 2023-04-05 19:06:25.513137 binderspace-1.0.1/setup.cfg
--rw-rw-r--   0 payam     (1000) payam     (1000)     1047 2023-04-05 19:11:38.499410 binderspace-1.0.1/setup.py
+drwxrwxr-x   0 payam     (1000) payam     (1000)        0 2023-04-10 18:47:12.492374 binderspace-1.0.2/
+-rw-rw-r--   0 payam     (1000) payam     (1000)      712 2023-04-10 18:47:12.492374 binderspace-1.0.2/PKG-INFO
+drwxrwxr-x   0 payam     (1000) payam     (1000)        0 2023-04-10 18:47:12.492374 binderspace-1.0.2/binderspace/
+-rw-rw-r--   0 payam     (1000) payam     (1000)        0 2023-04-10 18:33:13.000000 binderspace-1.0.2/binderspace/__init__.py
+-rw-rw-r--   0 payam     (1000) payam     (1000)     4396 2023-04-10 18:33:13.000000 binderspace-1.0.2/binderspace/binder_space.py
+-rw-rw-r--   0 payam     (1000) payam     (1000)    20662 2023-04-10 18:33:13.000000 binderspace-1.0.2/binderspace/module.py
+-rw-rw-r--   0 payam     (1000) payam     (1000)    11260 2023-04-10 18:33:13.000000 binderspace-1.0.2/binderspace/motif_search.py
+-rw-rw-r--   0 payam     (1000) payam     (1000)       40 2023-04-10 18:33:13.000000 binderspace-1.0.2/setup.cfg
+-rw-rw-r--   0 payam     (1000) payam     (1000)     1047 2023-04-10 18:44:08.866890 binderspace-1.0.2/setup.py
```

### Comparing `binderspace-1.0.1/PKG-INFO` & `binderspace-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: binderspace
-Version: 1.0.1
+Version: 1.0.2
 Summary: a library for finding the space for binding sequences
 Home-page: https://github.com/vukoviclab/BinderSpace
 Author: Vukovic Lab (Payam Kelich)
 Author-email: lvukovic@utep.edu
 License: mit
 Download-URL: https://github.com/vukoviclab/BinderSpace/archive/refs/tags/1.0.tar.gz
 Description: UNKNOWN
```

### Comparing `binderspace-1.0.1/binderspace/binder_space.py` & `binderspace-1.0.2/binderspace/binder_space.py`

 * *Files identical despite different names*

### Comparing `binderspace-1.0.1/binderspace/module.py` & `binderspace-1.0.2/binderspace/module.py`

 * *Files identical despite different names*

### Comparing `binderspace-1.0.1/binderspace/motif_search.py` & `binderspace-1.0.2/binderspace/motif_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -175,25 +175,31 @@
     data = []
     if negfile == -1:
         for i in re_dict.keys():
             pos_perc = (len(re_dict[i]) / len(posset)) * 100
             data.append([i, len(re_dict[i]), pos_perc, re_dict[i]])
             df = pd.DataFrame(data, columns=['motifs', 'positive_occurrence', 'pos_percentage (%)', 'index'])
             df2 = df.sort_values('pos_percentage', ascending=False)
+            df2.drop(['index'], axis=1, inplace=True)
 
     else:
         for i in re_dict.keys():
             pos_perc = (len(re_dict[i][0]) / len(posset)) * 100
             neg_perc = (len(re_dict[i][1]) / len(negset)) * 100
+            data_chi = np.array([[len(re_dict[i][0]),len(re_dict[i][1])],
+                                 [len(posset)-len(re_dict[i][0]),len(negset)-len(re_dict[i][1])]])
+            chi2, p_value, degrees_of_freedom, expected_values = chi2_contingency(data_chi)
+            
             if pos_perc > neg_perc:
                 data.append(
-                    [i, len(re_dict[i][0]), len(re_dict[i][1]), pos_perc, neg_perc, pos_perc - neg_perc, re_dict[i][0], re_dict[i][1]])
+                    [i, len(re_dict[i][0]), len(re_dict[i][1]), pos_perc, neg_perc, pos_perc - neg_perc, re_dict[i][0], re_dict[i][1],round(chi2, 2),p_value])
         df = pd.DataFrame(data, columns=['motifs', 'positive_occurrence', 'negative_occurrence ', 'pos_percentage (%)',
-                                         'neg_percentage (%)', 'difference (%)', 'index_pos', 'index_neg'])
+                                         'neg_percentage (%)', 'difference (%)', 'index_pos', 'index_neg','chi2','p-value'])
         df2 = df.sort_values('difference (%)', ascending=False)
+        df2.drop(['index_pos','index_neg'], axis=1, inplace=True)
 
     return df2
 
 
 def print_csv(dataframe):
     print("printing the motifs into different csv files regarding to their length")
     for i in range(min_length, max_length + 1):
```

### Comparing `binderspace-1.0.1/setup.py` & `binderspace-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='binderspace',
     packages=['binderspace'],
-    version='1.0.1',
+    version='1.0.2',
     license='mit',
     description='a library for finding the space for binding sequences',
     author='Vukovic Lab (Payam Kelich)',
     author_email='lvukovic@utep.edu',  # Type in your E-Mail
     url='https://github.com/vukoviclab/BinderSpace',  # Provide either the link to your github or to your website
     download_url='https://github.com/vukoviclab/BinderSpace/archive/refs/tags/1.0.tar.gz',
     keywords=['DNA', 'sequence', 'pca', 't-sne', 'peptide'],  # Keywords that define your package best
```

