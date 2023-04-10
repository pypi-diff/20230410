# Comparing `tmp/feedcrawler-18.0.1.tar.gz` & `tmp/feedcrawler-18.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedcrawler-18.0.1.tar", last modified: Fri Apr  7 16:15:28 2023, max compression
+gzip compressed data, was "feedcrawler-18.0.2.tar", last modified: Mon Apr 10 12:23:28 2023, max compression
```

## Comparing `feedcrawler-18.0.1.tar` & `feedcrawler-18.0.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.326677 feedcrawler-18.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-07 16:15:28.326677 feedcrawler-18.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.314676 feedcrawler-18.0.1/feedcrawler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.314676 feedcrawler-18.0.1/feedcrawler/external_sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.314676 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45464 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.318676 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.318676 feedcrawler-18.0.1/feedcrawler/external_sites/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/metadata/imdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.318676 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_nx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/external_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42359 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/myjd_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/ombi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/overseerr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/plex_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/jobs/feed_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    20896 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/jobs/package_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    44933 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/myjd_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/url_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.310675 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.326677 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
--rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
--rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
--rw-r--r--   0 runner    (1001) docker     (123)   144621 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
--rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
--rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    82814 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.314676 feedcrawler-18.0.1/feedcrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:15:28.326677 feedcrawler-18.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.471537 feedcrawler-18.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-10 12:23:28.471537 feedcrawler-18.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.455536 feedcrawler-18.0.2/feedcrawler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler/external_sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20331 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler/external_sites/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/metadata/imdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.463537 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.463537 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_nx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.463537 feedcrawler-18.0.2/feedcrawler/external_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42357 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/myjd_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/ombi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/overseerr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/plex_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.463537 feedcrawler-18.0.2/feedcrawler/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15020 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/jobs/feed_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20797 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/jobs/package_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.467537 feedcrawler-18.0.2/feedcrawler/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.467537 feedcrawler-18.0.2/feedcrawler/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46194 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/myjd_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/url_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.467537 feedcrawler-18.0.2/feedcrawler/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.455536 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.467537 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.471537 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
+-rw-r--r--   0 runner    (1001) docker     (123)   144621 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-10 12:23:27.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    83010 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:23:28.471537 feedcrawler-18.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/setup.py
```

### Comparing `feedcrawler-18.0.1/LICENSE.md` & `feedcrawler-18.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/PKG-INFO` & `feedcrawler-18.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.1
+Version: 18.0.2
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedcrawler-18.0.1/README.md` & `feedcrawler-18.0.2/README.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/crawler.py` & `feedcrawler-18.0.2/feedcrawler/crawler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,177 +1,175 @@
 # -*- coding: utf-8 -*-
 # FeedCrawler
 # Projekt von https://github.com/rix1337
 # Dieses Modul initialisiert die globalen Parameter und starte alle parallel laufenden Threads des FeedCrawlers.
 
 import argparse
-import ctypes
 import logging
 import multiprocessing
 import os
 import re
 import signal
 import sys
 import time
 
-from feedcrawler.jobs.feed_search import crawler
+from feedcrawler.jobs.feed_search import feed_crawler
 from feedcrawler.jobs.package_watcher import watch_packages
 from feedcrawler.providers import gui
 from feedcrawler.providers import shared_state
 from feedcrawler.providers import version
 from feedcrawler.providers.common_functions import Unbuffered, check_ip, configpath
 from feedcrawler.providers.config import CrawlerConfig
-from feedcrawler.providers.myjd_connection import get_device, get_if_one_device, myjd_input
+from feedcrawler.providers.myjd_connection import set_device_from_config, get_if_one_device, myjd_input
 from feedcrawler.providers.sqlite_database import FeedDb, remove_redundant_db_tables
 from feedcrawler.web_interface.web_server import web_server
 
 version = "v." + version.get_version()
 
 
 def start_feedcrawler():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--log-level", help="Legt fest, wie genau geloggt wird (INFO, DEBUG)")
-    parser.add_argument("--config", help="Legt den Ablageort für Einstellungen und Logs fest")
-    parser.add_argument("--port", help="Legt den Port des Webservers fest")
-    parser.add_argument("--jd-user", help="Legt den Nutzernamen für My JDownloader fest")
-    parser.add_argument("--jd-pass", help="Legt das Passwort für My JDownloader fest")
-    parser.add_argument("--jd-device", help="Legt den Gerätenamen für My JDownloader fest")
-    parser.add_argument("--delay", help="Verzögere Suchlauf nach Start um ganze Zahl in Sekunden")
-    parser.add_argument("--keep-cdc", action='store_true',
-                        help="Intern: Vergisst 'Feed ab hier bereits gecrawlt' nicht vor dem ersten Suchlauf")
-    parser.add_argument("--remove_cloudflare_time", action='store_true',
-                        help="Intern: Leere die Zeit des letzten Cloudflare-Umgehungs-Laufes vor dem ersten Suchlauf")
-    parser.add_argument("--test_run", action='store_true', help="Intern: Führt einen Testlauf durch")
-    parser.add_argument("--docker", action='store_true', help="Intern: Sperre Pfad und Port auf Docker-Standardwerte")
-    arguments = parser.parse_args()
-
-    if gui.enabled:
-        print_mem_size = 1024 * 1024  # 1 MB should handle very large print statements
-        shared_print_mem = multiprocessing.Array(ctypes.c_char, print_mem_size)
-        window = gui.create_main_window()
-        sys.stdout = gui.PrintToConsoleAndGui(window)
-    else:
-        shared_print_mem = False
-        window = False
-        sys.stdout = Unbuffered(sys.stdout)
-
-    print(u"┌──────────────────────────────────────────────┐")
-    print(u"  FeedCrawler " + version + " von RiX")
-    print(u"  https://github.com/rix1337/FeedCrawler")
-    print(u"└──────────────────────────────────────────────┘")
-
-    if arguments.docker:
-        config_path = "/config"
-    else:
-        config_path = configpath(arguments.config)
-
-    shared_state.set_files(config_path)
-
-    print(u'Nutze das Verzeichnis "' + config_path + u'" für Einstellungen/Logs')
-
-    log_level = logging.__dict__[
-        arguments.log_level] if arguments.log_level in logging.__dict__ else logging.INFO
-
-    shared_state.set_logger(log_level)
-
-    hostnames = CrawlerConfig('Hostnames')
-
-    def clean_up_hostname(host, string):
-        if string and '/' in string:
-            string = string.replace('https://', '').replace('http://', '')
-            string = re.findall(r'([a-z-.]*\.[a-z]*)', string)[0]
-            hostnames.save(host, string)
-        if string and re.match(r'.*[A-Z].*', string):
-            hostnames.save(host, string.lower())
-        if string:
-            print(u'Hostname für ' + host.upper() + ": " + string)
+    with multiprocessing.Manager() as manager:
+        shared_state_dict = manager.dict()
+        shared_state.set_shared_dict(shared_state_dict)
+
+        if gui.enabled:
+            window = gui.create_main_window()
+            sys.stdout = gui.PrintToConsoleAndGui(window)
         else:
-            print(u'Hostname für ' + host.upper() + ': -')
-        return string
+            window = False
+            sys.stdout = Unbuffered(sys.stdout)
 
-    set_hostnames = {}
-    shared_state.set_sites()
-    for name in shared_state.sites:
-        name = name.lower()
-        hostname = clean_up_hostname(name, hostnames.get(name))
-        if hostname:
-            set_hostnames[name] = hostname
+        parser = argparse.ArgumentParser()
+        parser.add_argument("--log-level", help="Legt fest, wie genau geloggt wird (INFO, DEBUG)")
+        parser.add_argument("--config", help="Legt den Ablageort für Einstellungen und Logs fest")
+        parser.add_argument("--port", help="Legt den Port des Webservers fest")
+        parser.add_argument("--jd-user", help="Legt den Nutzernamen für My JDownloader fest")
+        parser.add_argument("--jd-pass", help="Legt das Passwort für My JDownloader fest")
+        parser.add_argument("--jd-device", help="Legt den Gerätenamen für My JDownloader fest")
+        parser.add_argument("--delay", help="Verzögere Suchlauf nach Start um ganze Zahl in Sekunden")
+        parser.add_argument("--keep-cdc", action='store_true',
+                            help="Intern: Vergisst 'Feed ab hier bereits gecrawlt' nicht vor dem ersten Suchlauf")
+        parser.add_argument("--remove_cloudflare_time", action='store_true',
+                            help="Intern: Leere die Zeit des letzten Cloudflare-Umgehungs-Laufes vor dem ersten Suchlauf")
+        parser.add_argument("--test_run", action='store_true', help="Intern: Führt einen Testlauf durch")
+        parser.add_argument("--docker", action='store_true',
+                            help="Intern: Sperre Pfad und Port auf Docker-Standardwerte")
+        arguments = parser.parse_args()
+
+        shared_state.set_initial_values(arguments.test_run, arguments.remove_cloudflare_time)
+
+        print("┌──────────────────────────────────────────────┐")
+        print("  FeedCrawler " + version + " von RiX")
+        print("  https://github.com/rix1337/FeedCrawler")
+        print("└──────────────────────────────────────────────┘")
 
-    if not arguments.test_run and not set_hostnames:
-        if gui.enabled:
-            gui.no_hostnames_gui(shared_state.configfile)
+        if arguments.docker:
+            config_path = "/config"
         else:
-            print(u'Keine Hostnamen in der FeedCrawler.ini gefunden! Beende FeedCrawler!')
-            time.sleep(10)
-        sys.exit(1)
-
-    device_mem_size = 8 * 1024  # 0.008 MB is eight times the size of pickled device objects
-    shared_device_mem = multiprocessing.Array(ctypes.c_char, device_mem_size)
-    shared_state.set_device_memory(shared_device_mem)
+            config_path = configpath(arguments.config)
 
-    with multiprocessing.Manager() as manager:
-        shared_request_dict = manager.dict()
+        shared_state.set_files(config_path)
+
+        print('Nutze das Verzeichnis "' + config_path + '" für Einstellungen/Logs')
+
+        log_level = logging.__dict__[
+            arguments.log_level] if arguments.log_level in logging.__dict__ else logging.INFO
 
-        if not arguments.test_run:
-            if not os.path.exists(shared_state.configfile):
+        shared_state.set_log_level(log_level)
+        shared_state.set_logger()
+
+        hostnames = CrawlerConfig('Hostnames')
+
+        def clean_up_hostname(host, string):
+            if string and '/' in string:
+                string = string.replace('https://', '').replace('http://', '')
+                string = re.findall(r'([a-z-.]*\.[a-z]*)', string)[0]
+                hostnames.save(host, string)
+            if string and re.match(r'.*[A-Z].*', string):
+                hostnames.save(host, string.lower())
+            if string:
+                print('Hostname für ' + host.upper() + ": " + string)
+            else:
+                print('Hostname für ' + host.upper() + ': -')
+            return string
+
+        set_hostnames = {}
+        shared_state.set_sites()
+        for name in shared_state.values["sites"]:
+            name = name.lower()
+            hostname = clean_up_hostname(name, hostnames.get(name))
+            if hostname:
+                set_hostnames[name] = hostname
+
+        if not shared_state.values["test_run"] and not set_hostnames:
+            if gui.enabled:
+                gui.no_hostnames_gui(shared_state.values["configfile"])
+            else:
+                print('Keine Hostnamen in der FeedCrawler.ini gefunden! Beende FeedCrawler!')
+                time.sleep(10)
+            sys.exit(1)
+
+        if not shared_state.values["test_run"]:
+            if not os.path.exists(shared_state.values["configfile"]):
                 if arguments.docker:
                     if arguments.jd_user and arguments.jd_pass:
                         myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass, arguments.jd_device)
                 else:
                     myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass, arguments.jd_device)
             else:
                 feedcrawler = CrawlerConfig('FeedCrawler')
                 user = feedcrawler.get('myjd_user')
                 password = feedcrawler.get('myjd_pass')
                 if user and password:
-                    if not get_device():
+                    if not set_device_from_config():
                         device_set = feedcrawler.get('myjd_device')
                         if not device_set:
                             one_device = get_if_one_device(user, password)
                             if one_device:
-                                print(u'Gerätename "' + one_device + '" automatisch ermittelt.')
+                                print('Gerätename "' + one_device + '" automatisch ermittelt.')
                                 feedcrawler.save('myjd_device', one_device)
-                                get_device()
+                                set_device_from_config()
                 else:
                     myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass,
                                arguments.jd_device)
 
-        if not arguments.test_run:
-            if shared_state.device and shared_state.device.name:
+        if not shared_state.values["test_run"]:
+            if shared_state.values["device"] and shared_state.values["device"].name:
                 success = True
             else:
                 success = False
                 feedcrawler = CrawlerConfig('FeedCrawler')
 
                 device_name = feedcrawler.get('myjd_device')
                 if not device_name:
                     user = feedcrawler.get('myjd_user')
                     password = feedcrawler.get('myjd_pass')
                     one_device = get_if_one_device(user, password)
                     if one_device:
-                        print(u'Gerätename "' + one_device + '" automatisch ermittelt.')
+                        print('Gerätename "' + one_device + '" automatisch ermittelt.')
                         feedcrawler.save('myjd_device', one_device)
