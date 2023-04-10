# Comparing `tmp/ansys-sphinx-theme-0.9.6.tar.gz` & `tmp/ansys-sphinx-theme-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-sphinx-theme-0.9.6.tar", last modified: Fri Mar 31 09:30:04 2023, max compression
+gzip compressed data, was "ansys-sphinx-theme-0.9.7.tar", last modified: Mon Apr 10 08:29:28 2023, max compression
```

## Comparing `ansys-sphinx-theme-0.9.6.tar` & `ansys-sphinx-theme-0.9.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1089 2023-03-31 09:29:41.872072 ansys-sphinx-theme-0.9.6/LICENSE
--rw-r--r--   0        0        0     4224 2023-03-31 09:29:41.872072 ansys-sphinx-theme-0.9.6/README.rst
--rw-r--r--   0        0        0     2175 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     3919 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/__init__.py
--rw-r--r--   0        0        0       78 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/examples/__init__.py
--rw-r--r--   0        0        0      726 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/examples/sample_func.py
--rw-r--r--   0        0        0     6335 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/examples/samples.py
--rw-r--r--   0        0        0      755 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/examples/type_hint_example.py
--rw-r--r--   0        0        0      423 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/latex/404.html
--rw-r--r--   0        0        0     2432 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/latex/__init__.py
--rw-r--r--   0        0        0     4523 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/latex/cover.tex
--rw-r--r--   0        0        0      102 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      606 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      391 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/announcement_version.html
--rw-r--r--   0        0        0      237 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0        0        0     2560 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html
--rw-r--r--   0        0        0     1183 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html
--rw-r--r--   0        0        0      175 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/404.rst
--rw-r--r--   0        0        0      327 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys-favicon.png
--rw-r--r--   0        0        0    45165 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg
--rw-r--r--   0        0        0    50754 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg
--rw-r--r--   0        0        0     4788 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf
--rw-r--r--   0        0        0     4503 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf
--rw-r--r--   0        0        0    19674 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css
--rw-r--r--   0        0        0     1133 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css
--rw-r--r--   0        0        0     2626 2023-03-31 09:29:41.876073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css
--rw-r--r--   0        0        0   268588 2023-03-31 09:29:41.880073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf
--rw-r--r--   0        0        0   269108 2023-03-31 09:29:41.880073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf
--rw-r--r--   0        0        0   268280 2023-03-31 09:29:41.884073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf
--rw-r--r--   0        0        0      227 2023-03-31 09:29:41.884073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/download_target_blank.js
--rw-r--r--   0        0        0       76 2023-03-31 09:29:41.884073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/table.js
--rw-r--r--   0        0        0    64600 2023-03-31 09:29:41.884073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0    62063 2023-03-31 09:29:41.884073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png
--rw-r--r--   0        0        0    66106 2023-03-31 09:29:41.884073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png
--rw-r--r--   0        0        0    36194 2023-03-31 09:29:41.884073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png
--rw-r--r--   0        0        0    63718 2023-03-31 09:29:41.888073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png
--rw-r--r--   0        0        0    33524 2023-03-31 09:29:41.888073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png
--rw-r--r--   0        0        0     1729 2023-03-31 09:29:41.888073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf
--rw-r--r--   0        0        0      326 2023-03-31 09:29:41.888073 ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/theme.conf
--rw-r--r--   0        0        0     5624 1970-01-01 00:00:00.000000 ansys-sphinx-theme-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-10 08:29:14.208554 ansys-sphinx-theme-0.9.7/LICENSE
+-rw-r--r--   0        0        0     4224 2023-04-10 08:29:14.208554 ansys-sphinx-theme-0.9.7/README.rst
+-rw-r--r--   0        0        0     2175 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     3919 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/__init__.py
+-rw-r--r--   0        0        0      726 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/sample_func.py
+-rw-r--r--   0        0        0     6335 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/samples.py
+-rw-r--r--   0        0        0      755 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/type_hint_example.py
+-rw-r--r--   0        0        0      423 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/404.html
+-rw-r--r--   0        0        0     2432 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/__init__.py
+-rw-r--r--   0        0        0     4523 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/cover.tex
+-rw-r--r--   0        0        0      102 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      606 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      391 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/announcement_version.html
+-rw-r--r--   0        0        0      237 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0        0        0     2560 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html
+-rw-r--r--   0        0        0     1183 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html
+-rw-r--r--   0        0        0      175 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/404.rst
+-rw-r--r--   0        0        0      327 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys-favicon.png
+-rw-r--r--   0        0        0    45165 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg
+-rw-r--r--   0        0        0    50754 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg
+-rw-r--r--   0        0        0     4788 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf
+-rw-r--r--   0        0        0     4503 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf
+-rw-r--r--   0        0        0    19674 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css
+-rw-r--r--   0        0        0     1133 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css
+-rw-r--r--   0        0        0     2626 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css
+-rw-r--r--   0        0        0   268588 2023-04-10 08:29:14.216554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf
+-rw-r--r--   0        0        0   269108 2023-04-10 08:29:14.216554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf
+-rw-r--r--   0        0        0   268280 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf
+-rw-r--r--   0        0        0      227 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/download_target_blank.js
+-rw-r--r--   0        0        0       76 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/table.js
+-rw-r--r--   0        0        0    54761 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0    54600 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png
+-rw-r--r--   0        0        0    54836 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png
+-rw-r--r--   0        0        0    32456 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png
+-rw-r--r--   0        0        0    54325 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png
+-rw-r--r--   0        0        0    31713 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png
+-rw-r--r--   0        0        0     1729 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf
+-rw-r--r--   0        0        0      326 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/theme.conf
+-rw-r--r--   0        0        0     5624 1970-01-01 00:00:00.000000 ansys-sphinx-theme-0.9.7/PKG-INFO
```

### Comparing `ansys-sphinx-theme-0.9.6/LICENSE` & `ansys-sphinx-theme-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/README.rst` & `ansys-sphinx-theme-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/pyproject.toml` & `ansys-sphinx-theme-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/__init__.py` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 from typing import Dict
 
 from sphinx.application import Sphinx
 
 from ansys_sphinx_theme.latex import generate_404  # noqa: F401
 
-__version__ = "0.9.6"
+__version__ = "0.9.7"
 
 # Declare the fundamental paths of the theme
 THIS_PATH = pathlib.Path(__file__).parent.resolve()
 THEME_PATH = THIS_PATH / "theme" / "ansys_sphinx_theme"
 STATIC_PATH = THEME_PATH / "static"
 STYLE_PATH = STATIC_PATH / "css"
 JS_PATH = STATIC_PATH / "js"
```

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/examples/sample_func.py` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/sample_func.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/examples/samples.py` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/samples.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/examples/type_hint_example.py` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/type_hint_example.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/latex/__init__.py` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/latex/cover.tex` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/cover.tex`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf` & `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.6/PKG-INFO` & `ansys-sphinx-theme-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-sphinx-theme
-Version: 0.9.6
+Version: 0.9.7
 Summary: A theme devised by ANSYS, Inc. for Sphinx documentation.
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx
```

