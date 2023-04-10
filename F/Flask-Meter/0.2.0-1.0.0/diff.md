# Comparing `tmp/Flask-Meter-0.2.0.tar.gz` & `tmp/Flask-Meter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Meter-0.2.0.tar", last modified: Thu Apr 26 02:27:08 2018, max compression
+gzip compressed data, was "Flask-Meter-1.0.0.tar", last modified: Mon Apr 10 14:07:10 2023, max compression
```

## Comparing `Flask-Meter-0.2.0.tar` & `Flask-Meter-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/
--rw-rw-r--   0 herman    (1000) herman    (1000)      264 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/MANIFEST.in
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/docs/
--rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/make.bat
--rw-rw-r--   0 herman    (1000) herman    (1000)       77 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/usage.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      282 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/index.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       27 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/readme.rst
--rwxrwxr-x   0 herman    (1000) herman    (1000)     8459 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/conf.py
--rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/Makefile
--rw-rw-r--   0 herman    (1000) herman    (1000)       33 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/contributing.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/authors.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/history.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/docs/installation.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     2077 2018-04-26 01:55:57.000000 Flask-Meter-0.2.0/README.rst
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/Flask_Meter.egg-info/
--rw-rw-r--   0 herman    (1000) herman    (1000)      525 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/Flask_Meter.egg-info/SOURCES.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)       12 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/Flask_Meter.egg-info/top_level.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)        1 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/Flask_Meter.egg-info/dependency_links.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)     3784 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/Flask_Meter.egg-info/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)        1 2018-04-17 03:53:06.000000 Flask-Meter-0.2.0/Flask_Meter.egg-info/not-zip-safe
--rw-rw-r--   0 herman    (1000) herman    (1000)      161 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/AUTHORS.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      454 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/setup.cfg
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/tests/
--rw-rw-r--   0 herman    (1000) herman    (1000)     2082 2018-04-18 02:23:36.000000 Flask-Meter-0.2.0/tests/test_flask_meter.py
--rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2018-04-17 03:06:44.000000 Flask-Meter-0.2.0/LICENSE
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/flask_meter/
--rw-rw-r--   0 herman    (1000) herman    (1000)      154 2018-04-18 02:23:36.000000 Flask-Meter-0.2.0/flask_meter/__init__.py
--rw-rw-r--   0 herman    (1000) herman    (1000)     1247 2018-04-18 02:23:36.000000 Flask-Meter-0.2.0/flask_meter/flask_meter.py
--rw-rw-r--   0 herman    (1000) herman    (1000)      713 2018-04-18 02:23:36.000000 Flask-Meter-0.2.0/flask_meter/git.py
--rw-rw-r--   0 herman    (1000) herman    (1000)      223 2018-04-26 01:57:05.000000 Flask-Meter-0.2.0/HISTORY.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     3784 2018-04-26 02:27:08.000000 Flask-Meter-0.2.0/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)     1302 2018-04-18 02:23:36.000000 Flask-Meter-0.2.0/setup.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      156 2023-04-10 07:49:10.000000 Flask-Meter-1.0.0/AUTHORS.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      313 2023-04-10 06:49:10.000000 Flask-Meter-1.0.0/HISTORY.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/LICENSE
+-rw-rw-r--   0 herman    (1000) herman    (1000)      264 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/MANIFEST.in
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3514 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2085 2023-04-10 13:44:14.000000 Flask-Meter-1.0.0/README.rst
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/docs/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/Makefile
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.524392 Flask-Meter-1.0.0/docs/_build/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.524392 Flask-Meter-1.0.0/docs/_build/html/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/docs/_build/html/_static/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      286 2023-04-10 12:45:48.000000 Flask-Meter-1.0.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/authors.rst
+-rwxrwxr-x   0 herman    (1000) herman    (1000)     8585 2023-04-10 13:26:44.000000 Flask-Meter-1.0.0/docs/conf.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)       33 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/contributing.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      479 2023-04-10 14:06:54.000000 Flask-Meter-1.0.0/docs/flask_meter.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/history.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      298 2023-04-10 11:47:36.000000 Flask-Meter-1.0.0/docs/index.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/installation.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/make.bat
+-rw-rw-r--   0 herman    (1000) herman    (1000)       70 2023-04-10 14:06:54.000000 Flask-Meter-1.0.0/docs/modules.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       27 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/readme.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      420 2023-04-10 11:51:37.000000 Flask-Meter-1.0.0/docs/usage.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1724 2023-04-10 14:06:24.000000 Flask-Meter-1.0.0/pyproject.toml
+-rw-rw-r--   0 herman    (1000) herman    (1000)       69 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/setup.cfg
+-rw-rw-r--   0 herman    (1000) herman    (1000)       38 2023-04-10 08:04:42.000000 Flask-Meter-1.0.0/setup.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.524392 Flask-Meter-1.0.0/src/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3514 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)      713 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/SOURCES.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)        1 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/dependency_links.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/requires.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/top_level.txt
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/src/flask_meter/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      109 2023-04-10 13:09:47.000000 Flask-Meter-1.0.0/src/flask_meter/__init__.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1446 2023-04-10 13:09:59.000000 Flask-Meter-1.0.0/src/flask_meter/flask_meter.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)      742 2023-04-10 07:53:30.000000 Flask-Meter-1.0.0/src/flask_meter/git.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/tests/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2191 2023-04-10 13:12:53.000000 Flask-Meter-1.0.0/tests/test_flask_meter.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-Meter-0.2.0/docs/make.bat` & `Flask-Meter-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-Meter-0.2.0/docs/conf.py` & `Flask-Meter-1.0.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,260 +16,263 @@
 import sys
 import os
 
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # Get the project root dir, which is the parent dir of this
 cwd = os.getcwd()
 project_root = os.path.dirname(cwd)
 
 # Insert the project root dir as the first element in the PYTHONPATH.
 # This lets us ensure that the source package is imported, and that its
 # version is used.
