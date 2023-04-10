# Comparing `tmp/data_ecosystem_services-202304.0.4.tar.gz` & `tmp/data_ecosystem_services-202304.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202304.0.4.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202304.0.5.tar", max compression
```

## Comparing `data_ecosystem_services-202304.0.4.tar` & `data_ecosystem_services-202304.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      857 2023-04-08 14:05:48.841145 data_ecosystem_services-202304.0.4/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0      916 2023-04-08 14:05:48.841145 data_ecosystem_services-202304.0.4/data_ecosystem_services/admin_service/__init__.py
--rw-r--r--   0        0        0     4670 2023-04-08 14:05:48.841145 data_ecosystem_services-202304.0.4/data_ecosystem_services/admin_service/environment_logging.py
--rw-r--r--   0        0        0      958 2023-04-08 14:05:48.841145 data_ecosystem_services-202304.0.4/data_ecosystem_services/security_service/__init__.py
--rw-r--r--   0        0        0     3431 2023-04-08 14:05:48.841145 data_ecosystem_services-202304.0.4/data_ecosystem_services/security_service/security_alation.py
--rw-r--r--   0        0        0    14614 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/security_service/security_core.py
--rw-r--r--   0        0        0     1115 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/__init__.py
--rw-r--r--   0        0        0    41371 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/dataset_metadata.py
--rw-r--r--   0        0        0    32651 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/environment_metadata.py
--rw-r--r--   0        0        0    36036 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/job_metadata.py
--rw-r--r--   0        0        0     2261 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/logging_metadata.py
--rw-r--r--   0        0        0    22304 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1472 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33731 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8716 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    24963 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3777 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     1997 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    26185 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     4589 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17224 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/repo_core.py
--rw-r--r--   0        0        0    10094 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_schema/manifest.py
--rw-r--r--   0        0        0    11357 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/license.md
--rw-r--r--   0        0        0     3345 2023-04-08 14:08:31.739167 data_ecosystem_services-202304.0.4/pyproject.toml
--rw-r--r--   0        0        0    46407 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/readme.md
--rw-r--r--   0        0        0      118 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/setup.cfg
--rw-r--r--   0        0        0      127 2023-04-08 14:05:48.845145 data_ecosystem_services-202304.0.4/setup.py
--rw-r--r--   0        0        0    49218 1970-01-01 00:00:00.000000 data_ecosystem_services-202304.0.4/PKG-INFO
+-rw-r--r--   0        0        0      857 2023-04-10 16:14:11.361288 data_ecosystem_services-202304.0.5/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0      916 2023-04-10 16:14:11.361288 data_ecosystem_services-202304.0.5/data_ecosystem_services/admin_service/__init__.py
+-rw-r--r--   0        0        0     4670 2023-04-10 16:14:11.361288 data_ecosystem_services-202304.0.5/data_ecosystem_services/admin_service/environment_logging.py
+-rw-r--r--   0        0        0      958 2023-04-10 16:14:11.361288 data_ecosystem_services-202304.0.5/data_ecosystem_services/security_service/__init__.py
+-rw-r--r--   0        0        0     3431 2023-04-10 16:14:11.361288 data_ecosystem_services-202304.0.5/data_ecosystem_services/security_service/security_alation.py
+-rw-r--r--   0        0        0    14614 2023-04-10 16:14:11.361288 data_ecosystem_services-202304.0.5/data_ecosystem_services/security_service/security_core.py
+-rw-r--r--   0        0        0     1115 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/__init__.py
+-rw-r--r--   0        0        0    41371 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    32651 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36036 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/job_metadata.py
+-rw-r--r--   0        0        0     2261 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22304 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1472 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33731 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8716 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    24963 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3777 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     1997 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    26185 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     4589 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17224 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0    10094 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_schema/manifest.py
+-rw-r--r--   0        0        0    11357 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/license.md
+-rw-r--r--   0        0        0     3345 2023-04-10 16:17:09.037820 data_ecosystem_services-202304.0.5/pyproject.toml
+-rw-r--r--   0        0        0    46691 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/readme.md
+-rw-r--r--   0        0        0      118 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/setup.cfg
+-rw-r--r--   0        0        0      127 2023-04-10 16:14:11.365289 data_ecosystem_services-202304.0.5/setup.py
+-rw-r--r--   0        0        0    49502 1970-01-01 00:00:00.000000 data_ecosystem_services-202304.0.5/PKG-INFO
```

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/admin_service/__init__.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/admin_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/admin_service/environment_logging.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/admin_service/environment_logging.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/security_service/__init__.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/security_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/security_service/security_alation.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/security_service/security_alation.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/security_service/security_core.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/security_service/security_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/__init__.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/dataset_metadata.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/environment_metadata.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/environment_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/job_metadata.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/logging_metadata.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/self_service/pipeline_metadata.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/__init__.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/dataset_convert.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/dataset_core.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/dataset_crud.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/dataset_extract.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/environment_core.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/environment_file.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/environment_file.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/environment_spark.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/environment_spark.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/job_core.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_environment_service/repo_core.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/data_ecosystem_services/tech_schema/manifest.py` & `data_ecosystem_services-202304.0.5/data_ecosystem_services/tech_schema/manifest.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/license.md` & `data_ecosystem_services-202304.0.5/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.4/pyproject.toml` & `data_ecosystem_services-202304.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202304.0.4"
+version="202304.0.5"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
```