-                        get_device()
-                        success = shared_state.device and shared_state.device.name
+                        set_device_from_config()
+                        success = shared_state.values["device"] and shared_state.values["device"].name
                 if not success:
                     i = 0
                     while i < 10:
                         i += 1
                         print(
-                            u'Verbindungsversuch %s mit My JDownloader gescheitert. Gerätename: "%s"' % (
+                            'Verbindungsversuch %s mit My JDownloader gescheitert. Gerätename: "%s"' % (
                                 i, device_name))
                         time.sleep(60)
-                        get_device()
-                        success = shared_state.device and shared_state.device.name
+                        set_device_from_config()
+                        success = shared_state.values["device"] and shared_state.values["device"].name
                         if success:
                             break
             if success:
-                print(u'Erfolgreich mit My JDownloader verbunden. Gerätename: "' + shared_state.device.name + '"')
+                print('Erfolgreich mit My JDownloader verbunden. Gerätename: "' + shared_state.values[
+                    "device"].name + '"')
             else:
-                print(u'My JDownloader Zugangsversuche nicht erfolgreich! Beende FeedCrawler!')
+                print('My JDownloader Zugangsversuche nicht erfolgreich! Beende FeedCrawler!')
                 sys.exit(1)
 
         feedcrawler = CrawlerConfig('FeedCrawler')
         port = int(feedcrawler.get("port"))
         docker = False
         if arguments.docker:
             port = int('9090')
@@ -181,78 +179,66 @@
 
         if feedcrawler.get("prefix"):
             prefix = '/' + feedcrawler.get("prefix")
         else:
             prefix = ''
         local_address = 'http://' + check_ip() + ':' + str(port) + prefix
         if not arguments.docker:
-            print(u'Der Webserver ist erreichbar unter "' + local_address + u'"')
+            print('Der Webserver ist erreichbar unter "' + local_address + '"')
 
         shared_state.set_connection_info(local_address, port, prefix, docker)
 
         CrawlerConfig("FeedCrawler").remove_redundant_entries()
-        remove_redundant_db_tables(shared_state.dbfile)
+        remove_redundant_db_tables(shared_state.values["dbfile"])
 
         if arguments.keep_cdc:
-            print(u"CDC-Tabelle nicht geleert!")
+            print("CDC-Tabelle nicht geleert!")
         else:
             FeedDb('cdc').reset()
 
-        global_variables = shared_state.get_globals()
-
-        process_web_server = multiprocessing.Process(target=web_server,
-                                                     args=(shared_print_mem, global_variables, shared_request_dict,
-                                                           shared_device_mem,))
+        process_web_server = multiprocessing.Process(target=web_server, args=(shared_state_dict,))
         process_web_server.start()
 
         if arguments.delay:
             delay = int(arguments.delay)
-            print(u"Verzögere den ersten Suchlauf um " + str(delay) + u" Sekunden")
+            print("Verzögere den ersten Suchlauf um " + str(delay) + " Sekunden")
             time.sleep(delay)
 
-        if not arguments.test_run:
-            process_crawler = multiprocessing.Process(target=crawler,
-                                                      args=(shared_print_mem, global_variables, shared_request_dict,
-                                                            shared_device_mem,
-                                                            arguments.remove_cloudflare_time, False,))
-            process_crawler.start()
-
-            process_watch_packages = multiprocessing.Process(target=watch_packages,
-                                                             args=(
-                                                                 shared_print_mem, global_variables,
-                                                                 shared_request_dict,
-                                                                 shared_device_mem,))
+        if not shared_state.values["test_run"]:
+            process_feed_crawler = multiprocessing.Process(target=feed_crawler, args=(shared_state_dict,))
+            process_feed_crawler.start()
+
+            process_watch_packages = multiprocessing.Process(target=watch_packages, args=(shared_state_dict,))
             process_watch_packages.start()
 
             if not arguments.docker and gui.enabled:
-                gui.main_gui(window, shared_print_mem)
+                gui.main_gui(window, shared_state_dict)
 
                 sys.stdout = sys.__stdout__
                 process_web_server.terminate()
-                process_crawler.terminate()
+                process_feed_crawler.terminate()
                 process_watch_packages.terminate()
                 sys.exit(0)
 
             else:  # regular console
                 def signal_handler(sig, frame):
                     process_web_server.terminate()
-                    process_crawler.terminate()
+                    process_feed_crawler.terminate()
                     process_watch_packages.terminate()
                     sys.exit(0)
 
                 signal.signal(signal.SIGINT, signal_handler)
-                print(u'Drücke [Strg] + [C] zum Beenden')
+                print('Drücke [Strg] + [C] zum Beenden')
                 try:
                     while True:
                         signal.pause()
                 except AttributeError:
                     while True:
                         time.sleep(1)
         else:
-            crawler(shared_print_mem, global_variables, shared_request_dict, shared_device_mem,
-                    arguments.remove_cloudflare_time, True)
+            feed_crawler(shared_state_dict)
             process_web_server.terminate()
             sys.exit(0)
 
 
 if __name__ == "__main__":
     start_feedcrawler()
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/content_all.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/content_all.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,25 +92,23 @@
         if content:
             if "mkv" in content.lower():
                 hevc_retail = False
                 storage = self.db.retrieve_all(post.title)
                 storage_replaced = self.db.retrieve_all(
                     post.title.replace(".COMPLETE", "").replace(".Complete", ""))
                 if 'added' in storage or 'notdl' in storage or 'added' in storage_replaced or 'notdl' in storage_replaced:
-                    shared_state.logger.debug(
-                        "%s - Release ignoriert (bereits gefunden)" % post.title)
+                    shared_state.logger.debug("%s - Release ignoriert (bereits gefunden)" % post.title)
                     continue
                 elif not check_valid_release(post.title, self.retail_only, self.hevc_retail):
                     shared_state.logger.debug(
                         "%s - Release ignoriert (Gleiche oder bessere Quelle bereits vorhanden)" % post.title)
                     continue
                 quality_set = self.config.get('quality')
                 if '.3d.' in post.title.lower():
-                    shared_state.logger.debug(
-                        "%s - Release ignoriert (3D-Film)" % post.title)
+                    shared_state.logger.debug("%s - Release ignoriert (3D-Film)" % post.title)
                     return
                 else:
                     if quality_set == "480p":
                         if "720p" in post.title.lower() or "1080p" in post.title.lower() or "1080i" in post.title.lower() or "2160p" in post.title.lower():
                             quality_match = False
                         else:
                             quality_match = True
@@ -122,63 +120,56 @@
                             if is_hevc(post.title) and "1080p" in post.title:
                                 if is_retail(post.title, False):
                                     shared_state.logger.debug(
                                         "%s - Qualität ignoriert (Release ist 1080p-HEVC-Retail)" % post.title)
                                     hevc_retail = True
                                     quality_match = True
                     if not quality_match:
-                        shared_state.logger.debug(
-                            "%s - Release ignoriert (falsche Auflösung)" % post.title)
+                        shared_state.logger.debug("%s - Release ignoriert (falsche Auflösung)" % post.title)
                         continue
 
                 found = check_is_ignored(post.title, self.config.get("ignore"))
                 if found:
                     if self.hevc_retail:
                         if is_hevc(post.title) and "1080p" in post.title:
                             if is_retail(post.title, False):
                                 shared_state.logger.debug(
                                     "%s - Filterliste ignoriert (Release ist 1080p-HEVC-Retail)" % post.title)
                                 hevc_retail = True
                                 found = False
                 if found:
-                    shared_state.logger.debug(
-                        "%s - Release ignoriert (aufgrund der Filterliste)" % post.title)
+                    shared_state.logger.debug("%s - Release ignoriert (aufgrund der Filterliste)" % post.title)
                     continue
                 if self.feedcrawler.get("surround"):
                     if not re.match(r'.*\.(DTS|DD\+*51|DD\+*71|AC3\.5\.*1)\..*', post.title):
-                        shared_state.logger.debug(
-                            post.title + " - Release ignoriert (kein Mehrkanalton)")
+                        shared_state.logger.debug(post.title + " - Release ignoriert (kein Mehrkanalton)")
                         continue
                 season = re.search(r'\.S(\d{1,3})(\.|-|E)', post.title)
                 if season:
-                    shared_state.logger.debug(
-                        "%s - Release ignoriert (IMDb sucht nur Filme)" % post.title)
+                    shared_state.logger.debug("%s - Release ignoriert (IMDb sucht nur Filme)" % post.title)
                     continue
 
                 if post.imdb_id:
                     min_year = int(self.config.get("imdbyear"))
                     if min_year:
                         year = get_year(post.imdb_id)
                         if year:
                             if year < min_year:
-                                shared_state.logger.debug(
-                                    "%s - Release ignoriert (Film zu alt)" % post.title)
+                                shared_state.logger.debug("%s - Release ignoriert (Film zu alt)" % post.title)
                                 continue
                         else:
                             shared_state.logger.debug("%s - Release ignoriert (Alter nicht ermittelbar)" % post.title)
                             continue
                     votes = get_votes(post.imdb_id)
                     if votes:
                         if votes < 1500:
-                            shared_state.logger.debug(
-                                post.title + " - Release ignoriert (Weniger als 1500 IMDb-Votes)")
+                            shared_state.logger.debug(post.title + " - Release ignoriert (Weniger als 1500 IMDb-Votes)")
                             continue
                     else:
-                        shared_state.logger.debug(
-                            post.title + " - Release ignoriert (Konnte keine IMDb-Votes finden)")
+                        shared_state.logger.debug(post.title + " - Release ignoriert (Konnte keine IMDb-Votes finden)")
                         continue
                     rating = get_rating(post.imdb_id)
                     if rating and rating > desired_rating:
                         download_method = self.download_method
                         download_links = self.get_download_links_method(self, content, post.title)
                         if check_fallback_required(download_links):
                             download_method = add_decrypt_instead_of_download
@@ -241,21 +232,19 @@
                             if is_hevc(post.title) and "1080p" in post.title:
                                 if is_retail(post.title, False):
                                     shared_state.logger.debug(
                                         "%s - Filterliste ignoriert (Release ist 1080p-HEVC-Retail)" % post.title)
                                     hevc_retail = True
                                     found = False
                     if found:
-                        shared_state.logger.debug(
-                            "%s - Release ignoriert (aufgrund der Filterliste)" % post.title)
+                        shared_state.logger.debug("%s - Release ignoriert (aufgrund der Filterliste)" % post.title)
                         continue
                     if self.feedcrawler.get("surround"):
                         if not re.match(r'.*\.(DTS|DD\+*51|DD\+*71|AC3\.5\.*1)\..*', post.title):
-                            shared_state.logger.debug(
-                                post.title + " - Release ignoriert (kein Mehrkanalton)")
+                            shared_state.logger.debug(post.title + " - Release ignoriert (kein Mehrkanalton)")
                             continue
                     if self.filename == 'List_ContentAll_Seasons':
                         ss = self.config.get('seasonsquality')
                     elif 'Regex' not in self.filename:
                         ss = self.config.get('quality')
                     else:
                         ss = False
@@ -274,45 +263,40 @@
                                             "%s  - Qualität ignoriert (Release ist 1080p-HEVC-Retail)" % post.title)
                                         hevc_retail = True
                                         found = True
                         if found:
                             episode = re.search(
                                 r'([\w\.\s]*s\d{1,2}e\d{1,2})[\w\.\s]*', post.title.lower())
                             if episode:
-                                shared_state.logger.debug(
-                                    "%s - Release ignoriert (Serienepisode)" % post.title)
+                                shared_state.logger.debug("%s - Release ignoriert (Serienepisode)" % post.title)
                                 continue
                             found = download_feed(self, post.title, content, post.source, post.imdb_id, post.size,
                                                   hevc_retail)
                             if found:
                                 for i in found:
                                     added_items.append(i)
                     elif self.filename == 'List_ContentAll_Seasons':
                         validsource = re.search(self.config.get(
                             "seasonssource"), post.title.lower())
                         if not validsource:
-                            shared_state.logger.debug(
-                                post.title + " - Release hat falsche Quelle")
+                            shared_state.logger.debug(post.title + " - Release hat falsche Quelle")
                             continue
                         if ".complete." not in post.title.lower():
                             if "FX" not in self._SITE and "DW" not in self._SITE:
-                                shared_state.logger.debug(
-                                    post.title + " - Staffel noch nicht komplett")
+                                shared_state.logger.debug(post.title + " - Staffel noch nicht komplett")
                                 continue
                         season = re.search(r"\.s\d", post.title.lower())
                         if not season:
-                            shared_state.logger.debug(
-                                post.title + " - Release ist keine Staffel")
+                            shared_state.logger.debug(post.title + " - Release ist keine Staffel")
                             continue
                         if not self.config.get("seasonpacks"):
                             staffelpack = re.search(
                                 r"s\d.*(-|\.).*s\d", post.title.lower())
                             if staffelpack:
-                                shared_state.logger.debug(
-                                    "%s - Release ignoriert (Staffelpaket)" % post.title)
+                                shared_state.logger.debug("%s - Release ignoriert (Staffelpaket)" % post.title)
                                 continue
                         if self.filename == 'List_ContentAll_Seasons':
                             ss = self.config.get('seasonsquality')
                         elif 'Regex' not in self.filename:
                             ss = self.config.get('quality')
                         else:
                             ss = False
@@ -322,16 +306,15 @@
                             found = True
                         else:
                             found = re.search(ss, post.title.lower())
                         if found:
                             episode = re.search(
                                 r'([\w\.\s]*s\d{1,2}e\d{1,2})[\w\.\s]*', post.title.lower())
                             if episode:
-                                shared_state.logger.debug(
-                                    "%s - Release ignoriert (Serienepisode)" % post.title)
+                                shared_state.logger.debug("%s - Release ignoriert (Serienepisode)" % post.title)
                                 continue
                             found = download_feed(self, post.title, content, post.source, post.imdb_id, post.size,
                                                   hevc_retail)
                             if found:
                                 for i in found:
                                     added_items.append(i)
                     else:
@@ -376,50 +359,46 @@
             elif site == "NK":
                 get_download_links_method = content_all_nk.nk_page_download_link
                 download_method = myjd_download
             else:
                 continue
 
             if original_imdb_id and imdb_id and imdb_id != original_imdb_id:
-                shared_state.logger.debug(
-                    "%s - Abweichende IMDb-IDs identifiziert! Breche ab." % key)
+                shared_state.logger.debug("%s - Abweichende IMDb-IDs identifiziert! Breche ab." % key)
                 continue
 
             if is_hevc(key) and "1080p" in key:
                 download_links = get_download_links_method(self, link, key)
                 if check_fallback_required(download_links):
                     download_method = add_decrypt_instead_of_download
                 if download_links:
                     storage = self.db.retrieve_all(key)
                     storage_replaced = self.db.retrieve_all(key.replace(".COMPLETE", "").replace(".Complete", ""))
                     if 'added' in storage or 'notdl' in storage or 'added' in storage_replaced or 'notdl' in storage_replaced:
-                        shared_state.logger.debug(
-                            "%s - HEVC Release ignoriert (bereits gefunden)" % key)
+                        shared_state.logger.debug("%s - HEVC Release ignoriert (bereits gefunden)" % key)
                         return True
 
                     englisch = False
                     if "*englisch" in key.lower() or "*english" in key.lower():
                         key = key.replace(
                             '*ENGLISCH', '').replace("*Englisch", "").replace("*ENGLISH", "").replace("*English",
                                                                                                       "").replace(
                             "*", "")
                         englisch = True
                         if not self.feedcrawler.get('english'):
-                            shared_state.logger.debug(
-                                "%s - Englische Releases deaktiviert" % key)
+                            shared_state.logger.debug("%s - Englische Releases deaktiviert" % key)
                             continue
 
                     if self.config.get('enforcedl') and '.dl.' not in key.lower():
                         if not imdb_id:
                             dual_found = download_dual_language(self, key, imdb_id)
                             if dual_found and ".1080p." in key:
                                 continue
                             elif not dual_found and not englisch:
-                                shared_state.logger.debug(
-                                    "%s - Kein zweisprachiges HEVC-Release gefunden." % key)
+                                shared_state.logger.debug("%s - Kein zweisprachiges HEVC-Release gefunden." % key)
                                 self.dl_unsatisfied = True
                         else:
                             if original_language_not_german(imdb_id):
                                 dual_found = download_dual_language(self, key, imdb_id)
                                 if dual_found and ".1080p." in key:
                                     continue
                                 elif not dual_found and not englisch:
@@ -524,39 +503,35 @@
             elif site == "NK":
                 get_download_links_method = content_all_nk.nk_page_download_link
                 download_method = myjd_download
             else:
                 continue
 
             if original_imdb_id and imdb_id and imdb_id != original_imdb_id:
-                shared_state.logger.debug(
-                    "%s - Abweichende IMDb-IDs identifiziert! Breche ab." % key)
+                shared_state.logger.debug("%s - Abweichende IMDb-IDs identifiziert! Breche ab." % key)
                 continue
             if ".dl." not in key.lower():
-                shared_state.logger.debug(
-                    "%s - Release ignoriert (nicht zweisprachig)" % key)
+                shared_state.logger.debug("%s - Release ignoriert (nicht zweisprachig)" % key)
                 continue
             if hevc and hevc_found and not is_hevc(key):
-                shared_state.logger.debug(
-                    "%s - zweisprachiges Release ignoriert (nicht HEVC)" % key)
+                shared_state.logger.debug("%s - zweisprachiges Release ignoriert (nicht HEVC)" % key)
                 continue
             if ".720p." in key.lower():
                 path_suffix = "/Remux"
             else:
                 path_suffix = ""
 
             download_links = get_download_links_method(self, link, key)
             if check_fallback_required(download_links):
                 download_method = add_decrypt_instead_of_download
             if download_links:
                 storage = self.db.retrieve_all(key)
                 storage_replaced = self.db.retrieve_all(key.replace(".COMPLETE", "").replace(".Complete", ""))
                 if 'added' in storage or 'notdl' in storage or 'added' in storage_replaced or 'notdl' in storage_replaced:
-                    shared_state.logger.debug(
-                        "%s - zweisprachiges Release ignoriert (bereits gefunden)" % key)
+                    shared_state.logger.debug("%s - zweisprachiges Release ignoriert (bereits gefunden)" % key)
                     return True
                 elif self.filename == 'List_ContentAll_Movies' or self.filename == 'IMDb':
                     retail = False
                     if self.config.get('cutoff'):
                         if is_retail(key, True):
                             retail = True
                     if download_method(key, "FeedCrawler" + path_suffix, download_links, password):
@@ -607,44 +582,40 @@
     key = key.replace(" ", ".")
 
     added_items = []
     if not hevc_retail:
         if self.hevc_retail:
             if not is_hevc(key) and is_retail(key, False):
                 if download_hevc(self, key, imdb_id):
-                    shared_state.logger.debug(
-                        "%s - Release ignoriert (stattdessen 1080p-HEVC-Retail gefunden)" % key)
+                    shared_state.logger.debug("%s - Release ignoriert (stattdessen 1080p-HEVC-Retail gefunden)" % key)
                     return
     if download_links:
         englisch = False
         if "*englisch" in key.lower() or "*english" in key.lower():
             key = key.replace(
                 '*ENGLISCH', '').replace("*Englisch", "").replace("*ENGLISH", "").replace("*English",
                                                                                           "").replace(
                 "*", "")
             englisch = True
             if not self.feedcrawler.get('english'):
-                shared_state.logger.debug(
-                    "%s - Englische Releases deaktiviert" % key)
+                shared_state.logger.debug("%s - Englische Releases deaktiviert" % key)
                 return
         if self.config.get('enforcedl') and '.dl.' not in key.lower():
             if original_language_not_german(imdb_id):
                 dual_found = download_dual_language(self, key, imdb_id)
                 if dual_found:
                     added_items.append(dual_found)
                     if ".1080p." in key:
                         return added_items
                 elif not dual_found and not englisch:
-                    shared_state.logger.debug(
-                        "%s - Kein zweisprachiges Release gefunden!" % key)
+                    shared_state.logger.debug("%s - Kein zweisprachiges Release gefunden!" % key)
                     return
 
         if '.3d.' in key.lower():
-            shared_state.logger.debug(
-                "%s - Release ignoriert (3D-Film)" % key.title)
+            shared_state.logger.debug("%s - Release ignoriert (3D-Film)" % key.title)
             return
         else:
             retail = False
             if (self.config.get('enforcedl') and '.dl.' in key.lower()) or not self.config.get(
                     'enforcedl'):
                 if self.config.get('cutoff'):
                     if self.config.get('enforcedl'):
@@ -686,63 +657,57 @@
     key = key.replace(" ", ".")
 
     added_items = []
     if not hevc_retail:
         if self.hevc_retail:
             if not is_hevc(key) and is_retail(key, False):
                 if download_hevc(self, key, imdb_id):
-                    shared_state.logger.debug(
-                        "%s - Release ignoriert (stattdessen 1080p-HEVC-Retail gefunden)" % key)
+                    shared_state.logger.debug("%s - Release ignoriert (stattdessen 1080p-HEVC-Retail gefunden)" % key)
                     return
 
     download_method = self.download_method
     download_links = self.get_download_links_method(self, content, key)
     if check_fallback_required(download_links):
         download_method = add_decrypt_instead_of_download
     if download_links:
         storage = self.db.retrieve_all(key)
         storage_replaced = self.db.retrieve_all(key.replace(".COMPLETE", "").replace(".Complete", ""))
         if 'added' in storage or 'notdl' in storage or 'added' in storage_replaced or 'notdl' in storage_replaced:
