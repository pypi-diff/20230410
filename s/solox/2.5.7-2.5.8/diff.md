# Comparing `tmp/solox-2.5.7.tar.gz` & `tmp/solox-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-9j9ffjn7/solox-2.5.7.tar", last modified: Tue Apr  4 11:50:47 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-17vxvja6/solox-2.5.8.tar", last modified: Mon Apr 10 09:54:58 2023, max compression
```

## Comparing `solox-2.5.7.tar` & `solox-2.5.8.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-04 11:50:36.000000 solox-2.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-04 11:50:36.000000 solox-2.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-04 11:50:47.000000 solox-2.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-04 11:50:36.000000 solox-2.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-04 11:50:47.000000 solox-2.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-04 11:50:36.000000 solox-2.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-04 11:50:36.000000 solox-2.5.7/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-04 11:50:36.000000 solox-2.5.7/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-04 11:50:36.000000 solox-2.5.7/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23233 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39139 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-04 11:50:36.000000 solox-2.5.7/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-04-04 11:50:36.000000 solox-2.5.7/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-04 11:50:36.000000 solox-2.5.7/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-04 11:50:36.000000 solox-2.5.7/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-04-04 11:50:36.000000 solox-2.5.7/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-04-04 11:50:36.000000 solox-2.5.7/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    35627 2023-04-04 11:50:36.000000 solox-2.5.7/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    86782 2023-04-04 11:50:36.000000 solox-2.5.7/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-04-04 11:50:36.000000 solox-2.5.7/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-04-04 11:50:36.000000 solox-2.5.7/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 11:50:36.000000 solox-2.5.7/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22224 2023-04-04 11:50:36.000000 solox-2.5.7/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-04 11:50:36.000000 solox-2.5.7/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-04 11:50:36.000000 solox-2.5.7/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:50:47.000000 solox-2.5.7/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-04 11:50:47.000000 solox-2.5.7/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-04 11:50:47.000000 solox-2.5.7/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 11:50:47.000000 solox-2.5.7/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 11:50:47.000000 solox-2.5.7/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 11:50:47.000000 solox-2.5.7/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-10 09:54:47.000000 solox-2.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-10 09:54:47.000000 solox-2.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-10 09:54:58.000000 solox-2.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-10 09:54:47.000000 solox-2.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-10 09:54:58.000000 solox-2.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-10 09:54:47.000000 solox-2.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 09:54:47.000000 solox-2.5.8/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-10 09:54:47.000000 solox-2.5.8/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-10 09:54:47.000000 solox-2.5.8/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16374 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23595 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39139 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    47094 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35648 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    88804 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 09:54:47.000000 solox-2.5.8/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-04-10 09:54:47.000000 solox-2.5.8/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-10 09:54:47.000000 solox-2.5.8/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-10 09:54:47.000000 solox-2.5.8/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/top_level.txt
```

### Comparing `solox-2.5.7/LICENSE` & `solox-2.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/PKG-INFO` & `solox-2.5.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.5.7
+Version: 2.5.8
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -36,82 +36,90 @@
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
 ## Installation
+
 ```shell
-1.Python:3.10+ (Python 3.6 3.7 3.8 3.9 Please download a version of solox lower than 2.5.4)
+1.Python:3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
 2.pip install -U solox 
 3.pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox (China)
 
-notice: If Windows users need to test ios, install and start Itunes
+Note: If Windows users need to test ios, install and start Itunes
 ```
 
 ## Startup SoloX
+
 ### default
+
 ```shell
 python -m solox
 ```
+
 ### customize
 
 ```shell
 python -m solox --host={ip} --port={port}
 ```
 
-## Collect in python 
+## Collect in python
+
 ```python
 from solox.public.apm import APM
 # solox version >= 2.1.2
 
-apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True)
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
+# noLog : False (Save test data to log file)
 
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
 fps = apm.collectFps() # HZ
 battery = apm.collectBattery() # level:% temperature:°C current:mA voltage:mV power:w
 gpu = apm.collectGpu() # % only supports ios
 ```
 
-## Collect in API 
+## Collect in API
+
 ### Start the service in the background
 
 ```
 # solox version >= 2.1.5
 
 macOS/Linux: nohup python3 -m solox &
 Windows: start /min python3 -m solox &
 ```
 
 ### Request apm data from api
+
 ```shell
 Android: http://{ip}:{port}/apm/collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu
 
-target in ['cpu','memory','network','fps','battery']
+target in ['cpu','memory','network','fps','battery','gpu']
 ```
 
 ## PK Model
+
 - 2-devices: test the same app on two different phones
 - 2-apps: test two different apps on two phones with the same configuration
 
 notice: only supports android
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%">
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
 
 - windows: PowerShell
-- macOS：iTerm2 (https://iterm2.com/) 
+- macOS：iTerm2 (https://iterm2.com/)
 
 ## Thanks
 
 - https://github.com/alibaba/taobao-iphone-device
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solox Version: 2.5.7 Summary: SoloX - Real-time
+Metadata-Version: 2.1 Name: solox Version: 2.5.8 Summary: SoloX - Real-time
 collection tool for Android/iOS performance data. Home-page: https://
 github.com/smart-test-ti/SoloX Author: Rafa Chen Author-email:
 rafacheninc@gamil.com License: MIT Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE
                                English | ä¸­æ
@@ -10,35 +10,35 @@
 
             [solox_preview] [https://img.shields.io/pypi/dm/solox]
 ## Preview SoloX - Real-time collection tool for Android/iOS performance data.
 We are committed to solving inefficient, cumbersome test execution, and our
 goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/153412/
 1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
 process=image%2Fresize%2Cw_1500%2Climit_0] ## Installation ```shell 1.Python:
-3.10+ (Python 3.6 3.7 3.8 3.9 Please download a version of solox lower than
-2.5.4) 2.pip install -U solox 3.pip install -i https://mirrors.ustc.edu.cn/
-pypi/web/simple -U solox (China) notice: If Windows users need to test ios,
-install and start Itunes ``` ## Startup SoloX ### default ```shell python -
-m solox ``` ### customize ```shell python -m solox --host={ip} --port={port}
-``` ## Collect in python ```python from solox.public.apm import APM # solox
-version >= 2.1.2 apm = APM
-(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
-surfaceview=True) # apm = APM(pkgName='com.bilibili.app.in', platform='iOS')
-only supports one device # surfaceviewï¼ False = gfxinfo (Developer - GPU
-rendering mode - adb shell dumpsys gfxinfo) cpu = apm.collectCpu() # % memory =
+3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
+2.pip install -U solox 3.pip install -i https://mirrors.ustc.edu.cn/pypi/web/
+simple -U solox (China) Note: If Windows users need to test ios, install and
+start Itunes ``` ## Startup SoloX ### default ```shell python -m solox ``` ###
+customize ```shell python -m solox --host={ip} --port={port} ``` ## Collect in
+python ```python from solox.public.apm import APM # solox version >= 2.1.2 apm
+= APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
+surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
+platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
+(Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
+(Save test data to log file) cpu = apm.collectCpu() # % memory =
 apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
 apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
 current:mA voltage:mV power:w gpu = apm.collectGpu() # % only supports ios ```
 ## Collect in API ### Start the service in the background ``` # solox version
 >= 2.1.5 macOS/Linux: nohup python3 -m solox & Windows: start /min python3 -
 m solox & ``` ### Request apm data from api ```shell Android: http://{ip}:
 {port}/apm/
 collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/
 collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu target in
-['cpu','memory','network','fps','battery'] ``` ## PK Model - 2-devices: test
-the same app on two different phones - 2-apps: test two different apps on two
-phones with the same configuration notice: only supports android [https://
+['cpu','memory','network','fps','battery','gpu'] ``` ## PK Model - 2-devices:
+test the same app on two different phones - 2-apps: test two different apps on
+two phones with the same configuration notice: only supports android [https://
 cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-
 0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0] ## Browser
 [Chrome] ## Terminal - windows: PowerShell - macOSï¼iTerm2 (https://
 iterm2.com/) ## Thanks - https://github.com/alibaba/taobao-iphone-device
```

### Comparing `solox-2.5.7/README.md` & `solox-2.5.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,82 +21,90 @@
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
 ## Installation
+
 ```shell
-1.Python:3.10+ (Python 3.6 3.7 3.8 3.9 Please download a version of solox lower than 2.5.4)
+1.Python:3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
 2.pip install -U solox 
 3.pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox (China)
 
-notice: If Windows users need to test ios, install and start Itunes
+Note: If Windows users need to test ios, install and start Itunes
 ```
 
 ## Startup SoloX
+
 ### default
+
 ```shell
 python -m solox
 ```
+
 ### customize
 
 ```shell
 python -m solox --host={ip} --port={port}
 ```
 
-## Collect in python 
+## Collect in python
+
 ```python
 from solox.public.apm import APM
 # solox version >= 2.1.2
 
-apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True)
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
+# noLog : False (Save test data to log file)
 
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
 fps = apm.collectFps() # HZ
 battery = apm.collectBattery() # level:% temperature:°C current:mA voltage:mV power:w
 gpu = apm.collectGpu() # % only supports ios
 ```
 
-## Collect in API 
+## Collect in API
+
 ### Start the service in the background
 
 ```
 # solox version >= 2.1.5
 
 macOS/Linux: nohup python3 -m solox &
 Windows: start /min python3 -m solox &
 ```
 
 ### Request apm data from api
+
 ```shell
 Android: http://{ip}:{port}/apm/collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu
 
-target in ['cpu','memory','network','fps','battery']
+target in ['cpu','memory','network','fps','battery','gpu']
 ```
 
 ## PK Model
+
 - 2-devices: test the same app on two different phones
 - 2-apps: test two different apps on two phones with the same configuration
 
 notice: only supports android
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%">
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
 
 - windows: PowerShell
-- macOS：iTerm2 (https://iterm2.com/) 
+- macOS：iTerm2 (https://iterm2.com/)
 
 ## Thanks
 
 - https://github.com/alibaba/taobao-iphone-device
-
```

#### html2text {}

```diff
@@ -3,35 +3,35 @@
 
             [solox_preview] [https://img.shields.io/pypi/dm/solox]
 ## Preview SoloX - Real-time collection tool for Android/iOS performance data.
 We are committed to solving inefficient, cumbersome test execution, and our
 goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/153412/
 1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
 process=image%2Fresize%2Cw_1500%2Climit_0] ## Installation ```shell 1.Python:
-3.10+ (Python 3.6 3.7 3.8 3.9 Please download a version of solox lower than
-2.5.4) 2.pip install -U solox 3.pip install -i https://mirrors.ustc.edu.cn/
-pypi/web/simple -U solox (China) notice: If Windows users need to test ios,
-install and start Itunes ``` ## Startup SoloX ### default ```shell python -
-m solox ``` ### customize ```shell python -m solox --host={ip} --port={port}
-``` ## Collect in python ```python from solox.public.apm import APM # solox
-version >= 2.1.2 apm = APM
-(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
-surfaceview=True) # apm = APM(pkgName='com.bilibili.app.in', platform='iOS')
-only supports one device # surfaceviewï¼ False = gfxinfo (Developer - GPU
-rendering mode - adb shell dumpsys gfxinfo) cpu = apm.collectCpu() # % memory =
+3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
+2.pip install -U solox 3.pip install -i https://mirrors.ustc.edu.cn/pypi/web/
+simple -U solox (China) Note: If Windows users need to test ios, install and
+start Itunes ``` ## Startup SoloX ### default ```shell python -m solox ``` ###
+customize ```shell python -m solox --host={ip} --port={port} ``` ## Collect in
+python ```python from solox.public.apm import APM # solox version >= 2.1.2 apm
+= APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
+surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
+platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
+(Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
+(Save test data to log file) cpu = apm.collectCpu() # % memory =
 apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
 apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
 current:mA voltage:mV power:w gpu = apm.collectGpu() # % only supports ios ```
 ## Collect in API ### Start the service in the background ``` # solox version
 >= 2.1.5 macOS/Linux: nohup python3 -m solox & Windows: start /min python3 -
 m solox & ``` ### Request apm data from api ```shell Android: http://{ip}:
 {port}/apm/
 collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/
 collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu target in
-['cpu','memory','network','fps','battery'] ``` ## PK Model - 2-devices: test
-the same app on two different phones - 2-apps: test two different apps on two
-phones with the same configuration notice: only supports android [https://
+['cpu','memory','network','fps','battery','gpu'] ``` ## PK Model - 2-devices:
+test the same app on two different phones - 2-apps: test two different apps on
+two phones with the same configuration notice: only supports android [https://
 cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-
 0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0] ## Browser
 [Chrome] ## Terminal - windows: PowerShell - macOSï¼iTerm2 (https://
 iterm2.com/) ## Thanks - https://github.com/alibaba/taobao-iphone-device
```

### Comparing `solox-2.5.7/setup.py` & `solox-2.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/debug.py` & `solox-2.5.8/solox/debug.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/_iosPerf.py` & `solox-2.5.8/solox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/adb/mac/adb` & `solox-2.5.8/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/adb.py` & `solox-2.5.8/solox/public/adb.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/apm.py` & `solox-2.5.8/solox/public/apm.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 class Target:
     CPU = 'cpu'
     Memory = 'memory'
     Battery = 'battery'
     Network = 'network'
     FPS = 'fps'
+    GPU = 'gpu'
 
 class CPU(object):
 
     def __init__(self, pkgName, deviceId, platform='Android'):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
@@ -94,17 +95,17 @@
         sysCpuRate = round(float(apm.getPerformance(apm.cpu)[1]), 2)
         if sueApi is False:
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'cpu_app.log'), apm_time, appCpuRate)
             f.add_log(os.path.join(f.report_dir,'cpu_sys.log'), apm_time, sysCpuRate)
         return appCpuRate, sysCpuRate
 
