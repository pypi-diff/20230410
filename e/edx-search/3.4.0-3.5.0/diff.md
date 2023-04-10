# Comparing `tmp/edx-search-3.4.0.tar.gz` & `tmp/edx-search-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-search-3.4.0.tar", last modified: Wed May  4 16:32:44 2022, max compression
+gzip compressed data, was "edx-search-3.5.0.tar", last modified: Mon Apr 10 15:16:14 2023, max compression
```

## Comparing `edx-search-3.4.0.tar` & `edx-search-3.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 16:32:44.876675 edx-search-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-04 16:32:34.000000 edx-search-3.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    35135 2022-05-04 16:32:34.000000 edx-search-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-04 16:32:34.000000 edx-search-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-05-04 16:32:44.876675 edx-search-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12186 2022-05-04 16:32:34.000000 edx-search-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 16:32:44.872675 edx-search-3.4.0/edx_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-05-04 16:32:44.000000 edx-search-3.4.0/edx_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-05-04 16:32:44.000000 edx-search-3.4.0/edx_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 16:32:44.000000 edx-search-3.4.0/edx_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-04 16:32:44.000000 edx-search-3.4.0/edx_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-04 16:32:44.000000 edx-search-3.4.0/edx_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 16:32:44.872675 edx-search-3.4.0/edxsearch/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-05-04 16:32:34.000000 edx-search-3.4.0/edxsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-05-04 16:32:34.000000 edx-search-3.4.0/edxsearch/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-05-04 16:32:34.000000 edx-search-3.4.0/edxsearch/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-05-04 16:32:34.000000 edx-search-3.4.0/edxsearch/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 16:32:44.872675 edx-search-3.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-05-04 16:32:34.000000 edx-search-3.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-05-04 16:32:34.000000 edx-search-3.4.0/requirements/testing.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 16:32:44.872675 edx-search-3.4.0/search/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4071 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    22333 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/elastic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/filter_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/initializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6055 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/result_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/search_engine_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 16:32:44.876675 edx-search-3.4.0/search/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14988 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/mock_search_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)    15779 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/test_course_discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     6865 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/test_course_discovery_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     9958 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/test_engines.py
--rw-r--r--   0 runner    (1001) docker     (121)     5009 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/test_mock_search_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)    14297 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/test_search_result_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)    19532 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)    36456 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7137 2022-05-04 16:32:34.000000 edx-search-3.4.0/search/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-04 16:32:44.876675 edx-search-3.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2466 2022-05-04 16:32:34.000000 edx-search-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 15:16:05.000000 edx-search-3.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-04-10 15:16:05.000000 edx-search-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-04-10 15:16:05.000000 edx-search-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      870 2023-04-10 15:16:14.820492 edx-search-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12575 2023-04-10 15:16:05.000000 edx-search-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.816492 edx-search-3.5.0/edx_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      870 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      870 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/edxsearch/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-04-10 15:16:05.000000 edx-search-3.5.0/edxsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-04-10 15:16:05.000000 edx-search-3.5.0/edxsearch/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-04-10 15:16:05.000000 edx-search-3.5.0/edxsearch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-04-10 15:16:05.000000 edx-search-3.5.0/edxsearch/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-04-10 15:16:05.000000 edx-search-3.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-10 15:16:05.000000 edx-search-3.5.0/requirements/testing.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/search/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22812 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/filter_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6055 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/result_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/search_engine_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/search/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14988 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/mock_search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15779 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_course_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_course_discovery_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10533 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_engines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_mock_search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14297 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_search_result_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20485 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7137 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 15:16:14.824492 edx-search-3.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2470 2023-04-10 15:16:05.000000 edx-search-3.5.0/setup.py
```

### Comparing `edx-search-3.4.0/LICENSE` & `edx-search-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/PKG-INFO` & `edx-search-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-search
-Version: 3.4.0
+Version: 3.5.0
 Summary: Search and index routines for index access
