# Comparing `tmp/rechtspraak_extractor-1.1.7.tar.gz` & `tmp/rechtspraak_extractor-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rechtspraak_extractor-1.1.7.tar", last modified: Tue Apr  4 16:49:50 2023, max compression
+gzip compressed data, was "rechtspraak_extractor-1.1.8.tar", last modified: Mon Apr 10 11:11:24 2023, max compression
```

## Comparing `rechtspraak_extractor-1.1.7.tar` & `rechtspraak_extractor-1.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 16:49:50.871763 rechtspraak_extractor-1.1.7/
--rw-rw-rw-   0        0        0     6911 2023-04-04 16:49:50.870763 rechtspraak_extractor-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6386 2023-03-14 13:47:20.000000 rechtspraak_extractor-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 16:49:50.859764 rechtspraak_extractor-1.1.7/rechtspraak_extractor/
--rw-rw-rw-   0        0        0      251 2022-10-29 13:29:59.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor/__init__.py
--rw-rw-rw-   0        0        0     4712 2023-04-04 16:34:12.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor/rechtspraak.py
--rw-rw-rw-   0        0        0     1391 2023-04-04 16:48:14.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor/rechtspraak_functions.py
--rw-rw-rw-   0        0        0    14744 2023-04-04 16:28:38.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor/rechtspraak_metadata.py
--rw-rw-rw-   0        0        0      173 2023-04-04 16:34:12.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor/testing_file.py
-drwxrwxrwx   0        0        0        0 2023-04-04 16:49:50.868762 rechtspraak_extractor-1.1.7/rechtspraak_extractor.egg-info/
--rw-rw-rw-   0        0        0     6911 2023-04-04 16:49:50.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-04-04 16:49:50.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 16:49:50.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-04 16:49:50.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-04 16:49:50.000000 rechtspraak_extractor-1.1.7/rechtspraak_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 16:49:50.872763 rechtspraak_extractor-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-04-04 16:49:43.000000 rechtspraak_extractor-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:11:24.659837 rechtspraak_extractor-1.1.8/
+-rw-rw-rw-   0        0        0     6911 2023-04-10 11:11:24.658837 rechtspraak_extractor-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6386 2023-03-14 13:47:20.000000 rechtspraak_extractor-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 11:11:24.646834 rechtspraak_extractor-1.1.8/rechtspraak_extractor/
+-rw-rw-rw-   0        0        0      251 2022-10-29 13:29:59.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3800 2023-04-10 10:34:04.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak.py
+-rw-rw-rw-   0        0        0     1391 2023-04-04 16:48:14.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak_functions.py
+-rw-rw-rw-   0        0        0    14747 2023-04-10 10:34:04.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak_metadata.py
+-rw-rw-rw-   0        0        0      187 2023-04-10 10:58:00.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/testing_file.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:11:24.656834 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/
+-rw-rw-rw-   0        0        0     6911 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 11:11:24.659837 rechtspraak_extractor-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-04-10 11:11:16.000000 rechtspraak_extractor-1.1.8/setup.py
```

### Comparing `rechtspraak_extractor-1.1.7/PKG-INFO` & `rechtspraak_extractor-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak_extractor
-Version: 1.1.7
+Version: 1.1.8
 Summary: Library for extracting rechtspraak data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: pranav.bapat@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak_extractor Version: 1.1.7 Summary:
+Metadata-Version: 2.1 Name: rechtspraak_extractor Version: 1.1.8 Summary:
 Library for extracting rechtspraak data Home-page: UNKNOWN Author: LawTech Lab
 Author-email: pranav.bapat@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,extractor,rechtspraak extractor Platform: UNKNOWN Description-
 Content-Type: text/markdown ## Rechtspraak extractor This library contains two
```

### Comparing `rechtspraak_extractor-1.1.7/README.md` & `rechtspraak_extractor-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rechtspraak_extractor-1.1.7/rechtspraak_extractor/rechtspraak.py` & `rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 from datetime import date, datetime
 from rechtspraak_extractor.rechtspraak_functions import *
 
 
 # Define base URL
 RECHTSPRAAK_API_BASE_URL = "https://data.rechtspraak.nl/uitspraken/zoeken?"
 
-rs_ecli_df = []
-rs_title_df = []
-rs_summary_df = []
-rs_updated_df = []
-rs_link_df = []
-
 
 def get_data_from_url(url):
     res = requests.get(url)
     res.raw.decode_content = True
 
     # Convert the XML data to JSON format
     xpars = xmltodict.parse(res.text)
