# Comparing `tmp/nudecrawler-0.3.5.tar.gz` & `tmp/nudecrawler-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudecrawler-0.3.5.tar", last modified: Sat Apr  8 18:42:22 2023, max compression
+gzip compressed data, was "nudecrawler-0.3.6.tar", last modified: Mon Apr 10 18:07:10 2023, max compression
```

## Comparing `nudecrawler-0.3.5.tar` & `nudecrawler-0.3.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-08 18:42:22.935588 nudecrawler-0.3.5/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    13764 2023-04-08 18:42:22.935588 nudecrawler-0.3.5/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)    13252 2023-04-08 13:47:25.000000 nudecrawler-0.3.5/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-08 18:42:22.935588 nudecrawler-0.3.5/bin/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1458 2023-03-25 09:35:46.000000 nudecrawler-0.3.5/bin/detect-image-aid.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2497 2023-03-25 11:06:28.000000 nudecrawler-0.3.5/bin/detect-image-nsfw-api.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1527 2023-03-22 08:23:37.000000 nudecrawler-0.3.5/bin/detect-image-nudenet.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3368 2023-04-06 19:13:11.000000 nudecrawler-0.3.5/bin/detect-server-nudenet.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)    16255 2023-04-08 14:42:11.000000 nudecrawler-0.3.5/bin/nudecrawler
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      217 2023-04-01 23:30:57.000000 nudecrawler-0.3.5/bin/refresh-nsfw-api.sh
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-08 18:42:22.935588 nudecrawler-0.3.5/nudecrawler/
--rw-r--r--   0 xenon     (1000) xenon     (1000)       95 2023-03-20 17:34:21.000000 nudecrawler-0.3.5/nudecrawler/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1990 2023-04-03 19:10:18.000000 nudecrawler-0.3.5/nudecrawler/cache.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      293 2023-03-21 11:11:32.000000 nudecrawler-0.3.5/nudecrawler/exceptions.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      588 2023-03-25 09:36:26.000000 nudecrawler-0.3.5/nudecrawler/localimage.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12763 2023-04-08 14:41:03.000000 nudecrawler-0.3.5/nudecrawler/page.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2572 2023-04-08 18:41:44.000000 nudecrawler-0.3.5/nudecrawler/remoteimage.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      952 2023-04-03 17:15:52.000000 nudecrawler-0.3.5/nudecrawler/tgru.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      352 2023-02-28 18:19:59.000000 nudecrawler-0.3.5/nudecrawler/unbuffered.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1114 2023-04-08 13:56:10.000000 nudecrawler-0.3.5/nudecrawler/verbose.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)       15 2023-04-08 14:42:27.000000 nudecrawler-0.3.5/nudecrawler/version.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-08 18:42:22.935588 nudecrawler-0.3.5/nudecrawler.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    13764 2023-04-08 18:42:22.000000 nudecrawler-0.3.5/nudecrawler.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      619 2023-04-08 18:42:22.000000 nudecrawler-0.3.5/nudecrawler.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-08 18:42:22.000000 nudecrawler-0.3.5/nudecrawler.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)      104 2023-04-08 18:42:22.000000 nudecrawler-0.3.5/nudecrawler.egg-info/requires.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-04-08 18:42:22.000000 nudecrawler-0.3.5/nudecrawler.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)      880 2023-04-06 18:16:07.000000 nudecrawler-0.3.5/pyproject.toml
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-04-08 18:42:22.935588 nudecrawler-0.3.5/setup.cfg
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1688 2023-04-08 18:41:42.000000 nudecrawler-0.3.5/setup.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-08 18:42:22.935588 nudecrawler-0.3.5/tests/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      637 2023-04-03 22:33:06.000000 nudecrawler-0.3.5/tests/test_nudecrawler.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    14111 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    13599 2023-04-10 18:02:54.000000 nudecrawler-0.3.6/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/bin/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1458 2023-03-25 09:35:46.000000 nudecrawler-0.3.6/bin/detect-image-aid.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2497 2023-03-25 11:06:28.000000 nudecrawler-0.3.6/bin/detect-image-nsfw-api.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1527 2023-04-10 13:36:55.000000 nudecrawler-0.3.6/bin/detect-image-nudenet.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3527 2023-04-10 14:42:15.000000 nudecrawler-0.3.6/bin/detect-server-nudenet.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)    16034 2023-04-10 17:41:17.000000 nudecrawler-0.3.6/bin/nudecrawler
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      217 2023-04-01 23:30:57.000000 nudecrawler-0.3.6/bin/refresh-nsfw-api.sh
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/nudecrawler/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       95 2023-03-20 17:34:21.000000 nudecrawler-0.3.6/nudecrawler/__init__.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1990 2023-04-03 19:10:18.000000 nudecrawler-0.3.6/nudecrawler/cache.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      293 2023-03-21 11:11:32.000000 nudecrawler-0.3.6/nudecrawler/exceptions.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      588 2023-03-25 09:36:26.000000 nudecrawler-0.3.6/nudecrawler/localimage.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12822 2023-04-10 18:00:20.000000 nudecrawler-0.3.6/nudecrawler/page.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     3082 2023-04-10 16:46:51.000000 nudecrawler-0.3.6/nudecrawler/remoteimage.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      952 2023-04-03 17:15:52.000000 nudecrawler-0.3.6/nudecrawler/tgru.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      352 2023-02-28 18:19:59.000000 nudecrawler-0.3.6/nudecrawler/unbuffered.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1114 2023-04-08 13:56:10.000000 nudecrawler-0.3.6/nudecrawler/verbose.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       15 2023-04-10 18:06:29.000000 nudecrawler-0.3.6/nudecrawler/version.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/nudecrawler.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    14111 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      619 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      104 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/requires.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-04-10 18:07:10.000000 nudecrawler-0.3.6/nudecrawler.egg-info/top_level.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      880 2023-04-06 18:16:07.000000 nudecrawler-0.3.6/pyproject.toml
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/setup.cfg
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1688 2023-04-08 18:41:42.000000 nudecrawler-0.3.6/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 18:07:10.420645 nudecrawler-0.3.6/tests/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      637 2023-04-03 22:33:06.000000 nudecrawler-0.3.6/tests/test_nudecrawler.py
```

### Comparing `nudecrawler-0.3.5/PKG-INFO` & `nudecrawler-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudecrawler
-Version: 0.3.5
+Version: 0.3.6
 Summary: Crawl telegra.ph for nude pictures and videos
 Home-page: https://github.com/yaroslaff/nudecrawler
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -256,15 +256,18 @@
 - Image URL or PATH passed as argv[1]
 - Return 0 if image is safe and boring, return 1 if image is interesting
 - Return 0 if there are any technical problems (timeout or 404)
 - Additional configuration could be specified via environment, NudeCrawler will pass environment to your script
 - NudeCrawler also sets env variables `NUDECRAWLER_PAGE_URL` and `NUDECRAWLER_IMAGE_URL`
 
 ### Building docker container
