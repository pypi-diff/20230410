# Comparing `tmp/voliboli_pdf_scraper-1.4.tar.gz` & `tmp/voliboli_pdf_scraper-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voliboli_pdf_scraper-1.4.tar", last modified: Sat Mar 11 14:24:46 2023, max compression
+gzip compressed data, was "voliboli_pdf_scraper-1.5.tar", last modified: Mon Apr 10 06:28:52 2023, max compression
```

## Comparing `voliboli_pdf_scraper-1.4.tar` & `voliboli_pdf_scraper-1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-11 14:24:46.866249 voliboli_pdf_scraper-1.4/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1065 2023-03-07 14:17:09.000000 voliboli_pdf_scraper-1.4/LICENSE.md
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      929 2023-03-11 14:24:46.866249 voliboli_pdf_scraper-1.4/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      541 2023-03-11 12:17:05.000000 voliboli_pdf_scraper-1.4/README.md
--rw-rw-r--   0 dorka     (1000) dorka     (1000)       84 2023-03-05 11:20:22.000000 voliboli_pdf_scraper-1.4/pyproject.toml
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      496 2023-03-11 14:24:46.870249 voliboli_pdf_scraper-1.4/setup.cfg
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      340 2023-03-11 14:24:41.000000 voliboli_pdf_scraper-1.4/setup.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-11 14:24:46.862249 voliboli_pdf_scraper-1.4/src/
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-11 14:24:46.866249 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-03-05 10:11:19.000000 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9847 2023-03-11 11:19:59.000000 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper/constants.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4392 2023-03-11 14:18:36.000000 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper/main.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-11 14:24:46.866249 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper.egg-info/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      929 2023-03-11 14:24:46.000000 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      420 2023-03-11 14:24:46.000000 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-03-11 14:24:46.000000 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)       16 2023-03-11 14:24:46.000000 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper.egg-info/requires.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)       21 2023-03-11 14:24:46.000000 voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-11 14:24:46.866249 voliboli_pdf_scraper-1.4/tests/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      516 2023-03-11 11:45:01.000000 voliboli_pdf_scraper-1.4/tests/test_main.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1065 2023-03-07 14:17:09.000000 voliboli_pdf_scraper-1.5/LICENSE.md
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      929 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/PKG-INFO
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      541 2023-03-11 12:17:05.000000 voliboli_pdf_scraper-1.5/README.md
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)       84 2023-03-05 11:20:22.000000 voliboli_pdf_scraper-1.5/pyproject.toml
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      496 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/setup.cfg
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      340 2023-04-10 06:28:29.000000 voliboli_pdf_scraper-1.5/setup.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.006695 voliboli_pdf_scraper-1.5/src/
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-03-05 10:11:19.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9847 2023-03-11 11:19:59.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/constants.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4465 2023-04-09 12:53:21.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/main.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      929 2023-04-10 06:28:51.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      447 2023-04-10 06:28:52.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-10 06:28:51.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)       16 2023-04-10 06:28:51.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/requires.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)       21 2023-04-10 06:28:52.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/tests/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      517 2023-04-09 12:52:55.000000 voliboli_pdf_scraper-1.5/tests/test_main.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5653 2023-04-10 06:26:08.000000 voliboli_pdf_scraper-1.5/tests/test_with_db_main.py
```

### Comparing `voliboli_pdf_scraper-1.4/LICENSE.md` & `voliboli_pdf_scraper-1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voliboli_pdf_scraper-1.4/PKG-INFO` & `voliboli_pdf_scraper-1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voliboli_pdf_scraper
-Version: 1.4
+Version: 1.5
 Summary: Voliboli PDF Scraper
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `voliboli_pdf_scraper-1.4/README.md` & `voliboli_pdf_scraper-1.5/README.md`

 * *Files identical despite different names*

### Comparing `voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper/constants.py` & `voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/constants.py`

 * *Files identical despite different names*

### Comparing `voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper/main.py` & `voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,40 +28,39 @@
             return m
         elif name in w:
             return w
     return None
 
 def scrape_pdf(file, upper_bound, left_bound, lower_bound, right_bound, debug):
     res = tb.read_pdf(file, area = (upper_bound, left_bound, lower_bound, right_bound), pages = '1')[0]
