# Comparing `tmp/nudecrawler-0.3.6.tar.gz` & `tmp/nudecrawler-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudecrawler-0.3.6.tar", last modified: Mon Apr 10 18:07:10 2023, max compression
+gzip compressed data, was "nudecrawler-0.3.7.tar", last modified: Mon Apr 10 19:05:56 2023, max compression
```

## Comparing `nudecrawler-0.3.6.tar` & `nudecrawler-0.3.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    14111 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)    13599 2023-04-10 18:02:54.000000 nudecrawler-0.3.6/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/bin/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1458 2023-03-25 09:35:46.000000 nudecrawler-0.3.6/bin/detect-image-aid.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2497 2023-03-25 11:06:28.000000 nudecrawler-0.3.6/bin/detect-image-nsfw-api.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1527 2023-04-10 13:36:55.000000 nudecrawler-0.3.6/bin/detect-image-nudenet.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3527 2023-04-10 14:42:15.000000 nudecrawler-0.3.6/bin/detect-server-nudenet.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)    16034 2023-04-10 17:41:17.000000 nudecrawler-0.3.6/bin/nudecrawler
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      217 2023-04-01 23:30:57.000000 nudecrawler-0.3.6/bin/refresh-nsfw-api.sh
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/nudecrawler/
--rw-r--r--   0 xenon     (1000) xenon     (1000)       95 2023-03-20 17:34:21.000000 nudecrawler-0.3.6/nudecrawler/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1990 2023-04-03 19:10:18.000000 nudecrawler-0.3.6/nudecrawler/cache.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      293 2023-03-21 11:11:32.000000 nudecrawler-0.3.6/nudecrawler/exceptions.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      588 2023-03-25 09:36:26.000000 nudecrawler-0.3.6/nudecrawler/localimage.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12822 2023-04-10 18:00:20.000000 nudecrawler-0.3.6/nudecrawler/page.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     3082 2023-04-10 16:46:51.000000 nudecrawler-0.3.6/nudecrawler/remoteimage.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      952 2023-04-03 17:15:52.000000 nudecrawler-0.3.6/nudecrawler/tgru.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      352 2023-02-28 18:19:59.000000 nudecrawler-0.3.6/nudecrawler/unbuffered.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1114 2023-04-08 13:56:10.000000 nudecrawler-0.3.6/nudecrawler/verbose.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)       15 2023-04-10 18:06:29.000000 nudecrawler-0.3.6/nudecrawler/version.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/nudecrawler.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    14111 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      619 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)      104 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/requires.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)      880 2023-04-06 18:16:07.000000 nudecrawler-0.3.6/pyproject.toml
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/setup.cfg
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1688 2023-04-08 18:41:42.000000 nudecrawler-0.3.6/setup.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/tests/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      637 2023-04-03 22:33:06.000000 nudecrawler-0.3.6/tests/test_nudecrawler.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    15568 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    15056 2023-04-10 19:04:56.000000 nudecrawler-0.3.7/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.316023 nudecrawler-0.3.7/bin/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1458 2023-03-25 09:35:46.000000 nudecrawler-0.3.7/bin/detect-image-aid.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2497 2023-03-25 11:06:28.000000 nudecrawler-0.3.7/bin/detect-image-nsfw-api.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1527 2023-04-10 13:36:55.000000 nudecrawler-0.3.7/bin/detect-image-nudenet.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3527 2023-04-10 14:42:15.000000 nudecrawler-0.3.7/bin/detect-server-nudenet.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)    16115 2023-04-10 19:05:28.000000 nudecrawler-0.3.7/bin/nudecrawler
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      217 2023-04-01 23:30:57.000000 nudecrawler-0.3.7/bin/refresh-nsfw-api.sh
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.316023 nudecrawler-0.3.7/nudecrawler/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       95 2023-03-20 17:34:21.000000 nudecrawler-0.3.7/nudecrawler/__init__.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1990 2023-04-03 19:10:18.000000 nudecrawler-0.3.7/nudecrawler/cache.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      293 2023-03-21 11:11:32.000000 nudecrawler-0.3.7/nudecrawler/exceptions.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      588 2023-03-25 09:36:26.000000 nudecrawler-0.3.7/nudecrawler/localimage.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12822 2023-04-10 18:00:20.000000 nudecrawler-0.3.7/nudecrawler/page.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     3082 2023-04-10 16:46:51.000000 nudecrawler-0.3.7/nudecrawler/remoteimage.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      952 2023-04-03 17:15:52.000000 nudecrawler-0.3.7/nudecrawler/tgru.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      352 2023-02-28 18:19:59.000000 nudecrawler-0.3.7/nudecrawler/unbuffered.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1114 2023-04-08 13:56:10.000000 nudecrawler-0.3.7/nudecrawler/verbose.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       15 2023-04-10 19:03:16.000000 nudecrawler-0.3.7/nudecrawler/version.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/nudecrawler.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    15568 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      619 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      104 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/requires.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-04-10 19:05:56.000000 nudecrawler-0.3.7/nudecrawler.egg-info/top_level.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      880 2023-04-06 18:16:07.000000 nudecrawler-0.3.7/pyproject.toml
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/setup.cfg
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1688 2023-04-08 18:41:42.000000 nudecrawler-0.3.7/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:05:56.320023 nudecrawler-0.3.7/tests/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      637 2023-04-03 22:33:06.000000 nudecrawler-0.3.7/tests/test_nudecrawler.py
```

### Comparing `nudecrawler-0.3.6/PKG-INFO` & `nudecrawler-0.3.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,29 @@
-Metadata-Version: 2.1
-Name: nudecrawler
-Version: 0.3.6
-Summary: Crawl telegra.ph for nude pictures and videos
-Home-page: https://github.com/yaroslaff/nudecrawler
-Author: Yaroslav Polyakov
-Author-email: yaroslaff@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: nudenet
-
 # nude crawler
 
 Nude crawler crawls all pages on telegra.ph for today and N past days for specific words, checks number of nude, non-nude images, videos (not analysed) and reports pages which looks interesting (e.g. has more then 10 nude images, or has one video)
 
 ## Ineffective intriguing warning
 No matter how old you are, no matter how tolerant you are, no matter what your sexual orientation is, no matter what your favorite perversion is, no matter how big your sexual horizons are, with NudeCrawler you will find a lot of things that **you will NOT like**.
 
 I wrote this warning because I have seen some shit. LITERALLY.
 
 Please use it only for legal and ethical purposes. And it's 18+ surely. 
 
 ## Install
 
