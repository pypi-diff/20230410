# Comparing `tmp/pywebio-1.7.1.tar.gz` & `tmp/pywebio-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywebio-1.7.1.tar", last modified: Sun Dec 11 10:33:06 2022, max compression
+gzip compressed data, was "dist/pywebio-1.8.0.tar", last modified: Mon Apr 10 13:53:47 2023, max compression
```

## Comparing `pywebio-1.7.1.tar` & `pywebio-1.8.0.tar`

### file list

```diff
@@ -1,101 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-11 10:32:30.000000 pywebio-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2022-12-11 10:33:06.000000 pywebio-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2022-12-11 10:32:30.000000 pywebio-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/demos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/bmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/bokeh_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/chat_room.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/doc_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/gomoku_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/input_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/markdown_previewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/output_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/set_env_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13864 2022-12-11 10:32:30.000000 pywebio-1.7.1/demos/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/html/codemirror/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/codemirror/active-line.js
--rw-r--r--   0 runner    (1001) docker     (123)    29098 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/codemirror/addons.js
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/codemirror/autorefresh.js
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/codemirror/loadmode.js
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/codemirror/matchbrackets.js
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/codemirror/python.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/html/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/app.css
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/bootstrap-select.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/html/css/bs-theme/
--rw-r--r--   0 runner    (1001) docker     (123)   183536 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/bs-theme/dark.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   162100 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/bs-theme/default.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   166623 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/bs-theme/minty.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   167654 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/bs-theme/sketchy.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   169188 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/bs-theme/yeti.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/codemirror.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16294 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/markdown.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/css/toastify.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/html/image/
--rwxr-xr-x   0 runner    (1001) docker     (123)      265 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/image/favicon_closed_16.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      513 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/image/favicon_closed_32.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      251 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/image/favicon_open_16.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      466 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/image/favicon_open_32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/html/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2611 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/FileSaver.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    53596 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/bootstrap-select.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    60010 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/bs-custom-file-input.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   169793 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/codemirror.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    88145 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/jquery.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    11143 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/mustache.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    74085 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/prism.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17886 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/purify.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   117073 2022-12-11 10:32:54.000000 pywebio-1.7.1/pywebio/html/js/pywebio.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/require.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/html/js/toastify.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    36083 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/io_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (123)    75048 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/pin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/platform/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/platform/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/adaptor/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/adaptor/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/path_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/remote_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    18507 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/tornado_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/platform/tpl/
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/tpl/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/platform/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio/session/
--rw-r--r--   0 runner    (1001) docker     (123)    21572 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/session/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/session/coroutinebased.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/session/threadbased.py
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2022-12-11 10:32:30.000000 pywebio-1.7.1/pywebio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/pywebio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2022-12-11 10:33:04.000000 pywebio-1.7.1/pywebio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2022-12-11 10:33:05.000000 pywebio-1.7.1/pywebio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 10:33:04.000000 pywebio-1.7.1/pywebio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2022-12-11 10:33:04.000000 pywebio-1.7.1/pywebio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-11 10:33:04.000000 pywebio-1.7.1/pywebio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-11 10:33:06.000000 pywebio-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2022-12-11 10:32:30.000000 pywebio-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:33:06.000000 pywebio-1.7.1/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2022-12-11 10:32:30.000000 pywebio-1.7.1/tools/pywebio-path-deploy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 13:53:12.000000 pywebio-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-10 13:53:47.000000 pywebio-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-10 13:53:12.000000 pywebio-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/bmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/bokeh_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/chat_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/doc_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/gomoku_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/input_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/markdown_previewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/output_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/set_env_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-04-10 13:53:12.000000 pywebio-1.8.0/demos/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/html/codemirror/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/codemirror/active-line.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/codemirror/addons.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/codemirror/autorefresh.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/codemirror/loadmode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/codemirror/matchbrackets.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/codemirror/python.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/html/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/bootstrap-select.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/html/css/bs-theme/
+-rw-r--r--   0 runner    (1001) docker     (123)   183536 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/bs-theme/dark.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   162100 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/bs-theme/default.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   166623 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/bs-theme/minty.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   167654 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/bs-theme/sketchy.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   169188 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/bs-theme/yeti.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/codemirror.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/markdown.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/css/toastify.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/html/image/
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/image/apple-touch-icon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      265 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/image/favicon_closed_16.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/image/favicon_closed_32.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      251 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/image/favicon_open_16.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/image/favicon_open_32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/html/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2611 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/FileSaver.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    53596 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/bootstrap-select.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60010 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/bs-custom-file-input.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   169793 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/codemirror.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    88145 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/jquery.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11143 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/mustache.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74085 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/prism.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17886 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/purify.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   129471 2023-04-10 13:53:36.000000 pywebio-1.8.0/pywebio/html/js/pywebio.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/require.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/html/js/toastify.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    37649 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/io_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92960 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/pin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/platform/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15561 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/adaptor/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/adaptor/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/path_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/platform/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/pyinstaller/hook-pywebio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/remote_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18817 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/tornado_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/platform/tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/tpl/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/platform/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/session/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/session/coroutinebased.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/session/threadbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-04-10 13:53:12.000000 pywebio-1.8.0/pywebio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 13:53:47.000000 pywebio-1.8.0/pywebio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 13:53:47.000000 pywebio-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-10 13:53:12.000000 pywebio-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:53:47.000000 pywebio-1.8.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-10 13:53:12.000000 pywebio-1.8.0/tools/pywebio-path-deploy
```

### Comparing `pywebio-1.7.1/PKG-INFO` & `pywebio-1.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio
-Version: 1.7.1
+Version: 1.8.0
 Summary: Write interactive web app in script way.
 Home-page: https://pywebio.readthedocs.io
 Author: WangWeimin
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io
 Project-URL: Source, https://github.com/wang0618/PyWebIO
@@ -28,25 +28,19 @@
             <a href="https://pypi.org/project/PyWebIO/">
                 <img src="https://img.shields.io/pypi/v/pywebio?colorB=brightgreen" alt="Package version">
             </a>
             <a href="https://pypi.org/project/PyWebIO/">
                 <img src="https://img.shields.io/badge/python->%3D%203.5.2-brightgreen" alt="Python Version">
             </a>
             <br/>
-            <a href="https://lgtm.com/projects/g/wang0618/PyWebIO/context:python">
-                <img src="https://img.shields.io/lgtm/grade/python/github/wang0618/PyWebIO.svg?colorB=brightgreen" alt="Python code quality">
-            </a>
-            <a href="https://lgtm.com/projects/g/wang0618/PyWebIO/context:javascript">
-                <img src="https://img.shields.io/lgtm/grade/javascript/github/wang0618/PyWebIO.svg?colorB=brightgreen" alt="Javascript code quality">
-            </a>
             <a href="https://github.com/wang0618/PyWebIO/blob/master/LICENSE">
                 <img src="https://img.shields.io/github/license/wang0618/PyWebIO.svg" alt="License">
             </a>
             <br/>
-            <a href="https://pywebio.readthedocs.io">[Document]</a> | <a href="http://pywebio-demos.pywebio.online/">[Demos]</a> | <a href="https://github.com/wang0618/PyWebIO/wiki/Why-PyWebIO%3F">[Why PyWebIO?]</a>
+            <a href="https://pywebio.readthedocs.io">[Document]</a> | <a href="http://pywebio-demos.pywebio.online/">[Demos]</a> | <a href="https://play.pywebio.online">[Playground]</a> | <a href="https://github.com/wang0618/PyWebIO/wiki/Why-PyWebIO%3F">[Why PyWebIO?]</a>
         </p>
         
         [English](README.md) | [中文](README-zh.md)
         
         PyWebIO provides a series of imperative functions to obtain user input and output on the browser, turning the browser into a "rich text terminal", and can be used to build simple web applications or browser-based GUI applications without the need to have knowledge of HTML and JS. PyWebIO can also be easily integrated into existing Web services. PyWebIO is very suitable for quickly building applications that do not require complex UI.
         
         <p align="center">
@@ -70,15 +64,15 @@
         
         ```bash
         pip3 install -U pywebio
         ```
         
         Development version:
         ```bash
-        pip3 install -U https://code.aliyun.com/wang0618/pywebio/repository/archive.zip
+        pip3 install -U https://github.com/pywebio/PyWebIO/archive/dev-release.zip
         ```
         
         **Prerequisites**: PyWebIO requires Python 3.5.2 or newer
         
         ## Quickstart
         
         **Hello, world**
@@ -159,18 +153,18 @@
         For integration with other web frameworks, please refer to [document](https://pywebio.readthedocs.io/en/latest/advanced.html#integration-with-web-framework).
         
         ## Demos
         
          - [Basic demo](http://pywebio-demos.pywebio.online/) : PyWebIO basic input and output demos and some small applications written using PyWebIO.
          - [Data visualization demo](http://pywebio-charts.pywebio.online/) : Data visualization with the third-party libraries, e.g., `plotly`, `bokeh`, `pyecharts`.
         
-        ## Document
-        
-        Document is on [https://pywebio.readthedocs.io](https://pywebio.readthedocs.io)
+        ## Links
         
+        * Document [pywebio.readthedocs.io](https://pywebio.readthedocs.io)
+        * [PyWebIO Playground](https://play.pywebio.online/): Edit, Run, Share PyWebIO Code Online
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5.2
```

### Comparing `pywebio-1.7.1/README.md` & `pywebio-1.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,25 +18,19 @@
     <a href="https://pypi.org/project/PyWebIO/">
         <img src="https://img.shields.io/pypi/v/pywebio?colorB=brightgreen" alt="Package version">
     </a>
     <a href="https://pypi.org/project/PyWebIO/">
         <img src="https://img.shields.io/badge/python->%3D%203.5.2-brightgreen" alt="Python Version">
     </a>
     <br/>
-    <a href="https://lgtm.com/projects/g/wang0618/PyWebIO/context:python">
-        <img src="https://img.shields.io/lgtm/grade/python/github/wang0618/PyWebIO.svg?colorB=brightgreen" alt="Python code quality">
-    </a>
-    <a href="https://lgtm.com/projects/g/wang0618/PyWebIO/context:javascript">
-        <img src="https://img.shields.io/lgtm/grade/javascript/github/wang0618/PyWebIO.svg?colorB=brightgreen" alt="Javascript code quality">
-    </a>
     <a href="https://github.com/wang0618/PyWebIO/blob/master/LICENSE">
         <img src="https://img.shields.io/github/license/wang0618/PyWebIO.svg" alt="License">
     </a>
     <br/>
-    <a href="https://pywebio.readthedocs.io">[Document]</a> | <a href="http://pywebio-demos.pywebio.online/">[Demos]</a> | <a href="https://github.com/wang0618/PyWebIO/wiki/Why-PyWebIO%3F">[Why PyWebIO?]</a>
+    <a href="https://pywebio.readthedocs.io">[Document]</a> | <a href="http://pywebio-demos.pywebio.online/">[Demos]</a> | <a href="https://play.pywebio.online">[Playground]</a> | <a href="https://github.com/wang0618/PyWebIO/wiki/Why-PyWebIO%3F">[Why PyWebIO?]</a>
 </p>
 
 [English](README.md) | [中文](README-zh.md)
 
 PyWebIO provides a series of imperative functions to obtain user input and output on the browser, turning the browser into a "rich text terminal", and can be used to build simple web applications or browser-based GUI applications without the need to have knowledge of HTML and JS. PyWebIO can also be easily integrated into existing Web services. PyWebIO is very suitable for quickly building applications that do not require complex UI.
 
 <p align="center">
@@ -60,15 +54,15 @@
 
 ```bash
 pip3 install -U pywebio
 ```
 
 Development version:
 ```bash
-pip3 install -U https://code.aliyun.com/wang0618/pywebio/repository/archive.zip
+pip3 install -U https://github.com/pywebio/PyWebIO/archive/dev-release.zip
 ```
 
 **Prerequisites**: PyWebIO requires Python 3.5.2 or newer
 
 ## Quickstart
 
 **Hello, world**
@@ -149,10 +143,11 @@
 For integration with other web frameworks, please refer to [document](https://pywebio.readthedocs.io/en/latest/advanced.html#integration-with-web-framework).
 
 ## Demos
 
  - [Basic demo](http://pywebio-demos.pywebio.online/) : PyWebIO basic input and output demos and some small applications written using PyWebIO.
  - [Data visualization demo](http://pywebio-charts.pywebio.online/) : Data visualization with the third-party libraries, e.g., `plotly`, `bokeh`, `pyecharts`.
 
-## Document
+## Links
 
-Document is on [https://pywebio.readthedocs.io](https://pywebio.readthedocs.io)
+* Document [pywebio.readthedocs.io](https://pywebio.readthedocs.io)
+* [PyWebIO Playground](https://play.pywebio.online/): Edit, Run, Share PyWebIO Code Online
```

### Comparing `pywebio-1.7.1/demos/bmi.py` & `pywebio-1.8.0/demos/bmi.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/demos/bokeh_app.py` & `pywebio-1.8.0/demos/bokeh_app.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/demos/chat_room.py` & `pywebio-1.8.0/demos/chat_room.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/demos/doc_demo.py` & `pywebio-1.8.0/demos/doc_demo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 """
 Run the example code in the documentation online
 """
+import base64
+
 from functools import partial
 from os import path, listdir
-
 from pywebio import start_server
 from pywebio.platform import config
 from pywebio.session import local as session_local, info as session_info
+import pywebio_battery
 
 ##########################################
 # Pre-import modules for demo
 import time  # lgtm [py/unused-import]
 from pywebio.input import *
 from pywebio.output import *
 from pywebio.session import *
 from pywebio.pin import *
 from pywebio_battery import *
 
 ##########################################
 
+here_dir = path.dirname(path.abspath(__file__))
+playground_host = "https://play.pywebio.online"
+
 
 def t(eng, chinese):
     """return English or Chinese text according to the user's browser language"""
     return chinese if 'zh' in session_info.user_language else eng
 
 
-here_dir = path.dirname(path.abspath(__file__))
+def playground(code):
+    pre_import = PRE_IMPORT
+    battery_apis = pywebio_battery.__all__
+    if 'pywebio_battery import' not in code and any(api in code for api in battery_apis):
+        pre_import += 'from pywebio_battery import *\n'
+
+    code = f"{pre_import}\n{code}"
+    encode = base64.b64encode(code.encode('utf8')).decode('utf8')
+    url = f"{playground_host}/#{encode}"
+    run_js('window.open(url)', url=url)
 
 
 def gen_snippets(code):
     code = code.replace('# ..demo-only', '')
     code = '\n'.join(i for i in code.splitlines() if '# ..doc-only' not in i)
 
     parts = code.split('\n## ----\n')
@@ -47,62 +61,72 @@
             https://docs.python.org/3/library/functions.html#exec
             """
             exec(code, session_local.globals)
         except Exception as e:
             toast('Exception occurred: "%s:%s"' % (type(e).__name__, e), color='error')
 
 
-IMPORT_CODE = """from pywebio import start_server
-from pywebio.input import *
+PRE_IMPORT = """from pywebio.input import *
 from pywebio.output import *
 from pywebio.session import *
 from pywebio.pin import *
+from pywebio import start_server
+"""
 
+APP_TPL = f"""{PRE_IMPORT}
 def main():
     %s
 
 start_server(main, port=8080, debug=True)
 """
 
+CLIPBOARD_SETUP = """
+window.writeText = function(text) {
+    const input = document.createElement('textarea');
+    input.style.opacity  = 0;
+    input.style.position = 'absolute';
+    input.style.left = '-100000px';
+    document.body.appendChild(input);
+
+    input.value = text;
+    input.select();
+    input.setSelectionRange(0, text.length);
+    document.execCommand('copy');
+    document.body.removeChild(input);
+    return true;
+}
+"""
+
 
 def copytoclipboard(code):
-    code = IMPORT_CODE % code.replace('\n', '\n    ')
+    code = APP_TPL % code.replace('\n', '\n    ')
     run_js("writeText(text)", text=code)
     toast('The code has been copied to the clipboard')
 
 
 def handle_code(code, title):
-    run_js("""
-    window.writeText = function(text) {
-        const input = document.createElement('textarea');
-        input.style.opacity  = 0;
-        input.style.position = 'absolute';
-        input.style.left = '-100000px';
-        document.body.appendChild(input);
-
-        input.value = text;
-        input.select();
-        input.setSelectionRange(0, text.length);
-        document.execCommand('copy');
-        document.body.removeChild(input);
-        return true;
-    }
-    """)
+    run_js(CLIPBOARD_SETUP)
     session_local.globals = dict(globals())
     if title:
         put_markdown('## %s' % title)
 
     for p in gen_snippets(code):
         with use_scope() as scope:
             put_code(p, 'python')
 
-            put_buttons([t('Run', '运行'), t("Copy to clipboard", '复制代码')], onclick=[
-                partial(run_code, code=p, scope=scope),
-                partial(copytoclipboard, code=p)
-            ])
+            put_buttons(
+                [t('Run', '运行'),
+                 t("Edit", '编辑'),
+                 t("Copy to clipboard", '复制代码')],
+                onclick=[
+                    partial(run_code, code=p, scope=scope),
+                    partial(playground, code=p),
+                    partial(copytoclipboard, code=p)
+                ]
+            )
 
         put_markdown('----')
 
 
 def get_app():
     """PyWebIO demos from document
```

### Comparing `pywebio-1.7.1/demos/gomoku_game.py` & `pywebio-1.8.0/demos/gomoku_game.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/demos/index.py` & `pywebio-1.8.0/demos/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 <a href="{charts_demo_host}/?app=cutecharts">
     <img src="https://fastly.jsdelivr.net/gh/wang0618/pywebio-chart-gallery/assets/cutecharts.png" alt="cutecharts demo">
 </a>
 
 ### Links
 * PyWebIO Github [github.com/wang0618/PyWebIO](https://github.com/wang0618/PyWebIO)
 * Document [pywebio.readthedocs.io](https://pywebio.readthedocs.io)
+* [PyWebIO Playground](https://play.pywebio.online/): Edit, Run, Share PyWebIO Code Online
 
 """.format(charts_demo_host=charts_demo_host)
 
 index_md_zh = r"""### 基本demo
 
  - [BMI计算](./bmi): 根据身高体重计算BMI指数
  - [聊天室](./chat_room): 和当前所有在线的人聊天 (不到90行代码实现)
@@ -83,14 +84,15 @@
 <a href="{charts_demo_host}/?app=cutecharts">
     <img src="https://fastly.jsdelivr.net/gh/wang0618/pywebio-chart-gallery/assets/cutecharts.png" alt="cutecharts demo">
 </a>
 
 ### Links
 * PyWebIO Github [github.com/wang0618/PyWebIO](https://github.com/wang0618/PyWebIO)
 * 使用手册和实现文档见 [pywebio.readthedocs.io](https://pywebio.readthedocs.io/zh_CN/latest/)
+* [PyWebIO Playground](https://play.pywebio.online/): 在线编辑、运行和分享PyWebIO代码
 
 """.format(charts_demo_host=charts_demo_host)
 
 
 def main():
     """PyWebIO demos
```

### Comparing `pywebio-1.7.1/demos/input_usage.py` & `pywebio-1.8.0/demos/input_usage.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/demos/markdown_previewer.py` & `pywebio-1.8.0/demos/markdown_previewer.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/demos/output_usage.py` & `pywebio-1.8.0/demos/output_usage.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/demos/set_env_demo.py` & `pywebio-1.8.0/demos/set_env_demo.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/demos/theme.py` & `pywebio-1.8.0/demos/theme.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/__init__.py` & `pywebio-1.8.0/pywebio/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,23 +11,20 @@
 from .platform.bokeh import try_install_bokeh_hook
 from .platform.page import config
 from .utils import STATIC_PATH
 
 try_install_bokeh_hook()
 del try_install_bokeh_hook
 
-# Set default logging handler to avoid "No handler found" warnings.
-import logging
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
-
-
-def enable_debug(level=logging.DEBUG):
+def enable_debug(level=None):
     """Output PyWebIO logging message to sys.stderr"""
+    import logging
     from tornado.log import access_log, app_log, gen_log
+    level = level or logging.DEBUG
     ch = logging.StreamHandler()
     ch.setLevel(level)
     formatter = logging.Formatter('[%(levelname)s %(asctime)s %(module)s:%(lineno)d %(funcName)s] %(message)s',
                                   datefmt='%y%m%d %H:%M:%S')
     ch.setFormatter(formatter)
     for logger in [logging.getLogger(__name__), access_log, app_log, gen_log]:
         logger.handlers = [ch]
```

### Comparing `pywebio-1.7.1/pywebio/html/codemirror/active-line.js` & `pywebio-1.8.0/pywebio/html/codemirror/active-line.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/codemirror/addons.js` & `pywebio-1.8.0/pywebio/html/codemirror/addons.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/codemirror/autorefresh.js` & `pywebio-1.8.0/pywebio/html/codemirror/autorefresh.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/codemirror/loadmode.js` & `pywebio-1.8.0/pywebio/html/codemirror/loadmode.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/codemirror/matchbrackets.js` & `pywebio-1.8.0/pywebio/html/codemirror/matchbrackets.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/codemirror/python.js` & `pywebio-1.8.0/pywebio/html/codemirror/python.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/css/app.css` & `pywebio-1.8.0/pywebio/html/css/app.css`

 * *Files 16% similar despite different names*

```diff
@@ -369,8 +369,85 @@
 .form-control-range-value{
     display: inline-block;
     max-width: 35px;
     white-space: nowrap;
     color: #6c757d;
     line-height: 14px;
     vertical-align: text-top;
+}
+
+/* ag-grid datatable */
+.webio-datatable{
+    margin-bottom: 10px;
+}
+.ag-grid-cell-bar, .ag-grid-tools {
+    border-left: solid 1px #bdc3c7;
+    border-right: solid 1px #bdc3c7;
+    border-bottom: solid 1px #bdc3c7;
+    font-size: 13px;
+    line-height: 16px;
+}
+
+.ag-grid-cell-bar {
+    display: none;
+    padding: 4px 12px;
+    word-break: break-word;
+    min-height: 24px;
+}
+
+.ag-grid-tools {
+    display: -webkit-flex; /* Safari */
+    display: flex;
+    align-items: center;
+    min-height: 23px;
+    font-weight: 600;
+    font-size: 12px;
+    opacity: 0;
+}
+
+.ag-grid-tools > .grid-status {
+    display: -webkit-flex; /* Safari */
+    display: flex;
+    align-items: center;
+    flex-shrink: 0;; /* don't compress me when there no more space */
+    margin: 0 12px;
+    color: rgba(0, 0, 0, 0.38);
+    min-width: 170px;
+}
+
+.ag-grid-tools .select-count {
+    padding-right: 8px;
+}
+
+.ag-grid-tools > .grid-actions {
+    flex-grow: 1; /* use left space */
+    display: -webkit-flex; /* Safari */
+    display: flex;
+    flex-wrap: wrap;
+    justify-content: flex-end;
+    align-items: center;
+}
+
+.ag-grid-tools .sep {
+    background-color: rgba(189, 195, 199, 0.5);
+    width: 1px;
+    height: 14px;
+}
+
+.ag-grid-tools .act-btn {
+    font-weight: 600;
+    font-size: 12px;
+    box-shadow: none;
+    color: #0000008a;
+    cursor: pointer;
+    padding: 3px 8px;
+    border: none;
+    border-radius: 0;
+}
+
+.ag-grid-tools .act-btn:hover {
+    background-color: #f1f3f4;
+}
+
+.ag-grid-tools .act-btn:active {
+    background-color: #dadada;
 }
```

### Comparing `pywebio-1.7.1/pywebio/html/css/bootstrap-select.min.css` & `pywebio-1.8.0/pywebio/html/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/css/bs-theme/dark.min.css` & `pywebio-1.8.0/pywebio/html/css/bs-theme/dark.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/css/bs-theme/default.min.css` & `pywebio-1.8.0/pywebio/html/css/bs-theme/default.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/css/bs-theme/minty.min.css` & `pywebio-1.8.0/pywebio/html/css/bs-theme/minty.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/css/bs-theme/sketchy.min.css` & `pywebio-1.8.0/pywebio/html/css/bs-theme/sketchy.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/css/bs-theme/yeti.min.css` & `pywebio-1.8.0/pywebio/html/css/bs-theme/yeti.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/css/codemirror.min.css` & `pywebio-1.8.0/pywebio/html/css/codemirror.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/css/markdown.min.css` & `pywebio-1.8.0/pywebio/html/css/markdown.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/css/toastify.min.css` & `pywebio-1.8.0/pywebio/html/css/toastify.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/image/favicon_closed_32.png` & `pywebio-1.8.0/pywebio/html/image/favicon_closed_32.png`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/FileSaver.min.js` & `pywebio-1.8.0/pywebio/html/js/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/bootstrap-select.min.js` & `pywebio-1.8.0/pywebio/html/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/bootstrap.min.js` & `pywebio-1.8.0/pywebio/html/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/bs-custom-file-input.min.js` & `pywebio-1.8.0/pywebio/html/js/bs-custom-file-input.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/codemirror.min.js` & `pywebio-1.8.0/pywebio/html/js/codemirror.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/jquery.min.js` & `pywebio-1.8.0/pywebio/html/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/mustache.min.js` & `pywebio-1.8.0/pywebio/html/js/mustache.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/popper.min.js` & `pywebio-1.8.0/pywebio/html/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/prism.min.js` & `pywebio-1.8.0/pywebio/html/js/prism.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/purify.min.js` & `pywebio-1.8.0/pywebio/html/js/purify.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/pywebio.min.js` & `pywebio-1.8.0/pywebio/html/js/pywebio.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -130,20 +130,20 @@
                     "'": "&#39;"
                 },
                 c = function(e) {
                     return l[e]
                 },
                 u = /&(#(?:\d+)|(?:#x[0-9A-Fa-f]+)|(?:\w+));?/gi;
 
-            function p(e) {
+            function d(e) {
                 return e.replace(u, (function(e, t) {
                     return "colon" === (t = t.toLowerCase()) ? ":" : "#" === t.charAt(0) ? "x" === t.charAt(1) ? String.fromCharCode(parseInt(t.substring(2), 16)) : String.fromCharCode(+t.substring(1)) : ""
                 }))
             }
-            var d = /(^|[^\[])\^/g,
+            var p = /(^|[^\[])\^/g,
                 h = /[^\w:]/g,
                 f = /^$|^[a-z][a-z0-9+.-]*:|^[?#]/i,
                 _ = {},
                 m = /^[^:]+:\/*[^/]*$/,
                 v = /^([^:]+:)[\s\S]*$/,
                 g = /^([^:]+:\/*[^/]*)[\s\S]*$/;
 
@@ -167,32 +167,32 @@
             }
             var k = function(e, t) {
                     if (t) {
                         if (r.test(e)) return e.replace(a, c)
                     } else if (o.test(e)) return e.replace(s, c);
                     return e
                 },
-                w = p,
+                w = d,
                 x = function(e, t) {
                     e = e.source || e, t = t || "";
                     var n = {
                         replace: function(t, i) {
-                            return i = (i = i.source || i).replace(d, "$1"), e = e.replace(t, i), n
+                            return i = (i = i.source || i).replace(p, "$1"), e = e.replace(t, i), n
                         },
                         getRegex: function() {
                             return new RegExp(e, t)
                         }
                     };
                     return n
                 },
                 S = function(e, t, n) {
                     if (e) {
                         var i;
                         try {
-                            i = decodeURIComponent(p(n)).replace(h, "").toLowerCase()
+                            i = decodeURIComponent(d(n)).replace(h, "").toLowerCase()
                         } catch (e) {
                             return null
                         }
                         if (0 === i.indexOf("javascript:") || 0 === i.indexOf("vbscript:") || 0 === i.indexOf("data:")) return null
                     }
                     t && !f.test(n) && (n = b(t, n));
                     try {
@@ -206,70 +206,70 @@
                     exec: function() {}
                 },
                 O = function(e) {
                     for (var t, n, i = 1; i < arguments.length; i++)
                         for (n in t = arguments[i]) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n]);
                     return e
                 },
-                z = function(e, t) {
+                C = function(e, t) {
                     var n = e.replace(/\|/g, (function(e, t, n) {
                             for (var i = !1, r = t; --r >= 0 && "\\" === n[r];) i = !i;
                             return i ? "|" : " |"
                         })).split(/ \|/),
                         i = 0;
                     if (n.length > t) n.splice(t);
                     else
                         for (; n.length < t;) n.push("");
                     for (; i < n.length; i++) n[i] = n[i].trim().replace(/\\\|/g, "|");
                     return n
                 },
-                $ = y,
-                C = function(e, t) {
+                z = y,
+                j = function(e, t) {
                     if (-1 === e.indexOf(t[1])) return -1;
                     for (var n = e.length, i = 0, r = 0; r < n; r++)
                         if ("\\" === e[r]) r++;
                         else if (e[r] === t[0]) i++;
                     else if (e[r] === t[1] && --i < 0) return r;
                     return -1
                 },
-                M = function(e) {
+                P = function(e) {
                     e && e.sanitize && !e.silent && console.warn("marked(): sanitize and sanitizer parameters are deprecated since version 0.7.0, should not be used and will be removed in the future. Read more here: https://marked.js.org/#/USING_ADVANCED.md#options")
                 },
-                P = function(e, t) {
+                $ = function(e, t) {
                     if (t < 1) return "";
                     for (var n = ""; t > 1;) 1 & t && (n += e), t >>= 1, e += e;
                     return n + e
                 },
-                T = i.defaults,
-                j = $,
+                M = i.defaults,
                 I = z,
-                E = k,
-                R = C;
+                T = C,
+                R = k,
+                E = j;
 
-            function N(e, t, n) {
+            function D(e, t, n) {
                 var i = t.href,
-                    r = t.title ? E(t.title) : null,
+                    r = t.title ? R(t.title) : null,
                     a = e[1].replace(/\\([\[\]])/g, "$1");
                 return "!" !== e[0].charAt(0) ? {
                     type: "link",
                     raw: n,
                     href: i,
                     title: r,
                     text: a
                 } : {
                     type: "image",
                     raw: n,
                     href: i,
                     title: r,
-                    text: E(a)
+                    text: R(a)
                 }
             }
-            var B = function() {
+            var N = function() {
                     function e(e) {
-                        this.options = e || T
+                        this.options = e || M
                     }
                     var t = e.prototype;
                     return t.space = function(e) {
                         var t = this.rules.block.newline.exec(e);
                         if (t) return t[0].length > 1 ? {
                             type: "space",
                             raw: t[0]
@@ -285,15 +285,15 @@
                                 text: n[0].trimRight()
                             };
                             var r = n[0].replace(/^ {1,4}/gm, "");
                             return {
                                 type: "code",
                                 raw: n[0],
                                 codeBlockStyle: "indented",
-                                text: this.options.pedantic ? r : j(r, "\n")
+                                text: this.options.pedantic ? r : I(r, "\n")
                             }
                         }
                     }, t.fences = function(e) {
                         var t = this.rules.block.fences.exec(e);
                         if (t) {
                             var n = t[0],
                                 i = function(e, t) {
@@ -313,38 +313,38 @@
                             }
                         }
                     }, t.heading = function(e) {
                         var t = this.rules.block.heading.exec(e);
                         if (t) {
                             var n = t[2].trim();
                             if (/#$/.test(n)) {
-                                var i = j(n, "#");
+                                var i = I(n, "#");
                                 this.options.pedantic ? n = i.trim() : i && !/ $/.test(i) || (n = i.trim())
                             }
                             return {
                                 type: "heading",
                                 raw: t[0],
                                 depth: t[1].length,
                                 text: n
                             }
                         }
                     }, t.nptable = function(e) {
                         var t = this.rules.block.nptable.exec(e);
                         if (t) {
                             var n = {
                                 type: "table",
-                                header: I(t[1].replace(/^ *| *\| *$/g, "")),
+                                header: T(t[1].replace(/^ *| *\| *$/g, "")),
                                 align: t[2].replace(/^ *|\| *$/g, "").split(/ *\| */),
                                 cells: t[3] ? t[3].replace(/\n$/, "").split("\n") : [],
                                 raw: t[0]
                             };
                             if (n.header.length === n.align.length) {
                                 var i, r = n.align.length;
                                 for (i = 0; i < r; i++) /^ *-+: *$/.test(n.align[i]) ? n.align[i] = "right" : /^ *:-+: *$/.test(n.align[i]) ? n.align[i] = "center" : /^ *:-+ *$/.test(n.align[i]) ? n.align[i] = "left" : n.align[i] = null;
-                                for (r = n.cells.length, i = 0; i < r; i++) n.cells[i] = I(n.cells[i], n.header.length);
+                                for (r = n.cells.length, i = 0; i < r; i++) n.cells[i] = T(n.cells[i], n.header.length);
                                 return n
                             }
                         }
                     }, t.hr = function(e) {
                         var t = this.rules.block.hr.exec(e);
                         if (t) return {
                             type: "hr",
@@ -360,34 +360,34 @@
                                 text: n
                             }
                         }
                     }, t.list = function(e) {
                         var t = this.rules.block.list.exec(e);
                         if (t) {
                             var n, i, r, a, o, s, l, c, u = t[0],
-                                p = t[2],
-                                d = p.length > 1,
+                                d = t[2],
+                                p = d.length > 1,
                                 h = {
                                     type: "list",
                                     raw: u,
-                                    ordered: d,
-                                    start: d ? +p.slice(0, -1) : "",
+                                    ordered: p,
+                                    start: p ? +d.slice(0, -1) : "",
                                     loose: !1,
                                     items: []
                                 },
                                 f = t[0].match(this.rules.block.item),
                                 _ = !1,
                                 m = f.length;
                             r = this.rules.block.listItemStart.exec(f[0]);
                             for (var v = 0; v < m; v++) {
                                 if (u = n = f[v], v !== m - 1) {
                                     if ((a = this.rules.block.listItemStart.exec(f[v + 1]))[1].length > r[0].length || a[1].length > 3) {
                                         f.splice(v, 2, f[v] + "\n" + f[v + 1]), v--, m--;
                                         continue
-                                    }(!this.options.pedantic || this.options.smartLists ? a[2][a[2].length - 1] !== p[p.length - 1] : d === (1 === a[2].length)) && (o = f.slice(v + 1).join("\n"), h.raw = h.raw.substring(0, h.raw.length - o.length), v = m - 1), r = a
+                                    }(!this.options.pedantic || this.options.smartLists ? a[2][a[2].length - 1] !== d[d.length - 1] : p === (1 === a[2].length)) && (o = f.slice(v + 1).join("\n"), h.raw = h.raw.substring(0, h.raw.length - o.length), v = m - 1), r = a
                                 }
                                 i = n.length, ~(n = n.replace(/^ *([*+-]|\d+[.)]) ?/, "")).indexOf("\n ") && (i -= n.length, n = this.options.pedantic ? n.replace(/^ {1,4}/gm, "") : n.replace(new RegExp("^ {1," + i + "}", "gm"), "")), s = _ || /\n\n(?!\s*$)/.test(n), v !== m - 1 && (_ = "\n" === n.charAt(n.length - 1), s || (s = _)), s && (h.loose = !0), this.options.gfm && (c = void 0, (l = /^\[[ xX]\] /.test(n)) && (c = " " !== n[1], n = n.replace(/^\[[ xX]\] +/, ""))), h.items.push({
                                     type: "list_item",
                                     raw: u,
                                     task: l,
                                     checked: c,
                                     loose: s,
@@ -398,38 +398,38 @@
                         }
                     }, t.html = function(e) {
                         var t = this.rules.block.html.exec(e);
                         if (t) return {
                             type: this.options.sanitize ? "paragraph" : "html",
                             raw: t[0],
                             pre: !this.options.sanitizer && ("pre" === t[1] || "script" === t[1] || "style" === t[1]),
-                            text: this.options.sanitize ? this.options.sanitizer ? this.options.sanitizer(t[0]) : E(t[0]) : t[0]
+                            text: this.options.sanitize ? this.options.sanitizer ? this.options.sanitizer(t[0]) : R(t[0]) : t[0]
                         }
                     }, t.def = function(e) {
                         var t = this.rules.block.def.exec(e);
                         if (t) return t[3] && (t[3] = t[3].substring(1, t[3].length - 1)), {
                             tag: t[1].toLowerCase().replace(/\s+/g, " "),
                             raw: t[0],
                             href: t[2],
                             title: t[3]
                         }
                     }, t.table = function(e) {
                         var t = this.rules.block.table.exec(e);
                         if (t) {
                             var n = {
                                 type: "table",
-                                header: I(t[1].replace(/^ *| *\| *$/g, "")),
+                                header: T(t[1].replace(/^ *| *\| *$/g, "")),
                                 align: t[2].replace(/^ *|\| *$/g, "").split(/ *\| */),
                                 cells: t[3] ? t[3].replace(/\n$/, "").split("\n") : []
                             };
                             if (n.header.length === n.align.length) {
                                 n.raw = t[0];
                                 var i, r = n.align.length;
                                 for (i = 0; i < r; i++) /^ *-+: *$/.test(n.align[i]) ? n.align[i] = "right" : /^ *:-+: *$/.test(n.align[i]) ? n.align[i] = "center" : /^ *:-+ *$/.test(n.align[i]) ? n.align[i] = "left" : n.align[i] = null;
-                                for (r = n.cells.length, i = 0; i < r; i++) n.cells[i] = I(n.cells[i].replace(/^ *\| *| *\| *$/g, ""), n.header.length);
+                                for (r = n.cells.length, i = 0; i < r; i++) n.cells[i] = T(n.cells[i].replace(/^ *\| *| *\| *$/g, ""), n.header.length);
                                 return n
                             }
                         }
                     }, t.lheading = function(e) {
                         var t = this.rules.block.lheading.exec(e);
                         if (t) return {
                             type: "heading",
@@ -458,47 +458,47 @@
                             }
                         }
                     }, t.escape = function(e) {
                         var t = this.rules.inline.escape.exec(e);
                         if (t) return {
                             type: "escape",
                             raw: t[0],
-                            text: E(t[1])
+                            text: R(t[1])
                         }
                     }, t.tag = function(e, t, n) {
                         var i = this.rules.inline.tag.exec(e);
                         if (i) return !t && /^<a /i.test(i[0]) ? t = !0 : t && /^<\/a>/i.test(i[0]) && (t = !1), !n && /^<(pre|code|kbd|script)(\s|>)/i.test(i[0]) ? n = !0 : n && /^<\/(pre|code|kbd|script)(\s|>)/i.test(i[0]) && (n = !1), {
                             type: this.options.sanitize ? "text" : "html",
                             raw: i[0],
                             inLink: t,
                             inRawBlock: n,
-                            text: this.options.sanitize ? this.options.sanitizer ? this.options.sanitizer(i[0]) : E(i[0]) : i[0]
+                            text: this.options.sanitize ? this.options.sanitizer ? this.options.sanitizer(i[0]) : R(i[0]) : i[0]
                         }
                     }, t.link = function(e) {
                         var t = this.rules.inline.link.exec(e);
                         if (t) {
                             var n = t[2].trim();
                             if (!this.options.pedantic && /^</.test(n)) {
                                 if (!/>$/.test(n)) return;
-                                var i = j(n.slice(0, -1), "\\");
+                                var i = I(n.slice(0, -1), "\\");
                                 if ((n.length - i.length) % 2 == 0) return
                             } else {
-                                var r = R(t[2], "()");
+                                var r = E(t[2], "()");
                                 if (r > -1) {
                                     var a = (0 === t[0].indexOf("!") ? 5 : 4) + t[1].length + r;
                                     t[2] = t[2].substring(0, r), t[0] = t[0].substring(0, a).trim(), t[3] = ""
                                 }
                             }
                             var o = t[2],
                                 s = "";
                             if (this.options.pedantic) {
                                 var l = /^([^'"]*[^\s])\s+(['"])(.*)\2/.exec(o);
                                 l && (o = l[1], s = l[3])
                             } else s = t[3] ? t[3].slice(1, -1) : "";
-                            return o = o.trim(), /^</.test(o) && (o = this.options.pedantic && !/>$/.test(n) ? o.slice(1) : o.slice(1, -1)), N(t, {
+                            return o = o.trim(), /^</.test(o) && (o = this.options.pedantic && !/>$/.test(n) ? o.slice(1) : o.slice(1, -1)), D(t, {
                                 href: o ? o.replace(this.rules.inline._escapes, "$1") : o,
                                 title: s ? s.replace(this.rules.inline._escapes, "$1") : s
                             }, t[0])
                         }
                     }, t.reflink = function(e, t) {
                         var n;
                         if ((n = this.rules.inline.reflink.exec(e)) || (n = this.rules.inline.nolink.exec(e))) {
@@ -507,15 +507,15 @@
                                 var r = n[0].charAt(0);
                                 return {
                                     type: "text",
                                     raw: r,
                                     text: r
                                 }
                             }
-                            return N(n, i, n[0])
+                            return D(n, i, n[0])
                         }
                     }, t.strong = function(e, t, n) {
                         void 0 === n && (n = "");
                         var i = this.rules.inline.strong.start.exec(e);
                         if (i && (!i[1] || i[1] && ("" === n || this.rules.inline.punctuation.exec(n)))) {
                             t = t.slice(-1 * e.length);
                             var r, a = "**" === i[0] ? this.rules.inline.strong.endAst : this.rules.inline.strong.endUnd;
@@ -541,15 +541,15 @@
                         }
                     }, t.codespan = function(e) {
                         var t = this.rules.inline.code.exec(e);
                         if (t) {
                             var n = t[2].replace(/\n/g, " "),
                                 i = /[^ ]/.test(n),
                                 r = /^ /.test(n) && / $/.test(n);
-                            return i && r && (n = n.substring(1, n.length - 1)), n = E(n, !0), {
+                            return i && r && (n = n.substring(1, n.length - 1)), n = R(n, !0), {
                                 type: "codespan",
                                 raw: t[0],
                                 text: n
                             }
                         }
                     }, t.br = function(e) {
                         var t = this.rules.inline.br.exec(e);
@@ -562,36 +562,36 @@
                         if (t) return {
                             type: "del",
                             raw: t[0],
                             text: t[2]
                         }
                     }, t.autolink = function(e, t) {
                         var n, i, r = this.rules.inline.autolink.exec(e);
-                        if (r) return i = "@" === r[2] ? "mailto:" + (n = E(this.options.mangle ? t(r[1]) : r[1])) : n = E(r[1]), {
+                        if (r) return i = "@" === r[2] ? "mailto:" + (n = R(this.options.mangle ? t(r[1]) : r[1])) : n = R(r[1]), {
                             type: "link",
                             raw: r[0],
                             text: n,
                             href: i,
                             tokens: [{
                                 type: "text",
                                 raw: n,
                                 text: n
                             }]
                         }
                     }, t.url = function(e, t) {
                         var n;
                         if (n = this.rules.inline.url.exec(e)) {
                             var i, r;
-                            if ("@" === n[2]) r = "mailto:" + (i = E(this.options.mangle ? t(n[0]) : n[0]));
+                            if ("@" === n[2]) r = "mailto:" + (i = R(this.options.mangle ? t(n[0]) : n[0]));
                             else {
                                 var a;
                                 do {
                                     a = n[0], n[0] = this.rules.inline._backpedal.exec(n[0])[0]
                                 } while (a !== n[0]);
-                                i = E(n[0]), r = "www." === n[1] ? "http://" + i : i
+                                i = R(n[0]), r = "www." === n[1] ? "http://" + i : i
                             }
                             return {
                                 type: "link",
                                 raw: n[0],
                                 text: i,
                                 href: r,
                                 tokens: [{
@@ -599,56 +599,56 @@
                                     raw: i,
                                     text: i
                                 }]
                             }
                         }
                     }, t.inlineText = function(e, t, n) {
                         var i, r = this.rules.inline.text.exec(e);
-                        if (r) return i = t ? this.options.sanitize ? this.options.sanitizer ? this.options.sanitizer(r[0]) : E(r[0]) : r[0] : E(this.options.smartypants ? n(r[0]) : r[0]), {
+                        if (r) return i = t ? this.options.sanitize ? this.options.sanitizer ? this.options.sanitizer(r[0]) : R(r[0]) : r[0] : R(this.options.smartypants ? n(r[0]) : r[0]), {
                             type: "text",
                             raw: r[0],
                             text: i
                         }
                     }, e
                 }(),
-                D = A,
-                U = x,
-                q = O,
-                L = {
+                q = A,
+                B = x,
+                U = O,
+                W = {
                     newline: /^(?: *(?:\n|$))+/,
                     code: /^( {4}[^\n]+(?:\n(?: *(?:\n|$))*)?)+/,
                     fences: /^ {0,3}(`{3,}(?=[^`\n]*\n)|~{3,})([^\n]*)\n(?:|([\s\S]*?)\n)(?: {0,3}\1[~`]* *(?:\n+|$)|$)/,
                     hr: /^ {0,3}((?:- *){3,}|(?:_ *){3,}|(?:\* *){3,})(?:\n+|$)/,
                     heading: /^ {0,3}(#{1,6})(?=\s|$)(.*)(?:\n+|$)/,
                     blockquote: /^( {0,3}> ?(paragraph|[^\n]*)(?:\n|$))+/,
                     list: /^( {0,3})(bull) [\s\S]+?(?:hr|def|\n{2,}(?! )(?! {0,3}bull )\n*|\s*$)/,
                     html: "^ {0,3}(?:<(script|pre|style)[\\s>][\\s\\S]*?(?:</\\1>[^\\n]*\\n+|$)|comment[^\\n]*(\\n+|$)|<\\?[\\s\\S]*?(?:\\?>\\n*|$)|<![A-Z][\\s\\S]*?(?:>\\n*|$)|<!\\[CDATA\\[[\\s\\S]*?(?:\\]\\]>\\n*|$)|</?(tag)(?: +|\\n|/?>)[\\s\\S]*?(?:\\n{2,}|$)|<(?!script|pre|style)([a-z][\\w-]*)(?:attribute)*? */?>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:\\n{2,}|$)|</(?!script|pre|style)[a-z][\\w-]*\\s*>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:\\n{2,}|$))",
                     def: /^ {0,3}\[(label)\]: *\n? *<?([^\s>]+)>?(?:(?: +\n? *| *\n *)(title))? *(?:\n+|$)/,
-                    nptable: D,
-                    table: D,
+                    nptable: q,
+                    table: q,
                     lheading: /^([^\n]+)\n {0,3}(=+|-+) *(?:\n+|$)/,
                     _paragraph: /^([^\n]+(?:\n(?!hr|heading|lheading|blockquote|fences|list|html| +\n)[^\n]+)*)/,
                     text: /^[^\n]+/,
                     _label: /(?!\s*\])(?:\\[\[\]]|[^\[\]])+/,
                     _title: /(?:"(?:\\"?|[^"\\])*"|'[^'\n]*(?:\n[^'\n]+)*\n?'|\([^()]*\))/
                 };
-            L.def = U(L.def).replace("label", L._label).replace("title", L._title).getRegex(), L.bullet = /(?:[*+-]|\d{1,9}[.)])/, L.item = /^( *)(bull) ?[^\n]*(?:\n(?! *bull ?)[^\n]*)*/, L.item = U(L.item, "gm").replace(/bull/g, L.bullet).getRegex(), L.listItemStart = U(/^( *)(bull)/).replace("bull", L.bullet).getRegex(), L.list = U(L.list).replace(/bull/g, L.bullet).replace("hr", "\\n+(?=\\1?(?:(?:- *){3,}|(?:_ *){3,}|(?:\\* *){3,})(?:\\n+|$))").replace("def", "\\n+(?=" + L.def.source + ")").getRegex(), L._tag = "address|article|aside|base|basefont|blockquote|body|caption|center|col|colgroup|dd|details|dialog|dir|div|dl|dt|fieldset|figcaption|figure|footer|form|frame|frameset|h[1-6]|head|header|hr|html|iframe|legend|li|link|main|menu|menuitem|meta|nav|noframes|ol|optgroup|option|p|param|section|source|summary|table|tbody|td|tfoot|th|thead|title|tr|track|ul", L._comment = /<!--(?!-?>)[\s\S]*?(?:-->|$)/, L.html = U(L.html, "i").replace("comment", L._comment).replace("tag", L._tag).replace("attribute", / +[a-zA-Z:_][\w.:-]*(?: *= *"[^"\n]*"| *= *'[^'\n]*'| *= *[^\s"'=<>`]+)?/).getRegex(), L.paragraph = U(L._paragraph).replace("hr", L.hr).replace("heading", " {0,3}#{1,6} ").replace("|lheading", "").replace("blockquote", " {0,3}>").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|!--)").replace("tag", L._tag).getRegex(), L.blockquote = U(L.blockquote).replace("paragraph", L.paragraph).getRegex(), L.normal = q({}, L), L.gfm = q({}, L.normal, {
+            W.def = B(W.def).replace("label", W._label).replace("title", W._title).getRegex(), W.bullet = /(?:[*+-]|\d{1,9}[.)])/, W.item = /^( *)(bull) ?[^\n]*(?:\n(?! *bull ?)[^\n]*)*/, W.item = B(W.item, "gm").replace(/bull/g, W.bullet).getRegex(), W.listItemStart = B(/^( *)(bull)/).replace("bull", W.bullet).getRegex(), W.list = B(W.list).replace(/bull/g, W.bullet).replace("hr", "\\n+(?=\\1?(?:(?:- *){3,}|(?:_ *){3,}|(?:\\* *){3,})(?:\\n+|$))").replace("def", "\\n+(?=" + W.def.source + ")").getRegex(), W._tag = "address|article|aside|base|basefont|blockquote|body|caption|center|col|colgroup|dd|details|dialog|dir|div|dl|dt|fieldset|figcaption|figure|footer|form|frame|frameset|h[1-6]|head|header|hr|html|iframe|legend|li|link|main|menu|menuitem|meta|nav|noframes|ol|optgroup|option|p|param|section|source|summary|table|tbody|td|tfoot|th|thead|title|tr|track|ul", W._comment = /<!--(?!-?>)[\s\S]*?(?:-->|$)/, W.html = B(W.html, "i").replace("comment", W._comment).replace("tag", W._tag).replace("attribute", / +[a-zA-Z:_][\w.:-]*(?: *= *"[^"\n]*"| *= *'[^'\n]*'| *= *[^\s"'=<>`]+)?/).getRegex(), W.paragraph = B(W._paragraph).replace("hr", W.hr).replace("heading", " {0,3}#{1,6} ").replace("|lheading", "").replace("blockquote", " {0,3}>").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|!--)").replace("tag", W._tag).getRegex(), W.blockquote = B(W.blockquote).replace("paragraph", W.paragraph).getRegex(), W.normal = U({}, W), W.gfm = U({}, W.normal, {
                 nptable: "^ *([^|\\n ].*\\|.*)\\n {0,3}([-:]+ *\\|[-| :]*)(?:\\n((?:(?!\\n|hr|heading|blockquote|code|fences|list|html).*(?:\\n|$))*)\\n*|$)",
                 table: "^ *\\|(.+)\\n {0,3}\\|?( *[-:]+[-| :]*)(?:\\n *((?:(?!\\n|hr|heading|blockquote|code|fences|list|html).*(?:\\n|$))*)\\n*|$)"
-            }), L.gfm.nptable = U(L.gfm.nptable).replace("hr", L.hr).replace("heading", " {0,3}#{1,6} ").replace("blockquote", " {0,3}>").replace("code", " {4}[^\\n]").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|!--)").replace("tag", L._tag).getRegex(), L.gfm.table = U(L.gfm.table).replace("hr", L.hr).replace("heading", " {0,3}#{1,6} ").replace("blockquote", " {0,3}>").replace("code", " {4}[^\\n]").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|!--)").replace("tag", L._tag).getRegex(), L.pedantic = q({}, L.normal, {
-                html: U("^ *(?:comment *(?:\\n|\\s*$)|<(tag)[\\s\\S]+?</\\1> *(?:\\n{2,}|\\s*$)|<tag(?:\"[^\"]*\"|'[^']*'|\\s[^'\"/>\\s]*)*?/?> *(?:\\n{2,}|\\s*$))").replace("comment", L._comment).replace(/tag/g, "(?!(?:a|em|strong|small|s|cite|q|dfn|abbr|data|time|code|var|samp|kbd|sub|sup|i|b|u|mark|ruby|rt|rp|bdi|bdo|span|br|wbr|ins|del|img)\\b)\\w+(?!:|[^\\w\\s@]*@)\\b").getRegex(),
+            }), W.gfm.nptable = B(W.gfm.nptable).replace("hr", W.hr).replace("heading", " {0,3}#{1,6} ").replace("blockquote", " {0,3}>").replace("code", " {4}[^\\n]").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|!--)").replace("tag", W._tag).getRegex(), W.gfm.table = B(W.gfm.table).replace("hr", W.hr).replace("heading", " {0,3}#{1,6} ").replace("blockquote", " {0,3}>").replace("code", " {4}[^\\n]").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|!--)").replace("tag", W._tag).getRegex(), W.pedantic = U({}, W.normal, {
+                html: B("^ *(?:comment *(?:\\n|\\s*$)|<(tag)[\\s\\S]+?</\\1> *(?:\\n{2,}|\\s*$)|<tag(?:\"[^\"]*\"|'[^']*'|\\s[^'\"/>\\s]*)*?/?> *(?:\\n{2,}|\\s*$))").replace("comment", W._comment).replace(/tag/g, "(?!(?:a|em|strong|small|s|cite|q|dfn|abbr|data|time|code|var|samp|kbd|sub|sup|i|b|u|mark|ruby|rt|rp|bdi|bdo|span|br|wbr|ins|del|img)\\b)\\w+(?!:|[^\\w\\s@]*@)\\b").getRegex(),
                 def: /^ *\[([^\]]+)\]: *<?([^\s>]+)>?(?: +(["(][^\n]+[")]))? *(?:\n+|$)/,
                 heading: /^(#{1,6})(.*)(?:\n+|$)/,
-                fences: D,
-                paragraph: U(L.normal._paragraph).replace("hr", L.hr).replace("heading", " *#{1,6} *[^\n]").replace("lheading", L.lheading).replace("blockquote", " {0,3}>").replace("|fences", "").replace("|list", "").replace("|html", "").getRegex()
+                fences: q,
+                paragraph: B(W.normal._paragraph).replace("hr", W.hr).replace("heading", " *#{1,6} *[^\n]").replace("lheading", W.lheading).replace("blockquote", " {0,3}>").replace("|fences", "").replace("|list", "").replace("|html", "").getRegex()
             });
-            var W = {
+            var L = {
                 escape: /^\\([!"#$%&'()*+,\-./:;<=>?@\[\]\\^_`{|}~])/,
                 autolink: /^<(scheme:[^\s\x00-\x1f<>]*|email)>/,
-                url: D,
+                url: q,
                 tag: "^comment|^</[a-zA-Z][\\w:-]*\\s*>|^<[a-zA-Z][\\w-]*(?:attribute)*?\\s*/?>|^<\\?[\\s\\S]*?\\?>|^<![a-zA-Z]+\\s[\\s\\S]*?>|^<!\\[CDATA\\[[\\s\\S]*?\\]\\]>",
                 link: /^!?\[(label)\]\(\s*(href)(?:\s+(title))?\s*\)/,
                 reflink: /^!?\[(label)\]\[(?!\s*\])((?:\\[\[\]]?|[^\[\]\\])+)\]/,
                 nolink: /^!?\[(?!\s*\])((?:\[[^\[\]]*\]|\\[\[\]]|[^\[\]])*)\](?:\[\])?/,
                 reflinkSearch: "reflink|nolink(?!\\()",
                 strong: {
                     start: /^(?:(\*\*(?=[*punctuation]))|\*\*)(?![\s])|__/,
@@ -660,67 +660,67 @@
                     start: /^(?:(\*(?=[punctuation]))|\*)(?![*\s])|_/,
                     middle: /^\*(?:(?:(?!overlapSkip)(?:[^*]|\\\*)|overlapSkip)|\*(?:(?!overlapSkip)(?:[^*]|\\\*)|overlapSkip)*?\*)+?\*$|^_(?![_\s])(?:(?:(?!overlapSkip)(?:[^_]|\\_)|overlapSkip)|_(?:(?!overlapSkip)(?:[^_]|\\_)|overlapSkip)*?_)+?_$/,
                     endAst: /[^punctuation\s]\*(?!\*)|[punctuation]\*(?!\*)(?:(?=[punctuation_\s]|$))/,
                     endUnd: /[^\s]_(?!_)(?:(?=[punctuation*\s])|$)/
                 },
                 code: /^(`+)([^`]|[^`][\s\S]*?[^`])\1(?!`)/,
                 br: /^( {2,}|\\)\n(?!\s*$)/,
-                del: D,
+                del: q,
                 text: /^(`+|[^`])(?:(?= {2,}\n)|[\s\S]*?(?:(?=[\\<!\[`*]|\b_|$)|[^ ](?= {2,}\n)))/,
                 punctuation: /^([\s*punctuation])/,
                 _punctuation: "!\"#$%&'()+\\-.,/:;<=>?@\\[\\]`^{|}~"
             };
-            W.punctuation = U(W.punctuation).replace(/punctuation/g, W._punctuation).getRegex(), W._blockSkip = "\\[[^\\]]*?\\]\\([^\\)]*?\\)|`[^`]*?`|<[^>]*?>", W._overlapSkip = "__[^_]*?__|\\*\\*\\[^\\*\\]*?\\*\\*", W._comment = U(L._comment).replace("(?:--\x3e|$)", "--\x3e").getRegex(), W.em.start = U(W.em.start).replace(/punctuation/g, W._punctuation).getRegex(), W.em.middle = U(W.em.middle).replace(/punctuation/g, W._punctuation).replace(/overlapSkip/g, W._overlapSkip).getRegex(), W.em.endAst = U(W.em.endAst, "g").replace(/punctuation/g, W._punctuation).getRegex(), W.em.endUnd = U(W.em.endUnd, "g").replace(/punctuation/g, W._punctuation).getRegex(), W.strong.start = U(W.strong.start).replace(/punctuation/g, W._punctuation).getRegex(), W.strong.middle = U(W.strong.middle).replace(/punctuation/g, W._punctuation).replace(/overlapSkip/g, W._overlapSkip).getRegex(), W.strong.endAst = U(W.strong.endAst, "g").replace(/punctuation/g, W._punctuation).getRegex(), W.strong.endUnd = U(W.strong.endUnd, "g").replace(/punctuation/g, W._punctuation).getRegex(), W.blockSkip = U(W._blockSkip, "g").getRegex(), W.overlapSkip = U(W._overlapSkip, "g").getRegex(), W._escapes = /\\([!"#$%&'()*+,\-./:;<=>?@\[\]\\^_`{|}~])/g, W._scheme = /[a-zA-Z][a-zA-Z0-9+.-]{1,31}/, W._email = /[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+(@)[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)+(?![-_])/, W.autolink = U(W.autolink).replace("scheme", W._scheme).replace("email", W._email).getRegex(), W._attribute = /\s+[a-zA-Z:_][\w.:-]*(?:\s*=\s*"[^"]*"|\s*=\s*'[^']*'|\s*=\s*[^\s"'=<>`]+)?/, W.tag = U(W.tag).replace("comment", W._comment).replace("attribute", W._attribute).getRegex(), W._label = /(?:\[(?:\\.|[^\[\]\\])*\]|\\.|`[^`]*`|[^\[\]\\`])*?/, W._href = /<(?:\\.|[^\n<>\\])+>|[^\s\x00-\x1f]*/, W._title = /"(?:\\"?|[^"\\])*"|'(?:\\'?|[^'\\])*'|\((?:\\\)?|[^)\\])*\)/, W.link = U(W.link).replace("label", W._label).replace("href", W._href).replace("title", W._title).getRegex(), W.reflink = U(W.reflink).replace("label", W._label).getRegex(), W.reflinkSearch = U(W.reflinkSearch, "g").replace("reflink", W.reflink).replace("nolink", W.nolink).getRegex(), W.normal = q({}, W), W.pedantic = q({}, W.normal, {
+            L.punctuation = B(L.punctuation).replace(/punctuation/g, L._punctuation).getRegex(), L._blockSkip = "\\[[^\\]]*?\\]\\([^\\)]*?\\)|`[^`]*?`|<[^>]*?>", L._overlapSkip = "__[^_]*?__|\\*\\*\\[^\\*\\]*?\\*\\*", L._comment = B(W._comment).replace("(?:--\x3e|$)", "--\x3e").getRegex(), L.em.start = B(L.em.start).replace(/punctuation/g, L._punctuation).getRegex(), L.em.middle = B(L.em.middle).replace(/punctuation/g, L._punctuation).replace(/overlapSkip/g, L._overlapSkip).getRegex(), L.em.endAst = B(L.em.endAst, "g").replace(/punctuation/g, L._punctuation).getRegex(), L.em.endUnd = B(L.em.endUnd, "g").replace(/punctuation/g, L._punctuation).getRegex(), L.strong.start = B(L.strong.start).replace(/punctuation/g, L._punctuation).getRegex(), L.strong.middle = B(L.strong.middle).replace(/punctuation/g, L._punctuation).replace(/overlapSkip/g, L._overlapSkip).getRegex(), L.strong.endAst = B(L.strong.endAst, "g").replace(/punctuation/g, L._punctuation).getRegex(), L.strong.endUnd = B(L.strong.endUnd, "g").replace(/punctuation/g, L._punctuation).getRegex(), L.blockSkip = B(L._blockSkip, "g").getRegex(), L.overlapSkip = B(L._overlapSkip, "g").getRegex(), L._escapes = /\\([!"#$%&'()*+,\-./:;<=>?@\[\]\\^_`{|}~])/g, L._scheme = /[a-zA-Z][a-zA-Z0-9+.-]{1,31}/, L._email = /[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+(@)[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)+(?![-_])/, L.autolink = B(L.autolink).replace("scheme", L._scheme).replace("email", L._email).getRegex(), L._attribute = /\s+[a-zA-Z:_][\w.:-]*(?:\s*=\s*"[^"]*"|\s*=\s*'[^']*'|\s*=\s*[^\s"'=<>`]+)?/, L.tag = B(L.tag).replace("comment", L._comment).replace("attribute", L._attribute).getRegex(), L._label = /(?:\[(?:\\.|[^\[\]\\])*\]|\\.|`[^`]*`|[^\[\]\\`])*?/, L._href = /<(?:\\.|[^\n<>\\])+>|[^\s\x00-\x1f]*/, L._title = /"(?:\\"?|[^"\\])*"|'(?:\\'?|[^'\\])*'|\((?:\\\)?|[^)\\])*\)/, L.link = B(L.link).replace("label", L._label).replace("href", L._href).replace("title", L._title).getRegex(), L.reflink = B(L.reflink).replace("label", L._label).getRegex(), L.reflinkSearch = B(L.reflinkSearch, "g").replace("reflink", L.reflink).replace("nolink", L.nolink).getRegex(), L.normal = U({}, L), L.pedantic = U({}, L.normal, {
                 strong: {
                     start: /^__|\*\*/,
                     middle: /^__(?=\S)([\s\S]*?\S)__(?!_)|^\*\*(?=\S)([\s\S]*?\S)\*\*(?!\*)/,
                     endAst: /\*\*(?!\*)/g,
                     endUnd: /__(?!_)/g
                 },
                 em: {
                     start: /^_|\*/,
                     middle: /^()\*(?=\S)([\s\S]*?\S)\*(?!\*)|^_(?=\S)([\s\S]*?\S)_(?!_)/,
                     endAst: /\*(?!\*)/g,
                     endUnd: /_(?!_)/g
                 },
-                link: U(/^!?\[(label)\]\((.*?)\)/).replace("label", W._label).getRegex(),
-                reflink: U(/^!?\[(label)\]\s*\[([^\]]*)\]/).replace("label", W._label).getRegex()
-            }), W.gfm = q({}, W.normal, {
-                escape: U(W.escape).replace("])", "~|])").getRegex(),
+                link: B(/^!?\[(label)\]\((.*?)\)/).replace("label", L._label).getRegex(),
+                reflink: B(/^!?\[(label)\]\s*\[([^\]]*)\]/).replace("label", L._label).getRegex()
+            }), L.gfm = U({}, L.normal, {
+                escape: B(L.escape).replace("])", "~|])").getRegex(),
                 _extended_email: /[A-Za-z0-9._+-]+(@)[a-zA-Z0-9-_]+(?:\.[a-zA-Z0-9-_]*[a-zA-Z0-9])+(?![-_])/,
                 url: /^((?:ftp|https?):\/\/|www\.)(?:[a-zA-Z0-9\-]+\.?)+[^\s<]*|^email/,
                 _backpedal: /(?:[^?!.,:;*_~()&]+|\([^)]*\)|&(?![a-zA-Z0-9]+;$)|[?!.,:;*_~)]+(?!$))+/,
                 del: /^(~~?)(?=[^\s~])([\s\S]*?[^\s~])\1(?=[^~]|$)/,
                 text: /^([`~]+|[^`~])(?:(?= {2,}\n)|[\s\S]*?(?:(?=[\\<!\[`*~]|\b_|https?:\/\/|ftp:\/\/|www\.|$)|[^ ](?= {2,}\n)|[^a-zA-Z0-9.!#$%&'*+\/=?_`{\|}~-](?=[a-zA-Z0-9.!#$%&'*+\/=?_`{\|}~-]+@))|(?=[a-zA-Z0-9.!#$%&'*+\/=?_`{\|}~-]+@))/
-            }), W.gfm.url = U(W.gfm.url, "i").replace("email", W.gfm._extended_email).getRegex(), W.breaks = q({}, W.gfm, {
-                br: U(W.br).replace("{2,}", "*").getRegex(),
-                text: U(W.gfm.text).replace("\\b_", "\\b_| {2,}\\n").replace(/\{2,\}/g, "*").getRegex()
+            }), L.gfm.url = B(L.gfm.url, "i").replace("email", L.gfm._extended_email).getRegex(), L.breaks = U({}, L.gfm, {
+                br: B(L.br).replace("{2,}", "*").getRegex(),
+                text: B(L.gfm.text).replace("\\b_", "\\b_| {2,}\\n").replace(/\{2,\}/g, "*").getRegex()
             });
-            var H = {
-                    block: L,
-                    inline: W
+            var F = {
+                    block: W,
+                    inline: L
                 },
-                F = i.defaults,
-                J = H.block,
-                Z = H.inline,
-                Q = P;
+                H = i.defaults,
+                J = F.block,
+                Z = F.inline,
+                G = $;
 
-            function Y(e) {
+            function Q(e) {
                 return e.replace(/---/g, "—").replace(/--/g, "–").replace(/(^|[-\u2014/(\[{"\s])'/g, "$1‘").replace(/'/g, "’").replace(/(^|[-\u2014/(\[{\u2018\s])"/g, "$1“").replace(/"/g, "”").replace(/\.{3}/g, "…")
             }
 
-            function G(e) {
+            function Y(e) {
                 var t, n, i = "",
                     r = e.length;
                 for (t = 0; t < r; t++) n = e.charCodeAt(t), Math.random() > .5 && (n = "x" + n.toString(16)), i += "&#" + n + ";";
                 return i
             }
             var V = function() {
                     function t(e) {
-                        this.tokens = [], this.tokens.links = Object.create(null), this.options = e || F, this.options.tokenizer = this.options.tokenizer || new B, this.tokenizer = this.options.tokenizer, this.tokenizer.options = this.options;
+                        this.tokens = [], this.tokens.links = Object.create(null), this.options = e || H, this.options.tokenizer = this.options.tokenizer || new N, this.tokenizer = this.options.tokenizer, this.tokenizer.options = this.options;
                         var t = {
                             block: J.normal,
                             inline: Z.normal
                         };
                         this.options.pedantic ? (t.block = J.pedantic, t.inline = Z.pedantic) : this.options.gfm && (t.block = J.gfm, this.options.breaks ? t.inline = Z.breaks : t.inline = Z.gfm), this.tokenizer.rules = t
                     }
                     t.lex = function(e, n) {
@@ -788,30 +788,30 @@
                     }, a.inlineTokens = function(e, t, n, i) {
                         var r;
                         void 0 === t && (t = []), void 0 === n && (n = !1), void 0 === i && (i = !1);
                         var a, o, s, l = e;
                         if (this.tokens.links) {
                             var c = Object.keys(this.tokens.links);
                             if (c.length > 0)
-                                for (; null != (a = this.tokenizer.rules.inline.reflinkSearch.exec(l));) c.includes(a[0].slice(a[0].lastIndexOf("[") + 1, -1)) && (l = l.slice(0, a.index) + "[" + Q("a", a[0].length - 2) + "]" + l.slice(this.tokenizer.rules.inline.reflinkSearch.lastIndex))
+                                for (; null != (a = this.tokenizer.rules.inline.reflinkSearch.exec(l));) c.includes(a[0].slice(a[0].lastIndexOf("[") + 1, -1)) && (l = l.slice(0, a.index) + "[" + G("a", a[0].length - 2) + "]" + l.slice(this.tokenizer.rules.inline.reflinkSearch.lastIndex))
                         }
-                        for (; null != (a = this.tokenizer.rules.inline.blockSkip.exec(l));) l = l.slice(0, a.index) + "[" + Q("a", a[0].length - 2) + "]" + l.slice(this.tokenizer.rules.inline.blockSkip.lastIndex);
+                        for (; null != (a = this.tokenizer.rules.inline.blockSkip.exec(l));) l = l.slice(0, a.index) + "[" + G("a", a[0].length - 2) + "]" + l.slice(this.tokenizer.rules.inline.blockSkip.lastIndex);
                         for (; e;)
                             if (o || (s = ""), o = !1, r = this.tokenizer.escape(e)) e = e.substring(r.raw.length), t.push(r);
                             else if (r = this.tokenizer.tag(e, n, i)) e = e.substring(r.raw.length), n = r.inLink, i = r.inRawBlock, t.push(r);
                         else if (r = this.tokenizer.link(e)) e = e.substring(r.raw.length), "link" === r.type && (r.tokens = this.inlineTokens(r.text, [], !0, i)), t.push(r);
                         else if (r = this.tokenizer.reflink(e, this.tokens.links)) e = e.substring(r.raw.length), "link" === r.type && (r.tokens = this.inlineTokens(r.text, [], !0, i)), t.push(r);
                         else if (r = this.tokenizer.strong(e, l, s)) e = e.substring(r.raw.length), r.tokens = this.inlineTokens(r.text, [], n, i), t.push(r);
                         else if (r = this.tokenizer.em(e, l, s)) e = e.substring(r.raw.length), r.tokens = this.inlineTokens(r.text, [], n, i), t.push(r);
                         else if (r = this.tokenizer.codespan(e)) e = e.substring(r.raw.length), t.push(r);
                         else if (r = this.tokenizer.br(e)) e = e.substring(r.raw.length), t.push(r);
                         else if (r = this.tokenizer.del(e)) e = e.substring(r.raw.length), r.tokens = this.inlineTokens(r.text, [], n, i), t.push(r);
-                        else if (r = this.tokenizer.autolink(e, G)) e = e.substring(r.raw.length), t.push(r);
-                        else if (n || !(r = this.tokenizer.url(e, G))) {
-                            if (r = this.tokenizer.inlineText(e, i, Y)) e = e.substring(r.raw.length), s = r.raw.slice(-1), o = !0, t.push(r);
+                        else if (r = this.tokenizer.autolink(e, Y)) e = e.substring(r.raw.length), t.push(r);
+                        else if (n || !(r = this.tokenizer.url(e, Y))) {
+                            if (r = this.tokenizer.inlineText(e, i, Q)) e = e.substring(r.raw.length), s = r.raw.slice(-1), o = !0, t.push(r);
                             else if (e) {
                                 var u = "Infinite loop on byte: " + e.charCodeAt(0);
                                 if (this.options.silent) {
                                     console.error(u);
                                     break
                                 }
                                 throw new Error(u)
@@ -824,20 +824,20 @@
                             return {
                                 block: J,
                                 inline: Z
                             }
                         }
                     }], (i = null) && e(n.prototype, i), r && e(n, r), t
                 }(),
-                X = i.defaults,
-                K = S,
+                K = i.defaults,
+                X = S,
                 ee = k,
                 te = function() {
                     function e(e) {
-                        this.options = e || X
+                        this.options = e || K
                     }
                     var t = e.prototype;
                     return t.code = function(e, t, n) {
                         var i = (t || "").match(/\S*/)[0];
                         if (this.options.highlight) {
                             var r = this.options.highlight(e, i);
                             null != r && r !== e && (n = !0, e = r)
@@ -874,19 +874,19 @@
                     }, t.codespan = function(e) {
                         return "<code>" + e + "</code>"
                     }, t.br = function() {
                         return this.options.xhtml ? "<br/>" : "<br>"
                     }, t.del = function(e) {
                         return "<del>" + e + "</del>"
                     }, t.link = function(e, t, n) {
-                        if (null === (e = K(this.options.sanitize, this.options.baseUrl, e))) return n;
+                        if (null === (e = X(this.options.sanitize, this.options.baseUrl, e))) return n;
                         var i = '<a href="' + ee(e) + '"';
                         return t && (i += ' title="' + t + '"'), i += ">" + n + "</a>"
                     }, t.image = function(e, t, n) {
-                        if (null === (e = K(this.options.sanitize, this.options.baseUrl, e))) return n;
+                        if (null === (e = X(this.options.sanitize, this.options.baseUrl, e))) return n;
                         var i = '<img src="' + e + '" alt="' + n + '"';
                         return t && (i += ' title="' + t + '"'), i += this.options.xhtml ? "/>" : ">"
                     }, t.text = function(e) {
                         return e
                     }, e
                 }(),
                 ne = function() {
@@ -945,64 +945,64 @@
                         return new e(n).parse(t)
                     }, e.parseInline = function(t, n) {
                         return new e(n).parseInline(t)
                     };
                     var t = e.prototype;
                     return t.parse = function(e, t) {
                         void 0 === t && (t = !0);
-                        var n, i, r, a, o, s, l, c, u, p, d, h, f, _, m, v, g, b, y = "",
+                        var n, i, r, a, o, s, l, c, u, d, p, h, f, _, m, v, g, b, y = "",
                             k = e.length;
-                        for (n = 0; n < k; n++) switch ((p = e[n]).type) {
+                        for (n = 0; n < k; n++) switch ((d = e[n]).type) {
                             case "space":
                                 continue;
                             case "hr":
                                 y += this.renderer.hr();
                                 continue;
                             case "heading":
-                                y += this.renderer.heading(this.parseInline(p.tokens), p.depth, ae(this.parseInline(p.tokens, this.textRenderer)), this.slugger);
+                                y += this.renderer.heading(this.parseInline(d.tokens), d.depth, ae(this.parseInline(d.tokens, this.textRenderer)), this.slugger);
                                 continue;
                             case "code":
-                                y += this.renderer.code(p.text, p.lang, p.escaped);
+                                y += this.renderer.code(d.text, d.lang, d.escaped);
                                 continue;
                             case "table":
-                                for (c = "", l = "", a = p.header.length, i = 0; i < a; i++) l += this.renderer.tablecell(this.parseInline(p.tokens.header[i]), {
+                                for (c = "", l = "", a = d.header.length, i = 0; i < a; i++) l += this.renderer.tablecell(this.parseInline(d.tokens.header[i]), {
                                     header: !0,
-                                    align: p.align[i]
+                                    align: d.align[i]
                                 });
-                                for (c += this.renderer.tablerow(l), u = "", a = p.cells.length, i = 0; i < a; i++) {
-                                    for (l = "", o = (s = p.tokens.cells[i]).length, r = 0; r < o; r++) l += this.renderer.tablecell(this.parseInline(s[r]), {
+                                for (c += this.renderer.tablerow(l), u = "", a = d.cells.length, i = 0; i < a; i++) {
+                                    for (l = "", o = (s = d.tokens.cells[i]).length, r = 0; r < o; r++) l += this.renderer.tablecell(this.parseInline(s[r]), {
                                         header: !1,
-                                        align: p.align[r]
+                                        align: d.align[r]
                                     });
                                     u += this.renderer.tablerow(l)
                                 }
                                 y += this.renderer.table(c, u);
                                 continue;
                             case "blockquote":
-                                u = this.parse(p.tokens), y += this.renderer.blockquote(u);
+                                u = this.parse(d.tokens), y += this.renderer.blockquote(u);
                                 continue;
                             case "list":
-                                for (d = p.ordered, h = p.start, f = p.loose, a = p.items.length, u = "", i = 0; i < a; i++) v = (m = p.items[i]).checked, g = m.task, _ = "", m.task && (b = this.renderer.checkbox(v), f ? m.tokens.length > 0 && "text" === m.tokens[0].type ? (m.tokens[0].text = b + " " + m.tokens[0].text, m.tokens[0].tokens && m.tokens[0].tokens.length > 0 && "text" === m.tokens[0].tokens[0].type && (m.tokens[0].tokens[0].text = b + " " + m.tokens[0].tokens[0].text)) : m.tokens.unshift({
+                                for (p = d.ordered, h = d.start, f = d.loose, a = d.items.length, u = "", i = 0; i < a; i++) v = (m = d.items[i]).checked, g = m.task, _ = "", m.task && (b = this.renderer.checkbox(v), f ? m.tokens.length > 0 && "text" === m.tokens[0].type ? (m.tokens[0].text = b + " " + m.tokens[0].text, m.tokens[0].tokens && m.tokens[0].tokens.length > 0 && "text" === m.tokens[0].tokens[0].type && (m.tokens[0].tokens[0].text = b + " " + m.tokens[0].tokens[0].text)) : m.tokens.unshift({
                                     type: "text",
                                     text: b
                                 }) : _ += b), _ += this.parse(m.tokens, f), u += this.renderer.listitem(_, g, v);
-                                y += this.renderer.list(u, d, h);
+                                y += this.renderer.list(u, p, h);
                                 continue;
                             case "html":
-                                y += this.renderer.html(p.text);
+                                y += this.renderer.html(d.text);
                                 continue;
                             case "paragraph":
-                                y += this.renderer.paragraph(this.parseInline(p.tokens));
+                                y += this.renderer.paragraph(this.parseInline(d.tokens));
                                 continue;
                             case "text":
-                                for (u = p.tokens ? this.parseInline(p.tokens) : p.text; n + 1 < k && "text" === e[n + 1].type;) u += "\n" + ((p = e[++n]).tokens ? this.parseInline(p.tokens) : p.text);
+                                for (u = d.tokens ? this.parseInline(d.tokens) : d.text; n + 1 < k && "text" === e[n + 1].type;) u += "\n" + ((d = e[++n]).tokens ? this.parseInline(d.tokens) : d.text);
                                 y += t ? this.renderer.paragraph(u) : u;
                                 continue;
                             default:
-                                var w = 'Token with "' + p.type + '" type was not found.';
+                                var w = 'Token with "' + d.type + '" type was not found.';
                                 if (this.options.silent) return void console.error(w);
                                 throw new Error(w)
                         }
                         return y
                     }, t.parseInline = function(e, t) {
                         t = t || this.renderer;
                         var n, i, r = "",
@@ -1043,19 +1043,19 @@
                                 if (this.options.silent) return void console.error(o);
                                 throw new Error(o)
                         }
                         return r
                     }, e
                 }(),
                 se = O,
-                le = M,
+                le = P,
                 ce = k,
                 ue = i.getDefaults,
-                pe = i.changeDefaults,
-                de = i.defaults;
+                de = i.changeDefaults,
+                pe = i.defaults;
 
             function he(e, t, n) {
                 if (null == e) throw new Error("marked(): input parameter is undefined or null");
                 if ("string" != typeof e) throw new Error("marked(): input parameter is of type " + Object.prototype.toString.call(e) + ", string expected");
                 if ("function" == typeof t && (n = t, t = null), t = se({}, he.defaults, t || {}), le(t), n) {
                     var i, r = t.highlight;
                     try {
@@ -1089,31 +1089,31 @@
                     return t.walkTokens && he.walkTokens(s, t.walkTokens), oe.parse(s, t)
                 } catch (e) {
                     if (e.message += "\nPlease report this to https://github.com/markedjs/marked.", t.silent) return "<p>An error occurred:</p><pre>" + ce(e.message + "", !0) + "</pre>";
                     throw e
                 }
             }
             return he.options = he.setOptions = function(e) {
-                return se(he.defaults, e), pe(he.defaults), he
-            }, he.getDefaults = ue, he.defaults = de, he.use = function(e) {
+                return se(he.defaults, e), de(he.defaults), he
+            }, he.getDefaults = ue, he.defaults = pe, he.use = function(e) {
                 var t = se({}, e);
                 if (e.renderer && function() {
                         var n = he.defaults.renderer || new te,
                             i = function(t) {
                                 var i = n[t];
                                 n[t] = function() {
                                     for (var r = arguments.length, a = new Array(r), o = 0; o < r; o++) a[o] = arguments[o];
                                     var s = e.renderer[t].apply(n, a);
                                     return !1 === s && (s = i.apply(n, a)), s
                                 }
                             };
                         for (var r in e.renderer) i(r);
                         t.renderer = n
                     }(), e.tokenizer && function() {
-                        var n = he.defaults.tokenizer || new B,
+                        var n = he.defaults.tokenizer || new N,
                             i = function(t) {
                                 var i = n[t];
                                 n[t] = function() {
                                     for (var r = arguments.length, a = new Array(r), o = 0; o < r; o++) a[o] = arguments[o];
                                     var s = e.tokenizer[t].apply(n, a);
                                     return !1 === s && (s = i.apply(n, a)), s
                                 }
@@ -1133,16 +1133,16 @@
                     switch (t(a), a.type) {
                         case "table":
                             for (var o, s = n(a.tokens.header); !(o = s()).done;) {
                                 var l = o.value;
                                 he.walkTokens(l, t)
                             }
                             for (var c, u = n(a.tokens.cells); !(c = u()).done;)
-                                for (var p, d = n(c.value); !(p = d()).done;) {
-                                    var h = p.value;
+                                for (var d, p = n(c.value); !(d = p()).done;) {
+                                    var h = d.value;
                                     he.walkTokens(h, t)
                                 }
                             break;
                         case "list":
                             he.walkTokens(a.items, t);
                             break;
                         default:
@@ -1156,15 +1156,15 @@
                 try {
                     var n = V.lexInline(e, t);
                     return t.walkTokens && he.walkTokens(n, t.walkTokens), oe.parseInline(n, t)
                 } catch (e) {
                     if (e.message += "\nPlease report this to https://github.com/markedjs/marked.", t.silent) return "<p>An error occurred:</p><pre>" + ce(e.message + "", !0) + "</pre>";
                     throw e
                 }
-            }, he.Parser = oe, he.parser = oe.parse, he.Renderer = te, he.TextRenderer = ne, he.Lexer = V, he.lexer = V.lex, he.Tokenizer = B, he.Slugger = ie, he.parse = he, he
+            }, he.Parser = oe, he.parser = oe.parse, he.Renderer = te, he.TextRenderer = ne, he.Lexer = V, he.lexer = V.lex, he.Tokenizer = N, he.Slugger = ie, he.parse = he, he
         }, "object" == typeof n && void 0 !== t ? t.exports = r() : "function" == typeof define && define.amd ? define(r) : (i = "undefined" != typeof globalThis ? globalThis : i || self).marked = r()
     }, {}],
     2: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
@@ -1201,30 +1201,30 @@
                 for (var t = arguments.length, n = Array(t), i = 0; i < t; i++) n[i] = arguments[i];
                 var a = !0,
                     o = !1,
                     s = void 0;
                 try {
                     for (var l, c = n[Symbol.iterator](); !(a = (l = c.next()).done); a = !0) {
                         var u = l.value,
-                            p = !0,
-                            d = !1,
+                            d = !0,
+                            p = !1,
                             h = void 0;
                         try {
-                            for (var f, _ = u.accept_command[Symbol.iterator](); !(p = (f = _.next()).done); p = !0) {
+                            for (var f, _ = u.accept_command[Symbol.iterator](); !(d = (f = _.next()).done); d = !0) {
                                 var m = f.value;
                                 if (m in this.command2handler) throw new Error("Conflict command handler: both " + this.command2handler[m] + " and " + u + " accepts '" + m + "' command");
                                 this.command2handler[m] = u
                             }
                         } catch (e) {
-                            d = !0, h = e
+                            p = !0, h = e
                         } finally {
                             try {
-                                !p && _.return && _.return()
+                                !d && _.return && _.return()
                             } finally {
-                                if (d) throw h
+                                if (p) throw h
                             }
                         }
                     }
                 } catch (e) {
                     o = !0, s = e
                 } finally {
                     try {
@@ -1272,15 +1272,15 @@
                         var t = r.b64toBlob(e.spec.content);
                         saveAs(t, e.spec.name, {}, !1)
                     }
                 }]), e
             }();
         n.DownloadHandler = a
     }, {
-        "../utils": 27
+        "../utils": 28
     }],
     4: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
@@ -1308,16 +1308,16 @@
                         var t = e.spec;
                         void 0 !== t.title && (document.title = t.title), void 0 !== t.auto_scroll_bottom && (a.state.AutoScrollBottom = t.auto_scroll_bottom), void 0 !== t.output_animation && (a.config.outputAnimation = t.output_animation, t.output_animation ? document.body.classList.remove("no-animation") : document.body.classList.add("no-animation")), void 0 !== t.http_pull_interval && a.state.CurrentSession instanceof r.HttpSession && a.state.CurrentSession.change_pull_interval(t.http_pull_interval), void 0 !== t.input_panel_min_height && (a.state.InputPanelMinHeight = t.input_panel_min_height), void 0 !== t.input_panel_init_height && (a.state.InputPanelInitHeight = t.input_panel_init_height), void 0 !== t.input_panel_fixed && (a.state.FixedInputPanel = t.input_panel_fixed), void 0 !== t.input_auto_focus && (a.state.AutoFocusOnInput = t.input_auto_focus), void 0 !== t.output_max_width && $("#output-container").css("max-width", t.output_max_width)
                     }
                 }]), e
             }();
         n.EnvSettingHandler = o
     }, {
-        "../session": 24,
-        "../state": 25
+        "../session": 25,
+        "../state": 26
     }],
     5: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
@@ -1325,195 +1325,194 @@
                 }
             }
             return function(t, n, i) {
                 return n && e(t.prototype, n), i && e(t, i), t
             }
         }();
 
-        function r(e) {
-            if (Array.isArray(e)) {
-                for (var t = 0, n = Array(e.length); t < e.length; t++) n[t] = e[t];
-                return n
-            }
-            return Array.from(e)
-        }
-
-        function a(e, t) {
+        function r(e, t) {
             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
         }
         Object.defineProperty(n, "__esModule", {
             value: !0
         });
-        var o = e("../utils"),
-            s = e("../state"),
-            l = e("../models/input"),
-            c = e("../ui"),
-            u = e("../i18n"),
-            p = function() {
+        var a = e("../utils"),
+            o = e("../state"),
+            s = e("../models/input"),
+            l = e("../ui"),
+            c = e("../i18n"),
+            u = function() {
                 function e(t, n) {
-                    a(this, e), this.accept_command = ["input", "input_group", "update_input", "destroy_form"], this.session = t, this.container_elem = n, this.form_ctrls = new o.LRUMap
+                    r(this, e), this.accept_command = ["input", "input_group", "update_input", "destroy_form"], this.session = t, this.container_elem = n, this.form_ctrls = new a.LRUMap
                 }
                 return i(e, [{
                     key: "_after_show_form",
                     value: function() {
                         setTimeout((function() {
                             var e = $("#input-cards > .card")[0];
                             e.style.height = "unset", e.style.width = "unset"
-                        }), 50), c.show_input();
+                        }), 50), l.show_input();
                         var e = this.form_ctrls.get_top();
-                        e && e[e.length - 1].after_show(), s.state.AutoFocusOnInput && $('[auto_focus="true"]').focus()
+                        e && e[e.length - 1].after_show(), o.state.AutoFocusOnInput && $('[auto_focus="true"]').focus()
                     }
                 }, {
                     key: "_activate_form",
                     value: function(e, t) {
                         var n = this,
                             i = this.form_ctrls.get_value(e),
                             r = i[i.length - 1];
-                        if (r === t || void 0 === t) return r.element.show(s.state.ShowDuration, (function() {
+                        if (r === t || void 0 === t) return r.element.show(o.state.ShowDuration, (function() {
                             n._after_show_form()
                         }));
                         this.form_ctrls.move_to_top(e), t.element.hide(100, (function() {
                             var e = n.form_ctrls.get_top();
-                            e && e[e.length - 1].element.show(s.state.ShowDuration, (function() {
+                            e && e[e.length - 1].element.show(o.state.ShowDuration, (function() {
                                 n._after_show_form()
                             }))
                         }))
                     }
                 }, {
                     key: "handle_message",
                     value: function(e) {
                         var t = this,
                             n = this.form_ctrls.get_top(),
                             i = n && n[n.length - 1],
                             r = this.form_ctrls.get_value(e.task_id);
-                        if (void 0 === r && (this.form_ctrls.push(e.task_id, []), r = this.form_ctrls.get_value(e.task_id)), e.command in o.make_set(["input", "input_group"])) {
-                            var a = new d(this.session, e.task_id, e.spec);
-                            r.push(a), this.container_elem.append(a.create_element()), a.after_add_to_dom(), this._activate_form(e.task_id, i)
-                        } else if (e.command in o.make_set(["update_input"])) {
+                        if (void 0 === r && (this.form_ctrls.push(e.task_id, []), r = this.form_ctrls.get_value(e.task_id)), e.command in a.make_set(["input", "input_group"])) {
+                            var s = new d(this.session, e.task_id, e.spec);
+                            r.push(s), this.container_elem.append(s.create_element()), s.after_add_to_dom(), this._activate_form(e.task_id, i)
+                        } else if (e.command in a.make_set(["update_input"])) {
                             if (0 === r.length) return console.error("No form to current message. task_id:%s", e.task_id);
                             r[r.length - 1].dispatch_ctrl_message(e.spec)
                         } else if ("destroy_form" === e.command) {
                             if (0 === r.length) return console.error("No form to current message. task_id:%s", e.task_id);
-                            var l = r.pop();
-                            0 === r.length && this.form_ctrls.remove(e.task_id), n === r ? l.element.hide(100, (function() {
-                                l.element.remove(), c.close_input();
+                            var c = r.pop();
+                            0 === r.length && this.form_ctrls.remove(e.task_id), n === r ? c.element.hide(100, (function() {
+                                c.element.remove(), l.close_input();
                                 var e = t.form_ctrls.get_top();
-                                e && e[e.length - 1].element.show(s.state.ShowDuration, (function() {
+                                e && e[e.length - 1].element.show(o.state.ShowDuration, (function() {
                                     t._after_show_form()
                                 }))
-                            })) : (l.element.remove(), c.close_input())
+                            })) : (c.element.remove(), l.close_input())
                         }
                     }
                 }]), e
             }();
-        n.InputHandler = p;
+        n.InputHandler = u;
         var d = function() {
             function e(t, n, i) {
-                a(this, e), this.element = null, this.name2input = {}, this.show_count = 0, this.session = t, this.task_id = n, this.spec = i
+                r(this, e), this.element = null, this.name2input = {}, this.show_count = 0, this.session = t, this.task_id = n, this.spec = i
             }
             return i(e, [{
                 key: "create_element",
                 value: function() {
                     var t = this,
-                        n = '\n            <div class="card" style="display: none">\n                <h5 class="card-header">{{label}}</h5>\n                <div class="card-body">\n                    <form>\n                        <div class="input-container"></div>\n                        <div class="ws-form-submit-btns">\n                            <button type="submit" class="btn btn-primary">' + u.t("submit") + '</button>\n                            <button type="reset" class="btn btn-warning">' + u.t("reset") + '</button>\n                            {{#cancelable}}<button type="button" class="pywebio_cancel_btn btn btn-danger">' + u.t("cancel") + "</button>{{/cancelable}}\n                        </div>\n                    </form>\n                </div>\n            </div>",
+                        n = '\n            <div class="card" style="display: none">\n                <h5 class="card-header">{{label}}</h5>\n                <div class="card-body">\n                    <form>\n                        <div class="input-container"></div>\n                        <div class="ws-form-submit-btns">\n                            <button type="submit" class="btn btn-primary">' + c.t("submit") + '</button>\n                            <button type="reset" class="btn btn-warning">' + c.t("reset") + '</button>\n                            {{#cancelable}}<button type="button" class="pywebio_cancel_btn btn btn-danger">' + c.t("cancel") + "</button>{{/cancelable}}\n                        </div>\n                    </form>\n                </div>\n            </div>",
                         i = this,
-                        a = Mustache.render(n, {
+                        r = Mustache.render(n, {
                             label: this.spec.label,
                             cancelable: this.spec.cancelable
                         }),
-                        s = $(a);
-                    if (s.find(".pywebio_cancel_btn").on("click", (function(e) {
-                            s.find("button").prop("disabled", !0), i.session.send_message({
+                        o = $(r);
+                    if (o.find(".pywebio_cancel_btn").on("click", (function(e) {
+                            o.find("button").prop("disabled", !0), i.session.send_message({
                                 event: "from_cancel",
                                 task_id: i.task_id,
                                 data: null
                             })
                         })), this.spec.inputs.length && "actions" === this.spec.inputs[this.spec.inputs.length - 1].type) {
-                        var l = !0,
-                            c = !1,
-                            p = void 0;
+                        var s = !0,
+                            l = !1,
+                            u = void 0;
                         try {
-                            for (var d, h = this.spec.inputs[this.spec.inputs.length - 1].buttons[Symbol.iterator](); !(l = (d = h.next()).done); l = !0) {
+                            for (var d, p = this.spec.inputs[this.spec.inputs.length - 1].buttons[Symbol.iterator](); !(s = (d = p.next()).done); s = !0) {
                                 if ("submit" === d.value.type) {
-                                    s.find(".ws-form-submit-btns").hide();
+                                    o.find(".ws-form-submit-btns").hide();
                                     break
                                 }
                             }
                         } catch (e) {
-                            c = !0, p = e
+                            l = !0, u = e
                         } finally {
                             try {
-                                !l && h.return && h.return()
+                                !s && p.return && p.return()
                             } finally {
-                                if (c) throw p
+                                if (l) throw u
                             }
                         }
                     }
-                    var f = s.find(".input-container"),
-                        _ = function(n) {
+                    var h = o.find(".input-container"),
+                        f = function(n) {
                             var i = t.spec.inputs[n];
                             if (!(i.type in e.input_items)) throw new Error("Unknown input type '" + i.type + "'");
                             var r = new(0, e.input_items[i.type])(i, t.task_id, (function(e, n) {
                                 t.session.send_message({
                                     event: "input_event",
                                     task_id: t.task_id,
                                     data: {
                                         event_name: e,
                                         name: i.name,
                                         value: n.get_value()
                                     }
                                 })
                             }));
-                            t.name2input[i.name] = r, f.append(r.create_element())
+                            t.name2input[i.name] = r, h.append(r.create_element())
                         };
-                    for (var m in this.spec.inputs) _(m);
-                    return s.on("reset", "form", (function(e) {
+                    for (var _ in this.spec.inputs) f(_);
+                    return o.on("reset", "form", (function(e) {
                         for (var t in i.name2input) i.name2input[t].on_reset(e)
-                    })), s.on("submit", "form", (function(e) {
-                        for (var t in e.preventDefault(), s.find("button").prop("disabled", !0), i.name2input)
-                            if (!i.name2input[t].check_valid()) return s.find("button").prop("disabled", !1), o.error_alert(u.t("error_in_input"));
+                    })), o.on("submit", "form", (function(e) {
+                        for (var t in e.preventDefault(), o.find("button").prop("disabled", !0), i.name2input)
+                            if (!i.name2input[t].check_valid()) return o.find("button").prop("disabled", !1), a.error_alert(c.t("error_in_input"));
                         var n = [],
-                            a = [];
+                            r = [];
                         $.each(i.name2input, (function(e, t) {
-                            n.push(e), a.push(t.get_value())
+                            n.push(e), r.push(t.get_value())
                         }));
-                        var l = function(e, t) {},
-                            c = !0,
-                            p = !1,
+                        var s = function(e, t) {},
+                            l = !0,
+                            u = !1,
                             d = void 0;
                         try {
-                            for (var h, f = i.spec.inputs[Symbol.iterator](); !(c = (h = f.next()).done); c = !0) {
-                                if ("file" == h.value.type) {
-                                    l = i.make_progress();
+                            for (var p, h = i.spec.inputs[Symbol.iterator](); !(l = (p = h.next()).done); l = !0) {
+                                if ("file" == p.value.type) {
+                                    s = i.make_progress();
                                     break
                                 }
                             }
                         } catch (e) {
-                            p = !0, d = e
+                            u = !0, d = e
                         } finally {
                             try {
-                                !c && f.return && f.return()
+                                !l && h.return && h.return()
                             } finally {
-                                if (p) throw d
+                                if (u) throw d
                             }
                         }
-                        Promise.all(a).then((function(e) {
+                        Promise.all(r).then((function(e) {
                             var t = {},
-                                a = [];
-                            for (var s in n) t[n[s]] = e[s], "file" == i.spec.inputs[s].type && (t[n[s]] = [], a.push.apply(a, r(e[s])));
+                                r = [],
+                                o = function(o) {
+                                    var s = n[o],
+                                        l = e[o];
+                                    t[s] = l, "file" == i.spec.inputs[o].type && (t[s] = l.multiple ? [] : null, l.files.forEach((function(e) {
+                                        r.push(a.serialize_file(e, s))
+                                    })))
+                                };
+                            for (var l in n) o(l);
                             var c = {
                                 event: "from_submit",
                                 task_id: i.task_id,
                                 data: t
                             };
-                            a.length ? i.session.send_buffer(new Blob([o.serialize_json(c)].concat(a), {
+                            r.length ? i.session.send_buffer(new Blob([a.serialize_json(c)].concat(r), {
                                 type: "application/octet-stream"
-                            }), l) : i.session.send_message(c, l)
+                            }), s) : i.session.send_message(c, s)
                         }))
-                    })), this.element = s, s
+                    })), this.element = o, o
                 }
             }, {
                 key: "make_progress",
                 value: function() {
                     var e = $('<div class="progress" style="margin-top: 4px;">\n                        <div class="progress-bar bg-info progress-bar-striped progress-bar-animated" role="progressbar"\n                             style="width: 0%;" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100">0%\n                        </div>\n                    </div>');
                     this.element.find(".card-body").append(e);
                     var t = e.find(".progress-bar");
@@ -1560,37 +1559,37 @@
                             if (n) throw i
                         }
                     }
                 }
             }]), e
         }();
         d.input_items = {};
-        var h = !0,
-            f = !1,
-            _ = void 0;
+        var p = !0,
+            h = !1,
+            f = void 0;
         try {
-            for (var m, v = l.all_input_items[Symbol.iterator](); !(h = (m = v.next()).done); h = !0) {
-                var g = m.value;
-                d.register_inputitem(g)
+            for (var _, m = s.all_input_items[Symbol.iterator](); !(p = (_ = m.next()).done); p = !0) {
+                var v = _.value;
+                d.register_inputitem(v)
             }
         } catch (e) {
-            f = !0, _ = e
+            h = !0, f = e
         } finally {
             try {
-                !h && v.return && v.return()
+                !p && m.return && m.return()
             } finally {
-                if (f) throw _
+                if (h) throw f
             }
         }
     }, {
         "../i18n": 11,
-        "../models/input": 17,
-        "../state": 25,
-        "../ui": 26,
-        "../utils": 27
+        "../models/input": 18,
+        "../state": 26,
+        "../ui": 27,
+        "../utils": 28
     }],
     6: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
@@ -1673,24 +1672,24 @@
                         if (e.spec.scope && "#pywebio-scope-ROOT" !== e.spec.scope || (n = !0), 0 === e.spec.position) a.prepend(i);
                         else if (-1 === e.spec.position) a.append(i);
                         else {
                             var s = !0,
                                 l = !1,
                                 u = void 0;
                             try {
-                                for (var p, d = a[Symbol.iterator](); !(s = (p = d.next()).done); s = !0) {
-                                    var h = p.value,
+                                for (var d, p = a[Symbol.iterator](); !(s = (d = p.next()).done); s = !0) {
+                                    var h = d.value,
                                         f = $(h.children).eq(e.spec.position);
                                     e.spec.position >= 0 ? i.insertBefore(f) : i.insertAfter(f)
                                 }
                             } catch (e) {
                                 l = !0, u = e
                             } finally {
                                 try {
-                                    !s && d.return && d.return()
+                                    !s && p.return && p.return()
                                 } finally {
                                     if (l) throw u
                                 }
                             }
                         }
                         i.width() > this.container_elem.width() && i.wrap($(document.createElement("div")).css("overflow", "auto")), this.is_elem_visible(i) && 1 == a.length && (r.config.outputAnimation ? i.fadeIn({
                             complete: function() {
@@ -1731,91 +1730,141 @@
                             "margin-bottom": ""
                         }), void 0 !== e.spec.clear && $(e.spec.clear).empty(), void 0 !== e.spec.clear_before && $("" + e.spec.clear_before).prevAll().remove(), void 0 !== e.spec.clear_after && $(e.spec.clear_after + " ~ *").remove(), void 0 !== e.spec.scroll_to) {
                         var c = $("" + e.spec.scroll_to);
                         c.length ? a.body_scroll_to(c, e.spec.position) : console.error("Scope " + e.spec.scroll_to + " not found")
                     }
                     if (void 0 !== e.spec.clear_range && $("" + e.spec.clear_range[0]).length && $("" + e.spec.clear_range[1]).length) {
                         var u = [],
-                            p = !1;
+                            d = !1;
                         $(e.spec.clear_range[0] + " ~ *").each((function() {
-                            if (this.id === e.spec.clear_range[1]) return p = !0, !1;
+                            if (this.id === e.spec.clear_range[1]) return d = !0, !1;
                             u.push(this)
-                        })), p ? $(u).remove() : console.warn("clear_range not valid: can't find " + e.spec.clear_range[1] + " after " + e.spec.clear_range[0])
+                        })), d ? $(u).remove() : console.warn("clear_range not valid: can't find " + e.spec.clear_range[1] + " after " + e.spec.clear_range[0])
                     }
                     void 0 !== e.spec.remove && $("" + e.spec.remove).remove()
                 }
             }]), e
         }();
         n.OutputHandler = u
     }, {
-        "../models/output": 22,
-        "../state": 25,
-        "../utils": 27
+        "../models/output": 23,
+        "../state": 26,
+        "../utils": 28
     }],
     7: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
             }
             return function(t, n, i) {
                 return n && e(t.prototype, n), i && e(t, i), t
             }
         }();
+
+        function r(e) {
+            if (Array.isArray(e)) {
+                for (var t = 0, n = Array(e.length); t < e.length; t++) n[t] = e[t];
+                return n
+            }
+            return Array.from(e)
+        }
         Object.defineProperty(n, "__esModule", {
             value: !0
         });
-        var r = e("../models/pin"),
-            a = e("../state"),
-            o = function() {
+        var a = e("../models/pin"),
+            o = e("../state"),
+            s = e("../utils"),
+            l = e("../i18n"),
+            c = function() {
                 function e(t) {
                     ! function(e, t) {
                         if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                     }(this, e), this.accept_command = ["pin_value", "pin_update", "pin_wait", "pin_onchange"], this.session = t
                 }
                 return i(e, [{
                     key: "handle_message",
                     value: function(e) {
+                        var t = this;
                         if ("pin_value" === e.command) {
-                            var t = r.GetPinValue(e.spec.name),
-                                n = void 0 === t ? null : {
-                                    value: t
+                            var n = a.GetPinValue(e.spec.name),
+                                i = {
+                                    event: "js_yield",
+                                    task_id: e.task_id,
+                                    data: void 0 === n ? null : {
+                                        value: n
+                                    }
                                 };
-                            a.state.CurrentSession.send_message({
-                                event: "js_yield",
-                                task_id: e.task_id,
-                                data: n
-                            })
-                        } else if ("pin_update" === e.command) r.PinUpdate(e.spec.name, e.spec.attributes);
+                            this.submit(i, a.IsFileInput(e.spec.name))
+                        } else if ("pin_update" === e.command) a.PinUpdate(e.spec.name, e.spec.attributes);
                         else if ("pin_wait" === e.command) {
-                            var i = r.WaitChange(e.spec.names, e.spec.timeout);
-                            Promise.resolve(i).then((function(t) {
-                                a.state.CurrentSession.send_message({
+                            var r = a.WaitChange(e.spec.names, e.spec.timeout);
+                            Promise.resolve(r).then((function(n) {
+                                var i = {
                                     event: "js_yield",
                                     task_id: e.task_id,
-                                    data: t
-                                })
-                            })).catch((function(t) {
-                                console.error("error in `pin_wait`: %s", t), a.state.CurrentSession.send_message({
+                                    data: n
+                                };
+                                t.submit(i, a.IsFileInput(n.name))
+                            })).catch((function(n) {
+                                console.error("error in `pin_wait`: %s", n), t.submit({
                                     event: "js_yield",
                                     task_id: e.task_id,
                                     data: null
                                 })
                             }))
-                        } else "pin_onchange" === e.command && r.PinChangeCallback(e.spec.name, e.spec.callback_id, e.spec.clear)
+                        } else if ("pin_onchange" === e.command) {
+                            a.PinChangeCallback(e.spec.name, e.spec.callback_id ? function(n) {
+                                var i = {
+                                    event: "callback",
+                                    task_id: e.spec.callback_id,
+                                    data: {
+                                        value: n
+                                    }
+                                };
+                                t.submit(i, a.IsFileInput(e.spec.name))
+                            } : null, e.spec.clear)
+                        }
+                    }
+                }, {
+                    key: "submit",
+                    value: function(e) {
+                        var t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
+                        if (t && null !== e.data) {
+                            var n = e.data.value,
+                                i = n.multiple,
+                                a = n.files;
+                            e.data.value = i ? [] : null;
+                            var c = Toastify({
+                                text: "⏳" + l.t("file_uploading") + " 0%",
+                                duration: -1,
+                                gravity: "top",
+                                position: "center",
+                                backgroundColor: "#1565c0"
+                            });
+                            a.length > 0 && c.showToast(), o.state.CurrentSession.send_buffer(new Blob([s.serialize_json(e)].concat(r(a.map((function(e) {
+                                return s.serialize_file(e, "value")
+                            })))), {
+                                type: "application/octet-stream"
+                            }), (function(e, t) {
+                                c.toastElement.innerText = "⏳" + l.t("file_uploading") + " " + (e / t).toFixed(2) + "%", t - e < 100 && c.hideToast()
+                            }))
+                        } else o.state.CurrentSession.send_message(e)
                     }
                 }]), e
             }();
-        n.PinHandler = o
+        n.PinHandler = c
     }, {
-        "../models/pin": 23,
-        "../state": 25
+        "../i18n": 11,
+        "../models/pin": 24,
+        "../state": 26,
+        "../utils": 28
     }],
     8: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
@@ -1858,15 +1907,15 @@
                             small: "small" == e.size
                         }))
                     }
                 }]), e
             }();
         n.PopupHandler = o, o.current_elem = null
     }, {
-        "../models/output": 22,
+        "../models/output": 23,
         "./output": 6
     }],
     9: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
@@ -1917,15 +1966,15 @@
                             })
                         }))
                     }
                 }]), e
             }();
         n.ScriptHandler = a
     }, {
-        "../state": 25
+        "../state": 26
     }],
     10: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
@@ -1971,15 +2020,15 @@
                             });
                         n.showToast()
                     }
                 }]), e
             }();
         n.ToastHandler = a
     }, {
-        "../state": 25
+        "../state": 26
     }],
     11: [function(e, t, n) {
         "use strict";
         Object.defineProperty(n, "__esModule", {
             value: !0
         });
         var i = (navigator.language || navigator.userLanguage || "en").toLowerCase(),
@@ -1993,28 +2042,30 @@
                 file_size_exceed: 'File "%1" size exceeds limit: the size of a single file must not exceed %2',
                 file_total_size_exceed: "The total file size exceeds the limit: the total file size must not exceed %1",
                 submit: "Submit",
                 reset: "Reset",
                 cancel: "Cancel",
                 duplicated_pin_name: "This pin widget has expired (due to the output of a new pin widget with the same name).",
                 browse_file: "Browse",
-                duplicated_scope_name: "Error: The name of this scope is duplicated with the previous one!"
+                duplicated_scope_name: "Error: The name of this scope is duplicated with the previous one!",
+                file_uploading: "File Uploading..."
             },
             zh: {
                 disconnected_with_server: "与服务器连接已断开，请刷新页面重新操作",
                 connect_fail: "连接服务器失败!",
                 error_in_input: "输入项存在错误，请消除错误后再提交",
                 file_size_exceed: '文件"%1"大小超过限制: 单个文件大小不超过%2',
                 file_total_size_exceed: "文件总大小超过限制: 文件总大小不超过%1",
                 submit: "提交",
                 reset: "重置",
                 cancel: "取消",
                 duplicated_pin_name: "该 Pin widget 已失效（由于输出了新的同名 pin widget）",
                 browse_file: "浏览文件",
-                duplicated_scope_name: "错误: 此scope与已有scope重复!"
+                duplicated_scope_name: "错误: 此scope与已有scope重复!",
+                file_uploading: "文件上传中"
             },
             ru: {
                 disconnected_with_server: "Соединение с сервером потеряно, пожалуйста перезагрузите страницу",
                 connect_fail: "Ошибка подключения к серверу!",
                 error_in_input: "Пожалуйста, сначала исправьте ошибку",
                 file_size_exceed: 'Файл "%1" весит слишком много: максимально допустимый размер файла - %2',
                 file_total_size_exceed: "Общий размер файлов превышен: максимально допустимый объем - %1",
@@ -2045,14 +2096,27 @@
                 file_total_size_exceed: "اندازه کلی فایل از حد مجاز بیشتر است: اندازه کلی فایل نباید از %1 بیشتر باشد",
                 submit: "ارسال",
                 reset: "بازنشانی",
                 cancel: "لغو",
                 duplicated_pin_name: "این Pin Widget منقضی شده است (به دلیل خروجی یک Pin Widget جدید با نام یکسان)",
                 browse_file: "مرور",
                 duplicated_scope_name: "خطا: نام این Scope با نام قبلی تکراری است!"
+            },
+            uz: {
+                disconnected_with_server: "Server aloqasi uzildi, sahifani qayta yuklang",
+                connect_fail: "Serverga ulanib bo‘lmadi!",
+                error_in_input: "Iltimos, avval ma‘lumotlarni kiritish bilan bog‘liq xatoni tuzating",
+                file_size_exceed: "“%1” fayl hajmi cheklamadan oshib ketdi: ruxsat etilgan maksimal fayl hajmi - %2",
+                file_total_size_exceed: "Umumiy fayllar hajmi cheklamadan oshib ketdi: umumiy fayllar hajmi %1 dan oshmasligi kerak",
+                submit: "Yuborish",
+                reset: "Qaytadan",
+                cancel: "Bekor qilish",
+                duplicated_pin_name: "Bu pin widget muddati tugagan (xuddi shu nomdagi yangi pin widget chiqishi tufayli).",
+                browse_file: "Fayl yuklash",
+                duplicated_scope_name: "Xatolik: Ushbu Scope nomi avvalgisi bilan takrorlangan!"
             }
         };
 
         function o(e) {
             var t = arguments;
             return e.replace(/%%/g, "%% ").replace(/%(\d+)/g, (function(e, n) {
                 return t[n]
@@ -2063,15 +2127,15 @@
                 var l = n[s];
                 if (a[l] && a[l][e]) {
                     t = a[l][e];
                     break
                 }
             }
             if (null === t) throw Error('No translation for "' + e + '" in "' + i + '"');
-            for (var c = arguments.length, u = Array(c > 1 ? c - 1 : 0), p = 1; p < c; p++) u[p - 1] = arguments[p];
+            for (var c = arguments.length, u = Array(c > 1 ? c - 1 : 0), d = 1; d < c; d++) u[d - 1] = arguments[d];
             return o.apply(null, [t].concat(u))
         }
     }, {}],
     12: [function(e, t, n) {
         "use strict";
         Object.defineProperty(n, "__esModule", {
             value: !0
@@ -2080,16 +2144,16 @@
             r = e("./session"),
             a = e("./handlers/input"),
             o = e("./handlers/output"),
             s = e("./handlers/base"),
             l = e("./handlers/popup"),
             c = e("./utils"),
             u = e("./handlers/script"),
-            p = e("./handlers/download"),
-            d = e("./handlers/toast"),
+            d = e("./handlers/download"),
+            p = e("./handlers/toast"),
             h = e("./handlers/env"),
             f = e("./handlers/pin"),
             _ = e("./i18n");
         window.WebIO = {
             _state: i.state,
             startWebIOClient: function(e) {
                 for (var t in e.runtime_config) i.config[t] = e.runtime_config[t];
@@ -2104,16 +2168,16 @@
                             }));
                             var r = new o.OutputHandler(e, t),
                                 c = new a.InputHandler(e, n),
                                 _ = new l.PopupHandler(e),
                                 m = new s.SessionCtrlHandler(e),
                                 v = new u.ScriptHandler(e),
                                 g = new f.PinHandler(e),
-                                b = new p.DownloadHandler,
-                                y = new d.ToastHandler,
+                                b = new d.DownloadHandler,
+                                y = new p.ToastHandler,
                                 k = new h.EnvSettingHandler,
                                 w = new s.CommandDispatcher(r, c, _, m, v, b, y, k, g);
                             e.on_server_message((function(e) {
                                 try {
                                     w.dispatch_message(e) || console.error("Unknown command:%s", e.command)
                                 } catch (t) {
                                     console.error("Error(%s) in dispatch command: %s", t, e.command)
@@ -2134,20 +2198,320 @@
         "./handlers/input": 5,
         "./handlers/output": 6,
         "./handlers/pin": 7,
         "./handlers/popup": 8,
         "./handlers/script": 9,
         "./handlers/toast": 10,
         "./i18n": 11,
-        "./session": 24,
-        "./state": 25,
-        "./utils": 27
+        "./session": 25,
+        "./state": 26,
+        "./utils": 28
     }],
     13: [function(e, t, n) {
         "use strict";
+        var i = function(e, t) {
+                if (Array.isArray(e)) return e;
+                if (Symbol.iterator in Object(e)) return function(e, t) {
+                    var n = [],
+                        i = !0,
+                        r = !1,
+                        a = void 0;
+                    try {
+                        for (var o, s = e[Symbol.iterator](); !(i = (o = s.next()).done) && (n.push(o.value), !t || n.length !== t); i = !0);
+                    } catch (e) {
+                        r = !0, a = e
+                    } finally {
+                        try {
+                            !i && s.return && s.return()
+                        } finally {
+                            if (r) throw a
+                        }
+                    }
+                    return n
+                }(e, t);
+                throw new TypeError("Invalid attempt to destructure non-iterable instance")
+            },
+            r = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                return typeof e
+            } : function(e) {
+                return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+            };
+        Object.defineProperty(n, "__esModule", {
+            value: !0
+        });
+        var a = e("../session");
+
+        function o(e) {
+            return [e.join(""), e.map((function(e) {
+                return e.length
+            })).join("_"), e.length].join("_")
+        }
+
+        function s(e) {
+            for (var t = e.split("_"), n = parseInt(t[t.length - 1]), i = [], r = 0, a = 0; a < n; a++) {
+                var o = parseInt(t[t.length - 1 - n + a]);
+                i.push(e.substring(r, r + o)), r += o
+            }
+            return i
+        }
+
+        function l(e, t, n, i) {
+            if (e) {
+                var a = [];
+                try {
+                    a = Object.keys(e)
+                } catch (e) {}
+                a.forEach((function(a) {
+                    var s = e[a];
+                    i.push(a), a in t || (t[a] = {}), s && "object" == (void 0 === s ? "undefined" : r(s)) && !Array.isArray(s) ? l(s, t[a], n, i) : n[o(i)] = s, i.pop()
+                }))
+            }
+        }
+
+        function c(e) {
+            var t = {};
+            return l(e, {}, t, []), t
+        }
+
+        function u(e, t) {
+            return JSON.parse(JSON.stringify(e), (function(e, n) {
+                if ("object" === (void 0 === n ? "undefined" : r(n)) && n.__pywebio_js_function__ === t && "params" in n && "body" in n) try {
+                    return new(Function.prototype.bind.apply(Function, [null].concat(function(e) {
+                        if (Array.isArray(e)) {
+                            for (var t = 0, n = Array(e.length); t < e.length; t++) n[t] = e[t];
+                            return n
+                        }
+                        return Array.from(e)
+                    }(n.params), [n.body])))
+                } catch (e) {
+                    return console.error("Parse js function error: %s", e), null
+                }
+                return n
+            }))
+        }
+
+        function d(e, t) {
+            try {
+                for (var n = arguments.length, i = Array(n > 2 ? n - 2 : 0), r = 2; r < n; r++) i[r - 2] = arguments[r];
+                "function" == typeof t && t.bind(this).apply(void 0, i)
+            } catch (t) {
+                console.error("Error on %s function:\n", e, t)
+            }
+        }
+        var p = {
+                rowMultiSelectWithClick: !0,
+                groupSelectsChildren: !0,
+                groupSelectsFiltered: !0,
+                enableCellTextSelection: !0,
+                ensureDomOrder: !0,
+                autoGroupColumnDef: {
+                    pinned: "left"
+                },
+                enableCharts: !0,
+                enableRangeSelection: !0,
+                sideBar: {
+                    toolPanels: [{
+                        id: "columns",
+                        labelDefault: "Columns",
+                        labelKey: "columns",
+                        iconKey: "columns",
+                        toolPanel: "agColumnsToolPanel",
+                        minWidth: 225,
+                        width: 290,
+                        maxWidth: 400
+                    }, {
+                        id: "filters",
+                        labelDefault: "Filters",
+                        labelKey: "filters",
+                        iconKey: "filter",
+                        toolPanel: "agFiltersToolPanel",
+                        minWidth: 180,
+                        maxWidth: 400,
+                        width: 250
+                    }],
+                    position: "right"
+                }
+            },
+            h = {
+                wrapHeaderText: !0,
+                autoHeaderHeight: !0,
+                sortable: !0,
+                filter: !0,
+                resizable: !0,
+                enableValue: !0,
+                enableRowGroup: !0,
+                enablePivot: !0,
+                defaultAggFunc: "avg"
+            };
+        n.Datatable = {
+            handle_type: "datatable",
+            get_element: function(e) {
+                var t = Mustache.render('<div class="webio-datatable">\n<div class="ag-theme-{{theme}} ag-grid" style="width: 100%; height: {{height}}">\n    <div class="grid-loading">⌛️ Loading Datatable...</div>\n</div>\n<div class="ag-grid-cell-bar"></div>\n<div class="ag-grid-tools">\n    <div class="grid-status">\n        <div class="select-count">Selected <span class="ag-grid-row-count">0</span> <span\n                class="ag-grid-row-unit">row</span></div>\n        <div class="grid-unselect" style="display: flex;align-items: center;">\n            <div class="sep"></div>\n            <div class="act-btn">Unselect</div>\n        </div>\n    </div>\n    <div class="grid-actions"></div>\n</div>\n</div>', e),
+                    n = $(t);
+                e.field_args = u(e.field_args, e.js_func_key), e.path_args = u(e.path_args, e.js_func_key), e.grid_args = u(e.grid_args, e.js_func_key);
+                var f = "auto" == e.height,
+                    _ = function(e, t, n, a) {
+                        function s(e) {
+                            return e.charAt(0).toUpperCase() + e.slice(1)
+                        }
+                        var c = {},
+                            u = [],
+                            d = !0,
+                            p = !1,
+                            h = void 0;
+                        try {
+                            for (var f, _ = e[Symbol.iterator](); !(d = (f = _.next()).done); d = !0) {
+                                var m = f.value,
+                                    v = {};
+                                l(m, c, v, []), u.push(v)
+                            }
+                        } catch (e) {
+                            p = !0, h = e
+                        } finally {
+                            try {
+                                !d && _.return && _.return()
+                            } finally {
+                                if (p) throw h
+                            }
+                        }
+                        var g = {};
+                        return n.map((function(e) {
+                            var t = i(e, 2),
+                                n = t[0],
+                                r = t[1];
+                            g[o(n)] = r
+                        })), a && (c = JSON.parse(JSON.stringify(a), (function(e, t) {
+                            return t && "object" == (void 0 === t ? "undefined" : r(t)) && !Array.isArray(t) ? t : {}
+                        }))), {
+                            rowData: u,
+                            columnDefs: function e(t, n, i, r, a) {
+                                var l = [];
+                                return Object.keys(t).forEach((function(c) {
+                                    var u = t[c];
+                                    n.push(c);
+                                    var d = o(n);
+                                    if (Object.keys(u).length > 0) {
+                                        var p = Object.assign(Object.assign({}, a), r[d] || {});
+                                        l.push({
+                                            headerName: s(c.replace(/_/g, " ")),
+                                            children: e(u, n, i, r, p)
+                                        })
+                                    } else {
+                                        var h = Object.assign(Object.assign(Object.assign({
+                                            headerName: s(c.replace(/_/g, " ")),
+                                            field: d
+                                        }, a), i[c] || {}), r[d] || {});
+                                        l.push(h)
+                                    }
+                                    n.pop()
+                                })), l
+                            }(c, [], t, g, {})
+                        }
+                    }(e.records, e.field_args, e.path_args, e.column_order);
+                0 === e.actions.length ? n.find(".ag-grid-tools").hide() : n.find(".ag-grid-tools .grid-unselect, .ag-grid-tools .grid-actions").hide();
+                var m = void 0;
+                e.id_field && (m = function(t) {
+                    return t.data[o(e.id_field)]
+                });
+                var v = null,
+                    g = new Promise((function(e, t) {
+                        v = e
+                    }));
+                e.instance_id && (window["ag_grid_" + e.instance_id + "_promise"] = g);
+                var b = Object.assign(Object.assign(Object.assign({}, p), e.grid_args), {
+                        path2field: o,
+                        field2path: s,
+                        spec: e,
+                        flatten_row: c,
+                        getRowId: m,
+                        rowData: _.rowData,
+                        columnDefs: _.columnDefs,
+                        rowSelection: e.actions.length > 0 && (e.multiple_select ? "multiple" : "single"),
+                        defaultColDef: Object.assign(Object.assign({}, h), e.grid_args.defaultColDef || {}),
+                        getSelectedRowIDs: function() {
+                            var t = b.api.getSelectedNodes(),
+                                n = [],
+                                i = !0,
+                                r = !1,
+                                a = void 0;
+                            try {
+                                for (var o, s = t[Symbol.iterator](); !(i = (o = s.next()).done); i = !0) {
+                                    var l = o.value;
+                                    l.group || n.push(l.id)
+                                }
+                            } catch (e) {
+                                r = !0, a = e
+                            } finally {
+                                try {
+                                    !i && s.return && s.return()
+                                } finally {
+                                    if (r) throw a
+                                }
+                            }
+                            return e.id_field || (n = n.map((function(e) {
+                                return parseInt(e)
+                            }))), n
+                        },
+                        onGridReady: function(t) {
+                            v(b), f && b.api.setDomLayout("autoHeight");
+                            var i = n.find(".ag-grid")[0],
+                                r = Promise.resolve();
+                            0 === i.clientWidth && (r = new Promise((function(e) {
+                                new ResizeObserver((function(t, n) {
+                                    i.clientWidth > 0 && (n.disconnect(), e())
+                                })).observe(i)
+                            }))), r.then((function() {
+                                b.columnApi.autoSizeAllColumns();
+                                var e = 0;
+                                b.columnApi.getColumns().forEach((function(t) {
+                                    t.getColDef().hide || (e += t.getActualWidth())
+                                })), e < i.clientWidth && b.api.sizeColumnsToFit()
+                            })), e.actions.length > 0 && n.find(".ag-grid-tools").css("opacity", 1), n.find(".grid-unselect .act-btn").on("click", (function() {
+                                return b.api.deselectAll()
+                            }));
+                            var o = function(t) {
+                                var i = e.actions[t];
+                                if (null === i) n.find(".grid-actions").append('<div class="sep"></div>');
+                                else {
+                                    var r = $('<div class="act-btn">' + i + "</div>");
+                                    r.on("click", (function() {
+                                        a.pushData({
+                                            btn: parseInt(t),
+                                            rows: b.getSelectedRowIDs()
+                                        }, e.callback_id)
+                                    })), n.find(".grid-actions").append(r)
+                                }
+                            };
+                            for (var s in e.actions) o(s);
+                            d("agGrid.onGridReady()", e.grid_args.onGridReady, t)
+                        },
+                        onCellFocused: function(t) {
+                            var i = b.api.getDisplayedRowAtIndex(t.rowIndex),
+                                r = b.api.getValue(t.column, i);
+                            (void 0 === r && (r = ""), document.querySelector(".ag-grid-cell-bar").innerHTML = r, e.cell_content_bar) && n.find(".ag-grid-cell-bar").show();
+                            d("agGrid.onCellFocused()", e.grid_args.onCellFocused, t)
+                        },
+                        onSelectionChanged: function(t) {
+                            var i = b.getSelectedRowIDs();
+                            e.on_select && i.length > 0 && a.pushData({
+                                rows: i
+                            }, e.callback_id), n.find(".ag-grid-row-count").text(i.length), n.find(".ag-grid-row-unit").text(i.length > 1 ? "rows" : "row"), 0 === i.length && n.find(".ag-grid-tools .grid-unselect, .ag-grid-tools .grid-actions").hide(), i.length >= 1 && n.find(".ag-grid-tools .grid-unselect, .ag-grid-tools .grid-actions").fadeIn(200), d("agGrid.onSelectionChanged()", e.grid_args.onSelectionChanged, t)
+                        }
+                    }),
+                    y = e.enterprise_key ? "ag-grid-enterprise" : "ag-grid";
+                return requirejs([y], (function(t) {
+                    n.find(".grid-loading").remove(), new t.Grid(n.find(".ag-grid")[0], b), e.instance_id && (window["ag_grid_" + e.instance_id] = b)
+                })), n
+            }
+        }
+    }, {
+        "../session": 25
+    }],
+    14: [function(e, t, n) {
+        "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
             }
@@ -2229,18 +2593,18 @@
                     value: function() {
                         return this.submit_value
                     }
                 }]), t
             }(r.InputItem);
         n.Actions = o, o.accept_input_types = ["actions"]
     }, {
-        "../../state": 25,
-        "./base": 14
+        "../../state": 26,
+        "./base": 15
     }],
-    14: [function(e, t, n) {
+    15: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
@@ -2272,15 +2636,17 @@
                 key: "get_value",
                 value: function() {
                     throw new Error("Not implement!")
                 }
             }, {
                 key: "check_valid",
                 value: function() {
-                    return !0
+                    return this.update_input_helper(-1, {
+                        valid_status: 0
+                    }), !0
                 }
             }, {
                 key: "after_add_to_dom",
                 value: function() {}
             }, {
                 key: "after_show",
                 value: function(e) {}
@@ -2296,23 +2662,23 @@
                         help_text: "small.text-muted",
                         label: ">label"
                     };
                     for (var i in n) i in t && (this.element.find(n[i]).text(t[i]), delete t[i]);
                     var r = this.element.find("input,select,textarea");
                     if (e >= 0 && (r = r.eq(e)), "valid_status" in t) {
                         var a = t.valid_status ? "is-valid" : "is-invalid";
-                        0 === t.valid_status && (a = ""), r.removeClass("is-valid is-invalid").addClass(a), delete t.valid_status
+                        0 !== t.valid_status && null !== t.valid_status || (a = ""), r.removeClass("is-valid is-invalid").addClass(a), delete t.valid_status
                     }
                     r.prop(t)
                 }
             }]), e
         }();
         n.InputItem = r, r.accept_input_types = []
     }, {}],
-    15: [function(e, t, n) {
+    16: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
@@ -2415,18 +2781,18 @@
                             t.name === i.spec.name && n.push(JSON.parse(t.value))
                         })), n
                     }
                 }]), t
             }(r.InputItem);
         n.CheckboxRadio = s, s.accept_input_types = ["checkbox", "radio"]
     }, {
-        "../../utils": 27,
-        "./base": 14
+        "../../utils": 28,
+        "./base": 15
     }],
-    16: [function(e, t, n) {
+    17: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
@@ -2484,41 +2850,42 @@
                         var l = this;
                         return i.on("change", (function() {
                             l.files = [];
                             var t = 0;
                             l.valid = !0;
                             var n = i[0].files,
                                 r = !0,
-                                s = !1,
-                                c = void 0;
+                                a = !1,
+                                s = void 0;
                             try {
-                                for (var u, p = n[Symbol.iterator](); !(r = (u = p.next()).done); r = !0) {
-                                    var d = u.value;
+                                for (var c, u = n[Symbol.iterator](); !(r = (c = u.next()).done); r = !0) {
+                                    var d = c.value;
                                     if (t += d.size, l.spec.max_size && d.size > l.spec.max_size) l.valid = !1, l.update_input_helper(-1, {
                                         valid_status: !1,
                                         invalid_feedback: o.t("file_size_exceed", d.name, l._formate_size(l.spec.max_size))
                                     });
                                     else if (l.spec.max_total_size && t > l.spec.max_total_size) return l.valid = !1, void l.update_input_helper(-1, {
                                         valid_status: !1,
                                         invalid_feedback: o.t("file_total_size_exceed", l._formate_size(l.spec.max_total_size))
                                     });
                                     if (!l.valid) return;
                                     l.update_input_helper(-1, {
                                         valid_status: 0
-                                    }), l.files.push(a.serialize_file(d, e.name))
+                                    }), l.files.push(d)
                                 }
                             } catch (e) {
-                                s = !0, c = e
+                                a = !0, s = e
                             } finally {
                                 try {
-                                    !r && p.return && p.return()
+                                    !r && u.return && u.return()
                                 } finally {
-                                    if (s) throw c
+                                    if (a) throw s
                                 }
                             }
+                            e.onchange && l.on_input_event("change", l)
                         })), this.element
                     }
                 }, {
                     key: "_formate_size",
                     value: function(e) {
                         for (var t = ["Byte", "Kb", "Mb"], n = 0; n < t.length; n++) {
                             var i = t[n];
@@ -2537,50 +2904,53 @@
                     key: "check_valid",
                     value: function() {
                         return this.valid
                     }
                 }, {
                     key: "get_value",
                     value: function() {
-                        return this.files
+                        return {
+                            multiple: this.spec.multiple,
+                            files: this.files
+                        }
                     }
                 }, {
                     key: "after_add_to_dom",
                     value: function() {
                         bsCustomFileInput.init()
                     }
                 }]), t
             }(r.InputItem);
-        n.File = s, s.accept_input_types = ["file"]
+        n.FileUpload = s, s.accept_input_types = ["file"]
     }, {
         "../../i18n": 11,
-        "../../utils": 27,
-        "./base": 14
+        "../../utils": 28,
+        "./base": 15
     }],
-    17: [function(e, t, n) {
+    18: [function(e, t, n) {
         "use strict";
         Object.defineProperty(n, "__esModule", {
             value: !0
         });
         var i = e("./input"),
             r = e("./actions"),
             a = e("./checkbox_radio"),
             o = e("./textarea"),
             s = e("./file"),
             l = e("./select"),
             c = e("./slider");
-        n.all_input_items = [i.Input, r.Actions, a.CheckboxRadio, o.Textarea, s.File, l.Select, c.Slider], n.get_input_item_from_type = function(e) {
+        n.all_input_items = [i.Input, r.Actions, a.CheckboxRadio, o.Textarea, s.FileUpload, l.Select, c.Slider], n.get_input_item_from_type = function(e) {
             return u[e]
         };
         var u = {},
-            p = !0,
-            d = !1,
+            d = !0,
+            p = !1,
             h = void 0;
         try {
-            for (var f, _ = n.all_input_items[Symbol.iterator](); !(p = (f = _.next()).done); p = !0) {
+            for (var f, _ = n.all_input_items[Symbol.iterator](); !(d = (f = _.next()).done); d = !0) {
                 var m = f.value,
                     v = !0,
                     g = !1,
                     b = void 0;
                 try {
                     for (var y, k = m.accept_input_types[Symbol.iterator](); !(v = (y = k.next()).done); v = !0) {
                         var w = y.value;
@@ -2593,32 +2963,32 @@
                         !v && k.return && k.return()
                     } finally {
                         if (g) throw b
                     }
                 }
             }
         } catch (e) {
-            d = !0, h = e
+            p = !0, h = e
         } finally {
             try {
-                !p && _.return && _.return()
+                !d && _.return && _.return()
             } finally {
-                if (d) throw h
+                if (p) throw h
             }
         }
     }, {
-        "./actions": 13,
-        "./checkbox_radio": 15,
-        "./file": 16,
-        "./input": 18,
-        "./select": 19,
-        "./slider": 20,
-        "./textarea": 21
+        "./actions": 14,
+        "./checkbox_radio": 16,
+        "./file": 17,
+        "./input": 19,
+        "./select": 20,
+        "./slider": 21,
+        "./textarea": 22
     }],
-    18: [function(e, t, n) {
+    19: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
@@ -2717,19 +3087,19 @@
                         var e = this.element.find("input").val();
                         return "number" == this.spec.type ? e = parseInt(e) : "float" == this.spec.type && (e = parseFloat(e)), e
                     }
                 }]), t
             }(r.InputItem);
         n.Input = l, l.accept_input_types = ["text", "password", "number", "float", "color", "date", "range", "time", "email", "url", "datetime-local"]
     }, {
-        "../../state": 25,
-        "../../utils": 27,
-        "./base": 14
+        "../../state": 26,
+        "../../utils": 28,
+        "./base": 15
     }],
-    19: [function(e, t, n) {
+    20: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
@@ -2743,21 +3113,22 @@
         });
         var r = e("./base"),
             a = e("../../utils"),
             o = "\n{{#options}}\n<option {{#selected}}selected{{/selected}} {{#disabled}}disabled{{/disabled}}>{{label}}</option>\n{{/options}}\n";
         $.fn.selectpicker.Constructor.BootstrapVersion = "4";
         var s = function(e) {
             function t(e, n, i) {
-                return function(e, t) {
-                        if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                    }(this, t),
-                    function(e, t) {
-                        if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                        return !t || "object" != typeof t && "function" != typeof t ? e : t
-                    }(this, (t.__proto__ || Object.getPrototypeOf(t)).call(this, e, n, i))
+                ! function(e, t) {
+                    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+                }(this, t);
+                var r = function(e, t) {
+                    if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                    return !t || "object" != typeof t && "function" != typeof t ? e : t
+                }(this, (t.__proto__ || Object.getPrototypeOf(t)).call(this, e, n, i));
+                return r.use_bootstrap_select = !1, (!1 === e.native || void 0 === e.native && e.multiple && !a.is_mobile()) && (r.use_bootstrap_select = !0), r
             }
             return function(e, t) {
                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
                 e.prototype = Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         enumerable: !1,
@@ -2769,27 +3140,27 @@
                 key: "create_element",
                 value: function() {
                     var e = this,
                         t = a.deep_copy(this.spec),
                         n = t.name + "-" + Math.floor(Math.random() * Math.floor(9999));
                     t.id_name = n;
                     var i = Mustache.render('\n<div class="form-group">\n    {{#label}}<label for="{{id_name}}">{{label}}</label>{{/label}}\n    <select id="{{id_name}}" aria-describedby="{{id_name}}_help" class="form-control" {{#multiple}}multiple{{/multiple}}>\n        \n{{#options}}\n<option {{#selected}}selected{{/selected}} {{#disabled}}disabled{{/disabled}}>{{label}}</option>\n{{/options}}\n\n    </select>\n    <div class="invalid-feedback">{{invalid_feedback}}</div>\n    <div class="valid-feedback">{{valid_feedback}}</div>\n    <small id="{{id_name}}_help" class="form-text text-muted">{{help_text}}</small>\n</div>', t);
-                    return this.element = $(i), this.setup_select_options(this.element, t.options), this.element.find("select").selectpicker(), t.onblur && this.element.find("select").on("blur", (function(t) {
+                    return this.element = $(i), this.setup_select_options(this.element, t.options), this.use_bootstrap_select && this.element.find("select").selectpicker(), t.onblur && this.element.find("select").on("blur", (function(t) {
                         e.on_input_event("blur", e)
                     })), t.onchange && this.element.find("select").on("change", (function(t) {
                         e.on_input_event("change", e)
                     })), this.element
                 }
             }, {
                 key: "setup_select_options",
                 value: function(e, t) {
                     for (var n = e.find("select"), i = n.find("option"), r = 0; r < t.length; r++) i.eq(r).val(JSON.stringify(t[r].value));
                     var o = a.make_set(["type", "label", "invalid_feedback", "valid_feedback", "help_text", "options", "datalist", "multiple", "onchange", "onblur"]);
                     for (var s in this.spec) s in o || n.attr(s, this.spec[s]);
-                    n.selectpicker("refresh")
+                    this.use_bootstrap_select && n.selectpicker("refresh")
                 }
             }, {
                 key: "update_input",
                 value: function(e) {
                     var t = e.attributes;
                     if ("options" in t) {
                         var n = Mustache.render(o, {
@@ -2798,23 +3169,23 @@
                         this.element.find("select").empty().append(n), this.setup_select_options(this.element, t.options), delete t.options
                     }
                     if ("value" in t) {
                         this.element.find("option").prop("selected", !1);
                         var i = t.value;
                         this.spec.multiple || (i = [t.value]), this.element.find("option").each((function(e) {
                             var t = JSON.parse($(this).val()); - 1 != i.indexOf(t) && $(this).prop("selected", !0)
-                        })), this.element.find("select").selectpicker("render"), delete t.value
+                        })), this.use_bootstrap_select && this.element.find("select").selectpicker("render"), delete t.value
                     }
                     this.update_input_helper(-1, t)
                 }
             }, {
                 key: "on_reset",
                 value: function(e) {
                     var t = this;
-                    setTimeout((function() {
+                    this.use_bootstrap_select && setTimeout((function() {
                         t.element.find("select").selectpicker("render")
                     }), 100)
                 }
             }, {
                 key: "get_value",
                 value: function() {
                     var e = this.element.find("select").val();
@@ -2841,18 +3212,18 @@
                     }
                     return JSON.parse(e)
                 }
             }]), t
         }(r.InputItem);
         n.Select = s, s.accept_input_types = ["select"]
     }, {
-        "../../utils": 27,
-        "./base": 14
+        "../../utils": 28,
+        "./base": 15
     }],
-    20: [function(e, t, n) {
+    21: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
@@ -2920,18 +3291,18 @@
                         var e = this.element.find('input[type="range"]').val();
                         return e = this.spec.float ? parseFloat(e) : parseInt(e)
                     }
                 }]), t
             }(r.InputItem);
         n.Slider = o, o.accept_input_types = ["slider"]
     }, {
-        "../../utils": 27,
-        "./base": 14
+        "../../utils": 28,
+        "./base": 15
     }],
-    21: [function(e, t, n) {
+    22: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
@@ -2997,16 +3368,16 @@
                         var s = a.make_set(["value", "type", "label", "invalid_feedback", "valid_feedback", "help_text", "rows", "code", "onchange"]);
                         for (var l in n.code && n.required && (s.required = ""), this.spec) l in s || r.attr(l, this.spec[l]);
                         if (n.code) {
                             for (var c in !0 === n.code && (n.code = {
                                     mode: "text/plain"
                                 }), CodeMirror.modeURL = o.config.codeMirrorModeURL, this.spec.code) this.code_mirror_config[c] = this.spec.code[c];
                             var u = n.code.mode || "text/plain",
-                                p = CodeMirror.findModeByExtension(u) || CodeMirror.findModeByMIME(u);
-                            p && (this.code_mirror_config.mode = p.mode), (this.spec.readonly || this.spec.disabled) && (this.code_mirror_config.readOnly = "nocursor"), this.code_mirror_config.theme && "base16-light" !== this.code_mirror_config.theme && t.load_codemirror_theme(this.code_mirror_config.theme)
+                                d = CodeMirror.findModeByExtension(u) || CodeMirror.findModeByMIME(u);
+                            d && (this.code_mirror_config.mode = d.mode), (this.spec.readonly || this.spec.disabled) && (this.code_mirror_config.readOnly = "nocursor"), this.code_mirror_config.theme && "base16-light" !== this.code_mirror_config.theme && t.load_codemirror_theme(this.code_mirror_config.theme)
                         }
                         return this.element
                     }
                 }, {
                     key: "update_input",
                     value: function(e) {
                         var t = e.attributes;
@@ -3051,19 +3422,19 @@
                             r.id = n, r.rel = "stylesheet", r.type = "text/css", r.href = t.replace("%N", e), r.media = "all", i.appendChild(r)
                         }
                     }
                 }]), t
             }(r.InputItem);
         n.Textarea = s, s.accept_input_types = ["textarea"]
     }, {
-        "../../state": 25,
-        "../../utils": 27,
-        "./base": 14
+        "../../state": 26,
+        "../../utils": 28,
+        "./base": 15
     }],
-    22: [function(e, t, n) {
+    23: [function(e, t, n) {
         "use strict";
         var i = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         };
         Object.defineProperty(n, "__esModule", {
@@ -3071,15 +3442,16 @@
         });
         var r = e("../utils"),
             a = e("marked"),
             o = e("../session"),
             s = e("./pin"),
             l = e("../i18n"),
             c = e("../handlers/output"),
-            u = {
+            u = e("./datatable"),
+            d = {
                 handle_type: "text",
                 get_element: function(e) {
                     var t = e.inline ? $("<span></span>") : $("<p></p>");
                     return t.attr("style", "white-space: pre-wrap;"), t.append(document.createTextNode(e.content)), t
                 }
             };
 
@@ -3097,18 +3469,18 @@
                     e = Prism.highlight(e, Prism.languages[t])
                 } catch (e) {
                     console.error("Prism highlight error:" + e)
                 }
                 return n ? n(null, e) : e
             }
         });
-        var d = {
+        var h = {
                 handle_type: "scrollable",
                 get_element: function(e) {
-                    var t = x('<div>\n<div class="webio-scrollable{{#border}} scrollable-border{{/border}}" {{#keep_bottom}}tabindex="0"{{/keep_bottom}} \n    style="{{#min_height}}min-height: {{min_height}}px;{{/min_height}} {{#max_height}}max-height: {{max_height}}px;{{/max_height}}">\n    {{#contents}}\n        {{& pywebio_output_parse}}\n    {{/contents}}\n</div>\n</div>', e),
+                    var t = S('<div>\n<div class="webio-scrollable{{#border}} scrollable-border{{/border}}" {{#keep_bottom}}tabindex="0"{{/keep_bottom}} \n    style="{{#min_height}}min-height: {{min_height}}px;{{/min_height}} {{#max_height}}max-height: {{max_height}}px;{{/max_height}}">\n    {{#contents}}\n        {{& pywebio_output_parse}}\n    {{/contents}}\n</div>\n</div>', e),
                         n = t.find("> div");
                     if (e.keep_bottom) {
                         var i = !1;
                         n.on("focusin mouseenter", (function(e) {
                             i = !0
                         })).on("focusout mouseleave", (function(e) {
                             i = !1
@@ -3120,27 +3492,27 @@
                             childList: !0,
                             subtree: !0
                         })
                     }
                     return t
                 }
             },
-            h = {
+            f = {
                 handle_type: "scope",
                 get_element: function(e) {
-                    var t = x("<div>\n    {{#contents}}\n        {{& pywebio_output_parse}}\n    {{/contents}}\n</div>", e);
+                    var t = S("<div>\n    {{#contents}}\n        {{& pywebio_output_parse}}\n    {{/contents}}\n</div>", e);
                     return c.AfterCurrentOutputWidgetShow((function() {
                         if (0 !== $("#" + e.dom_id).length) {
                             var n = '<p style="color: grey; border:1px solid #ced4da; padding: .375rem .75rem;">' + l.t("duplicated_scope_name") + "</p>";
                             t.empty().html(n)
                         } else t.attr("id", e.dom_id)
                     })), t
                 }
             },
-            f = [u, {
+            _ = [d, {
                 handle_type: "markdown",
                 get_element: function(e) {
                     var t = a(e.content, e.options);
                     if (e.sanitize) try {
                         t = DOMPurify.sanitize(t)
                     } catch (e) {
                         console.log("Sanitize html failed: %s\nHTML: \n%s", e, t)
@@ -3180,15 +3552,15 @@
                             }
                         }
                     }
                     for (var s = Mustache.render('<div{{#group}} class="btn-group" role="group"{{/group}}>{{#buttons}} \n                                <button class="btn {{#color}}btn-{{#outline}}outline-{{/outline}}{{color}}{{/color}}{{#small}} btn-sm{{/small}}" {{#disabled}}disabled{{/disabled}}>{{label}}</button> \n                          {{/buttons}}</div>', e), l = $(s), c = l.find("button"), u = function(t) {
                             c.eq(t).on("click", (function(n) {
                                 o.pushData(e.buttons[t].value, e.callback_id)
                             }))
-                        }, p = 0; p < e.buttons.length; p++) u(p);
+                        }, d = 0; d < e.buttons.length; d++) u(d);
                     return l
                 }
             }, {
                 handle_type: "file",
                 get_element: function(e) {
                     var t = '<div><button type="button" class="btn btn-link">' + e.name + "</button></div>",
                         n = $(t),
@@ -3211,69 +3583,69 @@
                                 content: o,
                                 inline: !0
                             }), t[n].push(Object.assign({
                                 content: o
                             }, e.span[n + "," + a] || {}))
                         }
                     }
-                    return x('\n<table>\n    <tr>\n        {{#header}} \n        <th{{#col}} colspan="{{col}}"{{/col}}{{#row}} rowspan="{{row}}"{{/row}}>{{#content}}{{& pywebio_output_parse}}{{/content}}</th> \n        {{/header}}\n    </tr>\n      {{#tdata}} \n      <tr>\n        {{# . }} \n        <td{{#col}} colspan="{{col}}"{{/col}}{{#row}} rowspan="{{row}}"{{/row}}>{{#content}}{{& pywebio_output_parse}}{{/content}}</td> \n        {{/ . }} \n      </tr>\n      {{/tdata}}\n    \n</table>', {
+                    return S('\n<table>\n    <tr>\n        {{#header}} \n        <th{{#col}} colspan="{{col}}"{{/col}}{{#row}} rowspan="{{row}}"{{/row}}>{{#content}}{{& pywebio_output_parse}}{{/content}}</th> \n        {{/header}}\n    </tr>\n      {{#tdata}} \n      <tr>\n        {{# . }} \n        <td{{#col}} colspan="{{col}}"{{/col}}{{#row}} rowspan="{{row}}"{{/row}}>{{#content}}{{& pywebio_output_parse}}{{/content}}</td> \n        {{/ . }} \n      </tr>\n      {{/tdata}}\n    \n</table>', {
                         header: t[0],
                         tdata: t.slice(1)
                     })
                 }
             }, {
                 handle_type: "custom_widget",
                 get_element: function(e) {
-                    return x(e.template, e.data)
+                    return S(e.template, e.data)
                 }
             }, {
                 handle_type: "tabs",
                 get_element: function(e) {
                     e.tabs[0].checked = !0;
                     for (var t = 0; t < e.tabs.length; t++) e.tabs[t].index = t;
-                    return x('<div class="webio-tabs">\n{{#tabs}}\n    <input type="radio" class="toggle" name="{{#uniqueid}}name{{/uniqueid}}" id="{{#uniqueid}}name{{/uniqueid}}{{index}}" {{#checked}}checked{{/checked}}>\n    <label for="{{#uniqueid}}name{{/uniqueid}}{{index}}">{{title}}</label>\n    <div class="webio-tabs-content">\n    {{#content}}\n        {{& pywebio_output_parse}}\n    {{/content}}\n    </div>\n{{/tabs}}\n</div>', e)
+                    return S('<div class="webio-tabs">\n{{#tabs}}\n    <input type="radio" class="toggle" name="{{#uniqueid}}name{{/uniqueid}}" id="{{#uniqueid}}name{{/uniqueid}}{{index}}" {{#checked}}checked{{/checked}}>\n    <label for="{{#uniqueid}}name{{/uniqueid}}{{index}}">{{title}}</label>\n    <div class="webio-tabs-content">\n    {{#content}}\n        {{& pywebio_output_parse}}\n    {{/content}}\n    </div>\n{{/tabs}}\n</div>', e)
                 }
-            }, s.PinWidget, h, d],
-            _ = {},
-            m = !0,
-            v = !1,
-            g = void 0;
+            }, s.PinWidget, f, h, u.Datatable],
+            m = {},
+            v = !0,
+            g = !1,
+            b = void 0;
         try {
-            for (var b, y = f[Symbol.iterator](); !(m = (b = y.next()).done); m = !0) {
-                var k = b.value;
-                _[k.handle_type] = k
+            for (var y, k = _[Symbol.iterator](); !(v = (y = k.next()).done); v = !0) {
+                var w = y.value;
+                m[w.handle_type] = w
             }
         } catch (e) {
-            v = !0, g = e
+            g = !0, b = e
         } finally {
             try {
-                !m && y.return && y.return()
+                !v && k.return && k.return()
             } finally {
-                if (v) throw g
+                if (g) throw b
             }
         }
 
-        function w(e) {
-            if (!(e.type in _)) throw Error("Unknown type in getWidgetElement() :" + e.type);
-            var t = _[e.type].get_element(e);
+        function x(e) {
+            if (!(e.type in m)) throw Error("Unknown type in getWidgetElement() :" + e.type);
+            var t = m[e.type].get_element(e);
             if (1 != t.length && (t = $(document.createElement("div")).append(t)), e.style) {
                 var n = t.attr("style") || "";
                 t.attr({
                     style: n + ";" + e.style
                 })
             }
             return e.click_callback_id && (t.on("click", (function(t) {
                 o.pushData(null, e.click_callback_id)
             })), t.addClass("pywebio-clickable")), e.container_dom_id && (e.container_selector ? t.find(e.container_selector).attr("id", e.container_dom_id) : t.attr("id", e.container_dom_id)), t
         }
 
-        function x(e, t) {
+        function S(e, t) {
             var n = {};
             t.pywebio_output_parse = function() {
-                if (!this.type) return w({
+                if (!this.type) return x({
                     type: "text",
                     content: this,
                     inline: !0
                 })[0].outerHTML;
                 var e = "ph-" + r.randomid(10);
                 return n[e] = this, '<div id="' + e + '"></div>'
             };
@@ -3287,157 +3659,156 @@
             t.index = function() {
                 return a += 1
             };
             var o = p(Mustache.render(e, t));
             for (var s in n) {
                 var l = n[s];
                 try {
-                    var c = w(l);
+                    var c = x(l);
                     o.find("#" + s).replaceWith(c)
                 } catch (e) {
                     console.error("Error when render widget: \n%s\nSPEC:%s", e, JSON.stringify(l))
                 }
             }
             return o
         }
-        n.getWidgetElement = w, n.render_tpl = x
+        n.getWidgetElement = x, n.render_tpl = S
     }, {
         "../handlers/output": 6,
         "../i18n": 11,
-        "../session": 24,
-        "../utils": 27,
-        "./pin": 23,
+        "../session": 25,
+        "../utils": 28,
+        "./datatable": 13,
+        "./pin": 24,
         marked: 1
     }],
-    23: [function(e, t, n) {
+    24: [function(e, t, n) {
         "use strict";
         Object.defineProperty(n, "__esModule", {
             value: !0
         });
         var i = e("./input/index"),
             r = e("../i18n"),
             a = e("../handlers/output"),
             o = e("../utils"),
-            s = e("../session"),
-            l = {};
-        n.GetPinValue = function(e) {
-            if (null != l[e] && document.contains(l[e].element[0])) return l[e].get_value()
+            s = {};
+        n.IsFileInput = function(e) {
+            return void 0 !== s[e] && "file" == s[e].spec.type
+        }, n.GetPinValue = function(e) {
+            if (null != s[e] && document.contains(s[e].element[0])) return s[e].get_value()
         }, n.PinUpdate = function(e, t) {
-            l[e].update_input({
+            s[e].update_input({
                 attributes: t
             })
         };
-        var c = {},
-            u = {};
+        var l = {},
+            c = {};
         n.WaitChange = function(e, t) {
             var n = [],
                 i = {},
                 r = !0,
                 a = !1,
                 s = void 0;
             try {
-                for (var l, u = function() {
-                        var e = l.value;
+                for (var c, u = function() {
+                        var e = c.value;
                         n.push(new Promise((function(t) {
                             i[e] = function(e, t) {
                                 var n = o.randomid(10);
-                                e in c || (c[e] = {});
-                                return c[e][n] = t, n
+                                e in l || (l[e] = {});
+                                return l[e][n] = t, n
                             }(e, (function(n) {
                                 t({
                                     name: e,
                                     value: n
                                 })
                             }))
                         })))
-                    }, p = e[Symbol.iterator](); !(r = (l = p.next()).done); r = !0) u()
+                    }, d = e[Symbol.iterator](); !(r = (c = d.next()).done); r = !0) u()
             } catch (e) {
                 a = !0, s = e
             } finally {
                 try {
-                    !r && p.return && p.return()
+                    !r && d.return && d.return()
                 } finally {
                     if (a) throw s
                 }
             }
             return t && n.push(new Promise((function(e) {
                 setTimeout((function() {
                     e(null)
                 }), 1e3 * t)
             }))), Promise.race(n).then((function(t) {
                 var n = !0,
                     r = !1,
                     a = void 0;
                 try {
                     for (var o, s = e[Symbol.iterator](); !(n = (o = s.next()).done); n = !0) {
-                        var l = o.value,
-                            u = i[l];
-                        delete c[l][u]
+                        var c = o.value,
+                            u = i[c];
+                        delete l[c][u]
                     }
                 } catch (e) {
                     r = !0, a = e
                 } finally {
                     try {
                         !n && s.return && s.return()
                     } finally {
                         if (r) throw a
                     }
                 }
                 return t
             }))
         }, n.PinChangeCallback = function(e, t, n) {
-            e in u && !n || (u[e] = []), t && u[e].push((function(e) {
-                s.pushData(e, t)
-            }))
+            e in c && !n || (c[e] = []), t && c[e].push(t)
         }, n.PinWidget = {
             handle_type: "pin",
             get_element: function(e) {
                 var t = e.input;
-                if (t.name in l) {
+                if (t.name in s) {
                     var n = '<p style="color: grey; border:1px solid #ced4da; padding: .375rem .75rem;">' + r.t("duplicated_pin_name") + "</p>";
-                    l[t.name].element.replaceWith(n)
+                    s[t.name].element.replaceWith(n)
                 }
                 t.onchange = !0, t.onblur = !0;
                 var o = new(i.get_input_item_from_type(t.type))(t, null, (function(e, n) {
                     "change" == e && function(e, t) {
-                        var n = c[e] || {};
+                        var n = l[e] || {};
                         Object.keys(n).forEach((function(e) {
                             (0, n[e])(t)
                         }));
                         var i = !0,
                             r = !1,
                             a = void 0;
                         try {
-                            for (var o, s = (u[e] || [])[Symbol.iterator](); !(i = (o = s.next()).done); i = !0) {
+                            for (var o, s = (c[e] || [])[Symbol.iterator](); !(i = (o = s.next()).done); i = !0) {
                                 (0, o.value)(t)
                             }
                         } catch (e) {
                             r = !0, a = e
                         } finally {
                             try {
                                 !i && s.return && s.return()
                             } finally {
                                 if (r) throw a
                             }
                         }
                     }(t.name, n.get_value())
                 }));
-                return l[t.name] = o, a.AfterCurrentOutputWidgetShow((function() {
+                return s[t.name] = o, a.AfterCurrentOutputWidgetShow((function() {
                     o.after_add_to_dom(), o.after_show(!0)
                 })), o.create_element()
             }
         }
     }, {
         "../handlers/output": 6,
         "../i18n": 11,
-        "../session": 24,
-        "../utils": 27,
-        "./input/index": 17
+        "../utils": 28,
+        "./input/index": 18
     }],
-    24: [function(e, t, n) {
+    25: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
@@ -3550,17 +3921,17 @@
             }]), e
         }();
         n.WebSocketSession = c;
         var u = function() {
             function e(t) {
                 var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "index",
                     i = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 1e3;
-                r(this, e), this.api_url = t, this.pull_interval_ms = i, this.interval_pull_id = null, this.webio_session_id = "NEW", this.debug = !1, this._executed_command_msg_id = 0, this._closed = !1, this._session_create_callbacks = [], this._session_close_callbacks = [], this._on_server_message = function() {};
-                var a = new URL(t, window.location.href);
-                a.search = "?app=" + n, this.api_url = a.href
+                r(this, e), this.api_url = t, this.pull_interval_ms = i, this.interval_pull_id = null, this.webio_session_id = "", this.debug = !1, this.sender = null, this._executed_command_msg_id = -1, this._closed = !1, this._session_create_callbacks = [], this._session_close_callbacks = [], this._on_server_message = function() {};
+                var o = new URL(t, window.location.href);
+                o.search = "?app=" + n, this.api_url = o.href, this.sender = new a.ReliableSender(this._send.bind(this))
             }
             return i(e, [{
                 key: "on_session_create",
                 value: function(e) {
                     this._session_create_callbacks.push(e)
                 }
             }, {
@@ -3574,15 +3945,15 @@
                     this._on_server_message = e
                 }
             }, {
                 key: "start_session",
                 value: function() {
                     var e = this,
                         t = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
-                    this.debug = t, this.pull(), this.interval_pull_id = setInterval((function() {
+                    this.debug = t, this.webio_session_id = "NEW-" + a.randomid(24), this.pull(), this.interval_pull_id = setInterval((function() {
                         e.pull()
                     }), this.pull_interval_ms)
                 }
             }, {
                 key: "pull",
                 value: function() {
                     var e = this;
@@ -3591,92 +3962,128 @@
                         url: this.api_url + "&ack=" + this._executed_command_msg_id,
                         contentType: "application/json; charset=utf-8",
                         dataType: "json",
                         headers: {
                             "webio-session-id": this.webio_session_id
                         },
                         success: function(t, n, i) {
-                            l(e._session_create_callbacks, "session_create_callback"), e._on_request_success(t, n, i)
-                        },
-                        error: function() {
-                            console.error("Http pulling failed")
+                            l(e._session_create_callbacks, "session_create_callback"), e._on_request_success(t, n, i), e.webio_session_id.startsWith("NEW-") && (e.webio_session_id = e.webio_session_id.substring(4))
                         }
                     })
                 }
             }, {
                 key: "_on_request_success",
                 value: function(e, t, n) {
-                    if (e.seq != this._executed_command_msg_id) {
-                        this._executed_command_msg_id = e.seq;
-                        var i = n.getResponseHeader("webio-session-id");
-                        i && (this.webio_session_id = i);
-                        var r = !0,
-                            a = !1,
-                            o = void 0;
+                    this.sender.ack(e.ack);
+                    var i = this._executed_command_msg_id - e.seq + 1;
+                    if (!(e.commands.length <= i)) {
+                        this._executed_command_msg_id = e.seq + e.commands.length - 1;
+                        var r = n.getResponseHeader("webio-session-id");
+                        r && (this.webio_session_id = r);
+                        var a = !0,
+                            o = !1,
+                            s = void 0;
                         try {
-                            for (var s, l = e.commands[Symbol.iterator](); !(r = (s = l.next()).done); r = !0) {
-                                var c = s.value;
-                                this.debug && console.info(">>>", c), this._on_server_message(c)
+                            for (var l, c = e.commands.slice(i)[Symbol.iterator](); !(a = (l = c.next()).done); a = !0) {
+                                var u = l.value,
+                                    d = !0,
+                                    p = !1,
+                                    h = void 0;
+                                try {
+                                    for (var f, _ = u[Symbol.iterator](); !(d = (f = _.next()).done); d = !0) {
+                                        var m = f.value;
+                                        this.debug && console.info(">>>", m), this._on_server_message(m)
+                                    }
+                                } catch (e) {
+                                    p = !0, h = e
+                                } finally {
+                                    try {
+                                        !d && _.return && _.return()
+                                    } finally {
+                                        if (p) throw h
+                                    }
+                                }
                             }
                         } catch (e) {
-                            a = !0, o = e
+                            o = !0, s = e
                         } finally {
                             try {
-                                !r && l.return && l.return()
+                                !a && c.return && c.return()
                             } finally {
-                                if (a) throw o
+                                if (o) throw s
                             }
                         }
                     }
                 }
             }, {
                 key: "send_message",
                 value: function(e, t) {
-                    this.debug && console.info("<<<", e), this._send({
-                        data: JSON.stringify(e),
-                        contentType: "application/json; charset=utf-8"
-                    }, t)
+                    this.debug && console.info("<<<", e), this.sender.add_send_task({
+                        data: e,
+                        json: !0,
+                        onprogress: t
+                    })
                 }
             }, {
                 key: "send_buffer",
                 value: function(e, t) {
-                    this.debug && console.info("<<< Blob data..."), this._send({
+                    this.debug && console.info("<<< Blob data..."), this.sender.add_send_task({
                         data: e,
-                        cache: !1,
-                        processData: !1,
-                        contentType: "application/octet-stream"
-                    }, t)
+                        json: !1,
+                        onprogress: t
+                    }, !1)
                 }
             }, {
                 key: "_send",
                 value: function(e, t) {
-                    if (this.closed()) return a.error_alert(s.t("disconnected_with_server"));
-                    $.ajax(Object.assign(Object.assign({}, e), {
-                        type: "POST",
-                        url: this.api_url + "&ack=" + this._executed_command_msg_id,
-                        dataType: "json",
-                        headers: {
-                            "webio-session-id": this.webio_session_id
-                        },
-                        success: this._on_request_success.bind(this),
-                        xhr: function() {
-                            var e = new window.XMLHttpRequest;
-                            return e.upload.addEventListener("progress", (function(e) {
-                                e.lengthComputable && t && t(e.loaded, e.total)
-                            }), !1), e
-                        },
-                        error: function() {
-                            console.error("Http push blob data failed"), a.error_alert(s.t("connect_fail"))
-                        }
+                    var n = this;
+                    if (this.closed()) return this.sender.stop(), a.error_alert(s.t("disconnected_with_server")), Promise.reject();
+                    var i = void 0,
+                        r = void 0;
+                    return e.some((function(e) {
+                        return e.json
+                    })) ? (i = JSON.stringify(e.map((function(e) {
+                        return e.data
+                    }))), r = {
+                        contentType: "application/json; charset=utf-8"
+                    }) : (i = e[0].data, r = {
+                        cache: !1,
+                        processData: !1,
+                        contentType: "application/octet-stream"
+                    }), new Promise((function(a, o) {
+                        $.ajax(Object.assign(Object.assign({
+                            data: i
+                        }, r), {
+                            type: "POST",
+                            url: n.api_url + "&ack=" + n._executed_command_msg_id + "&seq=" + t,
+                            dataType: "json",
+                            headers: {
+                                "webio-session-id": n.webio_session_id
+                            },
+                            success: n._on_request_success.bind(n),
+                            xhr: function() {
+                                var t = new window.XMLHttpRequest;
+                                return t.upload.addEventListener("progress", (function(t) {
+                                    t.lengthComputable && e.forEach((function(e) {
+                                        e.onprogress && e.onprogress(t.loaded, t.total), e.onprogress = null
+                                    }))
+                                }), !1), t
+                            },
+                            error: function() {
+                                console.error("Http push event failed, will retry")
+                            }
+                        })).always((function() {
+                            return a()
+                        }))
                     }))
                 }
             }, {
                 key: "close_session",
                 value: function() {
-                    this._closed = !0, l(this._session_close_callbacks, "session_close_callback"), clearInterval(this.interval_pull_id)
+                    this._closed = !0, l(this._session_close_callbacks, "session_close_callback"), clearInterval(this.interval_pull_id), this.sender.stop()
                 }
             }, {
                 key: "closed",
                 value: function() {
                     return this._closed
                 }
             }, {
@@ -3707,18 +4114,18 @@
                 event: "callback",
                 task_id: t,
                 data: e
             })
         }
     }, {
         "./i18n": 11,
-        "./state": 25,
-        "./utils": 27
+        "./state": 26,
+        "./utils": 28
     }],
-    25: [function(e, t, n) {
+    26: [function(e, t, n) {
         "use strict";
         Object.defineProperty(n, "__esModule", {
             value: !0
         }), n.state = {
             AutoScrollBottom: !1,
             CurrentSession: null,
             ShowDuration: 200,
@@ -3730,15 +4137,15 @@
             codeMirrorModeURL: "https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.52.2/mode/%N/%N.min.js",
             codeMirrorThemeURL: "https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.52.2/theme/%N.min.css",
             outputAnimation: !0,
             httpPullInterval: 1e3,
             debug: !1
         }
     }, {}],
-    26: [function(e, t, n) {
+    27: [function(e, t, n) {
         "use strict";
         Object.defineProperty(n, "__esModule", {
             value: !0
         });
         var i = e("./state"),
             r = !1,
             a = $("#input-container"),
@@ -3759,66 +4166,68 @@
             if (e = i.state.FixedInputPanel && e) {
                 var t = (n = Math.max(i.state.InputPanelInitHeight, 175), r = o.height() + 80, Math.min(r, n));
                 s.height(t - 40), a.height(t), a.addClass("fixed")
             } else a.removeClass("fixed"), s.height(0), a.height("unset");
             var n, r
         }
 
-        function p(e) {
+        function d(e) {
             var t = a.height() + e;
             t >= o.height() ? t = o.height() : t <= c() - 80 && (t = c() - 80), a.height(t), s.height(t - 40)
         }
         n.show_input = function() {
             l(), r = !0, $(window).height() - a[0].getBoundingClientRect().top < c() - 40 && u(!0)
         }, n.close_input = l, $((function() {
             a = $("#input-container"), o = $("#input-cards"), s = $("#end-space");
             var e = 0;
             $(window).on("scroll", (function() {
                 var t = window.pageYOffset || document.documentElement.scrollTop,
                     n = t < e,
                     i = t > e;
                 a.hasClass("fixed") ? $(window).scrollTop() + window.innerHeight > $(document).height() - 50 && i && (u(!1), t = window.pageYOffset || document.documentElement.scrollTop) : $(window).height() - a[0].getBoundingClientRect().top < c() - 40 && n && r && (u(!0), t = window.pageYOffset || document.documentElement.scrollTop), e = t <= 0 ? 0 : t
             })), a[0].addEventListener("wheel", (function(e) {
-                a.hasClass("fixed") && (e.preventDefault(), p(parseInt(e.deltaY)))
+                a.hasClass("fixed") && (e.preventDefault(), d(parseInt(e.deltaY)))
             }));
             var t = -1;
             a[0].addEventListener("touchstart", (function(e) {
                 e.changedTouches.length > 1 || (t = e.changedTouches[0].screenY)
             })), a[0].addEventListener("touchmove", (function(e) {
                 if (a.hasClass("fixed") && !(e.changedTouches.length > 1)) {
                     e.preventDefault();
                     var n = t - e.changedTouches[0].screenY;
-                    t = e.changedTouches[0].screenY, p(n)
+                    t = e.changedTouches[0].screenY, d(n)
                 }
             }))
         }))
     }, {
-        "./state": 25
+        "./state": 26
     }],
-    27: [function(e, t, n) {
+    28: [function(e, t, n) {
         "use strict";
         var i = function() {
             function e(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     var i = t[n];
                     i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, i.key, i)
                 }
             }
             return function(t, n, i) {
                 return n && e(t.prototype, n), i && e(t, i), t
             }
         }();
+
+        function r(e, t) {
+            if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+        }
         Object.defineProperty(n, "__esModule", {
             value: !0
         });
-        var r = function() {
+        var a = function() {
             function e() {
-                ! function(e, t) {
-                    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                }(this, e), this.keys = [], this.map = {}
+                r(this, e), this.keys = [], this.map = {}
             }
             return i(e, [{
                 key: "push",
                 value: function(e, t) {
                     if (e in this.map) return console.error("LRUMap: key:%s already in map", e);
                     this.keys.push(e), this.map[e] = t
                 }
@@ -3851,28 +4260,28 @@
                 value: function(e) {
                     if (!(e in this.map)) return console.error("LRUMap: key:%s not in map when call `remove`", e);
                     delete this.map[e], this.keys.splice(this.keys.indexOf(e), 1)
                 }
             }]), e
         }();
 
-        function a(e) {
+        function o(e) {
             var t = JSON.stringify(e),
                 n = (new TextEncoder).encode(t).buffer;
-            return new Blob([o(n.byteLength), n], {
+            return new Blob([s(n.byteLength), n], {
                 type: "application/octet-stream"
             })
         }
 
-        function o(e) {
+        function s(e) {
             var t = new ArrayBuffer(8),
                 n = new DataView(t);
             return n.setUint32(0, e / 4294967296 | 0), n.setUint32(4, 0 | e), t
         }
-        n.LRUMap = r, n.b64toBlob = function(e) {
+        n.LRUMap = a, n.b64toBlob = function(e) {
             for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "application/octet-stream", n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 512, i = atob(e), r = [], a = 0; a < i.length; a += n) {
                 for (var o = i.slice(a, a + n), s = new Array(o.length), l = 0; l < o.length; l++) s[l] = o.charCodeAt(l);
                 var c = new Uint8Array(s);
                 r.push(c)
             }
             var u = new Blob(r, {
                 type: t
@@ -3939,14 +4348,95 @@
             var n = {
                 filename: e.name,
                 size: e.size,
                 mime_type: e.type,
                 last_modified: e.lastModified / 1e3,
                 input_name: t
             };
-            return new Blob([a(n), o(e.size), e], {
+            return new Blob([o(n), s(e.size), e], {
                 type: "application/octet-stream"
             })
-        }, n.serialize_json = a
+        }, n.serialize_json = o, n.is_mobile = function() {
+            if (navigator.userAgentData) return navigator.userAgentData.mobile;
+            var e = "MacIntel" === navigator.platform && navigator.maxTouchPoints > 1;
+            return /android|webos|iphone|ipad|ipod|blackberry|iemobile|opera mini/i.test(navigator.userAgent.toLowerCase()) || e
+        };
+        var l = function() {
+            function e(t) {
+                var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 8,
+                    i = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 0,
+                    a = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : 2e3,
+                    o = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : 1e3;
+                r(this, e), this.sender = t, this.window_size = n, this.min_send_interval = o, this.seq = 0, this.queue = [], this._stop = !1, this.ignore_interval_send = !1, this.last_send_time = 0, this.interval_send_id = 0, this.sender = t, this.window_size = n, this.seq = i, this.queue = [], this.ignore_interval_send = !1, this.interval_send_id = setInterval(this.interval_send.bind(this), a)
+            }
+            return i(e, [{
+                key: "add_send_task",
+                value: function(e) {
+                    var t = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1];
+                    this._stop || (this.queue.push({
+                        enable_batch: t,
+                        task: e
+                    }), this.do_send())
+                }
+            }, {
+                key: "get_tasks",
+                value: function() {
+                    var e = [],
+                        t = !0,
+                        n = !1,
+                        i = void 0;
+                    try {
+                        for (var r, a = this.queue[Symbol.iterator](); !(t = (r = a.next()).done); t = !0) {
+                            var o = r.value;
+                            if (!o.enable_batch) break;
+                            e.push(o.task)
+                        }
+                    } catch (e) {
+                        n = !0, i = e
+                    } finally {
+                        try {
+                            !t && a.return && a.return()
+                        } finally {
+                            if (n) throw i
+                        }
+                    }
+                    var s = !0;
+                    return 0 === e.length && this.queue.length > 0 && !this.queue[0].enable_batch && (s = !1, e.push(this.queue[0].task)), {
+                        tasks: e,
+                        batch_send: s
+                    }
+                }
+            }, {
+                key: "do_send",
+                value: function() {
+                    var e = this,
+                        t = this.get_tasks(),
+                        n = t.tasks,
+                        i = t.batch_send;
+                    0 !== n.length && (this.last_send_time = Date.now(), i || (this.ignore_interval_send = !0), this.sender(n, this.seq).then((function() {
+                        e.ignore_interval_send = !1
+                    })))
+                }
+            }, {
+                key: "interval_send",
+                value: function() {
+                    this._stop || this.ignore_interval_send || Date.now() - this.last_send_time < this.min_send_interval || this.do_send()
+                }
+            }, {
+                key: "ack",
+                value: function(e) {
+                    if (!(e < this.seq)) {
+                        var t = e - this.seq + 1;
+                        this.queue = this.queue.slice(t), this.seq = e + 1
+                    }
+                }
+            }, {
+                key: "stop",
+                value: function() {
+                    this._stop = !0, clearInterval(this.interval_send_id)
+                }
+            }]), e
+        }();
+        n.ReliableSender = l
     }, {}]
 }, {}, [12]);
 //# sourceMappingURL=pywebio.min.js.map
```

### Comparing `pywebio-1.7.1/pywebio/html/js/require.min.js` & `pywebio-1.8.0/pywebio/html/js/require.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/html/js/toastify.min.js` & `pywebio-1.8.0/pywebio/html/js/toastify.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/input.py` & `pywebio-1.8.0/pywebio/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,40 +72,43 @@
 Functions doc
 --------------
 """
 import copy
 import logging
 import os.path
 from collections.abc import Mapping
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from .io_ctrl import single_input, input_control, output_register_callback, send_msg, single_input_kwargs
+from .io_ctrl import input_control, output_register_callback, send_msg, single_input, single_input_kwargs
 from .platform import page as platform_setting
 from .session import get_current_session, get_current_task_id
-from .utils import Setter, parse_file_size, check_dom_name_value
+from .utils import Setter, check_dom_name_value, parse_file_size
 
 logger = logging.getLogger(__name__)
 
 TEXT = 'text'
 NUMBER = "number"
 FLOAT = "float"
 PASSWORD = "password"
 URL = "url"
 DATE = "date"
 TIME = "time"
 COLOR = "color"
 DATETIME_LOCAL = "datetime-local"
+DATETIME = DATETIME_LOCAL
 
 CHECKBOX = 'checkbox'
 RADIO = 'radio'
 SELECT = 'select'
 TEXTAREA = 'textarea'
 
-__all__ = ['TEXT', 'NUMBER', 'FLOAT', 'PASSWORD', 'URL', 'DATE', 'TIME', 'COLOR', 'DATETIME_LOCAL', 'input', 'textarea',
-           'select',
-           'checkbox', 'radio', 'actions', 'file_upload', 'slider', 'input_group', 'input_update']
+__all__ = ['TEXT', 'NUMBER', 'FLOAT', 'PASSWORD', 'URL', 'DATE',
+           'TIME', 'COLOR', 'DATETIME_LOCAL', 'DATETIME', 'input', 'textarea',
+           'select', 'checkbox', 'radio', 'actions', 'file_upload',
+           'slider', 'input_group', 'input_update']
 
 
 def _parse_args(kwargs, excludes=()):
     """parse the raw parameters that pass to input functions
 
      - excludes: the parameters that don't appear in returned spec
      - remove the parameters whose value is None
@@ -127,28 +130,33 @@
         kwargs['onchange'] = True
     else:
         onchange_func = lambda _: None
 
     return kwargs, valid_func, onchange_func
 
 
-def input(label='', type=TEXT, *, validate=None, name=None, value=None, action=None, onchange=None, placeholder=None,
-          required=None, readonly=None, datalist=None, help_text=None, **other_html_attrs):
+def input(label: str = '', type: str = TEXT, *, validate: Callable[[Any], Optional[str]] = None, name: str = None,
+          value: Union[str, int] = None,
+          action: Tuple[str, Callable[[Callable], None]] = None, onchange: Callable[[Any], None] = None,
+          placeholder: str = None, required: bool = None,
+          readonly: bool = None, datalist: List[str] = None, help_text: str = None, **other_html_attrs):
     r"""Text input
 
     :param str label: Label of input field.
-    :param str type: Input type. Currently, supported types are：`TEXT` , `NUMBER` , `FLOAT` , `PASSWORD` , `URL` , `DATE` , `TIME`, `COLOR`, `DATETIME_LOCAL`
+    :param str type: Input type. Currently, supported types are：`TEXT` , `NUMBER` , `FLOAT` , `PASSWORD` , `URL` , `DATE` , `TIME`, `DATETIME`, `COLOR`
 
-       Note that `DATE` and `TIME` type are not supported on some browsers,
-       for details see https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#Browser_compatibility
+       The value of `DATE` , `TIME`, `DATETIME` type is a string in the format of `YYYY-MM-DD` , `HH:MM:SS` , `YYYY-MM-DDTHH:MM` respectively
+       (`%Y-%m-%d`, `%H:%M:%S`, `%Y-%m-%dT%H:%M` in python `strptime() <https://docs.python.org/3/library/datetime.html#strftime-and-strptime-behavior>`_ format).
     :param callable validate: Input value validation function. If provided, the validation function will be called when
         user completes the input field or submits the form.
 
         ``validate`` receives the input value as a parameter. When the input value is valid, it returns ``None``.
-        When the input value is invalid, it returns an error message string. For example:
+        When the input value is invalid, it returns an error message string.
+
+        For example:
 
         .. exportable-codeblock::
             :name: input-valid-func
             :summary: `input()` validation
 
             def check_age(age):
                 if age>30:
@@ -256,16 +264,20 @@
             return value_setter.value
 
         return d
 
     return single_input(item_spec, valid_func, preprocess_func, onchange_func)
 
 
-def textarea(label='', *, rows=6, code=None, maxlength=None, minlength=None, validate=None, name=None, value=None,
-             onchange=None, placeholder=None, required=None, readonly=None, help_text=None, **other_html_attrs):
+def textarea(label: str = '', *, rows: int = 6, code: Union[bool, Dict] = None, maxlength: int = None,
+             minlength: int = None,
+             validate: Callable[[Any], Optional[str]] = None, name: str = None, value: str = None,
+             onchange: Callable[[Any], None] = None,
+             placeholder: str = None, required: bool = None, readonly: bool = None, help_text: str = None,
+             **other_html_attrs):
     r"""Text input area (multi-line text input)
 
     :param int rows: The number of visible text lines for the input area. Scroll bar will be used when content exceeds.
     :param int maxlength: The maximum number of characters (UTF-16 code units) that the user can enter.
         If this value isn't specified, the user can enter an unlimited number of characters.
     :param int minlength: The minimum number of characters (UTF-16 code units) required that the user should enter.
     :param dict/bool code: Enable a code style editor by providing the `Codemirror <https://codemirror.net/>`_ options:
@@ -322,16 +334,18 @@
         value = [value]
     for opt in options:
         if opt['value'] in value:
             opt['selected'] = True
     return options
 
 
-def select(label='', options=None, *, multiple=None, validate=None, name=None, value=None, onchange=None, required=None,
-           help_text=None, **other_html_attrs):
+def select(label: str = '', options: List[Union[Dict[str, Any], Tuple, List, str]] = None, *, multiple: bool = None,
+           validate: Callable[[Any], Optional[str]] = None, name: str = None, value: Union[List, str] = None,
+           onchange: Callable[[Any], None] = None, native: bool = True, required: bool = None, help_text: str = None,
+           **other_html_attrs):
     r"""Drop-down selection
 
     By default, only one option can be selected at a time, you can set ``multiple`` parameter to enable multiple selection.
 
     :param list options: list of options. The available formats of the list items are:
 
         * dict::
@@ -352,14 +366,16 @@
         2. If the ``multiple`` is not ``True``, the list of options can only have one ``selected`` item at most.
 
     :param bool multiple: whether multiple options can be selected
     :param value: The value of the initial selected item. When ``multiple=True``, ``value`` must be a list.
        You can also set the initial selected option by setting the ``selected`` field in the ``options`` list item.
     :type value: list or str
     :param bool required: Whether to select at least one item, only available when ``multiple=True``
+    :param bool native: Using browser's native select component rather than
+        `bootstrap-select <https://github.com/snapappointments/bootstrap-select>`_. This is the default behavior.
     :param - label, validate, name, onchange, help_text, other_html_attrs: Those arguments have the same meaning as for `input()`
     :return: If ``multiple=True``, return a list of the values in the ``options`` selected by the user;
         otherwise, return the single value selected by the user.
     """
     assert options is not None, 'Required `options` parameter in select()'
 
     item_spec, valid_func, onchange_func = _parse_args(locals(), excludes=['value'])
@@ -367,16 +383,18 @@
     if value is not None:
         item_spec['options'] = _set_options_selected(item_spec['options'], value)
     item_spec['type'] = SELECT
 
     return single_input(item_spec, valid_func=valid_func, preprocess_func=lambda d: d, onchange_func=onchange_func)
 
 
-def checkbox(label='', options=None, *, inline=None, validate=None, name=None, value=None, onchange=None,
-             help_text=None, **other_html_attrs):
+def checkbox(label: str = '', options: List[Union[Dict[str, Any], Tuple, List, str]] = None, *, inline: bool = None,
+             validate: Callable[[Any], Optional[str]] = None,
+             name: str = None, value: List = None, onchange: Callable[[Any], None] = None, help_text: str = None,
+             **other_html_attrs):
     r"""A group of check box that allowing single values to be selected/deselected.
 
     :param list options: List of options. The format is the same as the ``options`` parameter of the `select()` function
     :param bool inline: Whether to display the options on one line. Default is ``False``
     :param list value: The value list of the initial selected items.
        You can also set the initial selected option by setting the ``selected`` field in the ``options`` list item.
     :param - label, validate, name, onchange, help_text, other_html_attrs: Those arguments have the same meaning as for `input()`
@@ -389,16 +407,18 @@
     if value is not None:
         item_spec['options'] = _set_options_selected(item_spec['options'], value)
     item_spec['type'] = CHECKBOX
 
     return single_input(item_spec, valid_func, lambda d: d, onchange_func)
 
 
-def radio(label='', options=None, *, inline=None, validate=None, name=None, value=None, onchange=None, required=None,
-          help_text=None, **other_html_attrs):
+def radio(label: str = '', options: List[Union[Dict[str, Any], Tuple, List, str]] = None, *, inline: bool = None,
+          validate: Callable[[Any], Optional[str]] = None,
+          name: str = None, value: str = None, onchange: Callable[[Any], None] = None, required: bool = None,
+          help_text: str = None, **other_html_attrs):
     r"""A group of radio button. Only a single button can be selected.
 
     :param list options: List of options. The format is the same as the ``options`` parameter of the `select()` function
     :param bool inline: Whether to display the options on one line. Default is ``False``
     :param str value: The value of the initial selected items.
        You can also set the initial selected option by setting the ``selected`` field in the ``options`` list item.
     :param bool required: whether to must select one option. (the user can select nothing option by default)
@@ -453,15 +473,16 @@
         assert act['type'] in ('submit', 'reset', 'cancel'), \
             "submit type must be 'submit'/'reset'/'cancel', not %r" % act['type']
         act_res.append(act)
 
     return act_res
 
 
-def actions(label='', buttons=None, name=None, help_text=None):
+def actions(label: str = '', buttons: List[Union[Dict[str, Any], Tuple, List, str]] = None, name: str = None,
+            help_text: str = None):
     r"""Actions selection
 
     It is displayed as a group of buttons on the page. After the user clicks the button of it,
     it will behave differently depending on the type of the button.
 
     :param list buttons: list of buttons. The available formats of the list items are:
 
@@ -553,16 +574,17 @@
     item_spec, valid_func, onchange_func = _parse_args(locals())
     item_spec['type'] = 'actions'
     item_spec['buttons'] = _parse_action_buttons(buttons)
 
     return single_input(item_spec, valid_func, lambda d: d, onchange_func)
 
 
-def file_upload(label='', accept=None, name=None, placeholder='Choose file', multiple=False, max_size=0,
-                max_total_size=0, required=None, help_text=None, **other_html_attrs):
+def file_upload(label: str = '', accept: Union[List, str] = None, name: str = None, placeholder: str = 'Choose file',
+                multiple: bool = False, max_size: Union[int, str] = 0, max_total_size: Union[int, str] = 0,
+                required: bool = None, help_text: str = None, **other_html_attrs):
     r"""File uploading
 
     :param accept: Single value or list, indicating acceptable file types. The available formats of file types are:
 
         * A valid case-insensitive filename extension, starting with a period (".") character. For example: ``.jpg``, ``.pdf``, or ``.doc``.
         * A valid MIME type string, with no extensions.
           For examples: ``application/pdf``, ``audio/*``, ``video/*``, ``image/*``.
@@ -586,22 +608,22 @@
 
         {
             'filename': file name，
             'content'：content of the file (in bytes),
             'mime_type': MIME type of the file,
             'last_modified': Last modified time (timestamp) of the file
         }
-       
+
        If there is no file uploaded, return ``None``.
 
        When ``multiple=True``, a list is returned. The format of the list item is the same as the return value when ``multiple=False`` above.
        If the user does not upload a file, an empty list is returned.
 
     .. note::
-    
+
         If uploading large files, please pay attention to the file upload size limit setting of the web framework.
         When using :func:`start_server() <pywebio.platform.tornado.start_server>` or
         :func:`path_deploy() <pywebio.platform.path_deploy>` to start the PyWebIO application,
         the maximum file size to be uploaded allowed by the web framework can be set through the ``max_payload_size`` parameter.
 
     .. exportable-codeblock::
         :name: file_upload_example
@@ -623,28 +645,20 @@
 
     if platform_setting.MAX_PAYLOAD_SIZE:
         if item_spec['max_size'] > platform_setting.MAX_PAYLOAD_SIZE or \
                 item_spec['max_total_size'] > platform_setting.MAX_PAYLOAD_SIZE:
             raise ValueError('The `max_size` and `max_total_size` value can not exceed the backend payload size limit. '
                              'Please increase the `max_total_size` of `start_server()`/`path_deploy()`')
 
-    def read_file(data):
-        for file in data:
-            # Security fix: to avoid interpreting file name as path
-            file['filename'] = os.path.basename(file['filename'])
-
-        if not multiple:
-            return data[0] if len(data) >= 1 else None
-        return data
-
-    return single_input(item_spec, valid_func, read_file, onchange_func)
+    return single_input(item_spec, valid_func, lambda d: d, onchange_func)
 
 
-def slider(label='', *, name=None, value=0, min_value=0, max_value=100, step=1, validate=None, onchange=None,
-           required=None, help_text=None, **other_html_attrs):
+def slider(label: str = '', *, name: str = None, value: Union[int, float] = 0, min_value: Union[int, float] = 0,
+           max_value: Union[int, float] = 100, step: int = 1, validate: Callable[[Any], Optional[str]] = None,
+           onchange: Callable[[Any], None] = None, required: bool = None, help_text: str = None, **other_html_attrs):
     r"""Range input.
 
     :param int/float value: The initial value of the slider.
     :param int/float min_value: The minimum permitted value.
     :param int/float max_value: The maximum permitted value.
     :param int step: The stepping interval.
        Only available when ``value``, ``min_value`` and ``max_value`` are all integer.
@@ -657,15 +671,16 @@
     item_spec['float'] = any(isinstance(i, float) for i in (value, min_value, max_value))
     if item_spec['float']:
         item_spec['step'] = 'any'
 
     return single_input(item_spec, valid_func, lambda d: d, onchange_func)
 
 
-def input_group(label='', inputs=None, validate=None, cancelable=False):
+def input_group(label: str = '', inputs: List = None, validate: Callable[[Dict], Optional[Tuple[str, str]]] = None,
+                cancelable: bool = False):
     r"""Input group. Request a set of inputs from the user at once.
 
     :param str label: Label of input group.
     :param list inputs: Input items.
        The item of the list is the call to the single input function, and the ``name`` parameter need to be passed in the single input function.
     :param callable validate: validation function for the group. If provided, the validation function will be called when the user submits the form.
 
@@ -743,15 +758,15 @@
 
     attributes = dict((k, v) for k, v in spec.items() if v is not None)
     if 'options' in spec:
         attributes['options'] = _parse_select_options(spec['options'])
     return attributes
 
 
-def input_update(name=None, **spec):
+def input_update(name: str = None, **spec):
     """Update attributes of input field.
     This function can only be called in ``onchange`` callback of input functions.
 
     :param str name: The ``name`` of the target input item.
        Optional, default is the name of input field which triggers ``onchange``
     :param spec: The input parameters need to be updated.
        Note that those parameters can not be updated:
```

### Comparing `pywebio-1.7.1/pywebio/io_ctrl.py` & `pywebio-1.8.0/pywebio/io_ctrl.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,56 +72,50 @@
             type(self).safely_destruct(spec)
             raise
 
         # For Context manager
         self.enabled_context_manager = False
         self.container_selector = None
         self.container_dom_id = None  # todo: this name is ambiguous, rename it to `scope_name` or others
-        self.custom_enter = None
-        self.custom_exit = None
+        self.after_exit = None
 
         # Try to make sure current session exist.
         # If we leave the session interaction in `Output.__del__`,
         # the Exception raised from there will be ignored by python interpreter,
         # thus we can't end some session in some cases.
         # See also: https://github.com/pywebio/PyWebIO/issues/243
         get_current_session()
 
-    def enable_context_manager(self, container_selector=None, container_dom_id=None, custom_enter=None,
-                               custom_exit=None):
+    def enable_context_manager(self, container_selector=None, container_dom_id=None, after_exit=None):
         self.enabled_context_manager = True
         self.container_selector = container_selector
         self.container_dom_id = container_dom_id
-        self.custom_enter = custom_enter
-        self.custom_exit = custom_exit
+        self.after_exit = after_exit
         return self
 
     def __enter__(self):
         if not self.enabled_context_manager:
             raise RuntimeError("This output function can't be used as context manager!")
-        if self.custom_enter:
-            return self.custom_enter(self)
 
         self.container_dom_id = self.container_dom_id or random_str(10)
         self.spec['container_selector'] = self.container_selector
         self.spec['container_dom_id'] = scope2dom(self.container_dom_id, no_css_selector=True)
         self.send()
         get_current_session().push_scope(self.container_dom_id)
         return self.container_dom_id
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
         If this method returns True,
         it means that the context manager can handle the exception,
         so that the with statement terminates the propagation of the exception
         """
-        if self.custom_exit:
-            return self.custom_exit(self, exc_type=exc_type, exc_val=exc_val, exc_tb=exc_tb)
-
         get_current_session().pop_scope()
+        if self.after_exit:
+            self.after_exit()
         return False  # Propagate Exception
 
     def embed_data(self):
         """返回供嵌入到其他消息中的数据，可以设置一些默认值"""
         self.processed = True
         return self.on_embed(self.spec)
 
@@ -282,30 +276,30 @@
 
     data = yield input_event_handle(item_valid_funcs, form_valid_funcs, preprocess_funcs, onchange_funcs)
 
     send_msg('destroy_form')
     return data
 
 
-def check_item(name, data, valid_func, preprocess_func):
+def check_item(name, data, valid_func, preprocess_func, clear_invalid=False):
     try:
         data = preprocess_func(data)
         error_msg = valid_func(data)
     except Exception as e:
         logger.warning('Get %r in valid_func for name:"%s"', e, name)
         from pywebio.session import info as session_info
         error_msg = '字段内容不合法' if 'zh' in session_info.user_language else 'Your input is not valid'
 
     if error_msg is not None:
         send_msg('update_input', dict(target_name=name, attributes={
             'valid_status': False,
             'invalid_feedback': error_msg
         }))
         return False
-    else:
+    elif clear_invalid:
         send_msg('update_input', dict(target_name=name, attributes={
             'valid_status': 0,  # valid_status为0表示清空valid_status标志
         }))
     return True
 
 
 def trigger_onchange(event_data, onchange_funcs):
@@ -336,23 +330,24 @@
     :param item_valid_funcs: map(name -> valid_func)  valid_func 为 None 时，不进行验证
                         valid_func: callback(data) -> error_msg or None
     :param form_valid_funcs: callback(data) -> (name, error_msg) or None
     :param preprocess_funcs: map(name -> process_func)
     :param onchange_funcs: map(name -> onchange_func)
     :return:
     """
+    data = None
     while True:
         event = yield next_client_event()
         event_name, event_data = event['event'], event['data']
         if event_name == 'input_event':
             input_event = event_data['event_name']
             if input_event == 'blur':
                 onblur_name = event_data['name']
                 check_item(onblur_name, event_data['value'], item_valid_funcs[onblur_name],
-                           preprocess_funcs[onblur_name])
+                           preprocess_funcs[onblur_name], clear_invalid=True)
             elif input_event == 'change':
                 trigger_onchange(event_data, onchange_funcs)
 
         elif event_name == 'from_submit':
             all_valid = True
 
             # 调用输入项验证函数进行校验
@@ -377,18 +372,17 @@
 
                         send_msg('update_input', dict(target_name=onblur_name, attributes={
                             'valid_status': False,
                             'invalid_feedback': error_msg
                         }))
 
             if all_valid:
-                break
+                break  # form event loop
         elif event_name == 'from_cancel':
-            data = None
-            break
+            break  # break event loop
         else:
             logger.warning("Unhandled Event: %s", event)
 
     return data
 
 
 def output_register_callback(callback, **options):
```

### Comparing `pywebio-1.7.1/pywebio/output.py` & `pywebio-1.8.0/pywebio/output.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,22 +38,27 @@
 |                    | | `put_warning`:sup:`*†`  |                                                            |
 |                    | | `put_error`:sup:`*†`    |                                                            |
 |                    +---------------------------+------------------------------------------------------------+
 |                    | `put_html`                | Output html                                                |
 |                    +---------------------------+------------------------------------------------------------+
 |                    | `put_link`                | Output link                                                |
 |                    +---------------------------+------------------------------------------------------------+
-|                    | `put_processbar`          | Output a process bar                                       |
+|                    | `put_progressbar`         | Output a progress bar                                      |
 |                    +---------------------------+------------------------------------------------------------+
 |                    | `put_loading`:sup:`†`     | Output loading prompt                                      |
 |                    +---------------------------+------------------------------------------------------------+
 |                    | `put_code`                | Output code block                                          |
 |                    +---------------------------+------------------------------------------------------------+
 |                    | `put_table`:sup:`*`       | Output table                                               |
 |                    +---------------------------+------------------------------------------------------------+
+|                    | | `put_datatable`         | Output and update data table                               |
+|                    | | `datatable_update`      |                                                            |
+|                    | | `datatable_insert`      |                                                            |
+|                    | | `datatable_remove`      |                                                            |
+|                    +---------------------------+------------------------------------------------------------+
 |                    | | `put_button`            | Output button and bind click event                         |
 |                    | | `put_buttons`           |                                                            |
 |                    +---------------------------+------------------------------------------------------------+
 |                    | `put_image`               | Output image                                               |
 |                    +---------------------------+------------------------------------------------------------+
 |                    | `put_file`                | Output a link to download a file                           |
 |                    +---------------------------+------------------------------------------------------------+
@@ -169,27 +174,31 @@
     :param bool closable: Whether to show a dismiss button on the right of the message.
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
 
     .. versionadded:: 1.2
 
 .. autofunction:: put_html
 .. autofunction:: put_link
-.. autofunction:: put_processbar
-.. autofunction:: set_processbar
+.. autofunction:: put_progressbar
+.. autofunction:: set_progressbar
 .. autofunction:: put_loading
 .. autofunction:: put_code
 .. autofunction:: put_table
 .. autofunction:: span
 .. autofunction:: put_buttons
 .. autofunction:: put_button
 .. autofunction:: put_image
 .. autofunction:: put_file
 .. autofunction:: put_tabs
 .. autofunction:: put_collapse
 .. autofunction:: put_scrollable
+.. autofunction:: put_datatable
+.. autofunction:: datatable_update
+.. autofunction:: datatable_insert
+.. autofunction:: datatable_remove
 .. autofunction:: put_widget
 
 Other Interactions
 --------------------
 .. autofunction:: toast
 .. autofunction:: popup
 .. autofunction:: close_popup
@@ -204,38 +213,48 @@
 .. autofunction:: style
 
 
 """
 import copy
 import html
 import io
+import json
 import logging
 import string
 from base64 import b64encode
 from collections.abc import Mapping, Sequence
 from functools import wraps
-from typing import Union
+from typing import (
+    Any, Callable, Dict, List, Tuple, Union, Sequence as SequenceType, Mapping as MappingType
+)
+
+try:
+    from typing import Literal  # added in Python 3.8
+except ImportError:
+    pass
 
-from .io_ctrl import output_register_callback, send_msg, Output, safely_destruct_output_when_exp, OutputList, scope2dom
+from .io_ctrl import output_register_callback, send_msg, Output, \
+    safely_destruct_output_when_exp, OutputList, scope2dom
 from .session import get_current_session, download
 from .utils import random_str, iscoroutinefunction, check_dom_name_value
 
 try:
     from PIL.Image import Image as PILImage
 except ImportError:
     PILImage = type('MockPILImage', (), dict(__init__=None))
 
 logger = logging.getLogger(__name__)
 
-__all__ = ['Position', 'remove', 'scroll_to', 'put_tabs', 'put_scope',
+__all__ = ['Position', 'OutputPosition', 'remove', 'scroll_to', 'put_tabs', 'put_scope',
            'put_text', 'put_html', 'put_code', 'put_markdown', 'use_scope', 'set_scope', 'clear', 'remove',
            'put_table', 'put_buttons', 'put_image', 'put_file', 'PopupSize', 'popup', 'put_button',
            'close_popup', 'put_widget', 'put_collapse', 'put_link', 'put_scrollable', 'style', 'put_column',
-           'put_row', 'put_grid', 'span', 'put_processbar', 'set_processbar', 'put_loading',
-           'output', 'toast', 'get_scope', 'put_info', 'put_error', 'put_warning', 'put_success']
+           'put_row', 'put_grid', 'span', 'put_progressbar', 'set_progressbar', 'put_processbar', 'set_processbar',
+           'put_loading', 'output', 'toast', 'get_scope', 'put_info', 'put_error', 'put_warning', 'put_success',
+           'put_datatable', 'datatable_update', 'datatable_insert', 'datatable_remove', 'JSFunction']
 
 
 # popup size
 class PopupSize:
     LARGE = 'large'
     NORMAL = 'normal'
     SMALL = 'small'
@@ -252,19 +271,19 @@
     TOP = 0
     BOTTOM = -1
 
 
 _scope_name_allowed_chars = set(string.ascii_letters + string.digits + '_-')
 
 
-def set_scope(name, container_scope=None, position=OutputPosition.BOTTOM, if_exist=None):
+def set_scope(name: str, container_scope: str = None, position: int = OutputPosition.BOTTOM, if_exist: str = None):
     """Create a new scope.
 
     :param str name: scope name
-    :param str container_scope: Specify the parent scope of this scope. 
+    :param str container_scope: Specify the parent scope of this scope.
         When the scope doesn't exist, no operation is performed.
     :param int position: The location where this scope is created in the parent scope.
        (see :ref:`Scope related parameters <scope_param>`)
     :param str if_exist: What to do when the specified scope already exists:
 
         - `None`: Do nothing
         - `'remove'`: Remove the old scope first and then create a new one
@@ -276,15 +295,15 @@
         container_scope = get_scope()
     check_dom_name_value(name, 'scope name')
     send_msg('output_ctl', dict(set_scope=scope2dom(name, no_css_selector=True),
                                 container=scope2dom(container_scope),
                                 position=position, if_exist=if_exist))
 
 
-def get_scope(stack_idx=-1):
+def get_scope(stack_idx: int = -1):
     """Get the scope name of runtime scope stack
 
     :param int stack_idx: The index of the runtime scope stack. Default is -1.
 
        0 means the top level scope(the ``ROOT`` Scope),
        -1 means the current Scope,
        -2 means the scope used before entering the current scope, ...
@@ -293,36 +312,36 @@
     try:
         return get_current_session().get_scope_name(stack_idx)
     except IndexError:
         logger.exception("Scope stack index error")
         return None
 
 
-def clear(scope=None):
+def clear(scope: str = None):
     """Clear the content of the specified scope
 
     :param str scope: Target scope name. Default is the current scope.
     """
     if scope is None:
         scope = get_scope()
     send_msg('output_ctl', dict(clear=scope2dom(scope)))
 
 
-def remove(scope=None):
+def remove(scope: str = None):
     """Remove the specified scope
 
     :param str scope: Target scope name. Default is the current scope.
     """
     if scope is None:
         scope = get_scope()
     assert scope != 'ROOT', "Can not remove `ROOT` scope."
     send_msg('output_ctl', dict(remove=scope2dom(scope)))
 
 
-def scroll_to(scope=None, position=Position.TOP):
+def scroll_to(scope: str = None, position: str = Position.TOP):
     """
     Scroll the page to the specified scope
 
     :param str scope: Target scope. Default is the current scope.
     :param str position: Where to place the scope in the visible area of the page. Available value:
 
        * ``'top'`` : Keep the scope at the top of the visible area of the page
@@ -357,15 +376,16 @@
 
     spec['scope'] = scope2dom(scope_name)
     spec['position'] = position
 
     return spec
 
 
-def put_text(*texts, sep=' ', inline=False, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_text(*texts: Any, sep: str = ' ', inline: bool = False, scope: str = None,
+             position: int = OutputPosition.BOTTOM) -> Output:
     """
     Output plain text
 
     :param texts: Texts need to output. The type can be any object, and the `str()` function will be used for non-string objects.
     :param str sep: The separator between the texts
     :param bool inline: Use text as an inline element (no line break at the end of the text). Default is ``False``
     :param str scope: The target scope to output. If the scope does not exist, no operation will be performed.
@@ -393,50 +413,57 @@
 {{/dismissible}}
 </div>""".strip()
     contents = [c if isinstance(c, Output) else put_text(c) for c in contents]
     return put_widget(template=tpl, data=dict(color=color, contents=contents, dismissible=closable),
                       scope=scope, position=position).enable_context_manager()
 
 
-def put_info(*contents, closable=False, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_info(*contents: Any, closable: bool = False, scope: str = None,
+             position: int = OutputPosition.BOTTOM) -> Output:
     """Output information message.
 
     :param contents: Message contents.
        The item is ``put_xxx()`` call, and any other type will be converted to ``put_text(content)``.
     :param bool closable: Whether to show a dismiss button on the right of the message.
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
 
     .. versionadded:: 1.2
     """
     return _put_message(color='info', contents=contents, closable=closable, scope=scope, position=position)
 
 
-def put_success(*contents, closable=False, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_success(*contents: Any, closable: bool = False, scope: str = None,
+                position: int = OutputPosition.BOTTOM) -> Output:
     """Output success message.
     .. seealso:: `put_info()`
     .. versionadded:: 1.2
     """
     return _put_message(color='success', contents=contents, closable=closable, scope=scope, position=position)
 
 
-def put_warning(*contents, closable=False, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_warning(*contents: Any, closable: bool = False, scope: str = None,
+                position: int = OutputPosition.BOTTOM) -> Output:
     """Output warning message.
     .. seealso:: `put_info()`
     """
     return _put_message(color='warning', contents=contents, closable=closable, scope=scope, position=position)
 
 
-def put_error(*contents, closable=False, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_error(*contents: Any, closable: bool = False, scope: str = None,
+              position: int = OutputPosition.BOTTOM) -> Output:
     """Output error message.
     .. seealso:: `put_info()`
     """
     return _put_message(color='danger', contents=contents, closable=closable, scope=scope, position=position)
 
 
-def put_html(html, sanitize=False, scope=None, position=OutputPosition.BOTTOM) -> Output:
+# Due to the IPython rich output compatibility,
+# declare argument `html` to type `str` will cause type check error
+# so leave this argument's type `Any`
+def put_html(html: Any, sanitize: bool = False, scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """
     Output HTML content
 
     :param html: html string
     :param bool sanitize: Whether to use `DOMPurify <https://github.com/cure53/DOMPurify>`_ to filter the content to prevent XSS attacks.
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
     """
@@ -448,15 +475,16 @@
     elif hasattr(html, '_repr_html_'):
         html = html._repr_html_()
 
     spec = _get_output_spec('html', content=html, sanitize=sanitize, scope=scope, position=position)
     return Output(spec)
 
 
-def put_code(content, language='', rows=None, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_code(content: str, language: str = '', rows: int = None, scope: str = None,
+             position: int = OutputPosition.BOTTOM) -> Output:
     """
     Output code block
 
     :param str content: code string
     :param str language: language of code
     :param int rows: The max lines of code can be displayed, no limit by default. The scroll bar will be displayed when the content exceeds.
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
@@ -500,16 +528,17 @@
         while line.strip() and line[:strip_cnt] not in (' ' * strip_cnt, '\t' * strip_cnt):
             strip_cnt -= 1
 
     lines_ = [i[strip_cnt:] for i in lines[1:]]
     return '\n'.join(lines[:1] + lines_)
 
 
-def put_markdown(mdcontent, lstrip=True, options=None, sanitize=True,
-                 scope=None, position=OutputPosition.BOTTOM, **kwargs) -> Output:
+def put_markdown(mdcontent: str, lstrip: bool = True, options: Dict[str, Union[str, bool]] = None,
+                 sanitize: bool = True,
+                 scope: str = None, position: int = OutputPosition.BOTTOM, **kwargs) -> Output:
     """
     Output Markdown
 
     :param str mdcontent: Markdown string
     :param bool lstrip: Whether to remove the leading whitespace in each line of ``mdcontent``.
         The number of the whitespace to remove will be decided cleverly.
     :param dict options: Configuration when parsing Markdown.
@@ -530,14 +559,15 @@
 
     .. versionchanged:: 1.5
        Enable `lstrip` by default.
        Deprecate `strip_indent`.
     """
     if 'strip_indent' in kwargs:
         import warnings
+
         # use stacklevel=2 to make the warning refer to put_markdown() call
         warnings.warn("`strip_indent` parameter is deprecated in `put_markdown()`", DeprecationWarning, stacklevel=2)
 
     if lstrip:
         mdcontent = _left_strip_multiple_line_string_literal(mdcontent)
 
     spec = _get_output_spec('markdown', content=mdcontent, options=options, sanitize=sanitize,
@@ -547,15 +577,15 @@
 
 class span_:
     def __init__(self, content, row=1, col=1):
         self.content, self.row, self.col = content, row, col
 
 
 @safely_destruct_output_when_exp('content')
-def span(content, row=1, col=1):
+def span(content: Union[str, Output], row: int = 1, col: int = 1):
     """Create cross-cell content in :func:`put_table()` and :func:`put_grid()`
 
     :param content: cell content. It can be a string or ``put_xxx()`` call.
     :param int row: Vertical span, that is, the number of spanning rows
     :param int col: Horizontal span, that is, the number of spanning columns
 
     :Example:
@@ -575,26 +605,27 @@
         ])
 
     """
     return span_(content, row, col)
 
 
 @safely_destruct_output_when_exp('tdata')
-def put_table(tdata, header=None, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_table(tdata: List[Union[List, Dict]], header: List[Union[str, Tuple[Any, str]]] = None, scope: str = None,
+              position: int = OutputPosition.BOTTOM) -> Output:
     """
     Output table
 
     :param list tdata: Table data, which can be a two-dimensional list or a list of dict.
        The table cell can be a string or ``put_xxx()`` call. The cell can use the :func:`span()` to set the cell span.
     :param list header: Table header.
        When the item of ``tdata`` is of type ``list``, if the ``header`` parameter is omitted,
        the first item of ``tdata`` will be used as the header.
        The header item can also use the :func:`span()` function to set the cell span.
 
-       When ``tdata`` is list of dict, ``header`` is used to specify the order of table headers, which cannot be omitted.
+       When ``tdata`` is list of dict, ``header`` can be used to specify the order of table headers.
        In this case, the ``header`` can be a list of dict key or a list of ``(<label>, <dict key>)``.
 
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
 
     Example:
 
     .. exportable-codeblock::
@@ -636,35 +667,35 @@
             {"Course":"DB", "Score": "93"},
         ], header=["Course", "Score"])  # or header=[(put_markdown("*Course*"), "Course"), (put_markdown("*Score*") ,"Score")]
 
     .. versionadded:: 0.3
        The cell of table support ``put_xxx()`` calls.
     """
 
-    # Change ``dict`` row table to list row table
-    if tdata and isinstance(tdata[0], dict):
-        if isinstance(header[0], (list, tuple)):
+    if tdata and isinstance(tdata[0], dict):  # Change ``dict`` row table to list row table
+        if header is None:
+            order = list(tdata[0].keys())
+            header_ = [str(h).capitalize() for h in tdata[0].keys()]
+        elif isinstance(header[0], (list, tuple)):
             header_ = [h[0] for h in header]
             order = [h[-1] for h in header]
         else:
             header_ = order = header
 
         tdata = [
             [row.get(k, '') for k in order]
             for row in tdata
         ]
         header = header_
+    elif not tdata and isinstance(header[0], (list, tuple)):
+        header = [h[0] for h in header]
     else:
         tdata = [list(i) for i in tdata]  # copy data
 
     if header:
-        # when tdata is empty, header will not be process
-        # see https://github.com/pywebio/PyWebIO/issues/453
-        if isinstance(header[0], (list, tuple)):
-            header = [h[0] for h in header]
         tdata = [header, *tdata]
 
     span = {}
     for x in range(len(tdata)):
         for y in range(len(tdata[x])):
             cell = tdata[x][y]
             if isinstance(cell, span_):
@@ -701,16 +732,19 @@
             btn = dict(value=btn, label=btn)
         values.append(btn['value'])
         btn['value'] = idx
         btns.append(btn)
     return btns, values
 
 
-def put_buttons(buttons, onclick, small=None, link_style=False, outline=False, group=False, scope=None,
-                position=OutputPosition.BOTTOM, **callback_options) -> Output:
+def put_buttons(buttons: List[Union[Dict[str, Any], Tuple[str, Any], List, str]],
+                onclick: Union[Callable[[Any], None], SequenceType[Callable[[], None]]],
+                small: bool = None, link_style: bool = False, outline: bool = False, group: bool = False,
+                scope: str = None,
+                position: int = OutputPosition.BOTTOM, **callback_options) -> Output:
     """
     Output a group of buttons and bind click event
 
     :param list buttons: Button list. The available formats of list items are:
 
         * dict::
 
@@ -811,16 +845,17 @@
     callback_id = output_register_callback(click_callback, **callback_options)
     spec = _get_output_spec('buttons', callback_id=callback_id, buttons=btns, small=small,
                             scope=scope, position=position, link=link_style, outline=outline, group=group)
 
     return Output(spec)
 
 
-def put_button(label, onclick, color=None, small=None, link_style=False, outline=False, disabled=False, scope=None,
-               position=OutputPosition.BOTTOM) -> Output:
+def put_button(label: str, onclick: Callable[[], None], color: str = None, small: bool = None, link_style: bool = False,
+               outline: bool = False, disabled: bool = False, scope: str = None,
+               position: int = OutputPosition.BOTTOM) -> Output:
     """Output a single button and bind click event to it.
 
     :param str label: Button label
     :param callable onclick: Callback which will be called when button is clicked.
     :param str color: The color of the button,
         can be one of: `primary`, `secondary`, `success`, `danger`, `warning`, `info`, `light`, `dark`.
     :param bool disabled: Whether the button is disabled
@@ -840,16 +875,17 @@
        add ``disabled`` parameter
     """
     return put_buttons([{'label': label, 'value': '', 'color': color or 'primary', 'disabled': disabled}],
                        onclick=[onclick], small=small, link_style=link_style, outline=outline, scope=scope,
                        position=position)
 
 
-def put_image(src, format=None, title='', width=None, height=None,
-              scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_image(src: Union[str, bytes, PILImage], format: str = None, title: str = '', width: str = None,
+              height: str = None,
+              scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """Output image
 
     :param src: Source of image. It can be a string specifying image URL, a bytes-like object specifying
         the binary content of an image or an instance of ``PIL.Image.Image``
     :param str title: Image description.
     :param str width: The width of image. It can be CSS pixels (like `'30px'`) or percentage (like `'10%'`).
     :param str height: The height of image. It can be CSS pixels (like `'30px'`) or percentage (like `'10%'`).
@@ -887,15 +923,16 @@
     height = 'height="%s"' % html.escape(height, quote=True) if height is not None else ''
 
     tag = r'<img src="{src}" alt="{title}" {width} {height}/>'.format(src=src, title=html.escape(title, quote=True),
                                                                       height=height, width=width)
     return put_html(tag, scope=scope, position=position)
 
 
-def put_file(name, content, label=None, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_file(name: str, content: bytes, label: str = None, scope: str = None,
+             position: int = OutputPosition.BOTTOM) -> Output:
     """Output a link to download a file
 
     To show a link with the file name on the browser. When click the link, the browser automatically downloads the file.
 
     :param str name: File name downloaded as
     :param content: File content. It is a bytes-like object
     :param str label: The label of the download link, which is the same as the file name by default.
@@ -915,16 +952,16 @@
         label = name
     output = put_buttons(buttons=[label], link_style=True,
                          onclick=[lambda: download(name, content)],
                          scope=scope, position=position)
     return output
 
 
-def put_link(name, url=None, app=None, new_window=False, scope=None,
-             position=OutputPosition.BOTTOM) -> Output:
+def put_link(name: str, url: str = None, app: str = None, new_window: bool = False, scope: str = None,
+             position: int = OutputPosition.BOTTOM) -> Output:
     """Output hyperlinks to other web page or PyWebIO Application page.
 
     :param str name: The label of the link
     :param str url: Target url
     :param str app: Target PyWebIO Application name. See also: :ref:`Server mode <server_and_script_mode>`
     :param bool new_window: Whether to open the link in a new window
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
@@ -936,83 +973,88 @@
     href = 'javascript:WebIO.openApp(%r, %d)' % (app, new_window) if app is not None else url
     target = '_blank' if (new_window and url) else '_self'
     tag = '<a href="{href}" target="{target}">{name}</a>'.format(
         href=html.escape(href, quote=True), target=target, name=html.escape(name))
     return put_html(tag, scope=scope, position=position)
 
 
-def put_processbar(name, init=0, label=None, auto_close=False, scope=None,
-                   position=OutputPosition.BOTTOM) -> Output:
-    """Output a process bar
+def put_progressbar(name: str, init: float = 0, label: str = None, auto_close: bool = False, scope: str = None,
+                    position: int = OutputPosition.BOTTOM) -> Output:
+    """Output a progress bar
 
     :param str name: The name of the progress bar, which is the unique identifier of the progress bar
     :param float init: The initial progress value of the progress bar. The value is between 0 and 1
-    :param str label: The label of process bar. The default is the percentage value of the current progress.
+    :param str label: The label of progress bar. The default is the percentage value of the current progress.
     :param bool auto_close: Whether to remove the progress bar after the progress is completed
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
 
     Example:
 
     .. exportable-codeblock::
-        :name: put_processbar
-        :summary: `put_processbar()` usage
+        :name: put_progressbar
+        :summary: `put_progressbar()` usage
 
         import time
 
-        put_processbar('bar');
+        put_progressbar('bar');
         for i in range(1, 11):
-            set_processbar('bar', i / 10)
+            set_progressbar('bar', i / 10)
             time.sleep(0.1)
 
-    .. seealso:: use `set_processbar()` to set the progress of progress bar
+    .. seealso:: use `set_progressbar()` to set the progress of progress bar
     """
     check_dom_name_value(name)
-    processbar_id = 'webio-processbar-%s' % name
+    progressbar_id = 'webio-progressbar-%s' % name
     percentage = init * 100
     label = '%.1f%%' % percentage if label is None else label
     tpl = """<div class="progress" style="margin-top: 4px;">
                 <div id="{{elem_id}}" class="progress-bar bg-info progress-bar-striped progress-bar-animated" role="progressbar"
                      style="width: {{percentage}}%;" aria-valuenow="{{init}}" aria-valuemin="0" aria-valuemax="1" data-auto-close="{{auto_close}}">{{label}}
                 </div>
             </div>"""
-    return put_widget(tpl, data=dict(elem_id=processbar_id, init=init, label=label,
+    return put_widget(tpl, data=dict(elem_id=progressbar_id, init=init, label=label,
                                      percentage=percentage, auto_close=int(bool(auto_close))), scope=scope,
                       position=position)
 
 
-def set_processbar(name, value, label=None):
+def set_progressbar(name: str, value: float, label: str = None):
     """Set the progress of progress bar
 
     :param str name: The name of the progress bar
     :param float value: The progress value of the progress bar. The value is between 0 and 1
-    :param str label: The label of process bar. The default is the percentage value of the current progress.
+    :param str label: The label of progress bar. The default is the percentage value of the current progress.
 
-    See also: `put_processbar()`
+    See also: `put_progressbar()`
     """
     from pywebio.session import run_js
 
     check_dom_name_value(name)
 
-    processbar_id = 'webio-processbar-%s' % name
+    progressbar_id = 'webio-progressbar-%s' % name
     percentage = value * 100
     label = '%.1f%%' % percentage if label is None else label
 
     js_code = """
-    let bar = $("#{processbar_id}");
+    let bar = $("#{progressbar_id}");
     bar[0].style.width = "{percentage}%";
     bar.attr("aria-valuenow", "{value}");
     bar.text({label!r});
-    """.format(processbar_id=processbar_id, percentage=percentage, value=value, label=label)
+    """.format(progressbar_id=progressbar_id, percentage=percentage, value=value, label=label)
     if value == 1:
         js_code += "if(bar.data('autoClose')=='1')bar.parent().remove();"
 
     run_js(js_code)
 
 
-def put_loading(shape='border', color='dark', scope=None, position=OutputPosition.BOTTOM) -> Output:
+put_processbar = put_progressbar
+set_processbar = set_progressbar
+
+
+def put_loading(shape: str = 'border', color: str = 'dark', scope: str = None,
+                position: int = OutputPosition.BOTTOM) -> Output:
     """Output loading prompt
 
     :param str shape: The shape of loading prompt. The available values are: `'border'` (default)、 `'grow'`
     :param str color: The color of loading prompt. The available values are: `'primary'` 、 `'secondary'` 、
         `'success'` 、 `'danger'` 、 `'warning'` 、`'info'`  、`'light'`  、 `'dark'` (default)
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
 
@@ -1025,47 +1067,49 @@
         for shape in ('border', 'grow'):
             for color in ('primary', 'secondary', 'success', 'danger', 'warning', 'info', 'light', 'dark'):
                 put_text(shape, color)
                 put_loading(shape=shape, color=color)
 
         ## ----
         import time  # ..demo-only
-        # Use as context manager, the loading prompt will disappear automatically when the context block exits.
+        # The loading prompt and the output inside the context will disappear
+        # automatically when the context block exits.
         with put_loading():
+            put_text("Start waiting...")
             time.sleep(3)  # Some time-consuming operations
-            put_text("The answer of the universe is 42")
+        put_text("The answer of the universe is 42")
 
         ## ----
         # using style() to set the size of the loading prompt
         put_loading().style('width:4rem; height:4rem')
+
+    .. versionchanged:: 1.8
+       when use `put_loading()` as context manager, the output inside the context will also been removed
+       after the context block exits.
     """
     assert shape in ('border', 'grow'), "shape must in ('border', 'grow')"
     assert color in {'primary', 'secondary', 'success', 'danger', 'warning', 'info', 'light', 'dark'}
 
-    html = """<div class="spinner-{shape} text-{color}" role="status">
+    html = """<div><div class="spinner-{shape} text-{color}" role="status">
                 <span class="sr-only">Loading...</span>
-            </div>""".format(shape=shape, color=color)
+            </div></div>""".format(shape=shape, color=color)
 
     scope_name = random_str(10)
 
-    def enter(self):
-        self.spec['container_dom_id'] = scope2dom(scope_name, no_css_selector=True)
-        self.send()
-        return scope_name
-
-    def exit_(self, exc_type, exc_val, exc_tb):
+    def after_exit():
         remove(scope_name)
         return False  # Propagate Exception
 
     return put_html(html, sanitize=False, scope=scope, position=position). \
-        enable_context_manager(custom_enter=enter, custom_exit=exit_)
+        enable_context_manager(container_dom_id=scope_name, after_exit=after_exit)
 
 
 @safely_destruct_output_when_exp('content')
-def put_collapse(title, content=[], open=False, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_collapse(title: str, content: Union[str, Output, List[Union[str, Output]]] = [], open: bool = False,
+                 scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """Output collapsible content
 
     :param str title: Title of content
     :type content: list/str/put_xxx()
     :param content: The content can be a string, the ``put_xxx()`` calls , or a list of them.
     :param bool open: Whether to expand the content. Default is ``False``.
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
@@ -1101,16 +1145,17 @@
         {{/contents}}
     </details>"""
     return put_widget(tpl, dict(title=title, contents=content, open=open), scope=scope,
                       position=position).enable_context_manager()
 
 
 @safely_destruct_output_when_exp('content')
-def put_scrollable(content=[], height=400, keep_bottom=False, border=True,
-                   scope=None, position=OutputPosition.BOTTOM, **kwargs) -> Output:
+def put_scrollable(content: Union[str, Output, List[Union[str, Output]]] = [],
+                   height: Union[int, Tuple[int, int]] = 400, keep_bottom: bool = False, border: bool = True,
+                   scope: str = None, position: int = OutputPosition.BOTTOM, **kwargs) -> Output:
     """Output a fixed height content area. scroll bar is displayed when the content exceeds the limit
 
     :type content: list/str/put_xxx()
     :param content: The content can be a string, the ``put_xxx()`` calls , or a list of them.
     :param int/tuple height: The height of the area (in pixels).
        ``height`` parameter also accepts ``(min_height, max_height)`` to indicate the range of height, for example,
        ``(100, 200)`` means that the area has a minimum height of 100 pixels and a maximum of 200 pixels.
@@ -1144,31 +1189,32 @@
     if not isinstance(content, (list, tuple, OutputList)):
         content = [content]
 
     content = [i if isinstance(i, Output) else put_text(i) for i in content]
 
     if 'max_height' in kwargs:
         import warnings
+
         # use stacklevel=2 to make the warning refer to the put_scrollable() call
         warnings.warn("`max_height` parameter is deprecated in `put_scrollable()`, use `height` instead.",
                       DeprecationWarning, stacklevel=2)
         height = kwargs['max_height']  # Backward compatible
 
-    try:
-        min_height, max_height = height
-    except Exception:
+    if isinstance(height, int):  # height is a int
         min_height, max_height = height, height
+    else:  # height is a tuple of (min_height, max_height)
+        min_height, max_height = height
 
     spec = _get_output_spec('scrollable', contents=content, min_height=min_height, max_height=max_height,
                             keep_bottom=keep_bottom, border=border, scope=scope, position=position)
     return Output(spec).enable_context_manager(container_selector='> div')
 
 
 @safely_destruct_output_when_exp('tabs')
-def put_tabs(tabs, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_tabs(tabs: List[Dict[str, Any]], scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """Output tabs.
 
     :param list tabs: Tab list, each item is a dict: ``{"title": "Title", "content": ...}`` .
        The ``content`` can be a string, the ``put_xxx()`` calls , or a list of them.
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
 
     .. exportable-codeblock::
@@ -1195,15 +1241,15 @@
         assert 'title' in tab and 'content' in tab
 
     spec = _get_output_spec('tabs', tabs=tabs, scope=scope, position=position)
     return Output(spec)
 
 
 @safely_destruct_output_when_exp('data')
-def put_widget(template, data, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_widget(template: str, data: Dict[str, Any], scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """Output your own widget
 
     :param template: html template, using `mustache.js <https://github.com/janl/mustache.js>`_ syntax
     :param dict data: Data used to render the template.
 
        The data can include the ``put_xxx()`` calls, and the JS function ``pywebio_output_parse`` can be used to
        parse the content of ``put_xxx()``. For string input, ``pywebio_output_parse`` will parse into text.
@@ -1242,15 +1288,16 @@
         })
     """
     spec = _get_output_spec('custom_widget', template=template, data=data, scope=scope, position=position)
     return Output(spec)
 
 
 @safely_destruct_output_when_exp('content')
-def put_row(content=[], size=None, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_row(content: List[Union[Output, None]] = [], size: str = None, scope: str = None,
+            position: int = OutputPosition.BOTTOM) -> Output:
     """Use row layout to output content. The content is arranged horizontally
 
     :param list content: Content list, the item is ``put_xxx()`` call or ``None``. ``None`` represents the space between the output
     :param str size:
        | Used to indicate the width of the items, is a list of width values separated by space.
        | Each width value corresponds to the items one-to-one. (``None`` item should also correspond to a width value).
        | By default, ``size`` assigns a width of 10 pixels to the ``None`` item, and distributes the width equally to the remaining items.
@@ -1282,15 +1329,16 @@
 
     """
     return _row_column_layout(content, flow='column', size=size, scope=scope,
                               position=position).enable_context_manager()
 
 
 @safely_destruct_output_when_exp('content')
-def put_column(content=[], size=None, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_column(content: List[Union[Output, None]] = [], size: str = None, scope: str = None,
+               position: int = OutputPosition.BOTTOM) -> Output:
     """Use column layout to output content. The content is arranged vertically
 
     :param list content: Content list, the item is ``put_xxx()`` call or ``None``. ``None`` represents the space between the output
     :param str size: Used to indicate the width of the items, is a list of width values separated by space.
         The format is the same as the ``size`` parameter of the `put_row()` function.
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
     """
@@ -1317,16 +1365,17 @@
         {{/contents}}
     </div>""".strip() % html.escape(style, quote=True)
     return put_widget(template=tpl, data=dict(contents=content), scope=scope,
                       position=position)
 
 
 @safely_destruct_output_when_exp('content')
-def put_grid(content, cell_width='auto', cell_height='auto', cell_widths=None, cell_heights=None, direction='row',
-             scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_grid(content: List[List[Union[Output, None]]], cell_width: str = 'auto', cell_height: str = 'auto',
+             cell_widths: str = None, cell_heights: str = None, direction: str = 'row', scope: str = None,
+             position: int = OutputPosition.BOTTOM) -> Output:
     """Output content using grid layout
 
     :param content: Content of grid, which is a two-dimensional list. The item of list is ``put_xxx()`` call or ``None``.
        ``None`` represents the space between the output. The item can use the `span()` to set the cell span.
     :param str cell_width: The width of grid cell.
     :param str cell_height: The height of grid cell.
     :param str cell_widths: The width of each column of the grid. The width values are separated by a space.
@@ -1340,15 +1389,15 @@
         | ``'column'`` : Places items by filling each column
 
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
 
     The format of width/height value in ``cell_width``,``cell_height``,``cell_widths``,``cell_heights``
     can refer to the ``size`` parameter of the `put_row()` function.
 
-    :Example:
+    Example:
 
     .. exportable-codeblock::
         :name: put_grid
         :summary: `put_grid()` usage
 
         put_grid([
             [put_text('A'), put_text('B'), put_text('C')],
@@ -1403,15 +1452,16 @@
             {{/.}}
         {{/contents}}
     </div>""".strip() % html.escape(css, quote=True)
     return put_widget(template=tpl, data=dict(contents=content), scope=scope, position=position)
 
 
 @safely_destruct_output_when_exp('content')
-def put_scope(name, content=[], scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_scope(name: str, content: Union[Output, List[Output]] = [], scope: str = None,
+              position: int = OutputPosition.BOTTOM) -> Output:
     """Output a scope
 
     :param str name:
     :param list/put_xxx() content: The initial content of the scope, can be ``put_xxx()`` or a list of it.
     :param int scope, position: Those arguments have the same meaning as for `put_text()`
     """
     if not isinstance(content, list):
@@ -1420,14 +1470,336 @@
     check_dom_name_value(name, 'scope name')
     dom_id = scope2dom(name, no_css_selector=True)
 
     spec = _get_output_spec('scope', dom_id=dom_id, contents=content, scope=scope, position=position)
     return Output(spec)
 
 
+class JSFunction:
+    def __init__(self, *params_and_body: str):
+        if not params_and_body:
+            raise ValueError('JSFunction must have at least body')
+        self.params = params_and_body[:-1]
+        self.body = params_and_body[-1]
+
+
+def put_datatable(
+        records: SequenceType[MappingType],
+        actions: SequenceType[Tuple[str, Callable[[Union[str, int, List[Union[str, int]]]], None]]] = None,
+        onselect: Callable[[Union[str, int, List[Union[str, int]]]], None] = None,
+        multiple_select=False,
+        id_field: str = None,
+        height: Union[str, int] = 600,
+        theme: "Literal['alpine', 'alpine-dark', 'balham', 'balham-dark', 'material']" = 'balham',
+        cell_content_bar=True,
+        instance_id='',
+        column_order: Union[SequenceType[str], MappingType] = None,
+        column_args: MappingType[Union[str, Tuple], MappingType] = None,
+        grid_args: MappingType[str, MappingType] = None,
+        enterprise_key='',
+        scope: str = None,
+        position: int = OutputPosition.BOTTOM
+) -> Output:
+    """
+    Output a datatable.
+
+    Compared with `put_table()`, `put_datatable()` is more suitable for displaying large amounts of data
+    (both data fields and data entries), while `put_table()` is more suitable for displaying diverse data types
+    (pictures, buttons, etc.) in cells.
+
+    This widget is powered by the awesome `ag-grid <https://www.ag-grid.com/>`_ library.
+
+    :param list[dict] records: data of rows, each row is a python ``dict``, which can be nested.
+    :param list actions: actions for selected row(s), they will be shown as buttons when row is selected.
+        The format of the action item: `(button_label:str, on_click:callable)`.
+        Specifically, ``None`` item is allowed, which will be rendered as a separator.
+        The ``on_click`` callback receives the selected row ID as parameter.
+    :param callable onselect: callback when row is selected, receives the selected row ID as parameter.
+    :param bool multiple_select: whether multiple rows can be selected.
+        When enabled, the ``on_click`` callback in ``actions`` and the ``onselect`` callback will receive
+        ID list of selected rows as parameter.
+    :param str/tuple id_field: row ID field, that is, the key of the row dict to uniquely identifies a row.
+        When not provide, the datatable will use the index in ``records`` to assign row ID.
+
+        .. collapse:: Notes when the row record is nested dict
+
+            To specify the ID field of a nested dict, use a tuple to specify the path of the ID field.
+            For example, if the row record is in ``{'a': {'b': ...}}`` format, you can use ``id_field=('a', 'b')``
+            to set ``'b'`` column as the ID field.
+
+    :param int/str height: widget height. When pass ``int`` type, the unit is pixel,
+        when pass ``str`` type, you can specify any valid CSS height value.
+        In particular, you can use ``'auto'`` to make the datatable auto-size it's height to fit the content.
+    :param str theme: datatable theme.
+        Available themes are: ``'balham'`` (default), ``'alpine'``, ``'alpine-dark'``, ``'balham-dark'``, ``'material'``.
+        You can preview the themes in `ag-grid official example <https://www.ag-grid.com/example/?theme=ag-theme-balham>`_.
+    :param bool cell_content_bar: whether to add a text bar to datatable to show the content of current focused cell.
+        Default is ``True``.
+    :param str instance_id: Assign a unique ID to the datatable, so that you can refer this datatable in
+        `datatable_update()`, `datatable_insert()` and `datatable_remove()` functions.
+
+    :param list column_order: column order, the order of the column names in the list will be used as the column order.
+        If not provided, the column order will be the same as the order of the keys in the first row of ``records``.
+        When provided, the column not in the list will not be shown.
+
+        .. collapse:: Notes when the row record is nested dict
+
+           Since the ``dict`` in python is ordered after py3.7, you can use dict to specify the column order when the
+           row record is nested dict. For example::
+
+                column_order = {'a': {'b': {'c': None, 'd': None}, 'e': None}, 'f': None}
+
+    :param column_args: column properties.
+        Dict type, the key is str to specify the column field, the value is
+        `ag-grid column properties <https://www.ag-grid.com/javascript-data-grid/column-properties/>`_ in dict.
+
+        .. collapse:: Notes when the row record is nested dict
+
+           Given the row record is in this format::
+
+               {
+                   "a": {"b": ..., "c": ...},
+                   "b": ...,
+                   "c": ...
+               }
+
+           When you set ``column_args={"b": settings}``, the column settings will be applied to the column ``a.b`` and ``b``.
+           Use tuple as key to specify the nested key path, for example, ``column_args={("a", "b"): settings}`` will only
+           apply the settings to column ``a.b``.
+
+    :param grid_args: ag-grid grid options.
+        Refer `ag-grid doc - grid options <https://www.ag-grid.com/javascript-data-grid/grid-options/>`_ for more information.
+    :param str enterprise_key: `ag-grid enterprise  <https://www.ag-grid.com/javascript-data-grid/licensing/>`_ license key.
+        When not provided, will use the ag-grid community version.
+
+    The ag-grid library is so powerful, and you can use the ``column_args`` and ``grid_args`` parameters to achieve
+    high customization.
+
+    Example of ``put_datatable()``:
+
+    .. exportable-codeblock::
+        :name: datatable
+        :summary: `put_datatable()` usage
+
+        import urllib.request
+        import json
+
+        with urllib.request.urlopen('https://fakerapi.it/api/v1/persons?_quantity=30') as f:
+            data = json.load(f)['data']
+
+        put_datatable(
+            data,
+            actions=[
+                ("Edit Email", lambda row_id: datatable_update('user', input("Email"), row_id, "email")),
+                ("Insert a Row", lambda row_id: datatable_insert('user', data[0], row_id)),
+                None,  # separator
+                ("Delete", lambda row_id: datatable_remove('user', row_id)),
+            ],
+            onselect=lambda row_id: toast(f'Selected row: {row_id}'),
+            instance_id='user'
+        )
+
+
+    .. collapse:: Advanced topic: Interact with ag-grid in Javascript
+
+        The ag-grid instance can be accessed with JS global variable ``ag_grid_${instance_id}_promise``::
+
+            ag_grid_xxx_promise.then(function(gridOptions) {
+                // gridOptions is the ag-grid gridOptions object
+                gridOptions.columnApi.autoSizeAllColumns();
+            });
+
+        To pass JS functions as value of ``column_args`` or ``grid_args``, you can use ``JSFunction`` object:
+
+            .. py:function:: JSFunction([param1], [param2], ... , [param n], body)
+
+            Example::
+
+                put_datatable(..., grid_args=dict(sortChanged=JSFunction("event", "console.log(event.source)")))
+
+        Since the ag-grid don't native support nested dict as row record, PyWebIO will internally flatten the nested
+        dict before passing to ag-grid. So when you access or modify data in ag-grid directly, you need to use the
+        following functions to help you convert the data:
+
+         - ``gridOptions.flatten_row(nested_dict_record)``: flatten the nested dict record to a flat dict record
+         - ``gridOptions.path2field(field_path_array)``: convert the field path array to field name used in ag-grid
+         - ``gridOptions.field2path(ag_grid_column_field_name)``: convert the field name back to field path array
+
+        The implement of `datatable_update()`, `datatable_insert` and `datatable_remove` functions are good examples
+        to show how to interact with ag-grid in Javascript.
+    """
+    actions = actions or []
+    column_args = column_args or {}
+    grid_args = grid_args or {}
+
+    if isinstance(height, int):
+        height = f"{height}px"
+    if height == 'auto' and len(records) > 1000:
+        height = '600px'
+        logger.warning("put_datatable: numbers of rows are too large to use auto height, use fix height instead")
+
+    if isinstance(id_field, str):
+        id_field = [id_field]
+
+    js_func_key = random_str(10)
+
+    def json_encoder(obj):
+        if isinstance(obj, JSFunction):
+            return dict(
+                __pywebio_js_function__=js_func_key,
+                params=obj.params,
+                body=obj.body,
+            )
+        raise TypeError
+
+    column_args = json.loads(json.dumps(column_args, default=json_encoder))
+    grid_args = json.loads(json.dumps(grid_args, default=json_encoder))
+
+    def callback(data: Dict):
+        rows = data['rows'] if multiple_select else data['rows'][0]
+
+        if "btn" not in data and onselect is not None:
+            return onselect(rows)
+
+        _, cb = actions[data['btn']]
+        return cb(rows)
+
+    callback_id = None
+    if actions or onselect:
+        callback_id = output_register_callback(callback)
+
+    action_labels = [a[0] if a else None for a in actions]
+    field_args = {k: v for k, v in column_args.items() if isinstance(k, str)}
+    path_args = [(k, v) for k, v in column_args.items() if not isinstance(k, str)]
+
+    if isinstance(column_order, (list, tuple)):
+        column_order = {k: None for k in column_order}
+
+    spec = _get_output_spec(
+        'datatable',
+        records=records, callback_id=callback_id, actions=action_labels, on_select=onselect is not None,
+        id_field=id_field, column_order=column_order,
+        multiple_select=multiple_select, field_args=field_args, path_args=path_args,
+        grid_args=grid_args, js_func_key=js_func_key, cell_content_bar=cell_content_bar,
+        height=height, theme=theme, enterprise_key=enterprise_key,
+        instance_id=instance_id,
+        scope=scope, position=position
+    )
+    return Output(spec)
+
+
+def datatable_update(
+        instance_id: str,
+        data: Any,
+        row_id: Union[int, str] = None,
+        field: Union[str, List[str], Tuple[str]] = None
+):
+    """
+    Update the whole data / a row / a cell of the datatable.
+
+    To use `datatable_update()`, you need to specify the ``instance_id`` parameter when calling :py:func:`put_datatable()`.
+
+    When ``row_id`` and ``field`` is not specified (``datatable_update(instance_id, data)``),
+    the whole data of datatable will be updated, in this case,
+    the ``data`` parameter should be a list of dict (same as ``records`` in :py:func:`put_datatable()`).
+
+    To update a row, specify the ``row_id`` parameter and pass the row data in dict to ``data``
+    parameter (``datatable_update(instance_id, data, row_id)``).
+    See ``id_field`` of :py:func:`put_datatable()` for more info of ``row_id``.
+
+    To update a cell, specify the ``row_id`` and ``field`` parameters, in this case, the ``data`` parameter should be
+    the cell value To update a row, specify the ``row_id`` parameter and pass the row data in dict to ``data``
+    parameter (``datatable_update(instance_id, data, row_id, field)``).
+    The ``field`` can be a tuple to indicate nested key path.
+    """
+    from .session import run_js
+
+    instance_id = f"ag_grid_{instance_id}_promise"
+    if row_id is None and field is None:  # update whole table
+        run_js("""window[instance_id] ? window[instance_id].then((grid) => {
+            grid.api.setRowData(data.map((row) => grid.flatten_row(row)))
+        }) : console.error(`Datatable instance [${instance_id}] not found`);
+        """, instance_id=instance_id, data=data)
+
+    if row_id is not None and field is None:  # update whole row
+        run_js("""window[instance_id] ? window[instance_id].then((grid) => {
+            let row = grid.api.getRowNode(row_id);
+            if (row) row.setData(grid.flatten_row(data))
+        }) : console.error(`Datatable instance [${instance_id}] not found`);
+        """, instance_id=instance_id, row_id=row_id, data=data)
+
+    if row_id is not None and field is not None:  # update field
+        if not isinstance(field, (list, tuple)):
+            field = [field]
+        run_js("""window[instance_id] ? window[instance_id].then((grid) => {
+            let row = grid.api.getRowNode(row_id);
+            if (row) 
+                row.setDataValue(grid.path2field(path), data) && 
+                grid.api.refreshClientSideRowModel();
+        }) : console.error(`Datatable instance [${instance_id}] not found`);
+        """, instance_id=instance_id, row_id=row_id, data=data, path=field)
+
+    if row_id is None and field is not None:
+        raise ValueError("`row_id` is required when provide `field`")
+
+
+def datatable_insert(instance_id: str, records: List, row_id=None):
+    """
+    Insert rows to datatable.
+
+    :param str instance_id: Datatable instance id
+        (i.e., the ``instance_id`` parameter when calling :py:func:`put_datatable()`)
+    :param dict/list[dict] records: row record or row record list to insert
+    :param str/int row_id: row id to insert before, if not specified, insert to the end
+
+    Note:
+        When use ``id_field=None`` (default) in :py:func:`put_datatable()`, the row id of new inserted rows will
+        auto increase from the last max row id.
+    """
+    from .session import run_js
+
+    if not isinstance(records, (list, tuple)):
+        records = [records]
+
+    instance_id = f"ag_grid_{instance_id}_promise"
+    run_js("""window[instance_id] ? window[instance_id].then((grid) => {
+        let row = grid.api.getRowNode(row_id);
+        let idx = row ? row.rowIndex : null;
+        grid.api.applyTransaction({
+            add: records.map((row) => grid.flatten_row(row)),
+            addIndex: idx,
+        });
+    }) : console.error(`Datatable instance [${instance_id}] not found`);
+    """, instance_id=instance_id, records=records, row_id=row_id)
+
+
+def datatable_remove(instance_id: str, row_ids: List):
+    """
+    Remove rows from datatable.
+
+    :param str instance_id: Datatable instance id
+        (i.e., the ``instance_id`` parameter when calling :py:func:`put_datatable()`)
+    :param int/str/list row_ids: row id or row id list to remove
+    """
+    from .session import run_js
+
+    instance_id = f"ag_grid_{instance_id}_promise"
+    if not isinstance(row_ids, (list, tuple)):
+        row_ids = [row_ids]
+    run_js("""window[instance_id] ? window[instance_id].then((grid) => {
+        let remove_rows = [];
+        for (let row_id of row_ids) {
+            let row = grid.api.getRowNode(row_id);
+            if (row) remove_rows.push(row.data);
+        }
+        grid.api.applyTransaction({remove: remove_rows});
+    }) : console.error(`Datatable instance [${instance_id}] not found`);
+    """, instance_id=instance_id, row_ids=row_ids)
+
+
 @safely_destruct_output_when_exp('contents')
 def output(*contents):
     """Placeholder of output
 
     .. deprecated:: 1.5
         See :ref:`User Guide <put_scope>` for new way to set css style for output.
 
@@ -1465,14 +1837,15 @@
         hobby.append('Music', put_text('Drama'))  # append Music, Drama to hobby
         ## ----
         hobby.insert(0, put_markdown('**Coding**'))  # insert the Coding into the top of the hobby
 
     """
 
     import warnings
+
     # use stacklevel=2 to make the warning refer to the output() call
     warnings.warn("`pywebio.output.output()` is deprecated since v1.5 and will remove in the future version, "
                   "use `pywebio.output.put_scope()` instead", DeprecationWarning, stacklevel=2)
 
     class OutputHandler(Output):
         """
         与 `Output` 的不同在于， 不会在销毁时(__del__)自动输出
@@ -1526,15 +1899,15 @@
         </div>"""
     out_spec = put_widget(template=tpl,
                           data=dict(contents=contents, dom_class_name=scope2dom(dom_name, no_css_selector=True)))
     return OutputHandler(Output.dump_dict(out_spec), ('.', dom_name))
 
 
 @safely_destruct_output_when_exp('outputs')
-def style(outputs, css_style) -> Union[Output, OutputList]:
+def style(outputs: Union[Output, List[Output]], css_style: str) -> Union[Output, OutputList]:
     """Customize the css style of output content
 
     .. deprecated:: 1.3
         See :ref:`User Guide <style>` for new way to set css style for output.
 
     :param outputs: The output content can be a ``put_xxx()`` call or a list of it.
     :type outputs: list/put_xxx()
@@ -1586,15 +1959,17 @@
         o.spec.setdefault('style', '')
         o.spec['style'] += ';%s' % css_style
 
     return outputs
 
 
 @safely_destruct_output_when_exp('content')
-def popup(title, content=None, size=PopupSize.NORMAL, implicit_close=True, closable=True):
+def popup(title: str, content: Union[str, Output, List[Union[str, Output]]] = None, size: str = PopupSize.NORMAL,
+          implicit_close: bool = True,
+          closable: bool = True):
     """
     Show a popup.
 
     ⚠️: In PyWebIO, you can't show multiple popup windows at the same time. Before displaying a new pop-up window,
     the existing popup on the page will be automatically closed. You can use `close_popup()` to close the popup manually.
 
     :param str title: The title of the popup.
@@ -1604,15 +1979,15 @@
     :param bool implicit_close: If enabled, the popup can be closed implicitly by clicking the content outside
         the popup window or pressing the ``Esc`` key. Default is ``False``.
     :param bool closable: Whether the user can close the popup window. By default, the user can close the popup
         by clicking the close button in the upper right of the popup window.
         When set to ``False``, the popup window can only be closed by :func:`popup_close()`,
         at this time the ``implicit_close`` parameter will be ignored.
 
-    ``popup()`` can be used in 3 ways: direct call, context manager, and decorator.
+    ``popup()`` can be used in 2 ways: direct call and context manager.
 
     * direct call:
 
     .. exportable-codeblock::
         :name: popup
         :summary: `popup()` usage
 
@@ -1641,28 +2016,14 @@
 
 
     The context manager will open a new output scope and return the scope name.
     The output in the context manager will be displayed on the popup window by default.
     After the context manager exits, the popup window will not be closed.
     You can still use the ``scope`` parameter of the output function to output to the popup.
 
-    * decorator:
-
-    .. exportable-codeblock::
-        :name: popup-decorator
-        :summary: `popup()` as decorator
-
-        @popup('Popup title')
-        def show_popup():
-            put_html('<h3>Popup Content</h3>')
-            put_text("I'm in a popup!")
-            ...
-
-        show_popup()
-
     """
     if content is None:
         content = []
 
     if not isinstance(content, (list, tuple, OutputList)):
         content = [content]
 
@@ -1682,15 +2043,16 @@
     """Close the current popup window.
 
     See also: `popup()`
     """
     send_msg(cmd='close_popup')
 
 
-def toast(content, duration=2, position='center', color='info', onclick=None):
+def toast(content: str, duration: float = 2, position: str = 'center', color: str = 'info',
+          onclick: Callable[[], None] = None):
     """Show a notification message.
 
     :param str content: Notification content.
     :param float duration: The duration of the notification display, in seconds. `0` means not to close automatically
         (at this time, a close button will be displayed next to the message, and the user can close the message manually)
     :param str position: Where to display the notification message. Available values are `'left'`, `'center'` and `'right'`.
     :param str color: Background color of the notification.
@@ -1725,15 +2087,15 @@
     send_msg(cmd='toast', spec=dict(content=content, duration=int(duration * 1000), position=position,
                                     color=color, callback_id=callback_id))
 
 
 clear_scope = clear
 
 
-def use_scope(name=None, clear=False, **kwargs):
+def use_scope(name: str = None, clear: bool = False, **kwargs):
     """use_scope(name=None, clear=False)
 
     Open or enter a scope. Can be used as context manager and decorator.
 
     See :ref:`User manual - use_scope() <use_scope>`
 
     :param str name: Scope name. If it is None, a globally unique scope name is generated.
```

### Comparing `pywebio-1.7.1/pywebio/pin.py` & `pywebio-1.8.0/pywebio/pin.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 `pin_wait_change()` is used to wait for the value of one of a list of pin widget to change, it 's a blocking function.
 
 `pin_update()` can be used to update attributes of pin widgets.
 
 Pin widgets
 ------------------
 Each pin widget function corresponds to an input function of :doc:`input <./input>` module.
-(For performance reasons, no pin widget for `file_upload() <pywebio.input.file_upload>` input function)
 
 The function of pin widget supports most of the parameters of the corresponding input function.
 Here lists the difference between the two in parameters:
 
  * The first parameter of pin widget function is always the name of the widget,
    and if you output two pin widgets with the same name, the previous one will expire.
  * Pin functions don't support the ``on_change`` and ``validate`` callbacks, and the ``required`` parameter.
@@ -84,24 +83,25 @@
 .. autofunction:: put_input
 .. autofunction:: put_textarea
 .. autofunction:: put_select
 .. autofunction:: put_checkbox
 .. autofunction:: put_radio
 .. autofunction:: put_slider
 .. autofunction:: put_actions
+.. autofunction:: put_file_upload
 
 Pin utils
 ------------------
 .. data:: pin
 
     Pin widgets value getter and setter.
 
     You can use attribute or key index of ``pin`` object to get the current value of a pin widget.
     By default, when accessing the value of a widget that does not exist, it returns ``None`` instead of
-    throwing an exception.
+    throwing an exception. You can enable the error raising by ``pin.use_strict()`` method.
 
     You can also use the ``pin`` object to set the value of pin widget:
 
     .. exportable-codeblock::
         :name: set-pin-value
         :summary: Use the `pin` object to set the value of pin widget
 
@@ -121,97 +121,111 @@
 .. autofunction:: pin_wait_change
 .. autofunction:: pin_update
 .. autofunction:: pin_on_change
 
 """
 
 import string
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from pywebio.input import parse_input_update_spec
-from pywebio.output import OutputPosition, Output
-from pywebio.output import _get_output_spec
-from .io_ctrl import send_msg, single_input_kwargs, output_register_callback
-from .session import next_client_event, chose_impl
+from pywebio.output import Output, OutputPosition, _get_output_spec
+
+from .io_ctrl import output_register_callback, send_msg, single_input_kwargs
+from .session import chose_impl, next_client_event
 from .utils import check_dom_name_value
 
 _pin_name_chars = set(string.ascii_letters + string.digits + '_-')
 
 __all__ = ['put_input', 'put_textarea', 'put_select', 'put_checkbox', 'put_radio', 'put_slider', 'put_actions',
-           'pin', 'pin_update', 'pin_wait_change', 'pin_on_change']
+           'put_file_upload', 'pin', 'pin_update', 'pin_wait_change', 'pin_on_change']
 
 
 def _pin_output(single_input_return, scope, position):
     input_kwargs = single_input_kwargs(single_input_return)
     spec = _get_output_spec('pin', input=input_kwargs['item_spec'], scope=scope, position=position)
     return Output(spec)
 
 
-def put_input(name, type='text', *, label='', value=None, placeholder=None, readonly=None, datalist=None,
-              help_text=None, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_input(name: str, type: str = 'text', *, label: str = '', value: str = None, placeholder: str = None,
+              readonly: bool = None, datalist: List[str] = None, help_text: str = None, scope: str = None,
+              position: int = OutputPosition.BOTTOM) -> Output:
     """Output an input widget. Refer to: `pywebio.input.input()`"""
     from pywebio.input import input
     check_dom_name_value(name, 'pin `name`')
     single_input_return = input(name=name, label=label, value=value, type=type, placeholder=placeholder,
                                 readonly=readonly, datalist=datalist, help_text=help_text)
     return _pin_output(single_input_return, scope, position)
 
 
-def put_textarea(name, *, label='', rows=6, code=None, maxlength=None, minlength=None, value=None, placeholder=None,
-                 readonly=None, help_text=None, scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_textarea(name: str, *, label: str = '', rows: int = 6, code: Union[bool, Dict] = None, maxlength: int = None,
+                 minlength: int = None, value: str = None, placeholder: str = None, readonly: bool = None,
+                 help_text: str = None, scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """Output a textarea widget. Refer to: `pywebio.input.textarea()`"""
     from pywebio.input import textarea
     check_dom_name_value(name, 'pin `name`')
     single_input_return = textarea(
         name=name, label=label, rows=rows, code=code, maxlength=maxlength,
         minlength=minlength, value=value, placeholder=placeholder, readonly=readonly, help_text=help_text)
     return _pin_output(single_input_return, scope, position)
 
 
-def put_select(name, options=None, *, label='', multiple=None, value=None, help_text=None,
-               scope=None, position=OutputPosition.BOTTOM) -> Output:
-    """Output a select widget. Refer to: `pywebio.input.select()`"""
+def put_select(name: str, options: List[Union[Dict[str, Any], Tuple, List, str]] = None, *, label: str = '',
+               multiple: bool = None, value: Union[List, str] = None, native: bool = None, help_text: str = None,
+               scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
+    """Output a select widget. Refer to: `pywebio.input.select()`
+
+    .. note::
+
+        Unlike `pywebio.input.select()`, when ``multiple=True`` and the user is using PC/macOS, `put_select()` will use
+        `bootstrap-select <https://github.com/snapappointments/bootstrap-select>`_ by default. Setting
+        ``native=True`` will force PyWebIO to use native select component on all platforms and vice versa.
+    """
     from pywebio.input import select
     check_dom_name_value(name, 'pin `name`')
     single_input_return = select(name=name, options=options, label=label, multiple=multiple,
-                                 value=value, help_text=help_text)
+                                 value=value, help_text=help_text, native=native)
     return _pin_output(single_input_return, scope, position)
 
 
-def put_checkbox(name, options=None, *, label='', inline=None, value=None, help_text=None,
-                 scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_checkbox(name: str, options: List[Union[Dict[str, Any], Tuple, List, str]] = None, *, label: str = '',
+                 inline: bool = None, value: List = None, help_text: str = None, scope: str = None,
+                 position: int = OutputPosition.BOTTOM) -> Output:
     """Output a checkbox widget. Refer to: `pywebio.input.checkbox()`"""
     from pywebio.input import checkbox
     check_dom_name_value(name, 'pin `name`')
     single_input_return = checkbox(name=name, options=options, label=label, inline=inline, value=value,
                                    help_text=help_text)
     return _pin_output(single_input_return, scope, position)
 
 
-def put_radio(name, options=None, *, label='', inline=None, value=None, help_text=None,
-              scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_radio(name: str, options: List[Union[Dict[str, Any], Tuple, List, str]] = None, *, label: str = '',
+              inline: bool = None, value: str = None, help_text: str = None, scope: str = None,
+              position: int = OutputPosition.BOTTOM) -> Output:
     """Output a radio widget. Refer to: `pywebio.input.radio()`"""
     from pywebio.input import radio
     check_dom_name_value(name, 'pin `name`')
     single_input_return = radio(name=name, options=options, label=label, inline=inline, value=value,
                                 help_text=help_text)
     return _pin_output(single_input_return, scope, position)
 
 
-def put_slider(name, *, label='', value=0, min_value=0, max_value=100, step=1, required=None, help_text=None,
-               scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_slider(name: str, *, label: str = '', value: Union[int, float] = 0, min_value: Union[int, float] = 0,
+               max_value: Union[int, float] = 100, step: int = 1, required: bool = None, help_text: str = None,
+               scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """Output a slide widget. Refer to: `pywebio.input.slider()`"""
     from pywebio.input import slider
     check_dom_name_value(name, 'pin `name`')
     single_input_return = slider(name=name, label=label, value=value, min_value=min_value, max_value=max_value,
                                  step=step, required=required, help_text=help_text)
     return _pin_output(single_input_return, scope, position)
 
 
-def put_actions(name, *, label='', buttons=None, help_text=None,
-                scope=None, position=OutputPosition.BOTTOM) -> Output:
+def put_actions(name: str, *, label: str = '', buttons: List[Union[Dict[str, Any], Tuple, List, str]] = None,
+                help_text: str = None, scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """Output a group of action button. Refer to: `pywebio.input.actions()`
 
     Unlike the ``actions()``, ``put_actions()`` won't submit any form, it will only set the value of the pin widget.
     Only 'submit' type button is available in pin widget version.
 
     .. versionadded:: 1.4
     """
@@ -220,14 +234,25 @@
     single_input_return = actions(name=name, label=label, buttons=buttons, help_text=help_text)
     input_kwargs = single_input_kwargs(single_input_return)
     for btn in input_kwargs['item_spec']['buttons']:
         assert btn['type'] == 'submit', "The `put_actions()` pin widget only accept 'submit' type button."
     return _pin_output(input_kwargs, scope, position)
 
 
+def put_file_upload(name: str, *, label: str = '', accept: Union[List, str] = None, placeholder: str = 'Choose file',
+                    multiple: bool = False, max_size: Union[int, str] = 0, max_total_size: Union[int, str] = 0,
+                    help_text: str = None, scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
+    """Output a file uploading widget. Refer to: `pywebio.input.file_upload()`"""
+    from pywebio.input import file_upload
+    check_dom_name_value(name, 'pin `name`')
+    single_input_return = file_upload(label=label, accept=accept, name=name, placeholder=placeholder, multiple=multiple,
+                                      max_size=max_size, max_total_size=max_total_size, help_text=help_text)
+    return _pin_output(single_input_return, scope, position)
+
+
 @chose_impl
 def get_client_val():
     res = yield next_client_event()
     assert res['event'] == 'js_yield', "Internal Error, please report this bug on " \
                                        "https://github.com/wang0618/PyWebIO/issues"
     return res['data']
 
@@ -246,41 +271,41 @@
     def use_strict(self):
         """
         Enable strict mode for getting pin widget value.
         An AssertionError will be raised when try to get value of pin widgets that are currently not in the page.
         """
         object.__setattr__(self, '_strict', True)
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str):
         """__getattr__ is only invoked if the attribute wasn't found the usual ways"""
         if name.startswith('__'):
             raise AttributeError('Pin object has no attribute %r' % name)
         return self.__getitem__(name)
 
-    def __getitem__(self, name):
+    def __getitem__(self, name: str):
         check_dom_name_value(name, 'pin `name`')
         return get_pin_value(name, self._strict)
 
-    def __setattr__(self, name, value):
+    def __setattr__(self, name: str, value):
         """
         __setattr__ will be invoked regardless of whether the attribute be found
         """
         assert name != 'use_strict', "'use_strict' is a reserve name, can't use as pin widget name"
         check_dom_name_value(name, 'pin `name`')
         self.__setitem__(name, value)
 
-    def __setitem__(self, name, value):
+    def __setitem__(self, name: str, value):
         send_msg('pin_update', spec=dict(name=name, attributes={"value": value}))
 
 
 # pin widgets value getter (and setter).
 pin = Pin_()
 
 
-def pin_wait_change(*names, timeout=None):
+def pin_wait_change(*names, timeout: Optional[int] = None):
     """``pin_wait_change()`` listens to a list of pin widgets, when the value of any widgets changes,
     the function returns with the name and value of the changed widget.
 
     :param str names: List of names of pin widget
     :param int/None timeout: If ``timeout`` is a positive number, ``pin_wait_change()`` blocks at most ``timeout`` seconds
         and returns ``None`` if no changes to the widgets within that time. Set to ``None`` (the default) to disable timeout.
     :return dict/None: ``{"name": name of the changed widget, "value": current value of the changed widget }`` ,
@@ -314,27 +339,27 @@
         names = names[0]
 
     send_msg('pin_wait', spec=dict(names=names, timeout=timeout))
 
     return get_client_val()
 
 
-def pin_update(name, **spec):
+def pin_update(name: str, **spec):
     """Update attributes of pin widgets.
 
     :param str name: The ``name`` of the target input widget.
     :param spec: The pin widget parameters need to be updated.
        Note that those parameters can not be updated: ``type``, ``name``, ``code``, ``multiple``
     """
     check_dom_name_value(name, 'pin `name`')
     attributes = parse_input_update_spec(spec)
     send_msg('pin_update', spec=dict(name=name, attributes=attributes))
 
 
-def pin_on_change(name, onchange=None, clear=False, init_run=False, **callback_options):
+def pin_on_change(name: str, onchange: Callable[[Any], None] = None, clear: bool = False, init_run: bool = False, **callback_options):
     """
     Bind a callback function to pin widget, the function will be called when user change the value of the pin widget.
 
     The ``onchange`` callback is invoked with one argument, the changed value of the pin widget.
     You can bind multiple functions to one pin widget, those functions will be invoked sequentially
     (default behavior, can be changed by `clear` parameter).
 
@@ -347,13 +372,14 @@
     :param callback_options: Other options of the ``onclick`` callback.
        Refer to the ``callback_options`` parameter of :func:`put_buttons() <pywebio.output.put_buttons>`
 
     .. versionadded:: 1.6
     """
     assert not (onchange is None and clear is False), "When `onchange` is `None`, `clear` must be `True`"
     if onchange is not None:
-        callback_id = output_register_callback(onchange, **callback_options)
+        callback = lambda data: onchange(data['value'])
+        callback_id = output_register_callback(callback, **callback_options)
         if init_run:
             onchange(pin[name])
     else:
         callback_id = None
     send_msg('pin_onchange', spec=dict(name=name, callback_id=callback_id, clear=clear))
```

### Comparing `pywebio-1.7.1/pywebio/platform/__init__.py` & `pywebio-1.8.0/pywebio/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/platform/adaptor/http.py` & `pywebio-1.8.0/pywebio/platform/adaptor/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 import asyncio
 import fnmatch
 import json
 import logging
 import threading
 import time
 from contextlib import contextmanager
-from typing import Dict
+from typing import Dict, Optional, List
+from collections import deque
 
 from ..page import make_applications, render_page
 from ..utils import deserialize_binary_event
-from ...session import CoroutineBasedSession, Session, ThreadBasedSession, register_session_implement_for_target
-from ...session.base import get_session_info_from_headers
+from ...session import CoroutineBasedSession, ThreadBasedSession, register_session_implement_for_target
+from ...session.base import get_session_info_from_headers, Session
 from ...utils import random_str, LRUDict, isgeneratorfunction, iscoroutinefunction, check_webio_js
 
 
 class HttpContext:
     """一次Http请求的上下文， 不同的后端框架需要根据框架提供的方法实现本类的方法
 
     The context of an Http request"""
@@ -31,47 +32,37 @@
     backend_name = ''  # 当前使用的Web框架名
 
     def request_obj(self):
         """返回当前请求对象
         Return the current request object"""
         pass
 
-    def request_method(self):
+    def request_method(self) -> str:
         """返回当前请求的方法，大写
         Return the HTTP method of the current request, uppercase"""
         pass
 
-    def request_headers(self) -> dict:
+    def request_headers(self) -> Dict:
         """返回当前请求的header字典
         Return the header dictionary of the current request"""
         pass
 
-    def request_url_parameter(self, name, default=None):
+    def request_url_parameter(self, name, default=None) -> str:
         """返回当前请求的URL参数
         Returns the value of the given URL parameter of the current request"""
         pass
 
-    def request_body(self):
+    def request_body(self) -> bytes:
         """返回当前请求的body数据
         Returns the data of the current request body
 
         :return: bytes/bytearray
         """
         return b''
 
-    def request_json(self) -> dict:
-        """返回当前请求的json反序列化后的内容，若请求数据不为json格式，返回None
-        Return the data (json deserialization) of the currently requested, if the data is not in json format, return None"""
-        try:
-            if self.request_headers().get('content-type') == 'application/octet-stream':
-                return deserialize_binary_event(self.request_body())
-            return json.loads(self.request_body())
-        except Exception:
-            return None
-
     def set_header(self, name, value):
         """为当前响应设置header
         Set a header for the current response"""
         pass
 
     def set_status(self, status):
         """为当前响应设置http status
@@ -88,36 +79,85 @@
         pass
 
     def get_response(self):
         """获取当前的响应对象，用于在视图函数中返回
         Get the current response object"""
         pass
 
-    def get_client_ip(self):
+    def get_client_ip(self) -> str:
         """获取用户的ip
         Get the user's ip"""
         pass
 
 
 logger = logging.getLogger(__name__)
 _event_loop = None
 
 
+class ReliableTransport:
+    def __init__(self, session: Session, message_window: int = 4):
+        self.session = session
+        self.messages = deque()
+        self.window_size = message_window
+        self.min_msg_id = 0  # the id of the first message in the window
+        self.finished_event_id = -1  # the id of the last finished event
+
+    @staticmethod
+    def close_message(ack):
+        return dict(
+            commands=[[dict(command='close_session')]],
+            seq=ack + 1
+        )
+
+    def push_event(self, events: List[Dict], seq: int) -> int:
+        """Send client events to the session and return the success message count"""
+        if not events:
+            return 0
+
+        submit_cnt = 0
+        for eid, event in enumerate(events, start=seq):
+            if eid > self.finished_event_id:
+                self.finished_event_id = eid  # todo: use lock for check and set operation
+                self.session.send_client_event(event)
+                submit_cnt += 1
+
+        return submit_cnt
+
+    def get_response(self, ack=0):
+        """
+        ack num is the number of messages that the client has received.
+        response is a list of messages that the client should receive, along with their min id `seq`.
+        """
+        while ack >= self.min_msg_id and self.messages:
+            self.messages.popleft()
+            self.min_msg_id += 1
+
+        if len(self.messages) < self.window_size:
+            msgs = self.session.get_task_commands()
+            if msgs:
+                self.messages.append(msgs)
+
+        return dict(
+            commands=list(self.messages),
+            seq=self.min_msg_id,
+            ack=self.finished_event_id
+        )
+
+
 # todo: use lock to avoid thread race condition
 class HttpHandler:
     """基于HTTP的后端Handler实现
 
     .. note::
         Don't need a lock when access HttpHandler._webio_sessions, See：
         https://stackoverflow.com/questions/1312331/using-a-global-dictionary-with-threads-in-python
 
     """
-    # type: Dict[str, Session]
     _webio_sessions = {}  # WebIOSessionID -> WebIOSession()
-    _webio_last_commands = {}  # WebIOSessionID -> (last commands, commands sequence id)
+    _webio_transports = {}  # WebIOSessionID -> ReliableTransport(), type: Dict[str, ReliableTransport]
     _webio_expire = LRUDict()  # WebIOSessionID -> last active timestamp. In increasing order of last active time
     _webio_expire_lock = threading.Lock()
 
     _last_check_session_expire_ts = 0  # Timestamp of the last check session validation
 
     # After processing the POST request, wait for WAIT_MS_ON_POST milliseconds before generate response
     WAIT_MS_ON_POST = 100
@@ -140,31 +180,21 @@
 
             # clean this session
             logger.debug("session %s expired" % sid)
             session = cls._webio_sessions.get(sid)
             if session:
                 session.close(nonblock=True)
                 del cls._webio_sessions[sid]
+                del cls._webio_transports[sid]
 
     @classmethod
     def _remove_webio_session(cls, sid):
         cls._webio_sessions.pop(sid, None)
         cls._webio_expire.pop(sid, None)
 
-    @classmethod
-    def get_response(cls, sid, ack=0):
-        commands, seq = cls._webio_last_commands.get(sid, ([], 0))
-        if ack == seq:
-            webio_session = cls._webio_sessions[sid]
-            commands = webio_session.get_task_commands()
-            seq += 1
-            cls._webio_last_commands[sid] = (commands, seq)
-
-        return {'commands': commands, 'seq': seq}
-
     def _process_cors(self, context: HttpContext):
         """Handling cross-domain requests: check the source of the request and set headers"""
         origin = context.request_headers().get('Origin', '')
         if self.check_origin(origin):
             context.set_header('Access-Control-Allow-Origin', origin)
             context.set_header('Access-Control-Allow-Methods', 'GET, POST')
             context.set_header('Access-Control-Allow-Headers', 'content-type, webio-session-id')
@@ -206,14 +236,22 @@
         return context.get_response()
 
     def get_cdn(self, context):
         if self.cdn is True and context.request_url_parameter('_pywebio_cdn', '') == 'false':
             return False
         return self.cdn
 
+    def read_event_data(self, context: HttpContext) -> List[Dict]:
+        try:
+            if context.request_headers().get('content-type') == 'application/octet-stream':
+                return [deserialize_binary_event(context.request_body())]
+            return json.loads(context.request_body())
+        except Exception:
+            return []
+
     @contextmanager
     def handle_request_context(self, context: HttpContext):
         """called when every http request"""
         cls = type(self)
 
         if _event_loop:
             asyncio.set_event_loop(_event_loop)
@@ -237,59 +275,67 @@
         # 对首页HTML的请求
         if 'webio-session-id' not in request_headers:
             app = self.app_loader(context)
             html = render_page(app, protocol='http', cdn=self.get_cdn(context))
             context.set_content(html)
             return context.get_response()
 
-        webio_session_id = None
+        ack = int(context.request_url_parameter('ack', 0))
+        webio_session_id = request_headers['webio-session-id']
+        new_request = False
+        if webio_session_id.startswith('NEW-'):
+            new_request = True
+            webio_session_id = webio_session_id[4:]
 
-        # 初始请求，创建新 Session
-        if not request_headers['webio-session-id'] or request_headers['webio-session-id'] == 'NEW':
+        if new_request and webio_session_id not in cls._webio_sessions:  # 初始请求，创建新 Session
             if context.request_method() == 'POST':  # 不能在POST请求中创建Session，防止CSRF攻击
                 context.set_status(403)
                 return context.get_response()
 
-            webio_session_id = random_str(24)
-            context.set_header('webio-session-id', webio_session_id)
             session_info = get_session_info_from_headers(context.request_headers())
             session_info['user_ip'] = context.get_client_ip()
             session_info['request'] = context.request_obj()
             session_info['backend'] = context.backend_name
             session_info['protocol'] = 'http'
 
             application = self.app_loader(context)
 
             if iscoroutinefunction(application) or isgeneratorfunction(application):
                 session_cls = CoroutineBasedSession
             else:
                 session_cls = ThreadBasedSession
             webio_session = session_cls(application, session_info=session_info)
             cls._webio_sessions[webio_session_id] = webio_session
-            yield type(self).WAIT_MS_ON_POST / 1000.0  # <--- <--- <--- <--- <--- <--- <--- <--- <--- <--- <--- <---
-        elif request_headers['webio-session-id'] not in cls._webio_sessions:  # WebIOSession deleted
-            context.set_content(dict(commands=[dict(command='close_session')]), json_type=True)
+            cls._webio_transports[webio_session_id] = ReliableTransport(webio_session)
+            yield cls.WAIT_MS_ON_POST / 1000.0  # <--- <--- <--- <--- <--- <--- <--- <--- <--- <--- <--- <---
+        elif webio_session_id not in cls._webio_sessions:  # WebIOSession deleted
+            close_msg = ReliableTransport.close_message(ack)
+            context.set_content(close_msg, json_type=True)
             return context.get_response()
         else:
-            webio_session_id = request_headers['webio-session-id']
+            # in this case, the request_headers['webio-session-id'] may also startswith NEW,
+            # this is because the response for the previous new session request has not been received by the client,
+            # and the client has sent a new request with the same session id.
             webio_session = cls._webio_sessions[webio_session_id]
 
         if context.request_method() == 'POST':  # client push event
-            if context.request_json() is not None:
-                webio_session.send_client_event(context.request_json())
+            seq = int(context.request_url_parameter('seq', 0))
+            event_data = self.read_event_data(context)
+            submit_cnt = cls._webio_transports[webio_session_id].push_event(event_data, seq)
+            if submit_cnt > 0:
                 yield type(self).WAIT_MS_ON_POST / 1000.0  # <--- <--- <--- <--- <--- <--- <--- <--- <--- <--- <--- <---
         elif context.request_method() == 'GET':  # client pull messages
             pass
 
         cls._webio_expire[webio_session_id] = time.time()
 
         self.interval_cleaning()
 
-        ack = int(context.request_url_parameter('ack', 0))
-        context.set_content(type(self).get_response(webio_session_id, ack=ack), json_type=True)
+        resp = cls._webio_transports[webio_session_id].get_response(ack)
+        context.set_content(resp, json_type=True)
 
         if webio_session.closed():
             self._remove_webio_session(webio_session_id)
 
         return context.get_response()
 
     def __init__(self, applications=None, app_loader=None,
```

### Comparing `pywebio-1.7.1/pywebio/platform/adaptor/ws.py` & `pywebio-1.8.0/pywebio/platform/adaptor/ws.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,81 @@
+import abc
 import asyncio
 import json
 import logging
 import time
 import typing
-from typing import Dict
-import abc
+from typing import Dict, Optional
+
+from ...session import CoroutineBasedSession, Session, ThreadBasedSession
+from ...utils import LRUDict, iscoroutinefunction, isgeneratorfunction, random_str
 from ..utils import deserialize_binary_event
-from ...session import CoroutineBasedSession, ThreadBasedSession, Session
-from ...utils import iscoroutinefunction, isgeneratorfunction, \
-    random_str, LRUDict
 
 logger = logging.getLogger(__name__)
 
 
-class _state:
-    # only used in reconnect enabled
+# used to store global state when reconnect enabled
+class _reconnect_state:
     # used to clean up session
     detached_sessions = LRUDict()  # session_id -> detached timestamp. In increasing order of the time
 
     # unclosed and unexpired session
-    # only used in reconnect enabled
     # used to clean up session
     # used to retrieve session by id when new connection
     unclosed_sessions: Dict[str, Session] = {}  # session_id -> session
 
     # the messages that can't deliver to browser when session close due to connection lost
-    undelivered_messages: Dict[str, list] = {}  # session_id -> unhandled message list
+    session_will_messages: Dict[str, list] = {}  # session_id -> unhandled message list
 
     # used to get the active conn in session's callbacks
     active_connections: Dict[str, 'WebSocketConnection'] = {}  # session_id -> WSHandler
 
     expire_second = 0
 
 
 def set_expire_second(sec):
-    _state.expire_second = max(_state.expire_second, sec)
+    _reconnect_state.expire_second = max(_reconnect_state.expire_second, sec)
 
 
 def clean_expired_sessions():
-    while _state.detached_sessions:
-        session_id, detached_ts = _state.detached_sessions.popitem(last=False)  # 弹出最早过期的session
+    while _reconnect_state.detached_sessions:
+        session_id, detached_ts = _reconnect_state.detached_sessions.popitem(last=False)  # 弹出最早过期的session
 
-        if time.time() < detached_ts + _state.expire_second:
+        if time.time() < detached_ts + _reconnect_state.expire_second:
             # this session is not expired
-            _state.detached_sessions[session_id] = detached_ts  # restore
-            _state.detached_sessions.move_to_end(session_id, last=False)  # move to head
+            _reconnect_state.detached_sessions[session_id] = detached_ts  # restore
+            _reconnect_state.detached_sessions.move_to_end(session_id, last=False)  # move to head
             break
 
         # clean this session
         logger.debug("session %s expired" % session_id)
-        _state.active_connections.pop(session_id, None)
-        _state.undelivered_messages.pop(session_id, None)
-        session = _state.unclosed_sessions.pop(session_id, None)
+        _reconnect_state.active_connections.pop(session_id, None)
+        _reconnect_state.session_will_messages.pop(session_id, None)
+        session = _reconnect_state.unclosed_sessions.pop(session_id, None)
         if session:
             session.close(nonblock=True)
 
 
 _session_clean_task_started = False
 
 
 async def session_clean_task():
     global _session_clean_task_started
-    if _session_clean_task_started or not _state.expire_second:
+    if _session_clean_task_started or not _reconnect_state.expire_second:
         return
 
     _session_clean_task_started = True
     logger.debug("Start session cleaning task")
     while True:
         try:
             clean_expired_sessions()
         except Exception:
             logger.exception("Error when clean expired sessions")
 
-        await asyncio.sleep(_state.expire_second // 2)
+        await asyncio.sleep(_reconnect_state.expire_second // 2)
 
 
 class WebSocketConnection(abc.ABC):
     @abc.abstractmethod
     def get_query_argument(self, name) -> typing.Optional[str]:
         pass
 
@@ -99,71 +98,79 @@
 
 class WebSocketHandler:
     """
     hold by one connection,
     share one session with multiple connection in session lifetime, but one conn at a time
     """
 
-    session_id: str = None
-    session: Session = None  # the session that current connection attaches
+    session_id: Optional[str] = None
+    session: Optional[Session] = None  # the session that current connection attaches
     connection: WebSocketConnection
     reconnectable: bool
 
     def __init__(self, connection: WebSocketConnection, application, reconnectable: bool, ioloop=None):
         logger.debug("WebSocket opened")
         self.connection = connection
         self.reconnectable = reconnectable
         self.session_id = connection.get_query_argument('session')
         self.ioloop = ioloop or asyncio.get_event_loop()
 
         if self.session_id in ('NEW', None):  # 初始请求，创建新 Session
             self._init_session(application)
             if reconnectable:
+                _reconnect_state.active_connections[self.session_id] = self.connection
+                _reconnect_state.unclosed_sessions[self.session_id] = self.session
                 # set session id to client, so the client can send it back to server to recover a session when it
                 # resumes form a connection lost
                 connection.write_message(dict(command='set_session_id', spec=self.session_id))
-        elif self.session_id not in _state.unclosed_sessions:  # session is expired
+        elif self.session_id not in _reconnect_state.unclosed_sessions:  # session is expired
             bye_msg = dict(command='close_session')
-            for m in _state.undelivered_messages.get(self.session_id, [bye_msg]):
+            for m in _reconnect_state.session_will_messages.get(self.session_id, [bye_msg]):
                 try:
                     connection.write_message(m)
                 except Exception:
                     logger.exception("Error in sending message via websocket")
-        else:
-            self.session = _state.unclosed_sessions[self.session_id]
-            _state.detached_sessions.pop(self.session_id, None)
-            _state.active_connections[self.session_id] = connection
+        else:  # resumes form a connection lost
+            self.session = _reconnect_state.unclosed_sessions[self.session_id]
+            _reconnect_state.detached_sessions.pop(self.session_id, None)
+            _reconnect_state.active_connections[self.session_id] = connection
             # send the latest messages to client
-            self._send_msg_to_client(self.session)
+            self._send_msg_to_client()
 
         logger.debug('session id: %s' % self.session_id)
 
     def _init_session(self, application):
         session_info = self.connection.make_session_info()
         self.session_id = random_str(24)
-        # todo: only set item when reconnection enabled
-        _state.active_connections[self.session_id] = self.connection
 
         if iscoroutinefunction(application) or isgeneratorfunction(application):
             self.session = CoroutineBasedSession(
                 application, session_info=session_info,
                 on_task_command=self._send_msg_to_client,
                 on_session_close=self._close_from_session)
         else:
             self.session = ThreadBasedSession(
                 application, session_info=session_info,
                 on_task_command=self._send_msg_to_client,
                 on_session_close=self._close_from_session,
                 loop=self.ioloop)
-        _state.unclosed_sessions[self.session_id] = self.session
 
-    def _send_msg_to_client(self, session):
-        # self.connection may not be active,
-        # here we need the active connection for this session
-        conn = _state.active_connections.get(self.session_id)
+    def _get_active_connection(self) -> Optional[WebSocketConnection]:
+        # when reconnect enabled, the active connection for this session is in _reconnect_state.active_connections,
+        # otherwise, it's self.connection.
+        if self.reconnectable:
+            conn = _reconnect_state.active_connections.get(self.session_id)
+        else:
+            conn = self.connection
+
+        return conn
+
+    def _send_msg_to_client(self, session: Session = None):
+        conn = self._get_active_connection()
+        session = session or self.session
 
         if not conn or conn.closed():
             return
 
         for msg in session.get_task_commands():
             try:
                 conn.write_message(msg)
@@ -171,38 +178,36 @@
                 logger.exception('Data serialization error: %s\n'
                                  'This may be because you pass the wrong type of parameter to the function'
                                  ' of PyWebIO.\nData content: %s', e, msg)
             except Exception:
                 logger.exception("Error in sending message via websocket")
 
     def _close_from_session(self):
-        session = _state.unclosed_sessions[self.session_id]
-        if self.session_id in _state.active_connections:
-            # send the undelivered messages to client
-            self._send_msg_to_client(session=session)
-        else:
-            _state.undelivered_messages[self.session_id] = session.get_task_commands()
-
-        conn = _state.active_connections.pop(self.session_id, None)
-        _state.unclosed_sessions.pop(self.session_id, None)
+        conn = self._get_active_connection()
         if conn and not conn.closed():
+            self._send_msg_to_client()
             conn.close()
+        elif self.reconnectable:  # no active connection, and reconnect is enabled
+            _reconnect_state.session_will_messages[self.session_id] = self.session.get_task_commands()
+        self.session = None
 
     def send_client_data(self, data):
         if isinstance(data, bytes):
             event = deserialize_binary_event(data)
         else:
             event = json.loads(data)
         if event is None:
             return
         self.session.send_client_event(event)
 
     def notify_connection_lost(self):
-        _state.active_connections.pop(self.session_id, None)
-        if not self.reconnectable:
+        logger.debug("WebSocket closed")
+        if not self.reconnectable and self.session:
             # when the connection lost is caused by `on_session_close()`, it's OK to close the session here though.
             # because the `session.close()` is reentrant
             self.session.close(nonblock=True)
-        else:
-            if self.session_id in _state.unclosed_sessions:
-                _state.detached_sessions[self.session_id] = time.time()
-        logger.debug("WebSocket closed")
+            self.session = None  # reset the reference
+            return
+
+        _reconnect_state.active_connections.pop(self.session_id, None)
+        if self.session_id in _reconnect_state.unclosed_sessions:
+            _reconnect_state.detached_sessions[self.session_id] = time.time()
```

### Comparing `pywebio-1.7.1/pywebio/platform/aiohttp.py` & `pywebio-1.8.0/pywebio/platform/aiohttp.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 import os
 import typing
 from functools import partial
 from urllib.parse import urlparse
 
 from aiohttp import web
 
+from . import page
 from .adaptor import ws as ws_adaptor
 from .page import make_applications, render_page
 from .remote_access import start_remote_access_service
 from .tornado import open_webbrowser_on_server_started
 from .utils import cdn_validation, print_listen_address
 from ..session import register_session_implement_for_target, Session
 from ..session.base import get_session_info_from_headers
-from ..utils import get_free_port, STATIC_PATH
+from ..utils import get_free_port, STATIC_PATH, parse_file_size
 
 logger = logging.getLogger(__name__)
 
 
 def _check_origin(origin, allowed_origins, host):
     if _is_same_site(origin, host):
         return True
@@ -121,28 +122,31 @@
 
         return ws
 
     return wshandle
 
 
 def webio_handler(applications, cdn=True, reconnect_timeout=0, allowed_origins=None, check_origin=None,
-                  websocket_settings=None):
+                  max_payload_size='200M', websocket_settings=None):
     """Get the `Request Handler <https://docs.aiohttp.org/en/stable/web_quickstart.html#aiohttp-web-handler>`_ coroutine for running PyWebIO applications in aiohttp.
     The handler communicates with the browser by WebSocket protocol.
 
     The arguments of ``webio_handler()`` have the same meaning as for :func:`pywebio.platform.aiohttp.start_server`
 
     :return: aiohttp Request Handler
     """
     applications = make_applications(applications)
     for target in applications.values():
         register_session_implement_for_target(target)
 
     websocket_settings = websocket_settings or {}
 
+    page.MAX_PAYLOAD_SIZE = max_payload_size = parse_file_size(max_payload_size)
+    websocket_settings.setdefault('max_msg_size', max_payload_size)
+
     cdn = cdn_validation(cdn, 'error')
 
     if check_origin is None:
         check_origin_func = partial(_check_origin, allowed_origins=allowed_origins or [])
     else:
         check_origin_func = lambda origin, host: _is_same_site(origin, host) or check_origin(origin)
 
@@ -166,18 +170,20 @@
 
 
 def start_server(applications, port=0, host='', debug=False,
                  cdn=True, static_dir=None, remote_access=False,
                  reconnect_timeout=0,
                  allowed_origins=None, check_origin=None,
                  auto_open_webbrowser=False,
+                 max_payload_size='200M',
                  websocket_settings=None,
                  **aiohttp_settings):
     """Start a aiohttp server to provide the PyWebIO application as a web service.
 
+
     :param dict websocket_settings: The  parameters passed to the constructor of ``aiohttp.web.WebSocketResponse``.
        For details, please refer: https://docs.aiohttp.org/en/stable/web_reference.html#websocketresponse
     :param aiohttp_settings: Additional keyword arguments passed to the constructor of ``aiohttp.web.Application``.
        For details, please refer: https://docs.aiohttp.org/en/stable/web_reference.html#application
 
     The rest arguments of ``start_server()`` have the same meaning as for :func:`pywebio.platform.tornado.start_server`
     """
@@ -188,15 +194,16 @@
 
     if port == 0:
         port = get_free_port()
 
     cdn = cdn_validation(cdn, 'warn')
 
     handler = webio_handler(applications, cdn=cdn, allowed_origins=allowed_origins, reconnect_timeout=reconnect_timeout,
-                            check_origin=check_origin, websocket_settings=websocket_settings)
+                            check_origin=check_origin, max_payload_size=max_payload_size,
+                            websocket_settings=websocket_settings)
 
     app = web.Application(**aiohttp_settings)
     app.router.add_routes([web.get('/', handler)])
     if static_dir is not None:
         app.router.add_routes([web.static('/static', static_dir)])
     app.router.add_routes(static_routes())
```

### Comparing `pywebio-1.7.1/pywebio/platform/bokeh.py` & `pywebio-1.8.0/pywebio/platform/bokeh.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,21 +140,21 @@
 
     url = _server_url(info.server_host, server.port)
 
     from bokeh.embed import server_document
     script = server_document(url, resources=None)
 
     script = re.sub(r'<script(.*?)>([\s\S]*?)</script>',  # lgtm [py/bad-tag-filter]
-    r"""
-    <script \g<1>>
-        requirejs(['bokeh', 'bokeh-widgets', 'bokeh-tables'], function(Bokeh) {
-            \g<2>
-        });
-    </script>
-    """, script, flags=re.I)
+                    r"""
+                    <script \g<1>>
+                        requirejs(['bokeh', 'bokeh-widgets', 'bokeh-tables'], function(Bokeh) {
+                            \g<2>
+                        });
+                    </script>
+                    """, script, flags=re.I)
 
     put_html(script, sanitize=False)
 
 
 def try_install_bokeh_hook():
     """尝试安装bokeh支持"""
     try:
```

### Comparing `pywebio-1.7.1/pywebio/platform/django.py` & `pywebio-1.8.0/pywebio/platform/django.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,19 +98,19 @@
     return view_func
 
 
 urlpatterns = []
 
 
 def wsgi_app(applications, cdn=True,
-                 static_dir=None,
-                 allowed_origins=None, check_origin=None,
-                 session_expire_seconds=None,
-                 session_cleanup_interval=None,
-                 debug=False, max_payload_size='200M', **django_options):
+             static_dir=None,
+             allowed_origins=None, check_origin=None,
+             session_expire_seconds=None,
+             session_cleanup_interval=None,
+             debug=False, max_payload_size='200M', **django_options):
     """Get the Django WSGI app for running PyWebIO applications.
 
     The arguments of ``wsgi_app()`` have the same meaning as for :func:`pywebio.platform.django.start_server`
     """
     global urlpatterns
 
     from django.conf import settings
```

### Comparing `pywebio-1.7.1/pywebio/platform/fastapi.py` & `pywebio-1.8.0/pywebio/platform/fastapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.responses import HTMLResponse
 from starlette.routing import Route, WebSocketRoute, Mount
 from starlette.websockets import WebSocket, WebSocketState
 from starlette.websockets import WebSocketDisconnect
 
+from . import page
 from .page import make_applications, render_page
 from .remote_access import start_remote_access_service
 from .tornado import open_webbrowser_on_server_started
 from .utils import cdn_validation, OriginChecker, print_listen_address
 from ..session import register_session_implement_for_target, Session
 from ..session.base import get_session_info_from_headers
-from ..utils import get_free_port, STATIC_PATH, strip_space
+from ..utils import get_free_port, STATIC_PATH, strip_space, parse_file_size
 
 logger = logging.getLogger(__name__)
 from .adaptor import ws as ws_adaptor
 
 
 class WebSocketConnection(ws_adaptor.WebSocketConnection):
 
@@ -144,14 +145,15 @@
                          reconnect_timeout=reconnect_timeout)
 
 
 def start_server(applications, port=0, host='', cdn=True, reconnect_timeout=0,
                  static_dir=None, remote_access=False, debug=False,
                  allowed_origins=None, check_origin=None,
                  auto_open_webbrowser=False,
+                 max_payload_size='200M',
                  **uvicorn_settings):
     """Start a FastAPI/Starlette server using uvicorn to provide the PyWebIO application as a web service.
 
     :param bool debug: Boolean indicating if debug tracebacks should be returned on errors.
     :param uvicorn_settings: Additional keyword arguments passed to ``uvicorn.run()``.
        For details, please refer: https://www.uvicorn.org/settings/
 
@@ -174,14 +176,18 @@
         port = get_free_port()
 
     print_listen_address(host, port)
 
     if remote_access:
         start_remote_access_service(local_port=port)
 
+    page.MAX_PAYLOAD_SIZE = max_payload_size = parse_file_size(max_payload_size)
+    uvicorn_settings = uvicorn_settings or {}
+    uvicorn_settings.setdefault('ws_max_size', max_payload_size)
+
     uvicorn.run(app, host=host, port=port, **uvicorn_settings)
 
 
 def asgi_app(applications, cdn=True, reconnect_timeout=0, static_dir=None, debug=False, allowed_origins=None,
              check_origin=None):
     """Get the starlette/Fastapi ASGI app for running PyWebIO applications.
```

### Comparing `pywebio-1.7.1/pywebio/platform/flask.py` & `pywebio-1.8.0/pywebio/platform/flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import werkzeug
 from flask import Flask, request, send_from_directory, Response
 
 from . import page
 from .adaptor.http import HttpContext, HttpHandler, run_event_loop
 from .page import make_applications
 from .remote_access import start_remote_access_service
-from .utils import cdn_validation
+from .utils import cdn_validation, print_listen_address
 from ..session import Session
 from ..utils import STATIC_PATH, iscoroutinefunction, isgeneratorfunction
 from ..utils import get_free_port, parse_file_size
 
 logger = logging.getLogger(__name__)
 
 
@@ -159,14 +159,16 @@
     if port == 0:
         port = get_free_port()
 
     app = wsgi_app(applications, cdn=cdn, static_dir=static_dir, allowed_origins=allowed_origins,
                    check_origin=check_origin, session_expire_seconds=session_expire_seconds,
                    session_cleanup_interval=session_cleanup_interval, max_payload_size=max_payload_size)
 
+    print_listen_address(host, port)
+
     debug = Session.debug = os.environ.get('PYWEBIO_DEBUG', debug)
     if not debug:
         logging.getLogger('werkzeug').setLevel(logging.WARNING)
 
     running_from_reloader = werkzeug.serving.is_running_from_reloader()
     if remote_access and not running_from_reloader:
         start_remote_access_service(local_port=port)
```

### Comparing `pywebio-1.7.1/pywebio/platform/page.py` & `pywebio-1.8.0/pywebio/platform/page.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import urllib.parse
 from collections import namedtuple
 from collections.abc import Mapping, Sequence
 from functools import lru_cache
 from functools import partial
 from os import path, environ
 
@@ -9,23 +10,23 @@
 
 from ..__version__ import __version__ as version
 from ..utils import isgeneratorfunction, iscoroutinefunction, get_function_name, get_function_doc, \
     get_function_attr, STATIC_PATH
 
 """
 The maximum size in bytes of a http request body or a websocket message, after which the request or websocket is aborted
-Set by `start_server()` or `path_deploy()` 
-Used in `file_upload()` as the `max_size`/`max_total_size` parameter default or to validate the parameter. 
+Set by `start_server()` or `path_deploy()`
+Used in `file_upload()` as the `max_size`/`max_total_size` parameter default or to validate the parameter.
 """
 MAX_PAYLOAD_SIZE = 0
 
 DEFAULT_CDN = "https://cdn.jsdelivr.net/gh/wang0618/PyWebIO-assets@v{version}/"
 
 _global_config = {'title': 'PyWebIO Application'}
-config_keys = ['title', 'description', 'js_file', 'js_code', 'css_style', 'css_file', 'theme']
+config_keys = ['title', 'description', 'js_file', 'js_code', 'css_style', 'css_file', 'theme', 'manifest']
 AppMeta = namedtuple('App', config_keys)
 
 _here_dir = path.dirname(path.abspath(__file__))
 _index_page_tpl = template.Template(open(path.join(_here_dir, 'tpl', 'index.html'), encoding='utf8').read())
 
 
 def render_page(app, protocol, cdn):
@@ -41,47 +42,52 @@
     if cdn is True:
         base_url = DEFAULT_CDN.format(version=version)
     elif not cdn:
         base_url = ''
     else:  # user custom cdn
         base_url = cdn.rstrip('/') + '/'
 
+    manifest = manifest_tag(base_url, meta)
+
     theme = environ.get('PYWEBIO_THEME', meta.theme) or 'default'
     check_theme(theme)
 
     return _index_page_tpl.generate(title=meta.title, description=meta.description, protocol=protocol,
                                     script=True, content='', base_url=base_url, version=version,
                                     js_file=meta.js_file or [], js_code=meta.js_code, css_style=meta.css_style,
-                                    css_file=meta.css_file or [], theme=theme)
+                                    css_file=meta.css_file or [], theme=theme, manifest=manifest)
 
 
 @lru_cache(maxsize=64)
 def check_theme(theme):
     """check theme file existence"""
     if not theme:
         return
 
     theme_file = path.join(STATIC_PATH, 'css', 'bs-theme', theme + '.min.css')
     if not path.isfile(theme_file):
         raise RuntimeError("Can't find css file for theme `%s`" % theme)
 
 
-def parse_app_metadata(func):
+def parse_app_metadata(func) -> AppMeta:
     """Get metadata form pywebio task function, fallback to global config in empty meta field."""
     prefix = '_pywebio_'
     attrs = get_function_attr(func, [prefix + k for k in config_keys])
     meta = AppMeta(**{k: attrs.get(prefix + k) for k in config_keys})
 
     doc = get_function_doc(func)
     parts = doc.strip().split('\n\n', 1)
     if len(parts) == 2:
         title, description = parts
     else:
         title, description = parts[0], ''
 
+    if not title:
+        title = get_function_name(func)
+
     if not meta.title:
         meta = meta._replace(title=title, description=description)
 
     # fallback to global config
     for key in config_keys:
         if not getattr(meta, key, None) and _global_config.get(key):
             kwarg = {key: _global_config.get(key)}
@@ -98,15 +104,15 @@
         {% if other_arguments is not None %}
             <a href="?app={{name}}{{other_arguments}}">{{ meta.title or name }}</a>:
         {% else %}
             <a href="javascript:WebIO.openApp('{{ name }}', true)">{{ meta.title or name }}</a>:
         {% end %}
 
         {% if meta.description %}
-            {{ meta.description }} 
+            {{ meta.description }}
         {% else %}
             <i>No description.</i>
         {% end %}
     </li>
     {% end %}
 </ul>
 """.strip())
@@ -218,15 +224,50 @@
 
     if app is not None:
         return config(title=title, description=description)(app)
 
     return config(title=title, description=description)
 
 
-def config(*, title=None, description=None, theme=None, js_code=None, js_file=[], css_style=None, css_file=[]):
+def manifest_tag(base_url, meta: AppMeta):
+    """Generate inline web app manifest
+    https://stackoverflow.com/questions/46221528/inline-the-web-app-manifest
+    """
+    if meta.manifest is False:
+        return ""
+
+    manifest_ = meta.manifest or {}
+    if manifest_ is True:
+        manifest_ = {}
+
+    manifest = {
+        "name": meta.title,
+        "description": meta.description,
+        "start_url": ".",
+        "display": "standalone",
+        "theme_color": "white",
+        "background_color": "white",
+        "icons": [
+            {"src": f"{base_url}image/apple-touch-icon.png", "type": "image/png", "sizes": "180x180"},
+        ]
+    }
+    manifest.update(manifest_)
+
+    icon = manifest.pop("icon", None)
+    if not icon:
+        icon = base_url + 'image/apple-touch-icon.png'
+
+    manifest_encode = urllib.parse.quote(json.dumps(manifest))
+    tag = f"""<link rel="apple-touch-icon" href="{icon}">
+    <link rel="manifest" href='data:application/manifest+json,{manifest_encode}' />"""
+    return tag
+
+
+def config(*, title=None, description=None, theme=None, js_code=None, js_file=[], css_style=None, css_file=[],
+           manifest=True):
     """PyWebIO application configuration
 
     :param str title: Application title
     :param str description: Application description
     :param str theme: Application theme. Available themes are: ``dark``, ``sketchy``, ``minty``, ``yeti``.
         You can also use environment variable ``PYWEBIO_THEME`` to specify the theme (with high priority).
 
@@ -237,14 +278,23 @@
             The dark theme is modified from ForEvolve's `bootstrap-dark <https://github.com/ForEvolve/bootstrap-dark>`_.
             The sketchy, minty and yeti theme are from `bootswatch <https://bootswatch.com/4/>`_.
 
     :param str js_code: The javascript code that you want to inject to page.
     :param str/list js_file: The javascript files that inject to page, can be a URL in str or a list of it.
     :param str css_style: The CSS style that you want to inject to page.
     :param str/list css_file: The CSS files that inject to page, can be a URL in str or a list of it.
+    :param bool/dict manifest: `Web application manifest <https://developer.mozilla.org/en-US/docs/Web/Manifest>`_ configuration.
+        This feature allows you to add a shortcut to the home screen of your mobile device, and launch the app like a native app.
+        If set to ``True``, the default manifest will be used. You can also specify the manifest content in dict.
+        If ``False``, the manifest will be disabled.
+
+        .. collapse:: Note for icon configuration
+
+            Currently, the `icons <https://developer.mozilla.org/en-US/docs/Web/Manifest/icons>`_ field of the manifest
+            is not supported. Instead, you can use the ``icon`` field to specify the icon url.
 
     ``config()`` can be used in 2 ways: direct call and decorator.
     If you call ``config()`` directly, the configuration will be global.
     If you use ``config()`` as decorator, the configuration will only work on single PyWebIO application function.
     ::
 
         config(title="My application")  # global configuration
```

### Comparing `pywebio-1.7.1/pywebio/platform/path_deploy.py` & `pywebio-1.8.0/pywebio/platform/path_deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     <meta name="description" content="PyWebIO applications index">
     <style>a{text-decoration:none;display:inline-block;min-width:{{ max_name_width }}ch}span{color:grey}</style>
 </head>
 <body>
 <h1>{{ title }}</h1>
 <hr>
 <pre style="line-height: 1.6em; font-size: 16px;">
-{% for name,doc in files %} <a href="{{ name }}">{{ name }}</a>  <span>{{ doc }}</span> 
+{% for name,doc in files %} <a href="{{ name }}">{{ name }}</a>  <span>{{ doc }}</span>
 {% end %}</pre>
 <hr>
 </body>
 </html>
 """.strip())
```

### Comparing `pywebio-1.7.1/pywebio/platform/remote_access.py` & `pywebio-1.8.0/pywebio/platform/remote_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 logger = logging.getLogger(__name__)
 
 success_msg = """
 ================================================================================
 PyWebIO Application Remote Access
 
-Remote access address: {address} 
+Remote access address: {address}
 ================================================================================
 """
 
 _ssh_process = None  # type: Popen
 
 
 def am_i_the_only_thread():
```

### Comparing `pywebio-1.7.1/pywebio/platform/tornado.py` & `pywebio-1.8.0/pywebio/platform/tornado.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import logging
 import os
 import threading
 import typing
 import webbrowser
 from functools import partial
+from typing import Callable, Dict, List, Optional, Union
 from urllib.parse import urlparse
 
 import tornado
 import tornado.httpserver
 import tornado.ioloop
 import tornado.web
 import tornado.websocket
@@ -202,21 +203,19 @@
 
     app = tornado.web.Application(handlers=handlers, **tornado_app_settings)
     # Credit: https://stackoverflow.com/questions/19074972/content-length-too-long-when-uploading-file-using-tornado
     server = app.listen(port, address=host, max_buffer_size=max_buffer_size)
     return server, port
 
 
-def start_server(applications, port=0, host='',
-                 debug=False, cdn=True, static_dir=None,
-                 remote_access=False,
-                 reconnect_timeout=0,
-                 allowed_origins=None, check_origin=None,
-                 auto_open_webbrowser=False,
-                 max_payload_size='200M',
+def start_server(applications: Union[Callable[[], None], List[Callable[[], None]], Dict[str, Callable[[], None]]],
+                 port: int = 0, host: str = '', debug: bool = False, cdn: Union[bool, str] = True,
+                 static_dir: Optional[str] = None, remote_access: bool = False, reconnect_timeout: int = 0,
+                 allowed_origins: Optional[List[str]] = None, check_origin: Callable[[str], bool] = None,
+                 auto_open_webbrowser: bool = False, max_payload_size: Union[int, str] = '200M',
                  **tornado_app_settings):
     """Start a Tornado server to provide the PyWebIO application as a web service.
 
     The Tornado server communicates with the browser by WebSocket protocol.
 
     Tornado is the default backend server for PyWebIO applications,
     and ``start_server`` can be imported directly using ``from pywebio import start_server``.
@@ -273,15 +272,16 @@
     """
     set_ioloop(tornado.ioloop.IOLoop.current())  # to enable bokeh app
 
     cdn = cdn_validation(cdn, 'warn')  # if CDN is not available, warn user and disable CDN
 
     page.MAX_PAYLOAD_SIZE = max_payload_size = parse_file_size(max_payload_size)
 
-    debug = Session.debug = os.environ.get('PYWEBIO_DEBUG', debug)
+    # covered `os.environ.get()` func with `bool()` to pervent type check error
+    debug = Session.debug = bool(os.environ.get('PYWEBIO_DEBUG', debug))
 
     # Since some cloud server may close idle connections (such as heroku),
     # use `websocket_ping_interval` to  keep the connection alive
     tornado_app_settings.setdefault('websocket_ping_interval', 30)
     tornado_app_settings.setdefault('websocket_max_message_size', max_payload_size)  # Backward compatible
     tornado_app_settings['websocket_max_message_size'] = parse_file_size(
         tornado_app_settings['websocket_max_message_size'])
@@ -310,15 +310,15 @@
     The PYWEBIO_SCRIPT_MODE_PORT environment variable can set the listening port, just used in testing.
     """
     websocket_conn_opened = threading.Event()
     thread = threading.current_thread()
 
     class SingleSessionWSHandler(_webio_handler(cdn=False)):
         session: ScriptModeSession = None
-        instance: typing.ClassVar = None  # type: SingleSessionWSHandler
+        instance: typing.ClassVar = None
         closed = False
 
         def send_msg_to_client(self, session):
             for msg in session.get_task_commands():
                 try:
                     self.write_message(json.dumps(msg))
                 except TypeError as e:
```

### Comparing `pywebio-1.7.1/pywebio/platform/tornado_http.py` & `pywebio-1.8.0/pywebio/platform/tornado_http.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/platform/tpl/index.html` & `pywebio-1.8.0/pywebio/platform/tpl/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
     <title>{{ title }}</title>
     <meta name="description" content="{{ description }}">
     <link rel="icon" type="image/png" sizes="32x32" href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAAwklEQVQ4T63TvU5CQRCG4WcwMfEuqOgNtQ2Nd4CxV2LHtVhJ0N7AHdjQUBtrrLwLA4ks2Rx+/Qucw3Y78807M7sz4ft5dq6mI7RQX7o/JCNzfdfetkNifRk6k9wLN9jYdxMkyZPQ1faZXYUwB/OCix8V/W4Y4zJDCsBAX7jdM7iQJY+udELu+cTrP2X/xU2+NMPAg3B3UPaVOOmFoQkapQC8Z8AUpyUBs6MAKrZQ+RErf2PlQTrKKK8gpZdpewgOXOcFTTxEjYwMoIkAAAAASUVORK5CYII=" id="favicon32">
     <link rel="icon" type="image/png" sizes="16x16" href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAABmUlEQVRYR82XK0wDQRCGv21TUUUJGBwGDBggGCSGBIcAWnBAgsNAgkKhSMDgCA8HtEXgSDBIDC9DDRgcpoSiKo52yea49DiutMttsz27M/98N7s7OyNo9tujgxSTwDiCIaAXSH27l4AXJA/AFSUuWOajGWnR0ChLP3HWkWSAZEN716CM4JQKW6R5+sunPkCeJJJNBCtAosnAQTMHyS6CDWYoh2mEAxzTR4JzYOCfgYNuBRymmOc5uPAbIMswMS6BbkPBPZkiVSZIc+/X/Qng/vl1C4LXIBzG/JmoAag9hxuDaa+XwAIw6p2JGkCObQSrhtMeLifZYZY1tegCqKsW4zHCadfldqgyqK6oC3DGIZIFXZVI9oIjplkUqArXyatGkYkU1+dc5p0eQY4MghNTqlo6kjkFsI9gScvRlLHkQJDnFhgxpampc6cAikCXpqMp8zcF8AnETSlq6lTaAsD6Flg+hNavofVCZL0UW3+M2uI5VhBWGxIFYL0lUxBWm1KviFttyz0Iq4OJB2F1NPO/qdaG0+DD3qLx/AuMVJFhmC8dSgAAAABJRU5ErkJggg==" id="favicon16">
+    {% raw manifest %}
     <link rel="stylesheet" href="{{ base_url }}css/markdown.min.css">
     <link rel="stylesheet" href="{{ base_url }}css/codemirror.min.css">
     <link rel="stylesheet" href="{{ base_url }}css/toastify.min.css">
     <link rel="stylesheet" href="{{ base_url }}css/bs-theme/{{ theme }}.min.css">
     <link rel="stylesheet" href="{{ base_url }}css/bootstrap-select.min.css">
     <link rel="stylesheet" href="{{ base_url }}css/app.css?v={{ version }}">
     {% for css in css_file %}
@@ -74,14 +75,16 @@
             window.location.href = url.href;
         }
     }
 
     require.config({
         paths: {
             'plotly': "https://cdn.plot.ly/plotly-2.12.1.min",
+            "ag-grid": "https://unpkg.com/ag-grid-community@28.2.0/dist/ag-grid-community.min",
+            "ag-grid-enterprise": "https://unpkg.com/ag-grid-enterprise@28.2.0/dist/ag-grid-enterprise.min",
         },
     });
 
 
     $(function () {
         // https://www.npmjs.com/package/bs-custom-file-input
         bsCustomFileInput.init()
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 
 
 
-
+ {% raw manifest %}
 
 
 
 
 
  {% for css in css_file %} {% if css %}
 {% end %} {% end %} {% if css_style %}
```

### Comparing `pywebio-1.7.1/pywebio/session/__init__.py` & `pywebio-1.8.0/pywebio/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.7.1/pywebio/session/base.py` & `pywebio-1.8.0/pywebio/session/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,28 +130,27 @@
         return self._closed
 
     def on_task_exception(self):
         from ..output import toast, popup, put_error, PopupSize
         from . import run_js
         from . import info as session_info
 
-        logger.exception('Error')
-
-        toast_msg = "应用发生内部错误" if 'zh' in session_info.user_language else "An internal error occurred in the application"
-
-        e_type, e_value, e_tb = sys.exc_info()
-        lines = traceback.format_exception(e_type, e_value, e_tb)
-        traceback_msg = ''.join(lines)
+        # log exception in server
+        logger.exception('Unhandled error in pywebio app')
 
         try:
+            toast_msg = "应用发生内部错误" if 'zh' in session_info.user_language else "An internal error occurred in the application"
             if type(self).debug:
+                e_type, e_value, e_tb = sys.exc_info()
+                lines = traceback.format_exception(e_type, e_value, e_tb)
+                traceback_msg = ''.join(lines)
                 popup(title=toast_msg, content=put_error(traceback_msg), size=PopupSize.LARGE)
+                run_js("console.error(traceback_msg)", traceback_msg='Internal Server Error\n' + traceback_msg)
             else:
                 toast(toast_msg, duration=1, color='error')
-                run_js("console.error(traceback_msg)", traceback_msg='Internal Server Error\n' + traceback_msg)
         except Exception:
             pass
 
     def register_callback(self, callback, **options):
         """ 向Session注册一个回调函数，返回回调id
 
         Session需要保证当收到前端发送的事件消息 ``{event: "callback"，task_id: 回调id, data:...}`` 时，
```

### Comparing `pywebio-1.7.1/pywebio/session/coroutinebased.py` & `pywebio-1.8.0/pywebio/session/coroutinebased.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,17 +149,22 @@
         msgs = self.unhandled_task_msgs
         self.unhandled_task_msgs = []
         return msgs
 
     def _cleanup(self):
         for t in list(self.coros.values()):  # t.close() may cause self.coros changed size
             t.step(SessionClosedException, throw_exp=True)
+            # in case that the task catch the SessionClosedException, we need to close it manually
             t.close()
         self.coros = {}  # delete session tasks
 
+        # reset the reference, to avoid circular reference
+        self._on_session_close = None
+        self._on_task_command = None
+
     def close(self, nonblock=False):
         """关闭当前Session。由Backend调用"""
         if self.closed():
             return
 
         super().close()
 
@@ -291,15 +296,14 @@
         """
         :param coro: 协程对象
         :param session: 创建该Task的会话实例
         :param on_coro_stop: 任务结束(正常结束或外部调用Task.close)时运行的回调
         """
         self.session = session
         self.coro = coro
-        self.coro_id = None
         self.result = None
         self.task_closed = False  # 任务完毕/取消
         self.on_coro_stop = on_coro_stop or (lambda _: None)
 
         self.coro_id = self.gen_coro_id(self.coro)
 
         self.pending_futures = {}  # id(future) -> future
@@ -318,50 +322,56 @@
                 if throw_exp:
                     coro_yield = self.coro.throw(result)
                 else:
                     coro_yield = self.coro.send(result)
             except StopIteration as e:
                 if len(e.args) == 1:
                     self.result = e.args[0]
-                self.task_closed = True
+                self.close()
                 logger.debug('Task[%s] finished', self.coro_id)
-                self.on_coro_stop(self)
             except Exception as e:
                 if not isinstance(e, SessionException):
                     self.session.on_task_exception()
-                self.task_closed = True
-                self.on_coro_stop(self)
+                self.close()
+
+        if coro_yield is None:
+            return
 
         future = None
         if isinstance(coro_yield, WebIOFuture):
             if coro_yield.coro:
                 future = asyncio.run_coroutine_threadsafe(coro_yield.coro, asyncio.get_event_loop())
-        elif coro_yield is not None:
+        else:
             future = coro_yield
+
         if not self.session.closed() and hasattr(future, 'add_done_callback'):
             future.add_done_callback(self._wakeup)
             self.pending_futures[id(future)] = future
 
     def _wakeup(self, future):
         if not future.cancelled():
             del self.pending_futures[id(future)]
             self.step(future.result())
 
     def close(self):
         if self.task_closed:
             return
 
-        logger.debug('Task[%s] closed', self.coro_id)
+        self.task_closed = True
+
         self.coro.close()
         while self.pending_futures:
             _, f = self.pending_futures.popitem()
             f.cancel()
 
-        self.task_closed = True
         self.on_coro_stop(self)
+        self.on_coro_stop = None  # avoid circular reference
+        self.session = None
+
+        logger.debug('Task[%s] closed', self.coro_id)
 
     def __del__(self):
         if not self.task_closed:
             logger.warning('Task[%s] was destroyed but it is pending!', self.coro_id)
 
     def task_handle(self):
         handle = TaskHandler(close=self.close, closed=lambda: self.task_closed)
```

### Comparing `pywebio-1.7.1/pywebio/session/threadbased.py` & `pywebio-1.8.0/pywebio/session/threadbased.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,18 @@
             return
         if self._loop:
             self._loop.call_soon_threadsafe(self._on_session_close)
         else:
             self._on_session_close()
 
     def _cleanup(self, nonblock=False):
+        # reset the reference, to avoid circular reference
+        self._on_session_close = None
+        self._on_task_command = None
+
         cls = type(self)
         if not nonblock:
             self.unhandled_task_msgs.wait_empty(8)
 
         if not self.unhandled_task_msgs.empty():
             msg = self.unhandled_task_msgs.get()
             logger.warning("%d unhandled task messages when session close. [%s]", len(msg), threading.current_thread())
```

### Comparing `pywebio-1.7.1/pywebio/utils.py` & `pywebio-1.8.0/pywebio/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 Error: Missing pywebio.js library for frontend page.
 This may be because you cloned or downloaded the project directly from the Git repository.
 
 You Can:
   * Manually build the pywebio.js file. See `webiojs/README.md` for more info.
 OR
   * Use the following command to install the latest development version of PyWebIO:
-    pip3 install -U https://code.aliyun.com/wang0618/pywebio/repository/archive.zip
+    pip3 install -U https://github.com/pywebio/PyWebIO/archive/dev-release.zip
 """.strip()
     raise RuntimeError(error_msg)
 
 
 def parse_file_size(size):
     """Transform file size to byte
```

### Comparing `pywebio-1.7.1/pywebio.egg-info/PKG-INFO` & `pywebio-1.8.0/pywebio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio
-Version: 1.7.1
+Version: 1.8.0
 Summary: Write interactive web app in script way.
 Home-page: https://pywebio.readthedocs.io
 Author: WangWeimin
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io
 Project-URL: Source, https://github.com/wang0618/PyWebIO
@@ -28,25 +28,19 @@
             <a href="https://pypi.org/project/PyWebIO/">
                 <img src="https://img.shields.io/pypi/v/pywebio?colorB=brightgreen" alt="Package version">
             </a>
             <a href="https://pypi.org/project/PyWebIO/">
                 <img src="https://img.shields.io/badge/python->%3D%203.5.2-brightgreen" alt="Python Version">
             </a>
             <br/>
-            <a href="https://lgtm.com/projects/g/wang0618/PyWebIO/context:python">
-                <img src="https://img.shields.io/lgtm/grade/python/github/wang0618/PyWebIO.svg?colorB=brightgreen" alt="Python code quality">
-            </a>
-            <a href="https://lgtm.com/projects/g/wang0618/PyWebIO/context:javascript">
-                <img src="https://img.shields.io/lgtm/grade/javascript/github/wang0618/PyWebIO.svg?colorB=brightgreen" alt="Javascript code quality">
-            </a>
             <a href="https://github.com/wang0618/PyWebIO/blob/master/LICENSE">
                 <img src="https://img.shields.io/github/license/wang0618/PyWebIO.svg" alt="License">
             </a>
             <br/>
-            <a href="https://pywebio.readthedocs.io">[Document]</a> | <a href="http://pywebio-demos.pywebio.online/">[Demos]</a> | <a href="https://github.com/wang0618/PyWebIO/wiki/Why-PyWebIO%3F">[Why PyWebIO?]</a>
+            <a href="https://pywebio.readthedocs.io">[Document]</a> | <a href="http://pywebio-demos.pywebio.online/">[Demos]</a> | <a href="https://play.pywebio.online">[Playground]</a> | <a href="https://github.com/wang0618/PyWebIO/wiki/Why-PyWebIO%3F">[Why PyWebIO?]</a>
         </p>
         
         [English](README.md) | [中文](README-zh.md)
         
         PyWebIO provides a series of imperative functions to obtain user input and output on the browser, turning the browser into a "rich text terminal", and can be used to build simple web applications or browser-based GUI applications without the need to have knowledge of HTML and JS. PyWebIO can also be easily integrated into existing Web services. PyWebIO is very suitable for quickly building applications that do not require complex UI.
         
         <p align="center">
@@ -70,15 +64,15 @@
         
         ```bash
         pip3 install -U pywebio
         ```
         
         Development version:
         ```bash
-        pip3 install -U https://code.aliyun.com/wang0618/pywebio/repository/archive.zip
+        pip3 install -U https://github.com/pywebio/PyWebIO/archive/dev-release.zip
         ```
         
         **Prerequisites**: PyWebIO requires Python 3.5.2 or newer
         
         ## Quickstart
         
         **Hello, world**
@@ -159,18 +153,18 @@
         For integration with other web frameworks, please refer to [document](https://pywebio.readthedocs.io/en/latest/advanced.html#integration-with-web-framework).
         
         ## Demos
         
          - [Basic demo](http://pywebio-demos.pywebio.online/) : PyWebIO basic input and output demos and some small applications written using PyWebIO.
          - [Data visualization demo](http://pywebio-charts.pywebio.online/) : Data visualization with the third-party libraries, e.g., `plotly`, `bokeh`, `pyecharts`.
         
-        ## Document
-        
-        Document is on [https://pywebio.readthedocs.io](https://pywebio.readthedocs.io)
+        ## Links
         
+        * Document [pywebio.readthedocs.io](https://pywebio.readthedocs.io)
+        * [PyWebIO Playground](https://play.pywebio.online/): Edit, Run, Share PyWebIO Code Online
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5.2
```

### Comparing `pywebio-1.7.1/pywebio.egg-info/SOURCES.txt` & `pywebio-1.8.0/pywebio.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 pywebio/io_ctrl.py
 pywebio/output.py
 pywebio/pin.py
 pywebio/utils.py
 pywebio.egg-info/PKG-INFO
 pywebio.egg-info/SOURCES.txt
 pywebio.egg-info/dependency_links.txt
+pywebio.egg-info/entry_points.txt
 pywebio.egg-info/requires.txt
 pywebio.egg-info/top_level.txt
 pywebio/html/codemirror/active-line.js
 pywebio/html/codemirror/addons.js
 pywebio/html/codemirror/autorefresh.js
 pywebio/html/codemirror/loadmode.js
 pywebio/html/codemirror/matchbrackets.js
@@ -40,14 +41,15 @@
 pywebio/html/css/markdown.min.css
 pywebio/html/css/toastify.min.css
 pywebio/html/css/bs-theme/dark.min.css
 pywebio/html/css/bs-theme/default.min.css
 pywebio/html/css/bs-theme/minty.min.css
 pywebio/html/css/bs-theme/sketchy.min.css
 pywebio/html/css/bs-theme/yeti.min.css
+pywebio/html/image/apple-touch-icon.png
 pywebio/html/image/favicon_closed_16.png
 pywebio/html/image/favicon_closed_32.png
 pywebio/html/image/favicon_open_16.png
 pywebio/html/image/favicon_open_32.png
 pywebio/html/js/FileSaver.min.js
 pywebio/html/js/bootstrap-select.min.js
 pywebio/html/js/bootstrap.min.js
@@ -72,13 +74,15 @@
 pywebio/platform/remote_access.py
 pywebio/platform/tornado.py
 pywebio/platform/tornado_http.py
 pywebio/platform/utils.py
 pywebio/platform/adaptor/__init__.py
 pywebio/platform/adaptor/http.py
 pywebio/platform/adaptor/ws.py
+pywebio/platform/pyinstaller/__init__.py
+pywebio/platform/pyinstaller/hook-pywebio.py
 pywebio/platform/tpl/index.html
 pywebio/session/__init__.py
 pywebio/session/base.py
 pywebio/session/coroutinebased.py
 pywebio/session/threadbased.py
 tools/pywebio-path-deploy
```

### Comparing `pywebio-1.7.1/tools/pywebio-path-deploy` & `pywebio-1.8.0/tools/pywebio-path-deploy`

 * *Files identical despite different names*