### Comparing `data_ecosystem_services-202304.0.4/readme.md` & `data_ecosystem_services-202304.0.5/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,65 +13,72 @@
 
 ### Check if Python is installed
 
 Run in bash or powershell
 
 1. Check Python Version
 
-```sh
-python3 --version
-```
-
-2. Validate is 3.9
+        ```sh
+        python3 --version
+        ```
 
 ### Install Python 3.9
 
 #### Run Install Python on Ubuntu or WSL (Primary)
 
-```sh
-sudo apt update
-sudo apt install python3.9
-```
+        ```sh
+        sudo apt update
+        sudo apt install python3.9
+        ```
+
+Update Path
+
+        ```sh
+        nano ~/.bashrc
+        export PATH="/usr/bin/python3.9:$PATH"
+        source ~/.bashrc
+        ```
+        
 
 #### Run Install Python on windows
 
 Run Application
 
-```sh
-C:\Users\zfi4\OneDrive - CDC\DAVT Analytics\davt-analytics-software\python\python-3.9.0-amd64
-```
+        ```sh
+        C:\Users\zfi4\OneDrive - CDC\DAVT Analytics\davt-analytics-software\python\python-3.9.0-amd64
+        ```
 
 ### Install Pip
 
 #### Run Install Pip on Ubuntu or WSL (Primary)
 
-```sh
-sudo apt update
-sudo apt-get install python3-pip
-```
+        ```sh
+        sudo apt update
+        sudo apt-get install python3-pip
+        ```
 
 #### Run Install Pip on Windows
 