+Recommended (and most secure) way is using docker:
+```
+mkdir /tmp/run
+sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha grey" "Belle Delphine" Amouranth
+```
+
+See below how to refine your searching and filtering.
+
+### Alternative install
 ```
 pip3 install nudecrawler
 ```
 
 alternatively, install right from git repo:
 ```
 pip3 install git+https://github.com/yaroslaff/nudecrawler
@@ -51,18 +44,44 @@
 INTERESTING https://telegra.ph/sasha-grey-XXXXX
   Nude: 9 non-nude: 6
 
 INTERESTING https://telegra.ph/sasha-grey-XXXXX
   Nude: 6 non-nude: 3
 ~~~
 
-## Getting only interesting results
+## Refine search/filtering
 Nudecrawler uses [evalidate](https://github.com/yaroslaff/evalidate) to filter results with python expression (`--expr`). With `-h` help will list all avaliable variables, like: `total_images nude_images nonnude_images new_nude_images new_nonnude_images new_total_images total_video`.
 Default value: `(total_images>5 and new_nude_images>0) or total_video>0`.
 
+Use `-a`/`--all` to get some results ASAP (but later you may want to make some filtering)
+
+  -d DAYS, --days DAYS
+
+
+  -f FAILS, --fails FAILS
+  --total N             Boring if less then N total images (5)
+  --max-errors N        Max allowed errors on page ()
+  --min-content-length N
+                        Interesting if N+ total images (5)
+
+Image filtering options:
+  -a, --all             do not detect, print all found pages
+  --detect-image SCRIPT
+                        explicitly use this script to detect nudity on image file
+  --detect-url SCRIPT   explicitly use this script to detect nudity on image URL
+  --detect METHOD       One of true, false, nudepy, nudenetb, aid, nsfwapi, nudenet
+  --extensions [EXTENSIONS ...]
+                        interesting extensions (with dot, like .jpg)
+  --minsize MINSIZE     min size of image in Kb (10)
+  --max-pictures N      Detect only among first prefiltered N pictures
+
+
+
+
+
 ### Long-time run
 
 #### Stop/Resume
 When working with worklists an --stats file, current status is periodically saved to this file. If you need to resume it, just use command `nudecrawler --resume PATH/TO/stats.json`
 
 #### Memory leaking in containers
 You may check container memory usage with `sudo docker stats` or `sudo docker stats --no-stream`. Often containers consume more and more memory with time, leading to out-of-memory in the end. To prevent this problem use combination of `--stop` and `--refresh` like `--stop 1000 --refresh bin/refresh-nsfw-api.sh` this will call refresh script every 1000 images. Refresh script should stop current container and start it again. See source of refresh-nsfw-api.sh for example, it's very simple.
@@ -81,15 +100,14 @@
 
 ### Example usage:
 Check one page (using built-in :nude filter):
 ~~~
 nudecrawler -v --url1 https://telegra.ph/your-page-address 
 ~~~
 
-
 ~~~
 nudecrawler -w urls.txt --nude 5 -d 30 -f 5 --stats .local/mystats.json  --log .local/nudecrawler.log 
 ~~~
 process urls from urls.txt, report page if 5+ nude images (or 1 any video, default), nudity must be over 0.5 threshold, check from todays date to 30 days ago, append all found pages to .local/nudecrawler.log, save periodical statistics to .local/mystats.json
 
 If crawler will see page `Sasha-Grey-01-23-100`, but `Sasha-Grey-01-23-101` is 404 Not Found, it will try `-102` and so on. It will stop only if 5 (-f) pages in a row will fail. 
 
@@ -97,21 +115,20 @@
 nudecrawler -v --detect-image bin/detect-image-nsfw-api.py -f 5 --total 10 --nude 3 -w urls.txt --stats .local/stats.json --log .local/urls.log --stop 1000 --refresh bin/refresh-nsfw-api.sh
 ~~~
 
 Work verbosely (-v), use NSFW_API for resolving (and call refresh-nsfw-api.sh script to restart docker container every 1000 images).
 
 ## Options
 ~~~
-$ nudecrawler -h
 usage: nudecrawler [-h] [-d DAYS] [--url1 URL] [-f FAILS] [--day MONTH DAY] [--expr EXPR] [--total N] [--max-errors N] [--min-content-length N] [-a] [--detect-image SCRIPT]
-                   [--detect-url SCRIPT] [--detect METHOD] [--extensions [EXTENSIONS ...]] [--minsize MINSIZE] [--cache PATH] [-v] [--unbuffered] [--urls] [--log LOG] [-w WORDLIST]
-                   [--stats STATS_FILE] [--resume STATS_FILE] [--stop NUM_IMAGES] [--refresh SCRIPT [ARG ...]]
+                   [--detect-url SCRIPT] [--detect METHOD] [--extensions [EXTENSIONS ...]] [--minsize MINSIZE] [--max-pictures N] [--cache PATH] [-v] [--unbuffered] [--urls] [--log LOG]
+                   [--bugreport] [--workdir WORKDIR] [-w WORDLIST] [--stats STATS_FILE] [--resume STATS_FILE] [--stop NUM_IMAGES] [--refresh SCRIPT [ARG ...]]
                    [words ...]
 
-Nudecrawler: Telegra.ph Spider 0.3.0
+Nudecrawler: Telegra.ph Spider 0.3.6
 https://github.com/yaroslaff/nudecrawler
 
 positional arguments:
   words
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -128,25 +145,28 @@
                         Interesting if N+ total images (5)
 
 Image filtering options:
   -a, --all             do not detect, print all found pages
   --detect-image SCRIPT
                         explicitly use this script to detect nudity on image file
   --detect-url SCRIPT   explicitly use this script to detect nudity on image URL
-  --detect METHOD       One of true, false, nudepy, aid, nsfwapi, nudenet
+  --detect METHOD       One of true, false, nudepy, nudenetb, aid, nsfwapi, nudenet
   --extensions [EXTENSIONS ...]
                         interesting extensions (with dot, like .jpg)
   --minsize MINSIZE     min size of image in Kb (10)
+  --max-pictures N      Detect only among first prefiltered N pictures
   --cache PATH          path to cache file (will create if missing)
 
 Output options:
   -v, --verbose         verbose
   --unbuffered, -b      Use unbuffered stdout
   --urls                Do not detect, just generate and print URLs
   --log LOG             print all precious treasures to this logfile
+  --bugreport           print all precious treasures to this logfile
+  --workdir WORKDIR     Use all files (log, wordlist, cache) in this dir. def: .
 
 list-related options:
   -w WORDLIST, --wordlist WORDLIST
                         wordlist (urllist) file
   --stats STATS_FILE    periodical statistics file
   --resume STATS_FILE   resume from STATS_FILE (other args are not needed)
   --stop NUM_IMAGES     stop (or --refresh) after N images processed (or little after)
```

