# Comparing `tmp/letterboxd_stats-0.1.3.tar.gz` & `tmp/letterboxd_stats-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.1.3.tar", last modified: Wed Mar 15 15:36:13 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.1.4.tar", last modified: Sun Apr  9 23:05:01 2023, max compression
```

## Comparing `letterboxd_stats-0.1.3.tar` & `letterboxd_stats-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-03-15 15:36:13.809394 letterboxd_stats-0.1.3/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.3/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2697 2023-03-15 15:36:13.809394 letterboxd_stats-0.1.3/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2203 2023-03-08 15:15:35.000000 letterboxd_stats-0.1.3/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-03-15 15:36:13.809394 letterboxd_stats-0.1.3/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1486 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.3/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5201 2023-03-14 10:28:56.000000 letterboxd_stats-0.1.3/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2194 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.3/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2827 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.3/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-03-15 15:34:30.000000 letterboxd_stats-0.1.3/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     4697 2023-03-15 15:33:34.000000 letterboxd_stats-0.1.3/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-03-15 15:36:13.809394 letterboxd_stats-0.1.3/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2697 2023-03-15 15:36:13.000000 letterboxd_stats-0.1.3/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-03-15 15:36:13.000000 letterboxd_stats-0.1.3/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-03-15 15:36:13.000000 letterboxd_stats-0.1.3/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-03-15 15:36:13.000000 letterboxd_stats-0.1.3/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-03-15 15:36:13.000000 letterboxd_stats-0.1.3/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-03-15 15:36:13.000000 letterboxd_stats-0.1.3/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      841 2023-03-15 15:35:57.000000 letterboxd_stats-0.1.3/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-03-15 15:36:13.809394 letterboxd_stats-0.1.3/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.4/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2697 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2203 2023-03-08 15:15:35.000000 letterboxd_stats-0.1.4/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1563 2023-04-09 22:57:57.000000 letterboxd_stats-0.1.4/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5216 2023-04-09 22:57:57.000000 letterboxd_stats-0.1.4/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3494 2023-04-09 23:04:29.000000 letterboxd_stats-0.1.4/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3175 2023-04-09 22:57:57.000000 letterboxd_stats-0.1.4/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2574 2023-04-08 16:03:39.000000 letterboxd_stats-0.1.4/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     4697 2023-03-15 22:58:55.000000 letterboxd_stats-0.1.4/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2697 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      841 2023-04-09 22:58:10.000000 letterboxd_stats-0.1.4/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/setup.cfg
```

### Comparing `letterboxd_stats-0.1.3/LICENCE` & `letterboxd_stats-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.3/PKG-INFO` & `letterboxd_stats-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd_stats
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small example package
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.1.3/README.md` & `letterboxd_stats-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.3/letterboxd_stats/__init__.py` & `letterboxd_stats-0.1.4/letterboxd_stats/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "--download",
     help="Download letterboxd data from your account",
     action="store_true",
 )
 parser.add_argument("-W", "--wishlist", help="show wishlist", action="store_true")
 parser.add_argument("-D", "--diary", help="show diary", action="store_true")
 parser.add_argument("-R", "--ratings", help="show ratings", action="store_true")
+parser.add_argument("-L", "--lists", help="show lists", action="store_true")
 parser.add_argument("-l", "--limit", help="limit the number of items of your wishlist/diary", type=int)
 parser.add_argument("-a", "--ascending", help="Use ascending order when you sort the entries", action="store_true")
 parser.add_argument("-c", "--config_folder", help="Specifiy the folder of your config.toml file")
 
 
 args = parser.parse_args()
```

### Comparing `letterboxd_stats-0.1.3/letterboxd_stats/cli.py` & `letterboxd_stats-0.1.4/letterboxd_stats/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,16 +65,16 @@
         choices=[Choice(value=url, name=f"{title}") for url, title in zip(movie_df["Url"], movie_df["Title"])],
         keybindings={"skip": [{"key": "escape"}]},
         invalid_message="Input must be in the resulting IDs",
     ).execute()
     return result
 
 
-def print_film(film):
-    grid = Table.grid(expand=True, padding=1)
+def print_film(film, expand=True):
+    grid = Table.grid(expand=expand, padding=1)
     grid.add_column(style="bold yellow")
     grid.add_column()
     for k, v in film.items():
         grid.add_row(str(k), str(v))
     console = Console()
     console.print(grid)
```

### Comparing `letterboxd_stats-0.1.3/letterboxd_stats/main.py` & `letterboxd_stats-0.1.4/letterboxd_stats/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -67,24 +67,33 @@
 def get_ratings(args_limit, args_ascending):
     path = os.path.expanduser(os.path.join(config["root_folder"], "static", "ratings.csv"))
     check_path(path)
     letterboxd_url = data.open_file("Ratings", path, args_limit, args_ascending)
     get_movie_detail_from_url(letterboxd_url)
 
 
+def get_lists(args_limit, args_ascending):
+    path = os.path.expanduser(os.path.join(config["root_folder"], "static", "lists"))
+    check_path(path)
+    letterboxd_url = data.open_list(path, args_limit, args_ascending)
+    get_movie_detail_from_url(letterboxd_url)
+
+
 def main():
     if args.download:
         try_command(download_data, ())
     if args.search:
         try_command(search_person, (args.search,))
     if args.search_film:
         try_command(search_film, (args.search_film,))
     if args.wishlist:
         try_command(get_wishlist, (args.limit, args.ascending))
     if args.diary:
         try_command(get_diary, (args.limit, args.ascending))
     if args.ratings:
         try_command(get_ratings, (args.limit, args.ascending))
+    if args.lists:
+        try_command(get_lists, (args.limit, args.ascending))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `letterboxd_stats-0.1.3/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.1.4/letterboxd_stats/tmdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,21 @@
         raise Exception("No results for your search")
     result_index = cli.select_search_result(names)  # type: ignore
     search_result = search_results[result_index]
     p = person.details(search_result["id"])
     known_for_department = p["known_for_department"]
     movie_credits = person.movie_credits(search_result["id"])
     list_of_films = [
-        {"title": m.title, "release_date": m.release_date, "department": m.department, "id": m.id}
+        {
+            "title": m.title,
+            "release_date": m.release_date,
+            "department": m.department,
+            "id": m.id,
+            "duration": movie.details(m.id).runtime,  # type: ignore
+        }
         for m in movie_credits["crew"]
     ]
     if len(list_of_films) == 0:
         raise ValueError("The selected person doesn't have any film.")
     df = pd.DataFrame(list_of_films)
     department = cli.select_value(
         df["department"].unique(), f"Select a department for {p['name']}", known_for_department
```

### Comparing `letterboxd_stats-0.1.3/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.1.4/letterboxd_stats/web_scraper.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.3/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.1.4/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd-stats
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small example package
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.1.3/pyproject.toml` & `letterboxd_stats-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "mBaratta96" }]
 description = "A small example package"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
```

