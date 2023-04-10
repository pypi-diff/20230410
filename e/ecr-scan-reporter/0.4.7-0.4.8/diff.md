# Comparing `tmp/ecr_scan_reporter-0.4.7.tar.gz` & `tmp/ecr_scan_reporter-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecr_scan_reporter-0.4.7.tar", max compression
+gzip compressed data, was "ecr_scan_reporter-0.4.8.tar", max compression
```

## Comparing `ecr_scan_reporter-0.4.7.tar` & `ecr_scan_reporter-0.4.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    16725 2022-05-11 06:11:13.537553 ecr_scan_reporter-0.4.7/LICENSE
--rw-r--r--   0        0        0      262 2022-05-11 06:11:13.537553 ecr_scan_reporter-0.4.7/MANIFEST.in
--rw-r--r--   0        0        0      912 2022-05-11 06:11:13.537553 ecr_scan_reporter-0.4.7/README.rst
--rw-r--r--   0        0        0      134 2022-06-01 07:00:06.148385 ecr_scan_reporter-0.4.7/ecr_scan_reporter/__init__.py
--rw-r--r--   0        0        0     2144 2022-05-11 06:11:13.539553 ecr_scan_reporter-0.4.7/ecr_scan_reporter/cli.py
--rw-r--r--   0        0        0      490 2022-05-11 06:24:07.694123 ecr_scan_reporter-0.4.7/ecr_scan_reporter/common.py
--rw-r--r--   0        0        0     1716 2022-05-11 06:24:07.692123 ecr_scan_reporter-0.4.7/ecr_scan_reporter/ecr_scan_reporter.py
--rw-r--r--   0        0        0     9111 2022-05-11 06:24:07.730123 ecr_scan_reporter-0.4.7/ecr_scan_reporter/images_scanner.py
--rw-r--r--   0        0        0     5288 2022-05-11 06:24:07.713123 ecr_scan_reporter-0.4.7/ecr_scan_reporter/lambda_functions.py
--rw-r--r--   0        0        0     2515 2022-05-11 06:24:07.710123 ecr_scan_reporter-0.4.7/ecr_scan_reporter/repos_scanner.py
--rw-r--r--   0        0        0     5059 2022-05-11 06:24:07.703123 ecr_scan_reporter-0.4.7/ecr_scan_reporter/services_scanner.py
--rw-r--r--   0        0        0     1940 2022-06-01 07:00:06.148385 ecr_scan_reporter-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1784 2022-06-01 07:00:25.062695 ecr_scan_reporter-0.4.7/setup.py
--rw-r--r--   0        0        0     1768 2022-06-01 07:00:25.062969 ecr_scan_reporter-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-05-11 06:11:13.537553 ecr_scan_reporter-0.4.8/LICENSE
+-rw-r--r--   0        0        0      262 2022-05-11 06:11:13.537553 ecr_scan_reporter-0.4.8/MANIFEST.in
+-rw-r--r--   0        0        0      912 2022-05-11 06:11:13.537553 ecr_scan_reporter-0.4.8/README.rst
+-rw-r--r--   0        0        0      134 2023-04-10 16:18:24.062186 ecr_scan_reporter-0.4.8/ecr_scan_reporter/__init__.py
+-rw-r--r--   0        0        0     2144 2022-05-11 06:11:13.539553 ecr_scan_reporter-0.4.8/ecr_scan_reporter/cli.py
+-rw-r--r--   0        0        0      490 2022-05-11 06:24:07.694123 ecr_scan_reporter-0.4.8/ecr_scan_reporter/common.py
+-rw-r--r--   0        0        0     1716 2022-05-11 06:24:07.692123 ecr_scan_reporter-0.4.8/ecr_scan_reporter/ecr_scan_reporter.py
+-rw-r--r--   0        0        0     9494 2023-04-10 16:17:54.300824 ecr_scan_reporter-0.4.8/ecr_scan_reporter/images_scanner.py
+-rw-r--r--   0        0        0     5288 2022-05-11 06:24:07.713123 ecr_scan_reporter-0.4.8/ecr_scan_reporter/lambda_functions.py
+-rw-r--r--   0        0        0     2515 2022-05-11 06:24:07.710123 ecr_scan_reporter-0.4.8/ecr_scan_reporter/repos_scanner.py
+-rw-r--r--   0        0        0     5059 2022-05-11 06:24:07.703123 ecr_scan_reporter-0.4.8/ecr_scan_reporter/services_scanner.py
+-rw-r--r--   0        0        0     1876 2023-04-10 16:18:24.062186 ecr_scan_reporter-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 ecr_scan_reporter-0.4.8/setup.py
+-rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 ecr_scan_reporter-0.4.8/PKG-INFO
```

### Comparing `ecr_scan_reporter-0.4.7/LICENSE` & `ecr_scan_reporter-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ecr_scan_reporter-0.4.7/README.rst` & `ecr_scan_reporter-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `ecr_scan_reporter-0.4.7/ecr_scan_reporter/cli.py` & `ecr_scan_reporter-0.4.8/ecr_scan_reporter/cli.py`

 * *Files identical despite different names*

### Comparing `ecr_scan_reporter-0.4.7/ecr_scan_reporter/ecr_scan_reporter.py` & `ecr_scan_reporter-0.4.8/ecr_scan_reporter/ecr_scan_reporter.py`

 * *Files identical despite different names*

### Comparing `ecr_scan_reporter-0.4.7/ecr_scan_reporter/images_scanner.py` & `ecr_scan_reporter-0.4.8/ecr_scan_reporter/images_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import re
 import warnings
 from datetime import datetime as dt
 from os import environ
 from time import sleep
 
 from boto3 import session