-Home-page: https://github.com/edx/edx-search
+Home-page: https://github.com/openedx/edx-search
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `edx-search-3.4.0/README.md` & `edx-search-3.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# edx-search [![Build Status](https://github.com/edx/edx-search/workflows/Python%20CI/badge.svg?branch=master)](https://github.com/edx/edx-search/actions?query=workflow%3A%22Python+CI%22) [![Coverage Status](https://coveralls.io/repos/edx/edx-search/badge.svg?branch=master&service=github)](https://coveralls.io/github/edx/edx-search?branch=master)
+# edx-search [![Build Status](https://github.com/openedx/edx-search/workflows/Python%20CI/badge.svg?branch=master)](https://github.com/openedx/edx-search/actions?query=workflow%3A%22Python+CI%22) [![Coverage Status](https://coveralls.io/repos/edx/edx-search/badge.svg?branch=master&service=github)](https://coveralls.io/github/edx/edx-search?branch=master)
 
 This is a django application to provide access to search services from within edx-platform applications.
 
 Searching is accomplished by creating an index of documents, and then searching within that index for matching information. This application provides a way to add documents to the index, and then search for them.
 
 ## SearchEngine
 The SearchEngine is an abstract object which may have multiple implementations _(at the time of writing there are 2 in existence - Elasticsearch and MockSearchEngine, which is primarily used for testing)_
@@ -30,14 +30,23 @@
 
 1. `index` - the operation to add a document to the index
 
 2. `remove` - the operation to remove a document from the index
 
 3. `search` - the operation to find matching documents within the index. `doc_type` is supported as an optional keyword parameter to return results only with a certain doc_type
 
+## Configuring for multi-tenancy
+
+The modules exposes a setting `ELASTIC_SEARCH_INDEX_PREFIX` to enable so that the indices for multiple clients do not collide.
+
+```python
+SearchEngine(index_name="test")
+```
+
+When invoked, this line will create an index named `test` on Elastic Search. Setting `ELASTIC_SEARCH_INDEX_PREFIX="client1_"` will instead create the index `client1_test`.
 
 ## Index documents
 Index documents are passed to the search application as python dictionaries, along with a `doc_type` document type, which is also optionally supported as a way to return only certain document types from a search.
 
 ### Example indexing operation
 ```
 search_engine = SearchEngine.get_search_engine(index="test_index")
```

### Comparing `edx-search-3.4.0/edx_search.egg-info/PKG-INFO` & `edx-search-3.5.0/edx_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-search
-Version: 3.4.0
+Version: 3.5.0
 Summary: Search and index routines for index access
-Home-page: https://github.com/edx/edx-search
+Home-page: https://github.com/openedx/edx-search
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `edx-search-3.4.0/edx_search.egg-info/SOURCES.txt` & `edx-search-3.5.0/edx_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/edxsearch/settings.py` & `edx-search-3.5.0/edxsearch/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,23 +49,25 @@
 INSTALLED_APPS = (
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
+    'waffle',
 )
 
 MIDDLEWARE = (
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
+    'waffle.middleware.WaffleMiddleware',
 )
 
 ROOT_URLCONF = 'search.urls'
 
 WSGI_APPLICATION = 'edxsearch.wsgi.application'
```

### Comparing `edx-search-3.4.0/requirements/base.in` & `edx-search-3.5.0/requirements/base.in`

 * *Files 19% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 #
 
 -c constraints.txt
 
 
 Django                       # Web application framework
 elasticsearch>=7.8.0,<8.0.0
+edx-toggles
 event-tracking
```

### Comparing `edx-search-3.4.0/search/api.py` & `edx-search-3.5.0/search/api.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/elastic.py` & `edx-search-3.5.0/search/elastic.py`

 * *Files 4% similar despite different names*

```diff
@@ -300,41 +300,54 @@
             }
         }
 
         We cache the properties of each index, if they are not available,
         we'll load them again from Elasticsearch
         """
         # Try loading the mapping from the cache.
-        mapping = ElasticSearchEngine.get_mappings(self.index_name)
+        mapping = ElasticSearchEngine.get_mappings(self._prefixed_index_name)
 
         # Fall back to Elasticsearch
         if not mapping:
             mapping = self._es.indices.get_mapping(
-                index=self.index_name
-            ).get(self.index_name, {}).get("mappings", {})
+                index=self._prefixed_index_name
+            ).get(self._prefixed_index_name, {}).get("mappings", {})
             # Cache the mapping, if one was retrieved
             if mapping:
-                ElasticSearchEngine.set_mappings(self.index_name, mapping)
+                ElasticSearchEngine.set_mappings(self._prefixed_index_name, mapping)
 
         return mapping
 
     def _clear_mapping(self):
         """
         Remove the cached mappings.
 
         Next time ES mappings is are requested.
         """
-        ElasticSearchEngine.set_mappings(self.index_name, {})
+        ElasticSearchEngine.set_mappings(self._prefixed_index_name, {})
 
     def __init__(self, index=None):
         super().__init__(index)
         es_config = getattr(settings, "ELASTIC_SEARCH_CONFIG", [{}])
         self._es = getattr(settings, "ELASTIC_SEARCH_IMPL", Elasticsearch)(es_config)
-        if not self._es.indices.exists(index=self.index_name):
-            self._es.indices.create(index=self.index_name)
+        params = None
+
+        if not self._es.indices.exists(index=self._prefixed_index_name):
+            self._es.indices.create(index=self._prefixed_index_name, params=params)
+
+    @property
+    def _prefixed_index_name(self):
+        """
+        Property that returns the defined index_name with the configured
+        prefix.
+
+        To be used anywhere the index_name is required.
+        """
+        prefix = getattr(settings, "ELASTIC_SEARCH_INDEX_PREFIX", "")
+        return prefix + self.index_name
 
     def _check_mappings(self, body):
         """
         Put mapping to the index.
 
         We desire to index content so that anything we want to be textually
         searchable(and therefore needing to be analysed), but the other fields
