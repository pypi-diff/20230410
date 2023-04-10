# Comparing `tmp/kafka_connect_api-0.5.4.tar.gz` & `tmp/kafka_connect_api-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_connect_api-0.5.4.tar", max compression
+gzip compressed data, was "kafka_connect_api-0.5.5.tar", max compression
```

## Comparing `kafka_connect_api-0.5.4.tar` & `kafka_connect_api-0.5.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    16725 2022-06-01 07:03:28.022199 kafka_connect_api-0.5.4/LICENSE
--rw-r--r--   0        0        0     2718 2023-01-15 22:36:04.845700 kafka_connect_api-0.5.4/README.rst
--rw-r--r--   0        0        0      141 2023-03-21 06:04:07.116934 kafka_connect_api-0.5.4/kafka_connect_api/__init__.py
--rw-r--r--   0        0        0     7429 2023-01-16 10:00:08.040132 kafka_connect_api-0.5.4/kafka_connect_api/aws_lambdas.py
--rw-r--r--   0        0        0     3176 2023-03-21 05:47:47.410436 kafka_connect_api-0.5.4/kafka_connect_api/errors.py
--rw-r--r--   0        0        0    12094 2023-03-15 14:09:15.772930 kafka_connect_api-0.5.4/kafka_connect_api/kafka_connect_api.py
--rw-r--r--   0        0        0      162 2023-01-16 10:00:46.616584 kafka_connect_api-0.5.4/kafka_connect_api/tools.py
--rw-r--r--   0        0        0     2043 2023-03-21 06:04:07.115934 kafka_connect_api-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 kafka_connect_api-0.5.4/setup.py
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 kafka_connect_api-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-06-01 07:03:28.022199 kafka_connect_api-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2718 2023-01-15 22:36:04.845700 kafka_connect_api-0.5.5/README.rst
+-rw-r--r--   0        0        0      141 2023-04-10 08:06:25.511446 kafka_connect_api-0.5.5/kafka_connect_api/__init__.py
+-rw-r--r--   0        0        0     7429 2023-01-16 10:00:08.040132 kafka_connect_api-0.5.5/kafka_connect_api/aws_lambdas.py
+-rw-r--r--   0        0        0     3176 2023-03-21 05:47:47.410436 kafka_connect_api-0.5.5/kafka_connect_api/errors.py
+-rw-r--r--   0        0        0    12094 2023-03-15 14:09:15.772930 kafka_connect_api-0.5.5/kafka_connect_api/kafka_connect_api.py
+-rw-r--r--   0        0        0      162 2023-01-16 10:00:46.616584 kafka_connect_api-0.5.5/kafka_connect_api/tools.py
+-rw-r--r--   0        0        0     2043 2023-04-10 08:06:25.511446 kafka_connect_api-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 kafka_connect_api-0.5.5/setup.py
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 kafka_connect_api-0.5.5/PKG-INFO
```

### Comparing `kafka_connect_api-0.5.4/LICENSE` & `kafka_connect_api-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.4/README.rst` & `kafka_connect_api-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.4/kafka_connect_api/aws_lambdas.py` & `kafka_connect_api-0.5.5/kafka_connect_api/aws_lambdas.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.4/kafka_connect_api/errors.py` & `kafka_connect_api-0.5.5/kafka_connect_api/errors.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.4/kafka_connect_api/kafka_connect_api.py` & `kafka_connect_api-0.5.5/kafka_connect_api/kafka_connect_api.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.4/pyproject.toml` & `kafka_connect_api-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kafka_connect_api"
-version = "0.5.4"
+version = "0.5.5"
 description = "Apache Kafka Connect client"
 authors = ["John Preston <john@compose-x.io>"]
 license = "MPL-2.0"
 readme = "README.rst"
 classifiers = [
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
@@ -48,15 +48,15 @@
 [tool.poetry.group.dev.dependencies]
 sphinx-autodoc-typehints = "^1.19.4"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/kafka_connect_api"
 
 [tool.tbump.version]
-current = "0.5.4"
+current = "0.5.5"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `kafka_connect_api-0.5.4/setup.py` & `kafka_connect_api-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['requests>=2.26.0,<3.0.0']
 
 extras_require = \
 {':extra == "awslambda"': ['jsonschema>=4.3.0,<5.0.0']}
 
 setup_kwargs = {
     'name': 'kafka-connect-api',
-    'version': '0.5.4',
+    'version': '0.5.5',
     'description': 'Apache Kafka Connect client',
     'long_description': '========================================\nApache Kafka Connect API Python client\n========================================\n\n|PYPI_VERSION| |PYPI_LICENSE|\n\n|CODE_STYLE| |TDD| |BDD|\n\n|DOCS_BUILD|\n\nDocumentation: https://kafka-connect-api.readthedocs.io.\n\n\nInstall\n========\n\n.. code-block::\n\n    pip install kafka-connect-api\n\nUsage\n======\n\n.. code-block:: python\n\n    from kafka_connect_api.kafka_connect_api import Api, Cluster\n\n    api = Api(connect.cluster, port=8083)\n    cluster = Cluster(api)\n    print(cluster.connectors)\n\n\nFeatures\n==========\n\nAllows you to interact with the Kafka Connect API (`API Reference`_) in a simple way.\n\n* Connection to cluster (supports Basic Auth)\n* List all connectors in the cluster\n* Describe the connector configuration\n* Update the connector configuration\n* Pause / Resume Connector\n* Restart all tasks for the connector\n\nSome pre-made functions can help with operational activities.\nSee `kafka_connect_api.aws_lambdas.py`\n\n.. _API Reference: https://docs.confluent.io/platform/current/connect/references/restapi.html\n\n.. |DOCS_BUILD| image:: https://readthedocs.org/projects/kafka-connect-api/badge/?version=latest\n        :target: https://kafka-connect-api.readthedocs.io/en/latest/\n        :alt: Documentation Status\n\n.. |PYPI_VERSION| image:: https://img.shields.io/pypi/v/kafka-connect-api.svg\n        :target: https://pypi.python.org/pypi/kafka_connect_api\n\n.. |PYPI_LICENSE| image:: https://img.shields.io/pypi/l/kafka-connect-api\n    :alt: PyPI - License\n    :target: https://github.com/compose-x/kafka-connect-api/blob/master/LICENSE\n\n.. |PYPI_PYVERS| image:: https://img.shields.io/pypi/pyversions/kafka-connect-api\n    :alt: PyPI - Python Version\n    :target: https://pypi.python.org/pypi/kafka-connect-api\n\n.. |PYPI_WHEEL| image:: https://img.shields.io/pypi/wheel/kafka-connect-api\n    :alt: PyPI - Wheel\n    :target: https://pypi.python.org/pypi/kafka-connect-api\n\n.. |CODE_STYLE| image:: https://img.shields.io/badge/codestyle-black-black\n    :alt: CodeStyle\n    :target: https://pypi.org/project/black/\n\n.. |TDD| image:: https://img.shields.io/badge/tdd-pytest-black\n    :alt: TDD with pytest\n    :target: https://docs.pytest.org/en/latest/contents.html\n\n.. |BDD| image:: https://img.shields.io/badge/bdd-behave-black\n    :alt: BDD with Behave\n    :target: https://behave.readthedocs.io/en/latest/\n\n.. |QUALITY| image:: https://sonarcloud.io/api/project_badges/measure?project=compose-x_kafka-connect-api&metric=alert_status\n    :alt: Code scan with SonarCloud\n    :target: https://sonarcloud.io/dashboard?id=compose-x_kafka-connect-api\n\n.. |PY_DLS| image:: https://img.shields.io/pypi/dm/kafka-connect-api\n    :target: https://pypi.org/project/kafka-connect-api/\n',
     'author': 'John Preston',
     'author_email': 'john@compose-x.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kafka_connect_api-0.5.4/PKG-INFO` & `kafka_connect_api-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-connect-api
-Version: 0.5.4
+Version: 0.5.5
 Summary: Apache Kafka Connect client
 License: MPL-2.0
 Author: John Preston
 Author-email: john@compose-x.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
```

