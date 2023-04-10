# Comparing `tmp/saltpeter-0.3.5.tar.gz` & `tmp/saltpeter-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltpeter-0.3.5.tar", last modified: Wed Mar 15 21:00:57 2023, max compression
+gzip compressed data, was "saltpeter-0.3.6.tar", last modified: Mon Apr 10 12:28:07 2023, max compression
```

## Comparing `saltpeter-0.3.5.tar` & `saltpeter-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 marin     (1000) marin     (1000)        0 2023-03-15 21:00:57.511912 saltpeter-0.3.5/
--rw-rw-r--   0 marin     (1000) marin     (1000)      227 2023-03-15 21:00:57.511912 saltpeter-0.3.5/PKG-INFO
--rw-rw-r--   0 marin     (1000) marin     (1000)     2841 2021-03-31 09:08:49.000000 saltpeter-0.3.5/README.md
-drwxrwxr-x   0 marin     (1000) marin     (1000)        0 2023-03-15 21:00:57.511912 saltpeter-0.3.5/saltpeter/
--rw-rw-r--   0 marin     (1000) marin     (1000)       33 2023-02-09 22:19:42.000000 saltpeter-0.3.5/saltpeter/__init__.py
--rw-rw-r--   0 marin     (1000) marin     (1000)     6167 2023-03-13 09:35:10.000000 saltpeter-0.3.5/saltpeter/api.py
--rwxrwxr-x   0 marin     (1000) marin     (1000)    16723 2023-03-15 21:00:15.000000 saltpeter-0.3.5/saltpeter/main.py
--rw-rw-r--   0 marin     (1000) marin     (1000)       22 2023-03-15 21:00:15.000000 saltpeter-0.3.5/saltpeter/version.py
-drwxrwxr-x   0 marin     (1000) marin     (1000)        0 2023-03-15 21:00:57.511912 saltpeter-0.3.5/saltpeter.egg-info/
--rw-rw-r--   0 marin     (1000) marin     (1000)      227 2023-03-15 21:00:57.000000 saltpeter-0.3.5/saltpeter.egg-info/PKG-INFO
--rw-rw-r--   0 marin     (1000) marin     (1000)      328 2023-03-15 21:00:57.000000 saltpeter-0.3.5/saltpeter.egg-info/SOURCES.txt
--rw-rw-r--   0 marin     (1000) marin     (1000)        1 2023-03-15 21:00:57.000000 saltpeter-0.3.5/saltpeter.egg-info/dependency_links.txt
--rw-rw-r--   0 marin     (1000) marin     (1000)       50 2023-03-15 21:00:57.000000 saltpeter-0.3.5/saltpeter.egg-info/entry_points.txt
--rw-rw-r--   0 marin     (1000) marin     (1000)        1 2023-02-09 22:21:37.000000 saltpeter-0.3.5/saltpeter.egg-info/not-zip-safe
--rw-rw-r--   0 marin     (1000) marin     (1000)       42 2023-03-15 21:00:57.000000 saltpeter-0.3.5/saltpeter.egg-info/requires.txt
--rw-rw-r--   0 marin     (1000) marin     (1000)       10 2023-03-15 21:00:57.000000 saltpeter-0.3.5/saltpeter.egg-info/top_level.txt
--rw-rw-r--   0 marin     (1000) marin     (1000)       38 2023-03-15 21:00:57.515913 saltpeter-0.3.5/setup.cfg
--rw-rw-r--   0 marin     (1000) marin     (1000)      623 2023-02-09 22:19:42.000000 saltpeter-0.3.5/setup.py
+drwxrwxr-x   0 marin     (1000) marin     (1000)        0 2023-04-10 12:28:07.078497 saltpeter-0.3.6/
+-rw-rw-r--   0 marin     (1000) marin     (1000)      227 2023-04-10 12:28:07.078497 saltpeter-0.3.6/PKG-INFO
+-rw-rw-r--   0 marin     (1000) marin     (1000)     2841 2021-03-31 09:08:49.000000 saltpeter-0.3.6/README.md
+drwxrwxr-x   0 marin     (1000) marin     (1000)        0 2023-04-10 12:28:07.074496 saltpeter-0.3.6/saltpeter/
+-rw-rw-r--   0 marin     (1000) marin     (1000)       33 2023-02-09 22:19:42.000000 saltpeter-0.3.6/saltpeter/__init__.py
+-rw-rw-r--   0 marin     (1000) marin     (1000)     6167 2023-03-13 09:35:10.000000 saltpeter-0.3.6/saltpeter/api.py
+-rwxrwxr-x   0 marin     (1000) marin     (1000)    17632 2023-04-10 12:27:46.000000 saltpeter-0.3.6/saltpeter/main.py
+-rw-rw-r--   0 marin     (1000) marin     (1000)       22 2023-04-10 12:27:46.000000 saltpeter-0.3.6/saltpeter/version.py
+drwxrwxr-x   0 marin     (1000) marin     (1000)        0 2023-04-10 12:28:07.078497 saltpeter-0.3.6/saltpeter.egg-info/
+-rw-rw-r--   0 marin     (1000) marin     (1000)      227 2023-04-10 12:28:07.000000 saltpeter-0.3.6/saltpeter.egg-info/PKG-INFO
+-rw-rw-r--   0 marin     (1000) marin     (1000)      328 2023-04-10 12:28:07.000000 saltpeter-0.3.6/saltpeter.egg-info/SOURCES.txt
+-rw-rw-r--   0 marin     (1000) marin     (1000)        1 2023-04-10 12:28:07.000000 saltpeter-0.3.6/saltpeter.egg-info/dependency_links.txt
+-rw-rw-r--   0 marin     (1000) marin     (1000)       50 2023-04-10 12:28:07.000000 saltpeter-0.3.6/saltpeter.egg-info/entry_points.txt
+-rw-rw-r--   0 marin     (1000) marin     (1000)        1 2023-02-09 22:21:37.000000 saltpeter-0.3.6/saltpeter.egg-info/not-zip-safe
+-rw-rw-r--   0 marin     (1000) marin     (1000)       56 2023-04-10 12:28:07.000000 saltpeter-0.3.6/saltpeter.egg-info/requires.txt
+-rw-rw-r--   0 marin     (1000) marin     (1000)       10 2023-04-10 12:28:07.000000 saltpeter-0.3.6/saltpeter.egg-info/top_level.txt
+-rw-rw-r--   0 marin     (1000) marin     (1000)       38 2023-04-10 12:28:07.078497 saltpeter-0.3.6/setup.cfg
+-rw-rw-r--   0 marin     (1000) marin     (1000)      651 2023-04-10 12:27:46.000000 saltpeter-0.3.6/setup.py
```

### Comparing `saltpeter-0.3.5/README.md` & `saltpeter-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `saltpeter-0.3.5/saltpeter/api.py` & `saltpeter-0.3.6/saltpeter/api.py`

 * *Files identical despite different names*

