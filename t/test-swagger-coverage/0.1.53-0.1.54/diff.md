# Comparing `tmp/test-swagger-coverage-0.1.53.tar.gz` & `tmp/test_swagger_coverage-0.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-swagger-coverage-0.1.53.tar", max compression
+gzip compressed data, was "test_swagger_coverage-0.1.54.tar", max compression
```

## Comparing `test-swagger-coverage-0.1.53.tar` & `test_swagger_coverage-0.1.54.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0    11357 2022-04-12 06:02:17.000000 test-swagger-coverage-0.1.53/LICENSE
--rw-r--r--   0        0        0     5845 2023-02-06 09:39:53.948563 test-swagger-coverage-0.1.53/README.md
--rw-r--r--   0        0        0      703 2023-02-08 10:49:30.082547 test-swagger-coverage-0.1.53/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-13 12:28:55.000000 test-swagger-coverage-0.1.53/swagger_coverage/__init__.py
--rw-r--r--   0        0        0        0 2022-04-14 10:28:56.000000 test-swagger-coverage-0.1.53/swagger_coverage/scripts/__init__.py
--rw-r--r--   0        0        0     1314 2023-02-01 11:44:19.866972 test-swagger-coverage-0.1.53/swagger_coverage/scripts/swagger_report.py
--rw-r--r--   0        0        0     1300 2023-02-01 11:44:19.867322 test-swagger-coverage-0.1.53/swagger_coverage/src/check_data.py
--rw-r--r--   0        0        0     6292 2023-02-08 10:42:05.329100 test-swagger-coverage-0.1.53/swagger_coverage/src/coverage.py
--rw-r--r--   0        0        0      576 2023-01-27 11:38:26.129909 test-swagger-coverage-0.1.53/swagger_coverage/src/deco.py
--rw-r--r--   0        0        0     2897 2022-05-15 04:57:02.000000 test-swagger-coverage-0.1.53/swagger_coverage/src/files/script.js
--rw-r--r--   0        0        0     1297 2023-02-06 09:38:59.285713 test-swagger-coverage-0.1.53/swagger_coverage/src/files.py
--rw-r--r--   0        0        0      849 2022-05-15 04:57:02.000000 test-swagger-coverage-0.1.53/swagger_coverage/src/logger.py
--rw-r--r--   0        0        0      907 2022-05-15 04:57:02.000000 test-swagger-coverage-0.1.53/swagger_coverage/src/models.py
--rw-r--r--   0        0        0     1884 2023-02-01 11:44:19.869276 test-swagger-coverage-0.1.53/swagger_coverage/src/prepare_data.py
--rw-r--r--   0        0        0    16730 2023-02-08 08:51:35.873521 test-swagger-coverage-0.1.53/swagger_coverage/src/report.py
--rw-r--r--   0        0        0      326 2022-05-15 04:57:02.000000 test-swagger-coverage-0.1.53/swagger_coverage/src/singltone_like.py
--rw-r--r--   0        0        0     2008 2022-05-15 04:57:02.000000 test-swagger-coverage-0.1.53/swagger_coverage/src/swagger_diff.py
--rw-r--r--   0        0        0     4860 2023-02-08 10:49:17.407675 test-swagger-coverage-0.1.53/swagger_coverage/src/utils.py
--rw-r--r--   0        0        0     7018 2023-02-08 10:49:32.494826 test-swagger-coverage-0.1.53/setup.py
--rw-r--r--   0        0        0     6560 2023-02-08 10:49:32.495231 test-swagger-coverage-0.1.53/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 11:50:18.636935 test_swagger_coverage-0.1.54/LICENSE
+-rw-r--r--   0        0        0     5845 2023-04-10 11:50:18.637247 test_swagger_coverage-0.1.54/README.md
+-rw-r--r--   0        0        0      685 2023-04-10 12:01:19.306316 test_swagger_coverage-0.1.54/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:50:18.637989 test_swagger_coverage-0.1.54/swagger_coverage/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:50:18.638133 test_swagger_coverage-0.1.54/swagger_coverage/scripts/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-10 11:50:18.638296 test_swagger_coverage-0.1.54/swagger_coverage/scripts/swagger_report.py
+-rw-r--r--   0        0        0     1300 2023-04-10 11:50:18.638469 test_swagger_coverage-0.1.54/swagger_coverage/src/check_data.py
+-rw-r--r--   0        0        0     6302 2023-04-10 11:50:18.638626 test_swagger_coverage-0.1.54/swagger_coverage/src/coverage.py
+-rw-r--r--   0        0        0      576 2023-04-10 11:50:18.638741 test_swagger_coverage-0.1.54/swagger_coverage/src/deco.py
+-rw-r--r--   0        0        0     1297 2023-04-10 11:50:18.638879 test_swagger_coverage-0.1.54/swagger_coverage/src/files.py
+-rw-r--r--   0        0        0      849 2023-04-10 11:50:18.639190 test_swagger_coverage-0.1.54/swagger_coverage/src/logger.py
+-rw-r--r--   0        0        0      907 2023-04-10 11:50:18.639306 test_swagger_coverage-0.1.54/swagger_coverage/src/models.py
+-rw-r--r--   0        0        0     1884 2023-04-10 11:50:18.639434 test_swagger_coverage-0.1.54/swagger_coverage/src/prepare_data.py
+-rw-r--r--   0        0        0    16694 2023-04-10 11:50:18.639647 test_swagger_coverage-0.1.54/swagger_coverage/src/report.py
+-rw-r--r--   0        0        0      326 2023-04-10 11:50:18.639786 test_swagger_coverage-0.1.54/swagger_coverage/src/singltone_like.py
+-rw-r--r--   0        0        0     2008 2023-04-10 11:50:18.639926 test_swagger_coverage-0.1.54/swagger_coverage/src/swagger_diff.py
+-rw-r--r--   0        0        0     3992 2023-04-10 11:50:18.640099 test_swagger_coverage-0.1.54/swagger_coverage/src/utils.py
+-rw-r--r--   0        0        0     6571 1970-01-01 00:00:00.000000 test_swagger_coverage-0.1.54/PKG-INFO
```

### Comparing `test-swagger-coverage-0.1.53/LICENSE` & `test_swagger_coverage-0.1.54/LICENSE`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/README.md` & `test_swagger_coverage-0.1.54/README.md`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/pyproject.toml` & `test_swagger_coverage-0.1.54/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "test-swagger-coverage"
-version = "0.1.53"
+version = "0.1.54"
 description = "Swagger coverage for API tests"
 authors = ["alexanderlozovoy <berpress@gmail.com>"]
 packages = [{ include = "swagger_coverage" }]
 readme = "README.md"
 repository = "https://github.com/berpress/swagger-coverage"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.27.1"
 PyYAML = "^6.0"
