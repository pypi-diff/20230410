# Comparing `tmp/cookiecutter-namespace-template-0.3.0.tar.gz` & `tmp/cookiecutter_namespace_template-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter-namespace-template-0.3.0.tar", last modified: Sat Jan 21 17:11:41 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `cookiecutter-namespace-template-0.3.0.tar` & `cookiecutter_namespace_template-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,62 @@
-drwxr-xr-x   0 veit       (502) staff       (20)        0 2023-01-21 17:11:41.341343 cookiecutter-namespace-template-0.3.0/
--rw-r--r--   0 veit       (502) staff       (20)     1527 2021-10-10 13:35:20.000000 cookiecutter-namespace-template-0.3.0/LICENSE
--rw-r--r--   0 veit       (502) staff       (20)     4738 2023-01-21 17:11:41.340059 cookiecutter-namespace-template-0.3.0/PKG-INFO
--rw-r--r--   0 veit       (502) staff       (20)     3572 2023-01-20 21:38:33.000000 cookiecutter-namespace-template-0.3.0/README.rst
-drwxr-xr-x   0 veit       (502) staff       (20)        0 2023-01-21 17:11:41.337819 cookiecutter-namespace-template-0.3.0/cookiecutter_namespace_template.egg-info/
--rw-r--r--   0 veit       (502) staff       (20)     4738 2023-01-21 17:11:41.000000 cookiecutter-namespace-template-0.3.0/cookiecutter_namespace_template.egg-info/PKG-INFO
--rw-r--r--   0 veit       (502) staff       (20)      316 2023-01-21 17:11:41.000000 cookiecutter-namespace-template-0.3.0/cookiecutter_namespace_template.egg-info/SOURCES.txt
--rw-r--r--   0 veit       (502) staff       (20)        1 2023-01-21 17:11:41.000000 cookiecutter-namespace-template-0.3.0/cookiecutter_namespace_template.egg-info/dependency_links.txt
--rw-r--r--   0 veit       (502) staff       (20)       51 2023-01-21 17:11:41.000000 cookiecutter-namespace-template-0.3.0/cookiecutter_namespace_template.egg-info/requires.txt
--rw-r--r--   0 veit       (502) staff       (20)        1 2023-01-21 17:11:41.000000 cookiecutter-namespace-template-0.3.0/cookiecutter_namespace_template.egg-info/top_level.txt
--rw-r--r--   0 veit       (502) staff       (20)      362 2023-01-20 15:08:10.000000 cookiecutter-namespace-template-0.3.0/pyproject.toml
--rw-r--r--   0 veit       (502) staff       (20)       38 2023-01-21 17:11:41.341791 cookiecutter-namespace-template-0.3.0/setup.cfg
--rw-r--r--   0 veit       (502) staff       (20)     1795 2023-01-21 17:00:00.000000 cookiecutter-namespace-template-0.3.0/setup.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/.pyup.yml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/Makefile
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/cookiecutter.json
+-rw-r--r--   0        0        0    12290 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/cookiecutter_namespace_template-0.2.11.dev84-py3-none-any.whl
+-rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/cookiecutter_namespace_template-0.3.0-py3-none-any.whl
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/pytest.ini
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/tox.ini
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/.github/issue_template.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/docs/console-script-setup.rst
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/docs/index.rst
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/docs/prompts.rst
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/docs/pypi-release-checklist.rst
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/docs/readme.rst
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/docs/tutorial.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/hooks/post_gen_project.py
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/tests/test_bake_project.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/.bumpversion.cfg
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/.readthedocs.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/AUTHORS.rst
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/HISTORY.rst
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/LICENSE
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/MANIFEST.in
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/README.rst
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/requirements_dev_out.txt
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/tox.ini
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/Makefile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/authors.rst
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/contributing.rst
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/history.rst
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/index.rst
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/installation.rst
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/make.bat
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/readme.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/docs/_static/.gitkeep
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/tests/test_{{cookiecutter.namespace}}-{{cookiecutter.package_name}}.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/{{cookiecutter.namespace}}/__init__.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/{{cookiecutter.namespace}}/{{cookiecutter.package_name}}/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/{{cookiecutter.namespace}}/{{cookiecutter.package_name}}/cli.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/{{cookiecutter.project_name}}/{{cookiecutter.namespace}}/{{cookiecutter.package_name}}/main.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/README.rst
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 cookiecutter_namespace_template-0.4.0/PKG-INFO
```

### Comparing `cookiecutter-namespace-template-0.3.0/LICENSE` & `cookiecutter_namespace_template-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter-namespace-template-0.3.0/PKG-INFO` & `cookiecutter_namespace_template-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 Metadata-Version: 2.1
 Name: cookiecutter-namespace-template
-Version: 0.3.0
+Version: 0.4.0
 Summary: Cookiecutter template for a Python namespace package