### Comparing `nudecrawler-0.3.6/README.md` & `nudecrawler-0.3.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,45 @@
+Metadata-Version: 2.1
+Name: nudecrawler
+Version: 0.3.7
+Summary: Crawl telegra.ph for nude pictures and videos
+Home-page: https://github.com/yaroslaff/nudecrawler
+Author: Yaroslav Polyakov
+Author-email: yaroslaff@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: nudenet
+
 # nude crawler
 
 Nude crawler crawls all pages on telegra.ph for today and N past days for specific words, checks number of nude, non-nude images, videos (not analysed) and reports pages which looks interesting (e.g. has more then 10 nude images, or has one video)
 
 ## Ineffective intriguing warning
 No matter how old you are, no matter how tolerant you are, no matter what your sexual orientation is, no matter what your favorite perversion is, no matter how big your sexual horizons are, with NudeCrawler you will find a lot of things that **you will NOT like**.
 
 I wrote this warning because I have seen some shit. LITERALLY.
 
 Please use it only for legal and ethical purposes. And it's 18+ surely. 
 
 ## Install
 
+Recommended (and most secure) way is using docker:
+```
+mkdir /tmp/run
+sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha grey" "Belle Delphine" Amouranth
+```
+
+See below how to refine your searching and filtering.
+
+### Alternative install
 ```
 pip3 install nudecrawler
 ```
 
 alternatively, install right from git repo:
 ```
 pip3 install git+https://github.com/yaroslaff/nudecrawler
@@ -35,18 +60,44 @@
 INTERESTING https://telegra.ph/sasha-grey-XXXXX
   Nude: 9 non-nude: 6
 
 INTERESTING https://telegra.ph/sasha-grey-XXXXX
   Nude: 6 non-nude: 3
 ~~~
 
-## Getting only interesting results
+## Refine search/filtering
 Nudecrawler uses [evalidate](https://github.com/yaroslaff/evalidate) to filter results with python expression (`--expr`). With `-h` help will list all avaliable variables, like: `total_images nude_images nonnude_images new_nude_images new_nonnude_images new_total_images total_video`.
 Default value: `(total_images>5 and new_nude_images>0) or total_video>0`.
 
+Use `-a`/`--all` to get some results ASAP (but later you may want to make some filtering)
+
+  -d DAYS, --days DAYS
+
+
+  -f FAILS, --fails FAILS
+  --total N             Boring if less then N total images (5)
+  --max-errors N        Max allowed errors on page ()
+  --min-content-length N
+                        Interesting if N+ total images (5)
+
+Image filtering options:
+  -a, --all             do not detect, print all found pages
+  --detect-image SCRIPT
+                        explicitly use this script to detect nudity on image file
+  --detect-url SCRIPT   explicitly use this script to detect nudity on image URL
+  --detect METHOD       One of true, false, nudepy, nudenetb, aid, nsfwapi, nudenet
+  --extensions [EXTENSIONS ...]
+                        interesting extensions (with dot, like .jpg)
+  --minsize MINSIZE     min size of image in Kb (10)
+  --max-pictures N      Detect only among first prefiltered N pictures
+
+
+
+
+
 ### Long-time run
 
 #### Stop/Resume
 When working with worklists an --stats file, current status is periodically saved to this file. If you need to resume it, just use command `nudecrawler --resume PATH/TO/stats.json`
 
 #### Memory leaking in containers
 You may check container memory usage with `sudo docker stats` or `sudo docker stats --no-stream`. Often containers consume more and more memory with time, leading to out-of-memory in the end. To prevent this problem use combination of `--stop` and `--refresh` like `--stop 1000 --refresh bin/refresh-nsfw-api.sh` this will call refresh script every 1000 images. Refresh script should stop current container and start it again. See source of refresh-nsfw-api.sh for example, it's very simple.
@@ -65,15 +116,14 @@
 
 ### Example usage:
 Check one page (using built-in :nude filter):
 ~~~
 nudecrawler -v --url1 https://telegra.ph/your-page-address 
 ~~~
 
-
 ~~~
 nudecrawler -w urls.txt --nude 5 -d 30 -f 5 --stats .local/mystats.json  --log .local/nudecrawler.log 
 ~~~
 process urls from urls.txt, report page if 5+ nude images (or 1 any video, default), nudity must be over 0.5 threshold, check from todays date to 30 days ago, append all found pages to .local/nudecrawler.log, save periodical statistics to .local/mystats.json
 
 If crawler will see page `Sasha-Grey-01-23-100`, but `Sasha-Grey-01-23-101` is 404 Not Found, it will try `-102` and so on. It will stop only if 5 (-f) pages in a row will fail. 
 
@@ -81,21 +131,20 @@
 nudecrawler -v --detect-image bin/detect-image-nsfw-api.py -f 5 --total 10 --nude 3 -w urls.txt --stats .local/stats.json --log .local/urls.log --stop 1000 --refresh bin/refresh-nsfw-api.sh
 ~~~
 
 Work verbosely (-v), use NSFW_API for resolving (and call refresh-nsfw-api.sh script to restart docker container every 1000 images).
 
 ## Options
 ~~~
-$ nudecrawler -h
 usage: nudecrawler [-h] [-d DAYS] [--url1 URL] [-f FAILS] [--day MONTH DAY] [--expr EXPR] [--total N] [--max-errors N] [--min-content-length N] [-a] [--detect-image SCRIPT]
-                   [--detect-url SCRIPT] [--detect METHOD] [--extensions [EXTENSIONS ...]] [--minsize MINSIZE] [--cache PATH] [-v] [--unbuffered] [--urls] [--log LOG] [-w WORDLIST]
-                   [--stats STATS_FILE] [--resume STATS_FILE] [--stop NUM_IMAGES] [--refresh SCRIPT [ARG ...]]
+                   [--detect-url SCRIPT] [--detect METHOD] [--extensions [EXTENSIONS ...]] [--minsize MINSIZE] [--max-pictures N] [--cache PATH] [-v] [--unbuffered] [--urls] [--log LOG]
+                   [--bugreport] [--workdir WORKDIR] [-w WORDLIST] [--stats STATS_FILE] [--resume STATS_FILE] [--stop NUM_IMAGES] [--refresh SCRIPT [ARG ...]]
                    [words ...]
 
-Nudecrawler: Telegra.ph Spider 0.3.0
+Nudecrawler: Telegra.ph Spider 0.3.6
 https://github.com/yaroslaff/nudecrawler
 
 positional arguments:
   words
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -112,25 +161,28 @@
                         Interesting if N+ total images (5)
 
 Image filtering options:
   -a, --all             do not detect, print all found pages
   --detect-image SCRIPT
                         explicitly use this script to detect nudity on image file
   --detect-url SCRIPT   explicitly use this script to detect nudity on image URL
-  --detect METHOD       One of true, false, nudepy, aid, nsfwapi, nudenet
+  --detect METHOD       One of true, false, nudepy, nudenetb, aid, nsfwapi, nudenet
   --extensions [EXTENSIONS ...]
                         interesting extensions (with dot, like .jpg)
   --minsize MINSIZE     min size of image in Kb (10)
+  --max-pictures N      Detect only among first prefiltered N pictures
   --cache PATH          path to cache file (will create if missing)
 
 Output options:
   -v, --verbose         verbose
   --unbuffered, -b      Use unbuffered stdout
   --urls                Do not detect, just generate and print URLs
   --log LOG             print all precious treasures to this logfile
+  --bugreport           print all precious treasures to this logfile
+  --workdir WORKDIR     Use all files (log, wordlist, cache) in this dir. def: .
 
 list-related options:
   -w WORDLIST, --wordlist WORDLIST
                         wordlist (urllist) file
   --stats STATS_FILE    periodical statistics file
   --resume STATS_FILE   resume from STATS_FILE (other args are not needed)
   --stop NUM_IMAGES     stop (or --refresh) after N images processed (or little after)
```

