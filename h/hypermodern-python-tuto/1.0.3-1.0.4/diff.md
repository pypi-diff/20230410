# Comparing `tmp/hypermodern_python_tuto-1.0.3.tar.gz` & `tmp/hypermodern_python_tuto-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypermodern_python_tuto-1.0.3.tar", max compression
+gzip compressed data, was "hypermodern_python_tuto-1.0.4.tar", max compression
```

## Comparing `hypermodern_python_tuto-1.0.3.tar` & `hypermodern_python_tuto-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/LICENSE
--rw-r--r--   0        0        0     7758 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/README.md
--rw-r--r--   0        0        0     1661 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      221 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/__init__.py
--rw-r--r--   0        0        0     1234 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/__main__.py
--rw-r--r--   0        0        0      708 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/ui.py
--rw-r--r--   0        0        0      330 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/article.py
--rw-r--r--   0        0        0      918 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/article_schema.py
--rw-r--r--   0        0        0     2374 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/language.py
--rw-r--r--   0        0        0     1962 2023-04-10 15:55:39.980625 hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/requester.py
--rw-r--r--   0        0        0     9085 1970-01-01 00:00:00.000000 hypermodern_python_tuto-1.0.3/setup.py
--rw-r--r--   0        0        0     8694 1970-01-01 00:00:00.000000 hypermodern_python_tuto-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-10 20:20:31.549745 hypermodern_python_tuto-1.0.4/LICENSE
+-rw-r--r--   0        0        0     7030 2023-04-10 20:20:31.549745 hypermodern_python_tuto-1.0.4/README.md
+-rw-r--r--   0        0        0     5438 2023-04-10 20:20:31.549745 hypermodern_python_tuto-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-04-10 20:20:31.549745 hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/__init__.py
+-rw-r--r--   0        0        0     1064 2023-04-10 20:20:31.549745 hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/__main__.py
+-rw-r--r--   0        0        0      639 2023-04-10 20:20:31.549745 hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/ui.py
+-rw-r--r--   0        0        0      330 2023-04-10 20:20:31.553745 hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/wikipedia/article.py
+-rw-r--r--   0        0        0      918 2023-04-10 20:20:31.553745 hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/wikipedia/article_schema.py
+-rw-r--r--   0        0        0     2386 2023-04-10 20:20:31.553745 hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/wikipedia/language.py
+-rw-r--r--   0        0        0     2593 2023-04-10 20:20:31.553745 hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/wikipedia/requester.py
+-rw-r--r--   0        0        0     8350 1970-01-01 00:00:00.000000 hypermodern_python_tuto-1.0.4/setup.py
+-rw-r--r--   0        0        0     7966 1970-01-01 00:00:00.000000 hypermodern_python_tuto-1.0.4/PKG-INFO
```

### Comparing `hypermodern_python_tuto-1.0.3/LICENSE` & `hypermodern_python_tuto-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hypermodern_python_tuto-1.0.3/README.md` & `hypermodern_python_tuto-1.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -102,85 +102,77 @@
 
 ## Tools used
 
 ### Generic tools
 
 Tools that can be used in every development project, no matter if it's a Python project or not.
 