-attrs = "^21.4.0"
 Jinja2 = "^3.1.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 pytest-cov = "^3.0.0"
 coverage = "^6.3.2"
 pre-commit = "^2.18.1"
```

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/scripts/swagger_report.py` & `test_swagger_coverage-0.1.54/swagger_coverage/scripts/swagger_report.py`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/src/check_data.py` & `test_swagger_coverage-0.1.54/swagger_coverage/src/check_data.py`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/src/coverage.py` & `test_swagger_coverage-0.1.54/swagger_coverage/src/coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from swagger_coverage.src.report import ReportHtml
 from swagger_coverage.src.singltone_like import Singleton
 from swagger_coverage.src.swagger_diff import DataDiff
 from swagger_coverage.src.files import FileOperation
 from swagger_coverage.src.prepare_data import PrepareData
 from swagger_coverage.src.utils import to_dict, merge_results
 
-
 logger = logging.getLogger("swagger")
 
 
 class SwaggerCoverage(metaclass=Singleton):
     """
     Tool for calculating status coverage in api tests
     First, you need to create a file for verification, for example
@@ -102,40 +101,40 @@
 
     @staticmethod
     def create_results_from_json(path: str = None):
         # Load data from json files
         parent_dir = os.path.abspath(os.path.abspath(os.curdir))
         path_to_results = os.path.join(parent_dir, "swagger_report", "json_results")
         get_all_files = list(pathlib.Path(path_to_results).glob("*.json"))
-        results, summary_dict = merge_results(get_all_files)
+        results = merge_results(get_all_files)
         api_url = results.get("api_url")
         swagger_url = results.get("swagger_url")
-        # summary_dict = results.get("data").get("summary")
+        summary_dict = results.get("data").get("summary")
         if not path:
             path = results.get("path")
         summary_class = (
             EndpointStatisticsHtml(
-                endpoints=summary_dict[0].endpoints,
-                checked_endpoints=summary_dict[0].checked_endpoints,
-                not_checked_endpoints=summary_dict[0].not_checked_endpoints,
-                not_added_endpoints=summary_dict[0].not_added_endpoints,
+                endpoints=summary_dict[0].get("endpoints"),
+                checked_endpoints=summary_dict[0].get("checked_endpoints"),
+                not_checked_endpoints=summary_dict[0].get("not_checked_endpoints"),
+                not_added_endpoints=summary_dict[0].get("not_added_endpoints"),
             ),
             PercentStatistic(
-                summary_dict[1].success, summary_dict[1].failed)
-            )
+                summary_dict[1].get("success"), summary_dict[1].get("failed")
+            ),
+        )
         data_class = SwaggerData(
             swagger_data=results.get("data").get("swagger_data"),
             diff=results.get("data").get("diff"),
-            summary=summary_class
+            summary=summary_class,
         )
         reporter = ReportHtml(
             path=path, api_url=api_url, swagger_url=swagger_url, data=data_class
         )
         reporter.save_html()
-        return data_class
 
     def save_results(self, path: str = None):
         """
         Save result in json file
         :return:
         """
         paths = self.prepare.load_swagger(self.url)
```

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/src/deco.py` & `test_swagger_coverage-0.1.54/swagger_coverage/src/deco.py`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/src/files.py` & `test_swagger_coverage-0.1.54/swagger_coverage/src/files.py`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/src/logger.py` & `test_swagger_coverage-0.1.54/swagger_coverage/src/logger.py`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/src/models.py` & `test_swagger_coverage-0.1.54/swagger_coverage/src/models.py`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/src/prepare_data.py` & `test_swagger_coverage-0.1.54/swagger_coverage/src/prepare_data.py`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/src/report.py` & `test_swagger_coverage-0.1.54/swagger_coverage/src/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         for count, res in enumerate(results):
             table_body.append('<thead style="font-style: normal">\n')
             table_body.append(
                 f'<tr class="table-{res.get("color")}" style="font-style: normal">\n'
             )
             table_body.append(f'<th scope="col">{count + 1}</th>\n')
             table_body.append(f'<th scope="col">{res.get("name")}</th>\n')
-            table_body.append(f'<th scope="col">{str(res.get("results"))[:5]}</th>\n')
+            table_body.append(f'<th scope="col">{res.get("results")}</th>\n')
             table_body.append("</tr>\n")
             table_body.append("</thead>\n")
         return "".join(table_body)
 
     @staticmethod
     def _create_section(status: dict) -> str:
         st, result = list(status.items())[0]
@@ -311,15 +311,15 @@
             table_rows.append(res)
 
         desc = value.get("description", "-")
         if desc is None:
             desc = "-"
 
         avg_execution = value.get("time_executions")
-        if avg_execution is None or len(avg_execution) == 0:
+        if avg_execution is None:
             summery_time_exc = "-"
         else:
             summery_time_exc = sum(avg_execution) / len(avg_execution)
         return f"""
         <div class="accordion-item">
             <h2 class="accordion-header" id="{endpoint}">
                     <button class="accordion-button collapsed" type="button"
```

