# Comparing `tmp/gitlab-runner-tart-driver-0.0.2.tar.gz` & `tmp/gitlab-runner-tart-driver-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.0.2.tar", last modified: Mon Apr 10 08:51:50 2023, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.1.0.tar", last modified: Mon Apr 10 12:42:57 2023, max compression
```

## Comparing `gitlab-runner-tart-driver-0.0.2.tar` & `gitlab-runner-tart-driver-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 mschmieder   (501) staff       (20)        0 2023-04-10 08:51:50.939213 gitlab-runner-tart-driver-0.0.2/
--rw-r--r--   0 mschmieder   (501) staff       (20)     3303 2023-04-10 08:27:27.000000 gitlab-runner-tart-driver-0.0.2/LICENSE.txt
--rw-r--r--   0 mschmieder   (501) staff       (20)    13443 2023-04-10 08:51:50.938899 gitlab-runner-tart-driver-0.0.2/PKG-INFO
--rw-r--r--   0 mschmieder   (501) staff       (20)    12922 2023-04-10 05:42:40.000000 gitlab-runner-tart-driver-0.0.2/README.md
-drwxr-xr-x   0 mschmieder   (501) staff       (20)        0 2023-04-10 08:51:50.936100 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/
--rw-r--r--   0 mschmieder   (501) staff       (20)       22 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/__init__.py
--rw-r--r--   0 mschmieder   (501) staff       (20)      107 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/__main__.py
--rw-r--r--   0 mschmieder   (501) staff       (20)      596 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 mschmieder   (501) staff       (20)        0 2023-04-10 08:51:50.937834 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/
--rw-r--r--   0 mschmieder   (501) staff       (20)        0 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/__init__.py
--rw-r--r--   0 mschmieder   (501) staff       (20)      952 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/cleanup.py
--rw-r--r--   0 mschmieder   (501) staff       (20)      775 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/config.py
--rw-r--r--   0 mschmieder   (501) staff       (20)     5005 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/prepare.py
--rw-r--r--   0 mschmieder   (501) staff       (20)     3300 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 mschmieder   (501) staff       (20)        0 2023-04-10 08:51:50.938635 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/modules/
--rw-r--r--   0 mschmieder   (501) staff       (20)        0 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/modules/__init__.py
--rw-r--r--   0 mschmieder   (501) staff       (20)      908 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-r--r--   0 mschmieder   (501) staff       (20)      405 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-r--r--   0 mschmieder   (501) staff       (20)     5231 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/modules/tart.py
--rw-r--r--   0 mschmieder   (501) staff       (20)      923 2023-04-10 05:38:49.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 mschmieder   (501) staff       (20)        0 2023-04-10 08:51:50.937048 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 mschmieder   (501) staff       (20)    13443 2023-04-10 08:51:50.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 mschmieder   (501) staff       (20)      986 2023-04-10 08:51:50.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 mschmieder   (501) staff       (20)        1 2023-04-10 08:51:50.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 mschmieder   (501) staff       (20)       82 2023-04-10 08:51:50.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 mschmieder   (501) staff       (20)        1 2023-04-10 08:51:50.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 mschmieder   (501) staff       (20)       40 2023-04-10 08:51:50.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 mschmieder   (501) staff       (20)       26 2023-04-10 08:51:50.000000 gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-r--r--   0 mschmieder   (501) staff       (20)       31 2023-04-10 05:38:32.000000 gitlab-runner-tart-driver-0.0.2/pyproject.toml
--rw-r--r--   0 mschmieder   (501) staff       (20)       38 2023-04-10 08:51:50.939255 gitlab-runner-tart-driver-0.0.2/setup.cfg
--rw-r--r--   0 mschmieder   (501) staff       (20)     1461 2023-04-10 05:41:09.000000 gitlab-runner-tart-driver-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.657450 gitlab-runner-tart-driver-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    13443 2023-04-10 12:42:57.657450 gitlab-runner-tart-driver-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12922 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.650449 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.655449 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5005 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     3300 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.656450 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5231 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.653449 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13443 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      986 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 12:42:57.657450 gitlab-runner-tart-driver-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.0.2/LICENSE.txt` & `gitlab-runner-tart-driver-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/PKG-INFO` & `gitlab-runner-tart-driver-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.0.2
-Home-page: https://gitlab.com/matthias.schmieder/gitlab-runner-tart-driver
+Version: 0.1.0
+Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
```

### Comparing `gitlab-runner-tart-driver-0.0.2/README.md` & `gitlab-runner-tart-driver-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/cleanup.py` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/prepare.py` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/run.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/tart.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.0.2
-Home-page: https://gitlab.com/matthias.schmieder/gitlab-runner-tart-driver
+Version: 0.1.0
+Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
```

### Comparing `gitlab-runner-tart-driver-0.0.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.0.2/setup.py` & `gitlab-runner-tart-driver-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.0.2"
+version = "0.1.0"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
 
 setup(
     name="gitlab-runner-tart-driver",
     version=version,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://gitlab.com/matthias.schmieder/gitlab-runner-tart-driver",
+    url="https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver",
     author="Matthias Schmieder",
     author_email="schmieder.matthias@gmail.com",
     entry_points={"console_scripts": ["gitlab-runner-tart-driver = gitlab_runner_tart_driver.cli:start"]},
     license="BSD",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.9",
```