### Comparing `saltpeter-0.3.5/saltpeter/main.py` & `saltpeter-0.3.6/saltpeter/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,26 @@
         try:
             #es.indices.create(index=index_name, ignore=400)
             es.index(index=index_name, doc_type='_doc', body=doc, request_timeout=20)
         except Exception as e:
             print("Can't write to elasticsearch", doc)
             print(e)
 
+    if use_opensearch:
+        doc = { 'job_name': cron, "job_instance": instance, '@timestamp': time,
+                'return_code': code, 'machine': machine, 'output': out, 'msg_type': what } 
+        index_name = 'saltpeter-%s' % date.today().strftime('%Y.%m.%d')
+        try:
+            #es.indices.create(index=index_name, ignore=400)
+            opensearch.index(index=index_name, body=doc, request_timeout=20)
+        except Exception as e:
+            #print("Can't write to opensearch", doc)
+            print(e)
+
+
 
 def timeout(which, process):
     global processlist
     if which == 'hard':
         print('Process %s is about to reach hard timeout! It will be killed soon!'\
                 % process.name)
         processlist[process.name]['hard_timeout'] += timedelta(minutes=5)
@@ -345,16 +357,19 @@
 
     parser.add_argument('-p', '--port', type=int, default=8888,\
             help='HTTP api port')
 
     parser.add_argument('-e', '--elasticsearch', default='',\
             help='Elasticsearch host')
 
+    parser.add_argument('-o', '--opensearch', default='',\
+            help='Opensearch host')
+
     parser.add_argument('-i', '--index', default='saltpeter',\
-            help='Elasticsearch index name')
+            help='Elasticsearch/Opensearch index name')
 
     parser.add_argument('-v', '--version', action='store_true' ,\
             help='Print version and exit')
 
     global args
     args = parser.parse_args()
 
@@ -364,14 +379,16 @@
 
 
     global bad_crons
     global bad_files
     global processlist
     global use_es
     use_es = False
+    global use_opensearch
+    use_opensearch = False
     bad_files = []
     last_run = {}
     processlist = {}
 
     manager = multiprocessing.Manager()
     running = manager.dict()
     config = manager.dict()
@@ -386,14 +403,21 @@
 
     if args.elasticsearch != '':
         from elasticsearch import Elasticsearch
         use_es = True
         global es
         es = Elasticsearch(args.elasticsearch,maxsize=50)
 
+    if args.opensearch != '':
+        from opensearchpy import OpenSearch
+        use_opensearch = True
+        global opensearch
+        opensearch = OpenSearch(args.opensearch,maxsize=50,useSSL=False,verify_certs=False)
+
+
     #main loop
     prev = datetime.now(timezone.utc)
 
     while True:
         
         now = datetime.now(timezone.utc)
```

### Comparing `saltpeter-0.3.5/setup.py` & `saltpeter-0.3.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,10 +13,11 @@
           'console_scripts': ['saltpeter=saltpeter.main:main'],
       },
       install_requires=[
           'salt',
           'crontab',
           'pyyaml',
           'tornado',
-          'elasticsearch'
+          'elasticsearch',
+          'opensearch-py',
       ],
       zip_safe=False)
```