-            shared_state.logger.debug(
-                "%s - Release ignoriert (bereits gefunden)" % key)
+            shared_state.logger.debug("%s - Release ignoriert (bereits gefunden)" % key)
             return
         elif not check_valid_release(key, self.retail_only, self.hevc_retail):
-            shared_state.logger.debug(
-                "%s - Release ignoriert (Gleiche oder bessere Quelle bereits vorhanden)" % key)
+            shared_state.logger.debug("%s - Release ignoriert (Gleiche oder bessere Quelle bereits vorhanden)" % key)
             return
         englisch = False
         if "*englisch*" in key.lower() or "*english*" in key.lower():
             key = key.replace(
                 '*ENGLISCH*', '').replace("*Englisch*", "").replace("*ENGLISH*", "").replace("*English*", "")
             englisch = True
             if not self.feedcrawler.get('english'):
-                shared_state.logger.debug(
-                    "%s - Englische Releases deaktiviert" % key)
+                shared_state.logger.debug("%s - Englische Releases deaktiviert" % key)
                 return
         if self.config.get('enforcedl') and '.dl.' not in key.lower():
             if not imdb_id:
                 dual_found = download_dual_language(self, key, imdb_id)
                 if dual_found:
                     added_items.append(dual_found)
                     if ".1080p." in key:
                         return added_items
                 else:
-                    shared_state.logger.debug(
-                        "%s - Kein zweisprachiges Release gefunden." % key)
+                    shared_state.logger.debug("%s - Kein zweisprachiges Release gefunden." % key)
                     self.dl_unsatisfied = True
             else:
                 if original_language_not_german(imdb_id):
                     dual_found = download_dual_language(self, key, imdb_id)
                     if dual_found:
                         added_items.append(dual_found)
                         if ".1080p." in key:
                             return added_items
                     elif not dual_found and not englisch:
-                        shared_state.logger.debug(
-                            "%s - Kein zweisprachiges Release gefunden! Breche ab." % key)
+                        shared_state.logger.debug("%s - Kein zweisprachiges Release gefunden! Breche ab." % key)
                         self.dl_unsatisfied = True
                         return
         if self.filename == 'List_ContentAll_Movies':
             retail = False
             if (self.config.get('enforcedl') and '.dl.' in key.lower()) or not self.config.get(
                     'enforcedl'):
                 if self.config.get('cutoff'):
@@ -814,16 +779,15 @@
         if not self.config.get('crawlseasons'):
             return
         liste = get_movies_list(self.filename)
         if liste:
             self.pattern = r'(' + "|".join(liste).lower() + ').*'
     elif self.filename == 'List_ContentAll_Movies_Regex':
         if not self.config.get('regex'):
-            shared_state.logger.debug(
-                "Regex deaktiviert. Stoppe Suche für Filme! (" + self.filename + ")")
+            shared_state.logger.debug("Regex deaktiviert. Stoppe Suche für Filme! (" + self.filename + ")")
             return
         liste = get_movies_list(self.filename)
         if liste:
             self.pattern = r'(' + "|".join(liste).lower() + ').*'
     elif self.filename == "IMDb":
         self.pattern = self.filename
     else:
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/content_shows.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/content_shows.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,15 @@
     elif self.filename == 'List_CustomDJ_Documentaries_Regex':
         release_type = '[Doku/RegEx] - ' + englisch
     else:
         return
     try:
         storage = self.db.retrieve_all(title)
     except Exception as e:
-        shared_state.logger.debug(
-            "Fehler bei Datenbankzugriff: %s, Grund: %s" % (e, title))
+        shared_state.logger.debug("Fehler bei Datenbankzugriff: %s, Grund: %s" % (e, title))
 
     if 'added' in storage or 'notdl' in storage:
         shared_state.logger.debug(title + " - Release ignoriert (bereits gefunden)")
     else:
         if season and episode:
             link = link.replace('&_=', '&season=' + str(season) + '&episode=' + str(episode) + '&_=')
         download = add_decrypt(title, link, self.url)
@@ -137,15 +136,15 @@
                     if self.filename == "List_ContentAll_Seasons" or self.filename == "List_ContentShows_Seasons_Regex":
                         feed = self.get_feed_method(response["text"], "seasons", 'https://' + self.url, True)
                     else:
                         feed = self.get_feed_method(response["text"], "episodes", 'https://' + self.url, True)
                 else:
                     feed = False
             except:
-                print(self._SITE + u" hat die Feed-API angepasst. Breche Suche ab!")
+                print(self._SITE + " hat die Feed-API angepasst. Breche Suche ab!")
                 feed = False
 
             if response:
                 if response["status_code"] == 304:
                     shared_state.logger.debug(
                         self._SITE + "-Feed seit letztem Aufruf nicht aktualisiert - breche  Suche ab!")
                     return
@@ -158,41 +157,39 @@
                     if self.filename == "List_ContentAll_Seasons" or self.filename == "List_ContentShows_Seasons_Regex":
                         feed = self.get_feed_method(response, "seasons", 'https://' + self.url, True)
                     else:
                         feed = self.get_feed_method(response, "episodes", 'https://' + self.url, True)
                 else:
                     feed = False
             except:
-                print(self._SITE + u" hat die Feed-API angepasst. Breche Suche ab!")
+                print(self._SITE + " hat die Feed-API angepasst. Breche Suche ab!")
                 feed = False
 
         self.day += 1
 
         if feed and feed.entries:
             first_post = feed.entries[0]
             concat = first_post.title + first_post.published + str(self.settings) + str(self.pattern)
             sha = hashlib.sha256(concat.encode(
                 'ascii', 'ignore')).hexdigest()
         else:
-            if self._SITE == "SF" and not shared_state.sf_blocked:
-                print(u"SF hat den Feed-Anruf während der Feed-Suche blockiert.")
-                shared_state.sf_blocked = True
+            if self._SITE == "SF" and not shared_state.values["sf_blocked"]:
+                print("SF hat den Feed-Anruf während der Feed-Suche blockiert.")
+                shared_state.values["sf_blocked"] = True
             else:
-                shared_state.logger.debug(
-                    "Feed ist leer - breche die Suche für diesen Feed ab!")
+                shared_state.logger.debug("Feed ist leer - breche die Suche für diesen Feed ab!")
 
         if feed:
             for post in feed.entries:
                 concat = post.title + post.published + \
                          str(self.settings) + str(self.pattern)
                 sha = hashlib.sha256(concat.encode(
                     'ascii', 'ignore')).hexdigest()
                 if sha == self.last_sha:
-                    shared_state.logger.debug(
-                        "Feed ab hier bereits gecrawlt (" + post.title + ") - breche  Suche ab!")
+                    shared_state.logger.debug("Feed ab hier bereits gecrawlt (" + post.title + ") - breche  Suche ab!")
                     break
 
                 series_url = post.series_url
                 title = post.title.replace("-", "-")
 
                 if self.filename == 'List_ContentShows_Shows_Regex':
                     if self.config.get("regex"):
@@ -229,16 +226,15 @@
                                     season = package["season"]
                                     episode = package["episode"]
                                     size = package["size"]
                                     imdb_id = package["imdb_id"]
                                     send_package(self, title, download_link, language_id, season, episode, site,
                                                  post.source, size, imdb_id)
                         else:
-                            shared_state.logger.debug(
-                                "%s - Englische Releases deaktiviert" % title)
+                            shared_state.logger.debug("%s - Englische Releases deaktiviert" % title)
 
                     else:
                         continue
                 elif self.filename == 'List_ContentShows_Seasons_Regex':
                     if self.config.get("regex"):
                         if '.german.' in title.lower():
                             language_id = 1
@@ -273,16 +269,15 @@
                                     season = package["season"]
                                     episode = package["episode"]
                                     size = package["size"]
                                     imdb_id = package["imdb_id"]
                                     send_package(self, title, download_link, language_id, season, episode, site,
                                                  post.source, size, imdb_id)
                         else:
-                            shared_state.logger.debug(
-                                "%s - Englische Releases deaktiviert" % title)
+                            shared_state.logger.debug("%s - Englische Releases deaktiviert" % title)
 
                     else:
                         continue
                 else:
                     if self.config.get("quality") != '480p':
                         match = re.search(self.pattern, title.lower())
                         if match:
@@ -308,32 +303,30 @@
                                     try:
                                         storage = self.db.retrieve_all(title)
                                     except Exception as e:
                                         shared_state.logger.debug(
                                             "Fehler bei Datenbankzugriff: %s, Grund: %s" % (e, title))
                                         return
                                     if 'added' in storage:
-                                        shared_state.logger.debug(
-                                            title + " - Release ignoriert (bereits gefunden)")
+                                        shared_state.logger.debug(title + " - Release ignoriert (bereits gefunden)")
                                         continue
                                     package = self.parse_download_method(self, series_url, title, language_id)
                                     if package:
                                         title = package["title"]
                                         site = self._SITE
                                         download_link = package["download_link"]
                                         language_id = package["language_id"]
                                         season = package["season"]
                                         episode = package["episode"]
                                         size = package["size"]
                                         imdb_id = package["imdb_id"]
                                         send_package(self, title, download_link, language_id, season, episode, site,
                                                      post.source, size, imdb_id)
                             else:
-                                shared_state.logger.debug(
-                                    "%s - Englische Releases deaktiviert" % title)
+                                shared_state.logger.debug("%s - Englische Releases deaktiviert" % title)
 
                         else:
                             match = re.search(self.pattern, title.lower())
                             if match:
                                 if '.german.' in title.lower():
                                     language_id = 1
                                 elif self.feedcrawler.get('english'):
@@ -357,32 +350,30 @@
                                     try:
                                         storage = self.db.retrieve_all(title)
                                     except Exception as e:
                                         shared_state.logger.debug(
                                             "Fehler bei Datenbankzugriff: %s, Grund: %s" % (e, title))
                                         return
                                     if 'added' in storage:
-                                        shared_state.logger.debug(
-                                            title + " - Release ignoriert (bereits gefunden)")
+                                        shared_state.logger.debug(title + " - Release ignoriert (bereits gefunden)")
                                         continue
                                     package = self.parse_download_method(self, series_url, title, language_id)
                                     if package:
                                         title = package["title"]
                                         site = self._SITE
                                         download_link = package["download_link"]
                                         language_id = package["language_id"]
                                         season = package["season"]
                                         episode = package["episode"]
                                         size = package["size"]
                                         imdb_id = package["imdb_id"]
                                         send_package(self, title, download_link, language_id, season, episode, site,
                                                      post.source, size, imdb_id)
                                 else:
-                                    shared_state.logger.debug(
-                                        "%s - Englische Releases deaktiviert" % title)
+                                    shared_state.logger.debug("%s - Englische Releases deaktiviert" % title)
 
     if current_set and sha:
         new_set = settings_hash(self, True)
         if current_set == new_set:
             self.cdc.delete(self._INTERNAL_NAME + "Set-" + self.filename)
             self.cdc.store(self._INTERNAL_NAME + "Set-" + self.filename, current_set)
             self.cdc.delete(self._INTERNAL_NAME + "-" + self.filename)
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/shared.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_by.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_dw.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_dw.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     try:
         try:
             content = BeautifulSoup(content, "html.parser")
         except:
             content = BeautifulSoup(str(content), "html.parser")
         download_buttons = content.findAll("button", {"class": "show_link"})
     except:
-        print(u"DW hat die Detail-Seite angepasst. Parsen von Download-Links für " + title + " nicht möglich!")
+        print("DW hat die Detail-Seite angepasst. Parsen von Download-Links für " + title + " nicht möglich!")
         return False
 
     dw = CrawlerConfig('Hostnames').get('dw')
     ajax_url = "https://" + dw + "/wp-admin/admin-ajax.php"
 
     download_links = []
     try:
@@ -101,15 +101,15 @@
             payload = "action=show_link&link_id=" + button["value"]
             response = json.loads(post_url(ajax_url, payload))
             if response["success"]:
                 link = response["data"].split(",")[0]
                 hoster = button.nextSibling.img["src"].split("/")[-1].replace(".png", "")
                 download_links.append([link, hoster])
     except:
-        print(u"DW hat die Detail-Seite angepasst. Parsen von Download-Links nicht möglich!")
+        print("DW hat die Detail-Seite angepasst. Parsen von Download-Links nicht möglich!")
         pass
 
     return check_download_links(self, download_links)
 
 
 def dw_feed_enricher(feed):
     feed = BeautifulSoup(feed, "html.parser")
@@ -163,15 +163,15 @@
                             "value": str(details)
                         })],
                     "source": source,
                     "size": size,
                     "imdb_id": imdb_id
                 }))
         except:
-            print(u"DW hat den Feed angepasst. Parsen teilweise nicht möglich!")
+            print("DW hat den Feed angepasst. Parsen teilweise nicht möglich!")
             continue
 
     feed = {"entries": entries}
     feed = FakeFeedParserDict(feed)
     return feed
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_ff.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_ff.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         links = content.findAll("div", {'class': 'row'})[1].findAll('a')
         download_link = False
         for link in links:
             if check_hoster(link.text.replace('\n', '')):
                 download_link = "https://" + self.url + link['href']
                 break
     except:
-        print(u"FF hat die Detail-Seite angepasst. Parsen von Download-Links nicht möglich!")
+        print("FF hat die Detail-Seite angepasst. Parsen von Download-Links nicht möglich!")
         return False
 
     return [download_link]
 
 
 def ff_feed_enricher(releases):
     entries = []
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_fx.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_fx.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                             })],
                         "source": source,
                         "size": size,
                         "imdb_id": imdb_id
                     }))
                     i += 1
         except:
-            print(u"FX hat den Feed angepasst. Parsen teilweise nicht möglich!")
+            print("FX hat den Feed angepasst. Parsen teilweise nicht möglich!")
             continue
 
     feed = {"entries": entries}
     feed = FakeFeedParserDict(feed)
     return feed
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_hw.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_hw.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     try:
         try:
             content = BeautifulSoup(content, "html.parser")
         except:
             content = BeautifulSoup(str(content), "html.parser")
         download_links = content.findAll("a", href=re.compile('filecrypt'))
     except:
-        print(u"HW hat die Detail-Seite angepasst. Parsen von Download-Links nicht möglich!")
+        print("HW hat die Detail-Seite angepasst. Parsen von Download-Links nicht möglich!")
         return False
 
     links_string = ""
     for link in download_links:
         links_string += str(link)
 
     return get_download_links(self, links_string, title)
@@ -137,15 +137,15 @@
                             "value": str(article)
                         })],
                     "source": source,
                     "size": size,
                     "imdb_id": imdb_id
                 }))
         except:
-            print(u"HW hat den Feed angepasst. Parsen teilweise nicht möglich!")
+            print("HW hat den Feed angepasst. Parsen teilweise nicht möglich!")
             continue
 
     feed = {"entries": entries}
     feed = FakeFeedParserDict(feed)
     return feed
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_nk.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_nx.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_nx.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,13 +134,13 @@
                         })],
                     "source": source,
                     "size": size,
                     "imdb_id": imdb_id
                 }))
 
         except:
-            print(u"NX hat den Feed angepasst. Parsen teilweise nicht möglich!")
+            print("NX hat den Feed angepasst. Parsen teilweise nicht möglich!")
             continue
 
     feed = {"entries": entries}
     feed = FakeFeedParserDict(feed)
     return feed
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_ww.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_ww.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,34 +98,34 @@
         url = payload[0]
         referer = payload[0].replace("/ajax", payload[1])
         data = payload[2]
         headers["Referer"] = referer
         response = post_url_headers(url, headers, data)
         if not response["text"] or response["status_code"] is not (200 or 304) or not '<span class="main-rls">' in \
                                                                                       response["text"]:
-            if not shared_state.ww_blocked:
-                print(u"WW hat den Feed-Anruf während der Feed-Suche blockiert.")
-                shared_state.ww_blocked = True
+            if not shared_state.values["ww_blocked"]:
+                print("WW hat den Feed-Anruf während der Feed-Suche blockiert.")
+                shared_state.values["ww_blocked"] = True
             return ""
         return response
     except:
         return ""
 
 
 def ww_get_download_links(self, content, title):
     base_url = "https://" + CrawlerConfig('Hostnames').get('ww')
     content = content.replace("mkv|", "")
     download_links = []
     try:
         response = get_url(content)
         if not response or "NinjaFirewall 429" in response:
-            if not shared_state.ww_blocked:
+            if not shared_state.values["ww_blocked"]:
                 print(
-                    u"WW hat den Link-Abruf für " + title + " blockiert. Eine spätere Anfrage hat möglicherweise Erfolg!")
-                shared_state.ww_blocked = True
+                    "WW hat den Link-Abruf für " + title + " blockiert. Eine spätere Anfrage hat möglicherweise Erfolg!")
+                shared_state.values["ww_blocked"] = True
             return False
         links = BeautifulSoup(response, "html.parser").findAll("div", {"id": "download-links"})
         for link in links:
             hoster = link.text
             if 'Direct Download 100 MBit/s' not in hoster:
                 url = base_url + link.find("a")["href"]
                 download_links.append('href="' + url + '" ' + hoster + '<')
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                         for link in post.links:
                             if check_hoster(link):
                                 links.append(link)
                         if not links and self.hoster_fallback:
                             links = post.links
                         storage = self.db.retrieve_all(post.title)
                         if not links:
