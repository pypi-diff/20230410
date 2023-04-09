# Comparing `tmp/roboweb_server-0.1.18.tar.gz` & `tmp/roboweb_server-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboweb_server-0.1.18.tar", last modified: Sun Apr  9 21:48:03 2023, max compression
+gzip compressed data, was "roboweb_server-0.1.19.tar", last modified: Sun Apr  9 22:08:52 2023, max compression
```

## Comparing `roboweb_server-0.1.18.tar` & `roboweb_server-0.1.19.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.805618 roboweb_server-0.1.18/
--rw-r--r--   0 hamel      (501) staff       (20)      115 2023-04-09 04:20:21.000000 roboweb_server-0.1.18/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-09 21:48:03.805351 roboweb_server-0.1.18/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      322 2023-04-09 03:10:44.000000 roboweb_server-0.1.18/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.781034 roboweb_server-0.1.18/roboweb_server/
--rw-r--r--   0 hamel      (501) staff       (20)       49 2023-04-09 03:10:44.000000 roboweb_server-0.1.18/roboweb_server/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     1031 2023-04-09 03:10:44.000000 roboweb_server-0.1.18/roboweb_server/ext.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.786099 roboweb_server-0.1.18/roboweb_server/static/
--rw-r--r--   0 hamel      (501) staff       (20)       32 2023-04-09 21:48:03.000000 roboweb_server-0.1.18/roboweb_server/static/.last_build_id
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.786849 roboweb_server-0.1.18/roboweb_server/static/assets/
--rw-r--r--   0 hamel      (501) staff       (20)     1487 2023-04-09 21:48:01.000000 roboweb_server-0.1.18/roboweb_server/static/assets/AssetManifest.bin
--rw-r--r--   0 hamel      (501) staff       (20)     2245 2023-04-09 21:48:01.000000 roboweb_server-0.1.18/roboweb_server/static/assets/AssetManifest.json
--rw-r--r--   0 hamel      (501) staff       (20)      544 2023-04-09 21:48:01.000000 roboweb_server-0.1.18/roboweb_server/static/assets/FontManifest.json
--rw-r--r--   0 hamel      (501) staff       (20)  1793816 2023-04-09 21:48:01.000000 roboweb_server-0.1.18/roboweb_server/static/assets/NOTICES
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.788335 roboweb_server-0.1.18/roboweb_server/static/assets/assets/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.788944 roboweb_server-0.1.18/roboweb_server/static/assets/assets/apps/
--rw-r--r--   0 hamel      (501) staff       (20)     4722 2023-04-09 03:10:44.000000 roboweb_server-0.1.18/roboweb_server/static/assets/assets/apps/firebase.webp
--rw-r--r--   0 hamel      (501) staff       (20)    16313 2023-04-09 03:10:44.000000 roboweb_server-0.1.18/roboweb_server/static/assets/assets/apps/gcloud.png
--rw-r--r--   0 hamel      (501) staff       (20)     7966 2023-04-09 03:10:44.000000 roboweb_server-0.1.18/roboweb_server/static/assets/assets/apps/github.png
--rw-r--r--   0 hamel      (501) staff       (20)    21222 2023-04-09 03:10:44.000000 roboweb_server-0.1.18/roboweb_server/static/assets/assets/jupyter.jpg
--rw-r--r--   0 hamel      (501) staff       (20)     1600 2023-04-09 03:10:44.000000 roboweb_server-0.1.18/roboweb_server/static/assets/assets/oauth2redirect.html
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.789119 roboweb_server-0.1.18/roboweb_server/static/assets/fonts/
--rw-r--r--   0 hamel      (501) staff       (20)     9492 2023-04-09 21:48:02.000000 roboweb_server-0.1.18/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.779461 roboweb_server-0.1.18/roboweb_server/static/assets/packages/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.779153 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.779205 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.789614 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.790117 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/
--rw-r--r--   0 hamel      (501) staff       (20)     1387 2023-04-05 04:39:17.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)     1696 2023-04-05 04:39:17.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)     1515 2023-04-05 04:39:17.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.790845 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/
--rw-r--r--   0 hamel      (501) staff       (20)     2059 2023-04-05 04:39:17.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)     2503 2023-04-05 04:39:17.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)     2224 2023-04-05 04:39:17.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png
--rw-r--r--   0 hamel      (501) staff       (20)      745 2023-04-05 04:39:17.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)      888 2023-04-05 04:39:17.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)      807 2023-04-05 04:39:17.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.779514 roboweb_server-0.1.18/roboweb_server/static/assets/packages/font_awesome_flutter/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.779567 roboweb_server-0.1.18/roboweb_server/static/assets/packages/font_awesome_flutter/lib/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.791750 roboweb_server-0.1.18/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/
--rw-r--r--   0 hamel      (501) staff       (20)   169440 2023-04-09 21:48:02.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
--rw-r--r--   0 hamel      (501) staff       (20)    48796 2023-04-09 21:48:02.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
--rw-r--r--   0 hamel      (501) staff       (20)   357436 2023-04-09 21:48:02.000000 roboweb_server-0.1.18/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.792138 roboweb_server-0.1.18/roboweb_server/static/assets/shaders/
--rw-r--r--   0 hamel      (501) staff       (20)     9242 2023-04-09 21:48:01.000000 roboweb_server-0.1.18/roboweb_server/static/assets/shaders/ink_sparkle.frag
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.801524 roboweb_server-0.1.18/roboweb_server/static/canvaskit/
--rw-r--r--   0 hamel      (501) staff       (20)    95983 2023-04-04 22:53:10.000000 roboweb_server-0.1.18/roboweb_server/static/canvaskit/canvaskit.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  6756109 2023-04-04 22:53:06.000000 roboweb_server-0.1.18/roboweb_server/static/canvaskit/canvaskit.wasm
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.801904 roboweb_server-0.1.18/roboweb_server/static/canvaskit/chromium/
--rw-r--r--   0 hamel      (501) staff       (20)    95628 2023-04-04 22:53:10.000000 roboweb_server-0.1.18/roboweb_server/static/canvaskit/chromium/canvaskit.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  5357473 2023-04-04 22:53:04.000000 roboweb_server-0.1.18/roboweb_server/static/canvaskit/chromium/canvaskit.wasm
--rw-r--r--   0 hamel      (501) staff       (20)    60828 2023-04-04 22:54:14.000000 roboweb_server-0.1.18/roboweb_server/static/canvaskit/skwasm.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  4505819 2023-04-04 22:54:08.000000 roboweb_server-0.1.18/roboweb_server/static/canvaskit/skwasm.wasm
--rw-r--r--   0 hamel      (501) staff       (20)     2744 2023-04-04 22:54:14.000000 roboweb_server-0.1.18/roboweb_server/static/canvaskit/skwasm.worker.js
--rw-r--r--   0 hamel      (501) staff       (20)    15406 2023-04-09 03:10:44.000000 roboweb_server-0.1.18/roboweb_server/static/favicon.ico
--rw-r--r--   0 hamel      (501) staff       (20)    14233 2023-04-09 21:48:03.000000 roboweb_server-0.1.18/roboweb_server/static/flutter.js
--rw-r--r--   0 hamel      (501) staff       (20)     9022 2023-04-09 21:48:03.000000 roboweb_server-0.1.18/roboweb_server/static/flutter_service_worker.js
--rw-r--r--   0 hamel      (501) staff       (20)     3188 2023-04-09 21:48:02.000000 roboweb_server-0.1.18/roboweb_server/static/index.html
--rw-r--r--   0 hamel      (501) staff       (20)  3945877 2023-04-09 21:48:03.000000 roboweb_server-0.1.18/roboweb_server/static/main.dart.js
--rw-r--r--   0 hamel      (501) staff       (20)       84 2023-04-09 21:48:01.000000 roboweb_server-0.1.18/roboweb_server/static/version.json
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 21:48:03.782463 roboweb_server-0.1.18/roboweb_server.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-09 21:48:03.000000 roboweb_server-0.1.18/roboweb_server.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2565 2023-04-09 21:48:03.000000 roboweb_server-0.1.18/roboweb_server.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 21:48:03.000000 roboweb_server-0.1.18/roboweb_server.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 04:03:36.000000 roboweb_server-0.1.18/roboweb_server.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-09 21:48:03.000000 roboweb_server-0.1.18/roboweb_server.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-09 21:48:03.000000 roboweb_server-0.1.18/roboweb_server.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      430 2023-04-09 21:47:36.000000 roboweb_server-0.1.18/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-09 21:48:03.805667 roboweb_server-0.1.18/setup.cfg
--rw-r--r--   0 hamel      (501) staff       (20)     2803 2023-04-09 03:48:53.000000 roboweb_server-0.1.18/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.340526 roboweb_server-0.1.19/
+-rw-r--r--   0 hamel      (501) staff       (20)      115 2023-04-09 04:20:21.000000 roboweb_server-0.1.19/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-09 22:08:52.340323 roboweb_server-0.1.19/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      322 2023-04-09 03:10:44.000000 roboweb_server-0.1.19/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.319417 roboweb_server-0.1.19/roboweb_server/
+-rw-r--r--   0 hamel      (501) staff       (20)       49 2023-04-09 03:10:44.000000 roboweb_server-0.1.19/roboweb_server/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1031 2023-04-09 03:10:44.000000 roboweb_server-0.1.19/roboweb_server/ext.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.323889 roboweb_server-0.1.19/roboweb_server/static/
+-rw-r--r--   0 hamel      (501) staff       (20)       32 2023-04-09 22:08:51.000000 roboweb_server-0.1.19/roboweb_server/static/.last_build_id
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.324674 roboweb_server-0.1.19/roboweb_server/static/assets/
+-rw-r--r--   0 hamel      (501) staff       (20)     1487 2023-04-09 22:08:50.000000 roboweb_server-0.1.19/roboweb_server/static/assets/AssetManifest.bin
+-rw-r--r--   0 hamel      (501) staff       (20)     2245 2023-04-09 22:08:50.000000 roboweb_server-0.1.19/roboweb_server/static/assets/AssetManifest.json
+-rw-r--r--   0 hamel      (501) staff       (20)      544 2023-04-09 22:08:50.000000 roboweb_server-0.1.19/roboweb_server/static/assets/FontManifest.json
+-rw-r--r--   0 hamel      (501) staff       (20)  1793816 2023-04-09 22:08:50.000000 roboweb_server-0.1.19/roboweb_server/static/assets/NOTICES
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.326002 roboweb_server-0.1.19/roboweb_server/static/assets/assets/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.326429 roboweb_server-0.1.19/roboweb_server/static/assets/assets/apps/
+-rw-r--r--   0 hamel      (501) staff       (20)     4722 2023-04-09 03:10:44.000000 roboweb_server-0.1.19/roboweb_server/static/assets/assets/apps/firebase.webp
+-rw-r--r--   0 hamel      (501) staff       (20)    16313 2023-04-09 03:10:44.000000 roboweb_server-0.1.19/roboweb_server/static/assets/assets/apps/gcloud.png
+-rw-r--r--   0 hamel      (501) staff       (20)     7966 2023-04-09 03:10:44.000000 roboweb_server-0.1.19/roboweb_server/static/assets/assets/apps/github.png
+-rw-r--r--   0 hamel      (501) staff       (20)    21222 2023-04-09 03:10:44.000000 roboweb_server-0.1.19/roboweb_server/static/assets/assets/jupyter.jpg
+-rw-r--r--   0 hamel      (501) staff       (20)     1600 2023-04-09 03:10:44.000000 roboweb_server-0.1.19/roboweb_server/static/assets/assets/oauth2redirect.html
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.326563 roboweb_server-0.1.19/roboweb_server/static/assets/fonts/
+-rw-r--r--   0 hamel      (501) staff       (20)     9492 2023-04-09 22:08:51.000000 roboweb_server-0.1.19/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.318045 roboweb_server-0.1.19/roboweb_server/static/assets/packages/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.317710 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.317771 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.327260 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.327817 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/
+-rw-r--r--   0 hamel      (501) staff       (20)     1387 2023-04-05 04:39:17.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)     1696 2023-04-05 04:39:17.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)     1515 2023-04-05 04:39:17.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.328329 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/
+-rw-r--r--   0 hamel      (501) staff       (20)     2059 2023-04-05 04:39:17.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)     2503 2023-04-05 04:39:17.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)     2224 2023-04-05 04:39:17.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png
+-rw-r--r--   0 hamel      (501) staff       (20)      745 2023-04-05 04:39:17.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)      888 2023-04-05 04:39:17.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)      807 2023-04-05 04:39:17.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.318103 roboweb_server-0.1.19/roboweb_server/static/assets/packages/font_awesome_flutter/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.318159 roboweb_server-0.1.19/roboweb_server/static/assets/packages/font_awesome_flutter/lib/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.328995 roboweb_server-0.1.19/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/
+-rw-r--r--   0 hamel      (501) staff       (20)   169440 2023-04-09 22:08:51.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
+-rw-r--r--   0 hamel      (501) staff       (20)    48796 2023-04-09 22:08:51.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
+-rw-r--r--   0 hamel      (501) staff       (20)   357436 2023-04-09 22:08:51.000000 roboweb_server-0.1.19/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.329374 roboweb_server-0.1.19/roboweb_server/static/assets/shaders/
+-rw-r--r--   0 hamel      (501) staff       (20)     9242 2023-04-09 22:08:50.000000 roboweb_server-0.1.19/roboweb_server/static/assets/shaders/ink_sparkle.frag
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.336812 roboweb_server-0.1.19/roboweb_server/static/canvaskit/
+-rw-r--r--   0 hamel      (501) staff       (20)    95983 2023-04-04 22:53:10.000000 roboweb_server-0.1.19/roboweb_server/static/canvaskit/canvaskit.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  6756109 2023-04-04 22:53:06.000000 roboweb_server-0.1.19/roboweb_server/static/canvaskit/canvaskit.wasm
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.337206 roboweb_server-0.1.19/roboweb_server/static/canvaskit/chromium/
+-rw-r--r--   0 hamel      (501) staff       (20)    95628 2023-04-04 22:53:10.000000 roboweb_server-0.1.19/roboweb_server/static/canvaskit/chromium/canvaskit.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  5357473 2023-04-04 22:53:04.000000 roboweb_server-0.1.19/roboweb_server/static/canvaskit/chromium/canvaskit.wasm
+-rw-r--r--   0 hamel      (501) staff       (20)    60828 2023-04-04 22:54:14.000000 roboweb_server-0.1.19/roboweb_server/static/canvaskit/skwasm.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  4505819 2023-04-04 22:54:08.000000 roboweb_server-0.1.19/roboweb_server/static/canvaskit/skwasm.wasm
+-rw-r--r--   0 hamel      (501) staff       (20)     2744 2023-04-04 22:54:14.000000 roboweb_server-0.1.19/roboweb_server/static/canvaskit/skwasm.worker.js
+-rw-r--r--   0 hamel      (501) staff       (20)    15406 2023-04-09 03:10:44.000000 roboweb_server-0.1.19/roboweb_server/static/favicon.ico
+-rw-r--r--   0 hamel      (501) staff       (20)    14233 2023-04-09 22:08:51.000000 roboweb_server-0.1.19/roboweb_server/static/flutter.js
+-rw-r--r--   0 hamel      (501) staff       (20)     9022 2023-04-09 22:08:51.000000 roboweb_server-0.1.19/roboweb_server/static/flutter_service_worker.js
+-rw-r--r--   0 hamel      (501) staff       (20)     3188 2023-04-09 22:08:51.000000 roboweb_server-0.1.19/roboweb_server/static/index.html
+-rw-r--r--   0 hamel      (501) staff       (20)  3945877 2023-04-09 22:08:51.000000 roboweb_server-0.1.19/roboweb_server/static/main.dart.js
+-rw-r--r--   0 hamel      (501) staff       (20)       84 2023-04-09 22:08:50.000000 roboweb_server-0.1.19/roboweb_server/static/version.json
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 22:08:52.320510 roboweb_server-0.1.19/roboweb_server.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-09 22:08:52.000000 roboweb_server-0.1.19/roboweb_server.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2565 2023-04-09 22:08:52.000000 roboweb_server-0.1.19/roboweb_server.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 22:08:52.000000 roboweb_server-0.1.19/roboweb_server.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 04:03:36.000000 roboweb_server-0.1.19/roboweb_server.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-09 22:08:52.000000 roboweb_server-0.1.19/roboweb_server.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-09 22:08:52.000000 roboweb_server-0.1.19/roboweb_server.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      430 2023-04-09 22:08:24.000000 roboweb_server-0.1.19/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-09 22:08:52.340577 roboweb_server-0.1.19/setup.cfg
+-rw-r--r--   0 hamel      (501) staff       (20)     2803 2023-04-09 03:48:53.000000 roboweb_server-0.1.19/setup.py
```

### Comparing `roboweb_server-0.1.18/PKG-INFO` & `roboweb_server-0.1.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboweb_server
-Version: 0.1.18
+Version: 0.1.19
 Summary: ChatGPT plugin for Jupyter Server
 Home-page: https://github.com/jlewi/roboweb
 Author: Jeremy Lewi
 Author-email: jeremy@lewi.us
 License: Apache Software License 2.0
 Keywords: gpt jupyter-server llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `roboweb_server-0.1.18/roboweb_server/ext.py` & `roboweb_server-0.1.19/roboweb_server/ext.py`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/AssetManifest.bin` & `roboweb_server-0.1.19/roboweb_server/static/assets/AssetManifest.bin`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/AssetManifest.json` & `roboweb_server-0.1.19/roboweb_server/static/assets/AssetManifest.json`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/FontManifest.json` & `roboweb_server-0.1.19/roboweb_server/static/assets/FontManifest.json`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/NOTICES` & `roboweb_server-0.1.19/roboweb_server/static/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/assets/apps/firebase.webp` & `roboweb_server-0.1.19/roboweb_server/static/assets/assets/apps/firebase.webp`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/assets/apps/gcloud.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/assets/apps/gcloud.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/assets/apps/github.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/assets/apps/github.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/assets/jupyter.jpg` & `roboweb_server-0.1.19/roboweb_server/static/assets/assets/jupyter.jpg`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/assets/oauth2redirect.html` & `roboweb_server-0.1.19/roboweb_server/static/assets/assets/oauth2redirect.html`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf` & `roboweb_server-0.1.19/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf` & `roboweb_server-0.1.19/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/assets/shaders/ink_sparkle.frag` & `roboweb_server-0.1.19/roboweb_server/static/assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/canvaskit/canvaskit.js` & `roboweb_server-0.1.19/roboweb_server/static/canvaskit/canvaskit.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/canvaskit/canvaskit.wasm` & `roboweb_server-0.1.19/roboweb_server/static/canvaskit/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/canvaskit/chromium/canvaskit.js` & `roboweb_server-0.1.19/roboweb_server/static/canvaskit/chromium/canvaskit.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/canvaskit/chromium/canvaskit.wasm` & `roboweb_server-0.1.19/roboweb_server/static/canvaskit/chromium/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/canvaskit/skwasm.js` & `roboweb_server-0.1.19/roboweb_server/static/canvaskit/skwasm.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/canvaskit/skwasm.wasm` & `roboweb_server-0.1.19/roboweb_server/static/canvaskit/skwasm.wasm`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/canvaskit/skwasm.worker.js` & `roboweb_server-0.1.19/roboweb_server/static/canvaskit/skwasm.worker.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/favicon.ico` & `roboweb_server-0.1.19/roboweb_server/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/flutter.js` & `roboweb_server-0.1.19/roboweb_server/static/flutter.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/flutter_service_worker.js` & `roboweb_server-0.1.19/roboweb_server/static/flutter_service_worker.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/index.html` & `roboweb_server-0.1.19/roboweb_server/static/index.html`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server/static/main.dart.js` & `roboweb_server-0.1.19/roboweb_server/static/main.dart.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/roboweb_server.egg-info/PKG-INFO` & `roboweb_server-0.1.19/roboweb_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboweb-server
-Version: 0.1.18
+Version: 0.1.19
 Summary: ChatGPT plugin for Jupyter Server
 Home-page: https://github.com/jlewi/roboweb
 Author: Jeremy Lewi
 Author-email: jeremy@lewi.us
 License: Apache Software License 2.0
 Keywords: gpt jupyter-server llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `roboweb_server-0.1.18/roboweb_server.egg-info/SOURCES.txt` & `roboweb_server-0.1.19/roboweb_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.18/setup.py` & `roboweb_server-0.1.19/setup.py`

 * *Files identical despite different names*