### Comparing `test-swagger-coverage-0.1.53/swagger_coverage/src/swagger_diff.py` & `test_swagger_coverage-0.1.54/swagger_coverage/src/swagger_diff.py`

 * *Files identical despite different names*

### Comparing `test-swagger-coverage-0.1.53/setup.py` & `test_swagger_coverage-0.1.54/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,174 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: test-swagger-coverage
+Version: 0.1.54
+Summary: Swagger coverage for API tests
+Home-page: https://github.com/berpress/swagger-coverage
+Author: alexanderlozovoy
+Author-email: berpress@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Project-URL: Repository, https://github.com/berpress/swagger-coverage
+Description-Content-Type: text/markdown
 
-packages = \
-['swagger_coverage', 'swagger_coverage.scripts', 'swagger_coverage.src']
+# swagger-coverage
+[![Tests](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml/badge.svg)](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml)
+![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
+[![Maintainability](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/maintainability)](https://codeclimate.com/github/berpress/swagger-coverage/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/test_coverage)](https://codeclimate.com/github/berpress/swagger-coverage/test_coverage)
+[![PyPI version](https://badge.fury.io/py/test-swagger-coverage.svg)](https://badge.fury.io/py/test-swagger-coverage)
+[![Downloads](https://pepy.tech/badge/test-swagger-coverage)](https://pepy.tech/project/test-swagger-coverage)
 
-package_data = \
-{'': ['*'], 'swagger_coverage.src': ['files/*']}
+About
+------------
 
-install_requires = \
-['Jinja2>=3.1.2,<4.0.0',
- 'PyYAML>=6.0,<7.0',
- 'attrs>=21.4.0,<22.0.0',
- 'requests>=2.27.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['swagger_coverage = '
-                     'swagger_coverage.scripts.swagger_report:main']}
-
-setup_kwargs = {
-    'name': 'test-swagger-coverage',
-    'version': '0.1.53',
-    'description': 'Swagger coverage for API tests',
-    'long_description': '# swagger-coverage\n[![Tests](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml/badge.svg)](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml)\n![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)\n[![Maintainability](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/maintainability)](https://codeclimate.com/github/berpress/swagger-coverage/maintainability)\n[![Test Coverage](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/test_coverage)](https://codeclimate.com/github/berpress/swagger-coverage/test_coverage)\n[![PyPI version](https://badge.fury.io/py/test-swagger-coverage.svg)](https://badge.fury.io/py/test-swagger-coverage)\n[![Downloads](https://pepy.tech/badge/test-swagger-coverage)](https://pepy.tech/project/test-swagger-coverage)\n\nAbout\n------------\n\nSwagger coverage report helps the QA automation and developer to get a simple API coverage report for endpoints tests\n\n![](https://github.com/berpress/python-api-tests/blob/main/images/swagger_report_2.png)\n\nInstallation\n------------\n\nYou can install ``test-swagger-coverage`` via `pip`_ from `PyPI`_::\n\n    $ pip install test-swagger-coverage\n\nor with poetry\n\n    $ poetry add test-swagger-coverage\n\nHow it works\n------------\nWe take a swagger as data for testing coverage and, based on it, we create a file that will be the settings for our tests. The file can be created automatically or manually.\n\nNext, we set up api calls in our tests (we wrap them with decorators, see examples) and at the end of testing we generate html report.\nWe will check which endpoints were called and what statuses we checked.\n\nWe can\'t always trust our swagger, so you can manually set the status of the codes yourself, which need to be checked.\n\nExamples\n------------\n\nFirst, we need a link to your swagger. For example,  let\'s take this  https://app.swaggerhub.com/apis-docs/berpress/flask-rest-api/1.0.0 (see more about this api https://github.com/berpress/flask-restful-api),\nand take url to yaml/yml/json swagger file - https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0\n\nNext, in our project, we need to create a file describing our endpoints, which our tests will use to generate a coverage report.\n\nWe can do it automatically via the command line\n\n    $ swagger_coverage https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0\n\nResult\n\n    $ 2022-04-15 11:22:37 INFO Start load swagger https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0\n    $ 2022-04-15 11:22:38 INFO The swagger report was successfully saved to the folder: /Users/user/Documents/git/python-api-tests/swagger_report\n\n\n\nThe **swagger_report** directory will be created\nand a **data_swagger.yaml** file will appear inside, which will be the settings for building a test coverage report\n\nThe **data_swagger.yaml** file looks something like this\n\n\n ```\n ...\nregUser:\n  description: null\n  method: POST\n  path: /register\n  statuses:\n  - 201  <---- change from 200 to 201\n  - 400\n  - 401\n  - 403\n  tag: register\n  ...\n ```\n\nwhere **regUser** is the unique id of our endpoint\n\n**statuses** is a list of statuses that we will check (that they were called).\nYou can customize this list yourself.\n\nOnly we will check 201 status, as described in the user registration swagger. So I will add it.\n\n\nLet\'s create a simple test and build a report. For requests, you will use the **requests** library.\n\n```python\nimport requests\nfrom swagger_coverage.src.coverage import SwaggerCoverage\nfrom swagger_coverage.src.deco import swagger\n\n# swagger data preparation\nswagger_url = "https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0"\napi_url = "https://api.swaggerhub.com/apis/"\npath=\'/report\' # path to swagger coverage report\nswagger_rep = SwaggerCoverage(api_url=api_url, url=swagger_url, path=path)\nswagger_rep.create_coverage_data()\n\n\n# function to call a request to the server\n@swagger("regUser")\ndef register_user(payload: dict):\n    return requests.post(\'https://stores-tests-api.herokuapp.com/register\',\n                         json=payload)\n\n\n# test\ndata = {"username": "test2023@test.com", "password": "Password"}\nresponse = register_user(data)\nassert response.status_code == 201\n\n# create report\nswagger_rep.create_report()\n\n```\n**swagger data preparation**: Prepare our file data_swagger.yaml, it will be created automatically.\n\n**function to call a request to the server**:  We will write a user registration call. Declaring a function with a decorator **@swagger("regUser")**.\n**"regUser"** taken from file **data_swagger.yaml**, this is unique id of our endpoint.\n\n**test**: run the test\n\n**create report**: create a report.\n\n\nAfter that, in the folder **swagger_report** we will receive a report **index.html**.\n\nLet\'s see it\n\n![](https://github.com/berpress/python-api-tests/blob/main/images/swagger_register.png)\n\nAs you can see, we have increased the counter of verified endpoints\n\nIf you use **pytest**, add this code in conftest.py\n\n```python\n@pytest.fixture(scope="session", autouse=True)\ndef swagger_checker(request):\n    url = request.config.getoption("--swagger-url")\n    url_api = request.config.getoption("--api-url")\n    path = \'/report\'\n    swagger = SwaggerCoverage(api_url=url_api, url=url, path=path)\n    swagger.create_coverage_data()\n    yield\n    swagger.create_report()\n```\nAlso, at the end of the report, you can find a table of average request times for routes\n![](https://github.com/berpress/python-api-tests/blob/main/images/requets_time.png?raw=true)\n\n\nAlso, at the end of the report, you can find a table of average request times for routes\n\nMore example with pytest and API tests https://github.com/berpress/python-api-tests\n\nReport example [https://github.com/berpress/python-api-tests/tree/main/swagger_report](https://github.com/berpress/python-api-tests/tree/main/report)\n',
-    'author': 'alexanderlozovoy',
-    'author_email': 'berpress@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/berpress/swagger-coverage',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+Swagger coverage report helps the QA automation and developer to get a simple API coverage report for endpoints tests
 
+![](https://github.com/berpress/python-api-tests/blob/main/images/swagger_report_2.png)
+
+Installation
+------------
+
+You can install ``test-swagger-coverage`` via `pip`_ from `PyPI`_::
+
+    $ pip install test-swagger-coverage
+
+or with poetry
+
+    $ poetry add test-swagger-coverage
+
+How it works
+------------
+We take a swagger as data for testing coverage and, based on it, we create a file that will be the settings for our tests. The file can be created automatically or manually.
+
+Next, we set up api calls in our tests (we wrap them with decorators, see examples) and at the end of testing we generate html report.
+We will check which endpoints were called and what statuses we checked.
+
+We can't always trust our swagger, so you can manually set the status of the codes yourself, which need to be checked.
+
+Examples
+------------
+
+First, we need a link to your swagger. For example,  let's take this  https://app.swaggerhub.com/apis-docs/berpress/flask-rest-api/1.0.0 (see more about this api https://github.com/berpress/flask-restful-api),
+and take url to yaml/yml/json swagger file - https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0
+
+Next, in our project, we need to create a file describing our endpoints, which our tests will use to generate a coverage report.
+
+We can do it automatically via the command line
+
+    $ swagger_coverage https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0
+
+Result
+
+    $ 2022-04-15 11:22:37 INFO Start load swagger https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0
+    $ 2022-04-15 11:22:38 INFO The swagger report was successfully saved to the folder: /Users/user/Documents/git/python-api-tests/swagger_report
+
+
+
+The **swagger_report** directory will be created
+and a **data_swagger.yaml** file will appear inside, which will be the settings for building a test coverage report
+
+The **data_swagger.yaml** file looks something like this
+
+
+ ```
+ ...
+regUser:
+  description: null
+  method: POST
+  path: /register
+  statuses:
+  - 201  <---- change from 200 to 201
+  - 400
+  - 401
+  - 403
+  tag: register
+  ...
+ ```
+
+where **regUser** is the unique id of our endpoint
+
+**statuses** is a list of statuses that we will check (that they were called).
+You can customize this list yourself.
+
+Only we will check 201 status, as described in the user registration swagger. So I will add it.
+
+
+Let's create a simple test and build a report. For requests, you will use the **requests** library.
+
+```python
+import requests
+from swagger_coverage.src.coverage import SwaggerCoverage
+from swagger_coverage.src.deco import swagger
+
+# swagger data preparation
+swagger_url = "https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0"
+api_url = "https://api.swaggerhub.com/apis/"
+path='/report' # path to swagger coverage report
+swagger_rep = SwaggerCoverage(api_url=api_url, url=swagger_url, path=path)
+swagger_rep.create_coverage_data()
+
+
+# function to call a request to the server
+@swagger("regUser")
+def register_user(payload: dict):
+    return requests.post('https://stores-tests-api.herokuapp.com/register',
+                         json=payload)
+
+
+# test
+data = {"username": "test2023@test.com", "password": "Password"}
+response = register_user(data)
+assert response.status_code == 201
+
+# create report
+swagger_rep.create_report()
+
+```
+**swagger data preparation**: Prepare our file data_swagger.yaml, it will be created automatically.
+
+**function to call a request to the server**:  We will write a user registration call. Declaring a function with a decorator **@swagger("regUser")**.
+**"regUser"** taken from file **data_swagger.yaml**, this is unique id of our endpoint.
+
+**test**: run the test
+
+**create report**: create a report.
+
+
+After that, in the folder **swagger_report** we will receive a report **index.html**.
+
+Let's see it
+
+![](https://github.com/berpress/python-api-tests/blob/main/images/swagger_register.png)
+
+As you can see, we have increased the counter of verified endpoints
+
+If you use **pytest**, add this code in conftest.py
+
+```python
+@pytest.fixture(scope="session", autouse=True)
+def swagger_checker(request):
+    url = request.config.getoption("--swagger-url")
+    url_api = request.config.getoption("--api-url")
+    path = '/report'
+    swagger = SwaggerCoverage(api_url=url_api, url=url, path=path)
+    swagger.create_coverage_data()
+    yield
+    swagger.create_report()
+```
+Also, at the end of the report, you can find a table of average request times for routes
+![](https://github.com/berpress/python-api-tests/blob/main/images/requets_time.png?raw=true)
+
+
+Also, at the end of the report, you can find a table of average request times for routes
+
+More example with pytest and API tests https://github.com/berpress/python-api-tests
+
+Report example [https://github.com/berpress/python-api-tests/tree/main/swagger_report](https://github.com/berpress/python-api-tests/tree/main/report)
 
-setup(**setup_kwargs)
```