@@ -68,21 +62,15 @@
         # Create directory if not exists
         Path('data').mkdir(parents=True, exist_ok=True)
 
         # Save CSV file
         # file_path = os.path.join('data', file_name + '.csv')
         df.to_csv('data/' + file_name + '.csv', index=False, encoding='utf8')
         print("Data saved to CSV file successfully.")
-    else:
-        rs_ecli_df.extend(ecli_id)
-        rs_title_df.extend(title)
-        rs_summary_df.extend(summary)
-        rs_updated_df.extend(updated)
-        rs_link_df.extend(link)
-
+    return df
 
 def get_rechtspraak(max_ecli=100, sd='2022-08-01', ed=None, save_file='y'):
     print("Rechtspraak dump downloader API")
 
     amount = max_ecli
     starting_date = sd
     save_file = save_file
@@ -116,27 +104,14 @@
             # Build file name
             file_name = 'rechtspraak_' + starting_date + '_' + ending_date + '_' + current_time
 
 
             get_exe_time(start_time)
 
             if save_file == 'n':
-                global rs_ecli_df, rs_title_df, rs_summary_df, rs_updated_df, rs_link_df
-                global_rs_df = pd.DataFrame(columns=['id', 'title', 'summary', 'updated', 'link'])
-                global_rs_df['id'] = rs_ecli_df
-                global_rs_df['title'] = rs_title_df
-                global_rs_df['summary'] = rs_summary_df
-                global_rs_df['updated'] = rs_updated_df
-                global_rs_df['link'] = rs_link_df
-                print("Done")
-                # Clear the lists for the next usage
-                rs_ecli_df = []
-                rs_title_df = []
-                rs_summary_df = []
-                rs_updated_df = []
-                rs_link_df = []
+                global_rs_df = save_csv(json_object, file_name, save_file)
                 return global_rs_df
             else:
                 save_csv(json_object, file_name, save_file)
                 return
     else:
         print(f"URL returned with a {response_code} error code")
```

### Comparing `rechtspraak_extractor-1.1.7/rechtspraak_extractor/rechtspraak_functions.py` & `rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak_functions.py`

 * *Files identical despite different names*

### Comparing `rechtspraak_extractor-1.1.7/rechtspraak_extractor/rechtspraak_metadata.py` & `rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,21 +117,21 @@
                 hasVersion_df.append(hasVersion)
                 del full_text, creator, date_decision, issued, zaaknummer,relations, rs_type,\
                     references, subject,procedure, inhoudsindicatie, hasVersion
 
                 urllib.request.urlcleanup()
 
             except urllib.error.URLError as e:
-                b=2
+                pass
                 #print(e)
             except urllib.error.HTTPError as e:
-                b=2
+                pass
                # print(e)
             except Exception as e:
-                b=2
+                pass
                #print(e)
         else:
             ecli_df.append(ecli_id)
             full_text_df.append("API returned with error code: " + str(response_code))
     except requests.exceptions.RequestException as e:
         raise SystemExit(e)
```

### Comparing `rechtspraak_extractor-1.1.7/rechtspraak_extractor.egg-info/PKG-INFO` & `rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak-extractor
-Version: 1.1.7
+Version: 1.1.8
 Summary: Library for extracting rechtspraak data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: pranav.bapat@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak-extractor Version: 1.1.7 Summary:
+Metadata-Version: 2.1 Name: rechtspraak-extractor Version: 1.1.8 Summary:
 Library for extracting rechtspraak data Home-page: UNKNOWN Author: LawTech Lab
 Author-email: pranav.bapat@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,extractor,rechtspraak extractor Platform: UNKNOWN Description-
 Content-Type: text/markdown ## Rechtspraak extractor This library contains two
```

### Comparing `rechtspraak_extractor-1.1.7/setup.py` & `rechtspraak_extractor-1.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='rechtspraak_extractor',
     packages=find_packages(include=['rechtspraak_extractor']),
-    version='1.1.7',
+    version='1.1.8',
     description='Library for extracting rechtspraak data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4', 'lxml==4.6.3', 'requests==2.26.0', 'xmltodict==0.13.0', 'python_dotenv==0.15.0', 'pandas'],
     author_email='pranav.bapat@student.maastrichtuniversity.nl',
     keywords=['rechtspraak', 'extractor', 'rechtspraak extractor'],
     long_description=long_descr,
```