-Home-page: https://github.com/veit/cookiecutter-namespace-template
-Author: Veit Schiele
-Author-email: contact@veit-schiele.de
-License: BSD
-Keywords: cookiecutter,template,package
+Project-URL: Documentation, https://cookiecutter-namespace-template.readthedocs.io/
+Project-URL: Bug Tracker, https://github.com/veit/cookiecutter-namespace-template/issues
+Project-URL: Source Code, https://github.com/veit/cookiecutter-namespace-template
+Author-email: Veit Schiele <veit@cusy.io>
+License-Expression: BSD-3-Clause
+License-File: LICENSE
+Keywords: cookiecutter,package,template
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development
-Description-Content-Type: text/x-rst
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Provides-Extra: dev
+Requires-Dist: cookiecutter-namespace-template[docs,tests]; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-cookies; extra == 'tests'
+Description-Content-Type: text/x-rst
 
 ===============================
 Cookiecutter Namespace Template
 ===============================
 
 `Cookiecutter <https://github.com/cookiecutter/cookiecutter>`_ Namespace
 Template for a Python package.
@@ -59,35 +69,47 @@
 * Testing setup with ``unittest`` or ``pytest``
 * `Tox <https://tox.readthedocs.io/>`_ testing: Setup to easily test for Python
   3.7, 3.8, 3.9, 3.10 and 3.11.
 * `Sphinx <http://www.sphinx-doc.org/>`_ docs: Documentation ready for
   generation with, for example, ReadTheDocs_
 * `bump2version <https://github.com/c4urself/bump2version>`_: Pre-configured
   version bumping with a single command
+* If the `cookiecutter-namespace-template
+  <https://github.com/veit/cookiecutter-namespace-template>`_ project template
+  has been changed, you can apply these changes with
+
+  .. code-block:: console
+
+     $ cruft update
+
 * Optional auto-release to `PyPI <https://pypi.org/>`_ when you push a new tag
   to main (optional)
-* Optional command line interface using `Click
-  <https://palletsprojects.com/p/click/>`_
+* Optional command line interface using `Typer <https://typer.tiangolo.com>`_ or
+  `Click <https://palletsprojects.com/p/click/>`_
 
 If you really want to create a new package with Python 2, in spite of the
 `Python 2.7 countdown <https://pythonclock.org/>`_ and the `Sunsetting Python 2
 support <https://python3statement.org/>`_, then use
 ``cookiecutter-namespace-template`` <0.2.
 
 Quickstart
 ----------
 
-#. Install the latest Cookiecutter if you haven’t installed it yet (this requires
-   Cookiecutter 1.4.0 or higher)::
+#. Install the latest Cookiecutter if you haven’t installed it yet (this
+   requires Cookiecutter 1.4.0 or higher):
+
+   .. code-block:: console
+
+      $ python -m pip install -U cruft
 
-    $ python -m pip install -U cookiecutter
+#. Generate a Python package project:
 
-#. Generate a Python package project::
+   .. code-block:: console
 
-    $ python -m cookiecutter https://github.com/veit/cookiecutter-namespace-template.git
+      $ python -m cruft create https://github.com/veit/cookiecutter-namespace-template.git
 
 #. Create a repo and put it there.
 
 #. `Register <https://pypi.org/account/register/>`_ your project with PyPI.
 
 #. Add the repo to your `ReadTheDocs <https://readthedocs.io/>`_ account and
    turn on the ReadTheDocs service hook.
```

### Comparing `cookiecutter-namespace-template-0.3.0/README.rst` & `cookiecutter_namespace_template-0.4.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -30,35 +30,47 @@
 * Testing setup with ``unittest`` or ``pytest``
 * `Tox <https://tox.readthedocs.io/>`_ testing: Setup to easily test for Python
   3.7, 3.8, 3.9, 3.10 and 3.11.
 * `Sphinx <http://www.sphinx-doc.org/>`_ docs: Documentation ready for
   generation with, for example, ReadTheDocs_
 * `bump2version <https://github.com/c4urself/bump2version>`_: Pre-configured
   version bumping with a single command
+* If the `cookiecutter-namespace-template
+  <https://github.com/veit/cookiecutter-namespace-template>`_ project template
+  has been changed, you can apply these changes with
+
+  .. code-block:: console
+
+     $ cruft update
+
 * Optional auto-release to `PyPI <https://pypi.org/>`_ when you push a new tag
   to main (optional)
-* Optional command line interface using `Click
-  <https://palletsprojects.com/p/click/>`_
+* Optional command line interface using `Typer <https://typer.tiangolo.com>`_ or
+  `Click <https://palletsprojects.com/p/click/>`_
 
 If you really want to create a new package with Python 2, in spite of the
 `Python 2.7 countdown <https://pythonclock.org/>`_ and the `Sunsetting Python 2
 support <https://python3statement.org/>`_, then use
 ``cookiecutter-namespace-template`` <0.2.
 
 Quickstart
 ----------
 
-#. Install the latest Cookiecutter if you haven’t installed it yet (this requires
-   Cookiecutter 1.4.0 or higher)::
+#. Install the latest Cookiecutter if you haven’t installed it yet (this
+   requires Cookiecutter 1.4.0 or higher):
+
+   .. code-block:: console
+
+      $ python -m pip install -U cruft
 
-    $ python -m pip install -U cookiecutter
+#. Generate a Python package project:
 
-#. Generate a Python package project::
+   .. code-block:: console
 
-    $ python -m cookiecutter https://github.com/veit/cookiecutter-namespace-template.git
+      $ python -m cruft create https://github.com/veit/cookiecutter-namespace-template.git
 
 #. Create a repo and put it there.
 
 #. `Register <https://pypi.org/account/register/>`_ your project with PyPI.
 
 #. Add the repo to your `ReadTheDocs <https://readthedocs.io/>`_ account and
    turn on the ReadTheDocs service hook.
```