-Repository includes Dockerfile. Use `sudo docker build -t nudecrawler .` to build it.
+Repository includes Dockerfile. Use `sudo docker build -t nudecrawler -f docker/Dockerfile .` to build it.
+
+Running docker container (example): `sudo docker run -v /tmp/run/:/work nudecrawler nudecrawler -w urls.txt -v`
+If you specify files for docker (like `-w`, `--stats`, `--resume`, `--log`, `--cache`) path will be modified starting from /work. e.g. `-w urls.txt` will be `-w /work/urls.txt` which is /tmp/run/urls.txt on host.
 
 
 ### Little bit about internals
 
 #### Prefiltering
 To speed-up processing, nudecrawler uses pre-filtering, HTTP HEAD request is performed for any image, and further processing is performed only if images passes basic check:
 - Image URL must return status 200
```

### Comparing `nudecrawler-0.3.5/README.md` & `nudecrawler-0.3.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -240,15 +240,18 @@
 - Image URL or PATH passed as argv[1]
 - Return 0 if image is safe and boring, return 1 if image is interesting
 - Return 0 if there are any technical problems (timeout or 404)
 - Additional configuration could be specified via environment, NudeCrawler will pass environment to your script
 - NudeCrawler also sets env variables `NUDECRAWLER_PAGE_URL` and `NUDECRAWLER_IMAGE_URL`
 
 ### Building docker container
-Repository includes Dockerfile. Use `sudo docker build -t nudecrawler .` to build it.
+Repository includes Dockerfile. Use `sudo docker build -t nudecrawler -f docker/Dockerfile .` to build it.
+
+Running docker container (example): `sudo docker run -v /tmp/run/:/work nudecrawler nudecrawler -w urls.txt -v`
+If you specify files for docker (like `-w`, `--stats`, `--resume`, `--log`, `--cache`) path will be modified starting from /work. e.g. `-w urls.txt` will be `-w /work/urls.txt` which is /tmp/run/urls.txt on host.
 
 
 ### Little bit about internals
 
 #### Prefiltering
 To speed-up processing, nudecrawler uses pre-filtering, HTTP HEAD request is performed for any image, and further processing is performed only if images passes basic check:
 - Image URL must return status 200
