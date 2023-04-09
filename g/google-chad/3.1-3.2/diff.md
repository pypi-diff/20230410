# Comparing `tmp/google-chad-3.1.tar.gz` & `tmp/google-chad-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-chad-3.1.tar", last modified: Thu Apr  6 18:21:03 2023, max compression
+gzip compressed data, was "google-chad-3.2.tar", last modified: Sun Apr  9 22:32:40 2023, max compression
```

## Comparing `google-chad-3.1.tar` & `google-chad-3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 18:21:03.779134 google-chad-3.1/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-02 15:08:39.000000 google-chad-3.1/LICENSE
--rwxrwx---   0 root         (0) root         (0)      111 2023-04-02 15:08:39.000000 google-chad-3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9893 2023-04-06 18:21:03.779134 google-chad-3.1/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)     9487 2023-04-06 18:06:39.000000 google-chad-3.1/README.md
--rwxrwx---   0 root         (0) root         (0)      863 2023-04-06 18:07:57.000000 google-chad-3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 18:21:03.779134 google-chad-3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 18:21:03.775132 google-chad-3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 18:21:03.775132 google-chad-3.1/src/chad/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-06 14:54:32.000000 google-chad-3.1/src/chad/__init__.py
--rwxrwx---   0 root         (0) root         (0)    18045 2023-04-06 17:56:15.000000 google-chad-3.1/src/chad/chad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 18:21:03.775132 google-chad-3.1/src/chad_extractor/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-06 14:54:32.000000 google-chad-3.1/src/chad_extractor/__init__.py
--rwxrwx---   0 root         (0) root         (0)    22234 2023-04-06 18:06:18.000000 google-chad-3.1/src/chad_extractor/chad_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 18:21:03.775132 google-chad-3.1/src/dorks/
--rwxrwx---   0 root         (0) root         (0)      237 2023-04-06 18:08:24.000000 google-chad-3.1/src/dorks/social_media_dorks.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 18:21:03.779134 google-chad-3.1/src/google_chad.egg-info/
--rwxrwx---   0 root         (0) root         (0)     9893 2023-04-06 18:21:03.000000 google-chad-3.1/src/google_chad.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)      460 2023-04-06 18:21:03.000000 google-chad-3.1/src/google_chad.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) root         (0)        1 2023-04-06 18:21:03.000000 google-chad-3.1/src/google_chad.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) root         (0)       92 2023-04-06 18:21:03.000000 google-chad-3.1/src/google_chad.egg-info/entry_points.txt
--rwxrwx---   0 root         (0) root         (0)      129 2023-04-06 18:21:03.000000 google-chad-3.1/src/google_chad.egg-info/requires.txt
--rwxrwx---   0 root         (0) root         (0)       36 2023-04-06 18:21:03.000000 google-chad-3.1/src/google_chad.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 18:21:03.779134 google-chad-3.1/src/templates/
--rwxrwx---   0 root         (0) root         (0)     1705 2023-04-06 18:08:26.000000 google-chad-3.1/src/templates/social_media_template.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-04-06 18:22:56.000000 google-chad-3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-06 18:22:56.000000 google-chad-3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10408 2023-04-09 22:32:40.330834 google-chad-3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10002 2023-04-09 22:32:10.000000 google-chad-3.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      863 2023-04-08 21:46:58.000000 google-chad-3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 22:32:40.330834 google-chad-3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.326836 google-chad-3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.326836 google-chad-3.2/src/chad/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 18:22:56.000000 google-chad-3.2/src/chad/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19361 2023-04-09 21:26:00.000000 google-chad-3.2/src/chad/chad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/src/chad_extractor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 18:22:56.000000 google-chad-3.2/src/chad_extractor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22500 2023-04-09 21:28:17.000000 google-chad-3.2/src/chad_extractor/chad_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/src/dorks/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-06 18:22:56.000000 google-chad-3.2/src/dorks/social_media_dorks.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/src/google_chad.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10408 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/src/templates/
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-09 22:32:15.000000 google-chad-3.2/src/templates/social_media_template.json
```

### Comparing `google-chad-3.1/PKG-INFO` & `google-chad-3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 3.1
+Version: 3.2
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
@@ -54,15 +54,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.1-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.2-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -121,26 +121,26 @@
    },
    "youtube":{
       "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This page isn't available\\."
    },
    "twitter":{
-      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|i|intent|share|shearch|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|widgets\\.js)[\\w\\d\\-\\+]+)",
+      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
       "extract_prepend":"https://",
       "validate":"This account doesn.?t exist"
    },
    "instagram":{
       "extract":"instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
       "extract_append":"/",
       "validate":"Sorry, this page isn't available\\."
    },
    "facebook":{
-      "extract":"facebook\\.com\\/(?:(?!(?:about|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This page isn't available"
    },
    "linkedin-company":{
       "extract":"linkedin\\.com\\/company\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
       "extract_prepend":"https://hr.",
       "validate":"Page not found"
@@ -196,20 +196,22 @@
 chad-extractor -t social_media_template.json -res results -a user_agents.txt -o results_report.json -v yes
 ```
 
 ## Rate Limiting
 
 Google's cooling-off period can be from a few hours to a whole day.
 
-To avoid hitting the rate limit, increase minimum and maximum sleep between queries.
+To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
+
+Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.1 ( github.com/ivan-sincek/chad )
+Chad v3.2 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -225,22 +227,30 @@
     Total number of unique results
     Default: 100
     -tr <total-results> - 200 | etc.
 PAGE RESULTS
     Number of results per page - capped at 100 by Google
     Default: randint(75, 100) per page
     -pr <page-results> - 50 | etc.
-MINIMUM
-    Minimum sleep between queries
+MINIMUM QUERIES
+    Minimum sleep between Google queries
     Default: 75
-    -min <minimum> - 120 | etc.
-MAXIMUM
-    Maximum sleep between queries
+    -min-q <minimum-queries> - 120 | etc.
+MAXIMUM QUERIES
+    Maximum sleep between Google queries
     Default: minimum + 50
-    -max <maximum> - 180 | etc.
+    -max-q <maximum-queries> - 180 | etc.
+MINIMUM PAGES
+    Minimum sleep between Google pages
+    Default: 15
+    -min-p <minimum-pages> - 30 | etc.
+MAXIMUM PAGES
+    Maximum sleep between Google pages
+    Default: minimum + 10
+    -max-p <maximum-pages> - 60 | etc.
 AGENTS
     File with user agents to use
     Default: nagooglesearch user agents
     -a <agents> - user_agents.txt | etc.
 PROXIES
     File with proxies to use
     -p <proxies> - proxies.txt | etc.
@@ -260,15 +270,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.1 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.2 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.1/README.md` & `google-chad-3.2/src/google_chad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: google-chad
+Version: 3.2
+Summary: Not another Google Dorking tool.
+Author: Ivan Sincek
+Project-URL: Homepage, https://github.com/ivan-sincek/chad
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Chad
 
 Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
 
 Tested on Kali Linux v2023.1 (64-bit).
 
 Made for educational purposes. I hope it will help!
@@ -41,15 +54,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.1-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.2-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -108,26 +121,26 @@
    },
    "youtube":{
       "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This page isn't available\\."
    },
    "twitter":{
-      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|i|intent|share|shearch|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|widgets\\.js)[\\w\\d\\-\\+]+)",
+      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
       "extract_prepend":"https://",
       "validate":"This account doesn.?t exist"
    },
    "instagram":{
       "extract":"instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
       "extract_append":"/",
       "validate":"Sorry, this page isn't available\\."
    },
    "facebook":{
-      "extract":"facebook\\.com\\/(?:(?!(?:about|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This page isn't available"
    },
    "linkedin-company":{
       "extract":"linkedin\\.com\\/company\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
       "extract_prepend":"https://hr.",
       "validate":"Page not found"
@@ -183,20 +196,22 @@
 chad-extractor -t social_media_template.json -res results -a user_agents.txt -o results_report.json -v yes
 ```
 
 ## Rate Limiting
 
 Google's cooling-off period can be from a few hours to a whole day.
 
-To avoid hitting the rate limit, increase minimum and maximum sleep between queries.
+To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
+
+Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.1 ( github.com/ivan-sincek/chad )
+Chad v3.2 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -212,22 +227,30 @@
     Total number of unique results
     Default: 100
     -tr <total-results> - 200 | etc.
 PAGE RESULTS
     Number of results per page - capped at 100 by Google
     Default: randint(75, 100) per page
     -pr <page-results> - 50 | etc.
-MINIMUM
-    Minimum sleep between queries
+MINIMUM QUERIES
+    Minimum sleep between Google queries
     Default: 75
-    -min <minimum> - 120 | etc.
-MAXIMUM
-    Maximum sleep between queries
+    -min-q <minimum-queries> - 120 | etc.
+MAXIMUM QUERIES
+    Maximum sleep between Google queries
     Default: minimum + 50
-    -max <maximum> - 180 | etc.
+    -max-q <maximum-queries> - 180 | etc.
+MINIMUM PAGES
+    Minimum sleep between Google pages
+    Default: 15
+    -min-p <minimum-pages> - 30 | etc.
+MAXIMUM PAGES
+    Maximum sleep between Google pages
+    Default: minimum + 10
+    -max-p <maximum-pages> - 60 | etc.
 AGENTS
     File with user agents to use
     Default: nagooglesearch user agents
     -a <agents> - user_agents.txt | etc.
 PROXIES
     File with proxies to use
     -p <proxies> - proxies.txt | etc.
@@ -247,15 +270,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.1 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.2 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.1/pyproject.toml` & `google-chad-3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "google-chad"
-version = "3.1"
+version = "3.2"
 authors = [{ name = "Ivan Sincek" }]
 description = "Not another Google Dorking tool."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: POSIX :: Linux"
 ]
