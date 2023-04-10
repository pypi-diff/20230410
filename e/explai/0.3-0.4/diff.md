# Comparing `tmp/explai-0.3.tar.gz` & `tmp/explai-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explai-0.3.tar", last modified: Sun Apr  9 06:55:02 2023, max compression
+gzip compressed data, was "explai-0.4.tar", last modified: Mon Apr 10 06:54:02 2023, max compression
```

## Comparing `explai-0.3.tar` & `explai-0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:55:02.363129 explai-0.3/
--rw-rw-rw-   0        0        0      790 2023-04-09 06:55:02.363129 explai-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 06:55:02.362138 explai-0.3/explai/
--rw-rw-rw-   0        0        0       52 2023-04-09 06:28:24.804686 explai-0.3/explai/__init__.py
--rw-rw-rw-   0        0        0     9204 2023-04-09 06:01:58.571164 explai-0.3/explai/explai.py
--rw-rw-rw-   0        0        0       63 2023-04-09 06:19:21.827327 explai-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1713 2023-04-09 06:54:48.904231 explai-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:54:02.804678 explai-0.4/
+-rw-rw-rw-   0        0        0      790 2023-04-10 06:54:02.805676 explai-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 06:54:02.804678 explai-0.4/explai/
+-rw-rw-rw-   0        0        0       60 2023-04-10 06:48:30.939730 explai-0.4/explai/__init__.py
+-rw-rw-rw-   0        0        0     9230 2023-04-10 06:49:55.916146 explai-0.4/explai/reports.py
+-rw-rw-rw-   0        0        0       63 2023-04-09 06:19:21.827327 explai-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1713 2023-04-10 06:52:35.503804 explai-0.4/setup.py
```

### Comparing `explai-0.3/PKG-INFO` & `explai-0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: explai
-Version: 0.3
+Version: 0.4
 Summary: A reporting tool for explainable AI
 Home-page: https://github.com/ritwikbd/explai
 Author: Ritwik Bandyopadhyay
 Author-email: ritwikbanrg@gmail.com
 License: MIT
-Download-URL: https://github.com/ritwikbd/explai/archive/refs/tags/v03.tar.gz
+Download-URL: https://github.com/ritwikbd/explai/archive/refs/tags/v04.tar.gz
 Description: UNKNOWN
 Keywords: Explainable AI,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `explai-0.3/explai/explai.py` & `explai-0.4/explai/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     ct.drawString(110,558,'Label Distribution',)
     ct.drawImage("histPlot.png",x=20,y=325,width=266,height=225)
     os.remove("histPlot.png")
 
     
     feats_df=standardFeatImps(pca,df_x)
     getFeatImps(model,df_x,feats_df)
-    ct.drawString(116,248,'Feature Importance',)
+    ct.drawString(106,248,'Standardised Feature Importance',)
     ct.drawImage("featsBar.png",x=20,y=14,width=250,height=225)
     os.remove("featsBar.png")
     
     
     getPermFeatImp(df_x, df_y, model)
     ct.drawString(346,248,"Permutation Feature Importance")
     ct.drawImage("barPlot.png",x=295,y=14,height=225,width=270)
@@ -232,15 +232,15 @@
     ct.drawString(435,282,evals[2])
     
     feats_df=standardFeatImps(pca,df_x)
     
     
     getFeatImps(model,df_x,feats_df)
     ct.setFont(psfontname='Times-Roman',size=15)
-    ct.drawString(116,248,'Feature Importance',)
+    ct.drawString(106,248,'Standardised Feature Importance',)
     ct.drawImage("featsBar.png",x=20,y=14,width=255,height=225)
     os.remove("featsBar.png")
     
     getDistro(df_y)
     ct.setFont(psfontname='Times-Roman',size=15)
     ct.drawString(110,558,'Label Distribution',)
     ct.drawImage("histPlot.png",x=20,y=325,width=266,height=225)
```

### Comparing `explai-0.3/setup.py` & `explai-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'explai',         # How you named your package folder (MyLib)
   packages = ['explai'],   # Chose the same as "name"
-  version = '0.3',      # Start with a small number and increase it with every change you make
+  version = '0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A reporting tool for explainable AI',   # Give a short description about your library
   author = 'Ritwik Bandyopadhyay',                   # Type in your name
   author_email = 'ritwikbanrg@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ritwikbd/explai',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ritwikbd/explai/archive/refs/tags/v03.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ritwikbd/explai/archive/refs/tags/v04.tar.gz',    # I explain this later on
   keywords = ['Explainable AI', 'Machine Learning'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'reportlab','scikit-learn','matplotlib','seaborn','pandas'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