-    if debug:
-        logging.debug(res)
+    if debug: logging.debug(res)
 
     return unpack_df(res)
 
 def resolve_names(numbers, teams, team, gender):
     names = []
     for num in numbers:
         try:
             names.append(teams[team][str(num)])
         except:
-            logging.warn(f"Failed to match shirt number #{num} to a {gender} in team {team}!")
+            logging.warning(f"Failed to match shirt number #{num} to a {gender} in team {team}!")
             return None
     return names
 
 def extract_players(upper_bound, lower_bound, ateam, file, debug):
     team_numbers = scrape_pdf(file, upper_bound, 20, lower_bound, 40, debug)
 
     # Unpack names based on player number - men's (in case of failure try women's)
     names = resolve_names(team_numbers, teams_men, ateam, 'men')
     if names is None:
         names = resolve_names(team_numbers, teams_women, ateam, 'women')
     if not names:
         raise Exception("Failed to resolve numbers to names while processing")
 
-    logging.info(f"Players names from {ateam}: {names}")
+    if debug: logging.info(f"Players names from {ateam}: {names}")
 
     # call the function for each item in parallel
     pool = multiprocessing.Pool()
     conf = [(file, upper_bound, 190, lower_bound, 240, debug),
             (file, upper_bound, 230, lower_bound, 250, debug),
             (file, upper_bound, 250, lower_bound, 270, debug),
             (file, upper_bound, 270, lower_bound, 290, debug),
@@ -86,38 +85,37 @@
     # Transpose scraped statistics from columns to rows
     transposed = np.array(result).T.tolist()
     pool.close()
 
     return transposed
 
 def process_pdf(file, debug):
-    logging.info("Processing PDF...")
+    if debug: logging.info("Processing PDF...")
     try:
         game = scrape_pdf(file, 40, 300, 85, 480, debug)
-        logging.info(game)
+        if debug: logging.info(game)
         team1, team2 = game
         if (ateam1 := autocomplete_teamname(team1)) is None:
             logging.error(f"Failed to resolve team name: {team1}")
             return
         if (ateam2 := autocomplete_teamname(team2)) is None:
             logging.error(f"Failed to resolve team name: {team2}")
             return
 
-        logging.info(f"Match: {ateam1} - {ateam2}")
+        if debug: logging.info(f"Match: {ateam1} - {ateam2}")
         result = scrape_pdf(file, 40, 550, 85, 570, debug)
-        logging.info(f"Result: {result}")
+        if debug: logging.info(f"Result: {result}")
         date = scrape_pdf(file, 105, 70, 115, 150, debug)
-        logging.info(f"Date: {date}")
+        if debug: logging.info(f"Date: {date}")
         location = scrape_pdf(file, 120, 70, 135, 150, debug)
-        logging.info(f"Location: {location}")
-        if debug:
-            logging.debug(result, date, location)
+        if debug: logging.info(f"Location: {location}")
+        if debug: logging.debug(result, date, location)
 
         players1 = extract_players(TEAM1_UB, TEAM1_LB, ateam1, file, debug)
-        logging.info(players1)
+        if debug: logging.info(players1)
         players2 = extract_players(TEAM2_UB, TEAM2_LB, ateam2, file, debug)
-        logging.info(players2)
+        if debug: logging.info(players2)
 
         return result, date, location, ateam1, ateam2, players1, players2
     except Exception as e:
         logging.error(e)
         return None
```

### Comparing `voliboli_pdf_scraper-1.4/src/voliboli_pdf_scraper.egg-info/PKG-INFO` & `voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voliboli-pdf-scraper
-Version: 1.4
+Version: 1.5
 Summary: Voliboli PDF Scraper
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `voliboli_pdf_scraper-1.4/tests/test_main.py` & `voliboli_pdf_scraper-1.5/tests/test_main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import unittest
 from voliboli_pdf_scraper.main import process_pdf
 
 class TestPDFScraper(unittest.TestCase):
     STAT_DIRECTORY = 'stats'
-    DEBUG = True
+    DEBUG = False
 
     def test_processing(self):
         for f in os.listdir(self.STAT_DIRECTORY):
             print(f"Processing {f} file...")
             file = os.path.join(self.STAT_DIRECTORY, f)
             output = process_pdf(file, debug=self.DEBUG)
             print(output)
```

