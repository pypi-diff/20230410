# Comparing `tmp/columbus-0.1.8.tar.gz` & `tmp/columbus-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "columbus-0.1.8.tar", max compression
+gzip compressed data, was "columbus-0.1.9.tar", max compression
```

## Comparing `columbus-0.1.8.tar` & `columbus-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3261 2023-04-10 16:14:00.375339 columbus-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-02-17 00:47:49.660143 columbus-0.1.8/columbus/__init__.py
--rw-r--r--   0        0        0        0 2023-02-17 00:32:14.678096 columbus-0.1.8/columbus/framework/__init__.py
--rw-r--r--   0        0        0      223 2023-04-10 15:58:51.572616 columbus-0.1.8/columbus/framework/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6322 2023-02-17 00:32:14.678464 columbus-0.1.8/columbus/framework/__pycache__/parse_yaml.cpython-311.pyc
--rw-r--r--   0        0        0     2799 2023-04-08 14:19:29.565716 columbus-0.1.8/columbus/framework/application.py
--rw-r--r--   0        0        0     1694 2023-04-09 16:27:49.132207 columbus-0.1.8/columbus/framework/constants.py
--rw-r--r--   0        0        0     2390 2023-04-09 16:28:33.627425 columbus-0.1.8/columbus/framework/requests.py
--rw-r--r--   0        0        0     1542 2023-04-06 20:59:46.976691 columbus-0.1.8/columbus/framework/utils.py
--rw-r--r--   0        0        0     3806 2023-04-08 14:27:28.056489 columbus-0.1.8/columbus/framework/validators.py
--rw-r--r--   0        0        0     1207 2023-04-06 20:59:27.259465 columbus-0.1.8/columbus/main.py
--rw-r--r--   0        0        0      275 2023-04-10 20:50:46.403616 columbus-0.1.8/columbus/run.py
--rw-r--r--   0        0        0      601 2023-04-08 14:46:07.165675 columbus-0.1.8/columbus/start.py
--rw-r--r--   0        0        0      727 2023-04-10 20:51:27.871947 columbus-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4488 2023-04-10 20:51:38.424947 columbus-0.1.8/setup.py
--rw-r--r--   0        0        0     4284 2023-04-10 20:51:38.425268 columbus-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3286 2023-04-10 21:44:32.911823 columbus-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-02-17 00:47:49.660143 columbus-0.1.9/columbus/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-17 00:32:14.678096 columbus-0.1.9/columbus/framework/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-10 15:58:51.572616 columbus-0.1.9/columbus/framework/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6322 2023-02-17 00:32:14.678464 columbus-0.1.9/columbus/framework/__pycache__/parse_yaml.cpython-311.pyc
+-rw-r--r--   0        0        0     2799 2023-04-08 14:19:29.565716 columbus-0.1.9/columbus/framework/application.py
+-rw-r--r--   0        0        0     1694 2023-04-09 16:27:49.132207 columbus-0.1.9/columbus/framework/constants.py
+-rw-r--r--   0        0        0     2390 2023-04-09 16:28:33.627425 columbus-0.1.9/columbus/framework/requests.py
+-rw-r--r--   0        0        0     1542 2023-04-06 20:59:46.976691 columbus-0.1.9/columbus/framework/utils.py
+-rw-r--r--   0        0        0     3806 2023-04-08 14:27:28.056489 columbus-0.1.9/columbus/framework/validators.py
+-rw-r--r--   0        0        0     1207 2023-04-06 20:59:27.259465 columbus-0.1.9/columbus/main.py
+-rw-r--r--   0        0        0      275 2023-04-10 20:50:46.403616 columbus-0.1.9/columbus/run.py
+-rw-r--r--   0        0        0      601 2023-04-08 14:46:07.165675 columbus-0.1.9/columbus/start.py
+-rw-r--r--   0        0        0      728 2023-04-10 21:47:25.131924 columbus-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4514 2023-04-10 21:47:53.339449 columbus-0.1.9/setup.py
+-rw-r--r--   0        0        0     4260 2023-04-10 21:47:53.339811 columbus-0.1.9/PKG-INFO
```

### Comparing `columbus-0.1.8/README.md` & `columbus-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 	This command will generate two files for you:
 	main.yml with a basic config template and an empty models.py.
 
 2. **In models.py define your database table using SQLAlchemy.** <br><br>
 	Then create the tables ([Alembic](https://alembic.sqlalchemy.org/en/latest/) is generally the recommended way to do this) and add some data whichever way you like. Columbus doesn't need you to connect to the database or write any queries for the app to work, it will do that for you. All you need to do is provide it with the database url.
 
-3. **In main.yml add the database url** as a value for the 'database' key. **Add the name of your table** as the value for the 'table' key. <br><br>Here is a basic working example (provided you've set up the database with this url and your table is named my_table).
+3. **In main.yml add the database url** as a value for the 'database' key. **Add the name of your table** as the value for the 'table' key. <br><br>Here is a basic working example (provided you've set up the database with this url and your table is named my_table and located in models.py).
 
 	```
 	models: models.py
 	database: postgresql://someuser:postgres@localhost/mydatabase
 	APIs:
 	  hello_world:
 	    table: my_table
```

### Comparing `columbus-0.1.8/columbus/framework/__pycache__/parse_yaml.cpython-311.pyc` & `columbus-0.1.9/columbus/framework/__pycache__/parse_yaml.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `columbus-0.1.8/columbus/framework/application.py` & `columbus-0.1.9/columbus/framework/application.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.8/columbus/framework/constants.py` & `columbus-0.1.9/columbus/framework/constants.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.8/columbus/framework/requests.py` & `columbus-0.1.9/columbus/framework/requests.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.8/columbus/framework/utils.py` & `columbus-0.1.9/columbus/framework/utils.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.8/columbus/framework/validators.py` & `columbus-0.1.9/columbus/framework/validators.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.8/columbus/main.py` & `columbus-0.1.9/columbus/main.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.8/columbus/start.py` & `columbus-0.1.9/columbus/start.py`

 * *Files identical despite different names*

### Comparing `columbus-0.1.8/pyproject.toml` & `columbus-0.1.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "columbus"
-version = "0.1.8"
+version = "0.1.9"
 description = "Generate an async web API from an SQLAlchemy table"
 authors = ["alwalk0 <walkernotwalker@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/leftfile/columbus"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 Jinja2 = "^3.1.2"
 starlette = "^0.24.0"
 uvicorn = "^0.20.0"
 pyaml = "^21.10.1"
 databases = "^0.7.0"
 psycopg2 = "^2.9.5"
 alembic = "^1.9.3"
```

### Comparing `columbus-0.1.8/setup.py` & `columbus-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,24 @@
  'watchfiles>=0.18.1,<0.19.0']
 
 entry_points = \
 {'console_scripts': ['run = columbus.run:app', 'start = columbus.start:app']}
 
 setup_kwargs = {
     'name': 'columbus',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Generate an async web API from an SQLAlchemy table',
-    'long_description': "# Columbus\n\n![PyPI](https://img.shields.io/pypi/v/columbus)\n\n\n\n### What is Columbus?\n\nColumbus is a Python web framework that automatically generates an async CRUD REST API web application from an SQLAlchemy table.\n\n### How does it work?\n\nUnder the hood Columbus uses [Starlette](https://www.starlette.io), [Databases](https://pypi.org/project/databases/) and [SQLAlchemy](https://www.sqlalchemy.org) along with some interesting metaprogramming techniques to generate a web app based solely on your YAML specification and SQLalchemy table definition. \n\n### Installation\n\n ```pip install columbus```\n\n### Quickstart\n\nYou can have your API up and running in only a couple of simple steps:\n\n1. ```start```\n\n\tThis command will generate two files for you:\n\tmain.yml with a basic config template and an empty models.py.\n\n2. **In models.py define your database table using SQLAlchemy.** <br><br>\n\tThen create the tables ([Alembic](https://alembic.sqlalchemy.org/en/latest/) is generally the recommended way to do this) and add some data whichever way you like. Columbus doesn't need you to connect to the database or write any queries for the app to work, it will do that for you. All you need to do is provide it with the database url.\n\n3. **In main.yml add the database url** as a value for the 'database' key. **Add the name of your table** as the value for the 'table' key. <br><br>Here is a basic working example (provided you've set up the database with this url and your table is named my_table).\n\n\t```\n\tmodels: models.py\n\tdatabase: postgresql://someuser:postgres@localhost/mydatabase\n\tAPIs:\n\t  hello_world:\n\t    table: my_table\n\t    methods: [GET]\n\t```    \n\t\n\n\n4. ```run```\n\n\tThis command will run your app. **Navigate to localhost:8000/my_table and see your API in action**.\n\t\n\t\n### Documentation\n\nHere is a comprehensive list of possible keys and values in the YAML config.\n\nKeys:\n\n- **models**: relative path to the file where your SQLAlchemy table is defined\n\n\n- **database**: valid database url\n\n- **APIs**: the APIs you want Columbus to generate. Each API can be named whatever you want, but it has two mandatory keys:\n\t\n\t- **table**: name of SQLAlchemy table from which you want to generate the API\n\t\n\t-  **methods**: list of http methods (GET, PUT, POST, DELETE) you want the API to support. Attention: this is the only key that needs to be a list, so put the methods in square brackets.\n\nBelow is an example of a more comprehensive animals API, which should give you a feel for the correct YAML structure Columbus understands. Incorrect structures will throw an error and the app won't run.\n\n\n```\nmodels: models.py\ndatabase: postgresql://someuser:postgres@localhost/mydatabase\nAPIs:\n  dogs:\n    table: dogs\n    methods: [GET, POST]\n  cats:\n    table: cats   \n    methods: [GET, POST, PUT, DELETE] \n  snakes:\n    table: snakes\n    methods: [GET, POST, PUT]   \n  bears:\n    table: bears\n    methods: [GET]    \n```    \n    \n    \n    \n    \n    \n    \n### What use cases does it support?\n\nColumbus is still in the early days of active development, so it only supports the most basic use case for now. Feel free to open an issue for a missing feature and it will most likely be pushed to the top of the priority list and shipped soon.\n            \n\n\n\n\n\t\n\t\n\t\n",
+    'long_description': "# Columbus\n\n![PyPI](https://img.shields.io/pypi/v/columbus)\n\n\n\n### What is Columbus?\n\nColumbus is a Python web framework that automatically generates an async CRUD REST API web application from an SQLAlchemy table.\n\n### How does it work?\n\nUnder the hood Columbus uses [Starlette](https://www.starlette.io), [Databases](https://pypi.org/project/databases/) and [SQLAlchemy](https://www.sqlalchemy.org) along with some interesting metaprogramming techniques to generate a web app based solely on your YAML specification and SQLalchemy table definition. \n\n### Installation\n\n ```pip install columbus```\n\n### Quickstart\n\nYou can have your API up and running in only a couple of simple steps:\n\n1. ```start```\n\n\tThis command will generate two files for you:\n\tmain.yml with a basic config template and an empty models.py.\n\n2. **In models.py define your database table using SQLAlchemy.** <br><br>\n\tThen create the tables ([Alembic](https://alembic.sqlalchemy.org/en/latest/) is generally the recommended way to do this) and add some data whichever way you like. Columbus doesn't need you to connect to the database or write any queries for the app to work, it will do that for you. All you need to do is provide it with the database url.\n\n3. **In main.yml add the database url** as a value for the 'database' key. **Add the name of your table** as the value for the 'table' key. <br><br>Here is a basic working example (provided you've set up the database with this url and your table is named my_table and located in models.py).\n\n\t```\n\tmodels: models.py\n\tdatabase: postgresql://someuser:postgres@localhost/mydatabase\n\tAPIs:\n\t  hello_world:\n\t    table: my_table\n\t    methods: [GET]\n\t```    \n\t\n\n\n4. ```run```\n\n\tThis command will run your app. **Navigate to localhost:8000/my_table and see your API in action**.\n\t\n\t\n### Documentation\n\nHere is a comprehensive list of possible keys and values in the YAML config.\n\nKeys:\n\n- **models**: relative path to the file where your SQLAlchemy table is defined\n\n\n- **database**: valid database url\n\n- **APIs**: the APIs you want Columbus to generate. Each API can be named whatever you want, but it has two mandatory keys:\n\t\n\t- **table**: name of SQLAlchemy table from which you want to generate the API\n\t\n\t-  **methods**: list of http methods (GET, PUT, POST, DELETE) you want the API to support. Attention: this is the only key that needs to be a list, so put the methods in square brackets.\n\nBelow is an example of a more comprehensive animals API, which should give you a feel for the correct YAML structure Columbus understands. Incorrect structures will throw an error and the app won't run.\n\n\n```\nmodels: models.py\ndatabase: postgresql://someuser:postgres@localhost/mydatabase\nAPIs:\n  dogs:\n    table: dogs\n    methods: [GET, POST]\n  cats:\n    table: cats   \n    methods: [GET, POST, PUT, DELETE] \n  snakes:\n    table: snakes\n    methods: [GET, POST, PUT]   \n  bears:\n    table: bears\n    methods: [GET]    \n```    \n    \n    \n    \n    \n    \n    \n### What use cases does it support?\n\nColumbus is still in the early days of active development, so it only supports the most basic use case for now. Feel free to open an issue for a missing feature and it will most likely be pushed to the top of the priority list and shipped soon.\n            \n\n\n\n\n\t\n\t\n\t\n",
     'author': 'alwalk0',
     'author_email': 'walkernotwalker@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/leftfile/columbus',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `columbus-0.1.8/PKG-INFO` & `columbus-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: columbus
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate an async web API from an SQLAlchemy table
 Home-page: https://github.com/leftfile/columbus
 License: MIT
 Author: alwalk0
 Author-email: walkernotwalker@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: alembic (>=1.9.3,<2.0.0)
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
 Requires-Dist: databases (>=0.7.0,<0.8.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: pyaml (>=21.10.1,<22.0.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
@@ -51,15 +50,15 @@
 
 	This command will generate two files for you:
 	main.yml with a basic config template and an empty models.py.
 
 2. **In models.py define your database table using SQLAlchemy.** <br><br>
 	Then create the tables ([Alembic](https://alembic.sqlalchemy.org/en/latest/) is generally the recommended way to do this) and add some data whichever way you like. Columbus doesn't need you to connect to the database or write any queries for the app to work, it will do that for you. All you need to do is provide it with the database url.
 
-3. **In main.yml add the database url** as a value for the 'database' key. **Add the name of your table** as the value for the 'table' key. <br><br>Here is a basic working example (provided you've set up the database with this url and your table is named my_table).
+3. **In main.yml add the database url** as a value for the 'database' key. **Add the name of your table** as the value for the 'table' key. <br><br>Here is a basic working example (provided you've set up the database with this url and your table is named my_table and located in models.py).
 
 	```
 	models: models.py
 	database: postgresql://someuser:postgres@localhost/mydatabase
 	APIs:
 	  hello_world:
 	    table: my_table
```

