# Comparing `tmp/deezer_downloader-2.0.1.tar.gz` & `tmp/deezer_downloader-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_downloader-2.0.1.tar", max compression
+gzip compressed data, was "deezer_downloader-2.0.2.tar", max compression
```

## Comparing `deezer_downloader-2.0.1.tar` & `deezer_downloader-2.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.1/LICENSE
--rw-r--r--   0        0        0     7712 2023-04-09 20:58:29.658538 deezer_downloader-2.0.1/README.md
--rw-r--r--   0        0        0     1272 2023-04-09 20:57:18.943593 deezer_downloader-2.0.1/deezer_downloader/cli/deezer-downloader.ini.template
--rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.1/deezer_downloader/cli/runner.py
--rw-r--r--   0        0        0     1170 2023-04-09 20:20:53.021110 deezer_downloader-2.0.1/deezer_downloader/configuration.py
--rw-r--r--   0        0        0    20706 2023-04-09 20:20:53.021110 deezer_downloader-2.0.1/deezer_downloader/deezer.py
--rw-r--r--   0        0        0     4855 2023-04-09 20:20:53.021110 deezer_downloader-2.0.1/deezer_downloader/spotify.py
--rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.1/deezer_downloader/threadpool_queue.py
--rw-r--r--   0        0        0    10129 2023-04-09 20:20:53.021110 deezer_downloader-2.0.1/deezer_downloader/web/app.py
--rw-r--r--   0        0        0    10617 2023-04-09 20:20:53.021110 deezer_downloader-2.0.1/deezer_downloader/web/music_backend.py
--rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.1/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
--rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.1/deezer_downloader/web/static/css/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.1/deezer_downloader/web/static/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.1/deezer_downloader/web/static/css/font-awesome.min.css
--rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.1/deezer_downloader/web/static/css/jquery.jgrowl.min.css
--rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.1/deezer_downloader/web/static/favicon.ico
--rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.1/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.1/deezer_downloader/web/static/js/bootstrap.min.js
--rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.1/deezer_downloader/web/static/js/custom.js
--rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.1/deezer_downloader/web/static/js/jquery.jgrowl.min.js
--rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.1/deezer_downloader/web/static/js/jquery.min.js
--rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.1/deezer_downloader/web/static/js/popper.min.js
--rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.1/deezer_downloader/web/templates/autoindex.html
--rw-r--r--   0        0        0     8734 2023-04-09 20:59:58.143865 deezer_downloader-2.0.1/deezer_downloader/web/templates/index.html
--rw-r--r--   0        0        0     1856 2023-04-09 20:20:53.027777 deezer_downloader-2.0.1/deezer_downloader/youtubedl.py
--rw-r--r--   0        0        0      944 2023-04-10 09:58:03.507886 deezer_downloader-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     8585 1970-01-01 00:00:00.000000 deezer_downloader-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/LICENSE
+-rw-r--r--   0        0        0     7712 2023-04-09 20:58:29.658538 deezer_downloader-2.0.2/README.md
+-rw-r--r--   0        0        0     1272 2023-04-09 20:57:18.943593 deezer_downloader-2.0.2/deezer_downloader/cli/deezer-downloader.ini.template
+-rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.2/deezer_downloader/cli/runner.py
+-rw-r--r--   0        0        0     1170 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/configuration.py
+-rw-r--r--   0        0        0    20706 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/deezer.py
+-rw-r--r--   0        0        0     4855 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/spotify.py
+-rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/threadpool_queue.py
+-rw-r--r--   0        0        0    10129 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/web/app.py
+-rw-r--r--   0        0        0    10617 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/web/music_backend.py
+-rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
+-rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/font-awesome.min.css
+-rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/jquery.jgrowl.min.css
+-rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/favicon.ico
+-rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/static/js/custom.js
+-rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/static/js/jquery.jgrowl.min.js
+-rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/static/js/jquery.min.js
+-rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/static/js/popper.min.js
+-rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/templates/autoindex.html
+-rw-r--r--   0        0        0     8734 2023-04-09 20:59:58.143865 deezer_downloader-2.0.2/deezer_downloader/web/templates/index.html
+-rw-r--r--   0        0        0     1856 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/youtubedl.py
+-rw-r--r--   0        0        0      943 2023-04-10 10:08:19.034709 deezer_downloader-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8734 1970-01-01 00:00:00.000000 deezer_downloader-2.0.2/PKG-INFO
```

### Comparing `deezer_downloader-2.0.1/LICENSE` & `deezer_downloader-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/README.md` & `deezer_downloader-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/cli/deezer-downloader.ini.template` & `deezer_downloader-2.0.2/deezer_downloader/cli/deezer-downloader.ini.template`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/cli/runner.py` & `deezer_downloader-2.0.2/deezer_downloader/cli/runner.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/configuration.py` & `deezer_downloader-2.0.2/deezer_downloader/configuration.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/deezer.py` & `deezer_downloader-2.0.2/deezer_downloader/deezer.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/spotify.py` & `deezer_downloader-2.0.2/deezer_downloader/spotify.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/threadpool_queue.py` & `deezer_downloader-2.0.2/deezer_downloader/threadpool_queue.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/app.py` & `deezer_downloader-2.0.2/deezer_downloader/web/app.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/music_backend.py` & `deezer_downloader-2.0.2/deezer_downloader/web/music_backend.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip` & `deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/css/bootstrap.bundle.min.js` & `deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/css/bootstrap.min.css` & `deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/css/font-awesome.min.css` & `deezer_downloader-2.0.2/deezer_downloader/web/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/css/jquery.jgrowl.min.css` & `deezer_downloader-2.0.2/deezer_downloader/web/static/css/jquery.jgrowl.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2` & `deezer_downloader-2.0.2/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/js/bootstrap.min.js` & `deezer_downloader-2.0.2/deezer_downloader/web/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/js/custom.js` & `deezer_downloader-2.0.2/deezer_downloader/web/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/js/jquery.jgrowl.min.js` & `deezer_downloader-2.0.2/deezer_downloader/web/static/js/jquery.jgrowl.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/js/jquery.min.js` & `deezer_downloader-2.0.2/deezer_downloader/web/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/static/js/popper.min.js` & `deezer_downloader-2.0.2/deezer_downloader/web/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/web/templates/index.html` & `deezer_downloader-2.0.2/deezer_downloader/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/deezer_downloader/youtubedl.py` & `deezer_downloader-2.0.2/deezer_downloader/youtubedl.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.1/pyproject.toml` & `deezer_downloader-2.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "deezer-downloader"
-version = "2.0.1"
+version = "2.0.2"
 description = "download music from Deezer with a nice front end"
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 packages = [{include = "deezer_downloader"}]
 repository = "https://github.com/kmille/deezer-downloader"
 homepage = "https://github.com/kmille/deezer-downloader"
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.7"
 requests = "^2.28.1"
 flask = "^2.2.2"
 python-mpd2 = "^3.0.5"
 yt-dlp = "*"
 pycryptodome = "^3.16.0"
 jinja2 = "^3.1.2"
 flask-autoindex = "^0.6.6"
```

### Comparing `deezer_downloader-2.0.1/PKG-INFO` & `deezer_downloader-2.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: deezer-downloader
-Version: 2.0.1
+Version: 2.0.2
 Summary: download music from Deezer with a nice front end
 Home-page: https://github.com/kmille/deezer-downloader
 Author: kmille
 Author-email: github@androidloves.me
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flask (>=2.2.2,<3.0.0)
 Requires-Dist: flask-autoindex (>=0.6.6,<0.7.0)
 Requires-Dist: giphypop (>=0.3,<0.4)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pycryptodome (>=3.16.0,<4.0.0)
```

