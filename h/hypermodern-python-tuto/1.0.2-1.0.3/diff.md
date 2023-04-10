# Comparing `tmp/hypermodern_python_tuto-1.0.2.tar.gz` & `tmp/hypermodern_python_tuto-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypermodern_python_tuto-1.0.2.tar", max compression
+gzip compressed data, was "hypermodern_python_tuto-1.0.3.tar", max compression
```

## Comparing `hypermodern_python_tuto-1.0.2.tar` & `hypermodern_python_tuto-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-03-16 13:18:04.138127 hypermodern_python_tuto-1.0.2/LICENSE
--rw-r--r--   0        0        0     7763 2023-03-16 13:18:04.138127 hypermodern_python_tuto-1.0.2/README.md
--rw-r--r--   0        0        0     1874 2023-03-16 13:18:04.142127 hypermodern_python_tuto-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      222 2023-03-16 13:18:04.142127 hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/__init__.py
--rw-r--r--   0        0        0     1234 2023-03-16 13:18:04.142127 hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/__main__.py
--rw-r--r--   0        0        0      708 2023-03-16 13:18:04.142127 hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/ui.py
--rw-r--r--   0        0        0      330 2023-03-16 13:18:04.142127 hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/wikipedia/article.py
--rw-r--r--   0        0        0      918 2023-03-16 13:18:04.142127 hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/wikipedia/article_schema.py
--rw-r--r--   0        0        0     2374 2023-03-16 13:18:04.142127 hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/wikipedia/language.py
--rw-r--r--   0        0        0     1948 2023-03-16 13:18:04.142127 hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/wikipedia/requester.py
--rw-r--r--   0        0        0     9091 1970-01-01 00:00:00.000000 hypermodern_python_tuto-1.0.2/setup.py
--rw-r--r--   0        0        0     8699 1970-01-01 00:00:00.000000 hypermodern_python_tuto-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/LICENSE
+-rw-r--r--   0        0        0     7758 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/README.md
+-rw-r--r--   0        0        0     1661 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/__init__.py
+-rw-r--r--   0        0        0     1234 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/__main__.py
+-rw-r--r--   0        0        0      708 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/ui.py
+-rw-r--r--   0        0        0      330 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/article.py
+-rw-r--r--   0        0        0      918 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/article_schema.py
+-rw-r--r--   0        0        0     2374 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/language.py
+-rw-r--r--   0        0        0     1962 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/requester.py
+-rw-r--r--   0        0        0     9085 1970-01-01 00:00:00.000000 hypermodern_python_tuto-1.0.3/setup.py
+-rw-r--r--   0        0        0     8694 1970-01-01 00:00:00.000000 hypermodern_python_tuto-1.0.3/PKG-INFO
```

### Comparing `hypermodern_python_tuto-1.0.2/LICENSE` & `hypermodern_python_tuto-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hypermodern_python_tuto-1.0.2/README.md` & `hypermodern_python_tuto-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # hypermodern-python-tuto
 
 Repo to follow the Claudio Jolowicz's [tutorial about Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/).