-                            shared_state.logger.debug(u"Release ignoriert - keine Links gefunden")
+                            shared_state.logger.debug("Release ignoriert - keine Links gefunden")
                         elif 'added' in storage:
                             shared_state.logger.debug(post.title + " - Release ignoriert (bereits gefunden)")
                         else:
                             if myjd_download(post.title, "FeedCrawler", links, self.url):
                                 self.db.store(post.title, 'added')
                                 log_entry = '[Episode/Englisch] - ' + post.title + ' - [' + self._SITE + '] - ' \
                                             + post.size + ' - ' + post.source
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,22 +113,21 @@
     feed = {"entries": entries}
     feed = FakeFeedParserDict(feed)
     return feed
 
 
 def sf_parse_download(self, series_url, title, language_id):
     if not check_valid_release(title, self.retail_only, self.hevc_retail):
-        shared_state.logger.debug(title + u" - Release ignoriert (Gleiche oder bessere Quelle bereits vorhanden)")
+        shared_state.logger.debug(title + " - Release ignoriert (Gleiche oder bessere Quelle bereits vorhanden)")
         return False
     if self.filename == 'List_ContentAll_Seasons':
         if not self.config.get("seasonpacks"):
             staffelpack = re.search(r"s\d.*(-|\.).*s\d", title.lower())
             if staffelpack:
-                shared_state.logger.debug(
-                    "%s - Release ignoriert (Staffelpaket)" % title)
+                shared_state.logger.debug("%s - Release ignoriert (Staffelpaket)" % title)
                 return False
         if not re.search(self.seasonssource, title.lower()):
             shared_state.logger.debug(title + " - Release hat falsche Quelle")
             return False
     try:
         if language_id == 2:
             lang = 'EN'
@@ -256,9 +255,9 @@
                 "language_id": language_id,
                 "season": season,
                 "episode": episode,
                 "size": size,
                 "imdb_id": imdb_id
             }
     except:
-        print(u"SF hat die Serien-API angepasst. Breche Download-Prüfung ab!")
+        print("SF hat die Serien-API angepasst. Breche Download-Prüfung ab!")
         return False
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,22 +104,21 @@
     feed = {"entries": entries}
     feed = FakeFeedParserDict(feed)
     return feed
 
 
 def sj_parse_download(self, series_url, title, language_id):
     if not check_valid_release(title, self.retail_only, self.hevc_retail):
-        shared_state.logger.debug(title + u" - Release ignoriert (Gleiche oder bessere Quelle bereits vorhanden)")
+        shared_state.logger.debug(title + " - Release ignoriert (Gleiche oder bessere Quelle bereits vorhanden)")
         return False
     if self.filename == 'List_ContentAll_Seasons':
         if not self.config.get("seasonpacks"):
             staffelpack = re.search(r"s\d.*(-|\.).*s\d", title.lower())
             if staffelpack:
-                shared_state.logger.debug(
-                    "%s - Release ignoriert (Staffelpaket)" % title)
+                shared_state.logger.debug("%s - Release ignoriert (Staffelpaket)" % title)
                 return False
         if not re.search(self.seasonssource, title.lower()):
             shared_state.logger.debug(title + " - Release hat falsche Quelle")
             return False
     try:
         series_info = get_url(series_url)
         series_id = re.findall(r'data-mediaid="(.*?)"', series_info)[0]
@@ -154,9 +153,9 @@
                             "language_id": language_id,
                             "season": False,
                             "episode": False,
                             "size": "",  # Info not available
                             "imdb_id": ""  # Info not available
                         }
     except:
-        print(self._INTERNAL_NAME + u" hat die Serien-API angepasst. Breche Download-Prüfung ab!")
+        print(self._INTERNAL_NAME + " hat die Serien-API angepasst. Breche Download-Prüfung ab!")
         return False
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/metadata/imdb.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/metadata/imdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,15 @@
                 if year_in_title:
                     year = ' ' + result['titleReleaseText']
                 if simplified_search_term_in_title(title, result['titleNameText'] + year):
                     imdb_id = result['id']
                     break
     else:
         print("IMDb-Abfrage fehlgeschlagen: " + str(request["status_code"]))
-        shared_state.logger.debug(
-            "IMDb-Abfrage fehlgeschlagen: " + str(request["status_code"]))
+        shared_state.logger.debug("IMDb-Abfrage fehlgeschlagen: " + str(request["status_code"]))
 
     if not imdb_id:
         shared_state.logger.debug("[IMDb] - %s - Keine ID gefunden" % title.replace("+", " "))
     return imdb_id
 
 
 @imdb_id_not_none
@@ -142,15 +141,15 @@
 
     if original_language and original_language == "de":
         shared_state.logger.debug(
             "[IMDb] - %s - Original-Sprache ist Deutsch. Breche Suche nach zweisprachigem Release ab!" % imdb_id)
         return False
 
     if not original_language:
-        print(u"[IMDb] - %s - Original-Sprache nicht ermittelbar" % imdb_id)
+        print("[IMDb] - %s - Original-Sprache nicht ermittelbar" % imdb_id)
         shared_state.logger.debug("[IMDb] - %s - Original-Sprache nicht ermittelbar" % imdb_id)
 
     return original_language
 
 
 @imdb_id_not_none
 def get_episodes(imdb_id):
@@ -173,15 +172,15 @@
                     eps.append(i)
                     i += 1
                 episodes[int(sn)] = eps
     except:
         pass
 
     if not episodes:
-        print(u"[IMDb] - %s - Keine Episoden gefunden" % imdb_id)
+        print("[IMDb] - %s - Keine Episoden gefunden" % imdb_id)
         shared_state.logger.debug("[IMDb] - %s - Keine Episoden gefunden" % imdb_id)
 
     return episodes
 
 
 @imdb_id_not_none
 def get_localized_title(imdb_id):
@@ -195,15 +194,15 @@
         try:
             match = re.findall(r'<title>(.*?) - IMDb</title>', request["text"])
             localized_title = match[0]
         except:
             pass
 
     if not localized_title:
-        print(u"[IMDb] - %s - Deutscher Titel nicht ermittelbar" % imdb_id)
+        print("[IMDb] - %s - Deutscher Titel nicht ermittelbar" % imdb_id)
         shared_state.logger.debug("[IMDb] - %s - Deutscher Titel nicht ermittelbar" % imdb_id)
 
     return localized_title
 
 
 @imdb_id_not_none
 def get_rating(imdb_id):
@@ -215,15 +214,15 @@
         props = soup.find("script", text=re.compile("props"))
         details = loads(props.string)
         rating = details['props']['pageProps']['aboveTheFoldData']['ratingsSummary']['aggregateRating']
     except:
         pass
 
     if not rating:
-        print(u"[IMDb] - %s - Bewertungen nicht ermittelbar" % imdb_id)
+        print("[IMDb] - %s - Bewertungen nicht ermittelbar" % imdb_id)
         shared_state.logger.debug("[IMDb] - %s - Bewertungen nicht ermittelbar" % imdb_id)
 
     return rating
 
 
 @imdb_id_not_none
 def get_votes(imdb_id):
@@ -235,15 +234,15 @@
         props = soup.find("script", text=re.compile("props"))
         details = loads(props.string)
         votes = details['props']['pageProps']['aboveTheFoldData']['ratingsSummary']['voteCount']
     except:
         pass
 
     if not votes:
-        print(u"[IMDb] - %s - Anzahl der Bewertungen nicht ermittelbar" % imdb_id)
+        print("[IMDb] - %s - Anzahl der Bewertungen nicht ermittelbar" % imdb_id)
         shared_state.logger.debug("[IMDb] - %s - Anzahl der Bewertungen nicht ermittelbar" % imdb_id)
 
     return votes
 
 
 @imdb_id_not_none
 def get_year(imdb_id):
@@ -253,11 +252,11 @@
         request = get_url("https://www.imdb.com/title/%s/" % imdb_id)
         match = re.findall(r'<title>(?:.*?) \(.*?(\d{4}).*</title>', request)
         year = int("".join(re.findall(r'\d+', str(match[0]))))
     except:
         pass
 
     if not year:
-        print(u"[IMDb] - %s - Erscheinungsjahr nicht ermittelbar" % imdb_id)
+        print("[IMDb] - %s - Erscheinungsjahr nicht ermittelbar" % imdb_id)
         shared_state.logger.debug("[IMDb] - %s - Erscheinungsjahr nicht ermittelbar" % imdb_id)
 
     return year
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/content_all.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/content_all.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,24 +50,24 @@
             score = rate(result)
             if score > best_score:
                 best_score = score
                 best_match = result
                 best_payload = payload
 
     if not best_match or not best_payload:
-        shared_state.logger.debug(u'Kein Treffer für die Suche nach ' + title + '! Suchliste ergänzt.')
+        shared_state.logger.debug('Kein Treffer für die Suche nach ' + title + '! Suchliste ergänzt.')
         liste = "List_ContentAll_Movies"
         cont = ListDb(liste).retrieve()
         if not cont:
             cont = ""
         if title not in cont:
             ListDb(liste).store(title)
         return False
     if not is_retail(best_match, True):
-        shared_state.logger.debug(u'Kein Retail-Release für die Suche nach ' + title + ' gefunden! Suchliste ergänzt.')
+        shared_state.logger.debug('Kein Retail-Release für die Suche nach ' + title + ' gefunden! Suchliste ergänzt.')
         liste = "List_ContentAll_Movies"
         cont = ListDb(liste).retrieve()
         if not cont:
             cont = ""
         if title not in cont:
             ListDb(liste).store(title)
         return best_payload
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/content_shows.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/content_shows.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
             try:
                 if result_episodes[season]:
                     success = True
             except:
                 pass
 
         if success:
-            shared_state.logger.debug(u"Web-Suche erfolgreich für " + title + " - " + season)
+            shared_state.logger.debug("Web-Suche erfolgreich für " + title + " - " + season)
         else:
             for release in releases['items']:
                 name = release['name'].encode('ascii', errors='ignore').decode('utf-8')
                 hosters = release['hoster']
                 valid = True
                 if valid and special:
                     valid = bool("." + special.lower() + "." in name.lower())
@@ -333,15 +333,15 @@
                         result_seasons.update({season: name})
 
             try:
                 if result_seasons[season] and result_episodes[season]:
                     del result_episodes[season]
             except:
                 pass
-            shared_state.logger.debug(u"Web-Suche erfolgreich für " + title + " - " + season)
+            shared_state.logger.debug("Web-Suche erfolgreich für " + title + " - " + season)
 
     matches = []
 
     for season in result_seasons:
         matches.append(result_seasons[season])
     for season in result_episodes:
         for episode in result_episodes[season]:
@@ -373,18 +373,18 @@
                 incomplete = True
             url = source
 
         if url:
             if add_decrypt(title, url, password):
                 if incomplete:
                     db.store(title, 'incomplete')
-                    log_entry = u'[Suche/Serie/Unvollständig] - ' + title + ' - [' + site + '] - ' + size + ' - ' + source
+                    log_entry = '[Suche/Serie/Unvollständig] - ' + title + ' - [' + site + '] - ' + size + ' - ' + source
                 else:
                     db.store(title, 'added')
-                    log_entry = u'[Suche/Serie] - ' + title + ' - [' + site + '] - ' + size + ' - ' + source
+                    log_entry = '[Suche/Serie] - ' + title + ' - [' + site + '] - ' + size + ' - ' + source
                 shared_state.logger.info(log_entry)
                 notify_array.append({"text": log_entry})
 
     notify(notify_array)
 
     if not matches:
         return False
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/shared.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_by.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_dw.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_fx.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_hw.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_nk.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_nx.py` & `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_nx.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,11 +29,11 @@
                                 if check_release_not_sd(title):
                                     continue
                             else:
                                 continue
                         results.append([title, link])
 
         except:
-            print(u"NX hat die Suche angepasst. Parsen teilweise nicht möglich!")
+            print("NX hat die Suche angepasst. Parsen teilweise nicht möglich!")
             continue
 
     return results
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_tools/myjd_api.py` & `feedcrawler-18.0.2/feedcrawler/external_tools/myjd_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1144,15 +1144,15 @@
                                                   query[0] + "&".join(query[1:])))
                 ]
             query = query[0] + "&".join(query[1:])
             try:
                 encrypted_response = request(api + query, timeout=timeout, output_errors=output_errors)
             except URLError:
                 encrypted_response = request(api + query, timeout=timeout, output_errors=output_errors, verify=False)
-                print(u"Die sichere Verbindung zu My JDownloader konnte nicht verifiziert werden.")
+                print("Die sichere Verbindung zu My JDownloader konnte nicht verifiziert werden.")
         else:
             params_request = []
             if params is not None:
                 for param in params:
                     if not isinstance(param, list):
                         params_request += [json.dumps(param)]
                     else:
@@ -1191,15 +1191,15 @@
                             "Content-Type": "application/aesjson-jd; charset=utf-8"
                         },
                         data=encrypted_data,
                         method="POST",
                         timeout=timeout,
                         output_errors=output_errors,
                         verify=False)
-                    print(u"Die sichere Verbindung zu My JDownloader konnte nicht verifiziert werden.")
+                    print("Die sichere Verbindung zu My JDownloader konnte nicht verifiziert werden.")
                 except URLError:
                     return None
         if encrypted_response.status_code == 403:
             raise TokenExpiredException
         if encrypted_response.status_code == 503:
             raise RequestTimeoutException
         if encrypted_response.status_code != 200:
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_tools/ombi_api.py` & `feedcrawler-18.0.2/feedcrawler/external_tools/ombi_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,29 @@
         title = keep_alphanumeric_with_special_characters(get_localized_title(imdb_id))
         year = str(get_year(imdb_id))
         return title + " " + year
     except:
         if imdb_id is None:
             shared_state.logger.debug("Ein Film ohne IMDb-ID wurde angefordert.")
         else:
-            print(u"[Ombi] - Fehler beim Abruf der IMDb für: " + imdb_id)
+            print("[Ombi] - Fehler beim Abruf der IMDb für: " + imdb_id)
         return False
 
 
 def imdb_show(imdb_id):
     try:
         title = keep_alphanumeric_with_special_characters(get_localized_title(imdb_id))
         seasons = get_episodes(imdb_id)
 
         return title, seasons
     except:
         if imdb_id is None:
             shared_state.logger.debug("Eine Serie ohne IMDb-ID wurde angefordert.")
         else:
-            print(u"[Ombi] - Fehler beim Abruf der IMDb für: " + imdb_id)
+            print("[Ombi] - Fehler beim Abruf der IMDb für: " + imdb_id)
         return False
 
 
 def ombi_search(first_launch):
     db = FeedDb('Ombi')
     config = CrawlerConfig('Ombi')
     url = config.get('url')
@@ -66,39 +66,39 @@
         requested_movies = json.loads(requested_movies.text)
         requested_shows = request(url + '/api/v1/Request/tv', headers={'ApiKey': api})
         requested_shows = json.loads(requested_shows.text)
         len_movies = len(requested_movies)
         len_shows = len(requested_shows)
         if first_launch:
             shared_state.logger.debug("Erfolgreich mit Ombi verbunden.")
-            print(u"Erfolgreich mit Ombi verbunden.")
+            print("Erfolgreich mit Ombi verbunden.")
     except:
         shared_state.logger.debug("Ombi ist nicht erreichbar!")
-        print(u"Ombi ist nicht erreichbar!")
+        print("Ombi ist nicht erreichbar!")
         return [0, 0]
 
     if requested_movies:
         shared_state.logger.debug(
             "Die Suchfunktion für Filme nutzt BY, FX, HW, NK und NX, sofern deren Hostnamen gesetzt wurden.")
     for r in requested_movies:
         if bool(r.get("approved")):
             if not bool(r.get("available")):
                 imdb_id = r.get("imdbId")
                 if imdb_id:
                     if not db.retrieve('movie_' + str(imdb_id)) == 'added':
                         title = imdb_movie(imdb_id)
                         if title:
                             best_result = feedcrawler.external_sites.web_search.content_all.get_best_result(title)
-                            print(u"Film: " + title + u" durch Ombi hinzugefügt.")
+                            print("Film: " + title + " durch Ombi hinzugefügt.")
                             if best_result:
                                 feedcrawler.external_sites.web_search.content_all.download(best_result)
                             if english:
                                 title = r.get('title')
                                 best_result = feedcrawler.external_sites.web_search.content_all.get_best_result(title)
-                                print(u"Film: " + title + u"durch Ombi hinzugefügt.")
+                                print("Film: " + title + "durch Ombi hinzugefügt.")
                                 if best_result:
                                     feedcrawler.external_sites.web_search.content_all.download(best_result)
                             db.store('movie_' + str(imdb_id), 'added')
                 else:
                     print("Ein Film ohne IMDb-ID wurde in Ombi angefordert und kann nicht verarbeitet werden.")
                     shared_state.logger.debug(
                         "Ein Film ohne IMDb-ID wurde in Ombi angefordert und kann nicht verarbeitet werden.")
@@ -163,15 +163,15 @@
                                                             e = str(e)
                                                             if len(e) == 1:
                                                                 e = "0" + e
                                                             se = s + "E" + e
                                                             db.store('show_' + str(imdb_id) + '_' + se, 'added')
                                                         if not add_season:
                                                             shared_state.logger.debug(
-                                                                u"Konnte kein Release für " + title + " " + se + "finden.")
+                                                                "Konnte kein Release für " + title + " " + se + "finden.")
                                                         break
                                                 db.store('show_' + str(imdb_id) + '_' + se, 'added')
                                         else:
                                             payload = feedcrawler.external_sites.web_search. \
                                                 content_shows.get_best_result(title)
                                             if payload:
                                                 payload = decode_base64(payload).split("|")