-dependencies = ["datetime>=5.0", "termcolor>=1.1.0", "nagooglesearch>=5.9", "requests>=2.27.1", "jq>=1.2.1", "asyncio>=3.4.3", "playwright>=1.27.1", "regex>=2022.4.24"]
+dependencies = ["datetime>=5.0", "termcolor>=1.1.0", "nagooglesearch>=6.0", "requests>=2.27.1", "jq>=1.2.1", "asyncio>=3.4.3", "playwright>=1.27.1", "regex>=2022.4.24"]
 
 [project.urls]
 "Homepage" = "https://github.com/ivan-sincek/chad"
 
 [project.scripts]
 chad = "chad.chad:main"
 chad-extractor = "chad_extractor.chad_extractor:main"
```

### Comparing `google-chad-3.1/src/chad/chad.py` & `google-chad-3.2/src/chad/chad.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 requests.packages.urllib3.disable_warnings(requests.packages.urllib3.exceptions.InsecureRequestWarning)
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Chad v3.1 ( github.com/ivan-sincek/chad )")
+	print("Chad v3.2 ( github.com/ivan-sincek/chad )")
 	print("")
 	print("Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]")
 	print("Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]")
 
 def advanced():
 	basic()
 	print("")
@@ -47,22 +47,30 @@
 	print("    Total number of unique results")
 	print("    Default: 100")
 	print("    -tr <total-results> - 200 | etc.")
 	print("PAGE RESULTS")
 	print("    Number of results per page - capped at 100 by Google")
 	print("    Default: randint(75, 100) per page")
 	print("    -pr <page-results> - 50 | etc.")
