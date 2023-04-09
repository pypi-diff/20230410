# Comparing `tmp/roboweb_server-0.1.22.tar.gz` & `tmp/roboweb_server-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboweb_server-0.1.22.tar", last modified: Sun Apr  9 22:45:13 2023, max compression
+gzip compressed data, was "roboweb_server-0.1.23.tar", last modified: Sun Apr  9 23:04:01 2023, max compression
```

## Comparing `roboweb_server-0.1.22.tar` & `roboweb_server-0.1.23.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.730466 roboweb_server-0.1.22/
--rw-r--r--   0 hamel      (501) staff       (20)      115 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-09 22:45:13.730264 roboweb_server-0.1.22/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      322 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.708564 roboweb_server-0.1.22/roboweb_server/
--rw-r--r--   0 hamel      (501) staff       (20)       49 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/roboweb_server/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     1031 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/roboweb_server/ext.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.712849 roboweb_server-0.1.22/roboweb_server/static/
--rw-r--r--   0 hamel      (501) staff       (20)       32 2023-04-09 22:45:13.000000 roboweb_server-0.1.22/roboweb_server/static/.last_build_id
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.713542 roboweb_server-0.1.22/roboweb_server/static/assets/
--rw-r--r--   0 hamel      (501) staff       (20)     1487 2023-04-09 22:45:11.000000 roboweb_server-0.1.22/roboweb_server/static/assets/AssetManifest.bin
--rw-r--r--   0 hamel      (501) staff       (20)     2245 2023-04-09 22:45:11.000000 roboweb_server-0.1.22/roboweb_server/static/assets/AssetManifest.json
--rw-r--r--   0 hamel      (501) staff       (20)      544 2023-04-09 22:45:11.000000 roboweb_server-0.1.22/roboweb_server/static/assets/FontManifest.json
--rw-r--r--   0 hamel      (501) staff       (20)  1793816 2023-04-09 22:45:11.000000 roboweb_server-0.1.22/roboweb_server/static/assets/NOTICES
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.714823 roboweb_server-0.1.22/roboweb_server/static/assets/assets/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.715247 roboweb_server-0.1.22/roboweb_server/static/assets/assets/apps/
--rw-r--r--   0 hamel      (501) staff       (20)     4722 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/roboweb_server/static/assets/assets/apps/firebase.webp
--rw-r--r--   0 hamel      (501) staff       (20)    16313 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/roboweb_server/static/assets/assets/apps/gcloud.png
--rw-r--r--   0 hamel      (501) staff       (20)     7966 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/roboweb_server/static/assets/assets/apps/github.png
--rw-r--r--   0 hamel      (501) staff       (20)    21222 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/roboweb_server/static/assets/assets/jupyter.jpg
--rw-r--r--   0 hamel      (501) staff       (20)     1600 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/roboweb_server/static/assets/assets/oauth2redirect.html
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.715383 roboweb_server-0.1.22/roboweb_server/static/assets/fonts/
--rw-r--r--   0 hamel      (501) staff       (20)     9492 2023-04-09 22:45:12.000000 roboweb_server-0.1.22/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.707153 roboweb_server-0.1.22/roboweb_server/static/assets/packages/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.706836 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.706896 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.715823 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.718319 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/
--rw-r--r--   0 hamel      (501) staff       (20)     1387 2023-04-05 04:39:17.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)     1696 2023-04-05 04:39:17.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)     1515 2023-04-05 04:39:17.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.718847 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/
--rw-r--r--   0 hamel      (501) staff       (20)     2059 2023-04-05 04:39:17.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)     2503 2023-04-05 04:39:17.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)     2224 2023-04-05 04:39:17.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png
--rw-r--r--   0 hamel      (501) staff       (20)      745 2023-04-05 04:39:17.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)      888 2023-04-05 04:39:17.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)      807 2023-04-05 04:39:17.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.707209 roboweb_server-0.1.22/roboweb_server/static/assets/packages/font_awesome_flutter/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.707269 roboweb_server-0.1.22/roboweb_server/static/assets/packages/font_awesome_flutter/lib/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.719478 roboweb_server-0.1.22/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/
--rw-r--r--   0 hamel      (501) staff       (20)   169440 2023-04-09 22:45:12.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
--rw-r--r--   0 hamel      (501) staff       (20)    48796 2023-04-09 22:45:12.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
--rw-r--r--   0 hamel      (501) staff       (20)   357436 2023-04-09 22:45:12.000000 roboweb_server-0.1.22/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.719857 roboweb_server-0.1.22/roboweb_server/static/assets/shaders/
--rw-r--r--   0 hamel      (501) staff       (20)     9242 2023-04-09 22:45:11.000000 roboweb_server-0.1.22/roboweb_server/static/assets/shaders/ink_sparkle.frag
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.726892 roboweb_server-0.1.22/roboweb_server/static/canvaskit/
--rw-r--r--   0 hamel      (501) staff       (20)    95983 2023-04-04 22:53:10.000000 roboweb_server-0.1.22/roboweb_server/static/canvaskit/canvaskit.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  6756109 2023-04-04 22:53:06.000000 roboweb_server-0.1.22/roboweb_server/static/canvaskit/canvaskit.wasm
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.727267 roboweb_server-0.1.22/roboweb_server/static/canvaskit/chromium/
--rw-r--r--   0 hamel      (501) staff       (20)    95628 2023-04-04 22:53:10.000000 roboweb_server-0.1.22/roboweb_server/static/canvaskit/chromium/canvaskit.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  5357473 2023-04-04 22:53:04.000000 roboweb_server-0.1.22/roboweb_server/static/canvaskit/chromium/canvaskit.wasm
--rw-r--r--   0 hamel      (501) staff       (20)    60828 2023-04-04 22:54:14.000000 roboweb_server-0.1.22/roboweb_server/static/canvaskit/skwasm.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  4505819 2023-04-04 22:54:08.000000 roboweb_server-0.1.22/roboweb_server/static/canvaskit/skwasm.wasm
--rw-r--r--   0 hamel      (501) staff       (20)     2744 2023-04-04 22:54:14.000000 roboweb_server-0.1.22/roboweb_server/static/canvaskit/skwasm.worker.js
--rw-r--r--   0 hamel      (501) staff       (20)    15406 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/roboweb_server/static/favicon.ico
--rw-r--r--   0 hamel      (501) staff       (20)    14233 2023-04-09 22:45:13.000000 roboweb_server-0.1.22/roboweb_server/static/flutter.js
--rw-r--r--   0 hamel      (501) staff       (20)     9022 2023-04-09 22:45:13.000000 roboweb_server-0.1.22/roboweb_server/static/flutter_service_worker.js
--rw-r--r--   0 hamel      (501) staff       (20)     3188 2023-04-09 22:45:12.000000 roboweb_server-0.1.22/roboweb_server/static/index.html
--rw-r--r--   0 hamel      (501) staff       (20)  3945877 2023-04-09 22:45:13.000000 roboweb_server-0.1.22/roboweb_server/static/main.dart.js
--rw-r--r--   0 hamel      (501) staff       (20)       84 2023-04-09 22:45:11.000000 roboweb_server-0.1.22/roboweb_server/static/version.json
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:45:13.709633 roboweb_server-0.1.22/roboweb_server.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-09 22:45:13.000000 roboweb_server-0.1.22/roboweb_server.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2565 2023-04-09 22:45:13.000000 roboweb_server-0.1.22/roboweb_server.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 22:45:13.000000 roboweb_server-0.1.22/roboweb_server.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 22:23:46.000000 roboweb_server-0.1.22/roboweb_server.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-09 22:45:13.000000 roboweb_server-0.1.22/roboweb_server.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-09 22:45:13.000000 roboweb_server-0.1.22/roboweb_server.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      430 2023-04-09 22:44:45.000000 roboweb_server-0.1.22/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-09 22:45:13.730519 roboweb_server-0.1.22/setup.cfg
--rw-r--r--   0 hamel      (501) staff       (20)     2803 2023-04-09 22:21:06.000000 roboweb_server-0.1.22/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.823323 roboweb_server-0.1.23/
+-rw-r--r--   0 hamel      (501) staff       (20)      115 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-09 23:04:01.823125 roboweb_server-0.1.23/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      322 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.802749 roboweb_server-0.1.23/roboweb_server/
+-rw-r--r--   0 hamel      (501) staff       (20)       49 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/roboweb_server/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1031 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/roboweb_server/ext.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.807693 roboweb_server-0.1.23/roboweb_server/static/
+-rw-r--r--   0 hamel      (501) staff       (20)       32 2023-04-09 23:03:56.000000 roboweb_server-0.1.23/roboweb_server/static/.last_build_id
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.808318 roboweb_server-0.1.23/roboweb_server/static/assets/
+-rw-r--r--   0 hamel      (501) staff       (20)     1487 2023-04-09 23:03:55.000000 roboweb_server-0.1.23/roboweb_server/static/assets/AssetManifest.bin
+-rw-r--r--   0 hamel      (501) staff       (20)     2245 2023-04-09 23:03:55.000000 roboweb_server-0.1.23/roboweb_server/static/assets/AssetManifest.json
+-rw-r--r--   0 hamel      (501) staff       (20)      544 2023-04-09 23:03:55.000000 roboweb_server-0.1.23/roboweb_server/static/assets/FontManifest.json
+-rw-r--r--   0 hamel      (501) staff       (20)  1793816 2023-04-09 23:03:55.000000 roboweb_server-0.1.23/roboweb_server/static/assets/NOTICES
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.809842 roboweb_server-0.1.23/roboweb_server/static/assets/assets/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.810299 roboweb_server-0.1.23/roboweb_server/static/assets/assets/apps/
+-rw-r--r--   0 hamel      (501) staff       (20)     4722 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/roboweb_server/static/assets/assets/apps/firebase.webp
+-rw-r--r--   0 hamel      (501) staff       (20)    16313 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/roboweb_server/static/assets/assets/apps/gcloud.png
+-rw-r--r--   0 hamel      (501) staff       (20)     7966 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/roboweb_server/static/assets/assets/apps/github.png
+-rw-r--r--   0 hamel      (501) staff       (20)    21222 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/roboweb_server/static/assets/assets/jupyter.jpg
+-rw-r--r--   0 hamel      (501) staff       (20)     1600 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/roboweb_server/static/assets/assets/oauth2redirect.html
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.810444 roboweb_server-0.1.23/roboweb_server/static/assets/fonts/
+-rw-r--r--   0 hamel      (501) staff       (20)     9492 2023-04-09 23:03:56.000000 roboweb_server-0.1.23/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.801231 roboweb_server-0.1.23/roboweb_server/static/assets/packages/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.800896 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.800956 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.810907 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.811340 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/
+-rw-r--r--   0 hamel      (501) staff       (20)     1387 2023-04-05 04:39:17.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)     1696 2023-04-05 04:39:17.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)     1515 2023-04-05 04:39:17.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.811797 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/
+-rw-r--r--   0 hamel      (501) staff       (20)     2059 2023-04-05 04:39:17.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)     2503 2023-04-05 04:39:17.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)     2224 2023-04-05 04:39:17.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png
+-rw-r--r--   0 hamel      (501) staff       (20)      745 2023-04-05 04:39:17.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)      888 2023-04-05 04:39:17.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)      807 2023-04-05 04:39:17.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.801287 roboweb_server-0.1.23/roboweb_server/static/assets/packages/font_awesome_flutter/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.801345 roboweb_server-0.1.23/roboweb_server/static/assets/packages/font_awesome_flutter/lib/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.812357 roboweb_server-0.1.23/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/
+-rw-r--r--   0 hamel      (501) staff       (20)   169440 2023-04-09 23:03:56.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
+-rw-r--r--   0 hamel      (501) staff       (20)    48796 2023-04-09 23:03:56.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
+-rw-r--r--   0 hamel      (501) staff       (20)   357436 2023-04-09 23:03:56.000000 roboweb_server-0.1.23/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.812710 roboweb_server-0.1.23/roboweb_server/static/assets/shaders/
+-rw-r--r--   0 hamel      (501) staff       (20)     9242 2023-04-09 23:03:55.000000 roboweb_server-0.1.23/roboweb_server/static/assets/shaders/ink_sparkle.frag
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.819612 roboweb_server-0.1.23/roboweb_server/static/canvaskit/
+-rw-r--r--   0 hamel      (501) staff       (20)    95983 2023-04-04 22:53:10.000000 roboweb_server-0.1.23/roboweb_server/static/canvaskit/canvaskit.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  6756109 2023-04-04 22:53:06.000000 roboweb_server-0.1.23/roboweb_server/static/canvaskit/canvaskit.wasm
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.819961 roboweb_server-0.1.23/roboweb_server/static/canvaskit/chromium/
+-rw-r--r--   0 hamel      (501) staff       (20)    95628 2023-04-04 22:53:10.000000 roboweb_server-0.1.23/roboweb_server/static/canvaskit/chromium/canvaskit.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  5357473 2023-04-04 22:53:04.000000 roboweb_server-0.1.23/roboweb_server/static/canvaskit/chromium/canvaskit.wasm
+-rw-r--r--   0 hamel      (501) staff       (20)    60828 2023-04-04 22:54:14.000000 roboweb_server-0.1.23/roboweb_server/static/canvaskit/skwasm.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  4505819 2023-04-04 22:54:08.000000 roboweb_server-0.1.23/roboweb_server/static/canvaskit/skwasm.wasm
+-rw-r--r--   0 hamel      (501) staff       (20)     2744 2023-04-04 22:54:14.000000 roboweb_server-0.1.23/roboweb_server/static/canvaskit/skwasm.worker.js
+-rw-r--r--   0 hamel      (501) staff       (20)    15406 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/roboweb_server/static/favicon.ico
+-rw-r--r--   0 hamel      (501) staff       (20)    14233 2023-04-09 23:03:56.000000 roboweb_server-0.1.23/roboweb_server/static/flutter.js
+-rw-r--r--   0 hamel      (501) staff       (20)     9022 2023-04-09 23:03:56.000000 roboweb_server-0.1.23/roboweb_server/static/flutter_service_worker.js
+-rw-r--r--   0 hamel      (501) staff       (20)     3188 2023-04-09 23:03:56.000000 roboweb_server-0.1.23/roboweb_server/static/index.html
+-rw-r--r--   0 hamel      (501) staff       (20)  3945877 2023-04-09 23:03:57.000000 roboweb_server-0.1.23/roboweb_server/static/main.dart.js
+-rw-r--r--   0 hamel      (501) staff       (20)       84 2023-04-09 23:03:55.000000 roboweb_server-0.1.23/roboweb_server/static/version.json
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 23:04:01.804440 roboweb_server-0.1.23/roboweb_server.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-09 23:04:01.000000 roboweb_server-0.1.23/roboweb_server.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2565 2023-04-09 23:04:01.000000 roboweb_server-0.1.23/roboweb_server.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 23:04:01.000000 roboweb_server-0.1.23/roboweb_server.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 22:23:46.000000 roboweb_server-0.1.23/roboweb_server.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-09 23:04:01.000000 roboweb_server-0.1.23/roboweb_server.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-09 23:04:01.000000 roboweb_server-0.1.23/roboweb_server.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      430 2023-04-09 23:03:25.000000 roboweb_server-0.1.23/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-09 23:04:01.823372 roboweb_server-0.1.23/setup.cfg
+-rw-r--r--   0 hamel      (501) staff       (20)     2803 2023-04-09 22:21:06.000000 roboweb_server-0.1.23/setup.py
```

### Comparing `roboweb_server-0.1.22/PKG-INFO` & `roboweb_server-0.1.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboweb_server
-Version: 0.1.22
+Version: 0.1.23
 Summary: ChatGPT plugin for Jupyter Server
 Home-page: https://github.com/jlewi/roboweb
 Author: Jeremy Lewi
 Author-email: jeremy@lewi.us
 License: Apache Software License 2.0
 Keywords: gpt jupyter-server llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `roboweb_server-0.1.22/roboweb_server/ext.py` & `roboweb_server-0.1.23/roboweb_server/ext.py`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/AssetManifest.bin` & `roboweb_server-0.1.23/roboweb_server/static/assets/AssetManifest.bin`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/AssetManifest.json` & `roboweb_server-0.1.23/roboweb_server/static/assets/AssetManifest.json`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/FontManifest.json` & `roboweb_server-0.1.23/roboweb_server/static/assets/FontManifest.json`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/NOTICES` & `roboweb_server-0.1.23/roboweb_server/static/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/assets/apps/firebase.webp` & `roboweb_server-0.1.23/roboweb_server/static/assets/assets/apps/firebase.webp`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/assets/apps/gcloud.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/assets/apps/gcloud.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/assets/apps/github.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/assets/apps/github.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/assets/jupyter.jpg` & `roboweb_server-0.1.23/roboweb_server/static/assets/assets/jupyter.jpg`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/assets/oauth2redirect.html` & `roboweb_server-0.1.23/roboweb_server/static/assets/assets/oauth2redirect.html`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf` & `roboweb_server-0.1.23/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf` & `roboweb_server-0.1.23/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/assets/shaders/ink_sparkle.frag` & `roboweb_server-0.1.23/roboweb_server/static/assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/canvaskit/canvaskit.js` & `roboweb_server-0.1.23/roboweb_server/static/canvaskit/canvaskit.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/canvaskit/canvaskit.wasm` & `roboweb_server-0.1.23/roboweb_server/static/canvaskit/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/canvaskit/chromium/canvaskit.js` & `roboweb_server-0.1.23/roboweb_server/static/canvaskit/chromium/canvaskit.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/canvaskit/chromium/canvaskit.wasm` & `roboweb_server-0.1.23/roboweb_server/static/canvaskit/chromium/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/canvaskit/skwasm.js` & `roboweb_server-0.1.23/roboweb_server/static/canvaskit/skwasm.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/canvaskit/skwasm.wasm` & `roboweb_server-0.1.23/roboweb_server/static/canvaskit/skwasm.wasm`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/canvaskit/skwasm.worker.js` & `roboweb_server-0.1.23/roboweb_server/static/canvaskit/skwasm.worker.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/favicon.ico` & `roboweb_server-0.1.23/roboweb_server/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/flutter.js` & `roboweb_server-0.1.23/roboweb_server/static/flutter.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/flutter_service_worker.js` & `roboweb_server-0.1.23/roboweb_server/static/flutter_service_worker.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/index.html` & `roboweb_server-0.1.23/roboweb_server/static/index.html`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server/static/main.dart.js` & `roboweb_server-0.1.23/roboweb_server/static/main.dart.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/roboweb_server.egg-info/PKG-INFO` & `roboweb_server-0.1.23/roboweb_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboweb-server
-Version: 0.1.22
+Version: 0.1.23
 Summary: ChatGPT plugin for Jupyter Server
 Home-page: https://github.com/jlewi/roboweb
 Author: Jeremy Lewi
 Author-email: jeremy@lewi.us
 License: Apache Software License 2.0
 Keywords: gpt jupyter-server llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `roboweb_server-0.1.22/roboweb_server.egg-info/SOURCES.txt` & `roboweb_server-0.1.23/roboweb_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.22/setup.py` & `roboweb_server-0.1.23/setup.py`

 * *Files identical despite different names*

