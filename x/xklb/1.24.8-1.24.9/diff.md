# Comparing `tmp/xklb-1.24.8.tar.gz` & `tmp/xklb-1.24.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xklb-1.24.8.tar", max compression
+gzip compressed data, was "xklb-1.24.9.tar", max compression
```

## Comparing `xklb-1.24.8.tar` & `xklb-1.24.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1676 2023-04-02 15:25:43.226132 xklb-1.24.8/LICENSE
--rw-r--r--   0        0        0    39259 2023-04-02 15:25:43.226132 xklb-1.24.8/README.md
--rw-r--r--   0        0        0     8385 2023-04-02 15:25:43.226132 xklb-1.24.8/assets/kotobago.png
--rw-r--r--   0        0        0    13982 2023-04-02 15:25:44.346146 xklb-1.24.8/pyproject.toml
--rw-r--r--   0        0        0      686 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/__init__.py
--rw-r--r--   0        0        0     4199 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/bigdirs.py
--rw-r--r--   0        0        0     7880 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/invalid_paths.py
--rw-r--r--   0        0        0     1370 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4020 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/merge_online_local.py
--rw-r--r--   0        0        0      992 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1529 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2741 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2085 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/mining/reddit_self.py
--rw-r--r--   0        0        0    17101 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/mining/words.py
--rw-r--r--   0        0        0     6864 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/move_list.py
--rw-r--r--   0        0        0      547 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/optimize_db.py
--rw-r--r--   0        0        0     9412 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/redownload.py
--rw-r--r--   0        0        0      483 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/restore_listen_count.sql
--rw-r--r--   0        0        0    17018 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/scatter.py
--rw-r--r--   0        0        0     2610 2023-04-02 15:25:44.346146 xklb-1.24.8/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0       25 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/__init__.py
--rw-r--r--   0        0        0     6846 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/av.py
--rw-r--r--   0        0        0     6870 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/books.py
--rw-r--r--   0        0        0     7676 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/consts.py
--rw-r--r--   0        0        0     7602 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/db.py
--rw-r--r--   0        0        0     7051 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/dl_config.py
--rw-r--r--   0        0        0    14665 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/dl_extract.py
--rw-r--r--   0        0        0    13251 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/fs_extract.py
--rw-r--r--   0        0        0     5444 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/gui.py
--rw-r--r--   0        0        0     5904 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/hn_extract.py
--rw-r--r--   0        0        0     8992 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/lb.py
--rw-r--r--   0        0        0    32433 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/play_actions.py
--rw-r--r--   0        0        0     4677 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/playback.py
--rw-r--r--   0        0        0    25496 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/player.py
--rw-r--r--   0        0        0    14553 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/praw_extract.py
--rw-r--r--   0        0        0    16045 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/stats.py
--rw-r--r--   0        0        0     3824 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/subtitle.py
--rw-r--r--   0        0        0    11986 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3607 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21477 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/tube_backend.py
--rw-r--r--   0        0        0     6258 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/tube_extract.py
--rw-r--r--   0        0        0    26117 2023-04-02 15:25:44.350146 xklb-1.24.8/xklb/utils.py
--rw-r--r--   0        0        0    40447 1970-01-01 00:00:00.000000 xklb-1.24.8/PKG-INFO
+-rw-r--r--   0        0        0     1676 2023-04-02 15:38:48.248247 xklb-1.24.9/LICENSE
+-rw-r--r--   0        0        0    39259 2023-04-02 15:38:48.248247 xklb-1.24.9/README.md
+-rw-r--r--   0        0        0     8385 2023-04-02 15:38:48.248247 xklb-1.24.9/assets/kotobago.png
+-rw-r--r--   0        0        0    13982 2023-04-02 15:38:49.388317 xklb-1.24.9/pyproject.toml
+-rw-r--r--   0        0        0      686 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/__init__.py
+-rw-r--r--   0        0        0     4199 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7880 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/invalid_paths.py
+-rw-r--r--   0        0        0     1370 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4020 2023-04-02 15:38:49.388317 xklb-1.24.9/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     1009 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/nfb_ca.py
+-rw-r--r--   0        0        0     1569 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2741 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2085 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/reddit_self.py
+-rw-r--r--   0        0        0    17101 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/mining/words.py
+-rw-r--r--   0        0        0     6864 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/move_list.py
+-rw-r--r--   0        0        0      547 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9412 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/redownload.py
+-rw-r--r--   0        0        0      483 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/restore_listen_count.sql
+-rw-r--r--   0        0        0    17018 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/scatter.py
+-rw-r--r--   0        0        0     2610 2023-04-02 15:38:49.392317 xklb-1.24.9/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0       25 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/__init__.py
+-rw-r--r--   0        0        0     6846 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/av.py
+-rw-r--r--   0        0        0     6870 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/books.py
+-rw-r--r--   0        0        0     7676 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/consts.py
+-rw-r--r--   0        0        0     7602 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/db.py
+-rw-r--r--   0        0        0     7051 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/dl_config.py
+-rw-r--r--   0        0        0    14665 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13251 2023-04-02 15:38:49.392317 xklb-1.24.9/xklb/fs_extract.py
+-rw-r--r--   0        0        0     5444 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/gui.py
+-rw-r--r--   0        0        0     5904 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/hn_extract.py
+-rw-r--r--   0        0        0     8992 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/lb.py
+-rw-r--r--   0        0        0    32433 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/play_actions.py
+-rw-r--r--   0        0        0     4677 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/playback.py
+-rw-r--r--   0        0        0    25518 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/player.py
+-rw-r--r--   0        0        0    14553 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16062 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/stats.py
+-rw-r--r--   0        0        0     3824 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/subtitle.py
+-rw-r--r--   0        0        0    11986 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3607 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21477 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6258 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/tube_extract.py
+-rw-r--r--   0        0        0    26282 2023-04-02 15:38:49.396318 xklb-1.24.9/xklb/utils.py
+-rw-r--r--   0        0        0    40447 1970-01-01 00:00:00.000000 xklb-1.24.9/PKG-INFO
```

### Comparing `xklb-1.24.8/LICENSE` & `xklb-1.24.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/README.md` & `xklb-1.24.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.24.008)
+    xk media library subcommands (v1.24.009)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.24.8/assets/kotobago.png` & `xklb-1.24.9/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/pyproject.toml` & `xklb-1.24.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xklb"
-version = "1.24.008"
+version = "1.24.009"
 description = "xk library"
 authors = ["Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>"]
 readme = "README.md"
 documentation = "https://github.com/chapmanjacobd/library/wiki/Usage"
 homepage = "https://github.com/chapmanjacobd/library/"
 license = "BSD-3-Clause"
 packages = [
```

### Comparing `xklb-1.24.8/scripts/__init__.py` & `xklb-1.24.9/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/bigdirs.py` & `xklb-1.24.9/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/dedupe.py` & `xklb-1.24.9/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/invalid_paths.py` & `xklb-1.24.9/scripts/invalid_paths.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/merge_dbs.py` & `xklb-1.24.9/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/merge_online_local.py` & `xklb-1.24.9/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/mining/nfb_ca.py` & `xklb-1.24.9/scripts/mining/nfb_ca.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xklb.utils import log
+from xklb.utils import log, pipe_print
 
 
 def get_page_links(url):
     from urllib.parse import urlparse
 
     import requests
     from bs4 import BeautifulSoup
@@ -16,15 +16,15 @@
             if "/film/" in href:
                 up = urlparse(url)
                 film_list.add(up.scheme + "://" + up.netloc + href)
             else:
                 log.debug(href)
 
     for el in film_list:
-        print(el)
+        pipe_print(el)
 
 
 def nfb_films() -> None:
     import sys
 
     for l in sys.stdin:
         l = l.rstrip("\n")
```

### Comparing `xklb-1.24.8/scripts/mining/nouns.py` & `xklb-1.24.9/scripts/mining/nouns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sys
 from html.parser import HTMLParser
 from io import StringIO
 
+from xklb.utils import pipe_print
+
 from . import words
 
 """
 extract compound nouns and phrases from unstructured mixed HTML plain text
 
 xsv select text hn_comment_202210242109.csv | library nouns | sort | uniq -c | sort --numeric-sort
 """
@@ -42,15 +44,15 @@
         if not part:
             continue
 
         part_lookup = part.lower()
         if part_lookup in words.stop_words or part_lookup in words.prepositions or is_num(part):
             continue
 
-        print(part)
+        pipe_print(part)
 
 
 def line_processor(txt):
     txt = strip_tags(txt)
 
     if getattr(line_processor, "RE_NOUNS_SPLIT", None) is None:
         import regex
```

### Comparing `xklb-1.24.8/scripts/mining/pushshift.py` & `xklb-1.24.9/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/mining/reddit_self.py` & `xklb-1.24.9/scripts/mining/reddit_self.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/mining/words.py` & `xklb-1.24.9/scripts/mining/words.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/move_list.py` & `xklb-1.24.9/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/optimize_db.py` & `xklb-1.24.9/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/redownload.py` & `xklb-1.24.9/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/scatter.py` & `xklb-1.24.9/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/scripts/streaming_tab_loader.py` & `xklb-1.24.9/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/av.py` & `xklb-1.24.9/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/books.py` & `xklb-1.24.9/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/consts.py` & `xklb-1.24.9/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/db.py` & `xklb-1.24.9/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/dl_config.py` & `xklb-1.24.9/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/dl_extract.py` & `xklb-1.24.9/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/fs_extract.py` & `xklb-1.24.9/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/gui.py` & `xklb-1.24.9/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/hn_extract.py` & `xklb-1.24.9/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/lb.py` & `xklb-1.24.9/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/play_actions.py` & `xklb-1.24.9/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/playback.py` & `xklb-1.24.9/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/player.py` & `xklb-1.24.9/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,17 +714,17 @@
             wr = csv.writer(virtual_csv, quoting=csv.QUOTE_NONE)
             wr = csv.DictWriter(virtual_csv, fieldnames=args.cols)
             wr.writerows(selected_cols)
 
             virtual_csv.seek(0)
             for line in virtual_csv.readlines():
                 if args.moved:
-                    print(line.strip().replace(args.moved[0], "", 1))
+                    utils.pipe_print(line.strip().replace(args.moved[0], "", 1))
                 else:
-                    print(line.strip())
+                    utils.pipe_print(line.strip())
             if args.moved:
                 moved_media(args, list(map(operator.itemgetter("path"), media)), *args.moved)
     else:
         tbl = deepcopy(media)
         utils.col_resize(tbl, "path", 22)
         utils.col_resize(tbl, "title", 11)
```

### Comparing `xklb-1.24.8/xklb/praw_extract.py` & `xklb-1.24.9/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/stats.py` & `xklb-1.24.9/xklb/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import deepcopy
 from typing import Tuple
 
 from tabulate import tabulate
 
 from xklb import consts, db, dl_extract, play_actions, tube_backend, utils
 from xklb.player import delete_playlists
-from xklb.utils import human_time, log
+from xklb.utils import human_time, log, pipe_print
 
 
 def parse_args(prog, usage):
     parser = argparse.ArgumentParser(prog, usage)
     parser.add_argument("--fields", "-f", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--aggregate", "-a", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--json", "-j", action="store_true", help=argparse.SUPPRESS)
@@ -92,15 +92,15 @@
     tbl = deepcopy(media)
     utils.col_naturaldate(tbl, "avg_time_since_download")
     utils.col_naturalsize(tbl, "size")
     utils.col_duration(tbl, "duration")
     utils.col_duration(tbl, "avg_playlist_duration")
 
     if args.fields:
-        print("\n".join(list(map(operator.itemgetter("path"), media))))
+        pipe_print("\n".join(list(map(operator.itemgetter("path"), media))))
         return
     elif args.json or consts.TERMINAL_SIZE.columns < 80:
         print(json.dumps(tbl, indent=3))
     else:
         tbl = utils.col_resize(tbl, "path", 30)
         tbl = utils.col_resize(tbl, "title", 20)
         tbl = utils.col_resize(tbl, "uploader_url")
```

### Comparing `xklb-1.24.8/xklb/subtitle.py` & `xklb-1.24.9/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/tabs_actions.py` & `xklb-1.24.9/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/tabs_extract.py` & `xklb-1.24.9/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/tube_backend.py` & `xklb-1.24.9/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/tube_extract.py` & `xklb-1.24.9/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.24.8/xklb/utils.py` & `xklb-1.24.9/xklb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, enum, functools, hashlib, logging, math, multiprocessing, os, platform, re, shlex, shutil, signal, subprocess, sys, tempfile, textwrap
+import argparse, enum, errno, functools, hashlib, logging, math, multiprocessing, os, platform, re, shlex, shutil, signal, subprocess, sys, tempfile, textwrap
 from ast import literal_eval
 from collections.abc import Iterable
 from datetime import datetime, timedelta
 from functools import wraps
 from pathlib import Path
 from random import shuffle
 from shutil import which
@@ -871,7 +871,17 @@
         unit = unit[0]
         if unit != "s":
             unit = unit.rstrip("s")
     else:
         unit = "m"
 
     return int(float(value) * time_units[unit])
+
+
+def pipe_print(x):
+    try:
+        print(x)
+    except IOError as e:
+        if e.errno == errno.EPIPE:
+            pass
+        else:
+            raise e
```

### Comparing `xklb-1.24.8/PKG-INFO` & `xklb-1.24.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.24.8
+Version: 1.24.9
 Summary: xk library
 Home-page: https://github.com/chapmanjacobd/library/
 License: BSD-3-Clause
 Author: Jacob Chapman
 Author-email: 7908073+chapmanjacobd@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -56,15 +56,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.24.008)
+    xk media library subcommands (v1.24.009)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

