# Comparing `tmp/nudecrawler-0.3.7.tar.gz` & `tmp/nudecrawler-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudecrawler-0.3.7.tar", last modified: Mon Apr 10 19:05:56 2023, max compression
+gzip compressed data, was "nudecrawler-0.3.8.tar", last modified: Mon Apr 10 19:14:11 2023, max compression
```

## Comparing `nudecrawler-0.3.7.tar` & `nudecrawler-0.3.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    15568 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)    15056 2023-04-10 19:04:56.000000 nudecrawler-0.3.7/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.316023 nudecrawler-0.3.7/bin/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1458 2023-03-25 09:35:46.000000 nudecrawler-0.3.7/bin/detect-image-aid.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2497 2023-03-25 11:06:28.000000 nudecrawler-0.3.7/bin/detect-image-nsfw-api.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1527 2023-04-10 13:36:55.000000 nudecrawler-0.3.7/bin/detect-image-nudenet.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3527 2023-04-10 14:42:15.000000 nudecrawler-0.3.7/bin/detect-server-nudenet.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)    16115 2023-04-10 19:05:28.000000 nudecrawler-0.3.7/bin/nudecrawler
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      217 2023-04-01 23:30:57.000000 nudecrawler-0.3.7/bin/refresh-nsfw-api.sh
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.316023 nudecrawler-0.3.7/nudecrawler/
--rw-r--r--   0 xenon     (1000) xenon     (1000)       95 2023-03-20 17:34:21.000000 nudecrawler-0.3.7/nudecrawler/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1990 2023-04-03 19:10:18.000000 nudecrawler-0.3.7/nudecrawler/cache.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      293 2023-03-21 11:11:32.000000 nudecrawler-0.3.7/nudecrawler/exceptions.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      588 2023-03-25 09:36:26.000000 nudecrawler-0.3.7/nudecrawler/localimage.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12822 2023-04-10 18:00:20.000000 nudecrawler-0.3.7/nudecrawler/page.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     3082 2023-04-10 16:46:51.000000 nudecrawler-0.3.7/nudecrawler/remoteimage.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      952 2023-04-03 17:15:52.000000 nudecrawler-0.3.7/nudecrawler/tgru.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      352 2023-02-28 18:19:59.000000 nudecrawler-0.3.7/nudecrawler/unbuffered.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1114 2023-04-08 13:56:10.000000 nudecrawler-0.3.7/nudecrawler/verbose.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)       15 2023-04-10 19:03:16.000000 nudecrawler-0.3.7/nudecrawler/version.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/nudecrawler.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    15568 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      619 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)      104 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/requires.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)      880 2023-04-06 18:16:07.000000 nudecrawler-0.3.7/pyproject.toml
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/setup.cfg
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1688 2023-04-08 18:41:42.000000 nudecrawler-0.3.7/setup.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/tests/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      637 2023-04-03 22:33:06.000000 nudecrawler-0.3.7/tests/test_nudecrawler.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    14950 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    14438 2023-04-10 19:13:30.000000 nudecrawler-0.3.8/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/bin/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1458 2023-03-25 09:35:46.000000 nudecrawler-0.3.8/bin/detect-image-aid.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2497 2023-03-25 11:06:28.000000 nudecrawler-0.3.8/bin/detect-image-nsfw-api.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1527 2023-04-10 13:36:55.000000 nudecrawler-0.3.8/bin/detect-image-nudenet.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3527 2023-04-10 14:42:15.000000 nudecrawler-0.3.8/bin/detect-server-nudenet.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)    16131 2023-04-10 19:10:01.000000 nudecrawler-0.3.8/bin/nudecrawler
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      217 2023-04-01 23:30:57.000000 nudecrawler-0.3.8/bin/refresh-nsfw-api.sh
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/nudecrawler/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       95 2023-03-20 17:34:21.000000 nudecrawler-0.3.8/nudecrawler/__init__.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1990 2023-04-03 19:10:18.000000 nudecrawler-0.3.8/nudecrawler/cache.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      293 2023-03-21 11:11:32.000000 nudecrawler-0.3.8/nudecrawler/exceptions.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      588 2023-03-25 09:36:26.000000 nudecrawler-0.3.8/nudecrawler/localimage.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12822 2023-04-10 18:00:20.000000 nudecrawler-0.3.8/nudecrawler/page.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     3082 2023-04-10 16:46:51.000000 nudecrawler-0.3.8/nudecrawler/remoteimage.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      952 2023-04-03 17:15:52.000000 nudecrawler-0.3.8/nudecrawler/tgru.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      352 2023-02-28 18:19:59.000000 nudecrawler-0.3.8/nudecrawler/unbuffered.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1114 2023-04-08 13:56:10.000000 nudecrawler-0.3.8/nudecrawler/verbose.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       15 2023-04-10 19:13:41.000000 nudecrawler-0.3.8/nudecrawler/version.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/nudecrawler.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    14950 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      619 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      104 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/requires.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/top_level.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      880 2023-04-06 18:16:07.000000 nudecrawler-0.3.8/pyproject.toml
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/setup.cfg
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1688 2023-04-08 18:41:42.000000 nudecrawler-0.3.8/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/tests/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      637 2023-04-03 22:33:06.000000 nudecrawler-0.3.8/tests/test_nudecrawler.py
```

### Comparing `nudecrawler-0.3.7/PKG-INFO` & `nudecrawler-0.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudecrawler
-Version: 0.3.7
+Version: 0.3.8
 Summary: Crawl telegra.ph for nude pictures and videos
 Home-page: https://github.com/yaroslaff/nudecrawler
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,25 +26,27 @@
 Please use it only for legal and ethical purposes. And it's 18+ surely. 
 
 ## Install
 
 Recommended (and most secure) way is using docker:
 ```
 mkdir /tmp/run
-sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha grey" "Belle Delphine" Amouranth
+sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
 ```
 
 See below how to refine your searching and filtering.
 
 ### Alternative install
 ```
 pip3 install nudecrawler
 ```
 