-    def getCpuRate(self, useApi=False):
+    def getCpuRate(self, noLog=False):
         """Get the cpu rate of a process, unit:%"""
-        appCpuRate, systemCpuRate = self.getAndroidCpuRate(useApi) if self.platform == Platform.Android else self.getiOSCpuRate(useApi)
+        appCpuRate, systemCpuRate = self.getAndroidCpuRate(noLog) if self.platform == Platform.Android else self.getiOSCpuRate(noLog)
         return appCpuRate, systemCpuRate
 
 
 class MEM(object):
     def __init__(self, pkgName, deviceId, platform=Platform.Android):
         self.pkgName = pkgName
         self.deviceId = deviceId
@@ -127,66 +128,66 @@
         """Get the iOS memory"""
         apm = iosAPM(self.pkgName)
         totalPass = round(float(apm.getPerformance(apm.memory)), 2)
         nativePass = 0
         dalvikPass = 0
         return totalPass, nativePass, dalvikPass
 
-    def getProcessMem(self, useApi=False):
+    def getProcessMem(self, noLog=False):
         """Get the app memory"""
         totalPass, nativePass, dalvikPass = self.getAndroidMem() if self.platform == Platform.Android else self.getiOSMem()
-        if useApi is False:    
+        if noLog is False:    
             time.sleep(1)    
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'mem_total.log'), apm_time, totalPass)
             if self.platform == Platform.Android:
                 f.add_log(os.path.join(f.report_dir,'mem_native.log'), apm_time, nativePass)
                 f.add_log(os.path.join(f.report_dir,'mem_dalvik.log'), apm_time, dalvikPass)
         return totalPass, nativePass, dalvikPass
 
 
 class Battery(object):
     def __init__(self, deviceId, platform=Platform.Android):
         self.deviceId = deviceId
         self.platform = platform
     
-    def getBattery(self, useApi=False):
+    def getBattery(self, noLog=False):
         if self.platform == Platform.Android:
-            level, temperature = self.getAndroidBattery(useApi)
+            level, temperature = self.getAndroidBattery(noLog)
             return level, temperature
         else:
-            temperature, current, voltage, power = self.getiOSBattery(useApi)
+            temperature, current, voltage, power = self.getiOSBattery(noLog)
             return temperature, current, voltage, power
         
-    def getAndroidBattery(self, useApi=False):
+    def getAndroidBattery(self, noLog=False):
         """Get android battery info, unit:%"""
         # Switch mobile phone battery to non-charging state
         cmd = 'dumpsys battery set status 1'
         adb.shell(cmd=cmd, deviceId=self.deviceId)
         # Get phone battery info
         cmd = 'dumpsys battery'
         output = adb.shell(cmd=cmd, deviceId=self.deviceId)
         level = int(re.findall(u'level:\s?(\d+)', output)[0])
         temperature = int(re.findall(u'temperature:\s?(\d+)', output)[0]) / 10
-        if useApi is False:
+        if noLog is False:
              time.sleep(1)
              apm_time = datetime.datetime.now().strftime('%H:%M:%S')
              f.add_log(os.path.join(f.report_dir,'battery_level.log'), apm_time, level)
              f.add_log(os.path.join(f.report_dir,'battery_tem.log'), apm_time, temperature)
         return level, temperature
     
-    def getiOSBattery(self, useApi=False):
+    def getiOSBattery(self, noLog=False):
         """Get ios battery info, unit:%"""
         d  = tidevice.Device()
         ioDict =  d.get_io_power()
         tem = m._setValue(ioDict['Diagnostics']['IORegistry']['Temperature'])
         current = m._setValue(abs(ioDict['Diagnostics']['IORegistry']['InstantAmperage']))
         voltage = m._setValue(ioDict['Diagnostics']['IORegistry']['Voltage'])
         power = current * voltage / 1000
-        if useApi is False:
+        if noLog is False:
             time.sleep(1)
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'battery_tem.log'), apm_time, tem) # unknown
             f.add_log(os.path.join(f.report_dir,'battery_current.log'), apm_time, current) #mA
             f.add_log(os.path.join(f.report_dir,'battery_voltage.log'), apm_time, voltage) #mV
             f.add_log(os.path.join(f.report_dir,'battery_power.log'), apm_time, power)
         return tem, current, voltage, power
@@ -237,18 +238,18 @@
         """Get iOS upflow and downflow data"""
         apm = iosAPM(self.pkgName)
         apm_data = apm.getPerformance(apm.network)
         sendNum = round(float(apm_data[1]), 2)
         recNum = round(float(apm_data[0]), 2)
         return sendNum, recNum
 
-    def getNetWorkData(self, wifi=True, useApi=False):
+    def getNetWorkData(self, wifi=True, noLog=False):
         """Get the upflow and downflow data, unit:KB"""
         sendNum, recNum = self.getAndroidNet(wifi) if self.platform == Platform.Android else self.getiOSNet()
-        if useApi is False:
+        if noLog is False:
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'upflow.log'), apm_time, sendNum)
             f.add_log(os.path.join(f.report_dir,'downflow.log'), apm_time, recNum)
         return sendNum, recNum
 
 
 class FPS(object):
@@ -256,48 +257,48 @@
     def __init__(self, pkgName, deviceId, platform=Platform.Android, surfaceview=True):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
         self.surfaceview = surfaceview
         self.apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
 
-    def getAndroidFps(self, useApi=False):
+    def getAndroidFps(self, noLog=False):
         """get Android Fps, unit:HZ"""
         monitors = FPSMonitor(device_id=self.deviceId, package_name=self.pkgName, frequency=1,
                               surfaceview=self.surfaceview, start_time=TimeUtils.getCurrentTimeUnderline())
         monitors.start()
         fps, jank = monitors.stop()
-        if useApi is False:
+        if noLog is False:
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'fps.log'), apm_time, fps)
             f.add_log(os.path.join(f.report_dir,'jank.log'), apm_time, jank)
         return fps, jank
 
-    def getiOSFps(self, useApi=False):
+    def getiOSFps(self, noLog=False):
         """get iOS Fps"""
         apm = iosAPM(self.pkgName)
         fps = int(apm.getPerformance(apm.fps))
-        if useApi is False:
+        if noLog is False:
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'fps.log'), apm_time, fps)
         return fps, 0
 
-    def getFPS(self, useApi=False):
+    def getFPS(self, noLog=False):
         """get fps、jank"""
-        fps, jank = self.getAndroidFps(useApi) if self.platform == Platform.Android else self.getiOSFps(useApi)
+        fps, jank = self.getAndroidFps(noLog) if self.platform == Platform.Android else self.getiOSFps(noLog)
         return fps, jank
 
 class GPU(object):
     def __init__(self, pkgName):
         self.pkgName = pkgName
 
-    def getGPU(self, useApi=False):
+    def getGPU(self, noLog=False):
         apm = iosAPM(self.pkgName)
         gpu = apm.getPerformance(apm.gpu)
-        if useApi is False:
+        if noLog is False:
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'gpu.log'), apm_time, gpu)
         return gpu   
 
 class iosAPM(object):
 
     def __init__(self, pkgName, deviceId=tidevice.Device()):
@@ -334,60 +335,61 @@
             perf_value = perf.start(self.pkgName, callback=self.callback)
         return perf_value
 
 
 class APM(object):
     """for python api"""
 
-    def __init__(self, pkgName, deviceId='', platform=Platform.Android, surfaceview=True):
+    def __init__(self, pkgName, deviceId='', platform=Platform.Android, surfaceview=True, noLog=True):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
         self.surfaceview = surfaceview
+        self.noLog = noLog
         d.devicesCheck(platform=self.platform, deviceid=self.deviceId, pkgname=self.pkgName)
 
     def collectCpu(self):
         _cpu = CPU(self.pkgName, self.deviceId, self.platform)
-        appCpuRate, systemCpuRate = _cpu.getCpuRate(useApi=True)
+        appCpuRate, systemCpuRate = _cpu.getCpuRate(noLog=self.noLog)
         result = {'appCpuRate': appCpuRate, 'systemCpuRate': systemCpuRate}
         logger.info(f'cpu: {result}')
         return result
 
     def collectMemory(self):
         _memory = MEM(self.pkgName, self.deviceId, self.platform)
-        totalPass, nativePass, dalvikPass = _memory.getProcessMem(useApi=True)
+        totalPass, nativePass, dalvikPass = _memory.getProcessMem(noLog=self.noLog)
         result = {'totalPass': totalPass, 'nativePass': nativePass, 'dalvikPass': dalvikPass}
         logger.info(f'memory: {result}')
         return result
 
     def collectBattery(self):
         _battery = Battery(self.deviceId, self.platform)
-        final = _battery.getBattery(useApi=True)
+        final = _battery.getBattery(noLog=self.noLog)
         if self.platform == Platform.Android:
             result = {'level': final[0], 'temperature': final[1]}
         else:
             result = {'temperature': final[0], 'current': final[1], 'voltage': final[2], 'power': final[3]}
         logger.info(f'battery: {result}')
         return result
 
     def collectFlow(self, wifi=True):
         _flow = Flow(self.pkgName, self.deviceId, self.platform)
-        upFlow, downFlow = _flow.getNetWorkData(wifi=wifi,useApi=True)
+        upFlow, downFlow = _flow.getNetWorkData(wifi=wifi,noLog=self.noLog)
         result = {'upFlow': upFlow, 'downFlow': downFlow}
         logger.info(f'network: {result}')
         return result
 
     def collectFps(self):
         _fps = FPS(self.pkgName, self.deviceId, self.platform, self.surfaceview)
-        fps, jank = _fps.getFPS(useApi=True)
+        fps, jank = _fps.getFPS(noLog=self.noLog)
         result = {'fps': fps, 'jank': jank}
         logger.info(f'fps: {result}')
         return result
     
     def collectGpu(self):
         _gpu = GPU(self.pkgName)
         if self.platform == Platform.Android:
             raise Exception('not support android')
-        gpu = _gpu.getGPU(useApi=True)
+        gpu = _gpu.getGPU(noLog=self.noLog)
         result = {'gpu': gpu}
         logger.info(f'gpu: {result}')
         return result
```

### Comparing `solox-2.5.7/solox/public/apm_pk.py` & `solox-2.5.8/solox/public/apm_pk.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,24 +149,24 @@
         f.add_log(f'{f.report_dir}/network1.log', apm_time, network1)
         f.add_log(f'{f.report_dir}/network2.log', apm_time, network2)
         return network1, network2
 
 
 class FPS_PK:
 
-    def __init__(self, pkgNameList: list, deviceId1, deviceId2, surfaceview='true'):
+    def __init__(self, pkgNameList: list, deviceId1, deviceId2, surfaceview=True):
         self.pkgNameList = pkgNameList
         self.deviceId1 = deviceId1
         self.deviceId2 = deviceId2
         self.surfaceview = surfaceview
 
     def getAndroidFps(self, deviceId, pkgName):
         """get Android Fps, unit:HZ"""
         monitors = FPSMonitor(device_id=deviceId, package_name=pkgName, frequency=1,
-                              start_time=TimeUtils.getCurrentTimeUnderline(), surfaceview=self.surfaceview)
+                              surfaceview=self.surfaceview, start_time=TimeUtils.getCurrentTimeUnderline())
         monitors.start()
         fps, jank = monitors.stop()
         return fps
 
 
     def getFPS(self):
         """get fps"""
```

### Comparing `solox-2.5.7/solox/public/common.py` & `solox-2.5.8/solox/public/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         self.report_dir = self.get_repordir()
     
     def export_excel(self, platform, scene):
         
         android_log_file_list = ['cpu_app','cpu_sys','mem_total','mem_native','mem_dalvik',
                                  'battery_level', 'battery_tem','upflow','downflow','fps']
         ios_log_file_list = ['cpu_app','cpu_sys', 'mem_total', 'battery_tem', 'battery_current', 
-                             'battery_voltage', 'battery_power','upflow','downflow','fps']
+                             'battery_voltage', 'battery_power','upflow','downflow','fps','gpu']
         log_file_list = android_log_file_list if platform == 'Android' else ios_log_file_list
         wb = xlwt.Workbook(encoding = 'utf-8')
        
         k = 1
         for name in log_file_list:
             ws1 = wb.add_sheet(name)
             ws1.write(0,0,'Time') 