@@ -392,17 +405,18 @@
         new_properties = {
             field: field_property(field, value)
             for field, value in body.items()
             if (field not in exclude_fields) and (field not in self.mappings.get("properties", {}))
         }
 
         if new_properties:
+
             self._es.indices.put_mapping(
-                index=self.index_name,
-                body={"properties": new_properties}
+                index=self._prefixed_index_name,
+                body={"properties": new_properties},
             )
             self._clear_mapping()
 
     def index(self, sources, **kwargs):
         """
         Implements call to add documents to the ES index.
 
@@ -413,15 +427,15 @@
         try:
             actions = []
             for source in sources:
                 self._check_mappings(source)
                 id_ = source.get("id")
                 log.debug("indexing object with id %s", id_)
                 action = {
-                    "_index": self.index_name,
+                    "_index": self._prefixed_index_name,
                     "_id": id_,
                     "_source": source
                 }
                 actions.append(action)
             # bulk() returns a tuple with summary information
             # number of successfully executed actions and number of errors
             # if stats_only is set to True.
@@ -433,22 +447,21 @@
             log.exception("Error during ES bulk operation.")
             raise
 
     def remove(self, doc_ids, **kwargs):
         """
         Implements call to remove the documents from the index
         """
-
         try:
             actions = []
             for doc_id in doc_ids:
                 log.debug("Removing document with id %s", doc_id)
                 action = {
                     "_op_type": "delete",
-                    "_index": self.index_name,
+                    "_index": self._prefixed_index_name,
                     "_id": doc_id
                 }
                 actions.append(action)
             bulk(self._es, actions, **kwargs)
         except BulkIndexError as ex:
             valid_errors = [error for error in ex.errors if error["delete"]["status"] != 404]
 
@@ -564,15 +577,14 @@
                 {
 
                 }
             )
         """
 
         log.debug("searching index with %s", query_string)
-
         elastic_queries = []
         elastic_filters = []
 
         # We have a query string, search all fields for matching text
         # within the "content" node
         if query_string:
             query_string = query_string.translate(
@@ -638,13 +650,13 @@
                 }
 
         body = {"query": query}
         if aggregation_terms:
             body["aggs"] = _process_aggregation_terms(aggregation_terms)
 
         try:
-            es_response = self._es.search(index=self.index_name, body=body, **kwargs)
+            es_response = self._es.search(index=self._prefixed_index_name, body=body, **kwargs)
         except exceptions.ElasticsearchException as ex:
             log.exception("error while searching index - %r", ex)
             raise
 
         return _translate_hits(es_response)
```

### Comparing `edx-search-3.4.0/search/filter_generator.py` & `edx-search-3.5.0/search/filter_generator.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/initializer.py` & `edx-search-3.5.0/search/initializer.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/result_processor.py` & `edx-search-3.5.0/search/result_processor.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/tests/mock_search_engine.py` & `edx-search-3.5.0/search/tests/mock_search_engine.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/tests/test_course_discovery.py` & `edx-search-3.5.0/search/tests/test_course_discovery.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/tests/test_course_discovery_views.py` & `edx-search-3.5.0/search/tests/test_course_discovery_views.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/tests/test_engines.py` & `edx-search-3.5.0/search/tests/test_engines.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,43 @@
 # error, but they do get used when included as part of the override_settings
 # pylint: disable=too-few-public-methods
 """ Tests for search functionality """
 
 import json
 import os
 from datetime import datetime
-
 from unittest.mock import patch
+
 from django.test import TestCase
 from django.test.utils import override_settings
 from elasticsearch import exceptions
 from elasticsearch.helpers import BulkIndexError
