# Comparing `tmp/synthetic-dataset-0.0.0.1.tar.gz` & `tmp/synthetic-dataset-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetic-dataset-0.0.0.1.tar", last modified: Mon Apr 10 04:03:02 2023, max compression
+gzip compressed data, was "synthetic-dataset-0.0.0.2.tar", last modified: Mon Apr 10 04:36:45 2023, max compression
```

## Comparing `synthetic-dataset-0.0.0.1.tar` & `synthetic-dataset-0.0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 04:03:02.741350 synthetic-dataset-0.0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-04-10 03:34:47.000000 synthetic-dataset-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3275 2023-04-10 04:03:02.740374 synthetic-dataset-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2564 2023-04-10 03:58:32.000000 synthetic-dataset-0.0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 04:03:02.741350 synthetic-dataset-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1634 2023-04-10 04:02:33.000000 synthetic-dataset-0.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:03:02.739397 synthetic-dataset-0.0.0.1/synthetic_dataset.egg-info/
--rw-rw-rw-   0        0        0     3275 2023-04-10 04:03:02.000000 synthetic-dataset-0.0.0.1/synthetic_dataset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-04-10 04:03:02.000000 synthetic-dataset-0.0.0.1/synthetic_dataset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 04:03:02.000000 synthetic-dataset-0.0.0.1/synthetic_dataset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-10 04:03:02.000000 synthetic-dataset-0.0.0.1/synthetic_dataset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 04:03:02.000000 synthetic-dataset-0.0.0.1/synthetic_dataset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 04:36:45.237833 synthetic-dataset-0.0.0.2/
+-rw-rw-rw-   0        0        0     1118 2023-04-10 04:09:21.000000 synthetic-dataset-0.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3452 2023-04-10 04:36:45.237833 synthetic-dataset-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2647 2023-04-10 04:08:48.000000 synthetic-dataset-0.0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 04:36:45.238808 synthetic-dataset-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1737 2023-04-10 04:36:30.000000 synthetic-dataset-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:36:45.236853 synthetic-dataset-0.0.0.2/synthetic_dataset.egg-info/
+-rw-rw-rw-   0        0        0     3452 2023-04-10 04:36:45.000000 synthetic-dataset-0.0.0.2/synthetic_dataset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-04-10 04:36:45.000000 synthetic-dataset-0.0.0.2/synthetic_dataset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 04:36:45.000000 synthetic-dataset-0.0.0.2/synthetic_dataset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-10 04:36:45.000000 synthetic-dataset-0.0.0.2/synthetic_dataset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 04:36:45.000000 synthetic-dataset-0.0.0.2/synthetic_dataset.egg-info/top_level.txt
```

### Comparing `synthetic-dataset-0.0.0.1/LICENSE` & `synthetic-dataset-0.0.0.2/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
+we wil update it soon.
```

### Comparing `synthetic-dataset-0.0.0.1/PKG-INFO` & `synthetic-dataset-0.0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: synthetic-dataset
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: Generating accurate and safe synthetic datasets for tabular, classification, and time-series labeling tasks
-Author: Ali Nemati
-Author-email: <alinemati@gmail.com>
+Author: Synthetic Dataset AI Team
+Author-email: <admin@syntheticdataset.ai>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: Free To Use But Restricted
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Synthetic Data Generation for Tabular, Classification, and Time-Series Labels
 
 This repository contains a Python-based framework for generating accurate and safe synthetic datasets for tabular, classification, and time-series labeling tasks. It is designed to help researchers, data scientists, and machine learning engineers create high-quality, realistic datasets for training and evaluating their models while ensuring privacy and compliance with data protection regulations.
@@ -57,8 +59,8 @@
 ```
 
 
 ## Contributing
 Please read the CONTRIBUTING.md file for details on how to contribute to the project. We welcome pull requests, bug reports, and feature requests.
 
 ## License
-This project is licensed under the MIT License - see the  file for details.
+This project is licensed under the MIT License - [Licence](https://github.com/syntheticdataset/synthetic-dataset/blob/main/LICENSE) see the  file for details.
```

### Comparing `synthetic-dataset-0.0.0.1/README.md` & `synthetic-dataset-0.0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 ```
 
 
 ## Contributing
 Please read the CONTRIBUTING.md file for details on how to contribute to the project. We welcome pull requests, bug reports, and feature requests.
 
 ## License
-This project is licensed under the MIT License - see the  file for details.
+This project is licensed under the MIT License - [Licence](https://github.com/syntheticdataset/synthetic-dataset/blob/main/LICENSE) see the  file for details.
```

### Comparing `synthetic-dataset-0.0.0.1/setup.py` & `synthetic-dataset-0.0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,34 +3,37 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.0.1'
+VERSION = '0.0.0.2'
 DESCRIPTION = 'Generating accurate and safe synthetic datasets for tabular, classification, and time-series labeling tasks'
 LONG_DESCRIPTION = 'This repository contains a Python-based framework for generating accurate and safe synthetic datasets for tabular, \
 classification, and time-series labeling tasks. It is designed to help researchers, data scientists, and machine learning engineers \
 create high-quality, realistic datasets for training and evaluating their models while ensuring privacy and compliance with data protection regulations..'
 
 # Setting up
 setup(
     name="synthetic-dataset",
     version=VERSION,
-    author="Ali Nemati",
-    author_email="<alinemati@gmail.com>",
+    author="Synthetic Dataset AI Team",
+    author_email="<admin@syntheticdataset.ai>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['python', 'pandas', 'numpy', 'scikit-learn', 'scipy', 'matplotlib', 'seaborn', 'tqdm'],
     keywords=['python', 'pandas', 'numpy', 'scikit-learn', 'scipy', 'matplotlib', 'seaborn'],
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-    ]
+        "License :: Free To Use But Restricted",
+
+    ] ,
 )
```

### Comparing `synthetic-dataset-0.0.0.1/synthetic_dataset.egg-info/PKG-INFO` & `synthetic-dataset-0.0.0.2/synthetic_dataset.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: synthetic-dataset
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: Generating accurate and safe synthetic datasets for tabular, classification, and time-series labeling tasks
-Author: Ali Nemati
-Author-email: <alinemati@gmail.com>
+Author: Synthetic Dataset AI Team
+Author-email: <admin@syntheticdataset.ai>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: Free To Use But Restricted
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Synthetic Data Generation for Tabular, Classification, and Time-Series Labels
 
 This repository contains a Python-based framework for generating accurate and safe synthetic datasets for tabular, classification, and time-series labeling tasks. It is designed to help researchers, data scientists, and machine learning engineers create high-quality, realistic datasets for training and evaluating their models while ensuring privacy and compliance with data protection regulations.
@@ -57,8 +59,8 @@
 ```
 
 
 ## Contributing
 Please read the CONTRIBUTING.md file for details on how to contribute to the project. We welcome pull requests, bug reports, and feature requests.
 
 ## License
-This project is licensed under the MIT License - see the  file for details.
+This project is licensed under the MIT License - [Licence](https://github.com/syntheticdataset/synthetic-dataset/blob/main/LICENSE) see the  file for details.
```

