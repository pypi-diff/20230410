# Comparing `tmp/longitudinal_trends-0.0.5.tar.gz` & `tmp/longitudinal_trends-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longitudinal_trends-0.0.5.tar", last modified: Fri Apr  7 07:05:09 2023, max compression
+gzip compressed data, was "longitudinal_trends-0.1.0.tar", last modified: Mon Apr 10 18:34:04 2023, max compression
```

## Comparing `longitudinal_trends-0.0.5.tar` & `longitudinal_trends-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-07 07:05:09.576433 longitudinal_trends-0.0.5/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.0.5/LICENSE
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.0.5/MANIFEST.in
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9882 2023-04-07 07:05:09.570425 longitudinal_trends-0.0.5/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9349 2023-04-07 07:04:07.000000 longitudinal_trends-0.0.5/README.md
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-07 07:05:09.268182 longitudinal_trends-0.0.5/longitudinal_trends/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17278 2023-04-03 19:40:54.000000 longitudinal_trends-0.0.5/longitudinal_trends/__init__.py
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-07 07:05:09.507698 longitudinal_trends-0.0.5/longitudinal_trends.egg-info/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9882 2023-04-07 07:05:08.000000 longitudinal_trends-0.0.5/longitudinal_trends.egg-info/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-04-07 07:05:09.000000 longitudinal_trends-0.0.5/longitudinal_trends.egg-info/SOURCES.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-04-07 07:05:08.000000 longitudinal_trends-0.0.5/longitudinal_trends.egg-info/dependency_links.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-04-07 07:05:08.000000 longitudinal_trends-0.0.5/longitudinal_trends.egg-info/requires.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-04-07 07:05:08.000000 longitudinal_trends-0.0.5/longitudinal_trends.egg-info/top_level.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1096 2023-04-07 07:04:37.000000 longitudinal_trends-0.0.5/pyproject.toml
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      136 2023-04-03 18:57:25.000000 longitudinal_trends-0.0.5/requirements.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-04-07 07:05:09.578426 longitudinal_trends-0.0.5/setup.cfg
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-10 18:34:04.310888 longitudinal_trends-0.1.0/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.0/LICENSE
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.0/MANIFEST.in
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9883 2023-04-10 18:34:04.310888 longitudinal_trends-0.1.0/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9349 2023-04-07 07:04:07.000000 longitudinal_trends-0.1.0/README.md
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-10 18:34:04.115846 longitudinal_trends-0.1.0/longitudinal_trends/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17412 2023-04-10 18:21:23.000000 longitudinal_trends-0.1.0/longitudinal_trends/__init__.py
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-10 18:34:04.262911 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9883 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/SOURCES.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/dependency_links.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/requires.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/top_level.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1097 2023-04-10 18:23:40.000000 longitudinal_trends-0.1.0/pyproject.toml
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)      136 2023-04-03 18:57:25.000000 longitudinal_trends-0.1.0/requirements.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-04-10 18:34:04.315900 longitudinal_trends-0.1.0/setup.cfg
```

### Comparing `longitudinal_trends-0.0.5/LICENSE` & `longitudinal_trends-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.0.5/PKG-INFO` & `longitudinal_trends-0.1.0/longitudinal_trends.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: longitudinal_trends
-Version: 0.0.5
+Name: longitudinal-trends
+Version: 0.1.0
 Summary: Download long-term longitudinal Google Trends
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: google trends api search longtrends cross section
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `longitudinal_trends-0.0.5/README.md` & `longitudinal_trends-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.0.5/longitudinal_trends/__init__.py` & `longitudinal_trends-0.1.0/longitudinal_trends/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd
 import os
 import glob
 import json
 
+import requests
 from pytrends.exceptions import ResponseError
 from pytrends.request import TrendReq
 
 import datetime as dt
 from dateutil.relativedelta import *
 import time
 
@@ -14,14 +15,19 @@
 from rich.console import Console
 from rich.logging import RichHandler
 
 from math import ceil
 
 console = Console()
 
+session = requests.Session()
+session.get('https://trends.google.com')
+cookies_map = session.cookies.get_dict()
+nid_cookie = cookies_map['NID']
+
 class RequestTrends:
 
     logging.basicConfig(
         level="INFO", format="%(message)s", datefmt="%d-%b-%Y %H:%M:%S", handlers=[RichHandler(rich_tracebacks=True)]
     )
 
 
@@ -86,17 +92,16 @@
         }
         params_fl = '{}/{}/params.txt'.format(folder_name, data_format)
         with open(params_fl, 'w') as fl:
             fl.write(json.dumps(params, indent=4, sort_keys=True, default=str))
         fl.close()
 
         # Initiaate pytrends request to enquire later
-        self.__pytrend = TrendReq(hl='en-US', tz=360)
+        self.__pytrend = TrendReq(hl='en-US', tz=360, requests_args={'headers': {'Cookie': f'NID={nid_cookie}'}})
         self.__logger.info("Pytrend instance have been initiated for longitudinal_trend", extra={"markup": True})
-        # self.__logger.info("{} Number of Days".format(self.__num_of_days))
 
     def __in_notebook(self):
         try:
             from IPython import get_ipython
             if 'IPKernelApp' not in get_ipython().config:  # pragma: no cover
                 return False                
         except ImportError:
@@ -181,14 +186,15 @@
                     df.to_csv("{}/{}/by_region/{}_{}-{}-{}.csv".format(self.keyword, self.data_format,  form, i, current_time.strftime("%Y%m%d"), current_end_time.strftime("%Y%m%d")))
 
                     current_time += chng_delta
 
             self.__logger.info("[bold green]Successfully Collected Required Data![/]", extra={"markup": True})
 
 
+    # Time Series Data collection method for 'monthly'
     def __time_series_monthly(self, stats, reference_geo_code="US"):
         if os.path.exists("{}/{}/over_time/{}/{}-{}.csv".format(self.folder_name, self.data_format, reference_geo_code, self.start_date.strftime("%Y%m%d"), self.end_date.strftime("%Y%m%d"))):
             stats.stop()
             self.__logger.info("All Data for current request is already collected", extra={"markup": True})
         else:
             try:
                 self.__pytrend.build_payload(kw_list=[self.topic], geo=reference_geo_code, 
@@ -203,14 +209,15 @@
                 self.__logger.info("Please have patience as we reset rate limit ... ", extra={"markup": True})
                 time.sleep(15)
             except:
                 stats.stop()
                 self.__logger.error("[bold red]Whoops![/]", exc_info=1, extra={"markup": True})
 
 
+    # Time Series Data collection method for 'weekly'/'daily'
     def __time_series_nmonthly(self, stats, reference_geo_code="US"):
         for period in range(len(self.__times)-1):
             start, end = self.__times[period], self.__times[period+1]
 
             if self.data_format == "weekly":
                 num_days = (end - start).days
                 if num_days < 270:
@@ -219,28 +226,26 @@
             
             if os.path.exists("{}/{}/over_time/{}/{}-{}-{}.csv".format(self.folder_name, self.data_format, reference_geo_code, period+1, start.strftime("%Y%m%d"), end.strftime("%Y%m%d"))):
                 self.__logger.info("Data for {} to {} already collected. Moving to next date...".format(start.strftime("%#d/%m/%#Y"), end.strftime("%#d/%m/%#Y")), extra={"markup": True})
             else:
                 try:
                     self.__pytrend.build_payload(kw_list=[self.topic], geo=reference_geo_code, 
                                         timeframe='%s %s' % (start.strftime("%Y-%m-%d"), end.strftime("%Y-%m-%d"))) 
-                    time.sleep(5)
+                    time.sleep(15)
                     df = self.__pytrend.interest_over_time()
 
                 except ResponseError as e:
                     self.__logger.info("Please have patience as we reset rate limit ... ", extra={"markup": True})
-                    time.sleep(5)
+                    time.sleep(15)
                     continue
                 except:
                     stats.stop()
                     self.__logger.error("[bold red]Whoops![/]", exc_info=1, extra={"markup": True})
                     break
 
-                time.sleep(5)
-
                 if df.empty:
                     stats.stop()
                     self.__logger.info("No Data was returned for period: {} -> '{}' to '{}'".format(period+1, start.strftime("%#d/%m/%#Y"), end.strftime("%#d/%m/%#Y")), extra={"markup": True})
                 else:                    
                     df = df.rename(columns={self.topic:self.keyword})
                     df.drop('isPartial', axis=1, inplace=True)
                     df.to_csv("{}/{}/over_time/{}/{}-{}-{}.csv".format(self.folder_name, self.data_format, reference_geo_code, period+1, start.strftime("%Y%m%d"), end.strftime("%Y%m%d")))
@@ -260,16 +265,14 @@
             if self.TIME_WINDOW:
                 self.__time_series_nmonthly(stats, reference_geo_code)
             else:
                 self.__time_series_monthly(stats, reference_geo_code)
 
 
     def concat_time_series(self, reference_geo_code: str="US", zero_replace: float=0.1):
-        #TODO: Put a caution about the 100/0.1 inflating overall index by a factor of 1000
-
         self.__logger.info("Concatenating Over Time data now", extra={"markup": True})
 
         # Create Folder to save the concatenated time series data
         self.__create_required_directory("{}/{}/concat_time_series".format(self.folder_name, self.data_format))
 
         path_to_time_data = "{}/{}/over_time/{}".format(self.folder_name, self.data_format, reference_geo_code)
 
@@ -342,11 +345,8 @@
 
         # Next Merge/Concatenate over the time data into a single long term trend
         self.concat_time_series(reference_geo_code, zero_replace)
 
         # Finally rescale all across region data by converting them 
         self.convert_cross_section(reference_geo_code, zero_replace)
 
-        self.__logger.info("[bold green]DONE! :) [/]", extra={"markup": True})
-
-
-
+        self.__logger.info("[bold green]DONE! :) [/]", extra={"markup": True})
```

### Comparing `longitudinal_trends-0.0.5/longitudinal_trends.egg-info/PKG-INFO` & `longitudinal_trends-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: longitudinal-trends
-Version: 0.0.5
+Name: longitudinal_trends
+Version: 0.1.0
 Summary: Download long-term longitudinal Google Trends
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: google trends api search longtrends cross section
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `longitudinal_trends-0.0.5/pyproject.toml` & `longitudinal_trends-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools"]#, "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "longitudinal_trends"
-version='0.0.5'
+version='0.1.0'
 description="Download long-term longitudinal Google Trends"
 urls = {homepage = "https://github.com/Mohammad-sakir/longitudinalTrends"}
 requires-python = ">=3.6"
 authors = [
     {name = "Mohammad Saleh Ahsan Sakir"},
     {name = "Taeyong Park"}, 
     {email="ahsansakir506@gmail.com"},    
     {email = "taeyongp@andrew.cmu.edu"}
 ]
 license = {text="MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Development Status :: 1 - Planning",
+    "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 keywords = [
     "google trends api search longtrends cross section"
```