@@ -275,14 +275,20 @@
     def getCpuLog(self, platform, scene):
         targetDic = {}
         targetDic['cpuAppData'] = self.readLog(scene=scene, filename='cpu_app.log')[0]
         targetDic['cpuSysData'] = self.readLog(scene=scene, filename='cpu_sys.log')[0]
         result = {'status': 1, 'cpuAppData': targetDic['cpuAppData'], 'cpuSysData': targetDic['cpuSysData']}
         return result
     
+    def getGpuLog(self, platform, scene):
+        targetDic = {}
+        targetDic['gpu'] = self.readLog(scene=scene, filename='gpu.log')[0]
+        result = {'status': 1, 'gpu': targetDic['gpu']}
+        return result
+    
     def getMemLog(self, platform, scene):
         targetDic = {}
         targetDic['memTotalData'] = self.readLog(scene=scene, filename='mem_total.log')[0]
         if platform == Platform.Android:
             targetDic['memNativeData']  = self.readLog(scene=scene, filename='mem_native.log')[0]
             targetDic['memDalvikData']  = self.readLog(scene=scene, filename='mem_dalvik.log')[0]
             result = {'status': 1, 
@@ -404,81 +410,85 @@
         apm_dict['batteryLevel'] = batteryLevel
         apm_dict['batteryTeml'] = batteryTeml
         
         return apm_dict
 
     def _setiOSPerfs(self, scene):
         """Aggregate APM data for iOS"""
-        cpuAppData = self.readLog(scene=scene, filename=f'cpu_app.log')[1]
+        cpuAppData = self.readLog(scene=scene, filename='cpu_app.log')[1]
         cpuAppRate = f'{round(sum(cpuAppData) / len(cpuAppData), 2)}%'
 
-        cpuSystemData = self.readLog(scene=scene, filename=f'cpu_sys.log')[1]
+        cpuSystemData = self.readLog(scene=scene, filename='cpu_sys.log')[1]
         cpuSystemRate = f'{round(sum(cpuSystemData) / len(cpuSystemData), 2)}%'
 
-        totalPassData = self.readLog(scene=scene, filename=f'mem_total.log')[1]
+        totalPassData = self.readLog(scene=scene, filename='mem_total.log')[1]
         totalPassAvg = f'{round(sum(totalPassData) / len(totalPassData), 2)}MB'
 
-        fpsData = self.readLog(scene=scene, filename=f'fps.log')[1]
+        fpsData = self.readLog(scene=scene, filename='fps.log')[1]
         fpsAvg = f'{int(sum(fpsData) / len(fpsData))}HZ/s'
 
-        flowSendData = self.readLog(scene=scene, filename=f'upflow.log')[1]
+        flowSendData = self.readLog(scene=scene, filename='upflow.log')[1]
         flowSend = f'{round(float(sum(flowSendData) / 1024), 2)}MB'
 
-        flowRecvData = self.readLog(scene=scene, filename=f'downflow.log')[1]
+        flowRecvData = self.readLog(scene=scene, filename='downflow.log')[1]
         flowRecv = f'{round(float(sum(flowRecvData) / 1024), 2)}MB'
 
-        batteryTemlData = self.readLog(scene=scene, filename=f'battery_tem.log')[1]
+        batteryTemlData = self.readLog(scene=scene, filename='battery_tem.log')[1]
         batteryTeml = round(sum(batteryTemlData) / len(batteryTemlData), 2)
 
-        batteryCurrentData = self.readLog(scene=scene, filename=f'battery_current.log')[1]
+        batteryCurrentData = self.readLog(scene=scene, filename='battery_current.log')[1]
         batteryCurrent = round(sum(batteryCurrentData) / len(batteryCurrentData), 2)
 
-        batteryVoltageData = self.readLog(scene=scene, filename=f'battery_voltage.log')[1]
+        batteryVoltageData = self.readLog(scene=scene, filename='battery_voltage.log')[1]
         batteryVoltage = round(sum(batteryVoltageData) / len(batteryVoltageData), 2)
 
-        batteryPowerData = self.readLog(scene=scene, filename=f'battery_power.log')[1]
+        batteryPowerData = self.readLog(scene=scene, filename='battery_power.log')[1]
         batteryPower = round(sum(batteryPowerData) / len(batteryPowerData), 2)
 
+        gpuData = self.readLog(scene=scene, filename='gpu.log')[1]
+        gpu = round(sum(gpuData) / len(gpuData), 2)
+
         apm_dict = {}
         apm_dict['cpuAppRate'] = cpuAppRate
         apm_dict['cpuSystemRate'] = cpuSystemRate
         apm_dict['totalPassAvg'] = totalPassAvg
         apm_dict['nativePassAvg'] = 0
         apm_dict['dalvikPassAvg'] = 0
         apm_dict['fps'] = fpsAvg
         apm_dict['jank'] = 0
         apm_dict['flow_send'] = flowSend
         apm_dict['flow_recv'] = flowRecv
         apm_dict['batteryTeml'] = batteryTeml
         apm_dict['batteryCurrent'] = batteryCurrent
         apm_dict['batteryVoltage'] = batteryVoltage
         apm_dict['batteryPower'] = batteryPower
+        apm_dict['gpu'] = gpu
         
         return apm_dict
 
     def _setpkPerfs(self, scene):
         """Aggregate APM data for pk model"""
-        cpuAppData1 = self.readLog(scene=scene, filename=f'cpu_app1.log')[1]
+        cpuAppData1 = self.readLog(scene=scene, filename='cpu_app1.log')[1]
         cpuAppRate1 = f'{round(sum(cpuAppData1) / len(cpuAppData1), 2)}%'
-        cpuAppData2 = self.readLog(scene=scene, filename=f'cpu_app2.log')[1]
+        cpuAppData2 = self.readLog(scene=scene, filename='cpu_app2.log')[1]
         cpuAppRate2 = f'{round(sum(cpuAppData2) / len(cpuAppData2), 2)}%'
 
-        totalPassData1 = self.readLog(scene=scene, filename=f'mem1.log')[1]
+        totalPassData1 = self.readLog(scene=scene, filename='mem1.log')[1]
         totalPassAvg1 = f'{round(sum(totalPassData1) / len(totalPassData1), 2)}MB'
-        totalPassData2 = self.readLog(scene=scene, filename=f'mem2.log')[1]
+        totalPassData2 = self.readLog(scene=scene, filename='mem2.log')[1]
         totalPassAvg2 = f'{round(sum(totalPassData2) / len(totalPassData2), 2)}MB'
 
-        fpsData1 = self.readLog(scene=scene, filename=f'fps1.log')[1]
+        fpsData1 = self.readLog(scene=scene, filename='fps1.log')[1]
         fpsAvg1 = f'{int(sum(fpsData1) / len(fpsData1))}HZ/s'
-        fpsData2 = self.readLog(scene=scene, filename=f'fps2.log')[1]
+        fpsData2 = self.readLog(scene=scene, filename='fps2.log')[1]
         fpsAvg2 = f'{int(sum(fpsData2) / len(fpsData2))}HZ/s'
 
-        networkData1 = self.readLog(scene=scene, filename=f'network1.log')[1]
+        networkData1 = self.readLog(scene=scene, filename='network1.log')[1]
         network1 = f'{round(float(sum(networkData1) / 1024), 2)}MB'
-        networkData2 = self.readLog(scene=scene, filename=f'network2.log')[1]
+        networkData2 = self.readLog(scene=scene, filename='network2.log')[1]
         network2 = f'{round(float(sum(networkData2) / 1024), 2)}MB'
         
         apm_dict = {}
         apm_dict['cpuAppRate1'] = cpuAppRate1
         apm_dict['cpuAppRate2'] = cpuAppRate2
         apm_dict['totalPassAvg1'] = totalPassAvg1
         apm_dict['totalPassAvg2'] = totalPassAvg2
```

### Comparing `solox-2.5.7/solox/public/fps.py` & `solox-2.5.8/solox/public/fps.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/__main__.py` & `solox-2.5.8/solox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_crash.py` & `solox-2.5.8/solox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_device.py` & `solox-2.5.8/solox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_hexdump.py` & `solox-2.5.8/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_imagemounter.py` & `solox-2.5.8/solox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_installation.py` & `solox-2.5.8/solox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_instruments.py` & `solox-2.5.8/solox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_ipautil.py` & `solox-2.5.8/solox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_perf.py` & `solox-2.5.8/solox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_proto.py` & `solox-2.5.8/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_relay.py` & `solox-2.5.8/solox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_safe_socket.py` & `solox-2.5.8/solox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_ssl.py` & `solox-2.5.8/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_sync.py` & `solox-2.5.8/solox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_types.py` & `solox-2.5.8/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_usbmux.py` & `solox-2.5.8/solox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_utils.py` & `solox-2.5.8/solox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/_wdaproxy.py` & `solox-2.5.8/solox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/bplist.py` & `solox-2.5.8/solox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/exceptions.py` & `solox-2.5.8/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/plistlib2.py` & `solox-2.5.8/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/requests_usbmux.py` & `solox-2.5.8/solox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/public/iosperf/struct2.py` & `solox-2.5.8/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/css/highlight.min.css` & `solox-2.5.8/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.5.8/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.5.8/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/css/select2.min.css` & `solox-2.5.8/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/css/sweetalert2.min.css` & `solox-2.5.8/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/css/tabler.demo.min.css` & `solox-2.5.8/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/css/tabler.min.css` & `solox-2.5.8/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/image/404.png` & `solox-2.5.8/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/image/500.png` & `solox-2.5.8/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/image/avatar.png` & `solox-2.5.8/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/image/coffee.png` & `solox-2.5.8/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/image/empty.png` & `solox-2.5.8/solox/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/image/readme/home.png` & `solox-2.5.8/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/image/readme/pk.png` & `solox-2.5.8/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/apexcharts.js` & `solox-2.5.8/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/gray.js` & `solox-2.5.8/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/highlight.min.js` & `solox-2.5.8/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/highstock.js` & `solox-2.5.8/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/html2canvas.min.js` & `solox-2.5.8/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/jquery.min.js` & `solox-2.5.8/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/select2.min.js` & `solox-2.5.8/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/socket.io.js` & `solox-2.5.8/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/sweetalert2.min.js` & `solox-2.5.8/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/tabler.demo.min.js` & `solox-2.5.8/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/js/tabler.min.js` & `solox-2.5.8/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/static/logo/logo.png` & `solox-2.5.8/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/templates/404.html` & `solox-2.5.8/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/templates/500.html` & `solox-2.5.8/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/templates/analysis.html` & `solox-2.5.8/solox/templates/analysis.html`

 * *Files 2% similar despite different names*

```diff
@@ -364,14 +364,37 @@
                                 All：{{ apm_data.flow_recv }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
+        {% if platform == 'iOS' %}
+        <div class="col-sm-6 col-lg-2">
+            <div class="card card-sm">
+                <div class="card-body">
+                    <div class="row align-items-center">
+                        <div class="col-auto">
+                            <span class="bg-purple text-white avatar">
+                                GPU
+                            </span>
+                        </div>
+                        <div class="col">
+                            <div class="font-weight-medium">
+                                GPU
+                            </div>
+                            <div class="text-muted">
+                                Avg: {{ apm_data.gpu }}
+                            </div>
+                        </div>
+                    </div>
+                </div>
+            </div>
+        </div>
+        {% endif %}
     </div>
 </div>
 <div class="col-12">
     <div class="card cpu-card">
         <div class="card-header">
             <div class='card-title'>CPU（%）</div>
             <div class="card-actions btn-actions">
@@ -465,28 +488,49 @@
                 </a>
             </div>
         </div>
         <div class="card-body">
             <div id="chart-networkdata"></div>
         </div>
     </div>
+    {% if platform == 'iOS' %}
+    <div class="card gpu-card mt-3">
+        <div class="card-header">
+            <div class='card-title'>GPU（%）</div>
+            <div class="card-actions btn-actions">
+                <a class="btn-action cursor-pointer" id="gpu_loading">
+                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
+                </a>
+                <a class="btn-action cursor-pointer" id="gpu_png" onclick="screenshot('gpu-card','gpu.png')">
+                    <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
+                </a>
+            </div>
+        </div>
+        <div class="card-body">
+            <div id="chart-gpu"></div>
+        </div>
+    </div>
+    {% endif %}
 
 </div>
 {% endblock %}
 
 {% block js %}
 <script>
 
     $(document).ready(function() {
         $('#cpu_loading').click();
         $('#mem_loading').click();
         $('#fps_loading').click();
         if(platform == 'Android'){
             $('#jank_loading').click();
         }
+        if(platform == 'iOS'){
+            $('#gpu_loading').click();
+        }
         $('#battery_loading').click();
         $('#networkdata_loading').click();
     });
 
     function options(type,dataLabels=false) {
         let options = {
             chart: {
@@ -628,14 +672,44 @@
                         data: data['jank']
                     }])
                 }
             });
         });
     }
 