-```sh
-py -m ensurepip --upgrade
-```
+        ```sh
+        py -m ensurepip --upgrade
+        ```
 
 ### Install Virtual Environment
 
 #### Run Install Virtual Environment on Ubuntu or WSL (Primary)
 
 See [Virtual Environment Set Reference Article](https://www.freecodecamp.org/news/virtualenv-with-virtualenvwrapper-on-ubuntu-18-04/)
 
 If first virtual environment on desktop
 
 1. Open Terminal in home directory
 
-```sh
-cd $HOME
-```
+        ```sh
+        cd $HOME
+        ```
 
 2. Create Directory for virtual environment
 
 ```sh
 mkdir .virtualenv
 ```
 
@@ -1070,15 +1077,15 @@
 Solution:
 
 1. Run
 
 ```sh
 export PATH="$HOME/.local/bin:$PATH"
 echo "export WORKON_HOME=$HOME/.virtualenvs" | sudo tee -a $HOME/.bashrc
-echo "VIRTUALENVWRAPPER_PYTHON='/usr/lib/python3.8'" | sudo tee -a $HOME/.bashrc
+echo "VIRTUALENVWRAPPER_PYTHON='/usr/lib/python3.9'" | sudo tee -a $HOME/.bashrc
 echo "source $HOME/.local/bin/virtualenvwrapper.sh" | sudo tee -a $HOME/.bashrc
 source $HOME/.bashrc
 ```
 
 ### Error: Puppeteer: can't launch chromium, missing shared library libgbm.so
 
 Symptom: Receiving error: "Error: Failed to launch the browser process! /usr/bin/chromium: error while loading shared libraries: libgbm.so.1: cannot open shared object file: No such file or directory"
```

### Comparing `data_ecosystem_services-202304.0.4/PKG-INFO` & `data_ecosystem_services-202304.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202304.0.4
+Version: 202304.0.5
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -78,65 +78,72 @@
 
 ### Check if Python is installed
 
 Run in bash or powershell
 
 1. Check Python Version
 
-```sh
-python3 --version
-```
-
-2. Validate is 3.9
+        ```sh
+        python3 --version
+        ```
 
 ### Install Python 3.9
 
 #### Run Install Python on Ubuntu or WSL (Primary)
 
-```sh
-sudo apt update
-sudo apt install python3.9
-```
+        ```sh
+        sudo apt update
+        sudo apt install python3.9
+        ```
+
+Update Path
+
+        ```sh
+        nano ~/.bashrc
+        export PATH="/usr/bin/python3.9:$PATH"
+        source ~/.bashrc
+        ```
+        
 
 #### Run Install Python on windows
 
 Run Application
 
-```sh
-C:\Users\zfi4\OneDrive - CDC\DAVT Analytics\davt-analytics-software\python\python-3.9.0-amd64
-```
+        ```sh
+        C:\Users\zfi4\OneDrive - CDC\DAVT Analytics\davt-analytics-software\python\python-3.9.0-amd64
+        ```
 
 ### Install Pip
 
 #### Run Install Pip on Ubuntu or WSL (Primary)
 
-```sh
-sudo apt update
-sudo apt-get install python3-pip
-```
+        ```sh
+        sudo apt update
+        sudo apt-get install python3-pip
+        ```
 
 #### Run Install Pip on Windows
 
-```sh
-py -m ensurepip --upgrade
-```
+        ```sh
+        py -m ensurepip --upgrade
+        ```
 
 ### Install Virtual Environment
 
 #### Run Install Virtual Environment on Ubuntu or WSL (Primary)
 
 See [Virtual Environment Set Reference Article](https://www.freecodecamp.org/news/virtualenv-with-virtualenvwrapper-on-ubuntu-18-04/)
 
 If first virtual environment on desktop
 
 1. Open Terminal in home directory
 
-```sh
-cd $HOME
-```
+        ```sh
+        cd $HOME
+        ```
 
 2. Create Directory for virtual environment
 
 ```sh
 mkdir .virtualenv
 ```
 
@@ -1135,15 +1142,15 @@
 Solution:
 
 1. Run
 
 ```sh
 export PATH="$HOME/.local/bin:$PATH"
 echo "export WORKON_HOME=$HOME/.virtualenvs" | sudo tee -a $HOME/.bashrc
-echo "VIRTUALENVWRAPPER_PYTHON='/usr/lib/python3.8'" | sudo tee -a $HOME/.bashrc
+echo "VIRTUALENVWRAPPER_PYTHON='/usr/lib/python3.9'" | sudo tee -a $HOME/.bashrc
 echo "source $HOME/.local/bin/virtualenvwrapper.sh" | sudo tee -a $HOME/.bashrc
 source $HOME/.bashrc
 ```
 
 ### Error: Puppeteer: can't launch chromium, missing shared library libgbm.so
 
 Symptom: Receiving error: "Error: Failed to launch the browser process! /usr/bin/chromium: error while loading shared libraries: libgbm.so.1: cannot open shared object file: No such file or directory"
```