+from botocore.exceptions import ClientError
 from compose_x_common.compose_x_common import keyisset
 from dateutil.relativedelta import relativedelta
 from pytz import utc
 
 from ecr_scan_reporter.common import chunked_iterable
 
 DURATIONS_RE = re.compile(r"(?P<months>\dm)?(?P<weeks>\dw)?(?P<days>\dd)?(?P<hours>\dh)?")
@@ -221,14 +222,20 @@
                     )
                 except client.exceptions.ImageNotFoundException:
                     print("No image found with provided tag or digest.", image)
                     tries = 0
                 except client.exceptions.UnsupportedImageTypeException:
                     print("The image does not support scanning.")
                     tries = 0
+                except client.exceptions.InvalidParameterException as error:
+                    print(f"The scan could not be started on this repository image: {error}.")
+                    tries = 0
+                except ClientError as error:
+                    print(f"Failed to trigger scan: {error}")
+                    tries = 0
 
 
 def scan_repo_images(repo, repo_images=None, duration_override=None, no_scan_images=False, ecr_session=None):
     if ecr_session is None:
         ecr_session = session.Session()
     batch = False
     if not repo_images:
```

### Comparing `ecr_scan_reporter-0.4.7/ecr_scan_reporter/lambda_functions.py` & `ecr_scan_reporter-0.4.8/ecr_scan_reporter/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `ecr_scan_reporter-0.4.7/ecr_scan_reporter/repos_scanner.py` & `ecr_scan_reporter-0.4.8/ecr_scan_reporter/repos_scanner.py`

 * *Files identical despite different names*

### Comparing `ecr_scan_reporter-0.4.7/ecr_scan_reporter/services_scanner.py` & `ecr_scan_reporter-0.4.8/ecr_scan_reporter/services_scanner.py`

 * *Files identical despite different names*

### Comparing `ecr_scan_reporter-0.4.7/pyproject.toml` & `ecr_scan_reporter-0.4.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 [tool.poetry]
 name = "ecr_scan_reporter"
-version = "0.4.7"
+version = "0.4.8"
 description = "Stay on top of your docker images security vulnerabilities in AWS ECR"
 authors = ["John Preston <john@compose-x.io>"]
 license = "MPL-2.0"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 readme = "README.rst"
 keywords=["aws-ecr", "security", "vulnerabilities"]
 include = [
     "LICENSE",
     "MANIFEST.in"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 boto3 = "^1.22"
-pytz = "^2022.1"
-compose-x-common = "^1.0"
+pytz = "^2023.3"
+compose-x-common = "^1.2"
 
 [tool.poetry.dev-dependencies]
 sphinx-material = "^0.0.35"
 Sphinx = "^4.5.0"
-black = "^22.3"
-isort = "^5.10.1"
+black = "^23.3"
+isort = "^5.12"
 tbump = "^6.7,<7.0"
 placebo = "<1.0"
 behave = "^1.2.6"
 pytest = "^7.1"
-pre-commit = "^2.19.0"
-tox = "^3.25.0"
+pre-commit = "^3.2"
 
 [tool.poetry.scripts]
 ecr_scan_reporter = "ecr_scan_reporter.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -58,15 +56,15 @@
 line_length = 100
 known_first_party = "kelvin"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/ecr-scan-reporter"
 
 [tool.tbump.version]
-current = "0.4.7"
+current = "0.4.8"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `ecr_scan_reporter-0.4.7/setup.py` & `ecr_scan_reporter-0.4.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['ecr_scan_reporter']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3>=1.22,<2.0', 'compose-x-common>=1.0,<2.0', 'pytz>=2022.1,<2023.0']
+['boto3>=1.22,<2.0', 'compose-x-common>=1.2,<2.0', 'pytz>=2023.3,<2024.0']
 
 entry_points = \
 {'console_scripts': ['ecr_scan_reporter = ecr_scan_reporter.cli:main']}
 
 setup_kwargs = {
     'name': 'ecr-scan-reporter',
-    'version': '0.4.7',
+    'version': '0.4.8',
     'description': 'Stay on top of your docker images security vulnerabilities in AWS ECR',
     'long_description': '=================\nECR Scan Reporter\n=================\n\n\n.. image:: https://img.shields.io/pypi/v/ecr_scan_reporter.svg\n        :target: https://pypi.python.org/pypi/ecr_scan_reporter\n\n\n------------------------------------------------------------------------------------\nServerless Application to monitor ECR Repositories and capture scan results\n------------------------------------------------------------------------------------\n\nWorkflow\n==========\n\n.. image:: https://ecr-scan-reporter.compose-x.io/_images/EcrScanReporterWorkflow.jpg\n\n\nFull documentation https://ecr-scan-reporter.compose-x.io.\n\nInstall from `AWS Serveless Applications Repository`_\n\nCredits\n-------\n\nThis package was created with Cookiecutter_.\n\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _AWS Serveless Applications Repository: https://serverlessrepo.aws.amazon.com/applications/eu-west-1/518078317392/ecr-scan-reporter\n',
     'author': 'John Preston',
     'author_email': 'john@compose-x.io',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ecr_scan_reporter-0.4.7/PKG-INFO` & `ecr_scan_reporter-0.4.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: ecr-scan-reporter
-Version: 0.4.7
+Version: 0.4.8
 Summary: Stay on top of your docker images security vulnerabilities in AWS ECR
 License: MPL-2.0
 Keywords: aws-ecr,security,vulnerabilities
 Author: John Preston
 Author-email: john@compose-x.io
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: boto3 (>=1.22,<2.0)
-Requires-Dist: compose-x-common (>=1.0,<2.0)
-Requires-Dist: pytz (>=2022.1,<2023.0)
+Requires-Dist: compose-x-common (>=1.2,<2.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
 Description-Content-Type: text/x-rst
 
 =================
 ECR Scan Reporter
 =================
```