-	print("MINIMUM")
-	print("    Minimum sleep between queries")
+	print("MINIMUM QUERIES")
+	print("    Minimum sleep between Google queries")
 	print("    Default: 75")
-	print("    -min <minimum> - 120 | etc.")
-	print("MAXIMUM")
-	print("    Maximum sleep between queries")
+	print("    -min-q <minimum-queries> - 120 | etc.")
+	print("MAXIMUM QUERIES")
+	print("    Maximum sleep between Google queries")
 	print("    Default: minimum + 50")
-	print("    -max <maximum> - 180 | etc.")
+	print("    -max-q <maximum-queries> - 180 | etc.")
+	print("MINIMUM PAGES")
+	print("    Minimum sleep between Google pages")
+	print("    Default: 15")
+	print("    -min-p <minimum-pages> - 30 | etc.")
+	print("MAXIMUM PAGES")
+	print("    Maximum sleep between Google pages")
+	print("    Default: minimum + 10")
+	print("    -max-p <maximum-pages> - 60 | etc.")
 	print("AGENTS")
 	print("    File with user agents to use")
 	print("    Default: nagooglesearch user agents")
 	print("    -a <agents> - user_agents.txt | etc.")
 	print("PROXIES")
 	print("    File with proxies to use")
 	print("    -p <proxies> - proxies.txt | etc.")