### Comparing `nudecrawler-0.3.6/bin/detect-image-aid.py` & `nudecrawler-0.3.7/bin/detect-image-aid.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/bin/detect-image-nsfw-api.py` & `nudecrawler-0.3.7/bin/detect-image-nsfw-api.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/bin/detect-image-nudenet.py` & `nudecrawler-0.3.7/bin/detect-image-nudenet.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/bin/detect-server-nudenet.py` & `nudecrawler-0.3.7/bin/detect-server-nudenet.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/bin/nudecrawler` & `nudecrawler-0.3.7/bin/nudecrawler`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,16 @@
     def_unbuf = bool(os.getenv('NUDE_UNBUF'))
 
     parser = argparse.ArgumentParser(description=f'Nudecrawler: Telegra.ph Spider {version}\nhttps://github.com/yaroslaff/nudecrawler', formatter_class=argparse.RawTextHelpFormatter)
 
     def_expr = '(total_images>5 and new_nude_images>0) or total_video>0'
     def_workdir = os.getenv('NUDE_DIR', '.')
 
-    def_total =5
+    def_total = int(os.getenv('NUDE_TOTAL', '1'))
+    def_errors = 5
     def_minsize=10
 
     methods_list = ', '.join(filter_methods.keys())
 
     parser.add_argument('words', nargs='*')
     parser.add_argument('-d', '--days', type=int, default=30)
     # parser.add_argument('--nude', metavar='N', type=int, default=1, help='Interesting if N+ nude images')