@@ -179,14 +179,14 @@
                                                 feedcrawler.external_sites.web_search.content_shows.download(payload)
                                             for ep in eps:
                                                 e = str(ep)
                                                 if len(e) == 1:
                                                     e = "0" + e
                                                 se = s + "E" + e
                                                 db.store('show_' + str(imdb_id) + '_' + se, 'added')
-                                        print(u"Serie/Staffel/Episode: " + title + u" durch Ombi hinzugefügt.")
+                                        print("Serie/Staffel/Episode: " + title + " durch Ombi hinzugefügt.")
         else:
             print("Eine Serie ohne IMDb-ID wurde in Ombi angefordert und kann nicht verarbeitet werden.")
             shared_state.logger.debug(
                 "Eine Serie ohne IMDb-ID wurde in Ombi angefordert und kann nicht verarbeitet werden.")
 
     return [len_movies, len_shows]
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_tools/overseerr_api.py` & `feedcrawler-18.0.2/feedcrawler/external_tools/overseerr_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     english = CrawlerConfig('FeedCrawler').get('english')
 
     try:
         requested_titles_raw = request(url + '/api/v1/request?take=999', headers={'X-Api-Key': api})
         if requested_titles_raw.status_code != 200:
             shared_state.logger.debug("Overseerr API-Key ungültig!")
-            print(u"Overseerr API-Key ungültig!")
+            print("Overseerr API-Key ungültig!")
             return [0, 0]
 
         requested_titles = json.loads(requested_titles_raw.text)
 
         requested_movies = []
         requested_shows = []
 
@@ -47,57 +47,57 @@
                 shared_state.logger.debug("Anfrage mit ID " + str(item['id']) + " ist freigegeben.")
                 if item['type'] == 'movie':
                     details_raw = request(url + '/api/v1/movie/' + str(item['media']['tmdbId']),
                                           headers={'X-Api-Key': api})
                     if details_raw.status_code != 200:
                         shared_state.logger.debug(
                             "Overseerr fehlen die notwendigen Details für tmbbId: " + str(item['media']['tmdbId']))
-                        print(u"Overseerr fehlen die notwendigen Details für tmbbId: " + str(item['media']['tmdbId']))
+                        print("Overseerr fehlen die notwendigen Details für tmbbId: " + str(item['media']['tmdbId']))
                     else:
                         details = json.loads(details_raw.text)
                         requested_movies.append(details)
                 elif item['type'] == 'tv':
                     details_raw = request(url + '/api/v1/tv/' + str(item['media']['tmdbId']),
                                           headers={'X-Api-Key': api})
                     if details_raw.status_code != 200:
                         shared_state.logger.debug(
                             "Overseerr fehlen die notwendigen Details für tmbbId: " + str(item['media']['tmdbId']))
-                        print(u"Overseerr fehlen die notwendigen Details für tmbbId: " + str(item['media']['tmdbId']))
+                        print("Overseerr fehlen die notwendigen Details für tmbbId: " + str(item['media']['tmdbId']))
                     else:
                         details = json.loads(details_raw.text)
                         requested_shows.append(details)
             else:
                 shared_state.logger.debug("Anfrage mit ID " + str(item['id']) + " ist noch nicht freigegeben.")
 
         len_movies = len(requested_movies)
         len_shows = len(requested_shows)
         if first_launch:
             shared_state.logger.debug("Erfolgreich mit Overseerr verbunden.")
-            print(u"Erfolgreich mit Overseerr verbunden.")
+            print("Erfolgreich mit Overseerr verbunden.")
     except:
         shared_state.logger.debug("Overseerr ist nicht erreichbar!")
-        print(u"Overseerr ist nicht erreichbar!")
+        print("Overseerr ist nicht erreichbar!")
         return [0, 0]
 
     if requested_movies:
         shared_state.logger.debug(
             "Die Suchfunktion für Filme nutzt BY, FX, HW, NK und NX, sofern deren Hostnamen gesetzt wurden.")
     for r in requested_movies:
         item_id = r["id"]
         if not db.retrieve('movie_' + str(item_id)) == 'added':
             title = r["title"]
             if title:
                 best_result = feedcrawler.external_sites.web_search.content_all.get_best_result(title)
-                print(u"Film: " + title + u" durch Overseerr hinzugefügt.")
+                print("Film: " + title + " durch Overseerr hinzugefügt.")
                 if best_result:
                     feedcrawler.external_sites.web_search.content_all.download(best_result)
                 if english:
                     title = r.get('title')
                     best_result = feedcrawler.external_sites.web_search.content_all.get_best_result(title)
-                    print(u"Film: " + title + u"durch Overseerr hinzugefügt.")
+                    print("Film: " + title + "durch Overseerr hinzugefügt.")
                     if best_result:
                         feedcrawler.external_sites.web_search.content_all.download(best_result)
                 db.store('movie_' + str(item_id), 'added')
 
     if requested_shows:
         shared_state.logger.debug("Die Suchfunktion für Serien nutzt SF und SJ, sofern deren Hostnamen gesetzt wurden.")
     for r in requested_shows:
@@ -112,10 +112,10 @@
                 if title:
                     payload = feedcrawler.external_sites.web_search.content_shows.get_best_result(title)
                     if payload:
                         payload = decode_base64(payload).split("|")
                         payload = encode_base64(payload[0] + "|" + payload[1] + "|" + season)
                         if feedcrawler.external_sites.web_search.content_shows.download(payload):
                             db.store('show_' + str(item_id) + "_" + str(season), 'added')
-                            print(u"Serie/Staffel/Episode: " + title + u" durch Overseerr hinzugefügt.")
+                            print("Serie/Staffel/Episode: " + title + " durch Overseerr hinzugefügt.")
 
     return [len_movies, len_shows]
```

### Comparing `feedcrawler-18.0.1/feedcrawler/external_tools/plex_api.py` & `feedcrawler-18.0.2/feedcrawler/external_tools/plex_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,39 +27,39 @@
         title = keep_alphanumeric_with_special_characters(get_localized_title(imdb_id))
         year = str(get_year(imdb_id))
         return title + " " + year
     except:
         if imdb_id is None:
             shared_state.logger.debug("Ein Film ohne IMDb-ID wurde angefordert.")
         else:
-            print(u"[Plex] - Fehler beim Abruf der IMDb für: " + imdb_id)
+            print("[Plex] - Fehler beim Abruf der IMDb für: " + imdb_id)
         return False
 
 
 def imdb_show(imdb_id):
     try:
         title = keep_alphanumeric_with_special_characters(get_localized_title(imdb_id))
 
         return title
     except:
         if imdb_id is None:
             shared_state.logger.debug("Eine Serie ohne IMDb-ID wurde angefordert.")
         else:
-            print(u"[Plex] - Fehler beim Abruf der IMDb für: " + imdb_id)
+            print("[Plex] - Fehler beim Abruf der IMDb für: " + imdb_id)
         return False
 
 
 def get_imdb_id_from_plex_metadata(element, plex_headers):
     metadata = get_url_headers("https://metadata.provider.plex.tv" + element.attrib["key"] + "?includeExternalMedia=1",
                                headers=plex_headers)
     imdb = re.findall(r'id="imdb://(.*?)"', metadata["text"])
     if len(imdb) > 0:
         return imdb[0]
     else:
-        print(u"[Plex] - Metadaten enthalten keine IMDb-ID für: " + element.attrib["title"])
+        print("[Plex] - Metadaten enthalten keine IMDb-ID für: " + element.attrib["title"])
         return None
 
 
 def get_client_id():
     config = CrawlerConfig('Plex')
     client_id = config.get('client_id')
     if client_id:
@@ -106,15 +106,15 @@
             'sort=watchlistedAt:desc'
         ]
 
         metadata_url = 'https://metadata.provider.plex.tv/library/sections/watchlist/all?' + "&".join(params)
         watchlist_content = get_url_headers(metadata_url, headers=plex_headers)
 
         if not watchlist_content["status_code"] == 200:
-            print(u"[Plex] - Fehler beim Abruf der Plex Watchlist: " + watchlist_content["text"])
+            print("[Plex] - Fehler beim Abruf der Plex Watchlist: " + watchlist_content["text"])
             return [0, 0]
 
         watchlist = ElementTree.fromstring(watchlist_content["text"])
 
         requested_movies = []
         requested_shows = []
 
@@ -142,43 +142,43 @@
                                                      language="en", year_in_title=True)
                     if imdb_id:
                         requested_shows.append({
                             "title": title,
                             "imdb_id": imdb_id
                         })
                 else:
-                    print(u"[Plex] - Unbekannter Typ: " + element.attrib["type"] + " - " + element.attrib["title"])
+                    print("[Plex] - Unbekannter Typ: " + element.attrib["type"] + " - " + element.attrib["title"])
 
         len_movies = len(requested_movies)
         len_shows = len(requested_shows)
         if first_launch:
             shared_state.logger.debug("Erfolgreich mit Plex verbunden.")
-            print(u"Erfolgreich mit Plex verbunden.")
+            print("Erfolgreich mit Plex verbunden.")
     except:
         shared_state.logger.debug("Plex ist nicht erreichbar!")
-        print(u"Plex ist nicht erreichbar!")
+        print("Plex ist nicht erreichbar!")
         return [0, 0]
 
     if requested_movies:
         shared_state.logger.debug(
             "Die Suchfunktion für Filme nutzt BY, FX, HW, NK und NX, sofern deren Hostnamen gesetzt wurden.")
     for r in requested_movies:
         imdb_id = r.get("imdb_id")
         if imdb_id:
             if not db.retrieve('movie_' + str(imdb_id)) == 'added':
                 title = imdb_movie(imdb_id)
                 if title:
                     best_result = feedcrawler.external_sites.web_search.content_all.get_best_result(title)
-                    print(u"Film: " + title + u" durch Plex hinzugefügt.")
+                    print("Film: " + title + " durch Plex hinzugefügt.")
                     if best_result:
                         feedcrawler.external_sites.web_search.content_all.download(best_result)
                     if english:
                         title = r.get('title')
                         best_result = feedcrawler.external_sites.web_search.content_all.get_best_result(title)
-                        print(u"Film: " + title + u"durch Plex hinzugefügt.")
+                        print("Film: " + title + "durch Plex hinzugefügt.")
                         if best_result:
                             feedcrawler.external_sites.web_search.content_all.download(best_result)
                     db.store('movie_' + str(imdb_id), 'added')
         else:
             print("Ein Film ohne IMDb-ID wurde in Plex angefordert und kann nicht verarbeitet werden.")
             shared_state.logger.debug(
                 "Ein Film ohne IMDb-ID wurde in Plex angefordert und kann nicht verarbeitet werden.")
@@ -188,21 +188,21 @@
     for r in requested_shows:
         imdb_id = r.get("imdb_id")
         if imdb_id:
             if not db.retrieve('show_' + str(imdb_id)) == 'added':
                 title = imdb_show(imdb_id)
                 if title:
                     best_result = feedcrawler.external_sites.web_search.content_shows.get_best_result(title)
-                    print(u"Serie: " + title + u" durch Plex hinzugefügt.")
+                    print("Serie: " + title + " durch Plex hinzugefügt.")
                     if best_result:
                         feedcrawler.external_sites.web_search.content_shows.download(best_result)
                     if english:
                         title = r.get('title')
                         best_result = feedcrawler.external_sites.web_search.content_shows.get_best_result(title)
-                        print(u"Serie: " + title + u"durch Plex hinzugefügt.")
+                        print("Serie: " + title + "durch Plex hinzugefügt.")
                         if best_result:
                             feedcrawler.external_sites.web_search.content_shows.download(best_result)
                     db.store('show_' + str(imdb_id), 'added')
         else:
             print("Eine Serie ohne IMDb-ID wurde in Plex angefordert und kann nicht verarbeitet werden.")
             shared_state.logger.debug(
                 "Eine Serie ohne IMDb-ID wurde in Plex angefordert und kann nicht verarbeitet werden.")
```

### Comparing `feedcrawler-18.0.1/feedcrawler/jobs/feed_search.py` & `feedcrawler-18.0.2/feedcrawler/jobs/feed_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 from feedcrawler.external_tools.overseerr_api import overseerr_search
 from feedcrawler.external_tools.plex_api import plex_search
 from feedcrawler.providers import gui
 from feedcrawler.providers import shared_state
 from feedcrawler.providers.common_functions import Unbuffered, is_device, readable_time
 from feedcrawler.providers.config import CrawlerConfig
 from feedcrawler.providers.http_requests.cloudflare_handlers import get_solver_url
-from feedcrawler.providers.myjd_connection import get_device
 from feedcrawler.providers.myjd_connection import get_info
 from feedcrawler.providers.myjd_connection import jdownloader_update
+from feedcrawler.providers.myjd_connection import set_device_from_config
 from feedcrawler.providers.sqlite_database import FeedDb
 from feedcrawler.providers.url_functions import check_url
 
 
 def search_pool():
     return [
         FX(filename='IMDb'),
@@ -79,40 +79,39 @@
         SJ(filename='List_ContentAll_Seasons'),
         DJ(filename='List_CustomDJ_Documentaries'),
         DJ(filename='List_CustomDJ_Documentaries_Regex'),
         DD(filename='List_CustomDD_Feeds')
     ]
 
 
-def crawler(shared_print_mem, global_variables, shared_request_dict, shared_device_mem, remove_cloudflare_time,
-            test_run):
-    if gui.enabled and shared_print_mem:
-        sys.stdout = gui.AppendToPrintQueue(shared_print_mem)
+def feed_crawler(shared_state_dict):
+    if gui.enabled:
+        sys.stdout = gui.AppendToPrintQueue(shared_state_dict)
     else:
         sys.stdout = Unbuffered(sys.stdout)
 
-    shared_state.set_request_dict(shared_request_dict)
-    shared_state.set_device_memory(shared_device_mem)
-    shared_state.set_globals(global_variables)
+    shared_state.set_shared_dict(shared_state_dict)
+    shared_state.set_logger()
     logger = shared_state.logger
 
     request_management_first_run = True
     crawltimes = FeedDb("crawltimes")
     feedcrawler = CrawlerConfig('FeedCrawler')
 
-    if remove_cloudflare_time:
-        logger.debug(u"-----------Entferne Zeitpunkt des letzten Cloudflare-Umgehungs-Suchlaufes!-----------")
-        print(u"-----------Entferne Zeitpunkt des letzten Cloudflare-Umgehungs-Suchlaufes!-----------")
+    if shared_state.values["remove_cloudflare_time"]:
+        logger.debug("-----------Entferne Zeitpunkt des letzten Cloudflare-Umgehungs-Suchlaufes!-----------")
+        print("-----------Entferne Zeitpunkt des letzten Cloudflare-Umgehungs-Suchlaufes!-----------")
         FeedDb('crawltimes').delete("last_cloudflare_run")
 
     while True:
         try:
-            if not shared_state.device or not is_device(shared_state.device):
-                get_device()
-            shared_state.request_dict.clear()
+            if not shared_state.values["test_run"]:
+                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                    set_device_from_config()
+            shared_state.clear_request_cache()
             start_time = time.time()
             check_url(start_time)
             crawltimes.update_store("active", "True")
             crawltimes.update_store("start_time", start_time * 1000)
             logger.debug("-----------Alle Suchläufe gestartet.-----------")
 
             # Connect to and run request management services
@@ -120,57 +119,57 @@
             plex_string = ""
             try:
                 plex_results = plex_search(request_management_first_run)
                 requested_movies = plex_results[0]
                 requested_shows = plex_results[1]
                 request_management_first_run = False
                 if requested_movies or requested_shows:
-                    plex_string = u"Die Plex-Suche lief für: "
+                    plex_string = "Die Plex-Suche lief für: "
                     if requested_movies:
                         plex_string = plex_string + str(requested_movies) + " Filme"
                         if requested_shows:
                             plex_string = plex_string + " und "
                     if requested_shows:
                         plex_string = plex_string + str(requested_shows) + " Serien"
             except Exception as e:
-                print(u"Fehler bei der Plex-Suche: " + str(e))
+                print("Fehler bei der Plex-Suche: " + str(e))
 
             overseerr_string = ""
             try:
                 overseerr_results = overseerr_search(request_management_first_run)
                 requested_movies = overseerr_results[0]
                 requested_shows = overseerr_results[1]
                 request_management_first_run = False
                 if requested_movies or requested_shows:
-                    overseerr_string = u"Die Overseerr-Suche lief für: "
+                    overseerr_string = "Die Overseerr-Suche lief für: "
                     if requested_movies:
                         overseerr_string = overseerr_string + str(requested_movies) + " Filme"
                         if requested_shows:
                             overseerr_string = overseerr_string + " und "
                     if requested_shows:
                         overseerr_string = overseerr_string + str(requested_shows) + " Serien"
             except Exception as e:
-                print(u"Fehler bei der Overseerr-Suche: " + str(e))
+                print("Fehler bei der Overseerr-Suche: " + str(e))
             ombi_string = ""
 
             try:
                 ombi_results = ombi_search(request_management_first_run)
                 requested_movies = ombi_results[0]
                 requested_shows = ombi_results[1]
                 request_management_first_run = False
                 if requested_movies or requested_shows:
