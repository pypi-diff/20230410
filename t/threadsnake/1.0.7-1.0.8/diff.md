# Comparing `tmp/threadsnake-1.0.7.tar.gz` & `tmp/threadsnake-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsnake-1.0.7.tar", last modified: Sun Apr  9 21:47:02 2023, max compression
+gzip compressed data, was "threadsnake-1.0.8.tar", last modified: Mon Apr 10 00:03:51 2023, max compression
```

## Comparing `threadsnake-1.0.7.tar` & `threadsnake-1.0.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.567297 threadsnake-1.0.7/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-04-07 19:56:48.000000 threadsnake-1.0.7/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-04-07 21:41:56.000000 threadsnake-1.0.7/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      860 2023-04-09 21:47:02.567297 threadsnake-1.0.7/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       86 2023-04-07 21:41:56.000000 threadsnake-1.0.7/README.MD
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-04-07 19:56:48.000000 threadsnake-1.0.7/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-09 21:47:02.567297 threadsnake-1.0.7/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1152 2023-04-08 03:17:13.000000 threadsnake-1.0.7/setup.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.543296 threadsnake-1.0.7/src/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.555297 threadsnake-1.0.7/src/threadsnake/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.555297 threadsnake-1.0.7/src/threadsnake/html/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/html/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      595 2023-04-08 13:22:26.000000 threadsnake-1.0.7/src/threadsnake/html/tools.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.555297 threadsnake-1.0.7/src/threadsnake/http/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2407 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/application.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.559297 threadsnake-1.0.7/src/threadsnake/http/core/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/common.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1059 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/constants.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4060 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/httprequest.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     5898 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/httpresponse.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/httpserver.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     3112 2023-04-08 12:09:56.000000 threadsnake-1.0.7/src/threadsnake/http/core/server.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1272 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/session.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.559297 threadsnake-1.0.7/src/threadsnake/http/core/values/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       79 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/values/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      404 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/values/contenttypes.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2203 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/core/values/responsecodes.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.563297 threadsnake-1.0.7/src/threadsnake/http/middlewares/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      370 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/app.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1626 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/authorization.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1379 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/bodyparser.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      334 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/cors.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1340 2023-04-09 21:44:08.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/defaultheaders.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      679 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/jsonbodyparser.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4038 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/multipartformdataparser.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1970 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/requests.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/session.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1451 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/static.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      469 2023-04-09 21:44:08.000000 threadsnake-1.0.7/src/threadsnake/http/middlewares/timemeassure.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4916 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/router.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.563297 threadsnake-1.0.7/src/threadsnake/http/tools/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/tools/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1202 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/tools/common.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2919 2023-04-09 13:45:07.000000 threadsnake-1.0.7/src/threadsnake/http/tools/routing.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1342 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/http/types.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.567297 threadsnake-1.0.7/src/threadsnake/turbo/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      199 2023-04-07 19:56:48.000000 threadsnake-1.0.7/src/threadsnake/turbo/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.555297 threadsnake-1.0.7/src/threadsnake.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      860 2023-04-09 21:47:02.000000 threadsnake-1.0.7/src/threadsnake.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1694 2023-04-09 21:47:02.000000 threadsnake-1.0.7/src/threadsnake.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-04-09 21:47:02.000000 threadsnake-1.0.7/src/threadsnake.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       12 2023-04-09 21:47:02.000000 threadsnake-1.0.7/src/threadsnake.egg-info/top_level.txt
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 21:47:02.567297 threadsnake-1.0.7/tests/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      645 2023-04-09 21:44:08.000000 threadsnake-1.0.7/tests/test_get_app_authorization_middleware.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1562 2023-04-09 21:44:08.000000 threadsnake-1.0.7/tests/test_get_request_middlewares.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-04-09 21:46:55.000000 threadsnake-1.0.7/version.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.502133 threadsnake-1.0.8/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-04-07 19:56:48.000000 threadsnake-1.0.8/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-04-07 21:41:56.000000 threadsnake-1.0.8/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     5042 2023-04-10 00:03:51.502133 threadsnake-1.0.8/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4268 2023-04-10 00:03:44.000000 threadsnake-1.0.8/README.MD
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-04-07 19:56:48.000000 threadsnake-1.0.8/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-10 00:03:51.502133 threadsnake-1.0.8/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1152 2023-04-08 03:17:13.000000 threadsnake-1.0.8/setup.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.482132 threadsnake-1.0.8/src/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.486132 threadsnake-1.0.8/src/threadsnake/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.490132 threadsnake-1.0.8/src/threadsnake/html/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/html/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      595 2023-04-08 13:22:26.000000 threadsnake-1.0.8/src/threadsnake/html/tools.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.490132 threadsnake-1.0.8/src/threadsnake/http/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2407 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/application.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.490132 threadsnake-1.0.8/src/threadsnake/http/core/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/common.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1059 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/constants.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4060 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/httprequest.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     5898 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/httpresponse.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/httpserver.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     3112 2023-04-08 12:09:56.000000 threadsnake-1.0.8/src/threadsnake/http/core/server.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1272 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/session.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.490132 threadsnake-1.0.8/src/threadsnake/http/core/values/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       79 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/values/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      404 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/values/contenttypes.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2203 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/core/values/responsecodes.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.494132 threadsnake-1.0.8/src/threadsnake/http/middlewares/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      370 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/app.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1626 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/authorization.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1379 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/bodyparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      334 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/cors.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1340 2023-04-09 21:44:08.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/defaultheaders.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      679 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/jsonbodyparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4038 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/multipartformdataparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1970 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/requests.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/session.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1451 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/static.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      469 2023-04-09 21:44:08.000000 threadsnake-1.0.8/src/threadsnake/http/middlewares/timemeassure.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4916 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/router.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.494132 threadsnake-1.0.8/src/threadsnake/http/tools/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/tools/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1202 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/tools/common.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2919 2023-04-09 13:45:07.000000 threadsnake-1.0.8/src/threadsnake/http/tools/routing.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1342 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/http/types.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.494132 threadsnake-1.0.8/src/threadsnake/turbo/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      199 2023-04-07 19:56:48.000000 threadsnake-1.0.8/src/threadsnake/turbo/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.490132 threadsnake-1.0.8/src/threadsnake.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     5042 2023-04-10 00:03:51.000000 threadsnake-1.0.8/src/threadsnake.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1694 2023-04-10 00:03:51.000000 threadsnake-1.0.8/src/threadsnake.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-04-10 00:03:51.000000 threadsnake-1.0.8/src/threadsnake.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       12 2023-04-10 00:03:51.000000 threadsnake-1.0.8/src/threadsnake.egg-info/top_level.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 00:03:51.502133 threadsnake-1.0.8/tests/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      645 2023-04-09 21:44:08.000000 threadsnake-1.0.8/tests/test_get_app_authorization_middleware.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1562 2023-04-09 21:44:08.000000 threadsnake-1.0.8/tests/test_get_request_middlewares.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-04-10 00:03:44.000000 threadsnake-1.0.8/version.txt
```

### Comparing `threadsnake-1.0.7/LICENSE` & `threadsnake-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/setup.py` & `threadsnake-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/html/tools.py` & `threadsnake-1.0.8/src/threadsnake/html/tools.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/application.py` & `threadsnake-1.0.8/src/threadsnake/http/application.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/core/common.py` & `threadsnake-1.0.8/src/threadsnake/http/core/common.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/core/constants.py` & `threadsnake-1.0.8/src/threadsnake/http/core/constants.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/core/httprequest.py` & `threadsnake-1.0.8/src/threadsnake/http/core/httprequest.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/core/httpresponse.py` & `threadsnake-1.0.8/src/threadsnake/http/core/httpresponse.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/core/httpserver.py` & `threadsnake-1.0.8/src/threadsnake/http/core/httpserver.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/core/server.py` & `threadsnake-1.0.8/src/threadsnake/http/core/server.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/core/session.py` & `threadsnake-1.0.8/src/threadsnake/http/core/session.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/core/values/responsecodes.py` & `threadsnake-1.0.8/src/threadsnake/http/core/values/responsecodes.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/middlewares/authorization.py` & `threadsnake-1.0.8/src/threadsnake/http/middlewares/authorization.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/middlewares/bodyparser.py` & `threadsnake-1.0.8/src/threadsnake/http/middlewares/bodyparser.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/middlewares/defaultheaders.py` & `threadsnake-1.0.8/src/threadsnake/http/middlewares/defaultheaders.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/middlewares/jsonbodyparser.py` & `threadsnake-1.0.8/src/threadsnake/http/middlewares/jsonbodyparser.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/middlewares/multipartformdataparser.py` & `threadsnake-1.0.8/src/threadsnake/http/middlewares/multipartformdataparser.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/middlewares/requests.py` & `threadsnake-1.0.8/src/threadsnake/http/middlewares/requests.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/middlewares/session.py` & `threadsnake-1.0.8/src/threadsnake/http/middlewares/session.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/middlewares/static.py` & `threadsnake-1.0.8/src/threadsnake/http/middlewares/static.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/router.py` & `threadsnake-1.0.8/src/threadsnake/http/router.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/tools/common.py` & `threadsnake-1.0.8/src/threadsnake/http/tools/common.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/tools/routing.py` & `threadsnake-1.0.8/src/threadsnake/http/tools/routing.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake/http/types.py` & `threadsnake-1.0.8/src/threadsnake/http/types.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/src/threadsnake.egg-info/SOURCES.txt` & `threadsnake-1.0.8/src/threadsnake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/tests/test_get_app_authorization_middleware.py` & `threadsnake-1.0.8/tests/test_get_app_authorization_middleware.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.7/tests/test_get_request_middlewares.py` & `threadsnake-1.0.8/tests/test_get_request_middlewares.py`

 * *Files identical despite different names*