@@ -127,16 +128,16 @@
     parser.add_argument('--url1', metavar="URL", help='process only one url')
     parser.add_argument('-f', '--fails', type=int, default=5, help='stop searching next pages with same words after N failures')
     parser.add_argument('--day', nargs=2, type=int, metavar=('MONTH', 'DAY'), help='Current date (default is today) example: --day 12 31')
 
     g = parser.add_argument_group('Page filtering options')
     parser.add_argument('--expr', '-e', metavar='EXPR', default=def_expr, 
                         help=f'Interesting if EXPR is True. def: {def_expr!r}\nFields: ' + ' '.join(context_fields) )
-    parser.add_argument('--total', metavar='N', type=int, default=5, help=f'Boring if less then N total images ({def_total})')
-    parser.add_argument('--max-errors', metavar='N', type=int, default=5, help=f'Max allowed errors on page ()')
+    parser.add_argument('--total', metavar='N', type=int, default=def_total, help=f'Boring if less then N total images ({def_total})')
+    parser.add_argument('--max-errors', metavar='N', type=int, default=def_errors, help=f'Max allowed errors on page ({def_errors})')
     parser.add_argument('--min-content-length', metavar='N', type=int, default=None, help=f'Interesting if N+ total images ({def_total})')
 
     g = parser.add_argument_group('Image filtering options')
     g.add_argument('-a', '--all', default=False, action='store_true', help='do not detect, print all found pages')
     g.add_argument('--detect-image', metavar='SCRIPT', help='explicitly use this script to detect nudity on image file')
     g.add_argument('--detect-url', metavar='SCRIPT', help='explicitly use this script to detect nudity on image URL')
     g.add_argument('--detect', metavar='METHOD', default=def_detect, help=f'One of {methods_list}')