@@ -129,15 +137,15 @@
 def error(msg, help = False):
 	global proceed
 	proceed = False
 	print_error(msg)
 	if help:
 		print("Use -h for basic and --help for advanced info")
 
-args = {"queries": None, "site": None, "time": None, "total": None, "page": None, "minimum": None, "maximum": None, "sleep": None, "proxies": None, "agents": None, "out": None, "threads": None, "directory": None, "debug": None}
+args = {"queries": None, "site": None, "time": None, "total": None, "page": None, "min-q": None, "max-q": None, "min-p": None, "max-p": None, "sleep": None, "proxies": None, "agents": None, "out": None, "threads": None, "directory": None, "debug": None}
 
 # TO DO: Better site validation.
 def validate(key, value):
 	global args
 	value = value.strip()
 	if len(value) > 0:
 		if key == "-q" and args["queries"] is None:
@@ -177,30 +185,46 @@
 			args["page"] = value
 			if not args["page"].isdigit():
 				error("Number of results per page must be numeric")
 			else:
 				args["page"] = int(args["page"])
 				if args["page"] < 1 or args["page"] > 1000:
 					error("Number of results per page must be between 1 and 1000")
-		elif key == "-min" and args["minimum"] is None:
-			args["minimum"] = value
-			if not args["minimum"].isdigit():
-				error("Minimum sleep between queries must be numeric")
-			else:
-				args["minimum"] = int(args["minimum"])
-				if args["minimum"] < 1:
-					error("Minimum sleep between queries must be greater than zero")
-		elif key == "-max" and args["maximum"] is None:
-			args["maximum"] = value
-			if not args["maximum"].isdigit():
-				error("Maximum sleep between queries must be numeric")
-			else:
-				args["maximum"] = int(args["maximum"])
-				if args["maximum"] < 1:
-					error("Maximum sleep between queries must be greater than zero")
+		elif key == "-min-q" and args["min-q"] is None:
+			args["min-q"] = value
+			if not args["min-q"].isdigit():
+				error("Minimum sleep between Google queries must be numeric")
+			else:
+				args["min-q"] = int(args["min-q"])
+				if args["min-q"] < 1:
+					error("Minimum sleep between Google queries must be greater than zero")
+		elif key == "-max-q" and args["max-q"] is None:
+			args["max-q"] = value
+			if not args["max-q"].isdigit():
+				error("Maximum sleep between Google queries must be numeric")
+			else:
+				args["max-q"] = int(args["max-q"])
+				if args["max-q"] < 1:
+					error("Maximum sleep between Google queries must be greater than zero")
+		elif key == "-min-p" and args["min-p"] is None:
+			args["min-p"] = value
+			if not args["min-p"].isdigit():
+				error("Minimum sleep between Google pages must be numeric")
+			else:
+				args["min-p"] = int(args["min-p"])
+				if args["min-p"] < 1:
+					error("Minimum sleep between Google pages must be greater than zero")
+		elif key == "-max-p" and args["max-p"] is None:
+			args["max-p"] = value
+			if not args["max-p"].isdigit():
+				error("Maximum sleep between Google pages must be numeric")
+			else:
+				args["max-p"] = int(args["max-p"])
+				if args["max-p"] < 1:
+					error("Maximum sleep between Google pages must be greater than zero")
 		elif key == "-a" and args["agents"] is None:
 			args["agents"] = value
 			if not os.path.isfile(args["agents"]):
 				error("File with user agents does not exists")
 			elif not os.access(args["agents"], os.R_OK):
 				error("File with user agents does not have read permission")
 			elif not os.stat(args["agents"]).st_size > 0:
@@ -332,22 +356,22 @@
 def get_tbs(months = None):
 	tmp = "li:1"
 	if months:
 		today = datetime.datetime.today()
 		tmp = nagooglesearch.get_tbs(today, today - relativedelta.relativedelta(months = months))
 	return tmp
 
-def run(queries, tbs = "li:1", total = 100, page = None, minimum = 75, maximum = 125, agents = None, proxies = None, sleep = False, debug = False):
+def run(queries, tbs = "li:1", total = 100, page = None, min_q = 75, max_q = 125, min_p = 15, max_p = 25, agents = None, proxies = None, sleep = False, debug = False):
 	global round_robin
 	get_timestamp("Searching Google Dorks...")
 	print("Press CTRL + C to exit early - all results will be saved")
 	results = []
 	try:
 		if not sleep:
-			wait(minimum, maximum)
+			wait(min_q, max_q)
 		count = 0
 		length = len(queries)
 		exit = False
 		for query in queries:
 			count += 1
 			entry = {"query": query, "proxy": None, "urls": None}
 			parameters = {
@@ -357,30 +381,30 @@
 				"hl": "en",
 				"filter": "0",
 				"safe": "images"
 			}
 			while not exit:
 				if proxies:
 					if round_robin:
-						wait(minimum, maximum)
+						wait(min_q, max_q)
 						round_robin = False
 					entry["proxy"] = get_proxy(proxies)
 				elif count > 1:
-					wait(minimum, maximum)
+					wait(min_q, max_q)
 				status(count, length, entry["query"], entry["proxy"])
 				remove = False
 				try:
 					client = nagooglesearch.SearchClient(
 						tld = "com",
 						parameters = parameters,
 						max_results = total,
-						user_agent = agents[random.randint(0, len(agents) - 1)] if agents else None,
+						user_agent = agents[random.randint(0, len(agents) - 1)] if agents else nagooglesearch.get_random_user_agent(),
 						proxy = entry["proxy"],
-						min_sleep = 11,
-						max_sleep = 22,
+						min_sleep = min_p,
+						max_sleep = max_p,
 						verbose = debug
 					)
 					entry["urls"] = client.search()
 					if "429_TOO_MANY_REQUESTS" in entry["urls"]:
 						print(termcolor.colored("[ HTTP 429 Too Many Requests ]", "yellow"))
 						entry["urls"].pop(entry["urls"].index("429_TOO_MANY_REQUESTS"))
 						if entry["proxy"]:
@@ -428,15 +452,15 @@
 	session = requests.Session()
 	session.max_redirects = 10
 	response = None
 	try:
 		response = session.get(url, headers = headers, proxies = None, timeout = 90, verify = False, allow_redirects = True)
 		if response.status_code == 200:
 			tmp["data"] = response.content
-	except requests.exceptions.RequestException as ex:
+	except (requests.packages.urllib3.exceptions.LocationParseError, requests.exceptions.RequestException) as ex:
 		if debug:
 			print_error(ex)
 	finally:
 		if response is not None:
 			response.close()
 		session.close()
 	return tmp
@@ -491,46 +515,50 @@
 			advanced()
 		else:
 			error("Incorrect usage", True)
 	elif argc % 2 == 0 and argc <= len(args) * 2:
 		for i in range(1, argc, 2):
 			validate(sys.argv[i], sys.argv[i + 1])
 		if args["queries"] is None or not check(argc, args):