+    if(platform == 'iOS'){
+        var gpu_chart = new ApexCharts(document.querySelector("#chart-gpu"), options('line'));
+        gpu_chart.render();
+        $('#gpu_loading').click(function () {
+            $.ajax({
+                url: '/apm/log',
+                type: "GET",
+                async: true,
+                cache: false,
+                data:{
+                    scene:'{{ scene }}',
+                    target:'gpu',
+                    platform:platform
+                },
+                beforeSend: function () {
+                    SwalLoading('Loading','')
+                },
+                complete: function () {
+                    swal.close();
+                },
+                success: function (data) {
+                    gpu_chart.updateSeries([{
+                        name: 'gpu',
+                        data: data['gpu']
+                    }])
+                }
+            });
+        });
+    }
+
     var fps_chart = new ApexCharts(document.querySelector("#chart-fps"), options('line'));
     fps_chart.render();
     $('#fps_loading').click(function () {
         $.ajax({
             url: '/apm/log',
             type: "GET",
             async: true,
```

### Comparing `solox-2.5.7/solox/templates/analysis_pk.html` & `solox-2.5.8/solox/templates/analysis_pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/templates/base.html` & `solox-2.5.8/solox/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -40,29 +40,28 @@
                 <label style="margin-left: 10px;font-weight: bolder;font-style: normal;font-size: 20px;">SoloX</label>
             </h1>
             <div class="collapse navbar-collapse" id="navbar-menu" style="margin-left: 20px;">
                 <div class="d-flex flex-column flex-md-row flex-fill align-items-stretch align-items-md-center">
                     {% block navbar_nav %}{% endblock %}
                 </div>
             </div>
-            {% if platform %}
+            {% if model in ['2-app','2-devices'] %}
             <div class="nav-item dropdown d-none d-md-flex me-3">
-                <a href="/pk?model=2-devices&lan={{ lan }}" class="btn  btn-pill w-100" >
-                    <svg t="1661854041585" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="10784" width="2000" height="2000"><path d="M17.408 862.208a450.56 129.024 0 1 0 901.12 0 450.56 129.024 0 1 0-901.12 0Z" fill="#EEF2FF" p-id="10785"></path><path d="M509.952 880.64H75.776c-17.408 0-30.72-13.312-30.72-30.72V293.888c0-64.512 52.224-116.736 116.736-116.736h522.24c35.84 0 64.512 28.672 64.512 64.512v400.384C748.544 774.144 642.048 880.64 509.952 880.64z" fill="#70D4FF" p-id="10786"></path><path d="M764.928 880.64H212.992c-17.408 0-30.72-13.312-30.72-30.72V60.416h755.712c35.84 0 64.512 28.672 64.512 64.512v517.12C1002.496 774.144 896 880.64 764.928 880.64z" fill="#4E8EFF" p-id="10787"></path><path d="M555.008 403.456c0 20.48-7.168 35.84-22.528 48.128-14.336 11.264-30.72 16.384-51.2 16.384h-28.672v48.128c0 9.216 2.048 15.36 6.144 19.456 4.096 4.096 11.264 5.12 21.504 5.12V563.2H373.76v-22.528c15.36 0 23.552-8.192 23.552-24.576V389.12c0-16.384-8.192-24.576-23.552-24.576v-22.528h109.568c19.456 0 35.84 5.12 49.152 15.36 14.336 12.288 22.528 27.648 22.528 46.08z m-59.392 2.048c0-26.624-11.264-39.936-34.816-39.936h-9.216v80.896h11.264c13.312 0 22.528-3.072 26.624-10.24 4.096-7.168 6.144-17.408 6.144-30.72zM800.768 563.2h-60.416c-8.192-7.168-15.36-15.36-21.504-22.528l-57.344-74.752v50.176c0 16.384 9.216 24.576 26.624 24.576V563.2H584.704v-22.528c16.384 0 23.552-8.192 23.552-24.576V389.12c0-16.384-8.192-24.576-24.576-24.576v-22.528h105.472v22.528c-17.408 0-26.624 8.192-26.624 24.576v50.176l39.936-37.888c13.312-12.288 19.456-21.504 19.456-27.648 0-5.12-5.12-8.192-15.36-8.192v-22.528h81.92v22.528c-9.216 0-15.36 1.024-20.48 4.096-3.072 2.048-8.192 6.144-15.36 13.312L705.536 430.08l70.656 94.208c7.168 9.216 15.36 15.36 25.6 16.384V563.2z" fill="#FFFFFF" p-id="10788"></path></svg>
-                    {% if lan == 'cn' %} 比对模式 {% else %} PK Model {% endif %}
+                <a  href="/?platform=Android&lan={{ lan }}" class="btn  btn-pill w-100" >
+                    <svg t="1661854459800" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="24106" width="2000" height="2000"><path d="M555.52 943.616C339.456 943.616 163.84 768 163.84 552.448s175.616-391.68 391.68-391.68S947.2 336.384 947.2 552.448s-176.128 391.168-391.68 391.168z" fill="#38CEB1" p-id="24107"></path><path d="M815.616 820.224m-20.48 0a20.48 20.48 0 1 0 40.96 0 20.48 20.48 0 1 0-40.96 0Z" fill="#231815" p-id="24108"></path><path d="M512 61.952c-248.32 0-450.56 202.24-450.56 450.56s202.24 450.56 450.56 450.56c93.184 0 182.272-28.16 258.048-81.408 9.216-6.656 11.264-19.456 5.12-28.672-6.656-9.216-19.456-11.264-28.672-5.12-69.12 48.128-150.016 73.728-235.008 73.728-225.792 0-409.6-183.808-409.6-409.6s183.808-409.6 409.6-409.6 409.6 183.808 409.6 409.6c0 87.552-27.136 171.008-78.848 241.152-6.656 9.216-4.608 22.016 4.608 28.672 9.216 6.656 22.016 4.608 28.672-4.608 56.832-77.312 86.528-169.472 86.528-265.728 0.512-247.296-201.728-449.536-450.048-449.536z" fill="#231815" p-id="24109"></path><path d="M641.536 267.776c-8.192-8.192-20.992-8.192-29.184 0L389.632 491.008c-5.632 5.632-9.216 13.312-9.216 21.504s3.072 15.872 9.216 21.504l223.232 223.232c4.096 4.096 9.216 6.144 14.336 6.144s10.24-2.048 14.336-6.144c8.192-8.192 8.192-20.992 0-29.184L425.472 512l216.064-216.064c8.192-7.168 8.192-20.48 0-28.16z" fill="#231815" p-id="24110"></path></svg>
+                    {% if lan == 'cn' %} 普通模式 {% else %} Normal Model {% endif %}
                 </a>
             </div>
             {% else %}
             <div class="nav-item dropdown d-none d-md-flex me-3">
-                <a  href="/?platform=Android&lan={{ lan }}" class="btn  btn-pill w-100" >
-                    <svg t="1661854459800" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="24106" width="2000" height="2000"><path d="M555.52 943.616C339.456 943.616 163.84 768 163.84 552.448s175.616-391.68 391.68-391.68S947.2 336.384 947.2 552.448s-176.128 391.168-391.68 391.168z" fill="#38CEB1" p-id="24107"></path><path d="M815.616 820.224m-20.48 0a20.48 20.48 0 1 0 40.96 0 20.48 20.48 0 1 0-40.96 0Z" fill="#231815" p-id="24108"></path><path d="M512 61.952c-248.32 0-450.56 202.24-450.56 450.56s202.24 450.56 450.56 450.56c93.184 0 182.272-28.16 258.048-81.408 9.216-6.656 11.264-19.456 5.12-28.672-6.656-9.216-19.456-11.264-28.672-5.12-69.12 48.128-150.016 73.728-235.008 73.728-225.792 0-409.6-183.808-409.6-409.6s183.808-409.6 409.6-409.6 409.6 183.808 409.6 409.6c0 87.552-27.136 171.008-78.848 241.152-6.656 9.216-4.608 22.016 4.608 28.672 9.216 6.656 22.016 4.608 28.672-4.608 56.832-77.312 86.528-169.472 86.528-265.728 0.512-247.296-201.728-449.536-450.048-449.536z" fill="#231815" p-id="24109"></path><path d="M641.536 267.776c-8.192-8.192-20.992-8.192-29.184 0L389.632 491.008c-5.632 5.632-9.216 13.312-9.216 21.504s3.072 15.872 9.216 21.504l223.232 223.232c4.096 4.096 9.216 6.144 14.336 6.144s10.24-2.048 14.336-6.144c8.192-8.192 8.192-20.992 0-29.184L425.472 512l216.064-216.064c8.192-7.168 8.192-20.48 0-28.16z" fill="#231815" p-id="24110"></path></svg>
-                    {% if lan == 'cn' %} 普通模式 {% else %} Normal Model {% endif %}
+                <a href="/pk?model=2-devices&lan={{ lan }}" class="btn  btn-pill w-100" >
+                    <svg t="1661854041585" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="10784" width="2000" height="2000"><path d="M17.408 862.208a450.56 129.024 0 1 0 901.12 0 450.56 129.024 0 1 0-901.12 0Z" fill="#EEF2FF" p-id="10785"></path><path d="M509.952 880.64H75.776c-17.408 0-30.72-13.312-30.72-30.72V293.888c0-64.512 52.224-116.736 116.736-116.736h522.24c35.84 0 64.512 28.672 64.512 64.512v400.384C748.544 774.144 642.048 880.64 509.952 880.64z" fill="#70D4FF" p-id="10786"></path><path d="M764.928 880.64H212.992c-17.408 0-30.72-13.312-30.72-30.72V60.416h755.712c35.84 0 64.512 28.672 64.512 64.512v517.12C1002.496 774.144 896 880.64 764.928 880.64z" fill="#4E8EFF" p-id="10787"></path><path d="M555.008 403.456c0 20.48-7.168 35.84-22.528 48.128-14.336 11.264-30.72 16.384-51.2 16.384h-28.672v48.128c0 9.216 2.048 15.36 6.144 19.456 4.096 4.096 11.264 5.12 21.504 5.12V563.2H373.76v-22.528c15.36 0 23.552-8.192 23.552-24.576V389.12c0-16.384-8.192-24.576-23.552-24.576v-22.528h109.568c19.456 0 35.84 5.12 49.152 15.36 14.336 12.288 22.528 27.648 22.528 46.08z m-59.392 2.048c0-26.624-11.264-39.936-34.816-39.936h-9.216v80.896h11.264c13.312 0 22.528-3.072 26.624-10.24 4.096-7.168 6.144-17.408 6.144-30.72zM800.768 563.2h-60.416c-8.192-7.168-15.36-15.36-21.504-22.528l-57.344-74.752v50.176c0 16.384 9.216 24.576 26.624 24.576V563.2H584.704v-22.528c16.384 0 23.552-8.192 23.552-24.576V389.12c0-16.384-8.192-24.576-24.576-24.576v-22.528h105.472v22.528c-17.408 0-26.624 8.192-26.624 24.576v50.176l39.936-37.888c13.312-12.288 19.456-21.504 19.456-27.648 0-5.12-5.12-8.192-15.36-8.192v-22.528h81.92v22.528c-9.216 0-15.36 1.024-20.48 4.096-3.072 2.048-8.192 6.144-15.36 13.312L705.536 430.08l70.656 94.208c7.168 9.216 15.36 15.36 25.6 16.384V563.2z" fill="#FFFFFF" p-id="10788"></path></svg>
+                    {% if lan == 'cn' %} 比对模式 {% else %} PK Model {% endif %}
                 </a>
             </div>
-
             {% endif %}
             
             <div class="nav-item dropdown d-none d-md-flex me-3">
                 <a href="https://github.com/smart-test-ti/SoloX" target="_blank" class="btn  btn-pill w-100">
                     <svg t="1657096287296" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="28640" width="2000" height="2000"><path d="M511.4 511.9m-426.3 0a426.3 426.3 0 1 0 852.6 0 426.3 426.3 0 1 0-852.6 0Z" fill="#FF7A4E" p-id="28641"></path><path d="M511.4 958.2c-60.2 0-118.7-11.8-173.7-35.1-53.1-22.5-100.9-54.7-141.9-95.6-41-41-73.2-88.7-95.6-141.9-23.3-55-35.1-113.5-35.1-173.7s11.8-118.7 35.1-173.7c22.5-53.1 54.7-100.9 95.6-141.9 41-41 88.7-73.2 141.9-95.6 55-23.3 113.5-35.1 173.7-35.1 60.2 0 118.7 11.8 173.7 35.1 53.1 22.5 100.9 54.7 141.9 95.6 41 41 73.2 88.7 95.6 141.9 23.3 55 35.1 113.5 35.1 173.7s-11.7 118.7-35 173.7C900.2 738.8 868 786.5 827 827.5s-88.7 73.2-141.9 95.6c-55 23.3-113.4 35.1-173.7 35.1z m0-852.6c-224 0-406.3 182.3-406.3 406.3s182.3 406.3 406.3 406.3 406.3-182.3 406.3-406.3c0.1-224-182.2-406.3-406.3-406.3z" fill="#FF7A4E" p-id="28642"></path><path d="M716.2 547.3l-196 204.1L340.8 579l0.6-0.7-27.2-25.4c-50.3-46.9-53-125.6-6.2-175.9 46.9-50.3 125.6-53 175.9-6.2l29.9 27.9 22.9-23.9c19.5-20.3 44.2-32.6 70.1-36.7 37.2-5.9 76.6 5 105.9 33.1 49.5 47.7 51.1 126.5 3.5 176.1z" fill="#FFFFFF" p-id="28643"></path></svg>
                     {% if lan == 'cn' %} 点赞 {% else %} Star Me {% endif %}
                 </a>
@@ -133,15 +132,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/smart-test-ti" class="link-secondary">SoloX</a>.{% if lan == 'cn' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.5.6
+                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.5.8
                             </a>
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
```

#### html2text {}

```diff
@@ -9,31 +9,31 @@
 
 
 
  {% block css %} {% endblock %}
 
 ****** [SoloX] SoloX ******
 {% block navbar_nav %}{% endblock %}
-{% if platform %}
-_{%_if_lan_==_'cn'_%}_æ¯å¯¹æ¨¡å¼_{%_else_%}_PK_Model_{%_endif_%}
-{% else %}
+{% if model in ['2-app','2-devices'] %}
 _{%_if_lan_==_'cn'_%}_æ®éæ¨¡å¼_{%_else_%}_Normal_Model_{%_endif_%}
+{% else %}
+_{%_if_lan_==_'cn'_%}_æ¯å¯¹æ¨¡å¼_{%_else_%}_PK_Model_{%_endif_%}
 {% endif %}
 _{%_if_lan_==_'cn'_%}_ç¹èµ_{%_else_%}_Star_Me_{%_endif_%}
 ä¸­æ English
 
 ***** {% block page_title %} {% endblock %} *****
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'cn'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
     * _{%_if_lan_==_'cn'_%}_åæ¯åå¡_{%_else_%}_Sponsor_{%_endif_%}
     * Copyright ©  SoloX.{% if lan == 'cn' %} ä¿çæææå© {% else %} All
       rights reserved {% endif %}
-    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.5.6
+    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.5.8
 *****  {% if lan == 'cn' %} è®¾ç½® {% else %} Setting {% endif %} *****
     * Warning_Value
     * Timer
     * Agent_ _{%_if_lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'cn' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [{
 { cpuWarning }}    ]
 {% if lan == 'cn' %} åå­åè­¦å¼ {% else %} Memory warning value {% endif
```

### Comparing `solox-2.5.7/solox/templates/index.html` & `solox-2.5.8/solox/templates/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -71,24 +71,14 @@
             {% if lan == 'cn' %} 开始 {% else %} Start {% endif %}
         </a>
         <a id="stop-apm" onclick="stopTask()" class="btn btn-default" style="display: none">
             <svg t="1638096947956" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="235254" width="200" height="200"><path d="M512 512m-512 0a512 512 0 1 0 1024 0 512 512 0 1 0-1024 0Z" fill="#EE827F" p-id="235255"></path><path d="M512 512m-443.191534 0a443.191534 443.191534 0 1 0 886.383068 0 443.191534 443.191534 0 1 0-886.383068 0Z" fill="#E64537" p-id="235256"></path><path d="M0 512C0 794.638448 229.180952 1023.8194 512 1023.8194V0C229.180952 0 0 229.180952 0 512z" fill="#FEFFFF" opacity=".1" p-id="235257"></path><path d="M477.866667 683.208466H375.647266c-1.083598 0-1.986596-0.902998-1.986596-1.986597V342.597531c0-1.083598 0.902998-1.986596 1.986596-1.986596h102.4c1.083598 0 1.986596 0.902998 1.986596 1.986596v338.443739c-0.1806 1.264198-1.083598 2.167196-2.167195 2.167196zM648.352734 683.208466h-102.4c-1.083598 0-1.986596-0.902998-1.986596-1.986597V342.597531c0-1.083598 0.902998-1.986596 1.986596-1.986596H648.352734c1.083598 0 1.986596 0.902998 1.986596 1.986596v338.443739c0 1.264198-0.902998 2.167196-1.986596 2.167196z" fill="#FFFFFF" p-id="235258"></path></svg>
             {% if lan == 'cn' %} 停止 {% else %} Stop {% endif %}
         </a>
     </div>
-    <div class="btn-list logcat-btn-list" style="display:none">
-        <a id="logcat-copy" class="btn"  onclick="cppyLogcat()">
-            <svg t="1647757557543" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="26288" width="200" height="200"><path d="M943.4112 480.3072v101.3248c0 95.5904-61.3376 176.7936-146.7904 206.4896 7.936-22.6304 12.288-46.8992 12.288-72.192V437.248c0-120.7808-97.8944-218.6752-218.6752-218.6752H311.6032c-25.1904 0-49.3568 4.3008-71.8848 12.1344 29.8496-85.248 110.9504-146.432 206.3872-146.432h278.6816c120.7808 0 218.6752 97.8944 218.6752 218.6752v177.3568z" fill="#FFD833" p-id="26289"></path><path d="M943.4112 454.7072c-14.1312 0-25.6 11.4688-25.6 25.6v101.3248c0 64.9728-32.6144 124.416-84.6336 159.744 0.8704-8.448 1.3312-16.896 1.3312-25.4464V437.2992c0-134.7072-109.568-244.2752-244.2752-244.2752H311.6032c-8.3456 0-16.6912 0.4096-24.9856 1.28a193.05984 193.05984 0 0 1 159.5392-84.3776h278.6816c106.4448 0 193.0752 86.5792 193.0752 193.0752 0 14.1312 11.4688 25.6 25.6 25.6s25.6-11.4688 25.6-25.6c0-134.656-109.568-244.2752-244.2752-244.2752H446.1056c-89.5488 0-171.776 48.9472-214.6304 127.6928a41.69216 41.69216 0 0 0-5.0688 21.4528c-94.8736 28.5184-164.1984 116.6336-164.1984 220.672v306.3808c0 127.0272 103.3728 230.4 230.4 230.4h306.3808c101.6832 0 188.1088-66.2016 218.624-157.7984 91.0848-37.4272 151.4496-126.5152 151.4496-225.8944V480.3072c-0.0512-14.1312-11.52-25.6-25.6512-25.6z m-344.4224 459.4176H292.608c-98.816 0-179.2-80.384-179.2-179.2V428.544c0-98.816 80.384-179.2 179.2-179.2h306.3808c98.816 0 179.2 80.384 179.2 179.2v306.3808c0 15.3088-1.9456 30.1056-5.5296 44.288l-0.1536 0.4608c-0.4096 1.1264-0.7168 2.2528-0.9216 3.3792-21.1456 75.52-90.4704 131.072-172.5952 131.072z" fill="#44454A" p-id="26290"></path><path d="M943.4112 428.8512c-14.1312 0-25.6-11.4688-25.6-25.6v-17.92c0-14.1312 11.4688-25.6 25.6-25.6s25.6 11.4688 25.6 25.6v17.92c0 14.1312-11.4688 25.6-25.6 25.6z" fill="#44454A" p-id="26291"></path></svg>
-            {% if lan == 'cn' %} 复制 {% else %} Copy {% endif %}
-        </a>
-        <a id="logcat-clear" class="btn" onclick="clearLogcat()">
-            <svg t="1647762455383" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5349" width="200" height="200"><path d="M399.25 337.55l283.9 283.8c2.1 2.1 2.58 5.25 1.05 7.83-15.36 24.53-92.76 154.5-113.46 326.27a2.02 2.02 0 0 0-2.96 1.53l-96.38-58.12c-0.86-0.57-1.24-1.62-0.76-2.58 9.07-18.99 95.81-200.69 86.93-191.81-9.35 9.35-69.38 73.1-114.32 138.28l-25.86 35.59s-101.44-68.23-132.74-110.7c-0.48-0.67-0.57-1.24 0-1.81 20.61-25 127.87-164.42 127.87-164.42L230.15 710.77c-0.86 0.48-1.81 0.38-2.48-0.38-8.87-9.83-69.76-77.11-87.32-108.69-0.38-0.67-0.38-1.24 0.29-1.81 17.37-14.03 115.56-97.24 115.56-97.24L117.92 551.6c-0.95 0.29-2-0.1-2.48-0.95l-51.15-96c-0.67-1.15-0.19-2.58 1.15-2.86 24.33-4.87 227.41-47.05 325.98-115.09 2.49-1.73 5.73-1.35 7.83 0.85z m383.81 428.38c0-21.34 17.3-38.65 38.65-38.65 21.35 0 38.65 17.3 38.65 38.65 0 21.34-17.3 38.65-38.65 38.65-21.34-0.01-38.65-17.31-38.65-38.65z m-158.12 75c0-39.21 31.79-71 71-71s71 31.79 71 71-31.79 71-71 71-71-31.79-71-71zM281.59 214.54c0-31.31 25.38-56.68 56.68-56.68 31.31 0 56.68 25.38 56.68 56.68 0 31.31-25.38 56.68-56.68 56.68-31.3 0.01-56.68-25.37-56.68-56.68z m479.34 144.67c-0.29 2.48-0.57 4.1-0.76 6.58 39.98 69.09 39.79 149.06-18.9 210.71-1.72 1.81-4.87 1.91-6.68 0.1L449.83 291.84c-1.81-1.81-1.72-4.96 0.1-6.68 61.55-58.78 141.62-58.97 210.71-18.89 2.39-0.29 4.1-0.48 6.49-0.76L846.91 86.1c25.96-25.77 67.85-25.77 93.71 0.09 25.86 25.96 25.86 67.94-0.1 93.81L760.93 359.21z" p-id="5350"></path></svg>
-            {% if lan == 'cn' %} 清除 {% else %} Clear {% endif %}
-        </a>
-    </div>
 </div>
 {% endblock %}
 
 {% block page_body %}
 <div class="row">
     <div class="apm-info" style="width: 25%">
         <div class="dropdown-menu dropdown-menu-demo">
@@ -148,17 +138,17 @@
                                     <label class="form-check form-check-single form-switch">
                                         <input id="fps-switch" class="form-check-input cursor-pointer" type="checkbox" checked name="fps-switch" style="margin-right: 5px"> SurfaceView
                                     </label>
                                 </span>
                                 {% endif %}
                             </label>
                             <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="battery_checkbox" type="checkbox" name="battery" checked> {% if lan == 'cn' %} 电池 {% else %} Battery {% endif %}</label>
-                            <!-- {% if platform == 'iOS' %}
-                            <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="gpu_checkbox" type="checkbox" checked name="cpu"> GPU</label>
-                            {% endif %} -->
+                            {% if platform == 'iOS' %}
+                            <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="gpu_checkbox" type="checkbox" checked name="gpu"> GPU</label>
+                            {% endif %}
                         </div>
                         <div class="tab-pane" id="tabs-device-info">
                             <div class="mb-2">
                                 <strong>{% if lan == 'cn' %} 品牌 {% else %} Brand {% endif %}:</strong> <lable id="brand"></lable>
                             </div>
                             <div class="mb-2">
                                 <strong>{% if lan == 'cn' %} 设备名称 {% else %} Device Name {% endif %}:</strong> <lable id="device_name"></lable>
@@ -176,18 +166,16 @@
                     </div>
                 </div>
             </div>
             {% if platform == 'Android' %}
             <a class="dropdown-item" style="margin-top: 10px;">
                 <svg t="1657093102367" class="icon me-2" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="27860" width="2000" height="2000"><path d="M938.362 256.2V149.626c0-23.576-19.11-42.654-42.652-42.654H43.046C19.502 106.972 0.392 126.05 0.392 149.626V256.2h937.97z" fill="#E6E9ED" p-id="27861"></path><path d="M792.164 831.75H0.392V192.25h937.97v446.306z" fill="#656D78" p-id="27862"></path><path d="M85.67 149.626c0 11.772-9.526 21.296-21.328 21.296-11.74 0-21.294-9.524-21.294-21.296S52.602 128.3 64.342 128.3c11.802 0 21.328 9.556 21.328 21.326z" fill="#ED5564" p-id="27863"></path><path d="M149.62 149.626c0 11.772-9.524 21.296-21.326 21.296-11.742 0-21.296-9.524-21.296-21.296S116.55 128.3 128.292 128.3c11.804 0 21.328 9.556 21.328 21.326z" fill="#FFCE54" p-id="27864"></path><path d="M213.568 149.626c0 11.772-9.524 21.296-21.326 21.296-11.74 0-21.294-9.524-21.294-21.296S180.502 128.3 192.242 128.3c11.802 0 21.326 9.556 21.326 21.326z" fill="#A0D468" p-id="27865"></path><path d="M746.512 277.496H106.996c-11.772 0-21.326 9.554-21.326 21.326s9.554 21.328 21.326 21.328h639.516c11.74 0 21.294-9.556 21.294-21.328s-9.554-21.326-21.294-21.326z" fill="#FC6E51" p-id="27866"></path><path d="M106.996 405.426h341.046c11.802 0 21.326-9.554 21.326-21.328 0-11.772-9.524-21.326-21.326-21.326H106.996c-11.772 0-21.326 9.554-21.326 21.326 0 11.774 9.554 21.328 21.326 21.328z" fill="#AC92EB" p-id="27867"></path><path d="M575.958 448.05H106.996c-11.772 0-21.326 9.556-21.326 21.328s9.554 21.296 21.326 21.296h468.962c11.8 0 21.294-9.524 21.294-21.296s-9.492-21.328-21.294-21.328z" fill="#48CFAD" p-id="27868"></path><path d="M106.996 575.952H405.42c11.772 0 21.326-9.556 21.326-21.328s-9.554-21.296-21.326-21.296H106.996c-11.772 0-21.326 9.526-21.326 21.296s9.554 21.328 21.326 21.328z" fill="#5D9CEC" p-id="27869"></path><path d="M615.678 669.22c8.618 0 16.734-5.278 19.984-13.832 4.122-11.024-1.5-23.326-12.492-27.45-41.03-15.392-47.336-54.708-47.336-55.112a21.332 21.332 0 0 0-24.232-17.956c-11.662 1.716-19.688 12.552-17.97 24.2 0.376 2.624 10.242 64.668 74.55 88.776 2.5 0.938 4.996 1.374 7.496 1.374zM959.534 917.028c1 0 2.06-0.094 3.122-0.25 11.68-1.716 19.674-12.552 17.988-24.2-0.376-2.624-10.242-64.668-74.566-88.776-11.054-4.152-23.296 1.438-27.48 12.458-4.122 11.024 1.5 23.326 12.492 27.448 41.03 15.394 47.336 54.708 47.398 55.114a21.28 21.28 0 0 0 21.046 18.206zM448.042 618.572H106.996c-11.772 0-21.326 9.554-21.326 21.328 0 11.772 9.554 21.326 21.326 21.326h341.046c11.802 0 21.326-9.554 21.326-21.326a21.312 21.312 0 0 0-21.326-21.328z" fill="#FFCE54" p-id="27870"></path><path d="M277.52 703.85H106.996c-11.772 0-21.326 9.554-21.326 21.328 0 11.772 9.554 21.294 21.326 21.294h170.524c11.772 0 21.326-9.524 21.326-21.294 0-11.774-9.554-21.328-21.326-21.328z" fill="#ED5564" p-id="27871"></path><path d="M1002.312 746.472H533.318a21.28 21.28 0 0 1-21.294-21.294c0-11.774 9.524-21.328 21.294-21.328h468.994c11.74 0 21.294 9.554 21.294 21.328 0.002 11.772-9.554 21.294-21.294 21.294zM725.592 555.53a21.332 21.332 0 0 1-18.298-10.368l-64.388-107.478c-5.994-10.086-2.746-23.202 7.372-29.228a21.276 21.276 0 0 1 29.226 7.338l64.324 107.478c6.058 10.086 2.81 23.17-7.306 29.228a21.286 21.286 0 0 1-10.93 3.03zM810.212 555.53c-3.686 0-7.496-0.968-10.93-3.03-10.054-6.058-13.364-19.142-7.306-29.26l64.324-107.446a21.278 21.278 0 0 1 29.228-7.338c10.118 6.026 13.364 19.11 7.368 29.228l-64.324 107.478c-3.996 6.65-11.116 10.368-18.36 10.368zM920.002 669.22c-8.62 0-16.738-5.278-19.922-13.832-4.184-11.024 1.436-23.326 12.426-27.45 41.094-15.392 47.34-54.708 47.402-55.112 1.686-11.648 12.55-19.674 24.168-17.956 11.68 1.716 19.734 12.552 17.986 24.2-0.376 2.624-10.242 64.668-74.568 88.776a20.884 20.884 0 0 1-7.492 1.374zM575.958 917.028c-1 0-2.062-0.094-3.124-0.25-11.616-1.716-19.672-12.552-17.984-24.2 0.438-2.624 10.242-64.668 74.566-88.776 11.054-4.152 23.356 1.438 27.478 12.458 4.124 11.024-1.436 23.326-12.49 27.448-41.032 15.394-47.276 54.708-47.338 55.114-1.56 10.586-10.68 18.206-21.108 18.206z" fill="#FFCE54" p-id="27872"></path><path d="M938.236 682.524c0 129.524-48.71 234.504-170.43 234.504-121.716 0-170.43-104.98-170.43-234.504 0-129.494 63.39-191.85 170.43-191.85 107.044-0.002 170.43 62.356 170.43 191.85z" fill="#ED5564" p-id="27873"></path><path d="M746.512 915.872c6.806 0.75 13.928 1.156 21.294 1.156 7.372 0 14.49-0.406 21.296-1.156v-297.3h-42.592v297.3z" fill="#DA4453" p-id="27874"></path><path d="M603.56 618.572h328.494c-18.298-86.12-76.626-127.9-164.248-127.9-87.616 0-145.946 41.782-164.246 127.9z" fill="#DA4453" p-id="27875"></path></svg>
                 {% if lan == 'cn' %} 错误日志 {% else %} Error Log {% endif %}
-                <span class="ms-auto">
-                    <label class="form-check form-check-single form-switch">
-                        <input id="logcat-switch" class="form-check-input cursor-pointer" type="checkbox" name="logcat_content">
-                    </label>
+                <span class="ms-auto badge bg-red" data-bs-toggle="offcanvas" href="#offcanvasBottom" role="button" aria-controls="offcanvasBottom">
+                    OPEN
                 </span>
             </a>
             <div class="dropdown-divider"></div>
             {% endif %}
             <a class="dropdown-item" style="margin-top: 10px;">
                 <input type="file" class="form-control" id="app-file" accept=".apk,.ipa"/>
             </a>
@@ -213,24 +201,48 @@
         <div id="mem_android"  class="mb-3 mem" style="min-width:400px;height:310px"></div>
         <div id="fps" class="mb-3 fps" style="min-width:400px;height:300px"></div>
         <div id="battery_android" class="mb-3 battery" style="min-width:400px;height:310px"></div>
         {% else %}
         <div id="mem_ios"  class="mb-3 mem" style="min-width:400px;height:310px"></div>
         <div id="fps_ios" class="mb-3 fps" style="min-width:400px;height:310px"></div>
         <div id="battery_ios" class="mb-3 battery" style="min-width:400px;height:310px"></div>
-        <!-- <div id="gpu" class="mb-3 gpu" style="min-width:400px;height:310px"></div> -->
+        <div id="gpu" class="mb-3 gpu" style="min-width:400px;height:310px"></div>
         {% endif %}
         <div id="network" class="Network-Data mb-3" style="min-width:400px;height:310px"></div>
     </div>
-
-    <div class="logcat-data dropdown-menu dropdown-menu-demo" style="width: 75%;display:none">
-        <textarea id="logcat-content" class="form-control" spellcheck="false" style="height:700px;line-height: 30px;padding: 10px;font-size: 16px;color:#ff3136;outline:none;border: none"></textarea>
+</div>
+</div>
+<div class="offcanvas offcanvas-bottom layout-boxed" tabindex="-1" id="offcanvasBottom" aria-labelledby="offcanvasBottomLabel" style="height: 85%;margin-left: 10%;margin-right: 10%;">
+    <div class="offcanvas-header">
+      <h2 class="offcanvas-title" id="offcanvasBottomLabel">Error Log</h2>
+      <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
     </div>
+    <div class="offcanvas-body">
+        <div class="btn-list logcat-btn-list">
+            <a id="run-logcat" class="btn btn-default" onclick="startLogcat()">
+                <svg t="1647757457022" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="21859" width="200" height="200"><path d="M511.4 512.1m-448 0a448 448 0 1 0 896 0 448 448 0 1 0-896 0Z" fill="#006DFC" p-id="21860"></path><path d="M658.4 555.6L475.5 661.1c-33.4 19.3-75-4.8-75-43.3V406.6c0-38.5 41.7-62.6 75-43.3l182.9 105.6c33.3 19.3 33.3 67.4 0 86.7z" fill="#FFFFFF" p-id="21861"></path></svg>
+                {% if lan == 'cn' %} 开始 {% else %} Start {% endif %}
+            </a>
+            <a id="stop-logcat"  class="btn btn-default" style="display: none" onclick="stopLogcat()">
+                <svg t="1638096947956" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="235254" width="200" height="200"><path d="M512 512m-512 0a512 512 0 1 0 1024 0 512 512 0 1 0-1024 0Z" fill="#EE827F" p-id="235255"></path><path d="M512 512m-443.191534 0a443.191534 443.191534 0 1 0 886.383068 0 443.191534 443.191534 0 1 0-886.383068 0Z" fill="#E64537" p-id="235256"></path><path d="M0 512C0 794.638448 229.180952 1023.8194 512 1023.8194V0C229.180952 0 0 229.180952 0 512z" fill="#FEFFFF" opacity=".1" p-id="235257"></path><path d="M477.866667 683.208466H375.647266c-1.083598 0-1.986596-0.902998-1.986596-1.986597V342.597531c0-1.083598 0.902998-1.986596 1.986596-1.986596h102.4c1.083598 0 1.986596 0.902998 1.986596 1.986596v338.443739c-0.1806 1.264198-1.083598 2.167196-2.167195 2.167196zM648.352734 683.208466h-102.4c-1.083598 0-1.986596-0.902998-1.986596-1.986597V342.597531c0-1.083598 0.902998-1.986596 1.986596-1.986596H648.352734c1.083598 0 1.986596 0.902998 1.986596 1.986596v338.443739c0 1.264198-0.902998 2.167196-1.986596 2.167196z" fill="#FFFFFF" p-id="235258"></path></svg>
+                {% if lan == 'cn' %} 停止 {% else %} Stop {% endif %}
+            </a>
+            <a id="logcat-copy" class="btn"  onclick="cppyLogcat()">
+                <svg t="1681097872350" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="14723" width="50" height="50"><path d="M744.296296 128a151.703704 151.703704 0 0 1 151.703704 151.703704v344.613926a75.851852 75.851852 0 0 1-75.851852 75.851851h-38.589629V373.210074a130.787556 130.787556 0 0 0-130.768593-130.768593L323.830519 242.422519V203.851852a75.851852 75.851852 0 0 1 75.851851-75.851852h344.613926z m-93.50637 179.825778a65.384296 65.384296 0 0 1 65.384296 65.384296v10.467556a75.851852 75.851852 0 0 0-72.059259-75.757037l-3.792593-0.094815h10.467556z" fill="#0CCA8A" fill-opacity=".5" p-id="14724"></path><path d="M144.004741 307.825778m75.851852 0l420.465777 0q75.851852 0 75.851852 75.851852l0 420.465777q0 75.851852-75.851852 75.851852l-420.465777 0q-75.851852 0-75.851852-75.851852l0-420.465777q0-75.851852 75.851852-75.851852Z" fill="#0CCA8A" p-id="14725"></path></svg>
+                {% if lan == 'cn' %} 复制 {% else %} Copy {% endif %}
+            </a>
+            <a id="logcat-clear" class="btn" onclick="clearLogcat()">
+                <svg t="1681097907668" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="15706" width="50" height="50"><path d="M274.5344 582.0928h480.9728v265.0624H274.5344z" fill="#D9FFEC" p-id="15707"></path><path d="M852.6336 539.9552H177.408c-43.9296 0-79.6672-35.7376-79.6672-79.6672V335.8208c0-43.9296 35.7376-79.6672 79.6672-79.6672h159.8976V175.7184c0-48.5376 39.4752-88.064 88.064-88.064h179.3536c48.5376 0 88.064 39.4752 88.064 88.064v80.4864h159.8976c43.9296 0 79.6672 35.7376 79.6672 79.6672v124.5184c-0.0512 43.8784-35.7888 79.5648-79.7184 79.5648z m-672.9728-81.92h670.72V338.1248H651.776c-22.6304 0-40.96-18.3296-40.96-40.96V175.7184c0-3.3792-2.7648-6.144-6.144-6.144H425.3696c-3.3792 0-6.144 2.7648-6.144 6.144v121.4464c0 22.6304-18.3296 40.96-40.96 40.96H179.6608v119.9104z" fill="#34333A" p-id="15708"></path><path d="M390.5536 889.9072c-22.6304 0-40.96-18.3296-40.96-40.96v-173.6704c0-22.6304 18.3296-40.96 40.96-40.96s40.96 18.3296 40.96 40.96v173.6704c0 22.6304-18.3296 40.96-40.96 40.96z" fill="#3AD285" p-id="15709"></path><path d="M797.7472 932.1472H232.2944c-53.1456 0-96.3584-43.2128-96.3584-96.3584v-255.9488h81.92v255.9488c0 7.9872 6.5024 14.4384 14.4384 14.4384H797.696c7.9872 0 14.4384-6.5024 14.4384-14.4384v-255.9488h81.92v255.9488c0.0512 53.0944-43.1616 96.3584-96.3072 96.3584z" fill="#34333A" p-id="15710"></path></svg>
+                {% if lan == 'cn' %} 清除 {% else %} Clear {% endif %}
+            </a>
+        </div>
+        <div class="mt-2" id="logcat-content" style="color: rgba(214, 39, 8, 0.849);"></div>
+    </div>
+  </div>
 </div>
-
 {% endblock %}
 
 {% block js %}
 <script>
 
     var stop = false; // 任务状态
 
@@ -274,24 +286,24 @@
             },
             beforeSend: function () {
                 $('.select-app').empty();
                 $('.select-app').append('<option></option>');
                 if(lan == 'cn' ){
                     SwalLoading('初始化','正在获取该设备上的所有APP, 请您稍等！');
                 }else{
-                    SwalLoading('Package initialization!','Initializing Packages, please wait。');
+                    SwalLoading('Package initialization!','Initializing Packages, please wait a mmoment.');
                 }
                 
             },
             success: function (data) {
                 if(data['status'] != 1 ) {
                     if(lan == 'cn' ){
                         SwalFire('error', '连接失败','请检查当前移动设备的是否连接了PC端', 2000);
                     }else{
-                        SwalFire('error', 'Connet failed !', 'Please check if the device is connected', 2000);
+                        SwalFire('error', 'Connet failed !', 'No devices found', 2000);
                     } 
                 }else{
                     for(var i=0;i<data['pkgnames'].length;i++){
                         $('.select-app').append('<option>'+data['pkgnames'][i]+'</option>')
                     }
                     swal.close();
                 }
@@ -321,24 +333,24 @@
             beforeSend: function () {
                 $('.select-device').empty();
                 $('.select-app').empty();
                 $('.select-app').append('<option></option>');
                 if(lan == 'cn' ){
                     SwalLoading('初始化','正在初始化设备环境，请您稍等！');
                 }else{
-                    SwalLoading('Device initialization!','Initializing device environment, please wait。');
+                    SwalLoading('Device initialization!','Initializing device environment, please wait a moment.');
                 }
                 },
             success: function (data) {
                 console.log(data);
                 if(data['status'] != 1 ) {
                     if(lan == 'cn' ){
                         SwalFire('error', '连接失败','请检查当前移动设备的是否连接了PC端', 2000);
                     }else{
-                        SwalFire('error', 'Connet failed !', 'Please check if the device is connected', 2000);
+                        SwalFire('error', 'Connet failed !', 'No devices found', 2000);
                     } 
                 }else{
                     for(var i=0;i<data['devices'].length;i++){
                         $('.select-device').append('<option>'+data['devices'][i]+'</option>');
                     }
                     for(var i=0;i<data['pkgnames'].length;i++){
                         $('.select-app').append('<option>'+data['pkgnames'][i]+'</option>');
@@ -395,14 +407,48 @@
             },
             error: function(){
                 SwalFire('error','Host Error','Host is invalid',5000);
             }
         });
     }
 
+    function getGpu(pkgname){
+        $.ajax({
+            url: Host + "/apm/gpu",
+            type: "GET",
+            async: true,
+            cache: false,
+            data:{
+                pkgname:pkgname
+            },
+            beforeSend: function () {
+               window.clearTimeout(timerQ);
+            },
+            success: function (data) {
+                if(stop == false){
+                    console.log(data)
+                    if(data['status'] == 1){
+                        try {
+                            var series= gpu_chart.series[0];
+                            var x = (new Date()).getTime(),
+                            y = data['gpu'];
+                            series.addPoint([x, y], true, true);
+                            timerQ = setTimeout(getGpu(pkgname), 1000);
+                        }catch (e) {}
+                    }else{
+                        SwalFire('error','something error',data['msg'],2000);
+                    }
+                }
+            },
+            error: function(){
+                SwalFire('error','Host Error','Host is invalid',5000);
+            }
+        });
+    }
+
     function getBattery(device){
         $.ajax({
             url: Host + "/apm/battery",
             type: "GET",
             async: true,
             cache: false,
             data:{
@@ -702,41 +748,41 @@
                 ]);
             }
             return data;
         }())
     }];
 
     var seriesMem = [{
-        name : 'totalPass',
+        name : 'total',
         pointInterval: 120 * 1000,
         data : (function () {
             var data = [], time = (new Date()).getTime(), i;
             for (i = -999; i <= 0; i += 1) {
                 data.push([
                     time + i * 1000,
                     Math.round(0)
                 ]);
             }
             return data;
         }())
     },{
-        name : 'nativePass',
+        name : 'native',
         pointInterval: 120 * 1000,
         data : (function () {
             var data = [], time = (new Date()).getTime(), i;
             for (i = -999; i <= 0; i += 1) {
                 data.push([
                     time + i * 1000,
                     Math.round(0)
                 ]);
             }
             return data;
         }())
     },{
-        name : 'dalvikPass',
+        name : 'dalvik',
         pointInterval: 120 * 1000,
         data : (function () {
             var data = [], time = (new Date()).getTime(), i;
             for (i = -999; i <= 0; i += 1) {
                 data.push([
                     time + i * 1000,
                     Math.round(0)
@@ -1012,20 +1058,20 @@
 
     function networkInitialize(){
         //初始化network
         let network_chart = chartsInitialize('network','Network Data（KB)');
         return network_chart
     }
 
-    // function gpuInitialize(){
-    //     if(platform == 'iOS'){
-    //         let gpu_chart = chartsInitialize('gpu','GPU（%）');
-    //         return gpu_chart
-    //     }
-    // }
+    function gpuInitialize(){
+        if(platform == 'iOS'){
+            let gpu_chart = chartsInitialize('gpu','GPU（%）');
+            return gpu_chart
+        }
+    }
 
     function fpsInitialize(){
         //初始化fps
         if(platform === 'Android'){
             let title = 'FPS and Jank';
             let fps_chart = chartsInitialize('fps',title);
             return fps_chart
@@ -1037,15 +1083,15 @@
     }
 
     var cpu_chart = cpuInitialize();
     var mem_chart = memInitialize();
     var network_chart = networkInitialize();
     var fps_chart = fpsInitialize();
     var battery_chart = batteryInitialize();
-    // var gpu_chart = gpuInitialize()
+    var gpu_chart = gpuInitialize()
 
 
     function collectPers(device,pkgname=null,type,title,func){
         // 收集性能数据初始化
         let seriesFinal = series;
         let legend = false;
         let yAxis = {
@@ -1136,14 +1182,22 @@
         if(cpu_checkbox){
             cpuInitialize();
             let type = 'cpu';
             cpu_chart = collectPers(device,pkgname,type,'CPU（%）',getCpuRate(pkgname,device));
         }
     }
 
+    function collectGpu(pkgname){
+        var gpu_checkbox = $('#gpu_checkbox').is(':checked');
+        if(gpu_checkbox){
+            gpuInitialize();
+            cpu_chart = collectPers('',pkgname,'gpu','GPU（%）',getGpu(pkgname));
+        }
+    }
+
     function collectBattery(device){
         var battery_checkbox = $('#battery_checkbox').is(':checked');
         if(battery_checkbox){
             batteryInitialize();
             let type = platform == 'Android' ? 'battery_android' : 'battery_ios';
             battery_chart = collectPers(device,null,type,'Battery',getBattery(device));
         }
@@ -1180,18 +1234,14 @@
             }else{
                 let title = 'FPS（HZ）';
                 fps_chart = collectPers(device,pkgname,'fps_ios',title,getFps(pkgname,device,fps_switch));
             }
         }
     }
 
-    function stopRun(){
-        
-    }
-
     function stopTask(){
         stop = true;
         var wifi_switch = $('#net-switch').is(':checked');
         $('#run-apm').show();
         $('#stop-apm').hide();
         window.clearTimeout(timerQ);
         $.ajax({
@@ -1209,18 +1259,14 @@
             beforeSend: function () {
                 
                 if(lan == 'cn'){
                     SwalLoading('保存数据','正在保存数据生成报告, 请不要离开页面.')
                 }else{
                     SwalLoading('Save data','Saving data to generate report, please do not leave.')
                 }
-                // let device = $('.select-device').val();
-                // let pkgname = $('.select-app').val();
-                // var net_switch = $('#net-switch').is(':checked');
-                // setNetWork('end',device,pkgname,net_switch)
             },
             success: function (data) {
                 if(data['status']==1){
                     window.location.href = '/report?lan='+lan
                 }else{
                     SwalFire('error','Execution error',data['msg'],2000)
                 }
@@ -1238,73 +1284,66 @@
             var net_switch = $('#net-switch').is(':checked');
             setNetWork('pre',device,pkgname,net_switch)
             collectCpu(device,pkgname);
             collectMem(device,pkgname);
             collectNetwork(device,pkgname);
             collectFps(device,pkgname);
             collectBattery(device);
+            if(platform == 'iOS'){
+                collectGpu(pkgname);
+            }
             if(parseInt($('#running_value').val()) > 0){
                 var times = parseInt($('#running_value').val()) * 60 * 1000
                 setTimeout("stopTask()", times)
             }
         }else{
             if(lan == 'cn'){
                 SwalFire('error','执行错误','没有选择APP或者设备',2000);
             }else{
                 SwalFire('error','Execution error','No device or package name selected',2000);
             }
             $('#run-apm').show();
             $('#stop-apm').hide();
         }});
 
-    $('#logcat-switch').change(function() {
-        let  flag= $(this).is(':checked');
-        if(flag){
-            startLogcat();
-            $('.apm-btn-list').hide();
-            $('.apm-data').hide();
-            $('.logcat-btn-list').show();
-            $('.logcat-data').show();
-        }else{
-            $('.logcat-btn-list').hide();
-            $('.logcat-data').hide();
-            $('.apm-btn-list').show();
-            $('.apm-data').show();
-        }
-    });
-
     var status = false;
+    var socket = io.connect('http://' + document.domain + ':' + location.port + '/logcat',{'forceNew':true });
     function startLogcat() {
         let device = $('.select-device').val();
         if(device){
-            $('#logcat_start').hide();
-            $('#logcat_stop').show();
-            var socket = io.connect('http://' + document.domain + ':' + location.port + '/logcat',{'forceNew':true });
+            $('#run-logcat').hide();
+            $('#stop-logcat').show();
+            socket = io.connect('http://' + document.domain + ':' + location.port + '/logcat',{'forceNew':true });
             socket.on('message', function (msg) {
                 if(status){
-                    $('#logcat-content').prepend(msg.data);
+                    $('#logcat-content').prepend(msg.data + '<br>');
                 }
             });
         }else{
             SwalFire('error','Execution error','No device selected',2000)
         }
     };
 
     function stopLogcat() {
-        $('#logcat_stop').hide();
-        $('#logcat_start').show();
+        $('#run-logcat').show();
+        $('#stop-logcat').hide();
         status = false;
-        socket.emit('disconnect_request');
+        // socket.emit('disconnect_request');
+        socket.close()
 
     };
 
     function cppyLogcat() {
-        let url_content = $("#logcat-content");
-        url_content.select();
-        document.execCommand("copy");
+        const textValue = document.createElement('textarea');
+        document.body.appendChild(textValue);
+        textValue.value = $("#logcat-content").text(); 
+        textValue.select();
+        var result = document.execCommand('copy');
+        console.log(result)
+        document.body.removeChild(textValue);
         SwalFire('success','Copy Success','',1000);
     };
 
     function clearLogcat() {
         $('#logcat-content').empty();
     };
```

### Comparing `solox-2.5.7/solox/templates/pk.html` & `solox-2.5.8/solox/templates/pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/templates/report.html` & `solox-2.5.8/solox/templates/report.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox/view/apis.py` & `solox-2.5.8/solox/view/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 import time
 from flask import request, make_response
 from logzero import logger
 from flask import Blueprint
 import traceback
-from solox.public.apm import CPU, MEM, Flow, FPS, Battery,Target
+from solox.public.apm import CPU, MEM, Flow, FPS, Battery, GPU, Target
 from solox.public.apm_pk import CPU_PK, MEM_PK, Flow_PK, FPS_PK
 from solox.public.common import Devices, file, Method, Install, Platform
 
 d = Devices()
 f = file()
 api = Blueprint("api", __name__)
 method = Method()
@@ -129,15 +129,15 @@
                 pkgNameList = []
                 pkgNameList.append(pkgname)
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 cpu = CPU_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = cpu.getAndroidCpuRate()
                 result = {'status': 1, 'first': first, 'second': second}
-            case '2-devices':
+            case '2-app':
                 pkgNameList = pkgname.split(',')
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 cpu = CPU_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = cpu.getAndroidCpuRate()
                 result = {'status': 1, 'first': first, 'second': second}
             case _:
@@ -222,25 +222,25 @@
                 pkgNameList = []
                 pkgNameList.append(pkgname)
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 network = Flow_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = network.getNetWorkData()
                 result = {'status': 1, 'first': first, 'second': second}
-            case '2-devices':
+            case '2-app':
                 pkgNameList = pkgname.split(',')
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 network = Flow_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = network.getNetWorkData()
                 result = {'status': 1, 'first': first, 'second': second}
             case _:
                 deviceId = d.getIdbyDevice(device, platform)
                 flow = Flow(pkgName=pkgname, deviceId=deviceId, platform=platform)
-                data = flow.getNetWorkData(wifi=wifi,useApi=False)
+                data = flow.getNetWorkData(wifi=wifi,noLog=False)
                 result = {'status': 1, 'upflow': data[0], 'downflow': data[1]}    
     except Exception:
         logger.error('get network data failed')
         traceback.print_exc()
         result = {'status': 1, 'upflow': 0, 'downflow': 0, 'first': 0, 'second': 0}    
     return result
 
@@ -302,14 +302,27 @@
                 'voltage': final[2], 
                 'power': final[3]}    
     except Exception:
         traceback.print_exc()
         result = {'status': 1, 'level': 0, 'temperature': 0, 'current':0, 'voltage':0 , 'power':0}
     return result
 
+@api.route('/apm/gpu', methods=['post', 'get'])
+def getGpu():
+    """get gpu data"""
+    pkgname = method._request(request, 'pkgname')
+    try:
+        gpu = GPU(pkgname=pkgname)
+        final = gpu.getGPU()
+        result = {'status': 1, 'gpu': final}
+    except Exception:
+        traceback.print_exc()
+        result = {'status': 1, 'gpu': 0}
+    return result
+
 
 @api.route('/apm/create/report', methods=['post', 'get'])
 def makeReport():
     """Create test report records"""
     current_time = time.strftime("%Y-%m-%d-%H-%M-%S", time.localtime())
     platform = method._request(request, 'platform')
     app = method._request(request, 'app')
@@ -372,15 +385,16 @@
     platform = method._request(request, 'platform')
     try:
         fucDic = {
             'cpu': f.getCpuLog(platform, scene),
             'mem': f.getMemLog(platform, scene),
             'battery': f.getBatteryLog(platform, scene),
             'flow': f.getFlowLog(platform, scene),
-            'fps': f.getFpsLog(platform, scene)
+            'fps': f.getFpsLog(platform, scene),
+            'gpu': f.getGpuLog(platform, scene)
         }
         result = fucDic[target]
     except Exception as e:
         result = {'status': 0, 'msg': str(e)}
     return result
 
 @api.route('/apm/log/pk', methods=['post', 'get'])
@@ -418,35 +432,42 @@
     deviceid = method._request(request, 'deviceid')
     pkgname = method._request(request, 'pkgname')
     target = method._request(request, 'target')
     try:
         match(target):
             case Target.CPU:
                 cpu = CPU(pkgName=pkgname, deviceId=deviceid, platform=platform)
-                appCpuRate, systemCpuRate = cpu.getCpuRate(useApi=True)
+                appCpuRate, systemCpuRate = cpu.getCpuRate(noLog=True)
                 result = {'status': 1, 'appCpuRate': appCpuRate, 'systemCpuRate': systemCpuRate}
             case Target.Memory:
                 mem = MEM(pkgName=pkgname, deviceId=deviceid, platform=platform)
-                totalPass, nativePass, dalvikPass = mem.getProcessMem(useApi=True)
+                totalPass, nativePass, dalvikPass = mem.getProcessMem(noLog=True)
                 result = {'status': 1, 'totalPass': totalPass, 'nativePass': nativePass, 'dalvikPass': dalvikPass}
             case Target.Network:
                 flow = Flow(pkgName=pkgname, deviceId=deviceid, platform=platform)
-                data = flow.getNetWorkData(wifi=True, useApi=True)
+                data = flow.getNetWorkData(wifi=True, noLog=True)
                 result = {'status': 1, 'upflow': data[0], 'downflow': data[1]}
             case Target.FPS:
                 fps_monitor = FPS(pkgName=pkgname, deviceId=deviceid, platform=platform)
-                fps, jank = fps_monitor.getFPS(useApi=True)
+                fps, jank = fps_monitor.getFPS(noLog=True)
                 result = {'status': 1, 'fps': fps, 'jank': jank}
             case Target.Battery:
                 battery_monitor = Battery(deviceId=deviceid)
-                final = battery_monitor.getBattery(useApi=True)
+                final = battery_monitor.getBattery(noLog=True)
                 if platform == 'Android':
                     result = {'status': 1, 'level': final[0], 'temperature': final[1]}
                 else:
-                    result = {'status': 1, 'temperature': final[0], 'current': final[1], 'voltage': final[2], 'power': final[3]} 
+                    result = {'status': 1, 'temperature': final[0], 'current': final[1], 'voltage': final[2], 'power': final[3]}
+            case Target.GPU:
+                if platform == Platform.iOS:
+                    gpu = GPU(pkgname=pkgname)
+                    final = gpu.getGPU()
+                    result = {'status': 1, 'gpu': final}
+                else:
+                    result = {'status': 0, 'msg': 'not support android'}    
             case _:
                 result = {'status': 0, 'msg': 'no this target'}
     except Exception as e:
         traceback.print_exc()
         result = {'status': 0, 'msg': str(e)}
     return result
```

### Comparing `solox-2.5.7/solox/view/pages.py` & `solox-2.5.8/solox/view/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     cpuWarning = (0, request.cookies.get('cpuWarning'))[request.cookies.get('cpuWarning') not in [None, 'NaN']]
     memWarning = (0, request.cookies.get('memWarning'))[request.cookies.get('memWarning') not in [None, 'NaN']]
     fpsWarning = (0, request.cookies.get('fpsWarning'))[request.cookies.get('fpsWarning') not in [None, 'NaN']]
     netdataRecvWarning = (0, request.cookies.get('netdataRecvWarning'))[request.cookies.get('netdataRecvWarning') not in [None, 'NaN']]
     netdataSendWarning = (0, request.cookies.get('netdataSendWarning'))[request.cookies.get('netdataSendWarning') not in [None, 'NaN']]
     betteryWarning = (0, request.cookies.get('betteryWarning'))[request.cookies.get('betteryWarning') not in [None, 'NaN']]
     runningTime = (0, request.cookies.get('runningTime'))[request.cookies.get('runningTime') not in [None, 'NaN']]
-    solox_host = request.cookies.get('solox_host')
+    solox_host = ('', request.cookies.get('solox_host'))[request.cookies.get('solox_host') not in [None, 'NaN']]
     host_switch = request.cookies.get('host_switch')
     return render_template('index.html', **locals())
 
 @page.route('/pk')
 def pk():
     lan = request.args.get('lan')
     model = request.args.get('model')
@@ -106,14 +106,15 @@
                     apm_data['batteryLevel'] = m._setValue(json_data['batteryLevel'])
                     apm_data['batteryTeml'] = m._setValue(json_data['batteryTeml'])
                 else:
                     apm_data['batteryTeml'] = m._setValue(json_data['batteryTeml'])
                     apm_data['batteryCurrent'] = m._setValue(json_data['batteryCurrent'])
                     apm_data['batteryVoltage'] = m._setValue(json_data['batteryVoltage'])
                     apm_data['batteryPower'] = m._setValue(json_data['batteryPower'])
+                    apm_data['gpu'] = m._setValue(json_data['gpu'])
                 f.close()
             except ZeroDivisionError:
                 pass    
             except Exception:
                 traceback.print_exc()
             finally:
                 break
```

### Comparing `solox-2.5.7/solox/web.py` & `solox-2.5.8/solox/web.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.7/solox.egg-info/PKG-INFO` & `solox-2.5.8/solox.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.5.7
+Version: 2.5.8
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -36,82 +36,90 @@
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
 ## Installation
+
 ```shell
-1.Python:3.10+ (Python 3.6 3.7 3.8 3.9 Please download a version of solox lower than 2.5.4)
+1.Python:3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
 2.pip install -U solox 
 3.pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox (China)
 
-notice: If Windows users need to test ios, install and start Itunes
+Note: If Windows users need to test ios, install and start Itunes
 ```
 
 ## Startup SoloX
+
 ### default
+
 ```shell
 python -m solox
 ```
+
 ### customize
 
 ```shell
 python -m solox --host={ip} --port={port}
 ```
 
-## Collect in python 
+## Collect in python
+
 ```python
 from solox.public.apm import APM
 # solox version >= 2.1.2
 
-apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True)
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
+# noLog : False (Save test data to log file)
 
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
 fps = apm.collectFps() # HZ
 battery = apm.collectBattery() # level:% temperature:°C current:mA voltage:mV power:w
 gpu = apm.collectGpu() # % only supports ios
 ```
 
-## Collect in API 
+## Collect in API
+
 ### Start the service in the background
 
 ```
 # solox version >= 2.1.5
 
 macOS/Linux: nohup python3 -m solox &
 Windows: start /min python3 -m solox &
 ```
 
 ### Request apm data from api
+
 ```shell
 Android: http://{ip}:{port}/apm/collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu
 
-target in ['cpu','memory','network','fps','battery']
+target in ['cpu','memory','network','fps','battery','gpu']
 ```
 
 ## PK Model
+
 - 2-devices: test the same app on two different phones
 - 2-apps: test two different apps on two phones with the same configuration
 
 notice: only supports android
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%">
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
 
 - windows: PowerShell
-- macOS：iTerm2 (https://iterm2.com/) 
+- macOS：iTerm2 (https://iterm2.com/)
 
 ## Thanks
 
 - https://github.com/alibaba/taobao-iphone-device
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solox Version: 2.5.7 Summary: SoloX - Real-time
+Metadata-Version: 2.1 Name: solox Version: 2.5.8 Summary: SoloX - Real-time
 collection tool for Android/iOS performance data. Home-page: https://
 github.com/smart-test-ti/SoloX Author: Rafa Chen Author-email:
 rafacheninc@gamil.com License: MIT Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE
                                English | ä¸­æ
@@ -10,35 +10,35 @@
 
             [solox_preview] [https://img.shields.io/pypi/dm/solox]
 ## Preview SoloX - Real-time collection tool for Android/iOS performance data.
 We are committed to solving inefficient, cumbersome test execution, and our
 goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/153412/
 1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
 process=image%2Fresize%2Cw_1500%2Climit_0] ## Installation ```shell 1.Python:
-3.10+ (Python 3.6 3.7 3.8 3.9 Please download a version of solox lower than
-2.5.4) 2.pip install -U solox 3.pip install -i https://mirrors.ustc.edu.cn/
-pypi/web/simple -U solox (China) notice: If Windows users need to test ios,
-install and start Itunes ``` ## Startup SoloX ### default ```shell python -
-m solox ``` ### customize ```shell python -m solox --host={ip} --port={port}
-``` ## Collect in python ```python from solox.public.apm import APM # solox
-version >= 2.1.2 apm = APM
-(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
-surfaceview=True) # apm = APM(pkgName='com.bilibili.app.in', platform='iOS')
-only supports one device # surfaceviewï¼ False = gfxinfo (Developer - GPU
-rendering mode - adb shell dumpsys gfxinfo) cpu = apm.collectCpu() # % memory =
+3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
+2.pip install -U solox 3.pip install -i https://mirrors.ustc.edu.cn/pypi/web/
+simple -U solox (China) Note: If Windows users need to test ios, install and
+start Itunes ``` ## Startup SoloX ### default ```shell python -m solox ``` ###
+customize ```shell python -m solox --host={ip} --port={port} ``` ## Collect in
+python ```python from solox.public.apm import APM # solox version >= 2.1.2 apm
+= APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
+surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
+platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
+(Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
+(Save test data to log file) cpu = apm.collectCpu() # % memory =
 apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
 apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
 current:mA voltage:mV power:w gpu = apm.collectGpu() # % only supports ios ```
 ## Collect in API ### Start the service in the background ``` # solox version
 >= 2.1.5 macOS/Linux: nohup python3 -m solox & Windows: start /min python3 -
 m solox & ``` ### Request apm data from api ```shell Android: http://{ip}:
 {port}/apm/
 collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/
 collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu target in
-['cpu','memory','network','fps','battery'] ``` ## PK Model - 2-devices: test
-the same app on two different phones - 2-apps: test two different apps on two
-phones with the same configuration notice: only supports android [https://
+['cpu','memory','network','fps','battery','gpu'] ``` ## PK Model - 2-devices:
+test the same app on two different phones - 2-apps: test two different apps on
+two phones with the same configuration notice: only supports android [https://
 cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-
 0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0] ## Browser
 [Chrome] ## Terminal - windows: PowerShell - macOSï¼iTerm2 (https://
 iterm2.com/) ## Thanks - https://github.com/alibaba/taobao-iphone-device
```

### Comparing `solox-2.5.7/solox.egg-info/SOURCES.txt` & `solox-2.5.8/solox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