```

### Comparing `nudecrawler-0.3.6/nudecrawler/cache.py` & `nudecrawler-0.3.7/nudecrawler/cache.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/nudecrawler/localimage.py` & `nudecrawler-0.3.7/nudecrawler/localimage.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/nudecrawler/page.py` & `nudecrawler-0.3.7/nudecrawler/page.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/nudecrawler/remoteimage.py` & `nudecrawler-0.3.7/nudecrawler/remoteimage.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/nudecrawler/tgru.py` & `nudecrawler-0.3.7/nudecrawler/tgru.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/nudecrawler/verbose.py` & `nudecrawler-0.3.7/nudecrawler/verbose.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/nudecrawler.egg-info/PKG-INFO` & `nudecrawler-0.3.7/nudecrawler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudecrawler
-Version: 0.3.6
+Version: 0.3.7
 Summary: Crawl telegra.ph for nude pictures and videos
 Home-page: https://github.com/yaroslaff/nudecrawler
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,23 @@
 
 I wrote this warning because I have seen some shit. LITERALLY.
 
 Please use it only for legal and ethical purposes. And it's 18+ surely. 
 
 ## Install
 
+Recommended (and most secure) way is using docker:
+```
+mkdir /tmp/run
+sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha grey" "Belle Delphine" Amouranth
+```
+
+See below how to refine your searching and filtering.
+
+### Alternative install
 ```
 pip3 install nudecrawler
 ```
 
 alternatively, install right from git repo:
 ```
 pip3 install git+https://github.com/yaroslaff/nudecrawler
@@ -51,18 +60,44 @@
 INTERESTING https://telegra.ph/sasha-grey-XXXXX
   Nude: 9 non-nude: 6
 
 INTERESTING https://telegra.ph/sasha-grey-XXXXX
   Nude: 6 non-nude: 3
 ~~~
 
-## Getting only interesting results
+## Refine search/filtering
 Nudecrawler uses [evalidate](https://github.com/yaroslaff/evalidate) to filter results with python expression (`--expr`). With `-h` help will list all avaliable variables, like: `total_images nude_images nonnude_images new_nude_images new_nonnude_images new_total_images total_video`.
 Default value: `(total_images>5 and new_nude_images>0) or total_video>0`.
 
+Use `-a`/`--all` to get some results ASAP (but later you may want to make some filtering)
+
+  -d DAYS, --days DAYS
+
+
+  -f FAILS, --fails FAILS
+  --total N             Boring if less then N total images (5)
+  --max-errors N        Max allowed errors on page ()
+  --min-content-length N
+                        Interesting if N+ total images (5)
+
+Image filtering options:
+  -a, --all             do not detect, print all found pages
+  --detect-image SCRIPT
+                        explicitly use this script to detect nudity on image file
+  --detect-url SCRIPT   explicitly use this script to detect nudity on image URL
+  --detect METHOD       One of true, false, nudepy, nudenetb, aid, nsfwapi, nudenet
+  --extensions [EXTENSIONS ...]
+                        interesting extensions (with dot, like .jpg)
+  --minsize MINSIZE     min size of image in Kb (10)
+  --max-pictures N      Detect only among first prefiltered N pictures
+
+
+
+
+
 ### Long-time run
 
 #### Stop/Resume
 When working with worklists an --stats file, current status is periodically saved to this file. If you need to resume it, just use command `nudecrawler --resume PATH/TO/stats.json`
 
 #### Memory leaking in containers
 You may check container memory usage with `sudo docker stats` or `sudo docker stats --no-stream`. Often containers consume more and more memory with time, leading to out-of-memory in the end. To prevent this problem use combination of `--stop` and `--refresh` like `--stop 1000 --refresh bin/refresh-nsfw-api.sh` this will call refresh script every 1000 images. Refresh script should stop current container and start it again. See source of refresh-nsfw-api.sh for example, it's very simple.
@@ -81,15 +116,14 @@
 
 ### Example usage:
 Check one page (using built-in :nude filter):
 ~~~
 nudecrawler -v --url1 https://telegra.ph/your-page-address 
 ~~~
 
-
 ~~~
 nudecrawler -w urls.txt --nude 5 -d 30 -f 5 --stats .local/mystats.json  --log .local/nudecrawler.log 
 ~~~
 process urls from urls.txt, report page if 5+ nude images (or 1 any video, default), nudity must be over 0.5 threshold, check from todays date to 30 days ago, append all found pages to .local/nudecrawler.log, save periodical statistics to .local/mystats.json
 
 If crawler will see page `Sasha-Grey-01-23-100`, but `Sasha-Grey-01-23-101` is 404 Not Found, it will try `-102` and so on. It will stop only if 5 (-f) pages in a row will fail. 
 
@@ -97,21 +131,20 @@
 nudecrawler -v --detect-image bin/detect-image-nsfw-api.py -f 5 --total 10 --nude 3 -w urls.txt --stats .local/stats.json --log .local/urls.log --stop 1000 --refresh bin/refresh-nsfw-api.sh
 ~~~
 
 Work verbosely (-v), use NSFW_API for resolving (and call refresh-nsfw-api.sh script to restart docker container every 1000 images).
 
 ## Options
 ~~~
-$ nudecrawler -h
 usage: nudecrawler [-h] [-d DAYS] [--url1 URL] [-f FAILS] [--day MONTH DAY] [--expr EXPR] [--total N] [--max-errors N] [--min-content-length N] [-a] [--detect-image SCRIPT]
-                   [--detect-url SCRIPT] [--detect METHOD] [--extensions [EXTENSIONS ...]] [--minsize MINSIZE] [--cache PATH] [-v] [--unbuffered] [--urls] [--log LOG] [-w WORDLIST]
-                   [--stats STATS_FILE] [--resume STATS_FILE] [--stop NUM_IMAGES] [--refresh SCRIPT [ARG ...]]
+                   [--detect-url SCRIPT] [--detect METHOD] [--extensions [EXTENSIONS ...]] [--minsize MINSIZE] [--max-pictures N] [--cache PATH] [-v] [--unbuffered] [--urls] [--log LOG]
+                   [--bugreport] [--workdir WORKDIR] [-w WORDLIST] [--stats STATS_FILE] [--resume STATS_FILE] [--stop NUM_IMAGES] [--refresh SCRIPT [ARG ...]]
                    [words ...]
 
-Nudecrawler: Telegra.ph Spider 0.3.0
+Nudecrawler: Telegra.ph Spider 0.3.6
 https://github.com/yaroslaff/nudecrawler
 
 positional arguments:
   words
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -128,25 +161,28 @@
                         Interesting if N+ total images (5)
 
 Image filtering options:
   -a, --all             do not detect, print all found pages
   --detect-image SCRIPT
                         explicitly use this script to detect nudity on image file
   --detect-url SCRIPT   explicitly use this script to detect nudity on image URL
-  --detect METHOD       One of true, false, nudepy, aid, nsfwapi, nudenet
+  --detect METHOD       One of true, false, nudepy, nudenetb, aid, nsfwapi, nudenet
   --extensions [EXTENSIONS ...]
                         interesting extensions (with dot, like .jpg)
   --minsize MINSIZE     min size of image in Kb (10)
+  --max-pictures N      Detect only among first prefiltered N pictures
   --cache PATH          path to cache file (will create if missing)
 
 Output options:
   -v, --verbose         verbose
   --unbuffered, -b      Use unbuffered stdout
   --urls                Do not detect, just generate and print URLs
   --log LOG             print all precious treasures to this logfile
+  --bugreport           print all precious treasures to this logfile
+  --workdir WORKDIR     Use all files (log, wordlist, cache) in this dir. def: .
 
 list-related options:
   -w WORDLIST, --wordlist WORDLIST
                         wordlist (urllist) file
   --stats STATS_FILE    periodical statistics file
   --resume STATS_FILE   resume from STATS_FILE (other args are not needed)
   --stop NUM_IMAGES     stop (or --refresh) after N images processed (or little after)
```

### Comparing `nudecrawler-0.3.6/nudecrawler.egg-info/SOURCES.txt` & `nudecrawler-0.3.7/nudecrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/pyproject.toml` & `nudecrawler-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/setup.py` & `nudecrawler-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.6/tests/test_nudecrawler.py` & `nudecrawler-0.3.7/tests/test_nudecrawler.py`

 * *Files identical despite different names*