-
-from search.api import perform_search, NoSearchEngineError
+from search.api import NoSearchEngineError, perform_search
 from search.elastic import RESERVED_CHARACTERS
-from search.tests.mock_search_engine import MockSearchEngine, json_date_to_datetime
+from search.tests.mock_search_engine import (MockSearchEngine,
+                                             json_date_to_datetime)
 from search.tests.tests import MockSearchTests
-from search.tests.utils import ErroringElasticImpl, SearcherMixin
+from search.tests.utils import (TEST_INDEX_NAME, ErroringElasticImpl,
+                                SearcherMixin)
+
+
+@override_settings(ELASTIC_SEARCH_INDEX_PREFIX='prefixed_')
+@override_settings(SEARCH_ENGINE="search.tests.utils.ForceRefreshElasticSearchEngine")
+class ElasticSearchPrefixTests(MockSearchTests):
+    """
+    Override that runs the same tests for ElasticSearchTests,
+    but with a prefixed index name.
+    """
+
+    @property
+    def index_name(self):
+        """
+        The search index name to be used for this test.
+        """
+        return f"prefixed_{TEST_INDEX_NAME}"
 
 
 @override_settings(SEARCH_ENGINE="search.tests.utils.ForceRefreshElasticSearchEngine")
 class ElasticSearchTests(MockSearchTests):
     """ Override that runs the same tests for ElasticSearchEngine instead of MockSearchEngine """
 
     def test_reserved_characters(self):
```

### Comparing `edx-search-3.4.0/search/tests/test_mock_search_engine.py` & `edx-search-3.5.0/search/tests/test_mock_search_engine.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/tests/test_search_result_processor.py` & `edx-search-3.5.0/search/tests/test_search_result_processor.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/tests/test_views.py` & `edx-search-3.5.0/search/tests/test_views.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 from datetime import datetime
 from unittest.mock import patch, call
 import ddt
 
 from django.urls import Resolver404, resolve
 from django.test import TestCase
 from django.test.utils import override_settings
+from waffle.testutils import override_switch
 
 from search.search_engine_base import SearchEngine
+from search.search_engine_base import DEFAULT_ELASTIC_SEARCH_SWITCH
+from search.elastic import ElasticSearchEngine
 from search.tests.mock_search_engine import MockSearchEngine
-from search.tests.tests import TEST_INDEX_NAME
-from search.tests.utils import post_request, SearcherMixin
+from search.tests.utils import post_request, SearcherMixin, TEST_INDEX_NAME
 
 
 # Any class that inherits from TestCase will cause too-many-public-methods pylint error
 # pylint: disable=too-many-public-methods
 @override_settings(SEARCH_ENGINE="search.tests.mock_search_engine.MockSearchEngine")
 @override_settings(ELASTIC_FIELD_MAPPINGS={"start_date": {"type": "date"}})
 @override_settings(COURSEWARE_CONTENT_INDEX_NAME=TEST_INDEX_NAME)
@@ -352,14 +354,15 @@
         self.assertTrue("error" in results)
 
 
 @override_settings(SEARCH_ENGINE="search.tests.utils.ErroringSearchEngine")
 @override_settings(ELASTIC_FIELD_MAPPINGS={"start_date": {"type": "date"}})
 @override_settings(COURSEWARE_CONTENT_INDEX_NAME=TEST_INDEX_NAME)
 @override_settings(COURSEWARE_INFO_INDEX_NAME=TEST_INDEX_NAME)
+@override_switch(DEFAULT_ELASTIC_SEARCH_SWITCH, active=False)
 class BadSearchTest(TestCase, SearcherMixin):
     """ Make sure that we can error message when there is a problem """
 
     def setUp(self):
         super().setUp()
         MockSearchEngine.destroy()
 
@@ -396,14 +399,15 @@
         self.assertEqual(results["error"], 'An error occurred when searching for "sun"')
 
         with self.assertRaises(Exception):
             searcher.search(query_string="test search")
 
 
 @override_settings(SEARCH_ENGINE="search.tests.utils.ErroringIndexEngine")
+@override_switch(DEFAULT_ELASTIC_SEARCH_SWITCH, active=False)
 class BadIndexTest(TestCase, SearcherMixin):
     """ Make sure that we can error message when there is a problem """
 
     def setUp(self):
         super().setUp()
         MockSearchEngine.destroy()
 
@@ -414,14 +418,34 @@
     def test_search_from_url(self):
         """ ensure that we get the error back when the backend fails """
         searcher = SearchEngine.get_search_engine(TEST_INDEX_NAME)
         with self.assertRaises(Exception):
             searcher.index([{"id": "FAKE_ID_3", "content": {"text": "Here comes the sun"}}])
 
 