```

### Comparing `nudecrawler-0.3.5/bin/detect-image-aid.py` & `nudecrawler-0.3.6/bin/detect-image-aid.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/bin/detect-image-nsfw-api.py` & `nudecrawler-0.3.6/bin/detect-image-nsfw-api.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/bin/detect-image-nudenet.py` & `nudecrawler-0.3.6/bin/detect-image-nudenet.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/bin/detect-server-nudenet.py` & `nudecrawler-0.3.6/bin/detect-server-nudenet.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,35 +95,41 @@
 def main():
     global classifier
     global pidfile
     args = get_args()
     if not sanity_check():
         sys.exit(1)
     
+    print("load classified")
     classifier = NudeClassifier()
 
     if args.kill:
         try:
             with open(pidfile_path) as fh:
                 pid = int(fh.read())
                 print("Killing nudenet server with pid", pid)
                 os.kill(pid, signal.SIGINT)
             os.unlink(pidfile_path)
         except FileNotFoundError:
             print("no pidfile", pidfile_path, "not doing anything")
         sys.exit(0)
 
     if args.daemon:
+        print("work as daemon...")
         with daemon.DaemonContext(
             # pidfile=lockfile.FileLock(args.pidfile)
             pidfile=pidfile.TimeoutPIDLockFile(pidfile_path)
             ):
             # pid = os.getpid()
             # with open(pidfile, "w+") as fh:
             #    print(pid, file=fh)
+            print("daemon app.run")
             app.run(port=args.port)
+            print("after app.run")
     else:
-        app.run(port=args.port)    
+        app.run(port=args.port) 
+    
+    print("done.")   
 
 if __name__ == '__main__':
     main()
```

### Comparing `nudecrawler-0.3.5/bin/nudecrawler` & `nudecrawler-0.3.6/bin/nudecrawler`

 * *Files 4% similar despite different names*

```diff
@@ -90,53 +90,34 @@
 verbose = False
 all_found = True
 
 filter_methods = {
     "true": ("builtin", ":true"),
     "false": ("builtin", ":false"),
     "nudepy": ("builtin", ":nude"),
+    "nudenetb": ("builtin", ":nudenet"),
     "aid": ("image", "detect-image-aid.py"),
     "nsfwapi": ("image", "detect-image-nsfw-api.py"),
     "nudenet": ("image", "detect-image-nudenet.py")
 }
 
-nudenet_server_started = False
-
-def is_nudenet_running():
-    try:
-        r = requests.get('http://localhost:5000/ping')
-    except requests.RequestException:
-        return False
-    return r.status_code == 200
-
-def cond_start_nudenet():    
-    global nudenet_server_started
-
-    if is_nudenet_running():
-        return
-    
-    print("starting nudenet server...")
-    subprocess.run(['detect-server-nudenet.py', '-d'])
-    nudenet_server_started = True
-
-def cond_stop_nudenet():
-    if nudenet_server_started:
-        print("stopping nudenet server...")
-        subprocess.run(['detect-server-nudenet.py', '--kill'])
-        
-
 def get_args(argv=None):
 
     load_dotenv()  
 
-    def_detect = os.getenv('NUDE_DETECT', None)
+    def_detect = os.getenv('NUDE_DETECT')
+    def_cache = os.getenv('NUDE_CACHE')
+    def_log = os.getenv('NUDE_LOG')
+    def_stats = os.getenv('NUDE_STATS', '/tmp/nudecrawler-stats.txt')
+    def_unbuf = bool(os.getenv('NUDE_UNBUF'))
 
     parser = argparse.ArgumentParser(description=f'Nudecrawler: Telegra.ph Spider {version}\nhttps://github.com/yaroslaff/nudecrawler', formatter_class=argparse.RawTextHelpFormatter)
 
     def_expr = '(total_images>5 and new_nude_images>0) or total_video>0'
+    def_workdir = os.getenv('NUDE_DIR', '.')
 
     def_total =5
     def_minsize=10
 
     methods_list = ', '.join(filter_methods.keys())
 
     parser.add_argument('words', nargs='*')
@@ -158,28 +139,29 @@
     g.add_argument('-a', '--all', default=False, action='store_true', help='do not detect, print all found pages')
     g.add_argument('--detect-image', metavar='SCRIPT', help='explicitly use this script to detect nudity on image file')
     g.add_argument('--detect-url', metavar='SCRIPT', help='explicitly use this script to detect nudity on image URL')
     g.add_argument('--detect', metavar='METHOD', default=def_detect, help=f'One of {methods_list}')
     g.add_argument('--extensions', nargs='*', default=['.jpeg','.jpg', '.png'],help='interesting extensions (with dot, like .jpg)')
     g.add_argument('--minsize', type=int, default=def_minsize,help=f'min size of image in Kb ({def_minsize})')
     g.add_argument('--max-pictures', type=int, metavar='N', help=f'Detect only among first prefiltered N pictures')
