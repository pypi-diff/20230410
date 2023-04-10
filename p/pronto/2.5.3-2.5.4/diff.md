# Comparing `tmp/pronto-2.5.3.tar.gz` & `tmp/pronto-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pronto-2.5.3.tar", last modified: Wed Jan 11 13:07:42 2023, max compression
+gzip compressed data, was "pronto-2.5.4.tar", last modified: Mon Apr 10 17:49:17 2023, max compression
```

## Comparing `pronto-2.5.3.tar` & `pronto-2.5.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:42.129743 pronto-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-01-11 13:07:32.000000 pronto-2.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-11 13:07:32.000000 pronto-2.5.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-11 13:07:32.000000 pronto-2.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-01-11 13:07:42.129743 pronto-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-01-11 13:07:32.000000 pronto-2.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:42.125743 pronto-2.5.3/pronto/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:42.129743 pronto-2.5.3/pronto/entity/
--rw-r--r--   0 runner    (1001) docker     (123)    24215 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/entity/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:42.129743 pronto-2.5.3/pronto/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/logic/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    20624 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:42.129743 pronto-2.5.3/pronto/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/parsers/_fastobo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/parsers/obo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/parsers/obojson.py
--rw-r--r--   0 runner    (1001) docker     (123)    36581 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/parsers/rdfxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/relationship.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:42.129743 pronto-2.5.3/pronto/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/serializers/_fastobo.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/serializers/obo.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/serializers/obojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/serializers/ofn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/synonym.py
--rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/term.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:42.129743 pronto-2.5.3/pronto/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/utils/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-01-11 13:07:32.000000 pronto-2.5.3/pronto/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:07:42.129743 pronto-2.5.3/pronto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-01-11 13:07:42.000000 pronto-2.5.3/pronto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-01-11 13:07:42.000000 pronto-2.5.3/pronto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 13:07:42.000000 pronto-2.5.3/pronto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-11 13:07:42.000000 pronto-2.5.3/pronto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-11 13:07:42.000000 pronto-2.5.3/pronto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 13:07:42.000000 pronto-2.5.3/pronto.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-11 13:07:42.129743 pronto-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-11 13:07:32.000000 pronto-2.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:17.030093 pronto-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-04-10 17:49:05.000000 pronto-2.5.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 17:49:05.000000 pronto-2.5.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-10 17:49:05.000000 pronto-2.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-04-10 17:49:17.030093 pronto-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-04-10 17:49:05.000000 pronto-2.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:17.026093 pronto-2.5.4/pronto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:17.026093 pronto-2.5.4/pronto/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)    24216 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/entity/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:17.026093 pronto-2.5.4/pronto/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/logic/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20624 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:17.026093 pronto-2.5.4/pronto/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/parsers/_fastobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/parsers/obo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/parsers/obojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36581 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/parsers/rdfxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/relationship.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:17.030093 pronto-2.5.4/pronto/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/serializers/_fastobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/serializers/obo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/serializers/obojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/serializers/ofn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/synonym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/term.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:17.030093 pronto-2.5.4/pronto/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/utils/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-10 17:49:05.000000 pronto-2.5.4/pronto/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:49:17.026093 pronto-2.5.4/pronto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-04-10 17:49:17.000000 pronto-2.5.4/pronto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-10 17:49:17.000000 pronto-2.5.4/pronto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:49:17.000000 pronto-2.5.4/pronto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 17:49:17.000000 pronto-2.5.4/pronto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 17:49:17.000000 pronto-2.5.4/pronto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:49:17.000000 pronto-2.5.4/pronto.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-10 17:49:17.030093 pronto-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 17:49:05.000000 pronto-2.5.4/setup.py
```

### Comparing `pronto-2.5.3/CHANGELOG.md` & `pronto-2.5.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/pronto/compare/v2.5.3...HEAD
+[Unreleased]: https://github.com/althonos/pronto/compare/v2.5.4...HEAD
+
+## [v2.5.4] - 2023-04-10
+[v2.5.4]: https://github.com/althonos/pronto/compare/v2.5.3...v2.5.4
+### Fixed
+- `Entity.synonyms` setter not accepting `frozenset` arguments as expected (#207).
+### Changed
+- Bump supported `networkx` version to `v3.0` (#206).
 
 ## [v2.5.3]
 [v2.5.3]: https://github.com/althonos/pronto/compare/v2.5.2...v2.5.3
 ### Fixed
 - Crash in `LineageIterator.to_set` when starting from an empty set of entities.
 
 ## [v2.5.2] - 2022-12-07
```

### Comparing `pronto-2.5.3/COPYING` & `pronto-2.5.4/COPYING`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/PKG-INFO` & `pronto-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pronto
-Version: 2.5.3
+Version: 2.5.4
 Summary: Python frontend to ontologies.
 Home-page: https://github.com/althonos/pronto
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/pronto/issues
 Project-URL: Changelog, https://pronto.readthedocs.io/en/latest/changes.html
```

### Comparing `pronto-2.5.3/README.md` & `pronto-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/__init__.py` & `pronto-2.5.4/pronto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     LiteralPropertyValue.__name__,
     ResourcePropertyValue.__name__,
     Xref.__name__,
 ]
 
 __author__ = "Martin Larralde <martin.larralde@embl.de>"
 __license__ = "MIT"
-__version__ = "2.5.3"
+__version__ = "2.5.4"
 
 # Update the docstring with a link to the right version of the documentation
 # instead of the latest.
 if __doc__ is not None:
     __doc__ += f"""See Also:
     Online documentation for this version of the library on
     `Read The Docs <https://pronto.readthedocs.io/en/v{__version__}/>`_
```

### Comparing `pronto-2.5.3/pronto/definition.py` & `pronto-2.5.4/pronto/definition.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/entity/__init__.py` & `pronto-2.5.4/pronto/entity/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
     def synonyms(self) -> FrozenSet[Synonym]:
         """`frozenset` of `Synonym`: A set of synonyms for this entity."""
         ontology, termdata = self._ontology(), self._data()
         return frozenset(Synonym(ontology, s) for s in termdata.synonyms)
 
     @synonyms.setter  # type: ignore
     @typechecked(property=True)
-    def synonyms(self, synonyms: Iterable[Synonym]):
+    def synonyms(self, synonyms: FrozenSet[Synonym]):
         self._data().synonyms = {syn._data() for syn in synonyms}
 
     @property
     def union_of(self) -> _S:
         s = self._Set()
         s._ids = self._data().union_of
         s._ontology = self._ontology()
```

### Comparing `pronto-2.5.3/pronto/entity/attributes.py` & `pronto-2.5.4/pronto/entity/attributes.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/logic/lineage.py` & `pronto-2.5.4/pronto/logic/lineage.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/metadata.py` & `pronto-2.5.4/pronto/metadata.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/ontology.py` & `pronto-2.5.4/pronto/ontology.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/parsers/_fastobo.py` & `pronto-2.5.4/pronto/parsers/_fastobo.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/parsers/base.py` & `pronto-2.5.4/pronto/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/parsers/obo.py` & `pronto-2.5.4/pronto/parsers/obo.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/parsers/obojson.py` & `pronto-2.5.4/pronto/parsers/obojson.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/parsers/rdfxml.py` & `pronto-2.5.4/pronto/parsers/rdfxml.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/pv.py` & `pronto-2.5.4/pronto/pv.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/relationship.py` & `pronto-2.5.4/pronto/relationship.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/serializers/_fastobo.py` & `pronto-2.5.4/pronto/serializers/_fastobo.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/serializers/obo.py` & `pronto-2.5.4/pronto/serializers/obo.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/synonym.py` & `pronto-2.5.4/pronto/synonym.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/term.py` & `pronto-2.5.4/pronto/term.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/utils/io.py` & `pronto-2.5.4/pronto/utils/io.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/utils/iter.py` & `pronto-2.5.4/pronto/utils/iter.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/utils/meta.py` & `pronto-2.5.4/pronto/utils/meta.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/utils/warnings.py` & `pronto-2.5.4/pronto/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto/xref.py` & `pronto-2.5.4/pronto/xref.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/pronto.egg-info/PKG-INFO` & `pronto-2.5.4/pronto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pronto
-Version: 2.5.3
+Version: 2.5.4
 Summary: Python frontend to ontologies.
 Home-page: https://github.com/althonos/pronto
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/pronto/issues
 Project-URL: Changelog, https://pronto.readthedocs.io/en/latest/changes.html
```

### Comparing `pronto-2.5.3/pronto.egg-info/SOURCES.txt` & `pronto-2.5.4/pronto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pronto-2.5.3/setup.cfg` & `pronto-2.5.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 	pronto.serializers
 test_suite = tests
 setup_requires = 
 	setuptools >=46.4
 install_requires = 
 	chardet ~=5.0
 	fastobo ~=0.12.2
-	networkx ~=2.3
+	networkx >=2.3,<4.0
 	python-dateutil ~=2.8
 
 [options.package_data]
 pronto = py.typed
 
 [sdist]
 formats = zip
```