-                    ombi_string = u"Die Ombi-Suche lief für: "
+                    ombi_string = "Die Ombi-Suche lief für: "
                     if requested_movies:
                         ombi_string = ombi_string + str(requested_movies) + " Filme"
                         if requested_shows:
                             ombi_string = ombi_string + " und "
                     if requested_shows:
                         ombi_string = ombi_string + str(requested_shows) + " Serien"
             except Exception as e:
-                print(u"Fehler bei der Ombi-Suche: " + str(e))
+                print("Fehler bei der Ombi-Suche: " + str(e))
 
             # Start feed search
             current_cloudflare_run = False
             last_cloudflare_run = FeedDb('crawltimes').retrieve("last_cloudflare_run")
             for task in search_pool():
                 name = task._SITE
                 try:
@@ -193,53 +192,61 @@
                         logger.debug("-----------Suchlauf (" + name + file + ") übersprungen!-----------")
                         continue
 
                 logger.debug("-----------Suchlauf (" + name + file + ") gestartet!-----------")
                 try:
                     task.periodical_task()
                 except Exception as e:
-                    print(u"Fehler bei der Feed-Suche: " + str(e))
+                    print("Fehler bei der Feed-Suche: " + str(e))
                 logger.debug("-----------Suchlauf (" + name + file + ") ausgeführt!-----------")
 
             # Finish feed search and log results
             if current_cloudflare_run:
                 crawltimes.update_store("last_cloudflare_run", current_cloudflare_run * 1000)
-            cached_requests = len(shared_state.request_dict)
-            request_cache_string = u"Der FeedCrawler-Cache hat " + str(cached_requests) + " HTTP-Requests gespart!"
+
             end_time = time.time()
             total_time = end_time - start_time
             interval = int(feedcrawler.get('interval')) * 60
             random_range = random.randrange(0, interval // 4)
             wait = interval + random_range
             next_start = end_time + wait
             logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") +
                          " - Alle Suchläufe ausgeführt (Dauer: " + readable_time(
-                total_time) + u")!")
+                total_time) + ")!")
             print(time.strftime("%Y-%m-%d %H:%M:%S") +
-                  u" - Alle Suchläufe ausgeführt (Dauer: " + readable_time(
-                total_time) + u")!")
+                  " - Alle Suchläufe ausgeführt (Dauer: " + readable_time(
+                total_time) + ")!")
 
             if plex_string:
-                logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") + u" - " + plex_string)
-                print(time.strftime("%Y-%m-%d %H:%M:%S") + u" - " + plex_string)
+                logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") + " - " + plex_string)
+                print(time.strftime("%Y-%m-%d %H:%M:%S") + " - " + plex_string)
             if overseerr_string:
-                logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") + u" - " + overseerr_string)
-                print(time.strftime("%Y-%m-%d %H:%M:%S") + u" - " + overseerr_string)
+                logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") + " - " + overseerr_string)
+                print(time.strftime("%Y-%m-%d %H:%M:%S") + " - " + overseerr_string)
             if ombi_string:
-                logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") + u" - " + ombi_string)
-                print(time.strftime("%Y-%m-%d %H:%M:%S") + u" - " + ombi_string)
+                logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") + " - " + ombi_string)
+                print(time.strftime("%Y-%m-%d %H:%M:%S") + " - " + ombi_string)
+
+            try:
+                cache_hits = str(shared_state.values["request_cache_hits"])
+                request_cache_string = "Der FeedCrawler-Cache hat " + str(cache_hits) + " HTTP-Requests gespart!"
+            except KeyError:
+                request_cache_string = "Der FeedCrawler-Cache hat keine HTTP-Requests gespart!"
 
-            logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") + u" - " + request_cache_string)
+            logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") + " - " + request_cache_string)
             logger.debug("-----------Wartezeit bis zum nächsten Suchlauf: " + readable_time(wait) + '-----------')
-            print(u"-----------Wartezeit bis zum nächsten Suchlauf: " + readable_time(wait) + '-----------')
+            print(time.strftime("%Y-%m-%d %H:%M:%S") + " - " + request_cache_string)
+            print("-----------Wartezeit bis zum nächsten Suchlauf: " + readable_time(wait) + '-----------')
+
             crawltimes.update_store("end_time", end_time * 1000)
             crawltimes.update_store("total_time", readable_time(total_time))
             crawltimes.update_store("next_start", next_start * 1000)
             crawltimes.update_store("active", "False")
-            shared_state.request_dict.clear()
+
+            shared_state.clear_request_cache()
 
             myjd_auto_update = feedcrawler.get("myjd_auto_update")
             if myjd_auto_update:
                 myjd_infos = get_info()
                 myjd_state = myjd_infos[1]
                 myjd_grabber_collecting = myjd_infos[2]
                 myjd_update_ready = myjd_infos[3]
@@ -250,28 +257,28 @@
                         "JDownloader Update steht bereit und JDownloader ist inaktiv.\nFühre Update durch und starte JDownloader neu...")
                     jdownloader_update()
                 elif myjd_update_ready:
                     print(
                         "JDownloader Update steht bereit, aber JDownloader ist aktiv.\nFühre das Update nicht automatisch durch.")
             hide_donation_banner = CrawlerConfig('SponsorsHelper').get('hide_donation_banner')
             if hide_donation_banner:
-                current_donation_banner_setting = shared_state.device.config.get(
+                current_donation_banner_setting = shared_state.values["device"].config.get(
                     'org.jdownloader.settings.GraphicalUserInterfaceSettings',
                     'null',
                     'DonateButtonState')
                 if current_donation_banner_setting != "CUSTOM_HIDDEN":
                     print("Blende das Spenden-Banner im JDownloader aus.")
-                    shared_state.device.config.set('org.jdownloader.settings.GraphicalUserInterfaceSettings',
-                                                   'null',
-                                                   'DonateButtonState', "CUSTOM_HIDDEN")
+                    shared_state.values["device"].config.set('org.jdownloader.settings.GraphicalUserInterfaceSettings',
+                                                             'null',
+                                                             'DonateButtonState', "CUSTOM_HIDDEN")
 
             # Clean exit if test run active
-            if test_run:
-                logger.debug(u"-----------test_run beendet!-----------")
-                print(u"-----------test_run beendet!-----------")
+            if shared_state.values["test_run"]:
+                logger.debug("-----------Testlauf beendet!-----------")
+                print("-----------Testlauf beendet!-----------")
                 return
 
             # Wait until next start
             wait_chunks = wait // 10
             start_now_triggered = False
             while wait_chunks:
                 try:
```

### Comparing `feedcrawler-18.0.1/feedcrawler/jobs/package_watcher.py` & `feedcrawler-18.0.2/feedcrawler/jobs/package_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,47 +11,46 @@
 from feedcrawler.providers import gui
 from feedcrawler.providers import shared_state
 from feedcrawler.providers.common_functions import Unbuffered
 from feedcrawler.providers.common_functions import is_device
 from feedcrawler.providers.common_functions import longest_substr
 from feedcrawler.providers.config import CrawlerConfig
 from feedcrawler.providers.myjd_connection import add_decrypt
-from feedcrawler.providers.myjd_connection import get_device
 from feedcrawler.providers.myjd_connection import get_info
 from feedcrawler.providers.myjd_connection import hoster_check
 from feedcrawler.providers.myjd_connection import jdownloader_start
 from feedcrawler.providers.myjd_connection import move_to_downloads
 from feedcrawler.providers.myjd_connection import remove_from_linkgrabber
 from feedcrawler.providers.myjd_connection import rename_package_in_linkgrabber
 from feedcrawler.providers.myjd_connection import reset_in_downloads
 from feedcrawler.providers.myjd_connection import retry_decrypt
+from feedcrawler.providers.myjd_connection import set_device_from_config
 from feedcrawler.providers.notifications import notify
 from feedcrawler.providers.sqlite_database import FeedDb
 
 
-def watch_packages(shared_print_mem, global_variables, shared_request_dict, shared_device_mem):
-    if gui.enabled and shared_print_mem:
-        sys.stdout = gui.AppendToPrintQueue(shared_print_mem)
+def watch_packages(shared_state_dict):
+    if gui.enabled:
+        sys.stdout = gui.AppendToPrintQueue(shared_state_dict)
     else:
         sys.stdout = Unbuffered(sys.stdout)
 
-    shared_state.set_request_dict(shared_request_dict)
-    shared_state.set_device_memory(shared_device_mem)
-    shared_state.set_globals(global_variables)
+    shared_state.set_shared_dict(shared_state_dict)
+    shared_state.set_logger()
 
     crawljobs = CrawlerConfig('Crawljobs')
     autostart = crawljobs.get("autostart")
     db = FeedDb('crawldog')
 
     grabber_was_collecting = False
 
     while True:
         try:
-            if not shared_state.device or not is_device(shared_state.device):
-                get_device()
+            if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                set_device_from_config()
 
             myjd_packages = get_info()
             if myjd_packages:
                 grabber_collecting = myjd_packages[2]
 
                 if grabber_was_collecting or grabber_collecting:
                     grabber_was_collecting = grabber_collecting
@@ -257,15 +256,15 @@
                                                                   [package['uuid']])
                                             db.delete(title[0])
 
                                 if offline_packages:
                                     for package in offline_packages:
                                         if title[0] in package['name'] or title[0].replace(".", " ") in package['name']:
                                             notify_list.append({"text": "[Offline] - " + title[0]})