-			error("Missing a mandatory option (-q) and/or optional (-s, -t, -tr, -pr, -min, -max, -a, -p, -th, -d, -o, -sos, -dbg)", True)
+			error("Missing a mandatory option (-q) and/or optional (-s, -t, -tr, -pr, -min-q, -max-q, -min-p, -max-p, -a, -p, -th, -d, -o, -sos, -dbg)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed:
 		print("#######################################################################")
 		print("#                                                                     #")
-		print("#                              Chad v3.1                              #")
+		print("#                              Chad v3.2                              #")
 		print("#                                   by Ivan Sincek                    #")
 		print("#                                                                     #")
 		print("# Search Google Dorks like Chad.                                      #")
 		print("# GitHub repository at github.com/ivan-sincek/chad.                   #")
 		print("# Feel free to donate bitcoin at 1BrZM6T7G9RN8vbabnfXu4M6Lpgztq6Y14.  #")
 		print("#                                                                     #")
 		print("#######################################################################")
 		# --------------------
 		if not args["total"]:
 			args["total"] = 100
-		if not args["minimum"]:
-			args["minimum"] = 75
-		if not args["maximum"] or args["minimum"] > args["maximum"]:
-			args["maximum"] = args["minimum"] + 50
+		if not args["min-q"]:
+			args["min-q"] = 75
+		if not args["max-q"] or args["min-q"] > args["max-q"]:
+			args["max-q"] = args["min-q"] + 50
+		if not args["min-p"]:
+			args["min-p"] = 15
+		if not args["max-p"] or args["min-p"] > args["max-p"]:
+			args["max-p"] = args["min-p"] + 10
 		if not args["threads"]:
 			args["threads"] = 5
 		# --------------------
 		get_timestamp("Validating Google Dorks...")
 		print("Google only allows queries up to 32 words in length separated by space")
 		args["queries"] = validate_queries(args["queries"], args["site"])
 		if not args["queries"]:
 			print("No valid queries are left")
 		else:
-			results = run(args["queries"], get_tbs(args["time"]), args["total"], args["page"], args["minimum"], args["maximum"], args["agents"], args["proxies"], args["sleep"], args["debug"])
+			results = run(args["queries"], get_tbs(args["time"]), args["total"], args["page"], args["min-q"], args["max-q"], args["min-p"], args["max-p"], args["agents"], args["proxies"], args["sleep"], args["debug"])
 			if not results:
 				print("No results")
 			else:
 				if args["directory"]:
 					download_files(results, args["directory"], args["threads"], args["agents"], args["debug"])
 				results = jdump(results)
 				print(results)
```

### Comparing `google-chad-3.1/src/chad_extractor/chad_extractor.py` & `google-chad-3.2/src/chad_extractor/chad_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 start = datetime.datetime.now()
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Chad Extractor v3.1 ( github.com/ivan-sincek/chad )")
+	print("Chad Extractor v3.2 ( github.com/ivan-sincek/chad )")
 	print("")
 	print("Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]")
 	print("Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]")
 
 def advanced():
 	basic()
 	print("")
@@ -83,15 +83,15 @@
 	array = [x for x in sequence if not (x in seen or seen.add(x))]
 	if sort and array:
 		array = sorted(array, key = str.casefold)
 	return array
 
 def read_file(file, sort = False, text = False):
 	flags = "r"
-	encoding = "ISO-8859-1"
+	encoding = "UTF-8"
 	if text:
 		return open(file, flags, encoding = encoding).read()
 	else:
 		tmp = []
 		with open(file, flags, encoding = encoding) as stream:
 			for line in stream:
 				line = line.strip()
@@ -100,25 +100,24 @@
 		stream.close()
 		return unique(tmp, sort)
 
 def read_json(file):
 	tmp = []
 	try:
 		tmp = json.loads(open(file, "r", encoding = "UTF-8").read())
-	except Exception:
+	except json.decoder.JSONDecodeError:
 		pass
 	return tmp
 
 def jquery(obj, query):
 	tmp = []
-	if obj:
-		try:
-			tmp = jq.compile(query).input(obj).all()
-		except Exception:
-			pass
+	try:
+		tmp = jq.compile(query).input(obj).all()
+	except ValueError:
+		pass
 	return tmp
 
 def jdump(data):
 	return json.dumps(data, indent = 4, ensure_ascii = False)
 
 def write_file(data, out):
 	confirm = "yes"
@@ -253,23 +252,30 @@
 	return argc - count == argc / 2
 
 # --------------------- VALIDATION END ---------------------
 
 # ----------------- GLOBAL VARIABLES BEGIN -----------------
 
 def get_data():
-	return {"data": [], "lock": threading.Lock()}
+	return {
+		"data": [],
+		"lock": threading.Lock()
+	}
 
-data = {"extracted": get_data(), "failed_extraction": get_data(), "validated": get_data(), "failed_validation": get_data()}
+data = {
+	"extracted": get_data(),
+	"failed_extraction": get_data(),
+	"validated": get_data(),
+	"failed_validation": get_data()
+}
 
 def extend_data(key, array):
 	global data
-	if key in data:
-		with data[key]["lock"]:
-			data[key]["data"].extend(array)
+	with data[key]["lock"]:
+		data[key]["data"].extend(array)
 
 queries = {
 	"get_url": ".[].url",
 	"get_urls": ".[].urls[]",
 	"sort_by_url": "sort_by(.url | ascii_downcase)[]",
 	"group_by_url": "group_by(.url) | map((.[0] | del(.file)) + {files: (map(.file) | unique)})[]",
 	"get_file": ".[].file",
@@ -295,20 +301,32 @@
 	else:
 		return [records]
 
 def parse_response(skey, template, record, response):
 	tmp = {}
 	if skey == "extracted":
 		for key in template:
-			matches = re.findall(template[key]["extract"], response, re.MULTILINE | re.IGNORECASE)
-			if matches:
-				try:
-					tmp[key] = unique([(template[key]["extract_prepend"] if "extract_prepend" in template[key] else "") + match + (template[key]["extract_append"] if "extract_append" in template[key] else "") for match in matches], True)
-				except Exception as ex:
-					print_error(("{0} | {1}").format(key, ex))
+			try:
+				matches = re.findall(template[key]["extract"], response, re.MULTILINE | re.IGNORECASE)
+				if matches:
+					if "extract_prepend" in template[key] or "extract_append" in template[key]:
+						prepend = ""
+						if "extract_prepend" in template[key]:
+							prepend = template[key]["extract_prepend"]
+						append = ""
+						if "extract_append" in template[key]:
+							append = template[key]["extract_append"]
+						tmp[key] = []
+						for match in matches:
+							tmp[key].append(prepend + match + append)
+					else:
+						tmp[key] = matches
+					tmp[key] = unique(tmp[key], True)
+			except Exception as ex:
+				print_error(("{0} | {1}").format(key, ex))
 	elif skey == "validated" and re.search(template[record["id"]]["validate"], response, re.MULTILINE | re.IGNORECASE):
 		tmp = True
 	return tmp
 
 async def block(route):
 	await route.abort() if route.request.resource_type in ["stylesheet", "image", "media", "font", "ping"] else await route.continue_()
 
@@ -330,15 +348,15 @@
 			for exclude in excludes:
 				tmp["response"] = re.sub(exclude, "", tmp["response"], re.MULTILINE | re.IGNORECASE)
 	except PlaywrightTimeoutError:
 		pass
 	except Exception: # in case of a file or invalid domain, fallback
 		tmp["error"] = True
 	finally:
-		if page is not None:
+		if page:
 			await page.close()
 	return tmp
 
 async def request_get(context, url, excludes = []):
 	tmp = {"response": None, "error": False}
 	try:
 		response = await context.request.get(url)
@@ -395,15 +413,20 @@
 				await context.clear_cookies() # anti-bot evasion 3
 		await context.close()
 		await browser.close()
 	extend_data(skey, succeeded)
 	extend_data(fkey, failed)
 
 def proxy_browser_requests(template, records, excludes = [], retries = 2, wait = 4, agents = None, extract = True):
-	asyncio.run(browser_requests("extracted" if extract else "validated", "failed_extraction" if extract else "failed_validation", template, records, excludes, retries, wait, agents))
+	skey = "extracted"
+	fkey = "failed_extraction"
+	if not extract:
+		skey = "validated"
+		fkey = "failed_validation"
+	asyncio.run(browser_requests(skey, fkey, template, records, excludes, retries, wait, agents))
 
 def parse_template(template, extract = True):
 	tmp = {}
 	if extract:
 		for key in template:
 			if "extract" in template[key]:
 				tmp[key] = template[key]
@@ -519,15 +542,15 @@
 			error("Missing a mandatory option (-t, -res, -o) and/or optional (-pt, -e, -th, -r, -w, -a, -v)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed:
 		print("#######################################################################")
 		print("#                                                                     #")
-		print("#                         Chad Extractor v3.1                         #")
+		print("#                         Chad Extractor v3.2                         #")
 		print("#                                   by Ivan Sincek                    #")
 		print("#                                                                     #")
 		print("# Extract and validate data from Chad results.                        #")
 		print("# GitHub repository at github.com/ivan-sincek/chad.                   #")
 		print("# Feel free to donate bitcoin at 1BrZM6T7G9RN8vbabnfXu4M6Lpgztq6Y14.  #")
 		print("#                                                                     #")
 		print("#######################################################################")
```

### Comparing `google-chad-3.1/src/google_chad.egg-info/PKG-INFO` & `google-chad-3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: google-chad
-Version: 3.1
-Summary: Not another Google Dorking tool.
-Author: Ivan Sincek
-Project-URL: Homepage, https://github.com/ivan-sincek/chad
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Chad
 
 Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
 
 Tested on Kali Linux v2023.1 (64-bit).
 
 Made for educational purposes. I hope it will help!
@@ -54,15 +41,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.1-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.2-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -121,26 +108,26 @@
    },
    "youtube":{
       "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This page isn't available\\."
    },
    "twitter":{
-      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|i|intent|share|shearch|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|widgets\\.js)[\\w\\d\\-\\+]+)",
+      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
       "extract_prepend":"https://",
       "validate":"This account doesn.?t exist"
    },
    "instagram":{
       "extract":"instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
       "extract_append":"/",
       "validate":"Sorry, this page isn't available\\."
    },
    "facebook":{
-      "extract":"facebook\\.com\\/(?:(?!(?:about|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This page isn't available"
    },
    "linkedin-company":{
       "extract":"linkedin\\.com\\/company\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
       "extract_prepend":"https://hr.",
       "validate":"Page not found"
@@ -196,20 +183,22 @@
 chad-extractor -t social_media_template.json -res results -a user_agents.txt -o results_report.json -v yes
 ```
 
 ## Rate Limiting
 
 Google's cooling-off period can be from a few hours to a whole day.
 
-To avoid hitting the rate limit, increase minimum and maximum sleep between queries.
+To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
+
+Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.1 ( github.com/ivan-sincek/chad )
+Chad v3.2 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -225,22 +214,30 @@
     Total number of unique results
     Default: 100
     -tr <total-results> - 200 | etc.
 PAGE RESULTS
     Number of results per page - capped at 100 by Google
     Default: randint(75, 100) per page
     -pr <page-results> - 50 | etc.
-MINIMUM
-    Minimum sleep between queries
+MINIMUM QUERIES
+    Minimum sleep between Google queries
     Default: 75
-    -min <minimum> - 120 | etc.
-MAXIMUM
-    Maximum sleep between queries
+    -min-q <minimum-queries> - 120 | etc.
+MAXIMUM QUERIES
+    Maximum sleep between Google queries
     Default: minimum + 50
-    -max <maximum> - 180 | etc.
+    -max-q <maximum-queries> - 180 | etc.
+MINIMUM PAGES
+    Minimum sleep between Google pages
+    Default: 15
+    -min-p <minimum-pages> - 30 | etc.
+MAXIMUM PAGES
+    Maximum sleep between Google pages
+    Default: minimum + 10
+    -max-p <maximum-pages> - 60 | etc.
 AGENTS
     File with user agents to use
     Default: nagooglesearch user agents
     -a <agents> - user_agents.txt | etc.
 PROXIES
     File with proxies to use
     -p <proxies> - proxies.txt | etc.
@@ -260,15 +257,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.1 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.2 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.1/src/templates/social_media_template.json` & `google-chad-3.2/src/templates/social_media_template.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'facebook'": "{'extract': "*

 * *               "'facebook\\\\.com\\\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\\\/|\\\\?)[^\\\\s]+|share\\\\.php|terms\\\\.php)[\\\\w\\\\d\\\\-\\\\+\\\\.]+)(?<!\\\\.)'}",*

 * * "'twitter'": "{'extract': "*

 * *              "'(?<!pic\\\\.)twitter\\\\.com\\\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\\\/|\\\\?)[^\\\\s]+|[\\\\w]+\\\\/(?:privacy|tos)|personalization|widgets\\\\.js)[\\\\w\\\\d\\\\-\\\\+]+)'}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "discord": {
         "extract": "discord\\.com\\/invite\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
         "extract_prepend": "https://",
         "validate": "Invite Invalid"
     },
     "facebook": {
-        "extract": "facebook\\.com\\/(?:(?!(?:about|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+        "extract": "facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
         "extract_prepend": "https://",
         "validate": "This page isn't available"
     },
     "instagram": {
         "extract": "instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
         "extract_append": "/",
         "extract_prepend": "https://",
@@ -27,15 +27,15 @@
     },
     "telegram": {
         "extract": "t\\.me\\/[\\w\\d\\-\\+]+",
         "extract_prepend": "https://",
         "validate": "<meta property=\"og:title\" content=\"Telegram: Contact .+?\">"
     },
     "twitter": {
-        "extract": "(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|i|intent|share|shearch|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|widgets\\.js)[\\w\\d\\-\\+]+)",
+        "extract": "(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
         "extract_prepend": "https://",
         "validate": "This account doesn.?t exist"
     },
     "youtube": {
         "extract": "youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
         "extract_prepend": "https://",
         "validate": "This page isn't available\\."
```