-    g.add_argument('--cache', metavar='PATH', help=f'path to cache file (will create if missing)')
+    g.add_argument('--cache', metavar='PATH', default=def_cache, help=f'path to cache file (will create if missing)')
 
 
     g = parser.add_argument_group('Output options')
     g.add_argument('-v', '--verbose', default=False, action='store_true', help='verbose')
-    g.add_argument('--unbuffered', '-b', default=False, action='store_true', help='Use unbuffered stdout')
+    g.add_argument('--unbuffered', '-b', default=def_unbuf, action='store_true', help='Use unbuffered stdout')
     g.add_argument('--urls', default=False, action='store_true', help='Do not detect, just generate and print URLs')    
-    g.add_argument('--log', help='print all precious treasures to this logfile')
+    g.add_argument('--log', default=def_log, help='print all precious treasures to this logfile')
     g.add_argument('--bugreport', default=False, action='store_true', help='print all precious treasures to this logfile')
+    g.add_argument('--workdir', default=def_workdir, help=f'Use all files (log, wordlist, cache) in this dir. def: {def_workdir}')
 
 
     g = parser.add_argument_group('list-related options')
     g.add_argument('-w', '--wordlist', help='wordlist (urllist) file')
-    g.add_argument('--stats', metavar='STATS_FILE', default='/tmp/nudecrawler-stats.txt', help='periodical statistics file')
+    g.add_argument('--stats', metavar='STATS_FILE', default=def_stats, help='periodical statistics file')
     g.add_argument('--resume', metavar='STATS_FILE', help='resume from STATS_FILE (other args are not needed)')
     g.add_argument('--stop', type=int, metavar='NUM_IMAGES', help='stop (or --refresh) after N images processed (or little after)')
     g.add_argument('--refresh', metavar=('SCRIPT', 'ARG'), nargs='+', help='run this refresh script every --stop NUM_IMAGES images')
 
     return parser.parse_args(argv)
 
 
@@ -365,14 +347,28 @@
 
         cmd = stats['cmd']
         args = get_args(shlex.split(cmd)[1:])
         fastforward = True
     else:
         stats['cmd'] = ' '.join(sys.argv)
     
+
+
+    if args.unbuffered:
+        sys.stdout = Unbuffered(sys.stdout)
+
+
+    if args.workdir:
+        for attr in ['cache', 'wordlist', 'log', 'resume', 'stats']:
+            old = getattr(args, attr)
+            if old is not None:
+                new = os.path.join(args.workdir, old)
+                setattr(args, attr, new)
+
+
     # nude = args.nude
     # video = args.video
     verbose = args.verbose
     all_found = args.all    
     matched_resume = False
     skipped_words = 0
     stop_after = args.stop
@@ -398,41 +394,33 @@
 
         if kind in ['image', 'url']:
             if shutil.which(basename) is None:
                 print(f"Cannot find {basename}, maybe not in $PATH?" ,file=sys.stderr)
                 sys.exit(1)
 
         if kind == 'builtin':
-            if basename == ':nude':
+            if basename in [':nude', ':nudenet']:
                 detect_image = basename
             else:
                 detect_url = basename
         elif kind == 'image':
             detect_image = basename
             print(f"# Will use script {shutil.which(basename)} for filtering images")
         elif kind == 'url':
             detect_url = basename
             print(f"# Will use script {shutil.which(basename)} for filtering images")            
     
 
-        # special helper
-        if args.detect == 'nudenet':
-            cond_start_nudenet()
-
-
     # fix arguments
-    if not any([detect_image, detect_url, all_found]):
+    if not any([detect_image, detect_url, all_found]):        
         print("# No filter, using built-in :nude by default")
         detect_image=':nude'
 
     nudecrawler.verbose.verbose = verbose
 
-    if args.unbuffered:
-        sys.stdout = Unbuffered(sys.stdout)
-
     if args.extensions:
         stats['filter']['image_extensions'] = args.extensions
     
     if args.minsize:
         stats['filter']['min_image_size'] = args.minsize * 1024
 
     if args.total:
@@ -465,19 +453,14 @@
     
     if not words:
         print("Need either --url1 URL or words like 'nude' or -w wordlist.txt")
         sys.exit(1)
 
     logfile = args.log
 