-                                            print((u"[Offline] - " + title[0]))
+                                            print(("[Offline] - " + title[0]))
                                             db.delete(title[0])
 
                                 if encrypted_packages:
                                     for package in encrypted_packages:
                                         if title[0] in package['name'] or title[0].replace(".", " ") in package['name']:
                                             if title[1] == 'added':
                                                 if retry_decrypt(package['linkids'],
@@ -274,22 +273,22 @@
                                                     db.delete(title[0])
                                                     db.store(title[0], 'retried')
                                             else:
                                                 add_decrypt(package['name'], package['url'], "")
                                                 remove_from_linkgrabber(package['linkids'],
                                                                         [package['uuid']])
                                                 notify_list.append({"text": "[CAPTCHA zu lösen] - " + title[0]})
-                                                print(u"[CAPTCHA zu lösen] - " + title[0])
+                                                print("[CAPTCHA zu lösen] - " + title[0])
                                                 db.delete(title[0])
 
                         if encrypted_packages:
                             for package in encrypted_packages:
                                 if package['zero_byte_files']:
                                     reset_in_downloads(package['zero_byte_files'], [package['uuid']])
-                                    print(u'Falsch als "Fertig" markierte Dateien mit 0 Byte Größe in ' + package[
+                                    print('Falsch als "Fertig" markierte Dateien mit 0 Byte Größe in ' + package[
                                         'name'] + " wurden zurückgesetzt.")
                                     if autostart:
                                         time.sleep(5)
                                         jdownloader_start()
                     else:
                         if not grabber_collecting:
                             db.reset()
@@ -302,12 +301,12 @@
                 except KeyboardInterrupt:
                     break
             else:
                 try:
                     time.sleep(30)
                 except KeyboardInterrupt:
                     break
-                if not get_device():
-                    print(u"Scheinbar ist der JDownloader nicht erreichbar.")
+                if not set_device_from_config():
+                    print("Scheinbar ist der JDownloader nicht erreichbar.")
         except Exception:
             traceback.print_exc()
             time.sleep(30)
```

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/common_functions.py` & `feedcrawler-18.0.2/feedcrawler/providers/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,15 +503,15 @@
     elif os.path.exists(pathfile):
         f = open(pathfile, "r")
         configpath = f.readline()
     else:
         if gui.enabled:
             configpath = gui.configpath_gui(current_path)
         else:
-            print(u"Wo sollen Einstellungen und Logs abgelegt werden? Leer lassen, um den aktuellen Pfad zu nutzen.")
+            print("Wo sollen Einstellungen und Logs abgelegt werden? Leer lassen, um den aktuellen Pfad zu nutzen.")
             configpath = input("Pfad angeben:")
         if len(configpath) > 0:
             f = open(pathfile, "w")
             f.write(configpath)
             f.close()
     if len(configpath) == 0:
         configpath = current_path
@@ -526,24 +526,24 @@
         os.makedirs(configpath)
     return configpath
 
 
 def site_blocked(url):
     db_status = FeedDb('site_status')
     site = check_is_site(url)
-    for check_against in shared_state.sites:
+    for check_against in shared_state.values["sites"]:
         if site and check_against == site and db_status.retrieve(check_against + "_normal"):
             return True
     return False
 
 
 def site_blocked_with_advanced_methods(url):
     db_status = FeedDb('site_status')
     site = check_is_site(url)
-    for check_against in shared_state.sites:
+    for check_against in shared_state.values["sites"]:
         if site and check_against == site and db_status.retrieve(check_against + "_advanced"):
             return True
     return False
 
 
 def simplified_search_term_in_title(search_term, release_title, no_numbers=False):
     if no_numbers:
```

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/config.py` & `feedcrawler-18.0.2/feedcrawler/providers/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,27 +127,27 @@
         'CustomF': [
             ("search", "int", "3"),
         ]
     }
     __config__ = []
 
     def __init__(self, section):
-        self._configfile = shared_state.configfile
+        self._configfile = shared_state.values["configfile"]
         self._section = section
         self._config = configparser.RawConfigParser()
         try:
             self._config.read(self._configfile)
             self._config.has_section(
                 self._section) or self._set_default_config(self._section)
             self.__config__ = self._read_config(self._section)
         except configparser.DuplicateSectionError:
-            print(u'Doppelte Sektion in der Konfigurationsdatei.')
+            print('Doppelte Sektion in der Konfigurationsdatei.')
             raise
         except:
-            print(u'Ein unbekannter Fehler in der Konfigurationsdatei ist aufgetreten.')
+            print('Ein unbekannter Fehler in der Konfigurationsdatei ist aufgetreten.')
             raise
 
     def _set_default_config(self, section):
         self._config.add_section(section)
         for (key, key_type, value) in self._DEFAULT_CONFIG[section]:
             self._config.set(section, key, value)
         with open(self._configfile, 'w') as configfile:
```

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/gui.py` & `feedcrawler-18.0.2/feedcrawler/providers/gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,24 +18,33 @@
 
     enabled = True
 except ImportError:
     enabled = False
 
 if platform.system() == 'Windows':
     font = ('Consolas', 12)
-    myappid = 'feedcrawler'  # arbitrary string
-    ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
+    ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID('FeedCrawler')
 elif platform.system() == 'Linux':
     font = ('Monospace', 12)
 else:
     font = ('Monaco', 12)
 
 title = 'FeedCrawler v.' + get_version()
 
 
+def check_gui_enabled(func):
+    def wrapper(*args, **kwargs):
+        if enabled:
+            return func(*args, **kwargs)
+        else:
+            return False
+
+    return wrapper
+
+
 def get_icon_path():
     base_dir = './feedcrawler'
     if getattr(sys, 'frozen', False):
         base_dir = os.path.join(sys._MEIPASS).replace("\\", "/")
 
     icon_path = base_dir + '/web_interface/vuejs_frontend/dist/favicon.ico'
     return icon_path
@@ -45,14 +54,15 @@
     icon_path = get_icon_path()
     with open(icon_path, 'rb') as f:
         icon_data = f.read()
     icon_base64 = base64.b64encode(icon_data)
     return icon_base64
 
 
+@check_gui_enabled
 def create_main_window():
     sg.theme('dark grey 9')
     sg.set_options(font=font)
 
     layout = [
         [sg.Multiline(size=(100, 20), key="-OUTPUT-", background_color="grey20", text_color="white", font=font,
                       autoscroll=True, )],
@@ -67,15 +77,16 @@
                        icon=get_icon_path())
 
     window.hide()
 
     return window
 
 
-def main_gui(window, shared_mem):
+@check_gui_enabled
+def main_gui(window, shared_state_dict):
     if not window:
         print("GUI-Fenster falsch initialisiert.")
         window = create_main_window()
     try:
         menu = ['', [title,
                      '---',
                      'GUI',
@@ -85,15 +96,15 @@
                 ]
         tray = SystemTray(menu, single_click_events=False, window=window, tooltip='Tooltip', icon=get_icon())
         tray.show_message(title, 'Gestartet und im Tray verfügbar.')
 
         while True:
             event, values = window.read(timeout=500)
 
-            print_from_queue(shared_mem)
+            print_from_queue(shared_state_dict)
 
             if event == tray.key:
                 event = values[event]  # use the System Tray's event as if was from the window
 
             if event in 'Beenden':
                 break
 
@@ -110,30 +121,32 @@
         tray.close()
         window.close()
 
     except KeyboardInterrupt:
         pass
 
 
+@check_gui_enabled
 def get_devices(myjd_user, myjd_pass):
     import feedcrawler.external_tools.myjd_api
     from feedcrawler.external_tools.myjd_api import TokenExpiredException, RequestTimeoutException, MYJDException
 
     jd = feedcrawler.external_tools.myjd_api.Myjdapi()
     jd.set_app_key('FeedCrawler')
     try:
         jd.connect(myjd_user, myjd_pass)
         jd.update_devices()
         devices = jd.list_devices()
         return devices
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
+        print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return []
 
 
+@check_gui_enabled
 def no_hostnames_gui(configfile):
     # warn user if no hostnames are configured
     sg.theme('dark grey 9')
     layout = [
         [sg.Text('Keine Hostnamen in der FeedCrawler.ini gefunden! Beende FeedCrawler!')],
         [sg.Button('OK', bind_return_key=True)]
     ]
@@ -144,14 +157,15 @@
     while True:
         event, values = window.read()
         if event == sg.WIN_CLOSED:
             break
         window.close()
 
 
+@check_gui_enabled
 def configpath_gui(current_path):
     configpath = ''
 
     sg.theme('dark grey 9')
     layout = [
         [sg.Button('"' + current_path + '" verwenden', bind_return_key=True)],
         [sg.Input(key='-FOLDER-', enable_events=True, visible=False),
@@ -168,14 +182,15 @@
         window.close()
 
     if not configpath:
         configpath = ''
     return configpath
 
 
+@check_gui_enabled
 def myjd_credentials_gui():
     user = ''
     password = ''
     device = ''
 
     sg.theme('dark grey 9')
     layout = [
@@ -234,27 +249,43 @@
         user = ""
         password = ""
         device = ""
     return user, password, device
 
 
 class PrintToGui(object):
-    def __init__(self, widget):
+    def __init__(self, widget, max_lines=999):
         self.widget = widget
+        self.max_lines = max_lines
+        self.line_count = 0
 
     def write(self, text):
         try:
             output = self.widget.get()
         except:
             output = ''
-        if len(output) > 0:
-            output += '\n'
+
+        # Split text into individual lines
+        lines = text.split('\n')
+
+        # Add each line to the output
+        for line in lines:
+            if len(line) > 0:
+                if self.line_count >= self.max_lines:
+                    # Remove oldest line
+                    output_lines = output.split('\n')
+                    output = '\n'.join(output_lines[1:])
+                else:
+                    self.line_count += 1
+                output += '\n' + line
+                if output.startswith('\n'):
+                    output = output[1:]
 
         try:
-            self.widget.update(value=output + text)
+            self.widget.update(value=output)
         except:
             pass
 
     def flush(self):
         pass
 
 
@@ -285,22 +316,29 @@
         self.gui.write(message)
 
     def flush(self):
         pass
 
 
 class AppendToPrintQueue(object):
-    def __init__(self, shared_mem):
-        self.shared_mem = shared_mem
+    def __init__(self, shared_state_dict):
+        self.shared_state_dict = shared_state_dict
+        try:
+            self.shared_state_dict["print_queue"]
+        except KeyError:
+            self.shared_state_dict["print_queue"] = ''
 
     def write(self, s):
-        self.shared_mem.value += s.encode('utf-8')
+        self.shared_state_dict["print_queue"] += s
 
     def flush(self):
-        self.shared_mem.value += b''
+        self.shared_state_dict["print_queue"] += ''
 
 
-def print_from_queue(shared_mem):
-    output = shared_mem.value.decode('utf-8')
-    if len(output) > 0:
-        print(output)
-        shared_mem.value = b''
+def print_from_queue(shared_state_dict):
+    try:
+        output = shared_state_dict["print_queue"]
+        if len(output) > 0:
+            print(output)
+            shared_state_dict["print_queue"] = ''
+    except KeyError:
+        pass
```

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/http_requests/cache_handler.py` & `feedcrawler-18.0.2/feedcrawler/providers/http_requests/cache_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # -*- coding: utf-8 -*-
 # FeedCrawler
 # Projekt von https://github.com/rix1337
 # Dieses Modul sorgt durch Caching dafür, dass derselbe Request nur einmal pro Suchlauf an den Server geht.
 
-import codecs
-import hashlib
-import pickle
-import sys
 from functools import wraps
 from urllib.error import URLError
 
 from feedcrawler.providers import shared_state
 from feedcrawler.providers.common_functions import check_is_site
 from feedcrawler.providers.common_functions import site_blocked, site_blocked_with_advanced_methods
 from feedcrawler.providers.http_requests.cloudflare_handlers import flaresolverr_task
@@ -21,40 +17,36 @@
 
 
 def cache(func):
     """Decorator that caches a functions return values for specific arguments."""
 
     @wraps(func)
     def cache_returned_values(*args, **kwargs):
-        to_hash = ""
-        dont_cache = False
-        for a in args:
-            to_hash += codecs.encode(pickle.dumps(a), "base64").decode()
-        for k in kwargs:
-            to_hash += codecs.encode(pickle.dumps(k), "base64").decode()
-            to_hash += codecs.encode(pickle.dumps(kwargs[k]), "base64").decode()
-            if k == "dont_cache" and k:
-                dont_cache = True
-        # This hash is based on all arguments of the request
-        hashed = hashlib.sha256(to_hash.encode('ascii', 'ignore')).hexdigest()
+        if "dont_cache" in kwargs and kwargs["dont_cache"]:
+            caching_allowed = False
+        else:
+            caching_allowed = True
+
+        function_arguments_hash = str(hash(str(args) + str(kwargs)))
 
         try:
-            cached = shared_state.request_dict[hashed]
+            cached_response = shared_state.values["request_" + function_arguments_hash]
         except KeyError:
-            cached = None
-        if cached:
-            # Unpack and return the cached result instead of processing the request
-            cached_response = pickle.loads(codecs.decode(cached.encode(), "base64"))
+            cached_response = None
+        if cached_response:
+            try:
+                shared_state.values["request_cache_hits"] += 1
+            except KeyError:
+                shared_state.values["request_cache_hits"] = 1
             return cached_response
         else:
             #
             value = func(*args, **kwargs)
-            if not dont_cache:
-                cached_response = codecs.encode(pickle.dumps(value), "base64").decode()
-                shared_state.request_dict[hashed] = cached_response
+            if caching_allowed:
+                shared_state.values["request_" + function_arguments_hash] = value
             return value
 
     return cache_returned_values
 
 
 @cache
 def cached_request(url, method='get', params=None, headers=None, redirect_url=False, dont_cache=False):
@@ -75,15 +67,15 @@
     if "ajax" in url.lower():
         headers['X-Requested-With'] = 'XMLHttpRequest'
 
     status_code = 500
     text = ""
     response_headers = {}
 
-    headers['User-Agent'] = shared_state.user_agent
+    headers['User-Agent'] = shared_state.values["user_agent"]
     cookiejar = None
     proxies = {}
     force_ipv4 = False
 
     flaresolverr_run = False
     allow_sponsors_helper_run = False
     if sponsors_helper_url and not flaresolverr_url:
```

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/http_requests/cloudflare_handlers.py` & `feedcrawler-18.0.2/feedcrawler/providers/http_requests/cloudflare_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,16 @@
                     return cookiejar, user_agent, proxy
             else:
                 clean_db("sponsors_helper", base_domain)
         except:
             pass
 
     if test_solver_url("sponsors_helper", solver_url + "/status"):
-        shared_state.logger.debug("Versuche Cloudflare auf der Seite %s mit Sponsors Helper zu umgehen..." % url)
+        shared_state.logger.debug(
+            "Versuche Cloudflare auf der Seite %s mit Sponsors Helper zu umgehen..." % url)
 
         solver_endpoint = "/cloudflare_cookie/"
         solver_payload = {
             'url': "https://" + base_domain + test_challenge_path(url)
         }
 
         response = request(
@@ -208,23 +209,25 @@
     last_solution = unpickle_db("flaresolverr", base_domain)
     if last_solution:
         try:
             if last_solution["valid_until"] > int(time.time()):
                 cookiejar = cookie_dict_to_cookiejar(last_solution["cookies"])
                 user_agent = last_solution["user_agent"]
                 if cookiejar:
-                    shared_state.logger.debug("Bestehende Cloudflare-Cookies werden für " + url + " verwendet.")
+                    shared_state.logger.debug(
+                        "Bestehende Cloudflare-Cookies werden für " + url + " verwendet.")
                     return cookiejar, user_agent
             else:
                 clean_db("flaresolverr", base_domain)
         except:
             pass
 
     if test_solver_url("flaresolverr", solver_url):
-        shared_state.logger.debug("Versuche Cloudflare auf der Seite %s mit  FlareSolverr zu umgehen..." % url)
+        shared_state.logger.debug(
+            "Versuche Cloudflare auf der Seite %s mit  FlareSolverr zu umgehen..." % url)
 
         solver_endpoint = "/v1"
         solver_payload = {
             'cmd': 'request.get',
             'url': "https://" + base_domain + test_challenge_path(url)
         }
```

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/http_requests/request_handler.py` & `feedcrawler-18.0.2/feedcrawler/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/notifications.py` & `feedcrawler-18.0.2/feedcrawler/providers/notifications.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/sqlite_database.py` & `feedcrawler-18.0.2/feedcrawler/providers/sqlite_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,35 +47,34 @@
 
     tables_to_drop = set(table_names) - set(keep_tables)
 
     for table in tables_to_drop:
         cursor.execute(f"DROP TABLE IF EXISTS {table}")
         print(f"Entferne überflüssige Tabelle '{table}' aus der Datenbank.")
 
-
     conn.commit()
     cursor.execute("VACUUM")
     conn.close()
 
 
 class FeedDb(object):
     def __init__(self, table):
         try:
-            self._conn = sqlite3.connect(shared_state.dbfile, check_same_thread=False, timeout=5)
+            self._conn = sqlite3.connect(shared_state.values["dbfile"], check_same_thread=False, timeout=5)
             self._table = table
             if not self._conn.execute(
                     "SELECT sql FROM sqlite_master WHERE type = 'table' AND name = '%s';" % self._table).fetchall():
                 self._conn.execute("CREATE TABLE %s (key, value)" % self._table)
                 self._conn.commit()
         except sqlite3.OperationalError as e:
             try:
                 shared_state.logger.debug(
                     "Fehler bei Zugriff auf FeedCrawler.db: " + str(e) + " (neuer Versuch in 5 Sekunden).")
                 time.sleep(5)
-                self._conn = sqlite3.connect(shared_state.dbfile, check_same_thread=False, timeout=10)
+                self._conn = sqlite3.connect(shared_state.values["dbfile"], check_same_thread=False, timeout=10)
                 self._table = table
                 if not self._conn.execute(
                         "SELECT sql FROM sqlite_master WHERE type = 'table' AND name = '%s';" % self._table).fetchall():
                     self._conn.execute("CREATE TABLE %s (key, value)" % self._table)
                     self._conn.commit()
                     shared_state.logger.debug("Zugriff auf FeedCrawler.db nach Wartezeit war erfolgreich.")
             except sqlite3.OperationalError as e:
@@ -147,15 +146,15 @@
         self._conn.execute("ALTER TABLE '%s' RENAME TO '%s'" %
                            (self._table, new_name))
         self._conn.commit()
 
 
 class ListDb(object):
     def __init__(self, table):
-        self._conn = sqlite3.connect(shared_state.dbfile, check_same_thread=False, timeout=10)
+        self._conn = sqlite3.connect(shared_state.values["dbfile"], check_same_thread=False, timeout=10)
         self._table = table
         if not self._conn.execute(
                 "SELECT sql FROM sqlite_master WHERE type = 'table' AND name = '%s';" % self._table).fetchall():
             self._conn.execute(
                 '''CREATE TABLE %s (key)''' % self._table)
             self._conn.commit()
```

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/url_functions.py` & `feedcrawler-18.0.2/feedcrawler/providers/url_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from feedcrawler.providers.sqlite_database import FeedDb
 
 
 def check_url(start_time):
     hostnames = CrawlerConfig('Hostnames')
     db_status = FeedDb('site_status')
 
-    for site in shared_state.sites:
+    for site in shared_state.values["sites"]:
         if site in ["SJ", "DJ", "SF", "FF", "HW", "WW"]:  # all sites know to use cloudflare
             last_cloudflare_run = FeedDb('crawltimes').retrieve("last_cloudflare_run")
             cloudflare_wait_time = int(CrawlerConfig('Cloudflare').get('wait_time'))
             if last_cloudflare_run and start_time < float(last_cloudflare_run) // 1000 + cloudflare_wait_time * 60 * 60:
                 shared_state.logger.debug(
                     "-----------Wartezeit bei " + site + " (6h) nicht verstrichen - überspringe Prüfung!-----------")
                 continue
@@ -31,39 +31,39 @@
             db_status.update_store(site + "_normal", "Blocked")
             db_status.update_store(site + "_advanced", "Blocked")
         else:
             db_status.delete(site + "_normal")
             db_status.delete(site + "_advanced")
             sponsors_helper_url = get_solver_url("sponsors_helper")
             flaresolverr_url = get_solver_url("flaresolverr")
-            skip_sites = ["SF", "FF", "HW", "WW", ]  # SJ/DJ not listed, because they rarely block scraping attempts
+            skip_sites = ["HW", "WW", ]  # SJ/DJ not listed, because they rarely block scraping attempts
             skip_normal_ip = (sponsors_helper_url or flaresolverr_url) and (site in skip_sites)
             if skip_normal_ip:
                 blocked_with_normal_ip = True
             else:
                 blocked_with_normal_ip = check_if_blocked(site, "https://" + hostname)
             if not blocked_with_normal_ip:
-                print(u"Der Zugriff auf " + site + " funktioniert!")
+                print("Der Zugriff auf " + site + " funktioniert!")
             else:
                 if skip_normal_ip:
-                    print(u"Der Zugriff auf " + site + " ist nur mit FlareSolverr bzw. Sponsors Helper möglich!")
+                    print("Der Zugriff auf " + site + " ist nur mit FlareSolverr bzw. Sponsors Helper möglich!")
                 else:
-                    print(u"Der Zugriff auf " + site + " ist gesperrt!")
+                    print("Der Zugriff auf " + site + " ist gesperrt!")
                 db_status.update_store(site + "_normal", "Blocked")
                 if not sponsors_helper_url and not flaresolverr_url:
                     print(
-                        u"Der Zugriff auf " + site + " ist ohne FlareSolverr bzw. Sponsors Helper derzeit nicht möglich!")
+                        "Der Zugriff auf " + site + " ist ohne FlareSolverr bzw. Sponsors Helper derzeit nicht möglich!")
                     db_status.update_store(site + "_advanced", "Blocked")
                 else:
                     # Since we are aware this site is blocked Sponsors Helper/FlareSolverr will be used for subsequent requests
                     still_blocked = check_if_blocked(site, "https://" + hostname)
                     if not still_blocked:
-                        print(u"Die Cloudflare-Blockade auf " + site + " wurde erfolgreich umgangen!")
+                        print("Die Cloudflare-Blockade auf " + site + " wurde erfolgreich umgangen!")
                     else:
-                        print(u"Die Cloudflare-Blockade auf " + site + " konnte nicht umgangen werden!")
+                        print("Die Cloudflare-Blockade auf " + site + " konnte nicht umgangen werden!")
                         db_status.update_store(site + "_advanced", "Blocked")
 
 
 def check_if_blocked(site, url):
     try:
         # These can be checked the same way
         if site in ["FX", "DW", "BY", "NK", "NX", "DD"]:
@@ -93,68 +93,68 @@
                     200 or 304) or '<span class="main-rls">' not in ww_test["text"]:
                 return True
         elif site in ["SJ", "DJ"]:
             status = cached_request(url + '/api/releases/latest/0', dont_cache=True)["status_code"]
             if status is not (200 or 304):
                 return True
         else:
-            print(u"Keine Prüfung für " + site + " implementiert.")
+            print("Keine Prüfung für " + site + " implementiert.")
     except:
         return True
     return False
 
 
 def get_url(url):
     if url:
         try:
             response = cached_request(url)["text"]
             return response
         except Exception as e:
-            print(u"Fehler beim Abruf von: " + str(url) + " " + str(e))
+            print("Fehler beim Abruf von: " + str(url) + " " + str(e))
             pass
     return ""
 
 
 def get_url_headers(url, headers=False):
     if url:
         try:
             response = cached_request(url, headers=headers)
             return response
         except Exception as e:
-            print(u"Fehler beim Abruf von: " + url + " " + str(e))
+            print("Fehler beim Abruf von: " + url + " " + str(e))
     return ""
 
 
 def get_redirected_url(url):
     if url:
         try:
             redirect_url = cached_request(url, redirect_url=True)["url"]
             return redirect_url
         except Exception as e:
-            print(u"Fehler beim Abruf von: " + url + " " + str(e))
+            print("Fehler beim Abruf von: " + url + " " + str(e))
     return url
 
 
 def post_url(url, data=False):
     if url:
         try:
             response = cached_request(url, method='post', params=data)["text"]
             return response
         except Exception as e:
-            print(u"Fehler beim Abruf von: " + url + " " + str(e))
+            print("Fehler beim Abruf von: " + url + " " + str(e))
     return ""
 
 
 def post_url_headers(url, headers, data=False):
     if url:
         try:
             response = cached_request(url, method='post', params=data, headers=headers)
             return response
         except Exception as e:
-            print(u"Fehler beim Abruf von: " + url + " " + str(e))
+            print("Fehler beim Abruf von: " + url + " " + str(e))
     return ""
 
 
 def get_urls_async(urls):
     results = []
 
     def load_url(url):
```

### Comparing `feedcrawler-18.0.1/feedcrawler/providers/version.py` & `feedcrawler-18.0.2/feedcrawler/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "18.0.1"
+    return "18.0.2"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/index.html` & `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/feedcrawler/web_interface/web_server.py` & `feedcrawler-18.0.2/feedcrawler/web_interface/web_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 from feedcrawler.providers.common_functions import is_device
 from feedcrawler.providers.common_functions import keep_alphanumeric_with_regex_characters
 from feedcrawler.providers.common_functions import keep_alphanumeric_with_special_characters
 from feedcrawler.providers.common_functions import keep_numbers
 from feedcrawler.providers.common_functions import remove_decrypt
 from feedcrawler.providers.common_functions import rreplace
 from feedcrawler.providers.config import CrawlerConfig
-from feedcrawler.providers.myjd_connection import check_device
+from feedcrawler.providers.myjd_connection import set_device
 from feedcrawler.providers.myjd_connection import do_add_decrypted
 from feedcrawler.providers.myjd_connection import download
-from feedcrawler.providers.myjd_connection import get_device
+from feedcrawler.providers.myjd_connection import set_device_from_config
 from feedcrawler.providers.myjd_connection import get_if_one_device
 from feedcrawler.providers.myjd_connection import get_info
 from feedcrawler.providers.myjd_connection import get_packages_in_linkgrabber
 from feedcrawler.providers.myjd_connection import get_state
 from feedcrawler.providers.myjd_connection import jdownloader_pause
 from feedcrawler.providers.myjd_connection import jdownloader_start
 from feedcrawler.providers.myjd_connection import jdownloader_stop
@@ -109,15 +109,15 @@
     global auth_user
     global auth_hash
     global known_hashes
 
     base_dir = './feedcrawler'
     if getattr(sys, 'frozen', False):
         base_dir = os.path.join(sys._MEIPASS).replace("\\", "/")
-    elif shared_state.docker:
+    elif shared_state.values["docker"]:
         static_location = site.getsitepackages()[0]
         base_dir = static_location + "/feedcrawler"
 
     general = CrawlerConfig('FeedCrawler')
     if general.get("prefix"):
         prefix = '/' + general.get("prefix")
     else:
@@ -259,16 +259,16 @@
         return to_bool(str(db.retrieve(site)).replace("Blocked", "True"))
 
     @app.get(prefix + "/api/log/")
     @auth_basic(is_authenticated_user)
     def get_log():
         try:
             log = []
-            if os.path.isfile(shared_state.log_file):
-                logfile = open(shared_state.log_file)
+            if os.path.isfile(shared_state.values["log_file"]):
+                logfile = open(shared_state.values["log_file"])
                 i = 0
                 for line in reversed(logfile.readlines()):
                     if line and line != "\n":
                         payload = [i]
                         line = line.replace("]", "")
                         line = line.replace("[", "")
                         line = re.sub(r",\d{3}", "", line)
@@ -284,33 +284,33 @@
         except:
             return abort(400, "Failed")
 
     @app.delete(prefix + "/api/log/")
     @auth_basic(is_authenticated_user)
     def delete_log():
         try:
-            open(shared_state.log_file, 'w').close()
+            open(shared_state.values["log_file"], 'w').close()
             return "Success"
         except:
             return abort(400, "Failed")
 
     @app.delete(prefix + "/api/log_entry/<b64_entry>")
     @auth_basic(is_authenticated_user)
     def delete_log_entry(b64_entry):
         try:
             entry = decode_base64(b64_entry)
             log = []
-            if os.path.isfile(shared_state.log_file):
-                logfile = open(shared_state.log_file)
+            if os.path.isfile(shared_state.values["log_file"]):
+                logfile = open(shared_state.values["log_file"])
                 for line in reversed(logfile.readlines()):
                     if line and line != "\n":
                         if entry not in line:
                             log.append(line)
                 log = "".join(reversed(log))
-                with open(shared_state.log_file, 'w') as file:
+                with open(shared_state.values["log_file"], 'w') as file:
                     file.write(log)
             return "Success"
         except:
             return abort(400, "Failed")
 
     @app.get(prefix + "/api/settings/")
     @auth_basic(is_authenticated_user)
@@ -459,24 +459,24 @@
             myjd_user = to_str(data['general']['myjd_user'])
             myjd_pass = to_str(data['general']['myjd_pass'])
             myjd_device = to_str(data['general']['myjd_device'])
 
             if myjd_user and myjd_pass and not myjd_device:
                 myjd_device = get_if_one_device(myjd_user, myjd_pass)
                 if myjd_device:
-                    print(u"Gerätename " + myjd_device + " automatisch ermittelt.")
+                    print("Gerätename " + myjd_device + " automatisch ermittelt.")
 
             if myjd_user and myjd_pass and myjd_device:
-                device_check = check_device(myjd_user, myjd_pass, myjd_device)
+                device_check = set_device(myjd_user, myjd_pass, myjd_device)
                 if not device_check:
                     myjd_device = get_if_one_device(myjd_user, myjd_pass)
                     if myjd_device:
-                        print(u"Gerätename " + myjd_device + " automatisch ermittelt.")
+                        print("Gerätename " + myjd_device + " automatisch ermittelt.")
                     else:
-                        print(u"Fehlerhafte My JDownloader Zugangsdaten. Bitte vor dem Speichern prüfen!")
+                        print("Fehlerhafte My JDownloader Zugangsdaten. Bitte vor dem Speichern prüfen!")
                         return abort(400, "Failed")
 
             myjd_auto_update = to_str(data['general']['myjd_auto_update'])
 
             section.save("myjd_user", myjd_user)
             section.save("myjd_pass", myjd_pass)
             section.save("myjd_device", myjd_device)
@@ -706,23 +706,23 @@
     @auth_basic(is_authenticated_user)
     def get_version():
         try:
             ver = "v." + version.get_version()
             if version.update_check()[0]:
                 updateready = True
                 updateversion = version.update_check()[1]
-                print(u'Update steht bereit (' + updateversion +
+                print('Update steht bereit (' + updateversion +
                       ')! Weitere Informationen unter https://github.com/rix1337/FeedCrawler/releases/latest')
             else:
                 updateready = False
             return {
                 "version": {
                     "ver": ver,
                     "update_ready": updateready,
-                    "docker": shared_state.docker,
+                    "docker": shared_state.values["docker"],
                     "helper_active": helper_active
                 }
             }
         except:
             return abort(400, "Failed")
 
     @app.get(prefix + "/api/crawltimes/")
@@ -785,15 +785,15 @@
                     return value
 
             cloudflare_shorthands = []
             for site_name in cloudflare.split(" / "):
                 site_shorthand = check_is_site(site_name)
                 if site_shorthand:
                     cloudflare_shorthands.append(site_shorthand)
-            cloudflare_shorthands = " / ".join(cloudflare_shorthands)
+            cloudflare_shorthands = "/".join(cloudflare_shorthands)
 
             return {
                 "hostnames": {
                     "fx": check_if_set(fx),
                     "sf": check_if_set(sf),
                     "dw": check_if_set(dw),
                     "hw": check_if_set(hw),
@@ -948,16 +948,16 @@
         try:
             try:
                 myjd = get_info()
                 packages_to_decrypt = get_to_decrypt()
                 general_conf = CrawlerConfig('FeedCrawler')
                 packages_per_myjd_page = to_int(general_conf.get("packages_per_myjd_page"))
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
-                get_device()
-                if not shared_state.device or not is_device(shared_state.device):
+                set_device_from_config()
+                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
                     return abort(500, "Failed")
                 myjd = get_info()
                 packages_to_decrypt = get_to_decrypt()
                 packages_per_myjd_page = 3
             if myjd:
                 return {
                     "downloader_state": myjd[1],
@@ -979,16 +979,16 @@
     @app.get(prefix + "/api/myjd_state/")
     @auth_basic(is_authenticated_user)
     def myjd_state():
         try:
             try:
                 myjd = get_state()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
-                get_device()
-                if not shared_state.device or not is_device(shared_state.device):
+                set_device_from_config()
+                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
                     return abort(500, "Failed")
                 myjd = get_state()
             if myjd:
                 return {
                     "downloader_state": myjd[1],
                     "grabber_collecting": myjd[2]
                 }
@@ -1159,16 +1159,16 @@
     @app.post(prefix + "/api/myjd_start/")
     @auth_basic(is_authenticated_user)
     def myjd_start():
         try:
             try:
                 started = jdownloader_start()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
-                get_device()
-                if not shared_state.device or not is_device(shared_state.device):
+                set_device_from_config()
+                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
                     return abort(500, "Failed")
                 started = jdownloader_start()
             if started:
                 return "Success"
         except:
             pass
         return abort(400, "Failed")
@@ -1177,16 +1177,16 @@
     @auth_basic(is_authenticated_user)
     def myjd_pause(bl):
         try:
             bl = json.loads(bl)
             try:
                 paused = jdownloader_pause(bl)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
-                get_device()
-                if not shared_state.device or not is_device(shared_state.device):
+                set_device_from_config()
+                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
                     return abort(500, "Failed")
                 paused = jdownloader_pause(bl)
             if paused:
                 return "Success"
         except:
             pass
         return abort(400, "Failed")
@@ -1194,16 +1194,16 @@
     @app.post(prefix + "/api/myjd_stop/")
     @auth_basic(is_authenticated_user)
     def myjd_stop():
         try:
             try:
                 stopped = jdownloader_stop()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
-                get_device()
-                if not shared_state.device or not is_device(shared_state.device):
+                set_device_from_config()
+                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
                     return abort(500, "Failed")
                 stopped = jdownloader_stop()
             if stopped:
                 return "Success"
         except:
             pass
         return abort(400, "Failed")
@@ -1211,16 +1211,16 @@
     @app.post(prefix + "/api/myjd_update/")
     @auth_basic(is_authenticated_user)
     def myjd_update():
         try:
             try:
                 updated = jdownloader_update()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
-                get_device()
-                if not shared_state.device or not is_device(shared_state.device):
+                set_device_from_config()
+                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
                     return abort(500, "Failed")
                 updated = jdownloader_update()
             if updated:
                 return "Success"
         except:
             pass
         return abort(400, "Failed")
@@ -1421,15 +1421,15 @@
 // @match           https://""" + dj + """/*
 // @exclude         https://""" + sj + """/serie/search?q=*
 // @exclude         https://""" + dj + """/serie/search?q=*
 // @grant           window.close
 // ==/UserScript==
 
 // Hier muss die von außen erreichbare Adresse des FeedCrawlers stehen (nicht bspw. die Docker-interne):
-const sponsorsURL = '""" + shared_state.local_address + """';
+const sponsorsURL = '""" + shared_state.values["local_address"] + """';
 // Hier kann ein Wunschhoster eingetragen werden (ohne www. und .tld):
 const sponsorsHoster = '';
 
 $.extend($.expr[':'], {
 'containsi': function(elem, i, match, array) {
 return (elem.textContent || elem.innerText || '').toLowerCase()
     .indexOf((match[3] || "").toLowerCase()) >= 0;
@@ -1530,15 +1530,15 @@
 // @exclude         http://filecrypt.cc/helper.html*
 // @exclude         http://filecrypt.co/helper.html*
 // @exclude         http://filecrypt.to/helper.html*
 // @grant           window.close
 // ==/UserScript==
 
 // Hier muss die von außen erreichbare Adresse des FeedCrawlers stehen (nicht bspw. die Docker-interne):
-const sponsorsURL = '""" + shared_state.local_address + """';
+const sponsorsURL = '""" + shared_state.values["local_address"] + """';
 // Hier kann ein Wunschhoster eingetragen werden (ohne www. und .tld):
 const sponsorsHoster = '';
 
 const tag = window.location.hash.replace("#", "").split('|');
 const title = tag[0];
 const password = tag[1];
 const ids = tag[2];
@@ -1659,15 +1659,15 @@
 // @description     Forwards decrypted links to FeedCrawler
 // @version         0.1.1
 // @require         https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js
 // @match           https://""" + nx + """/release/*
 // @grant           window.close
 // ==/UserScript==
 // Hier muss die von außen erreichbare Adresse des FeedCrawlers stehen (nicht bspw. die Docker-interne):
-const sponsorsURL = '""" + shared_state.local_address + """';
+const sponsorsURL = '""" + shared_state.values["local_address"] + """';
 
 function Sleep(milliseconds) {
     return new Promise(resolve => setTimeout(resolve, milliseconds));
 }
 
 var tag = window.location.hash.replace("#", "").split('|');
 var title = tag[0];
@@ -1742,17 +1742,17 @@
                 name.encode("ascii", errors="ignore").decode().replace("/", "").replace(" ", ".")
                 max_attempts = str(CrawlerConfig('SponsorsHelper').get("max_attempts"))
                 if remove_decrypt(name):
                     try:
                         notify([{
                             "text": "[CAPTCHA nicht gelöst] - " + name + " (Paket nach " + max_attempts + " Versuchen gelöscht)"}])
                     except:
-                        print(u"Benachrichtigung konnte nicht versendet werden!")
+                        print("Benachrichtigung konnte nicht versendet werden!")
                     print(
-                        u"[CAPTCHA nicht gelöst] - " + name + " (Paket nach " + max_attempts + " Versuchen gelöscht)")
+                        "[CAPTCHA nicht gelöst] - " + name + " (Paket nach " + max_attempts + " Versuchen gelöscht)")
                     return "<script type='text/javascript'>" \
                            "function closeWindow(){window.close()}window.onload=closeWindow;</script>" \
                            "[CAPTCHA nicht gelöst] - " + name + " (Paket nach " + max_attempts + " Versuchen gelöscht)"
         except:
             pass
         return abort(400, "Failed")
 
@@ -1856,22 +1856,22 @@
 
             result = attempt_download(package_name, links, password, ids)
             return result
         except:
             pass
         return abort(400, "Failed")
 
-    Server(app, listen='0.0.0.0', port=shared_state.port).serve_forever()
+    Server(app, listen='0.0.0.0', port=shared_state.values["port"]).serve_forever()
 
 
 def attempt_download(package_name, links, password, ids):
     global already_added
 
     FeedDb('crawldog').store(package_name, 'added')
-    if shared_state.device:
+    if shared_state.values["device"]:
         if ids:
             try:
                 ids = ids.replace("%20", "").split(";")
                 linkids = ids[0]
                 uuids = ids[1]
             except:
                 linkids = False
@@ -1919,16 +1919,16 @@
             if season_string:
                 season_string = season_string[0].replace("s", "S")
             else:
                 season_string = "^unmatchable$"
             try:
                 packages = get_packages_in_linkgrabber()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
-                get_device()
-                if not shared_state.device or not is_device(shared_state.device):
+                set_device_from_config()
+                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
                     return abort(500, "Failed")
                 packages = get_packages_in_linkgrabber()
 
             if packages:
                 failed = packages[0]
                 offline = packages[1]
 
@@ -1984,50 +1984,49 @@
             time.sleep(1)
             remove_decrypt(package_name)
         try:
             epoch = int(time.time())
             for item in already_added:
                 if item[0] == package_name:
                     if int(item[1]) + 5 > epoch:
-                        print(package_name + u" wurde in den letzten 5 Sekunden bereits hinzugefügt")
-                        return abort(500, package_name + u" wurde in den letzten 5 Sekunden bereits hinzugefügt")
+                        print(package_name + " wurde in den letzten 5 Sekunden bereits hinzugefügt")
+                        return abort(500, package_name + " wurde in den letzten 5 Sekunden bereits hinzugefügt")
                     else:
                         already_added.remove(item)
 
             download(package_name, "FeedCrawler", links, password)
             db = FeedDb('FeedCrawler')
             if not db.retrieve(package_name):
                 db.store(package_name, 'added')
             try:
                 notify([{"text": "[CAPTCHA gelöst] - " + package_name}])
             except:
-                print(u"Benachrichtigung konnte nicht versendet werden!")
-            print(u"[CAPTCHA gelöst] - " + package_name)
+                print("Benachrichtigung konnte nicht versendet werden!")
+            print("[CAPTCHA gelöst] - " + package_name)
             already_added.append([package_name, str(epoch)])
             return "<script type='text/javascript'>" \
                    "function closeWindow(){window.close()}window.onload=closeWindow;</script>" \
                    "[CAPTCHA gelöst] - " + package_name
         except:
-            print(package_name + u" konnte nicht hinzugefügt werden!")
-            return abort(500, package_name + u" konnte nicht hinzugefügt werden!")
+            print(package_name + " konnte nicht hinzugefügt werden!")
+            return abort(500, package_name + " konnte nicht hinzugefügt werden!")
 
 
 def start():
     if version.update_check()[0]:
         updateversion = version.update_check()[1]
-        print(u'Update steht bereit (' + updateversion +
+        print('Update steht bereit (' + updateversion +
               ')! Weitere Informationen unter https://github.com/rix1337/FeedCrawler/releases/latest')
 
     app_container()
 
 
-def web_server(shared_print_mem, global_variables, shared_request_dict, shared_device_mem):
-    if gui.enabled and shared_print_mem:
-        sys.stdout = gui.AppendToPrintQueue(shared_print_mem)
+def web_server(shared_state_dict):
+    if gui.enabled:
+        sys.stdout = gui.AppendToPrintQueue(shared_state_dict)
     else:
         sys.stdout = Unbuffered(sys.stdout)
 
-    shared_state.set_request_dict(shared_request_dict)
-    shared_state.set_device_memory(shared_device_mem)
-    shared_state.set_globals(global_variables)
+    shared_state.set_shared_dict(shared_state_dict)
+    shared_state.set_logger()
 
     start()
```

### Comparing `feedcrawler-18.0.1/feedcrawler.egg-info/PKG-INFO` & `feedcrawler-18.0.2/feedcrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.1
+Version: 18.0.2
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedcrawler-18.0.1/feedcrawler.egg-info/SOURCES.txt` & `feedcrawler-18.0.2/feedcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.1/setup.py` & `feedcrawler-18.0.2/setup.py`

 * *Files identical despite different names*