+It follows it until [this release](https://github.com/le-chartreux/hypermodern-python-tuto/releases/tag/v1.0.3). After this one, I started adding further tools, deleting some that I consider useless and replacing some others.
 
 ---
 
 <table>
     <tr>
         <td>
             <b>Package</b>
@@ -127,40 +128,40 @@
 - [pyenv](https://github.com/pyenv/pyenv), to manage Python versions
 
 #### Test
 
 - [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests
 - [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite)
 - [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way
-- [xdoctest](https://pypi.org/project/xdoctest/), to execute the doctests (tests in documentation strings)
 
 #### Linting
 
 - [flake8](https://flake8.pycqa.org/en/latest/), a linter aggregator
-- [flake8-import-order](https://github.com/PyCQA/flake8-import-order), to verify that imports are grouped and ordered in a consistent way
+- [flake8-isort](https://pypi.org/project/flake8-isort/), to verify that imports are grouped and ordered in a consistent way
 - [flake8-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design problems
 - [flake8-annotations](https://pypi.org/project/flake8-annotations/), to detect the absence of type annotations
 - [flake8-black](https://pypi.org/project/flake8-black/), to check if the code follows [black](https://black.readthedocs.io/en/stable/) formatting
 - [flake8-docstrings](https://pypi.org/project/flake8-docstrings/), to check that the code is correctly documented
+- [flake8-pytest-style](https://pypi.org/project/flake8-pytest-style/), to check style issues with pytest-based tests
 - [darglint](https://pypi.org/project/darglint/), to check that docstrings match function definitions
 
 #### Security
 
 - [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/))
 - [Safety](https://pyup.io/safety/), to check if some packages are insecure
 
 #### Formatting
 
 - [black](https://black.readthedocs.io/en/stable/), to format the code
+- [isort](https://pycqa.github.io/isort/index.html), to sort imports
 
 #### Type checking
 
 - [mypy](https://mypy-lang.org/), the classic type checker
-- [pytype](https://google.github.io/pytype/), a static type checker
-- [typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type check
+- [typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type checker
 
 #### Documentation
 
 - [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation.
 - [Read the Docs](https://readthedocs.org/), to host the documentation.
 - [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.
 - [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.
@@ -177,10 +178,9 @@
 #### Communication
 
 - [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests
 
 #### Data validation
 
 - [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data
-- ~~[dessert](https://desert.readthedocs.io/en/stable/), to generate marshmallow serialization schemas~~ → not used because too limited (can't work with data where fields names are different from the ones of the target dataclass)
 
 I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but  [pydantic](https://docs.pydantic.dev/) is more known, and I find it easier to use.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,10 +1,13 @@
 # hypermodern-python-tuto Repo to follow the Claudio Jolowicz's [tutorial about
 Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-
-setup/). ---
+setup/). It follows it until [this release](https://github.com/le-chartreux/
+hypermodern-python-tuto/releases/tag/v1.0.3). After this one, I started adding
+further tools, deleting some that I consider useless and replacing some others.
+---
 Package [Supported_Python_Versions] [PyPI_version] [PyPI_downloads]
 CI      [Tests_status] [Documentation_status] [Coverage_status]
 Code    [Code_quality] [pre-commit]
 --- ## Table of contents - [Overview](#overview) - [Install](#install) - [Use]
 (#use) - [Tools used](#tools-used) - [Generic tools](#generic-tools) - [Generic
 Python tools](#generic-python-tools) - [Multi-purpose](#multi-purpose) -
 [Setup](#setup) - [Test](#test) - [Linting](#linting) - [Security](#security) -
@@ -34,46 +37,44 @@
 Setup - [pyenv](https://github.com/pyenv/pyenv), to manage Python versions ####
 Test - [pytest](https://docs.pytest.org/en/latest/), a framework to write unit
 tests. Also used to run doctests - [pytest-cov](https://pytest-
 cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which
 the source code of a program is executed while running its test suite) -
 [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the
 [unittest](https://docs.python.org/3/library/unittest.html) mocking in the
-pytest way - [xdoctest](https://pypi.org/project/xdoctest/), to execute the
-doctests (tests in documentation strings) #### Linting - [flake8](https://
-flake8.pycqa.org/en/latest/), a linter aggregator - [flake8-import-order]
-(https://github.com/PyCQA/flake8-import-order), to verify that imports are
-grouped and ordered in a consistent way - [flake8-bugbear](https://github.com/
-PyCQA/flake8-bugbear), to find bugs and design problems - [flake8-annotations]
-(https://pypi.org/project/flake8-annotations/), to detect the absence of type
-annotations - [flake8-black](https://pypi.org/project/flake8-black/), to check
-if the code follows [black](https://black.readthedocs.io/en/stable/) formatting
-- [flake8-docstrings](https://pypi.org/project/flake8-docstrings/), to check
-that the code is correctly documented - [darglint](https://pypi.org/project/
-darglint/), to check that docstrings match function definitions #### Security -
-[Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues
-(used inside linting with [flake8-bandit](https://pypi.org/project/flake8-
-bandit/)) - [Safety](https://pyup.io/safety/), to check if some packages are
-insecure #### Formatting - [black](https://black.readthedocs.io/en/stable/), to
-format the code #### Type checking - [mypy](https://mypy-lang.org/), the
-classic type checker - [pytype](https://google.github.io/pytype/), a static
-type checker - [typeguard](https://typeguard.readthedocs.io/en/latest/), a
-runtime type check #### Documentation - [Sphinx](https://www.sphinx-doc.org/en/
-master/), the documentation tool used by the official Python documentation. -
-[Read the Docs](https://readthedocs.org/), to host the documentation. -
-[autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html),
-Sphinx official plugin to generate API documentation from the docstrings. -
-[napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/
-napoleon.html), Sphinx official plugin to allow compatibility with Google-style
-docstrings. - [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-
-autodoc-typehints/), Sphinx plugin to detect type hints in generated
-documentation. ### Specific Python tools Tools to match specific needs of the
-projet. #### UI - [click](https://click.palletsprojects.com/en/8.1.x/), to
-create CLI applications #### Communication - [requests](https://
-requests.readthedocs.io/en/latest/), to make HTTP requests #### Data validation
-- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize,
-deserialize and validate data - ~~[dessert](https://desert.readthedocs.io/en/
-stable/), to generate marshmallow serialization schemas~~ â not used because
-too limited (can't work with data where fields names are different from the
-ones of the target dataclass) I used [marshmallow](https://
-marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but [pydantic]
-(https://docs.pydantic.dev/) is more known, and I find it easier to use.
+pytest way #### Linting - [flake8](https://flake8.pycqa.org/en/latest/), a
+linter aggregator - [flake8-isort](https://pypi.org/project/flake8-isort/), to
+verify that imports are grouped and ordered in a consistent way - [flake8-
+bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design
+problems - [flake8-annotations](https://pypi.org/project/flake8-annotations/),
+to detect the absence of type annotations - [flake8-black](https://pypi.org/
+project/flake8-black/), to check if the code follows [black](https://
+black.readthedocs.io/en/stable/) formatting - [flake8-docstrings](https://
+pypi.org/project/flake8-docstrings/), to check that the code is correctly
+documented - [flake8-pytest-style](https://pypi.org/project/flake8-pytest-
+style/), to check style issues with pytest-based tests - [darglint](https://
+pypi.org/project/darglint/), to check that docstrings match function
+definitions #### Security - [Bandit](https://bandit.readthedocs.io/en/latest/),
+to find security issues (used inside linting with [flake8-bandit](https://
+pypi.org/project/flake8-bandit/)) - [Safety](https://pyup.io/safety/), to check
+if some packages are insecure #### Formatting - [black](https://
+black.readthedocs.io/en/stable/), to format the code - [isort](https://
+pycqa.github.io/isort/index.html), to sort imports #### Type checking - [mypy]
+(https://mypy-lang.org/), the classic type checker - [typeguard](https://
+typeguard.readthedocs.io/en/latest/), a runtime type checker #### Documentation
+- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used
+by the official Python documentation. - [Read the Docs](https://
+readthedocs.org/), to host the documentation. - [autodoc](https://www.sphinx-
+doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to
+generate API documentation from the docstrings. - [napoleon](https://
+www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official
+plugin to allow compatibility with Google-style docstrings. - [sphinx-autodoc-
+typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin
+to detect type hints in generated documentation. ### Specific Python tools
+Tools to match specific needs of the projet. #### UI - [click](https://
+click.palletsprojects.com/en/8.1.x/), to create CLI applications ####
+Communication - [requests](https://requests.readthedocs.io/en/latest/), to make
+HTTP requests #### Data validation - [marshmallow](https://
+marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate
+data I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to
+follow the tutorial, but [pydantic](https://docs.pydantic.dev/) is more known,
+and I find it easier to use.
```

### Comparing `hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/__main__.py` & `hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/__main__.py`

 * *Files identical despite different names*

### Comparing `hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/ui.py` & `hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/ui.py`

 * *Files identical despite different names*

### Comparing `hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/wikipedia/article_schema.py` & `hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/article_schema.py`

 * *Files identical despite different names*

### Comparing `hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/wikipedia/language.py` & `hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/language.py`

 * *Files identical despite different names*

### Comparing `hypermodern_python_tuto-1.0.2/src/hypermodern_python_tuto/wikipedia/requester.py` & `hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """WikipediaRequester class declaration."""
-from typing import Any
+from typing import Any, Final
 
 import requests
 
 from hypermodern_python_tuto.wikipedia.article import WikipediaArticle
 from hypermodern_python_tuto.wikipedia.article_schema import WikipediaArticleSchema
 from hypermodern_python_tuto.wikipedia.language import Language
 
 
 class WikipediaRequester:
     """Class to get information from Wikipedia."""
 
     def __init__(self) -> None:
         """Set up the WikipediaRequester."""
-        self.__base_url = (
+        self.__base_url: Final = (
             "https://{language}.wikipedia.org/api/rest_v1/page/random/summary"
         )
         self.__language = "en"
 
     def get_random_article(self) -> WikipediaArticle:
         """Query a random article from Wikipedia.
```

### Comparing `hypermodern_python_tuto-1.0.2/setup.py` & `hypermodern_python_tuto-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'console_scripts': ['hypermodern-python-tuto = '
                      'hypermodern_python_tuto.__main__:main']}
 
 setup_kwargs = {
     'name': 'hypermodern-python-tuto',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': "Repo to follow the Claudio Jolowicz's tutorial about Hypermodern Python (https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)",
-    'long_description': '# hypermodern-python-tuto\n\nRepo to follow the Claudio Jolowicz\'s [tutorial about Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/).\n\n---\n\n<table>\n    <tr>\n        <td>\n            <b>Package</b>\n        </td>\n        <td>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/pyversions/hypermodern-python-tuto.svg" alt="Supported Python Versions">\n            </a>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/v/hypermodern-python-tuto.svg" alt="PyPI version">\n            </a>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/dm/hypermodern-python-tuto.svg" alt="PyPI downloads">\n            </a>\n        </td>\n    </tr>\n    <tr>\n        <td>\n            <b>CI</b>\n        </td>\n        <td>\n            <a href="https://github.com/le-chartreux/hypermodern-python-tuto/actions?workflow=Tests">\n                <img src="https://github.com/le-chartreux/hypermodern-python-tuto/workflows/Tests/badge.svg" alt="Tests status">\n            </a>\n            <a href="https://hypermodern-python-tuto.readthedocs.io/">\n                <img src="https://readthedocs.org/projects/hypermodern-python-tuto/badge/" alt="Documentation status">\n            </a>\n            <a href="https://codecov.io/gh/le-chartreux/hypermodern-python-tuto">\n                <img src="https://codecov.io/gh/le-chartreux/hypermodern-python-tuto/branch/master/graph/badge.svg" alt="Coverage status">\n            </a>\n        </td>\n    </tr>\n    <tr>\n        <td>\n            <b>Code</b>\n        </td>\n        <td>\n            <a href="https://github.com/psf/black">\n                <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code quality">\n            </a>\n            <a href="https://github.com/pre-commit/pre-commit">\n                <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen" alt="pre-commit">\n            </a>\n        </td>\n    </tr>\n</table>\n\n---\n\n## Table of contents\n\n- [Overview](#overview)\n- [Install](#install)\n- [Use](#use)\n- [Tools used](#tools-used)\n  - [Generic tools](#generic-tools)\n  - [Generic Python tools](#generic-python-tools)\n    - [Multi-purpose](#multi-purpose)\n    - [Setup](#setup)\n    - [Test](#test)\n    - [Linting](#linting)\n    - [Security](#security)\n    - [Formatting](#formatting)\n    - [Type checking](#type-checking)\n    - [Documentation](#documentation)\n  - [Specific Python tools](#specific-python-tools)\n    - [UI](#ui)\n    - [Communication](#communication)\n    - [Data validation](#data-validation)\n\n## Overview\n\nThe app created is a CLI application that queries a random Wikipedia page and displays its title and summary.\n\n## Install\n\n```shell\npip install hypermodern-python-tuto\n```\n\n## Use\n\n### Basic usage\n\nJust run the following command:\n\n```shell\nhypermodern-python-tuto\n```\n\n### Other options\n\nLook at the [documentation](https://hypermodern-python-tuto.readthedocs.io/).\n\n## Tools used\n\n### Generic tools\n\nTools that can be used in every development project, no matter if it\'s a Python project or not.\n\n- [git](https://git-scm.com/), to manage versions of the source code\n- [GitHub](https://github.com/le-chartreux/hypermodern-python-tuto), to host the git repository and automate tasks with [GitHub Actions](https://docs.github.com/en/actions):\n  - [Release Drafter](https://github.com/marketplace/actions/release-drafter), to create release templates\n- [pre-commit](https://pre-commit.com/), to manage pre-commit hooks\n- [Codecov](https://about.codecov.io/), to mesure code coverage on repos\n\n### Generic Python tools\n\nTools that can be used in every Python project, no matter its content.\n\n#### Multi-purpose\n\n- [PyPI](https://pypi.org/), to install and publish Python packages\n- [TestPyPI](https://pypi.org/), PyPI but for testing purposes\n- [poetry](https://python-poetry.org/), to make development and distribution easy (packaging, virtualization, dependencies, launching and publishing)\n- [nox](https://nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like tests, linting, reformatting, etc.)\n\n#### Setup\n\n- [pyenv](https://github.com/pyenv/pyenv), to manage Python versions\n\n#### Test\n\n- [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests\n- [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite)\n- [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way\n- [xdoctest](https://pypi.org/project/xdoctest/), to execute the doctests (tests in documentation strings)\n\n#### Linting\n\n- [flake8](https://flake8.pycqa.org/en/latest/), a linter aggregator\n- [flake8-import-order](https://github.com/PyCQA/flake8-import-order), to verify that imports are grouped and ordered in a consistent way\n- [flake8-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design problems\n- [flake8-annotations](https://pypi.org/project/flake8-annotations/), to detect the absence of type annotations\n- [flake8-black](https://pypi.org/project/flake8-black/), to check if the code follows [black](https://black.readthedocs.io/en/stable/) formatting\n- [flake8-docstrings](https://pypi.org/project/flake8-docstrings/), to check that the code is correctly documented\n- [darglint](https://pypi.org/project/darglint/), to check that docstrings match function definitions\n\n#### Security\n\n- [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/))\n- [Safety](https://pyup.io/safety/), to check if some packages are insecure\n\n#### Formatting\n\n- [black](https://black.readthedocs.io/en/stable/), to format the code\n\n#### Type checking\n\n- [mypy](https://mypy-lang.org/), the classic type checker\n- [pytype](https://google.github.io/pytype/), a static type checker\n- [typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type check\n\n#### Documentation\n\n- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation.\n- [Read the Docs](https://readthedocs.org/), to host the documentation.\n- [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.\n- [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.\n- [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin to detect type hints in generated documentation.\n\n### Specific Python tools\n\nTools to match specific needs of the projet.\n\n#### UI\n\n- [click](https://click.palletsprojects.com/en/8.1.x/), to create CLI applications\n\n#### Communication\n\n- [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests\n\n#### Data validation\n\n- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data\n- ~~[dessert](https://desert.readthedocs.io/en/stable/), to generate marshmallow serialization schemas~~ → not used because too limited (can\'t work with data where fields names are different from the ones of the target dataclass)\n\nI used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but  [pydantic](https://docs.pydantic.dev/) is more known, and I find it easier to use.\n',
+    'long_description': '# hypermodern-python-tuto\n\nRepo to follow the Claudio Jolowicz\'s [tutorial about Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/).\nIt follows it until [this release](https://github.com/le-chartreux/hypermodern-python-tuto/releases/tag/v1.0.3). After this one, I started adding further tools, deleting some that I consider useless and replacing some others.\n\n---\n\n<table>\n    <tr>\n        <td>\n            <b>Package</b>\n        </td>\n        <td>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/pyversions/hypermodern-python-tuto.svg" alt="Supported Python Versions">\n            </a>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/v/hypermodern-python-tuto.svg" alt="PyPI version">\n            </a>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/dm/hypermodern-python-tuto.svg" alt="PyPI downloads">\n            </a>\n        </td>\n    </tr>\n    <tr>\n        <td>\n            <b>CI</b>\n        </td>\n        <td>\n            <a href="https://github.com/le-chartreux/hypermodern-python-tuto/actions?workflow=Tests">\n                <img src="https://github.com/le-chartreux/hypermodern-python-tuto/workflows/Tests/badge.svg" alt="Tests status">\n            </a>\n            <a href="https://hypermodern-python-tuto.readthedocs.io/">\n                <img src="https://readthedocs.org/projects/hypermodern-python-tuto/badge/" alt="Documentation status">\n            </a>\n            <a href="https://codecov.io/gh/le-chartreux/hypermodern-python-tuto">\n                <img src="https://codecov.io/gh/le-chartreux/hypermodern-python-tuto/branch/master/graph/badge.svg" alt="Coverage status">\n            </a>\n        </td>\n    </tr>\n    <tr>\n        <td>\n            <b>Code</b>\n        </td>\n        <td>\n            <a href="https://github.com/psf/black">\n                <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code quality">\n            </a>\n            <a href="https://github.com/pre-commit/pre-commit">\n                <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen" alt="pre-commit">\n            </a>\n        </td>\n    </tr>\n</table>\n\n---\n\n## Table of contents\n\n- [Overview](#overview)\n- [Install](#install)\n- [Use](#use)\n- [Tools used](#tools-used)\n  - [Generic tools](#generic-tools)\n  - [Generic Python tools](#generic-python-tools)\n    - [Multi-purpose](#multi-purpose)\n    - [Setup](#setup)\n    - [Test](#test)\n    - [Linting](#linting)\n    - [Security](#security)\n    - [Formatting](#formatting)\n    - [Type checking](#type-checking)\n    - [Documentation](#documentation)\n  - [Specific Python tools](#specific-python-tools)\n    - [UI](#ui)\n    - [Communication](#communication)\n    - [Data validation](#data-validation)\n\n## Overview\n\nThe app created is a CLI application that queries a random Wikipedia page and displays its title and summary.\n\n## Install\n\n```shell\npip install hypermodern-python-tuto\n```\n\n## Use\n\n### Basic usage\n\nJust run the following command:\n\n```shell\nhypermodern-python-tuto\n```\n\n### Other options\n\nLook at the [documentation](https://hypermodern-python-tuto.readthedocs.io/).\n\n## Tools used\n\n### Generic tools\n\nTools that can be used in every development project, no matter if it\'s a Python project or not.\n\n- [git](https://git-scm.com/), to manage versions of the source code\n- [GitHub](https://github.com/le-chartreux/hypermodern-python-tuto), to host the git repository and automate tasks with [GitHub Actions](https://docs.github.com/en/actions):\n  - [Release Drafter](https://github.com/marketplace/actions/release-drafter), to create release templates\n- [pre-commit](https://pre-commit.com/), to manage pre-commit hooks\n- [Codecov](https://about.codecov.io/), to mesure code coverage on repos\n\n### Generic Python tools\n\nTools that can be used in every Python project, no matter its content.\n\n#### Multi-purpose\n\n- [PyPI](https://pypi.org/), to install and publish Python packages\n- [TestPyPI](https://pypi.org/), PyPI but for testing purposes\n- [poetry](https://python-poetry.org/), to make development and distribution easy (packaging, virtualization, dependencies, launching and publishing)\n- [nox](https://nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like tests, linting, reformatting, etc.)\n\n#### Setup\n\n- [pyenv](https://github.com/pyenv/pyenv), to manage Python versions\n\n#### Test\n\n- [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests\n- [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite)\n- [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way\n\n#### Linting\n\n- [flake8](https://flake8.pycqa.org/en/latest/), a linter aggregator\n- [flake8-isort](https://pypi.org/project/flake8-isort/), to verify that imports are grouped and ordered in a consistent way\n- [flake8-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design problems\n- [flake8-annotations](https://pypi.org/project/flake8-annotations/), to detect the absence of type annotations\n- [flake8-black](https://pypi.org/project/flake8-black/), to check if the code follows [black](https://black.readthedocs.io/en/stable/) formatting\n- [flake8-docstrings](https://pypi.org/project/flake8-docstrings/), to check that the code is correctly documented\n- [flake8-pytest-style](https://pypi.org/project/flake8-pytest-style/), to check style issues with pytest-based tests\n- [darglint](https://pypi.org/project/darglint/), to check that docstrings match function definitions\n\n#### Security\n\n- [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/))\n- [Safety](https://pyup.io/safety/), to check if some packages are insecure\n\n#### Formatting\n\n- [black](https://black.readthedocs.io/en/stable/), to format the code\n- [isort](https://pycqa.github.io/isort/index.html), to sort imports\n\n#### Type checking\n\n- [mypy](https://mypy-lang.org/), the classic type checker\n- [typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type checker\n\n#### Documentation\n\n- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation.\n- [Read the Docs](https://readthedocs.org/), to host the documentation.\n- [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.\n- [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.\n- [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin to detect type hints in generated documentation.\n\n### Specific Python tools\n\nTools to match specific needs of the projet.\n\n#### UI\n\n- [click](https://click.palletsprojects.com/en/8.1.x/), to create CLI applications\n\n#### Communication\n\n- [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests\n\n#### Data validation\n\n- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data\n\nI used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but  [pydantic](https://docs.pydantic.dev/) is more known, and I find it easier to use.\n',
     'author': 'le-chartreux',
     'author_email': 'le-chartreux-vert@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/le-chartreux/hypermodern-python-tuto',
     'package_dir': package_dir,
     'packages': packages,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['hypermodern_python_tuto',
 'hypermodern_python_tuto.wikipedia'] package_data = \ {'': ['*']}
 install_requires = \ ['click>=8.1.3,<9.0.0', 'marshmallow>=3.19.0,<4.0.0',
 'requests>=2.28.2,<3.0.0'] entry_points = \ {'console_scripts': ['hypermodern-
 python-tuto = ' 'hypermodern_python_tuto.__main__:main']} setup_kwargs =
-{ 'name': 'hypermodern-python-tuto', 'version': '1.0.2', 'description': "Repo
+{ 'name': 'hypermodern-python-tuto', 'version': '1.0.3', 'description': "Repo
 to follow the Claudio Jolowicz's tutorial about Hypermodern Python (https://
 cjolowicz.github.io/posts/hypermodern-python-01-setup/)", 'long_description':
 '# hypermodern-python-tuto\n\nRepo to follow the Claudio Jolowicz\'s [tutorial
 about Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-
-01-setup/).\n\n---\n\n
+01-setup/).\nIt follows it until [this release](https://github.com/le-
+chartreux/hypermodern-python-tuto/releases/tag/v1.0.3). After this one, I
+started adding further tools, deleting some that I consider useless and
+replacing some others.\n\n---\n\n
 \n Package\n \n \n_[Supported_Python_Versions]\n\n \n_[PyPI_version]\n\n \n_
              [PyPI_downloads]\n\n
 \n CI\n      \n \n_[Tests_status]\n\n \n_[Documentation_status]\n\n \n_
              [Coverage_status]\n\n
 \n Code\n    \n \n_[Code_quality]\n\n \n_[pre-commit]\n\n
 \n\n---\n\n## Table of contents\n\n- [Overview](#overview)\n- [Install]
 (#install)\n- [Use](#use)\n- [Tools used](#tools-used)\n - [Generic tools]
@@ -47,53 +50,50 @@
 Setup\n\n- [pyenv](https://github.com/pyenv/pyenv), to manage Python
 versions\n\n#### Test\n\n- [pytest](https://docs.pytest.org/en/latest/), a
 framework to write unit tests. Also used to run doctests\n- [pytest-cov](https:
 //pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to
 which the source code of a program is executed while running its test suite)\n-
 [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the
 [unittest](https://docs.python.org/3/library/unittest.html) mocking in the
-pytest way\n- [xdoctest](https://pypi.org/project/xdoctest/), to execute the
-doctests (tests in documentation strings)\n\n#### Linting\n\n- [flake8](https:/
-/flake8.pycqa.org/en/latest/), a linter aggregator\n- [flake8-import-order]
-(https://github.com/PyCQA/flake8-import-order), to verify that imports are
-grouped and ordered in a consistent way\n- [flake8-bugbear](https://github.com/
-PyCQA/flake8-bugbear), to find bugs and design problems\n- [flake8-annotations]
-(https://pypi.org/project/flake8-annotations/), to detect the absence of type
-annotations\n- [flake8-black](https://pypi.org/project/flake8-black/), to check
-if the code follows [black](https://black.readthedocs.io/en/stable/
-) formatting\n- [flake8-docstrings](https://pypi.org/project/flake8-docstrings/
-), to check that the code is correctly documented\n- [darglint](https://
+pytest way\n\n#### Linting\n\n- [flake8](https://flake8.pycqa.org/en/latest/),
+a linter aggregator\n- [flake8-isort](https://pypi.org/project/flake8-isort/),
+to verify that imports are grouped and ordered in a consistent way\n- [flake8-
+bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design
+problems\n- [flake8-annotations](https://pypi.org/project/flake8-annotations/),
+to detect the absence of type annotations\n- [flake8-black](https://pypi.org/
+project/flake8-black/), to check if the code follows [black](https://
+black.readthedocs.io/en/stable/) formatting\n- [flake8-docstrings](https://
+pypi.org/project/flake8-docstrings/), to check that the code is correctly
+documented\n- [flake8-pytest-style](https://pypi.org/project/flake8-pytest-
+style/), to check style issues with pytest-based tests\n- [darglint](https://
 pypi.org/project/darglint/), to check that docstrings match function
 definitions\n\n#### Security\n\n- [Bandit](https://bandit.readthedocs.io/en/
 latest/), to find security issues (used inside linting with [flake8-bandit]
 (https://pypi.org/project/flake8-bandit/))\n- [Safety](https://pyup.io/safety/
 ), to check if some packages are insecure\n\n#### Formatting\n\n- [black]
-(https://black.readthedocs.io/en/stable/), to format the code\n\n#### Type
-checking\n\n- [mypy](https://mypy-lang.org/), the classic type checker\n-
-[pytype](https://google.github.io/pytype/), a static type checker\n-
-[typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type
-check\n\n#### Documentation\n\n- [Sphinx](https://www.sphinx-doc.org/en/master/
-), the documentation tool used by the official Python documentation.\n- [Read
-the Docs](https://readthedocs.org/), to host the documentation.\n- [autodoc]
-(https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx
-official plugin to generate API documentation from the docstrings.\n-
-[napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/
-napoleon.html), Sphinx official plugin to allow compatibility with Google-style
-docstrings.\n- [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-
-autodoc-typehints/), Sphinx plugin to detect type hints in generated
-documentation.\n\n### Specific Python tools\n\nTools to match specific needs of
-the projet.\n\n#### UI\n\n- [click](https://click.palletsprojects.com/en/8.1.x/
-), to create CLI applications\n\n#### Communication\n\n- [requests](https://
+(https://black.readthedocs.io/en/stable/), to format the code\n- [isort](https:
+//pycqa.github.io/isort/index.html), to sort imports\n\n#### Type checking\n\n-
+[mypy](https://mypy-lang.org/), the classic type checker\n- [typeguard](https:/
+/typeguard.readthedocs.io/en/latest/), a runtime type checker\n\n####
+Documentation\n\n- [Sphinx](https://www.sphinx-doc.org/en/master/), the
+documentation tool used by the official Python documentation.\n- [Read the
+Docs](https://readthedocs.org/), to host the documentation.\n- [autodoc](https:
+//www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official
+plugin to generate API documentation from the docstrings.\n- [napoleon](https:/
+/www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official
+plugin to allow compatibility with Google-style docstrings.\n- [sphinx-autodoc-
+typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin
+to detect type hints in generated documentation.\n\n### Specific Python
+tools\n\nTools to match specific needs of the projet.\n\n#### UI\n\n- [click]
+(https://click.palletsprojects.com/en/8.1.x/), to create CLI
+applications\n\n#### Communication\n\n- [requests](https://
 requests.readthedocs.io/en/latest/), to make HTTP requests\n\n#### Data
 validation\n\n- [marshmallow](https://marshmallow.readthedocs.io/en/stable/),
-to serialize, deserialize and validate data\n- ~~[dessert](https://
-desert.readthedocs.io/en/stable/), to generate marshmallow serialization
-schemas~~ â not used because too limited (can\'t work with data where fields
-names are different from the ones of the target dataclass)\n\nI used
-[marshmallow](https://marshmallow.readthedocs.io/en/stable/) to follow the
-tutorial, but [pydantic](https://docs.pydantic.dev/) is more known, and I find
-it easier to use.\n', 'author': 'le-chartreux', 'author_email': 'le-chartreux-
-vert@protonmail.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/le-chartreux/hypermodern-python-tuto', 'package_dir':
-package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
+to serialize, deserialize and validate data\n\nI used [marshmallow](https://
+marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but [pydantic]
+(https://docs.pydantic.dev/) is more known, and I find it easier to use.\n',
+'author': 'le-chartreux', 'author_email': 'le-chartreux-vert@protonmail.com',
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
+le-chartreux/hypermodern-python-tuto', 'package_dir': package_dir, 'packages':
+packages, 'package_data': package_data, 'install_requires': install_requires,
+'entry_points': entry_points, 'python_requires': '>=3.10,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `hypermodern_python_tuto-1.0.2/PKG-INFO` & `hypermodern_python_tuto-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypermodern-python-tuto
-Version: 1.0.2
+Version: 1.0.3
 Summary: Repo to follow the Claudio Jolowicz's tutorial about Hypermodern Python (https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)
 Home-page: https://github.com/le-chartreux/hypermodern-python-tuto
 License: MIT
 Keywords: hypermodern
 Author: le-chartreux
 Author-email: le-chartreux-vert@protonmail.com
 Requires-Python: >=3.10,<4.0
@@ -18,14 +18,15 @@
 Project-URL: Documentation, https://hypermodern-python-tuto.readthedocs.io
 Project-URL: Repository, https://github.com/le-chartreux/hypermodern-python-tuto
 Description-Content-Type: text/markdown
 
 # hypermodern-python-tuto
 
 Repo to follow the Claudio Jolowicz's [tutorial about Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/).
+It follows it until [this release](https://github.com/le-chartreux/hypermodern-python-tuto/releases/tag/v1.0.3). After this one, I started adding further tools, deleting some that I consider useless and replacing some others.
 
 ---
 
 <table>
     <tr>
         <td>
             <b>Package</b>
@@ -148,40 +149,40 @@
 - [pyenv](https://github.com/pyenv/pyenv), to manage Python versions
 
 #### Test
 
 - [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests
 - [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite)
 - [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way
-- [xdoctest](https://pypi.org/project/xdoctest/), to execute the doctests (tests in documentation strings)
 
 #### Linting
 
 - [flake8](https://flake8.pycqa.org/en/latest/), a linter aggregator
-- [flake8-import-order](https://github.com/PyCQA/flake8-import-order), to verify that imports are grouped and ordered in a consistent way
+- [flake8-isort](https://pypi.org/project/flake8-isort/), to verify that imports are grouped and ordered in a consistent way
 - [flake8-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design problems
 - [flake8-annotations](https://pypi.org/project/flake8-annotations/), to detect the absence of type annotations
 - [flake8-black](https://pypi.org/project/flake8-black/), to check if the code follows [black](https://black.readthedocs.io/en/stable/) formatting
 - [flake8-docstrings](https://pypi.org/project/flake8-docstrings/), to check that the code is correctly documented
+- [flake8-pytest-style](https://pypi.org/project/flake8-pytest-style/), to check style issues with pytest-based tests
 - [darglint](https://pypi.org/project/darglint/), to check that docstrings match function definitions
 
 #### Security
 
 - [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/))
 - [Safety](https://pyup.io/safety/), to check if some packages are insecure
 
 #### Formatting
 
 - [black](https://black.readthedocs.io/en/stable/), to format the code
+- [isort](https://pycqa.github.io/isort/index.html), to sort imports
 
 #### Type checking
 
 - [mypy](https://mypy-lang.org/), the classic type checker
-- [pytype](https://google.github.io/pytype/), a static type checker
-- [typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type check
+- [typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type checker
 
 #### Documentation
 
 - [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation.
 - [Read the Docs](https://readthedocs.org/), to host the documentation.
 - [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.
 - [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.
@@ -198,11 +199,10 @@
 #### Communication
 
 - [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests
 
 #### Data validation
 
 - [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data
-- ~~[dessert](https://desert.readthedocs.io/en/stable/), to generate marshmallow serialization schemas~~ → not used because too limited (can't work with data where fields names are different from the ones of the target dataclass)
 
 I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but  [pydantic](https://docs.pydantic.dev/) is more known, and I find it easier to use.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 2.1 Name: hypermodern-python-tuto Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: hypermodern-python-tuto Version: 1.0.3 Summary:
 Repo to follow the Claudio Jolowicz's tutorial about Hypermodern Python (https:
 //cjolowicz.github.io/posts/hypermodern-python-01-setup/) Home-page: https://
 github.com/le-chartreux/hypermodern-python-tuto License: MIT Keywords:
 hypermodern Author: le-chartreux Author-email: le-chartreux-vert@protonmail.com
 Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: marshmallow
 (>=3.19.0,<4.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Project-URL:
 Documentation, https://hypermodern-python-tuto.readthedocs.io Project-URL:
 Repository, https://github.com/le-chartreux/hypermodern-python-tuto
 Description-Content-Type: text/markdown # hypermodern-python-tuto Repo to
 follow the Claudio Jolowicz's [tutorial about Hypermodern Python](https://
-cjolowicz.github.io/posts/hypermodern-python-01-setup/). ---
+cjolowicz.github.io/posts/hypermodern-python-01-setup/). It follows it until
+[this release](https://github.com/le-chartreux/hypermodern-python-tuto/
+releases/tag/v1.0.3). After this one, I started adding further tools, deleting
+some that I consider useless and replacing some others. ---
 Package [Supported_Python_Versions] [PyPI_version] [PyPI_downloads]
 CI      [Tests_status] [Documentation_status] [Coverage_status]
 Code    [Code_quality] [pre-commit]
 --- ## Table of contents - [Overview](#overview) - [Install](#install) - [Use]
 (#use) - [Tools used](#tools-used) - [Generic tools](#generic-tools) - [Generic
 Python tools](#generic-python-tools) - [Multi-purpose](#multi-purpose) -
 [Setup](#setup) - [Test](#test) - [Linting](#linting) - [Security](#security) -
@@ -46,46 +49,44 @@
 Setup - [pyenv](https://github.com/pyenv/pyenv), to manage Python versions ####
 Test - [pytest](https://docs.pytest.org/en/latest/), a framework to write unit
 tests. Also used to run doctests - [pytest-cov](https://pytest-
 cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which
 the source code of a program is executed while running its test suite) -
 [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the
 [unittest](https://docs.python.org/3/library/unittest.html) mocking in the
-pytest way - [xdoctest](https://pypi.org/project/xdoctest/), to execute the
-doctests (tests in documentation strings) #### Linting - [flake8](https://
-flake8.pycqa.org/en/latest/), a linter aggregator - [flake8-import-order]
-(https://github.com/PyCQA/flake8-import-order), to verify that imports are
-grouped and ordered in a consistent way - [flake8-bugbear](https://github.com/
-PyCQA/flake8-bugbear), to find bugs and design problems - [flake8-annotations]
-(https://pypi.org/project/flake8-annotations/), to detect the absence of type
-annotations - [flake8-black](https://pypi.org/project/flake8-black/), to check
-if the code follows [black](https://black.readthedocs.io/en/stable/) formatting
-- [flake8-docstrings](https://pypi.org/project/flake8-docstrings/), to check
-that the code is correctly documented - [darglint](https://pypi.org/project/
-darglint/), to check that docstrings match function definitions #### Security -
-[Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues
-(used inside linting with [flake8-bandit](https://pypi.org/project/flake8-
-bandit/)) - [Safety](https://pyup.io/safety/), to check if some packages are
-insecure #### Formatting - [black](https://black.readthedocs.io/en/stable/), to
-format the code #### Type checking - [mypy](https://mypy-lang.org/), the
-classic type checker - [pytype](https://google.github.io/pytype/), a static
-type checker - [typeguard](https://typeguard.readthedocs.io/en/latest/), a
-runtime type check #### Documentation - [Sphinx](https://www.sphinx-doc.org/en/
-master/), the documentation tool used by the official Python documentation. -
-[Read the Docs](https://readthedocs.org/), to host the documentation. -
-[autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html),
-Sphinx official plugin to generate API documentation from the docstrings. -
-[napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/
-napoleon.html), Sphinx official plugin to allow compatibility with Google-style
-docstrings. - [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-
-autodoc-typehints/), Sphinx plugin to detect type hints in generated
-documentation. ### Specific Python tools Tools to match specific needs of the
-projet. #### UI - [click](https://click.palletsprojects.com/en/8.1.x/), to
-create CLI applications #### Communication - [requests](https://
-requests.readthedocs.io/en/latest/), to make HTTP requests #### Data validation
-- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize,
-deserialize and validate data - ~~[dessert](https://desert.readthedocs.io/en/
-stable/), to generate marshmallow serialization schemas~~ â not used because
-too limited (can't work with data where fields names are different from the
-ones of the target dataclass) I used [marshmallow](https://
-marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but [pydantic]
-(https://docs.pydantic.dev/) is more known, and I find it easier to use.
+pytest way #### Linting - [flake8](https://flake8.pycqa.org/en/latest/), a
+linter aggregator - [flake8-isort](https://pypi.org/project/flake8-isort/), to
+verify that imports are grouped and ordered in a consistent way - [flake8-
+bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design
+problems - [flake8-annotations](https://pypi.org/project/flake8-annotations/),
+to detect the absence of type annotations - [flake8-black](https://pypi.org/
+project/flake8-black/), to check if the code follows [black](https://
+black.readthedocs.io/en/stable/) formatting - [flake8-docstrings](https://
+pypi.org/project/flake8-docstrings/), to check that the code is correctly
+documented - [flake8-pytest-style](https://pypi.org/project/flake8-pytest-
+style/), to check style issues with pytest-based tests - [darglint](https://
+pypi.org/project/darglint/), to check that docstrings match function
+definitions #### Security - [Bandit](https://bandit.readthedocs.io/en/latest/),
+to find security issues (used inside linting with [flake8-bandit](https://
+pypi.org/project/flake8-bandit/)) - [Safety](https://pyup.io/safety/), to check
+if some packages are insecure #### Formatting - [black](https://
+black.readthedocs.io/en/stable/), to format the code - [isort](https://
+pycqa.github.io/isort/index.html), to sort imports #### Type checking - [mypy]
+(https://mypy-lang.org/), the classic type checker - [typeguard](https://
+typeguard.readthedocs.io/en/latest/), a runtime type checker #### Documentation
+- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used
+by the official Python documentation. - [Read the Docs](https://
+readthedocs.org/), to host the documentation. - [autodoc](https://www.sphinx-
+doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to
+generate API documentation from the docstrings. - [napoleon](https://
+www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official
+plugin to allow compatibility with Google-style docstrings. - [sphinx-autodoc-
+typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin
+to detect type hints in generated documentation. ### Specific Python tools
+Tools to match specific needs of the projet. #### UI - [click](https://
+click.palletsprojects.com/en/8.1.x/), to create CLI applications ####
+Communication - [requests](https://requests.readthedocs.io/en/latest/), to make
+HTTP requests #### Data validation - [marshmallow](https://
+marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate
+data I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to
+follow the tutorial, but [pydantic](https://docs.pydantic.dev/) is more known,
+and I find it easier to use.
```

