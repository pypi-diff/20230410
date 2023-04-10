# Comparing `tmp/deezer_downloader-2.0.2.tar.gz` & `tmp/deezer_downloader-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_downloader-2.0.2.tar", max compression
+gzip compressed data, was "deezer_downloader-2.0.3.tar", max compression
```

## Comparing `deezer_downloader-2.0.2.tar` & `deezer_downloader-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/LICENSE
--rw-r--r--   0        0        0     7712 2023-04-09 20:58:29.658538 deezer_downloader-2.0.2/README.md
--rw-r--r--   0        0        0     1272 2023-04-09 20:57:18.943593 deezer_downloader-2.0.2/deezer_downloader/cli/deezer-downloader.ini.template
--rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.2/deezer_downloader/cli/runner.py
--rw-r--r--   0        0        0     1170 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/configuration.py
--rw-r--r--   0        0        0    20706 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/deezer.py
--rw-r--r--   0        0        0     4855 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/spotify.py
--rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/threadpool_queue.py
--rw-r--r--   0        0        0    10129 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/web/app.py
--rw-r--r--   0        0        0    10617 2023-04-09 20:20:53.021110 deezer_downloader-2.0.2/deezer_downloader/web/music_backend.py
--rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
--rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/font-awesome.min.css
--rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/css/jquery.jgrowl.min.css
--rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/favicon.ico
--rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.2/deezer_downloader/web/static/js/bootstrap.min.js
--rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/static/js/custom.js
--rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/static/js/jquery.jgrowl.min.js
--rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/static/js/jquery.min.js
--rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/static/js/popper.min.js
--rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/web/templates/autoindex.html
--rw-r--r--   0        0        0     8734 2023-04-09 20:59:58.143865 deezer_downloader-2.0.2/deezer_downloader/web/templates/index.html
--rw-r--r--   0        0        0     1856 2023-04-09 20:20:53.027777 deezer_downloader-2.0.2/deezer_downloader/youtubedl.py
--rw-r--r--   0        0        0      943 2023-04-10 10:08:19.034709 deezer_downloader-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     8734 1970-01-01 00:00:00.000000 deezer_downloader-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/LICENSE
+-rw-r--r--   0        0        0     7712 2023-04-09 20:58:29.658538 deezer_downloader-2.0.3/README.md
+-rw-r--r--   0        0        0     1272 2023-04-09 20:57:18.943593 deezer_downloader-2.0.3/deezer_downloader/cli/deezer-downloader.ini.template
+-rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.3/deezer_downloader/cli/runner.py
+-rw-r--r--   0        0        0     1170 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/configuration.py
+-rw-r--r--   0        0        0    20706 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/deezer.py
+-rw-r--r--   0        0        0     4855 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/spotify.py
+-rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/threadpool_queue.py
+-rw-r--r--   0        0        0    10129 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/web/app.py
+-rw-r--r--   0        0        0    10617 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/web/music_backend.py
+-rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
+-rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/font-awesome.min.css
+-rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/jquery.jgrowl.min.css
+-rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/favicon.ico
+-rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/static/js/custom.js
+-rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/static/js/jquery.jgrowl.min.js
+-rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/static/js/jquery.min.js
+-rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/static/js/popper.min.js
+-rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/templates/autoindex.html
+-rw-r--r--   0        0        0     8735 2023-04-10 10:27:40.860066 deezer_downloader-2.0.3/deezer_downloader/web/templates/index.html
+-rw-r--r--   0        0        0     1856 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/youtubedl.py
+-rw-r--r--   0        0        0      943 2023-04-10 10:28:46.714332 deezer_downloader-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8734 1970-01-01 00:00:00.000000 deezer_downloader-2.0.3/PKG-INFO
```

### Comparing `deezer_downloader-2.0.2/LICENSE` & `deezer_downloader-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/README.md` & `deezer_downloader-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/cli/deezer-downloader.ini.template` & `deezer_downloader-2.0.3/deezer_downloader/cli/deezer-downloader.ini.template`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/cli/runner.py` & `deezer_downloader-2.0.3/deezer_downloader/cli/runner.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/configuration.py` & `deezer_downloader-2.0.3/deezer_downloader/configuration.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/deezer.py` & `deezer_downloader-2.0.3/deezer_downloader/deezer.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/spotify.py` & `deezer_downloader-2.0.3/deezer_downloader/spotify.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/threadpool_queue.py` & `deezer_downloader-2.0.3/deezer_downloader/threadpool_queue.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/app.py` & `deezer_downloader-2.0.3/deezer_downloader/web/app.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/music_backend.py` & `deezer_downloader-2.0.3/deezer_downloader/web/music_backend.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip` & `deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap.bundle.min.js` & `deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/css/bootstrap.min.css` & `deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/css/font-awesome.min.css` & `deezer_downloader-2.0.3/deezer_downloader/web/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/css/jquery.jgrowl.min.css` & `deezer_downloader-2.0.3/deezer_downloader/web/static/css/jquery.jgrowl.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2` & `deezer_downloader-2.0.3/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/js/bootstrap.min.js` & `deezer_downloader-2.0.3/deezer_downloader/web/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/js/custom.js` & `deezer_downloader-2.0.3/deezer_downloader/web/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/js/jquery.jgrowl.min.js` & `deezer_downloader-2.0.3/deezer_downloader/web/static/js/jquery.jgrowl.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/js/jquery.min.js` & `deezer_downloader-2.0.3/deezer_downloader/web/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/static/js/popper.min.js` & `deezer_downloader-2.0.3/deezer_downloader/web/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/deezer_downloader/web/templates/index.html` & `deezer_downloader-2.0.3/deezer_downloader/web/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,17 @@
 
         <div class="input-group">
             <div class="col-md-6 col-lg-5 col-xs-12">
                 <input type="text" class="form-control" id="songs-albums-query" placeholder="Search for ..." >
             </div>
             <div class="col-md-6 col-xs-12">
                 <span class="input-group-btn">
+                    <button type="button" class="btn btn-info" id="search_track">Search Track</button>
                     <button type="button" class="btn btn-info" id="search_album">Search Album</button>
-                    <button type="button" class="btn btn-info" id="search_album">Search Album</button>
+
                     <button type="button" class="btn btn-info" onclick="$('#songs-albums-query').val('')" id="clear_search">Clear</button>
                 </span>
             </div>
         </div>
         
          </br>
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
     * Files_(5)
     * Debug_(6)
     * Queue_(7)
 
 
 **** Download songs and albums ****
 [                    ]
- Search Album Search Album Clear
+ Search Track Search Album Clear
 Artist Title Album
 
 **** Download stuff via youtube-dl ****
 [                    ]  
 
  Download & Play Download Clear
```

### Comparing `deezer_downloader-2.0.2/deezer_downloader/youtubedl.py` & `deezer_downloader-2.0.3/deezer_downloader/youtubedl.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.2/pyproject.toml` & `deezer_downloader-2.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-downloader"
-version = "2.0.2"
+version = "2.0.3"
 description = "download music from Deezer with a nice front end"
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 packages = [{include = "deezer_downloader"}]
 repository = "https://github.com/kmille/deezer-downloader"
 homepage = "https://github.com/kmille/deezer-downloader"
```

### Comparing `deezer_downloader-2.0.2/PKG-INFO` & `deezer_downloader-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deezer-downloader
-Version: 2.0.2
+Version: 2.0.3
 Summary: download music from Deezer with a nice front end
 Home-page: https://github.com/kmille/deezer-downloader
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