-alternatively, install right from git repo:
+
+
+or, install right from git repo:
 ```
 pip3 install git+https://github.com/yaroslaff/nudecrawler
 ```
 
 ## Launch Nude Crawler!
 
 (I intentionally changed links, do not want to violate github policy)
@@ -66,36 +68,17 @@
 
 ## Refine search/filtering
 Nudecrawler uses [evalidate](https://github.com/yaroslaff/evalidate) to filter results with python expression (`--expr`). With `-h` help will list all avaliable variables, like: `total_images nude_images nonnude_images new_nude_images new_nonnude_images new_total_images total_video`.
 Default value: `(total_images>5 and new_nude_images>0) or total_video>0`.
 
 Use `-a`/`--all` to get some results ASAP (but later you may want to make some filtering)
 
-  -d DAYS, --days DAYS
-
-
-  -f FAILS, --fails FAILS
-  --total N             Boring if less then N total images (5)
-  --max-errors N        Max allowed errors on page ()
-  --min-content-length N
-                        Interesting if N+ total images (5)
-
-Image filtering options:
-  -a, --all             do not detect, print all found pages
-  --detect-image SCRIPT
-                        explicitly use this script to detect nudity on image file
-  --detect-url SCRIPT   explicitly use this script to detect nudity on image URL
-  --detect METHOD       One of true, false, nudepy, nudenetb, aid, nsfwapi, nudenet
-  --extensions [EXTENSIONS ...]
-                        interesting extensions (with dot, like .jpg)
-  --minsize MINSIZE     min size of image in Kb (10)
-  --max-pictures N      Detect only among first prefiltered N pictures
-
-
+Consider using `--days`, `--total` to narrow/wider search.
 
+Also, `--cache`, `--max-pictures`, `--max-errors`, `--min-content-length` and `--minsize` to speed-up searching and discard some images/pages before wasting time on it.
 
 
 ### Long-time run
 
 #### Stop/Resume
 When working with worklists an --stats file, current status is periodically saved to this file. If you need to resume it, just use command `nudecrawler --resume PATH/TO/stats.json`
```

### Comparing `nudecrawler-0.3.7/README.md` & `nudecrawler-0.3.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 Please use it only for legal and ethical purposes. And it's 18+ surely. 
 
 ## Install
 
 Recommended (and most secure) way is using docker:
 ```
 mkdir /tmp/run
-sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha grey" "Belle Delphine" Amouranth
+sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
 ```
 
 See below how to refine your searching and filtering.
 
 ### Alternative install
 ```
 pip3 install nudecrawler
 ```
 
-alternatively, install right from git repo:
+
+
+or, install right from git repo:
 ```
 pip3 install git+https://github.com/yaroslaff/nudecrawler
 ```
 
 ## Launch Nude Crawler!
 
 (I intentionally changed links, do not want to violate github policy)
@@ -50,36 +52,17 @@
 
 ## Refine search/filtering
 Nudecrawler uses [evalidate](https://github.com/yaroslaff/evalidate) to filter results with python expression (`--expr`). With `-h` help will list all avaliable variables, like: `total_images nude_images nonnude_images new_nude_images new_nonnude_images new_total_images total_video`.
 Default value: `(total_images>5 and new_nude_images>0) or total_video>0`.
 
 Use `-a`/`--all` to get some results ASAP (but later you may want to make some filtering)
 
-  -d DAYS, --days DAYS
-
-
-  -f FAILS, --fails FAILS
-  --total N             Boring if less then N total images (5)
-  --max-errors N        Max allowed errors on page ()
-  --min-content-length N
-                        Interesting if N+ total images (5)
-
-Image filtering options:
-  -a, --all             do not detect, print all found pages
-  --detect-image SCRIPT
-                        explicitly use this script to detect nudity on image file
-  --detect-url SCRIPT   explicitly use this script to detect nudity on image URL
-  --detect METHOD       One of true, false, nudepy, nudenetb, aid, nsfwapi, nudenet
-  --extensions [EXTENSIONS ...]
-                        interesting extensions (with dot, like .jpg)
-  --minsize MINSIZE     min size of image in Kb (10)
-  --max-pictures N      Detect only among first prefiltered N pictures
-
-
+Consider using `--days`, `--total` to narrow/wider search.
 
+Also, `--cache`, `--max-pictures`, `--max-errors`, `--min-content-length` and `--minsize` to speed-up searching and discard some images/pages before wasting time on it.
 
 
 ### Long-time run
 
 #### Stop/Resume
 When working with worklists an --stats file, current status is periodically saved to this file. If you need to resume it, just use command `nudecrawler --resume PATH/TO/stats.json`
```

### Comparing `nudecrawler-0.3.7/bin/detect-image-aid.py` & `nudecrawler-0.3.8/bin/detect-image-aid.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/bin/detect-image-nsfw-api.py` & `nudecrawler-0.3.8/bin/detect-image-nsfw-api.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/bin/detect-image-nudenet.py` & `nudecrawler-0.3.8/bin/detect-image-nudenet.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/bin/detect-server-nudenet.py` & `nudecrawler-0.3.8/bin/detect-server-nudenet.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/bin/nudecrawler` & `nudecrawler-0.3.8/bin/nudecrawler`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     parser.add_argument('--day', nargs=2, type=int, metavar=('MONTH', 'DAY'), help='Current date (default is today) example: --day 12 31')
 
     g = parser.add_argument_group('Page filtering options')
     parser.add_argument('--expr', '-e', metavar='EXPR', default=def_expr, 
                         help=f'Interesting if EXPR is True. def: {def_expr!r}\nFields: ' + ' '.join(context_fields) )
     parser.add_argument('--total', metavar='N', type=int, default=def_total, help=f'Boring if less then N total images ({def_total})')
     parser.add_argument('--max-errors', metavar='N', type=int, default=def_errors, help=f'Max allowed errors on page ({def_errors})')
-    parser.add_argument('--min-content-length', metavar='N', type=int, default=None, help=f'Interesting if N+ total images ({def_total})')
+    parser.add_argument('--min-content-length', metavar='N', type=int, default=None, help=f'Skip page if content-length less then N (try 5000 or higher)')
 
     g = parser.add_argument_group('Image filtering options')
     g.add_argument('-a', '--all', default=False, action='store_true', help='do not detect, print all found pages')
     g.add_argument('--detect-image', metavar='SCRIPT', help='explicitly use this script to detect nudity on image file')
     g.add_argument('--detect-url', metavar='SCRIPT', help='explicitly use this script to detect nudity on image URL')
     g.add_argument('--detect', metavar='METHOD', default=def_detect, help=f'One of {methods_list}')
     g.add_argument('--extensions', nargs='*', default=['.jpeg','.jpg', '.png'],help='interesting extensions (with dot, like .jpg)')
```

### Comparing `nudecrawler-0.3.7/nudecrawler/cache.py` & `nudecrawler-0.3.8/nudecrawler/cache.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/nudecrawler/localimage.py` & `nudecrawler-0.3.8/nudecrawler/localimage.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/nudecrawler/page.py` & `nudecrawler-0.3.8/nudecrawler/page.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/nudecrawler/remoteimage.py` & `nudecrawler-0.3.8/nudecrawler/remoteimage.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/nudecrawler/tgru.py` & `nudecrawler-0.3.8/nudecrawler/tgru.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/nudecrawler/verbose.py` & `nudecrawler-0.3.8/nudecrawler/verbose.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/nudecrawler.egg-info/PKG-INFO` & `nudecrawler-0.3.8/nudecrawler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudecrawler
-Version: 0.3.7
+Version: 0.3.8
 Summary: Crawl telegra.ph for nude pictures and videos
 Home-page: https://github.com/yaroslaff/nudecrawler
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,25 +26,27 @@
 Please use it only for legal and ethical purposes. And it's 18+ surely. 
 
 ## Install
 
 Recommended (and most secure) way is using docker:
 ```
 mkdir /tmp/run
-sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha grey" "Belle Delphine" Amouranth
+sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
 ```
 
 See below how to refine your searching and filtering.
 
 ### Alternative install
 ```
 pip3 install nudecrawler
 ```
 
-alternatively, install right from git repo:
+
+
+or, install right from git repo:
 ```
 pip3 install git+https://github.com/yaroslaff/nudecrawler
 ```
 
 ## Launch Nude Crawler!
 
 (I intentionally changed links, do not want to violate github policy)
@@ -66,36 +68,17 @@
 
 ## Refine search/filtering
 Nudecrawler uses [evalidate](https://github.com/yaroslaff/evalidate) to filter results with python expression (`--expr`). With `-h` help will list all avaliable variables, like: `total_images nude_images nonnude_images new_nude_images new_nonnude_images new_total_images total_video`.
 Default value: `(total_images>5 and new_nude_images>0) or total_video>0`.
 
 Use `-a`/`--all` to get some results ASAP (but later you may want to make some filtering)
 
-  -d DAYS, --days DAYS
-
-
-  -f FAILS, --fails FAILS
-  --total N             Boring if less then N total images (5)
-  --max-errors N        Max allowed errors on page ()
-  --min-content-length N
-                        Interesting if N+ total images (5)
-
-Image filtering options:
-  -a, --all             do not detect, print all found pages
-  --detect-image SCRIPT
-                        explicitly use this script to detect nudity on image file
-  --detect-url SCRIPT   explicitly use this script to detect nudity on image URL
-  --detect METHOD       One of true, false, nudepy, nudenetb, aid, nsfwapi, nudenet
-  --extensions [EXTENSIONS ...]
-                        interesting extensions (with dot, like .jpg)
-  --minsize MINSIZE     min size of image in Kb (10)
-  --max-pictures N      Detect only among first prefiltered N pictures
-
-
+Consider using `--days`, `--total` to narrow/wider search.
 
+Also, `--cache`, `--max-pictures`, `--max-errors`, `--min-content-length` and `--minsize` to speed-up searching and discard some images/pages before wasting time on it.
 
 
 ### Long-time run
 
 #### Stop/Resume
 When working with worklists an --stats file, current status is periodically saved to this file. If you need to resume it, just use command `nudecrawler --resume PATH/TO/stats.json`
```

### Comparing `nudecrawler-0.3.7/nudecrawler.egg-info/SOURCES.txt` & `nudecrawler-0.3.8/nudecrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/pyproject.toml` & `nudecrawler-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/setup.py` & `nudecrawler-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.7/tests/test_nudecrawler.py` & `nudecrawler-0.3.8/tests/test_nudecrawler.py`

 * *Files identical despite different names*