-    #if args.stats and os.path.exists(args.stats):
-    #    with open(args.stats) as fh:
-    #        stats = json.load(fh)
-    #        fastforward = True
-
     for w in words:
         if fastforward and not matched_resume:
             if w == stats['resume']['word']:
                 matched_resume = True
             else:
                 skipped_words += 1
                 continue
@@ -501,20 +484,20 @@
             # stop fastforward
             fastforward=False
             check_word(w, day, args.fails, print_urls = args.urls, resumecount=resumecount)
             
             days_tried += 1
             day = day - datetime.timedelta(days=1)
 
-    cond_stop_nudenet()
+
     print(f"Finished {len(words)} (skipped {skipped_words}) words in {time.time() - started:.2f} seconds, found {stats['found_interesting_pages']} pages")
     if fastforward and not matched_resume:
         abort(f"Did not found word {stats['resume']['word']}")
 
 if __name__ == '__main__':
     try:
         main()
     except KeyboardInterrupt as e:
         print("KEYBOARD INTERRUPT")
         print(e)
         save_stats(force=True)
-        cond_stop_nudenet()
+
```

### Comparing `nudecrawler-0.3.5/nudecrawler/cache.py` & `nudecrawler-0.3.6/nudecrawler/cache.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/nudecrawler/localimage.py` & `nudecrawler-0.3.6/nudecrawler/localimage.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/nudecrawler/page.py` & `nudecrawler-0.3.6/nudecrawler/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 
 
 from urllib.parse import urlparse
 import subprocess
 import sys
 import os
 
-
-
 #def trivial_iterator(xx):
 #    for x in xx:
 #        yield x
 
 processed_images = 0
 context_fields = ['total_images', 'nude_images', 'nonnude_images', 'new_nude_images', 'new_nonnude_images', 'new_total_images', 'total_video']
 
@@ -106,15 +104,16 @@
             if self.content_length is not None:
                 self.content_length = int(self.content_length)
 
             if self.content_length and min_content_length and self.content_length < min_content_length:
                 self.ignore(f"content-length {self.content_length} < minimal {min_content_length}")
                 return
         except (urllib.error.URLError, ConnectionError, http.client.RemoteDisconnected) as e:
-            if e.status == 404:
+            if hasattr(e, 'status') and e.status == 404:
+                # print(e, type(e))
                 # silent ignore most usual error (unless verbose)
                 printv(url, 404)
                 self._status = "IGNORED"
                 self._status_detailed = "404"
                 self._ignore = True
                 self.http_code = e.status
             else:
```

### Comparing `nudecrawler-0.3.5/nudecrawler/tgru.py` & `nudecrawler-0.3.6/nudecrawler/tgru.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/nudecrawler/verbose.py` & `nudecrawler-0.3.6/nudecrawler/verbose.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/nudecrawler.egg-info/PKG-INFO` & `nudecrawler-0.3.6/nudecrawler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudecrawler
-Version: 0.3.5
+Version: 0.3.6
 Summary: Crawl telegra.ph for nude pictures and videos
 Home-page: https://github.com/yaroslaff/nudecrawler
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -256,15 +256,18 @@
 - Image URL or PATH passed as argv[1]
 - Return 0 if image is safe and boring, return 1 if image is interesting
 - Return 0 if there are any technical problems (timeout or 404)
 - Additional configuration could be specified via environment, NudeCrawler will pass environment to your script
 - NudeCrawler also sets env variables `NUDECRAWLER_PAGE_URL` and `NUDECRAWLER_IMAGE_URL`
 
 ### Building docker container
-Repository includes Dockerfile. Use `sudo docker build -t nudecrawler .` to build it.
+Repository includes Dockerfile. Use `sudo docker build -t nudecrawler -f docker/Dockerfile .` to build it.
+
+Running docker container (example): `sudo docker run -v /tmp/run/:/work nudecrawler nudecrawler -w urls.txt -v`
+If you specify files for docker (like `-w`, `--stats`, `--resume`, `--log`, `--cache`) path will be modified starting from /work. e.g. `-w urls.txt` will be `-w /work/urls.txt` which is /tmp/run/urls.txt on host.
 
 
 ### Little bit about internals
 
 #### Prefiltering
 To speed-up processing, nudecrawler uses pre-filtering, HTTP HEAD request is performed for any image, and further processing is performed only if images passes basic check:
 - Image URL must return status 200
```

### Comparing `nudecrawler-0.3.5/nudecrawler.egg-info/SOURCES.txt` & `nudecrawler-0.3.6/nudecrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/pyproject.toml` & `nudecrawler-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/setup.py` & `nudecrawler-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.5/tests/test_nudecrawler.py` & `nudecrawler-0.3.6/tests/test_nudecrawler.py`

 * *Files identical despite different names*