+@override_settings(SEARCH_ENGINE="nonexistentengine")
+@override_switch(DEFAULT_ELASTIC_SEARCH_SWITCH, active=True)
+class DefaultElasticSearchSwitchTest(TestCase, SearcherMixin):
+    """ When the DEFAULT_ELASTIC_SEARCH_SWITCH is enabled,
+    make sure ElasticSearch is used by default. """
+
+    def setUp(self):
+        super().setUp()
+        MockSearchEngine.destroy()
+
+    def tearDown(self):
+        MockSearchEngine.destroy()
+        super().tearDown()
+
+    def test_search_with_switch(self):
+        """ ensure we use ElasticSearch when the switch is on """
+        searcher = SearchEngine.get_search_engine(TEST_INDEX_NAME)
+        self.assertTrue(isinstance(searcher, ElasticSearchEngine))
+
+
 @override_settings(SEARCH_ENGINE="search.tests.utils.ForceRefreshElasticSearchEngine")
 @override_settings(ELASTIC_FIELD_MAPPINGS={"start_date": {"type": "date"}})
 @override_settings(COURSEWARE_CONTENT_INDEX_NAME=TEST_INDEX_NAME)
 @override_settings(COURSEWARE_INFO_INDEX_NAME=TEST_INDEX_NAME)
 @ddt.ddt
 class ElasticSearchUrlTest(TestCase, SearcherMixin):
     """
```

### Comparing `edx-search-3.4.0/search/tests/tests.py` & `edx-search-3.5.0/search/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,43 +23,51 @@
 # Any class that inherits from TestCase will cause too-many-public-methods pylint error
 # pylint: disable=too-many-public-methods
 @override_settings(SEARCH_ENGINE="search.tests.mock_search_engine.MockSearchEngine")
 @override_settings(ELASTIC_FIELD_MAPPINGS={"start_date": {"type": "date"}})
 @override_settings(MOCK_SEARCH_BACKING_FILE=None)
 class MockSearchTests(TestCase, SearcherMixin):
     """ Test operation of search activities """
+
+    @property
+    def index_name(self):
+        """
+        The search index name to be used for this test.
+        """
+        return TEST_INDEX_NAME
+
     @property
     def _is_elastic(self):
         """ check search engine implementation, to manage cleanup differently """
         return isinstance(self.searcher, ElasticSearchEngine)
 
     def setUp(self):
         super().setUp()
         # ignore unexpected-keyword-arg; ES python client documents that it can be used
         # pylint: disable=unexpected-keyword-arg
         if self._is_elastic:
             _elasticsearch = Elasticsearch()
             # Make sure that we are fresh
-            _elasticsearch.indices.delete(index=TEST_INDEX_NAME, ignore=[400, 404])
+            _elasticsearch.indices.delete(index=self.index_name, ignore=[400, 404])
 
             config_body = {}
             # ignore unexpected-keyword-arg; ES python client documents that it can be used
-            _elasticsearch.indices.create(index=TEST_INDEX_NAME, ignore=400, body=config_body)
+            _elasticsearch.indices.create(index=self.index_name, ignore=400, body=config_body)
         else:
             MockSearchEngine.destroy()
         self._searcher = None
         cache.clear()
 
     def tearDown(self):
         # ignore unexpected-keyword-arg; ES python client documents that it can be used
         # pylint: disable=unexpected-keyword-arg
         if self._is_elastic:
             _elasticsearch = Elasticsearch()
             # ignore unexpected-keyword-arg; ES python client documents that it can be used
-            _elasticsearch.indices.delete(index=TEST_INDEX_NAME, ignore=[400, 404])
+            _elasticsearch.indices.delete(index=self.index_name, ignore=[400, 404])
         else:
             MockSearchEngine.destroy()
 
         self._searcher = None
         super().tearDown()
 
     def test_factory_creator(self):
```

### Comparing `edx-search-3.4.0/search/tests/utils.py` & `edx-search-3.5.0/search/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/urls.py` & `edx-search-3.5.0/search/urls.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/utils.py` & `edx-search-3.5.0/search/utils.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/search/views.py` & `edx-search-3.5.0/search/views.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.4.0/setup.py` & `edx-search-3.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 setup(
     name='edx-search',
     version=VERSION,
     description='Search and index routines for index access',
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/edx-search',
+    url='https://github.com/openedx/edx-search',
     license='AGPL',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
```