-sys.path.insert(0, project_root)
+sys.path.insert(0, os.path.abspath(os.path.join("..", "src")))
 
 import flask_meter
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'Flask-Meter'
-copyright = u"2017, Herman Paul Singh"
+project = "Flask-Meter"
+copyright = "2017, Herman Paul Singh"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = flask_meter.__version__
 # The full version, including alpha/beta/rc tags.
 release = flask_meter.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to
 # some non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built
 # documents.
-#keep_warnings = False
+# keep_warnings = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = "default"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as
 # html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the
 # top of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon
 # of the docs.  This file should be a Windows icon file (.ico) being
 # 16x16 or 32x32 pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets)
 # here, relative to this directory. They are copied after the builtin
 # static files, so a file named "default.css" will overwrite the builtin
 # "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page
 # bottom, using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names
 # to template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer.
 # Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer.
 # Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages
 # will contain a <link> tag referring to it.  The value of this option
 # must be the base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'flask_meterdoc'
+htmlhelp_basename = "flask_meterdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto/manual]).
 latex_documents = [
-    ('index', 'flask_meter.tex',
-     u'Flask-Meter Documentation',
-     u'Herman Paul Singh', 'manual'),
+    (
+        "index",
+        "flask_meter.tex",
+        "Flask-Meter Documentation",
+        "Herman Paul Singh",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at
 # the top of the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings
 # are parts, not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'flask_meter',
-     u'Flask-Meter Documentation',
-     [u'Herman Paul Singh'], 1)
+    ("index", "flask_meter", "Flask-Meter Documentation", ["Herman Paul Singh"], 1)
 ]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    ('index', 'flask_meter',
-     u'Flask-Meter Documentation',
-     u'Herman Paul Singh',
-     'flask_meter',
-     'One line description of project.',
-     'Miscellaneous'),
+    (
+        "index",
+        "flask_meter",
+        "Flask-Meter Documentation",
+        "Herman Paul Singh",
+        "flask_meter",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
```

### Comparing `Flask-Meter-0.2.0/docs/Makefile` & `Flask-Meter-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Meter-0.2.0/docs/installation.rst` & `Flask-Meter-1.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-0.2.0/CONTRIBUTING.rst` & `Flask-Meter-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-0.2.0/README.rst` & `Flask-Meter-1.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 ===============================
 Flask-Meter
 ===============================
+Healthchecks for Flask
+
+.. image:: https://img.shields.io/pypi/v/Flask-Meter.svg
+        :target: https://pypi.python.org/pypi/Flask-Meter
+
+.. image:: https://tc.spin-flip.com/app/rest/builds/buildType:id:FlaskMeter_TestPython310/statusIcon.svg
+        :target: https://tc.spin-flip.com/project/FlaskMeter?mode=trends
+
+.. image:: https://readthedocs.org/projects/Flask-Meter/badge/?version=latest
+        :target: https://Flask-Meter.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://codecov.io/gh/Kartstig/flask-meter/branch/master/graph/badge.svg?token=NsmixA2iCH
+        :target: https://codecov.io/gh/Kartstig/flask-meter
 
 Flask-Meter is an add-on to the Flask web framework. Flask-Meter adds a
 monitoring endpoint for consuming application metrics. It can be really simple
 to set up. Flask-Meter modifies the Flask application to provide an enpoint
 at `/_health` where you will get a JSON response of the system's uptime,
 current git revision.
 
@@ -12,15 +26,16 @@
 constructor.
 
 Installing
 ----------
 
 Install and update using `pip`:
 .. code-block:: text
-  pip install -U Flask-Meter
+
+    pip install -U Flask-Meter
 
 Flask Configuration
 -------------------
 
 .. code-block:: python
 
   from Flask import Flask
@@ -38,32 +53,14 @@
     from flask_meter import FlaskMeter
 
     app = Flask(__name__)
 
     flask_meter = FlaskMeter()
     flask_meter.init_app(app)
 
-.. image:: https://travis-ci.org/Kartstig/flask-meter.svg?branch=master
-        :target: https://travis-ci.org/Kartstig/flask-meter
-
-.. image:: https://img.shields.io/travis/KartStig/flask_meter.svg
-        :target: https://travis-ci.org/Kartstig/flask-meter
-
-.. image:: https://readthedocs.org/projects/flask-meter/badge/?version=latest
-        :target: https://flask-meter.readthedocs.io
-        :alt: Documentation Status
-
-.. image:: https://pyup.io/repos/github/KartStig/flask_meter/shield.svg
-     :target: https://pyup.io/repos/github/KartStig/flask_meter/
-     :alt: Updates
-
-
-Flask-Meter adds a monitoring endpoint for consuming application host metrics.
-
-
 * Free software: MIT license
 * Documentation: https://flask-meter.readthedocs.io.
 
 
 Features
 --------
```

### Comparing `Flask-Meter-0.2.0/Flask_Meter.egg-info/SOURCES.txt` & `Flask-Meter-1.0.0/src/Flask_Meter.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
-Flask_Meter.egg-info/PKG-INFO
-Flask_Meter.egg-info/SOURCES.txt
-Flask_Meter.egg-info/dependency_links.txt
-Flask_Meter.egg-info/not-zip-safe
-Flask_Meter.egg-info/top_level.txt
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
+docs/flask_meter.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
+docs/modules.rst
 docs/readme.rst
 docs/usage.rst
-flask_meter/__init__.py
-flask_meter/flask_meter.py
-flask_meter/git.py
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
+src/Flask_Meter.egg-info/PKG-INFO
+src/Flask_Meter.egg-info/SOURCES.txt
+src/Flask_Meter.egg-info/dependency_links.txt
+src/Flask_Meter.egg-info/requires.txt
+src/Flask_Meter.egg-info/top_level.txt
+src/flask_meter/__init__.py
+src/flask_meter/flask_meter.py
+src/flask_meter/git.py
 tests/test_flask_meter.py
```

### Comparing `Flask-Meter-0.2.0/LICENSE` & `Flask-Meter-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Meter-0.2.0/flask_meter/flask_meter.py` & `Flask-Meter-1.0.0/src/flask_meter/flask_meter.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,38 +4,44 @@
 
 from .git import git_stats
 
 FuncList = List[Callable]
 
 
 class FlaskMeter(object):
+    def __init__(self, app: flask.Flask = None, extra_checks: FuncList = []) -> None:
+        if app is not None:
+            self.init_app(app, extra_checks)
+
+    def init_app(self, app: flask.Flask, extra_checks: list = []):
+        if not isinstance(app, flask.Flask):
+            raise TypeError("Not a Flask Application")
+
+        self.app = app
+        self.app.config["FLASK_METER_ENABLE"] = self.app.config.get(
+            "FLASK_METER_ENABLE", True
+        )
+        self.app.config["FLASK_METER_GIT"] = self.app.config.get(
+            "FLASK_METER_GIT", True
+        )
+        self.start_time = datetime.now()
+
+        def _health():
+            data = {
+                "status": "OK",
+                "uptime": str(datetime.now() - self.start_time),
+                "app": self.app.name,
+            }
+
+            if extra_checks:
+                extra_results = {
+                    func.__doc__: "OK" if func() else "DOWN" for func in extra_checks
+                }
+                data.update(extra_results)
 
-  def __init__(self, app: flask.Flask=None, extra_checks: FuncList=[]) -> None:
-    if app is not None:
-      self.init_app(app, extra_checks)
-
-  def init_app(self, app: flask.Flask, extra_checks: list=[]):
-    if not isinstance(app, flask.Flask):
-      raise TypeError("Not a Flask Application")
-
-    self.app = app
-    self.app.config['FLASK_METER_ENABLE'] = self.app.config.get('FLASK_METER_ENABLE', True)
-    self.app.config['FLASK_METER_GIT'] = self.app.config.get('FLASK_METER_GIT', True)
-    self.start_time = datetime.now()
-
-    def _health():
-      data = {"status": "OK",
-              "uptime": str(datetime.now() - self.start_time),
-              "app": self.app.name}
-
-      if extra_checks:
-        extra_results = {func.__doc__: "OK" if func() else "DOWN"
-                         for func in extra_checks}
-        data.update(extra_results)
+            if self.app.config["FLASK_METER_GIT"]:
+                data.update({"git": git_stats()})
 
-      if self.app.config['FLASK_METER_GIT']:
-        data.update({"git": git_stats()})
+            return flask.jsonify(data)
 
-      return flask.jsonify(data)
-
-    if self.app.config['FLASK_METER_ENABLE']:
-      self.app.add_url_rule('/_health', '_health', _health)
+        if self.app.config["FLASK_METER_ENABLE"]:
+            self.app.add_url_rule("/_health", "_health", _health)
```

### Comparing `Flask-Meter-0.2.0/flask_meter/git.py` & `Flask-Meter-1.0.0/src/flask_meter/git.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import re
 import subprocess
 
 
-GIT_CMD = 'git log | head -4'
-RE_COMMIT = re.compile(r'commit[\W]+(\w+)', re.MULTILINE)
-RE_AUTHOR = re.compile(r'Author\:[\W]+(.*)', re.MULTILINE)
-RE_DATE = re.compile(r'Date\:[\W]+(.*)', re.MULTILINE)
+GIT_CMD = "git log | head -4"
+RE_COMMIT = re.compile(r"commit[\W]+(\w+)", re.MULTILINE)
+RE_AUTHOR = re.compile(r"Author\:[\W]+(.*)", re.MULTILINE)
+RE_DATE = re.compile(r"Date\:[\W]+(.*)", re.MULTILINE)
 
 
 def git_stats():
-  try:
-    ret = subprocess.check_output([GIT_CMD], shell=True)\
-                    .decode('utf-8')
-    commit = re.search(RE_COMMIT, ret)
-    author = re.search(RE_AUTHOR, ret)
-    date = re.search(RE_DATE, ret)
-    return {"commit": commit.group(1) if commit else "Unknown",
+    try:
+        ret = subprocess.check_output([GIT_CMD], shell=True).decode("utf-8")
+        commit = re.search(RE_COMMIT, ret)
+        author = re.search(RE_AUTHOR, ret)
+        date = re.search(RE_DATE, ret)
+        return {
+            "commit": commit.group(1) if commit else "Unknown",
             "author": author.group(1) if author else "Unknown",
-            "date": date.group(1) if date else "Unknown"}
-  except subprocess.CalledProcessError:
-    return {"Error"}
+            "date": date.group(1) if date else "Unknown",
+        }
+    except subprocess.CalledProcessError:
+        return {"Error"}
```