-- [git](https://git-scm.com/), to manage versions of the source code
+- [Codecov](https://about.codecov.io/), to mesure code coverage on repos. I let it in this project since it is already setup, but I don't think I will use it in other projects.
+- [git](https://git-scm.com/), to manage versions of the source code.
 - [GitHub](https://github.com/le-chartreux/hypermodern-python-tuto), to host the git repository and automate tasks with [GitHub Actions](https://docs.github.com/en/actions):
-  - [Release Drafter](https://github.com/marketplace/actions/release-drafter), to create release templates
-- [pre-commit](https://pre-commit.com/), to manage pre-commit hooks
-- [Codecov](https://about.codecov.io/), to mesure code coverage on repos
+  - [Release Drafter](https://github.com/marketplace/actions/release-drafter), to create release templates.
+- [pre-commit](https://pre-commit.com/), to manage pre-commit hooks.
 
 ### Generic Python tools
 
 Tools that can be used in every Python project, no matter its content.
 
 #### Multi-purpose
 
-- [PyPI](https://pypi.org/), to install and publish Python packages
-- [TestPyPI](https://pypi.org/), PyPI but for testing purposes
-- [poetry](https://python-poetry.org/), to make development and distribution easy (packaging, virtualization, dependencies, launching and publishing)
-- [nox](https://nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like tests, linting, reformatting, etc.)
+- [nox](https://nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like tests, linting, reformatting, etc.).
+- [PyPI](https://pypi.org/), to install and publish Python packages.
+- [poetry](https://python-poetry.org/), to make development and distribution easy (packaging, virtualization, dependencies, launching and publishing).
+- [TestPyPI](https://pypi.org/), PyPI but for testing purposes.
 
 #### Setup
 
-- [pyenv](https://github.com/pyenv/pyenv), to manage Python versions
+- [pyenv](https://github.com/pyenv/pyenv), to manage Python versions.
 
 #### Test
 
-- [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests
-- [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite)
-- [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way
+- [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests.
+- [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite).
+- [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way.
 
 #### Linting
 
-- [flake8](https://flake8.pycqa.org/en/latest/), a linter aggregator
-- [flake8-isort](https://pypi.org/project/flake8-isort/), to verify that imports are grouped and ordered in a consistent way
-- [flake8-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design problems
-- [flake8-annotations](https://pypi.org/project/flake8-annotations/), to detect the absence of type annotations
-- [flake8-black](https://pypi.org/project/flake8-black/), to check if the code follows [black](https://black.readthedocs.io/en/stable/) formatting
-- [flake8-docstrings](https://pypi.org/project/flake8-docstrings/), to check that the code is correctly documented
-- [flake8-pytest-style](https://pypi.org/project/flake8-pytest-style/), to check style issues with pytest-based tests
-- [darglint](https://pypi.org/project/darglint/), to check that docstrings match function definitions
+- [Ruff](https://beta.ruff.rs/docs/), an extremely fast linter that support of all main linter rules.
 
 #### Security
 
-- [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/))
-- [Safety](https://pyup.io/safety/), to check if some packages are insecure
+- [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/)).
+- [Safety](https://pyup.io/safety/), to check if some packages are insecure.
 
 #### Formatting
 
-- [black](https://black.readthedocs.io/en/stable/), to format the code
-- [isort](https://pycqa.github.io/isort/index.html), to sort imports
+- [black](https://black.readthedocs.io/en/stable/), to format the code.
+- [isort](https://pycqa.github.io/isort/index.html), to sort imports.
 
 #### Type checking
 
-- [mypy](https://mypy-lang.org/), the classic type checker
-- [typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type checker
+- [mypy](https://mypy-lang.org/), the classic type checker.
 
 #### Documentation
 
-- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation.
 - [Read the Docs](https://readthedocs.org/), to host the documentation.
-- [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.
-- [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.
-- [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin to detect type hints in generated documentation.
+- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation, with:
+  - [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.
+  - [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.
+  - [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin to detect type hints in generated documentation.
 
 ### Specific Python tools
 
 Tools to match specific needs of the projet.
 
 #### UI
 
-- [click](https://click.palletsprojects.com/en/8.1.x/), to create CLI applications
+- [click](https://click.palletsprojects.com/en/8.1.x/), to create CLI applications.
 
 #### Communication
 
-- [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests
+- [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests.
 
 #### Data validation
 
-- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data
+- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data.
 
 I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but  [pydantic](https://docs.pydantic.dev/) is more known, and I find it easier to use.
```

#### html2text {}

```diff
@@ -16,65 +16,54 @@
 - [Communication](#communication) - [Data validation](#data-validation) ##
 Overview The app created is a CLI application that queries a random Wikipedia
 page and displays its title and summary. ## Install ```shell pip install
 hypermodern-python-tuto ``` ## Use ### Basic usage Just run the following
 command: ```shell hypermodern-python-tuto ``` ### Other options Look at the
 [documentation](https://hypermodern-python-tuto.readthedocs.io/). ## Tools used
 ### Generic tools Tools that can be used in every development project, no
-matter if it's a Python project or not. - [git](https://git-scm.com/), to
-manage versions of the source code - [GitHub](https://github.com/le-chartreux/
-hypermodern-python-tuto), to host the git repository and automate tasks with
-[GitHub Actions](https://docs.github.com/en/actions): - [Release Drafter]
-(https://github.com/marketplace/actions/release-drafter), to create release
-templates - [pre-commit](https://pre-commit.com/), to manage pre-commit hooks -
-[Codecov](https://about.codecov.io/), to mesure code coverage on repos ###
-Generic Python tools Tools that can be used in every Python project, no matter
-its content. #### Multi-purpose - [PyPI](https://pypi.org/), to install and
-publish Python packages - [TestPyPI](https://pypi.org/), PyPI but for testing
-purposes - [poetry](https://python-poetry.org/), to make development and
-distribution easy (packaging, virtualization, dependencies, launching and
-publishing) - [nox](https://nox.thea.codes/en/stable/), to run tasks in
-multiple Python environments (like tests, linting, reformatting, etc.) ####
-Setup - [pyenv](https://github.com/pyenv/pyenv), to manage Python versions ####
-Test - [pytest](https://docs.pytest.org/en/latest/), a framework to write unit
-tests. Also used to run doctests - [pytest-cov](https://pytest-
-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which
-the source code of a program is executed while running its test suite) -
-[pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the
-[unittest](https://docs.python.org/3/library/unittest.html) mocking in the
-pytest way #### Linting - [flake8](https://flake8.pycqa.org/en/latest/), a
-linter aggregator - [flake8-isort](https://pypi.org/project/flake8-isort/), to
-verify that imports are grouped and ordered in a consistent way - [flake8-
-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design
-problems - [flake8-annotations](https://pypi.org/project/flake8-annotations/),
-to detect the absence of type annotations - [flake8-black](https://pypi.org/
-project/flake8-black/), to check if the code follows [black](https://
-black.readthedocs.io/en/stable/) formatting - [flake8-docstrings](https://
-pypi.org/project/flake8-docstrings/), to check that the code is correctly
-documented - [flake8-pytest-style](https://pypi.org/project/flake8-pytest-
-style/), to check style issues with pytest-based tests - [darglint](https://
-pypi.org/project/darglint/), to check that docstrings match function
-definitions #### Security - [Bandit](https://bandit.readthedocs.io/en/latest/),
-to find security issues (used inside linting with [flake8-bandit](https://
-pypi.org/project/flake8-bandit/)) - [Safety](https://pyup.io/safety/), to check
-if some packages are insecure #### Formatting - [black](https://
-black.readthedocs.io/en/stable/), to format the code - [isort](https://
-pycqa.github.io/isort/index.html), to sort imports #### Type checking - [mypy]
-(https://mypy-lang.org/), the classic type checker - [typeguard](https://
-typeguard.readthedocs.io/en/latest/), a runtime type checker #### Documentation
-- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used
-by the official Python documentation. - [Read the Docs](https://
-readthedocs.org/), to host the documentation. - [autodoc](https://www.sphinx-
-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to
-generate API documentation from the docstrings. - [napoleon](https://
-www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official
-plugin to allow compatibility with Google-style docstrings. - [sphinx-autodoc-
-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin
-to detect type hints in generated documentation. ### Specific Python tools
-Tools to match specific needs of the projet. #### UI - [click](https://
-click.palletsprojects.com/en/8.1.x/), to create CLI applications ####
+matter if it's a Python project or not. - [Codecov](https://about.codecov.io/),
+to mesure code coverage on repos. I let it in this project since it is already
+setup, but I don't think I will use it in other projects. - [git](https://git-
+scm.com/), to manage versions of the source code. - [GitHub](https://
+github.com/le-chartreux/hypermodern-python-tuto), to host the git repository
+and automate tasks with [GitHub Actions](https://docs.github.com/en/actions): -
+[Release Drafter](https://github.com/marketplace/actions/release-drafter), to
+create release templates. - [pre-commit](https://pre-commit.com/), to manage
+pre-commit hooks. ### Generic Python tools Tools that can be used in every
+Python project, no matter its content. #### Multi-purpose - [nox](https://
+nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like
+tests, linting, reformatting, etc.). - [PyPI](https://pypi.org/), to install
+and publish Python packages. - [poetry](https://python-poetry.org/), to make
+development and distribution easy (packaging, virtualization, dependencies,
+launching and publishing). - [TestPyPI](https://pypi.org/), PyPI but for
+testing purposes. #### Setup - [pyenv](https://github.com/pyenv/pyenv), to
+manage Python versions. #### Test - [pytest](https://docs.pytest.org/en/latest/
+), a framework to write unit tests. Also used to run doctests. - [pytest-cov]
+(https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage
+(degree to which the source code of a program is executed while running its
+test suite). - [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to
+use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in
+the pytest way. #### Linting - [Ruff](https://beta.ruff.rs/docs/), an extremely
+fast linter that support of all main linter rules. #### Security - [Bandit]
+(https://bandit.readthedocs.io/en/latest/), to find security issues (used
+inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/)).
+- [Safety](https://pyup.io/safety/), to check if some packages are insecure.
+#### Formatting - [black](https://black.readthedocs.io/en/stable/), to format
+the code. - [isort](https://pycqa.github.io/isort/index.html), to sort imports.
+#### Type checking - [mypy](https://mypy-lang.org/), the classic type checker.
+#### Documentation - [Read the Docs](https://readthedocs.org/), to host the
+documentation. - [Sphinx](https://www.sphinx-doc.org/en/master/), the
+documentation tool used by the official Python documentation, with: - [autodoc]
+(https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx
+official plugin to generate API documentation from the docstrings. - [napoleon]
+(https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx
+official plugin to allow compatibility with Google-style docstrings. - [sphinx-
+autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx
+plugin to detect type hints in generated documentation. ### Specific Python
+tools Tools to match specific needs of the projet. #### UI - [click](https://
+click.palletsprojects.com/en/8.1.x/), to create CLI applications. ####
 Communication - [requests](https://requests.readthedocs.io/en/latest/), to make
-HTTP requests #### Data validation - [marshmallow](https://
+HTTP requests. #### Data validation - [marshmallow](https://
 marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate
-data I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to
+data. I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to
 follow the tutorial, but [pydantic](https://docs.pydantic.dev/) is more known,
 and I find it easier to use.
```

### Comparing `hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/__main__.py` & `hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 """Command-line interface."""
 import click
 import marshmallow
 import requests
 
-import hypermodern_python_tuto
-import hypermodern_python_tuto.ui
-import hypermodern_python_tuto.wikipedia.language
-import hypermodern_python_tuto.wikipedia.requester
+from hypermodern_python_tuto import __version__
+from hypermodern_python_tuto.ui import print_wikipedia_article
+from hypermodern_python_tuto.wikipedia.language import Language
+from hypermodern_python_tuto.wikipedia.requester import WikipediaRequester
 
 
 @click.command()
-@click.version_option(version=hypermodern_python_tuto.__version__)
+@click.version_option(version=__version__)
 @click.option(
     "--language",
-    type=click.Choice(
-        list(hypermodern_python_tuto.wikipedia.language.Language), case_sensitive=False
-    ),
+    type=click.Choice(list(Language), case_sensitive=False),
     help="Set the language of the page",
-    default=hypermodern_python_tuto.wikipedia.language.Language.from_preferences(),
+    default=Language.from_preferences(),
 )
-def main(language: hypermodern_python_tuto.wikipedia.language.Language) -> None:
+def main(language: Language) -> None:
     """Display the title and the summary of a random Wikipedia article."""
-    wikipedia_requester = (
-        hypermodern_python_tuto.wikipedia.requester.WikipediaRequester()
-    )
+    wikipedia_requester = WikipediaRequester()
     wikipedia_requester.set_language(language)
     try:
         wikipedia_article = wikipedia_requester.get_random_article()
     except (requests.RequestException, marshmallow.ValidationError) as error:
         message = str(error)
         raise click.ClickException(message) from error
 
-    hypermodern_python_tuto.ui.print_wikipedia_article(wikipedia_article)
+    print_wikipedia_article(wikipedia_article)
```

### Comparing `hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/ui.py` & `hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/ui.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Utilities to show content to the user."""
 import textwrap
 
 import click
 
-import hypermodern_python_tuto.wikipedia.article
+from hypermodern_python_tuto.wikipedia.article import WikipediaArticle
 
 
-def print_wikipedia_article(
-    wikipedia_article: hypermodern_python_tuto.wikipedia.article.WikipediaArticle,
-) -> None:
+def print_wikipedia_article(wikipedia_article: WikipediaArticle) -> None:
     """Show an article on the standard text output.
 
     Prints in green the title, followed by the summary.
 
     Args:
         wikipedia_article: the article to print.
 
     Examples:
-        >>> article = hypermodern_python_tuto.wikipedia.article.WikipediaArticle("a", "b")
+        >>> article = WikipediaArticle("a", "b")
         >>> print_wikipedia_article(article)
         a
         b
     """
     click.secho(wikipedia_article.title, fg="green")
     click.echo(textwrap.fill(wikipedia_article.summary))
```

### Comparing `hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/article_schema.py` & `hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/wikipedia/article_schema.py`

 * *Files identical despite different names*

### Comparing `hypermodern_python_tuto-1.0.3/src/hypermodern_python_tuto/wikipedia/language.py` & `hypermodern_python_tuto-1.0.4/src/hypermodern_python_tuto/wikipedia/language.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,27 +28,27 @@
         Examples:
             >>> language = Language.from_preferences()
             >>> isinstance(language, Language)
             True
         """
         if os.name == "posix":
             return cls._from_preferences_posix()
-        elif os.name == "nt":
+        if os.name == "nt":
             return cls._from_preferences_windows()
-        else:
-            raise RuntimeError(f"Unsupported operating system: {os.name}.")
+        error_message = f"Unsupported operating system: {os.name}."
+        raise RuntimeError(error_message)
 
     @classmethod
     def _from_preferences_posix(cls) -> "Language":
         language = os.environ["LANG"]
         return cls.from_str(language)
 
     @classmethod
     def _from_preferences_windows(cls) -> "Language":
-        windll = ctypes.windll.kernel32  # type: ignore
+        windll = ctypes.windll.kernel32  # type: ignore[attr-defined]
         language = locale.windows_locale[windll.GetUserDefaultUILanguage()]
         return cls.from_str(language)
 
     @classmethod
     def from_str(cls, language: str) -> "Language":
         """Convert a language name to its equivalent Enum.
 
@@ -69,11 +69,10 @@
             True
             >>> Language.from_str("unrecognized") is Language.OTHER
             True
         """
         language = language.lower()
         if language.startswith("fr"):
             return cls.FRENCH
-        elif language.startswith("en"):
+        if language.startswith("en"):
             return cls.ENGLISH
-        else:
-            return cls.OTHER
+        return cls.OTHER
```

### Comparing `hypermodern_python_tuto-1.0.3/setup.py` & `hypermodern_python_tuto-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'console_scripts': ['hypermodern-python-tuto = '
                      'hypermodern_python_tuto.__main__:main']}
 
 setup_kwargs = {
     'name': 'hypermodern-python-tuto',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': "Repo to follow the Claudio Jolowicz's tutorial about Hypermodern Python (https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)",
-    'long_description': '# hypermodern-python-tuto\n\nRepo to follow the Claudio Jolowicz\'s [tutorial about Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/).\nIt follows it until [this release](https://github.com/le-chartreux/hypermodern-python-tuto/releases/tag/v1.0.3). After this one, I started adding further tools, deleting some that I consider useless and replacing some others.\n\n---\n\n<table>\n    <tr>\n        <td>\n            <b>Package</b>\n        </td>\n        <td>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/pyversions/hypermodern-python-tuto.svg" alt="Supported Python Versions">\n            </a>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/v/hypermodern-python-tuto.svg" alt="PyPI version">\n            </a>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/dm/hypermodern-python-tuto.svg" alt="PyPI downloads">\n            </a>\n        </td>\n    </tr>\n    <tr>\n        <td>\n            <b>CI</b>\n        </td>\n        <td>\n            <a href="https://github.com/le-chartreux/hypermodern-python-tuto/actions?workflow=Tests">\n                <img src="https://github.com/le-chartreux/hypermodern-python-tuto/workflows/Tests/badge.svg" alt="Tests status">\n            </a>\n            <a href="https://hypermodern-python-tuto.readthedocs.io/">\n                <img src="https://readthedocs.org/projects/hypermodern-python-tuto/badge/" alt="Documentation status">\n            </a>\n            <a href="https://codecov.io/gh/le-chartreux/hypermodern-python-tuto">\n                <img src="https://codecov.io/gh/le-chartreux/hypermodern-python-tuto/branch/master/graph/badge.svg" alt="Coverage status">\n            </a>\n        </td>\n    </tr>\n    <tr>\n        <td>\n            <b>Code</b>\n        </td>\n        <td>\n            <a href="https://github.com/psf/black">\n                <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code quality">\n            </a>\n            <a href="https://github.com/pre-commit/pre-commit">\n                <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen" alt="pre-commit">\n            </a>\n        </td>\n    </tr>\n</table>\n\n---\n\n## Table of contents\n\n- [Overview](#overview)\n- [Install](#install)\n- [Use](#use)\n- [Tools used](#tools-used)\n  - [Generic tools](#generic-tools)\n  - [Generic Python tools](#generic-python-tools)\n    - [Multi-purpose](#multi-purpose)\n    - [Setup](#setup)\n    - [Test](#test)\n    - [Linting](#linting)\n    - [Security](#security)\n    - [Formatting](#formatting)\n    - [Type checking](#type-checking)\n    - [Documentation](#documentation)\n  - [Specific Python tools](#specific-python-tools)\n    - [UI](#ui)\n    - [Communication](#communication)\n    - [Data validation](#data-validation)\n\n## Overview\n\nThe app created is a CLI application that queries a random Wikipedia page and displays its title and summary.\n\n## Install\n\n```shell\npip install hypermodern-python-tuto\n```\n\n## Use\n\n### Basic usage\n\nJust run the following command:\n\n```shell\nhypermodern-python-tuto\n```\n\n### Other options\n\nLook at the [documentation](https://hypermodern-python-tuto.readthedocs.io/).\n\n## Tools used\n\n### Generic tools\n\nTools that can be used in every development project, no matter if it\'s a Python project or not.\n\n- [git](https://git-scm.com/), to manage versions of the source code\n- [GitHub](https://github.com/le-chartreux/hypermodern-python-tuto), to host the git repository and automate tasks with [GitHub Actions](https://docs.github.com/en/actions):\n  - [Release Drafter](https://github.com/marketplace/actions/release-drafter), to create release templates\n- [pre-commit](https://pre-commit.com/), to manage pre-commit hooks\n- [Codecov](https://about.codecov.io/), to mesure code coverage on repos\n\n### Generic Python tools\n\nTools that can be used in every Python project, no matter its content.\n\n#### Multi-purpose\n\n- [PyPI](https://pypi.org/), to install and publish Python packages\n- [TestPyPI](https://pypi.org/), PyPI but for testing purposes\n- [poetry](https://python-poetry.org/), to make development and distribution easy (packaging, virtualization, dependencies, launching and publishing)\n- [nox](https://nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like tests, linting, reformatting, etc.)\n\n#### Setup\n\n- [pyenv](https://github.com/pyenv/pyenv), to manage Python versions\n\n#### Test\n\n- [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests\n- [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite)\n- [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way\n\n#### Linting\n\n- [flake8](https://flake8.pycqa.org/en/latest/), a linter aggregator\n- [flake8-isort](https://pypi.org/project/flake8-isort/), to verify that imports are grouped and ordered in a consistent way\n- [flake8-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design problems\n- [flake8-annotations](https://pypi.org/project/flake8-annotations/), to detect the absence of type annotations\n- [flake8-black](https://pypi.org/project/flake8-black/), to check if the code follows [black](https://black.readthedocs.io/en/stable/) formatting\n- [flake8-docstrings](https://pypi.org/project/flake8-docstrings/), to check that the code is correctly documented\n- [flake8-pytest-style](https://pypi.org/project/flake8-pytest-style/), to check style issues with pytest-based tests\n- [darglint](https://pypi.org/project/darglint/), to check that docstrings match function definitions\n\n#### Security\n\n- [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/))\n- [Safety](https://pyup.io/safety/), to check if some packages are insecure\n\n#### Formatting\n\n- [black](https://black.readthedocs.io/en/stable/), to format the code\n- [isort](https://pycqa.github.io/isort/index.html), to sort imports\n\n#### Type checking\n\n- [mypy](https://mypy-lang.org/), the classic type checker\n- [typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type checker\n\n#### Documentation\n\n- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation.\n- [Read the Docs](https://readthedocs.org/), to host the documentation.\n- [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.\n- [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.\n- [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin to detect type hints in generated documentation.\n\n### Specific Python tools\n\nTools to match specific needs of the projet.\n\n#### UI\n\n- [click](https://click.palletsprojects.com/en/8.1.x/), to create CLI applications\n\n#### Communication\n\n- [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests\n\n#### Data validation\n\n- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data\n\nI used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but  [pydantic](https://docs.pydantic.dev/) is more known, and I find it easier to use.\n',
+    'long_description': '# hypermodern-python-tuto\n\nRepo to follow the Claudio Jolowicz\'s [tutorial about Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/).\nIt follows it until [this release](https://github.com/le-chartreux/hypermodern-python-tuto/releases/tag/v1.0.3). After this one, I started adding further tools, deleting some that I consider useless and replacing some others.\n\n---\n\n<table>\n    <tr>\n        <td>\n            <b>Package</b>\n        </td>\n        <td>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/pyversions/hypermodern-python-tuto.svg" alt="Supported Python Versions">\n            </a>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/v/hypermodern-python-tuto.svg" alt="PyPI version">\n            </a>\n            <a href="https://pypi.org/project/hypermodern-python-tuto/">\n                <img src="https://img.shields.io/pypi/dm/hypermodern-python-tuto.svg" alt="PyPI downloads">\n            </a>\n        </td>\n    </tr>\n    <tr>\n        <td>\n            <b>CI</b>\n        </td>\n        <td>\n            <a href="https://github.com/le-chartreux/hypermodern-python-tuto/actions?workflow=Tests">\n                <img src="https://github.com/le-chartreux/hypermodern-python-tuto/workflows/Tests/badge.svg" alt="Tests status">\n            </a>\n            <a href="https://hypermodern-python-tuto.readthedocs.io/">\n                <img src="https://readthedocs.org/projects/hypermodern-python-tuto/badge/" alt="Documentation status">\n            </a>\n            <a href="https://codecov.io/gh/le-chartreux/hypermodern-python-tuto">\n                <img src="https://codecov.io/gh/le-chartreux/hypermodern-python-tuto/branch/master/graph/badge.svg" alt="Coverage status">\n            </a>\n        </td>\n    </tr>\n    <tr>\n        <td>\n            <b>Code</b>\n        </td>\n        <td>\n            <a href="https://github.com/psf/black">\n                <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code quality">\n            </a>\n            <a href="https://github.com/pre-commit/pre-commit">\n                <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen" alt="pre-commit">\n            </a>\n        </td>\n    </tr>\n</table>\n\n---\n\n## Table of contents\n\n- [Overview](#overview)\n- [Install](#install)\n- [Use](#use)\n- [Tools used](#tools-used)\n  - [Generic tools](#generic-tools)\n  - [Generic Python tools](#generic-python-tools)\n    - [Multi-purpose](#multi-purpose)\n    - [Setup](#setup)\n    - [Test](#test)\n    - [Linting](#linting)\n    - [Security](#security)\n    - [Formatting](#formatting)\n    - [Type checking](#type-checking)\n    - [Documentation](#documentation)\n  - [Specific Python tools](#specific-python-tools)\n    - [UI](#ui)\n    - [Communication](#communication)\n    - [Data validation](#data-validation)\n\n## Overview\n\nThe app created is a CLI application that queries a random Wikipedia page and displays its title and summary.\n\n## Install\n\n```shell\npip install hypermodern-python-tuto\n```\n\n## Use\n\n### Basic usage\n\nJust run the following command:\n\n```shell\nhypermodern-python-tuto\n```\n\n### Other options\n\nLook at the [documentation](https://hypermodern-python-tuto.readthedocs.io/).\n\n## Tools used\n\n### Generic tools\n\nTools that can be used in every development project, no matter if it\'s a Python project or not.\n\n- [Codecov](https://about.codecov.io/), to mesure code coverage on repos. I let it in this project since it is already setup, but I don\'t think I will use it in other projects.\n- [git](https://git-scm.com/), to manage versions of the source code.\n- [GitHub](https://github.com/le-chartreux/hypermodern-python-tuto), to host the git repository and automate tasks with [GitHub Actions](https://docs.github.com/en/actions):\n  - [Release Drafter](https://github.com/marketplace/actions/release-drafter), to create release templates.\n- [pre-commit](https://pre-commit.com/), to manage pre-commit hooks.\n\n### Generic Python tools\n\nTools that can be used in every Python project, no matter its content.\n\n#### Multi-purpose\n\n- [nox](https://nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like tests, linting, reformatting, etc.).\n- [PyPI](https://pypi.org/), to install and publish Python packages.\n- [poetry](https://python-poetry.org/), to make development and distribution easy (packaging, virtualization, dependencies, launching and publishing).\n- [TestPyPI](https://pypi.org/), PyPI but for testing purposes.\n\n#### Setup\n\n- [pyenv](https://github.com/pyenv/pyenv), to manage Python versions.\n\n#### Test\n\n- [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests.\n- [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite).\n- [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way.\n\n#### Linting\n\n- [Ruff](https://beta.ruff.rs/docs/), an extremely fast linter that support of all main linter rules.\n\n#### Security\n\n- [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/)).\n- [Safety](https://pyup.io/safety/), to check if some packages are insecure.\n\n#### Formatting\n\n- [black](https://black.readthedocs.io/en/stable/), to format the code.\n- [isort](https://pycqa.github.io/isort/index.html), to sort imports.\n\n#### Type checking\n\n- [mypy](https://mypy-lang.org/), the classic type checker.\n\n#### Documentation\n\n- [Read the Docs](https://readthedocs.org/), to host the documentation.\n- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation, with:\n  - [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.\n  - [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.\n  - [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin to detect type hints in generated documentation.\n\n### Specific Python tools\n\nTools to match specific needs of the projet.\n\n#### UI\n\n- [click](https://click.palletsprojects.com/en/8.1.x/), to create CLI applications.\n\n#### Communication\n\n- [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests.\n\n#### Data validation\n\n- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data.\n\nI used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but  [pydantic](https://docs.pydantic.dev/) is more known, and I find it easier to use.\n',
     'author': 'le-chartreux',
     'author_email': 'le-chartreux-vert@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/le-chartreux/hypermodern-python-tuto',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['hypermodern_python_tuto',
 'hypermodern_python_tuto.wikipedia'] package_data = \ {'': ['*']}
 install_requires = \ ['click>=8.1.3,<9.0.0', 'marshmallow>=3.19.0,<4.0.0',
 'requests>=2.28.2,<3.0.0'] entry_points = \ {'console_scripts': ['hypermodern-
 python-tuto = ' 'hypermodern_python_tuto.__main__:main']} setup_kwargs =
-{ 'name': 'hypermodern-python-tuto', 'version': '1.0.3', 'description': "Repo
+{ 'name': 'hypermodern-python-tuto', 'version': '1.0.4', 'description': "Repo
 to follow the Claudio Jolowicz's tutorial about Hypermodern Python (https://
 cjolowicz.github.io/posts/hypermodern-python-01-setup/)", 'long_description':
 '# hypermodern-python-tuto\n\nRepo to follow the Claudio Jolowicz\'s [tutorial
 about Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-
 01-setup/).\nIt follows it until [this release](https://github.com/le-
 chartreux/hypermodern-python-tuto/releases/tag/v1.0.3). After this one, I
 started adding further tools, deleting some that I consider useless and
@@ -29,70 +29,60 @@
 app created is a CLI application that queries a random Wikipedia page and
 displays its title and summary.\n\n## Install\n\n```shell\npip install
 hypermodern-python-tuto\n```\n\n## Use\n\n### Basic usage\n\nJust run the
 following command:\n\n```shell\nhypermodern-python-tuto\n```\n\n### Other
 options\n\nLook at the [documentation](https://hypermodern-python-
 tuto.readthedocs.io/).\n\n## Tools used\n\n### Generic tools\n\nTools that can
 be used in every development project, no matter if it\'s a Python project or
-not.\n\n- [git](https://git-scm.com/), to manage versions of the source code\n-
-[GitHub](https://github.com/le-chartreux/hypermodern-python-tuto), to host the
-git repository and automate tasks with [GitHub Actions](https://
-docs.github.com/en/actions):\n - [Release Drafter](https://github.com/
-marketplace/actions/release-drafter), to create release templates\n- [pre-
-commit](https://pre-commit.com/), to manage pre-commit hooks\n- [Codecov]
-(https://about.codecov.io/), to mesure code coverage on repos\n\n### Generic
-Python tools\n\nTools that can be used in every Python project, no matter its
-content.\n\n#### Multi-purpose\n\n- [PyPI](https://pypi.org/), to install and
-publish Python packages\n- [TestPyPI](https://pypi.org/), PyPI but for testing
-purposes\n- [poetry](https://python-poetry.org/), to make development and
-distribution easy (packaging, virtualization, dependencies, launching and
-publishing)\n- [nox](https://nox.thea.codes/en/stable/), to run tasks in
-multiple Python environments (like tests, linting, reformatting, etc.)\n\n####
-Setup\n\n- [pyenv](https://github.com/pyenv/pyenv), to manage Python
-versions\n\n#### Test\n\n- [pytest](https://docs.pytest.org/en/latest/), a
-framework to write unit tests. Also used to run doctests\n- [pytest-cov](https:
-//pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to
-which the source code of a program is executed while running its test suite)\n-
-[pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the
-[unittest](https://docs.python.org/3/library/unittest.html) mocking in the
-pytest way\n\n#### Linting\n\n- [flake8](https://flake8.pycqa.org/en/latest/),
-a linter aggregator\n- [flake8-isort](https://pypi.org/project/flake8-isort/),
-to verify that imports are grouped and ordered in a consistent way\n- [flake8-
-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design
-problems\n- [flake8-annotations](https://pypi.org/project/flake8-annotations/),
-to detect the absence of type annotations\n- [flake8-black](https://pypi.org/
-project/flake8-black/), to check if the code follows [black](https://
-black.readthedocs.io/en/stable/) formatting\n- [flake8-docstrings](https://
-pypi.org/project/flake8-docstrings/), to check that the code is correctly
-documented\n- [flake8-pytest-style](https://pypi.org/project/flake8-pytest-
-style/), to check style issues with pytest-based tests\n- [darglint](https://
-pypi.org/project/darglint/), to check that docstrings match function
-definitions\n\n#### Security\n\n- [Bandit](https://bandit.readthedocs.io/en/
-latest/), to find security issues (used inside linting with [flake8-bandit]
-(https://pypi.org/project/flake8-bandit/))\n- [Safety](https://pyup.io/safety/
-), to check if some packages are insecure\n\n#### Formatting\n\n- [black]
-(https://black.readthedocs.io/en/stable/), to format the code\n- [isort](https:
-//pycqa.github.io/isort/index.html), to sort imports\n\n#### Type checking\n\n-
-[mypy](https://mypy-lang.org/), the classic type checker\n- [typeguard](https:/
-/typeguard.readthedocs.io/en/latest/), a runtime type checker\n\n####
-Documentation\n\n- [Sphinx](https://www.sphinx-doc.org/en/master/), the
-documentation tool used by the official Python documentation.\n- [Read the
-Docs](https://readthedocs.org/), to host the documentation.\n- [autodoc](https:
-//www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official
-plugin to generate API documentation from the docstrings.\n- [napoleon](https:/
-/www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official
-plugin to allow compatibility with Google-style docstrings.\n- [sphinx-autodoc-
-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin
-to detect type hints in generated documentation.\n\n### Specific Python
-tools\n\nTools to match specific needs of the projet.\n\n#### UI\n\n- [click]
-(https://click.palletsprojects.com/en/8.1.x/), to create CLI
-applications\n\n#### Communication\n\n- [requests](https://
-requests.readthedocs.io/en/latest/), to make HTTP requests\n\n#### Data
+not.\n\n- [Codecov](https://about.codecov.io/), to mesure code coverage on
+repos. I let it in this project since it is already setup, but I don\'t think I
+will use it in other projects.\n- [git](https://git-scm.com/), to manage
+versions of the source code.\n- [GitHub](https://github.com/le-chartreux/
+hypermodern-python-tuto), to host the git repository and automate tasks with
+[GitHub Actions](https://docs.github.com/en/actions):\n - [Release Drafter]
+(https://github.com/marketplace/actions/release-drafter), to create release
+templates.\n- [pre-commit](https://pre-commit.com/), to manage pre-commit
+hooks.\n\n### Generic Python tools\n\nTools that can be used in every Python
+project, no matter its content.\n\n#### Multi-purpose\n\n- [nox](https://
+nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like
+tests, linting, reformatting, etc.).\n- [PyPI](https://pypi.org/), to install
+and publish Python packages.\n- [poetry](https://python-poetry.org/), to make
+development and distribution easy (packaging, virtualization, dependencies,
+launching and publishing).\n- [TestPyPI](https://pypi.org/), PyPI but for
+testing purposes.\n\n#### Setup\n\n- [pyenv](https://github.com/pyenv/pyenv),
+to manage Python versions.\n\n#### Test\n\n- [pytest](https://docs.pytest.org/
+en/latest/), a framework to write unit tests. Also used to run doctests.\n-
+[pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code
+coverage (degree to which the source code of a program is executed while
+running its test suite).\n- [pytest-mock](https://pytest-mock.readthedocs.io/
+en/latest/), to use the [unittest](https://docs.python.org/3/library/
+unittest.html) mocking in the pytest way.\n\n#### Linting\n\n- [Ruff](https://
+beta.ruff.rs/docs/), an extremely fast linter that support of all main linter
+rules.\n\n#### Security\n\n- [Bandit](https://bandit.readthedocs.io/en/latest/
+), to find security issues (used inside linting with [flake8-bandit](https://
+pypi.org/project/flake8-bandit/)).\n- [Safety](https://pyup.io/safety/), to
+check if some packages are insecure.\n\n#### Formatting\n\n- [black](https://
+black.readthedocs.io/en/stable/), to format the code.\n- [isort](https://
+pycqa.github.io/isort/index.html), to sort imports.\n\n#### Type checking\n\n-
+[mypy](https://mypy-lang.org/), the classic type checker.\n\n####
+Documentation\n\n- [Read the Docs](https://readthedocs.org/), to host the
+documentation.\n- [Sphinx](https://www.sphinx-doc.org/en/master/), the
+documentation tool used by the official Python documentation, with:\n -
+[autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html),
+Sphinx official plugin to generate API documentation from the docstrings.\n -
+[napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/
+napoleon.html), Sphinx official plugin to allow compatibility with Google-style
+docstrings.\n - [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-
+autodoc-typehints/), Sphinx plugin to detect type hints in generated
+documentation.\n\n### Specific Python tools\n\nTools to match specific needs of
+the projet.\n\n#### UI\n\n- [click](https://click.palletsprojects.com/en/8.1.x/
+), to create CLI applications.\n\n#### Communication\n\n- [requests](https://
+requests.readthedocs.io/en/latest/), to make HTTP requests.\n\n#### Data
 validation\n\n- [marshmallow](https://marshmallow.readthedocs.io/en/stable/),
-to serialize, deserialize and validate data\n\nI used [marshmallow](https://
+to serialize, deserialize and validate data.\n\nI used [marshmallow](https://
 marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but [pydantic]
 (https://docs.pydantic.dev/) is more known, and I find it easier to use.\n',
 'author': 'le-chartreux', 'author_email': 'le-chartreux-vert@protonmail.com',
 'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
 le-chartreux/hypermodern-python-tuto', 'package_dir': package_dir, 'packages':
 packages, 'package_data': package_data, 'install_requires': install_requires,
 'entry_points': entry_points, 'python_requires': '>=3.10,<4.0', } setup
```

### Comparing `hypermodern_python_tuto-1.0.3/PKG-INFO` & `hypermodern_python_tuto-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypermodern-python-tuto
-Version: 1.0.3
+Version: 1.0.4
 Summary: Repo to follow the Claudio Jolowicz's tutorial about Hypermodern Python (https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)
 Home-page: https://github.com/le-chartreux/hypermodern-python-tuto
 License: MIT
 Keywords: hypermodern
 Author: le-chartreux
 Author-email: le-chartreux-vert@protonmail.com
 Requires-Python: >=3.10,<4.0
@@ -123,86 +123,78 @@
 
 ## Tools used
 
 ### Generic tools
 
 Tools that can be used in every development project, no matter if it's a Python project or not.
 
-- [git](https://git-scm.com/), to manage versions of the source code
+- [Codecov](https://about.codecov.io/), to mesure code coverage on repos. I let it in this project since it is already setup, but I don't think I will use it in other projects.
+- [git](https://git-scm.com/), to manage versions of the source code.
 - [GitHub](https://github.com/le-chartreux/hypermodern-python-tuto), to host the git repository and automate tasks with [GitHub Actions](https://docs.github.com/en/actions):
-  - [Release Drafter](https://github.com/marketplace/actions/release-drafter), to create release templates
-- [pre-commit](https://pre-commit.com/), to manage pre-commit hooks
-- [Codecov](https://about.codecov.io/), to mesure code coverage on repos
+  - [Release Drafter](https://github.com/marketplace/actions/release-drafter), to create release templates.
+- [pre-commit](https://pre-commit.com/), to manage pre-commit hooks.
 
 ### Generic Python tools
 
 Tools that can be used in every Python project, no matter its content.
 
 #### Multi-purpose
 
-- [PyPI](https://pypi.org/), to install and publish Python packages
-- [TestPyPI](https://pypi.org/), PyPI but for testing purposes
-- [poetry](https://python-poetry.org/), to make development and distribution easy (packaging, virtualization, dependencies, launching and publishing)
-- [nox](https://nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like tests, linting, reformatting, etc.)
+- [nox](https://nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like tests, linting, reformatting, etc.).
+- [PyPI](https://pypi.org/), to install and publish Python packages.
+- [poetry](https://python-poetry.org/), to make development and distribution easy (packaging, virtualization, dependencies, launching and publishing).
+- [TestPyPI](https://pypi.org/), PyPI but for testing purposes.
 
 #### Setup
 
-- [pyenv](https://github.com/pyenv/pyenv), to manage Python versions
+- [pyenv](https://github.com/pyenv/pyenv), to manage Python versions.
 
 #### Test
 
-- [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests
-- [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite)
-- [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way
+- [pytest](https://docs.pytest.org/en/latest/), a framework to write unit tests. Also used to run doctests.
+- [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which the source code of a program is executed while running its test suite).
+- [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in the pytest way.
 
 #### Linting
 
-- [flake8](https://flake8.pycqa.org/en/latest/), a linter aggregator
-- [flake8-isort](https://pypi.org/project/flake8-isort/), to verify that imports are grouped and ordered in a consistent way
-- [flake8-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design problems
-- [flake8-annotations](https://pypi.org/project/flake8-annotations/), to detect the absence of type annotations
-- [flake8-black](https://pypi.org/project/flake8-black/), to check if the code follows [black](https://black.readthedocs.io/en/stable/) formatting
-- [flake8-docstrings](https://pypi.org/project/flake8-docstrings/), to check that the code is correctly documented
-- [flake8-pytest-style](https://pypi.org/project/flake8-pytest-style/), to check style issues with pytest-based tests
-- [darglint](https://pypi.org/project/darglint/), to check that docstrings match function definitions
+- [Ruff](https://beta.ruff.rs/docs/), an extremely fast linter that support of all main linter rules.
 
 #### Security
 
-- [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/))
-- [Safety](https://pyup.io/safety/), to check if some packages are insecure
+- [Bandit](https://bandit.readthedocs.io/en/latest/), to find security issues (used inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/)).
+- [Safety](https://pyup.io/safety/), to check if some packages are insecure.
 
 #### Formatting
 
-- [black](https://black.readthedocs.io/en/stable/), to format the code
-- [isort](https://pycqa.github.io/isort/index.html), to sort imports
+- [black](https://black.readthedocs.io/en/stable/), to format the code.
+- [isort](https://pycqa.github.io/isort/index.html), to sort imports.
 
 #### Type checking
 
-- [mypy](https://mypy-lang.org/), the classic type checker
-- [typeguard](https://typeguard.readthedocs.io/en/latest/), a runtime type checker
+- [mypy](https://mypy-lang.org/), the classic type checker.
 
 #### Documentation
 
-- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation.
 - [Read the Docs](https://readthedocs.org/), to host the documentation.
-- [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.
-- [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.
-- [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin to detect type hints in generated documentation.
+- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used by the official Python documentation, with:
+  - [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to generate API documentation from the docstrings.
+  - [napoleon](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official plugin to allow compatibility with Google-style docstrings.
+  - [sphinx-autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin to detect type hints in generated documentation.
 
 ### Specific Python tools
 
 Tools to match specific needs of the projet.
 
 #### UI
 
-- [click](https://click.palletsprojects.com/en/8.1.x/), to create CLI applications
+- [click](https://click.palletsprojects.com/en/8.1.x/), to create CLI applications.
 
 #### Communication
 
-- [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests
+- [requests](https://requests.readthedocs.io/en/latest/), to make HTTP requests.
 
 #### Data validation
 
-- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data
+- [marshmallow](https://marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate data.
 
 I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to follow the tutorial, but  [pydantic](https://docs.pydantic.dev/) is more known, and I find it easier to use.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hypermodern-python-tuto Version: 1.0.3 Summary:
+Metadata-Version: 2.1 Name: hypermodern-python-tuto Version: 1.0.4 Summary:
 Repo to follow the Claudio Jolowicz's tutorial about Hypermodern Python (https:
 //cjolowicz.github.io/posts/hypermodern-python-01-setup/) Home-page: https://
 github.com/le-chartreux/hypermodern-python-tuto License: MIT Keywords:
 hypermodern Author: le-chartreux Author-email: le-chartreux-vert@protonmail.com
 Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -28,65 +28,54 @@
 - [Communication](#communication) - [Data validation](#data-validation) ##
 Overview The app created is a CLI application that queries a random Wikipedia
 page and displays its title and summary. ## Install ```shell pip install
 hypermodern-python-tuto ``` ## Use ### Basic usage Just run the following
 command: ```shell hypermodern-python-tuto ``` ### Other options Look at the
 [documentation](https://hypermodern-python-tuto.readthedocs.io/). ## Tools used
 ### Generic tools Tools that can be used in every development project, no
-matter if it's a Python project or not. - [git](https://git-scm.com/), to
-manage versions of the source code - [GitHub](https://github.com/le-chartreux/
-hypermodern-python-tuto), to host the git repository and automate tasks with
-[GitHub Actions](https://docs.github.com/en/actions): - [Release Drafter]
-(https://github.com/marketplace/actions/release-drafter), to create release
-templates - [pre-commit](https://pre-commit.com/), to manage pre-commit hooks -
-[Codecov](https://about.codecov.io/), to mesure code coverage on repos ###
-Generic Python tools Tools that can be used in every Python project, no matter
-its content. #### Multi-purpose - [PyPI](https://pypi.org/), to install and
-publish Python packages - [TestPyPI](https://pypi.org/), PyPI but for testing
-purposes - [poetry](https://python-poetry.org/), to make development and
-distribution easy (packaging, virtualization, dependencies, launching and
-publishing) - [nox](https://nox.thea.codes/en/stable/), to run tasks in
-multiple Python environments (like tests, linting, reformatting, etc.) ####
-Setup - [pyenv](https://github.com/pyenv/pyenv), to manage Python versions ####
-Test - [pytest](https://docs.pytest.org/en/latest/), a framework to write unit
-tests. Also used to run doctests - [pytest-cov](https://pytest-
-cov.readthedocs.io/en/latest/), to mesure the code coverage (degree to which
-the source code of a program is executed while running its test suite) -
-[pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to use the
-[unittest](https://docs.python.org/3/library/unittest.html) mocking in the
-pytest way #### Linting - [flake8](https://flake8.pycqa.org/en/latest/), a
-linter aggregator - [flake8-isort](https://pypi.org/project/flake8-isort/), to
-verify that imports are grouped and ordered in a consistent way - [flake8-
-bugbear](https://github.com/PyCQA/flake8-bugbear), to find bugs and design
-problems - [flake8-annotations](https://pypi.org/project/flake8-annotations/),
-to detect the absence of type annotations - [flake8-black](https://pypi.org/
-project/flake8-black/), to check if the code follows [black](https://
-black.readthedocs.io/en/stable/) formatting - [flake8-docstrings](https://
-pypi.org/project/flake8-docstrings/), to check that the code is correctly
-documented - [flake8-pytest-style](https://pypi.org/project/flake8-pytest-
-style/), to check style issues with pytest-based tests - [darglint](https://
-pypi.org/project/darglint/), to check that docstrings match function
-definitions #### Security - [Bandit](https://bandit.readthedocs.io/en/latest/),
-to find security issues (used inside linting with [flake8-bandit](https://
-pypi.org/project/flake8-bandit/)) - [Safety](https://pyup.io/safety/), to check
-if some packages are insecure #### Formatting - [black](https://
-black.readthedocs.io/en/stable/), to format the code - [isort](https://
-pycqa.github.io/isort/index.html), to sort imports #### Type checking - [mypy]
-(https://mypy-lang.org/), the classic type checker - [typeguard](https://
-typeguard.readthedocs.io/en/latest/), a runtime type checker #### Documentation
-- [Sphinx](https://www.sphinx-doc.org/en/master/), the documentation tool used
-by the official Python documentation. - [Read the Docs](https://
-readthedocs.org/), to host the documentation. - [autodoc](https://www.sphinx-
-doc.org/en/master/usage/extensions/autodoc.html), Sphinx official plugin to
-generate API documentation from the docstrings. - [napoleon](https://
-www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx official
-plugin to allow compatibility with Google-style docstrings. - [sphinx-autodoc-
-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx plugin
-to detect type hints in generated documentation. ### Specific Python tools
-Tools to match specific needs of the projet. #### UI - [click](https://
-click.palletsprojects.com/en/8.1.x/), to create CLI applications ####
+matter if it's a Python project or not. - [Codecov](https://about.codecov.io/),
+to mesure code coverage on repos. I let it in this project since it is already
+setup, but I don't think I will use it in other projects. - [git](https://git-
+scm.com/), to manage versions of the source code. - [GitHub](https://
+github.com/le-chartreux/hypermodern-python-tuto), to host the git repository
+and automate tasks with [GitHub Actions](https://docs.github.com/en/actions): -
+[Release Drafter](https://github.com/marketplace/actions/release-drafter), to
+create release templates. - [pre-commit](https://pre-commit.com/), to manage
+pre-commit hooks. ### Generic Python tools Tools that can be used in every
+Python project, no matter its content. #### Multi-purpose - [nox](https://
+nox.thea.codes/en/stable/), to run tasks in multiple Python environments (like
+tests, linting, reformatting, etc.). - [PyPI](https://pypi.org/), to install
+and publish Python packages. - [poetry](https://python-poetry.org/), to make
+development and distribution easy (packaging, virtualization, dependencies,
+launching and publishing). - [TestPyPI](https://pypi.org/), PyPI but for
+testing purposes. #### Setup - [pyenv](https://github.com/pyenv/pyenv), to
+manage Python versions. #### Test - [pytest](https://docs.pytest.org/en/latest/
+), a framework to write unit tests. Also used to run doctests. - [pytest-cov]
+(https://pytest-cov.readthedocs.io/en/latest/), to mesure the code coverage
+(degree to which the source code of a program is executed while running its
+test suite). - [pytest-mock](https://pytest-mock.readthedocs.io/en/latest/), to
+use the [unittest](https://docs.python.org/3/library/unittest.html) mocking in
+the pytest way. #### Linting - [Ruff](https://beta.ruff.rs/docs/), an extremely
+fast linter that support of all main linter rules. #### Security - [Bandit]
+(https://bandit.readthedocs.io/en/latest/), to find security issues (used
+inside linting with [flake8-bandit](https://pypi.org/project/flake8-bandit/)).
+- [Safety](https://pyup.io/safety/), to check if some packages are insecure.
+#### Formatting - [black](https://black.readthedocs.io/en/stable/), to format
+the code. - [isort](https://pycqa.github.io/isort/index.html), to sort imports.
+#### Type checking - [mypy](https://mypy-lang.org/), the classic type checker.
+#### Documentation - [Read the Docs](https://readthedocs.org/), to host the
+documentation. - [Sphinx](https://www.sphinx-doc.org/en/master/), the
+documentation tool used by the official Python documentation, with: - [autodoc]
+(https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html), Sphinx
+official plugin to generate API documentation from the docstrings. - [napoleon]
+(https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html), Sphinx
+official plugin to allow compatibility with Google-style docstrings. - [sphinx-
+autodoc-typehints](https://pypi.org/project/sphinx-autodoc-typehints/), Sphinx
+plugin to detect type hints in generated documentation. ### Specific Python
+tools Tools to match specific needs of the projet. #### UI - [click](https://
+click.palletsprojects.com/en/8.1.x/), to create CLI applications. ####
 Communication - [requests](https://requests.readthedocs.io/en/latest/), to make
-HTTP requests #### Data validation - [marshmallow](https://
+HTTP requests. #### Data validation - [marshmallow](https://
 marshmallow.readthedocs.io/en/stable/), to serialize, deserialize and validate
-data I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to
+data. I used [marshmallow](https://marshmallow.readthedocs.io/en/stable/) to
 follow the tutorial, but [pydantic](https://docs.pydantic.dev/) is more known,
 and I find it easier to use.
```

