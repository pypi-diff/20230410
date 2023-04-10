# Comparing `tmp/explai-0.4.tar.gz` & `tmp/explai-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explai-0.4.tar", last modified: Mon Apr 10 06:54:02 2023, max compression
+gzip compressed data, was "explai-0.5.tar", last modified: Mon Apr 10 07:29:19 2023, max compression
```

## Comparing `explai-0.4.tar` & `explai-0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 06:54:02.804678 explai-0.4/
--rw-rw-rw-   0        0        0      790 2023-04-10 06:54:02.805676 explai-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 06:54:02.804678 explai-0.4/explai/
--rw-rw-rw-   0        0        0       60 2023-04-10 06:48:30.939730 explai-0.4/explai/__init__.py
--rw-rw-rw-   0        0        0     9230 2023-04-10 06:49:55.916146 explai-0.4/explai/reports.py
--rw-rw-rw-   0        0        0       63 2023-04-09 06:19:21.827327 explai-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1713 2023-04-10 06:52:35.503804 explai-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:29:19.188089 explai-0.5/
+-rw-rw-rw-   0        0        0      790 2023-04-10 07:29:19.188089 explai-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 07:29:19.188089 explai-0.5/explai/
+-rw-rw-rw-   0        0        0       60 2023-04-10 06:48:30.939730 explai-0.5/explai/__init__.py
+-rw-rw-rw-   0        0        0     9229 2023-04-10 07:25:45.539083 explai-0.5/explai/reports.py
+-rw-rw-rw-   0        0        0       63 2023-04-09 06:19:21.827327 explai-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1713 2023-04-10 07:27:01.805807 explai-0.5/setup.py
```

### Comparing `explai-0.4/PKG-INFO` & `explai-0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: explai
-Version: 0.4
+Version: 0.5
 Summary: A reporting tool for explainable AI
 Home-page: https://github.com/ritwikbd/explai
 Author: Ritwik Bandyopadhyay
 Author-email: ritwikbanrg@gmail.com
 License: MIT
-Download-URL: https://github.com/ritwikbd/explai/archive/refs/tags/v04.tar.gz
+Download-URL: https://github.com/ritwikbd/explai/archive/refs/tags/v05.tar.gz
 Description: UNKNOWN
 Keywords: Explainable AI,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `explai-0.4/explai/reports.py` & `explai-0.5/explai/reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from reportlab.lib.units import inch, cm
 from reportlab.lib.utils import ImageReader
 
 import matplotlib
 import seaborn as sns
 
 import pandas as pd
-matplotlib.pyplot.ticklabel_format(style='plain', axis='y')
+#matplotlib.pyplot.ticklabel_format(style='plain', axis='y')
 
 
 def getPcaPlot(df_x,yval,title,image_name):
     
     from sklearn.decomposition import PCA
     pca = PCA(n_components=2)
 
@@ -81,15 +81,15 @@
     df_features=pd.concat([df_featimp2.iloc[0:4,],dfother])
     return df_features
 
 
 def getFeatImps(model,df_x,df_feats):
     
     t3=sns.barplot(y=df_feats['importance'],x=df_feats['feature'])
-    t3.set_xticklabels(df_feats['feature'],rotation='14')
+    t3.set_xticklabels(df_feats['feature'],rotation=14)
     img3=t3.get_figure()
     img3.savefig("featsBar.png",bbox_inches='tight')
     t3.remove()
     matplotlib.pyplot.close()
```

### Comparing `explai-0.4/setup.py` & `explai-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'explai',         # How you named your package folder (MyLib)
   packages = ['explai'],   # Chose the same as "name"
-  version = '0.4',      # Start with a small number and increase it with every change you make
+  version = '0.5',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A reporting tool for explainable AI',   # Give a short description about your library
   author = 'Ritwik Bandyopadhyay',                   # Type in your name
   author_email = 'ritwikbanrg@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ritwikbd/explai',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ritwikbd/explai/archive/refs/tags/v04.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ritwikbd/explai/archive/refs/tags/v05.tar.gz',    # I explain this later on
   keywords = ['Explainable AI', 'Machine Learning'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'reportlab','scikit-learn','matplotlib','seaborn','pandas'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

