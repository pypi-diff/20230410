# Comparing `tmp/cellar_extractor-1.0.44.tar.gz` & `tmp/cellar_extractor-1.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.44.tar", last modified: Fri Mar 24 13:10:19 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.45.tar", last modified: Mon Apr 10 10:38:55 2023, max compression
```

## Comparing `cellar_extractor-1.0.44.tar` & `cellar_extractor-1.0.45.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 13:10:19.181287 cellar_extractor-1.0.44/
--rw-rw-rw-   0        0        0     6377 2023-03-24 13:10:19.180286 cellar_extractor-1.0.44/PKG-INFO
--rw-rw-rw-   0        0        0     5887 2023-02-08 13:05:21.000000 cellar_extractor-1.0.44/README.md
-drwxrwxrwx   0        0        0        0 2023-03-24 13:10:19.168285 cellar_extractor-1.0.44/cellar_extractor/
--rw-rw-rw-   0        0        0      650 2023-03-24 13:06:34.000000 cellar_extractor-1.0.44/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      100 2022-11-04 13:15:55.000000 cellar_extractor-1.0.44/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     2811 2023-02-08 13:50:39.000000 cellar_extractor-1.0.44/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.44/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.44/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11264 2023-01-09 12:41:12.000000 cellar_extractor-1.0.44/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.44/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.44/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6403 2023-03-24 12:49:14.000000 cellar_extractor-1.0.44/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.44/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1558 2023-01-18 16:43:50.000000 cellar_extractor-1.0.44/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.44/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-03-24 13:10:19.178285 cellar_extractor-1.0.44/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     6377 2023-03-24 13:10:19.000000 cellar_extractor-1.0.44/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-03-24 13:10:19.000000 cellar_extractor-1.0.44/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 13:10:19.000000 cellar_extractor-1.0.44/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-03-24 13:10:19.000000 cellar_extractor-1.0.44/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-24 13:10:19.000000 cellar_extractor-1.0.44/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-24 13:10:19.181287 cellar_extractor-1.0.44/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-03-24 13:10:12.000000 cellar_extractor-1.0.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:38:55.842426 cellar_extractor-1.0.45/
+-rw-rw-rw-   0        0        0     7020 2023-04-10 10:38:55.840426 cellar_extractor-1.0.45/PKG-INFO
+-rw-rw-rw-   0        0        0     6530 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 10:38:55.830425 cellar_extractor-1.0.45/cellar_extractor/
+-rw-rw-rw-   0        0        0      704 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      100 2022-11-04 13:15:55.000000 cellar_extractor-1.0.45/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3423 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.45/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.45/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11264 2023-01-09 12:41:12.000000 cellar_extractor-1.0.45/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.45/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.45/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6403 2023-03-24 12:49:14.000000 cellar_extractor-1.0.45/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.45/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1524 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.45/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:38:55.839425 cellar_extractor-1.0.45/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     7020 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 10:38:55.842426 cellar_extractor-1.0.45/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/setup.py
```

### Comparing `cellar_extractor-1.0.44/PKG-INFO` & `cellar_extractor-1.0.45/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: cellar_extractor
-Version: 1.0.44
-Summary: Library for extracting cellar data
-Home-page: UNKNOWN
-Author: LawTech Lab
-Author-email: p.lewandowski@student.maastrichtuniversity.nl
-License: MIT
-Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
-Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
-Keywords: cellar,extractor
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 ## Cellar extractor
 This library contains two functions to get cellar case law data from eurlex.
 
 ## Version
 Python 3.9
 
 ## Contributors
@@ -64,55 +50,64 @@
     Gets all the ECLI data from the eurlex sparql endpoint and saves them in the CSV or JSON format, in-memory or as a saved file.
     <br>
     <li><code>get_cellar_extra</code></li>
     Gets all the ECLI data from the eurlex sparql endpoint, and on top of that scrapes the eurlex websites to acquire 
     the full text, keywords, case law directory code and eurovoc identifiers. If the user does have an eurlex account with access to the eurlex webservices, he can also 
     pass his webservices login credentials to the method, in order to extract data about works citing work and works 
     being cited by work. The full text is returned as a JSON file, rest of data as a CSV.  Can be in-memory or as saved files.
+    <li><code>get_nodes_and_edges_lists</code></li>
+    Gets 2 dataframe objects, one for the nodes and edges of the citations within the passed dataframe.
+    Allows the creation of a network graph of the citations. Can be saved in-memory or in the data folder as csv files.
+    <br>
 </ol>
 
 ## What are the parameters?
 <ol>
     <li><code>get_cellar</code></li>
     <strong>Parameters:</strong>
     <ul>
-        <li><strong>max_ecli: int, optional</strong></li>
-        Maximum number of ECLIs to retrieve
-        <br>Default: 100
+        <li><strong>max_ecli: int, optional, default 100</strong></li>
+        Maximum number of ECLIs to retrieve.
         <li><strong>sd: date, optional, default '2022-05-01'</strong></li>
-        The start last modification date (yyyy-mm-dd)
+        The start last modification date (yyyy-mm-dd).
         <li><strong>ed: date, optional, default current date</strong></li>
-        The end last modification date (yyyy-mm-dd)
+        The end last modification date (yyyy-mm-dd).
         <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
-        Save data in a data folder, or return in-memory
+        Save data in a data folder, or return in-memory.
         <li><strong>file_format: ['csv', 'json'],optional, default 'csv'</strong></li>
         Returns the data as a JSON/dictionary, or as a CSV/Pandas Dataframe object.
     </ul>
     <li><code>get_cellar_extra</code></li>
     <ul> 
-        <li><strong>max_ecli: int, optional</strong></li>
-        Maximum number of ECLIs to retrieve
-        <br>Default: 100
+        <li><strong>max_ecli: int, optional, default 100</strong></li>
+        Maximum number of ECLIs to retrieve.
         <li><strong>sd: date, optional, default '2022-05-01'</strong></li>
-        The start last modification date (yyyy-mm-dd)
+        The start last modification date (yyyy-mm-dd).
         <li><strong>ed: date, optional, default current date</strong></li>
-        The end last modification date (yyyy-mm-dd)
+        The end last modification date (yyyy-mm-dd).
         <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
         Save the full text of cases as JSON file / return as a dictionary and save the rest of
-        the data as a CSV file / return as a Pandas Dataframe object
+        the data as a CSV file / return as a Pandas Dataframe object.
         <li><strong>threads: int ,optional, default 10</strong></li>
         Extracting the additional data takes a lot of time. The use of multi-threading can cut down this time.
         Even with this, the method may take a couple of minutes for a couple of hundred cases. A maximum number
         of 10 recommended, as this method may also affect the device's internet connection.
         <li><strong>username: string, optional, default empty string</strong></li>
         The username to the eurlex webservices.
         <li><strong>password: string, optional, default empty string</strong></li>
         The password to the eurlex webservices.
         <br>
     </ul>
+    <li><code>get_nodes_and_edges_lists</code></li>
+    <ul>
+        <li><strong>df: DataFrame object, required, default None</strong></li>
+        DataFrame of cellar metadata acquired from the get_cellar_extra method.
+        <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
+        Save data in a data folder, or return in-memory.
+    </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
 
@@ -145,9 +140,7 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,9 @@
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.44 Summary: Library
-for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
-p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
-Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
-Build Source, https://github.com/maastrichtlawtech/extraction_libraries
-Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
-markdown ## Cellar extractor This library contains two functions to get cellar
-case law data from eurlex. ## Version Python 3.9 ## Contributors
+## Cellar extractor This library contains two functions to get cellar case law
+data from eurlex. ## Version Python 3.9 ## Contributors
 [pranavnbapat]_    [Cloud956]_    [shashankmc]_ [gijsvd]_
  Pranav_Bapat   Piotr_Lewandowski  shashankmc    gijsvd
  ## How to install? pip install cellar-extractor ## What are the functions?
    1. get_cellar
    2. Gets all the ECLI data from the eurlex sparql endpoint and saves them in
       the CSV or JSON format, in-memory or as a saved file.
    3. get_cellar_extra
@@ -17,51 +11,60 @@
       that scrapes the eurlex websites to acquire the full text, keywords, case
       law directory code and eurovoc identifiers. If the user does have an
       eurlex account with access to the eurlex webservices, he can also pass
       his webservices login credentials to the method, in order to extract data
       about works citing work and works being cited by work. The full text is
       returned as a JSON file, rest of data as a CSV. Can be in-memory or as
       saved files.
+   5. get_nodes_and_edges_lists
+   6. Gets 2 dataframe objects, one for the nodes and edges of the citations
+      within the passed dataframe. Allows the creation of a network graph of
+      the citations. Can be saved in-memory or in the data folder as csv files.
+
 ## What are the parameters?
    1. get_cellar
    2. Parameters:
-          o max_ecli: int, optional
-          o Maximum number of ECLIs to retrieve
-            Default: 100
+          o max_ecli: int, optional, default 100
+          o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
-          o The start last modification date (yyyy-mm-dd)
+          o The start last modification date (yyyy-mm-dd).
           o ed: date, optional, default current date
-          o The end last modification date (yyyy-mm-dd)
+          o The end last modification date (yyyy-mm-dd).
           o save_file: ['y', 'n'],optional, default 'y'
-          o Save data in a data folder, or return in-memory
+          o Save data in a data folder, or return in-memory.
           o file_format: ['csv', 'json'],optional, default 'csv'
           o Returns the data as a JSON/dictionary, or as a CSV/Pandas Dataframe
             object.
    3. get_cellar_extra
-          o max_ecli: int, optional
-          o Maximum number of ECLIs to retrieve
-            Default: 100
+          o max_ecli: int, optional, default 100
+          o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
-          o The start last modification date (yyyy-mm-dd)
+          o The start last modification date (yyyy-mm-dd).
           o ed: date, optional, default current date
-          o The end last modification date (yyyy-mm-dd)
+          o The end last modification date (yyyy-mm-dd).
           o save_file: ['y', 'n'],optional, default 'y'
           o Save the full text of cases as JSON file / return as a dictionary
             and save the rest of the data as a CSV file / return as a Pandas
-            Dataframe object
+            Dataframe object.
           o threads: int ,optional, default 10
           o Extracting the additional data takes a lot of time. The use of
             multi-threading can cut down this time. Even with this, the method
             may take a couple of minutes for a couple of hundred cases. A
             maximum number of 10 recommended, as this method may also affect
             the device's internet connection.
           o username: string, optional, default empty string
           o The username to the eurlex webservices.
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
+   4. get_nodes_and_edges_lists
+          o df: DataFrame object, required, default None
+          o DataFrame of cellar metadata acquired from the get_cellar_extra
+            method.
+          o save_file: ['y', 'n'],optional, default 'y'
+          o Save data in a data folder, or return in-memory.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.44/README.md` & `cellar_extractor-1.0.45/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: cellar_extractor
+Version: 1.0.45
+Summary: Library for extracting cellar data
+Home-page: UNKNOWN
+Author: LawTech Lab
+Author-email: p.lewandowski@student.maastrichtuniversity.nl
+License: MIT
+Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
+Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
+Keywords: cellar,extractor
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 ## Cellar extractor
 This library contains two functions to get cellar case law data from eurlex.
 
 ## Version
 Python 3.9
 
 ## Contributors
@@ -50,55 +64,64 @@
     Gets all the ECLI data from the eurlex sparql endpoint and saves them in the CSV or JSON format, in-memory or as a saved file.
     <br>
     <li><code>get_cellar_extra</code></li>
     Gets all the ECLI data from the eurlex sparql endpoint, and on top of that scrapes the eurlex websites to acquire 
     the full text, keywords, case law directory code and eurovoc identifiers. If the user does have an eurlex account with access to the eurlex webservices, he can also 
     pass his webservices login credentials to the method, in order to extract data about works citing work and works 
     being cited by work. The full text is returned as a JSON file, rest of data as a CSV.  Can be in-memory or as saved files.
+    <li><code>get_nodes_and_edges_lists</code></li>
+    Gets 2 dataframe objects, one for the nodes and edges of the citations within the passed dataframe.
+    Allows the creation of a network graph of the citations. Can be saved in-memory or in the data folder as csv files.
+    <br>
 </ol>
 
 ## What are the parameters?
 <ol>
     <li><code>get_cellar</code></li>
     <strong>Parameters:</strong>
     <ul>
-        <li><strong>max_ecli: int, optional</strong></li>
-        Maximum number of ECLIs to retrieve
-        <br>Default: 100
+        <li><strong>max_ecli: int, optional, default 100</strong></li>
+        Maximum number of ECLIs to retrieve.
         <li><strong>sd: date, optional, default '2022-05-01'</strong></li>
-        The start last modification date (yyyy-mm-dd)
+        The start last modification date (yyyy-mm-dd).
         <li><strong>ed: date, optional, default current date</strong></li>
-        The end last modification date (yyyy-mm-dd)
+        The end last modification date (yyyy-mm-dd).
         <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
-        Save data in a data folder, or return in-memory
+        Save data in a data folder, or return in-memory.
         <li><strong>file_format: ['csv', 'json'],optional, default 'csv'</strong></li>
         Returns the data as a JSON/dictionary, or as a CSV/Pandas Dataframe object.
     </ul>
     <li><code>get_cellar_extra</code></li>
     <ul> 
-        <li><strong>max_ecli: int, optional</strong></li>
-        Maximum number of ECLIs to retrieve
-        <br>Default: 100
+        <li><strong>max_ecli: int, optional, default 100</strong></li>
+        Maximum number of ECLIs to retrieve.
         <li><strong>sd: date, optional, default '2022-05-01'</strong></li>
-        The start last modification date (yyyy-mm-dd)
+        The start last modification date (yyyy-mm-dd).
         <li><strong>ed: date, optional, default current date</strong></li>
-        The end last modification date (yyyy-mm-dd)
+        The end last modification date (yyyy-mm-dd).
         <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
         Save the full text of cases as JSON file / return as a dictionary and save the rest of
-        the data as a CSV file / return as a Pandas Dataframe object
+        the data as a CSV file / return as a Pandas Dataframe object.
         <li><strong>threads: int ,optional, default 10</strong></li>
         Extracting the additional data takes a lot of time. The use of multi-threading can cut down this time.
         Even with this, the method may take a couple of minutes for a couple of hundred cases. A maximum number
         of 10 recommended, as this method may also affect the device's internet connection.
         <li><strong>username: string, optional, default empty string</strong></li>
         The username to the eurlex webservices.
         <li><strong>password: string, optional, default empty string</strong></li>
         The password to the eurlex webservices.
         <br>
     </ul>
+    <li><code>get_nodes_and_edges_lists</code></li>
+    <ul>
+        <li><strong>df: DataFrame object, required, default None</strong></li>
+        DataFrame of cellar metadata acquired from the get_cellar_extra method.
+        <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
+        Save data in a data folder, or return in-memory.
+    </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
 
@@ -131,7 +154,9 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
+
+
```

#### html2text {}

```diff
@@ -1,9 +1,15 @@
-## Cellar extractor This library contains two functions to get cellar case law
-data from eurlex. ## Version Python 3.9 ## Contributors
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.45 Summary: Library
+for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
+p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
+Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
+Build Source, https://github.com/maastrichtlawtech/extraction_libraries
+Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
+markdown ## Cellar extractor This library contains two functions to get cellar
+case law data from eurlex. ## Version Python 3.9 ## Contributors
 [pranavnbapat]_    [Cloud956]_    [shashankmc]_ [gijsvd]_
  Pranav_Bapat   Piotr_Lewandowski  shashankmc    gijsvd
  ## How to install? pip install cellar-extractor ## What are the functions?
    1. get_cellar
    2. Gets all the ECLI data from the eurlex sparql endpoint and saves them in
       the CSV or JSON format, in-memory or as a saved file.
    3. get_cellar_extra
@@ -11,51 +17,60 @@
       that scrapes the eurlex websites to acquire the full text, keywords, case
       law directory code and eurovoc identifiers. If the user does have an
       eurlex account with access to the eurlex webservices, he can also pass
       his webservices login credentials to the method, in order to extract data
       about works citing work and works being cited by work. The full text is
       returned as a JSON file, rest of data as a CSV. Can be in-memory or as
       saved files.
+   5. get_nodes_and_edges_lists
+   6. Gets 2 dataframe objects, one for the nodes and edges of the citations
+      within the passed dataframe. Allows the creation of a network graph of
+      the citations. Can be saved in-memory or in the data folder as csv files.
+
 ## What are the parameters?
    1. get_cellar
    2. Parameters:
-          o max_ecli: int, optional
-          o Maximum number of ECLIs to retrieve
-            Default: 100
+          o max_ecli: int, optional, default 100
+          o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
-          o The start last modification date (yyyy-mm-dd)
+          o The start last modification date (yyyy-mm-dd).
           o ed: date, optional, default current date
-          o The end last modification date (yyyy-mm-dd)
+          o The end last modification date (yyyy-mm-dd).
           o save_file: ['y', 'n'],optional, default 'y'
-          o Save data in a data folder, or return in-memory
+          o Save data in a data folder, or return in-memory.
           o file_format: ['csv', 'json'],optional, default 'csv'
           o Returns the data as a JSON/dictionary, or as a CSV/Pandas Dataframe
             object.
    3. get_cellar_extra
-          o max_ecli: int, optional
-          o Maximum number of ECLIs to retrieve
-            Default: 100
+          o max_ecli: int, optional, default 100
+          o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
-          o The start last modification date (yyyy-mm-dd)
+          o The start last modification date (yyyy-mm-dd).
           o ed: date, optional, default current date
-          o The end last modification date (yyyy-mm-dd)
+          o The end last modification date (yyyy-mm-dd).
           o save_file: ['y', 'n'],optional, default 'y'
           o Save the full text of cases as JSON file / return as a dictionary
             and save the rest of the data as a CSV file / return as a Pandas
-            Dataframe object
+            Dataframe object.
           o threads: int ,optional, default 10
           o Extracting the additional data takes a lot of time. The use of
             multi-threading can cut down this time. Even with this, the method
             may take a couple of minutes for a couple of hundred cases. A
             maximum number of 10 recommended, as this method may also affect
             the device's internet connection.
           o username: string, optional, default empty string
           o The username to the eurlex webservices.
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
+   4. get_nodes_and_edges_lists
+          o df: DataFrame object, required, default None
+          o DataFrame of cellar metadata acquired from the get_cellar_extra
+            method.
+          o save_file: ['y', 'n'],optional, default 'y'
+          o Save data in a data folder, or return in-memory.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.44/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.45/cellar_extractor/Testing_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 
 if __name__ == '__main__':
    celex = "62004CJ0292"
    site = get_entire_page(celex)
    text = get_full_text_from_html(site)
    cits = get_citations_with_extra_info(text)
    print(cits)
-   data = get_cellar_extra(sd='2023-01-01',max_ecli=100,save_file='n')
-   b=2
+   data,d2 = get_cellar_extra(sd='2023-01-01',max_ecli=100,save_file='n')
+   nodes_edges = get_nodes_and_edges_lists(data)
+   pass
```

### Comparing `cellar_extractor-1.0.44/cellar_extractor/cellar.py` & `cellar_extractor-1.0.45/cellar_extractor/cellar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,85 @@
-import json
-import os
-from datetime import datetime
-from pathlib import Path
-from tqdm import tqdm
-from cellar_extractor.cellar_queries import get_all_eclis, get_raw_cellar_metadata
-from cellar_extractor.json_to_csv import json_to_csv_main, json_to_csv_returning
-from cellar_extractor.cellar_extra_extract import extra_cellar
-import time
-
-def get_cellar(ed=None, save_file='y', max_ecli=100, sd="2022-05-01", file_format='csv'):
-    if not ed:
-        ed = datetime.now().isoformat(timespec='seconds')
-    file_name = 'cellar_' + sd + '_' + ed
-    file_name = file_name.replace(":", "_")
-    print('\n--- PREPARATION ---\n')
-    print(f'Starting from specified start date: {sd}')
-    print(f'Up until the specified end date {ed}')
-    eclis = get_all_eclis(starting_date=sd, ending_date=ed)
-    print(f"Found {len(eclis)} ECLIs")
-    time.sleep(1)
-    if len(eclis) > max_ecli:
-        eclis = eclis[:max_ecli]
-    if len(eclis) == 0:
-        print(f"No data to download found between {sd} and {ed}")
-        return False
-    all_eclis = {}
-    concurrent_docs = 100
-    for i in tqdm(range(0, len(eclis), concurrent_docs),colour="GREEN"):
-        new_eclis = get_raw_cellar_metadata(eclis[i:(i + concurrent_docs)])
-        all_eclis = {**all_eclis, **new_eclis}
-    if save_file == 'y':
-        Path('data').mkdir(parents=True, exist_ok=True)
-        if file_format == 'csv':
-            file_path = os.path.join('data', file_name + '.csv')
-            json_to_csv_main(all_eclis, file_path)
-        else:
-            file_path = os.path.join('data', file_name + '.json')
-            with open(file_path, "w") as f:
-                json.dump(all_eclis, f)
-    else:
-        if file_format == 'csv':
-            df = json_to_csv_returning(all_eclis)
-            return df
-        else:
-            return all_eclis
-    print("\n--- DONE ---")
-
-
-def get_cellar_extra(ed=None, save_file='y', max_ecli=100, sd="2022-05-01", threads=10, username="", password=""):
-    if not ed:
-        ed = datetime.now().isoformat(timespec='seconds')
-    data = get_cellar(ed=ed, save_file='n', max_ecli=max_ecli, sd=sd, file_format='csv')
-    if data is False:
-        print("Cellar extraction unsuccessful")
-        return False, False
-    print("\n--- START OF EXTRA EXTRACTION ---")
-    file_name = 'cellar_extra_' + sd + '_' + ed
-    file_name = file_name.replace(":", "_")
-    file_path = os.path.join('data', file_name + '.csv')
-    if save_file == 'y':
-        Path('data').mkdir(parents=True, exist_ok=True)
-        extra_cellar(data = data ,filepath=file_path, threads=threads, username=username, password=password)
-        print("\n--- DONE ---")
-
-    else:
-        data,json = extra_cellar(data= data, threads = threads, username= username,password=password)
-        print("\n--- DONE ---")
-
-        return data,json
+import json
+import os
+from os.path import join
+from datetime import datetime
+from pathlib import Path
+from tqdm import tqdm
+from cellar_extractor.cellar_queries import get_all_eclis, get_raw_cellar_metadata
+from cellar_extractor.json_to_csv import json_to_csv_main, json_to_csv_returning
+from cellar_extractor.cellar_extra_extract import extra_cellar
+from cellar_extractor.nodes_and_edges import get_nodes_and_edges
+import time
+
+def get_cellar(ed=None, save_file='y', max_ecli=100, sd="2022-05-01", file_format='csv'):
+    if not ed:
+        ed = datetime.now().isoformat(timespec='seconds')
+    file_name = 'cellar_' + sd + '_' + ed
+    file_name = file_name.replace(":", "_")
+    print('\n--- PREPARATION ---\n')
+    print(f'Starting from specified start date: {sd}')
+    print(f'Up until the specified end date {ed}')
+    eclis = get_all_eclis(starting_date=sd, ending_date=ed)
+    print(f"Found {len(eclis)} ECLIs")
+    time.sleep(1)
+    if len(eclis) > max_ecli:
+        eclis = eclis[:max_ecli]
+    if len(eclis) == 0:
+        print(f"No data to download found between {sd} and {ed}")
+        return False
+    all_eclis = {}
+    concurrent_docs = 100
+    for i in tqdm(range(0, len(eclis), concurrent_docs),colour="GREEN"):
+        new_eclis = get_raw_cellar_metadata(eclis[i:(i + concurrent_docs)])
+        all_eclis = {**all_eclis, **new_eclis}
+    if save_file == 'y':
+        Path('data').mkdir(parents=True, exist_ok=True)
+        if file_format == 'csv':
+            file_path = os.path.join('data', file_name + '.csv')
+            json_to_csv_main(all_eclis, file_path)
+        else:
+            file_path = os.path.join('data', file_name + '.json')
+            with open(file_path, "w") as f:
+                json.dump(all_eclis, f)
+    else:
+        if file_format == 'csv':
+            df = json_to_csv_returning(all_eclis)
+            return df
+        else:
+            return all_eclis
+    print("\n--- DONE ---")
+
+
+def get_cellar_extra(ed=None, save_file='y', max_ecli=100, sd="2022-05-01", threads=10, username="", password=""):
+    if not ed:
+        ed = datetime.now().isoformat(timespec='seconds')
+    data = get_cellar(ed=ed, save_file='n', max_ecli=max_ecli, sd=sd, file_format='csv')
+    if data is False:
+        print("Cellar extraction unsuccessful")
+        return False, False
+    print("\n--- START OF EXTRA EXTRACTION ---")
+    file_name = 'cellar_extra_' + sd + '_' + ed
+    file_name = file_name.replace(":", "_")
+    file_path = os.path.join('data', file_name + '.csv')
+    if save_file == 'y':
+        Path('data').mkdir(parents=True, exist_ok=True)
+        extra_cellar(data = data ,filepath=file_path, threads=threads, username=username, password=password)
+        print("\n--- DONE ---")
+
+    else:
+        data,json = extra_cellar(data= data, threads = threads, username= username,password=password)
+        print("\n--- DONE ---")
+
+        return data,json
+
+def get_nodes_and_edges_lists(df = None,save_file='y'):
+    if df is None:
+        print("No dataframe passed!")
+        return
+    else:
+        nodes,edges = get_nodes_and_edges(df)
+        if save_file == 'y':
+            Path('data').mkdir(parents=True, exist_ok=True)
+            nodes.to_csv(join('data','nodes'),index=False)
+            edges.to_csv(join('data','edges'),index=False)
+        else:
+            return nodes,edges
```

### Comparing `cellar_extractor-1.0.44/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.45/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.44/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.45/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.44/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.45/cellar_extractor/citations_adder.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.44/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.45/cellar_extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.44/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.45/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.44/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.45/cellar_extractor/fulltext_saving.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.44/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.45/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.44/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.45/cellar_extractor/nodes_and_edges.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
              'Target' :  t_list
              }
     for i in range(len(keys)):
         k = keys[i]
         val = vals[i]
         if val == val:
             val_unpacked = val.split(";")
-            final_val = [i for i in val_unpacked if i.startswith("6")]
+            final_val = val_unpacked
             if len(final_val) == 0:
                 s_list.append(k)
                 all_celexes.add(k)
                 t_list.append("")
             else:
                 for val in final_val:
                     s_list.append(k)
```

### Comparing `cellar_extractor-1.0.44/cellar_extractor/sparql.py` & `cellar_extractor-1.0.45/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.44/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.45/cellar_extractor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar-extractor
-Version: 1.0.44
+Version: 1.0.45
 Summary: Library for extracting cellar data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
@@ -64,55 +64,64 @@
     Gets all the ECLI data from the eurlex sparql endpoint and saves them in the CSV or JSON format, in-memory or as a saved file.
     <br>
     <li><code>get_cellar_extra</code></li>
     Gets all the ECLI data from the eurlex sparql endpoint, and on top of that scrapes the eurlex websites to acquire 
     the full text, keywords, case law directory code and eurovoc identifiers. If the user does have an eurlex account with access to the eurlex webservices, he can also 
     pass his webservices login credentials to the method, in order to extract data about works citing work and works 
     being cited by work. The full text is returned as a JSON file, rest of data as a CSV.  Can be in-memory or as saved files.
+    <li><code>get_nodes_and_edges_lists</code></li>
+    Gets 2 dataframe objects, one for the nodes and edges of the citations within the passed dataframe.
+    Allows the creation of a network graph of the citations. Can be saved in-memory or in the data folder as csv files.
+    <br>
 </ol>
 
 ## What are the parameters?
 <ol>
     <li><code>get_cellar</code></li>
     <strong>Parameters:</strong>
     <ul>
-        <li><strong>max_ecli: int, optional</strong></li>
-        Maximum number of ECLIs to retrieve
-        <br>Default: 100
+        <li><strong>max_ecli: int, optional, default 100</strong></li>
+        Maximum number of ECLIs to retrieve.
         <li><strong>sd: date, optional, default '2022-05-01'</strong></li>
-        The start last modification date (yyyy-mm-dd)
+        The start last modification date (yyyy-mm-dd).
         <li><strong>ed: date, optional, default current date</strong></li>
-        The end last modification date (yyyy-mm-dd)
+        The end last modification date (yyyy-mm-dd).
         <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
-        Save data in a data folder, or return in-memory
+        Save data in a data folder, or return in-memory.
         <li><strong>file_format: ['csv', 'json'],optional, default 'csv'</strong></li>
         Returns the data as a JSON/dictionary, or as a CSV/Pandas Dataframe object.
     </ul>
     <li><code>get_cellar_extra</code></li>
     <ul> 
-        <li><strong>max_ecli: int, optional</strong></li>
-        Maximum number of ECLIs to retrieve
-        <br>Default: 100
+        <li><strong>max_ecli: int, optional, default 100</strong></li>
+        Maximum number of ECLIs to retrieve.
         <li><strong>sd: date, optional, default '2022-05-01'</strong></li>
-        The start last modification date (yyyy-mm-dd)
+        The start last modification date (yyyy-mm-dd).
         <li><strong>ed: date, optional, default current date</strong></li>
-        The end last modification date (yyyy-mm-dd)
+        The end last modification date (yyyy-mm-dd).
         <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
         Save the full text of cases as JSON file / return as a dictionary and save the rest of
-        the data as a CSV file / return as a Pandas Dataframe object
+        the data as a CSV file / return as a Pandas Dataframe object.
         <li><strong>threads: int ,optional, default 10</strong></li>
         Extracting the additional data takes a lot of time. The use of multi-threading can cut down this time.
         Even with this, the method may take a couple of minutes for a couple of hundred cases. A maximum number
         of 10 recommended, as this method may also affect the device's internet connection.
         <li><strong>username: string, optional, default empty string</strong></li>
         The username to the eurlex webservices.
         <li><strong>password: string, optional, default empty string</strong></li>
         The password to the eurlex webservices.
         <br>
     </ul>
+    <li><code>get_nodes_and_edges_lists</code></li>
+    <ul>
+        <li><strong>df: DataFrame object, required, default None</strong></li>
+        DataFrame of cellar metadata acquired from the get_cellar_extra method.
+        <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
+        Save data in a data folder, or return in-memory.
+    </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.44 Summary: Library
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.45 Summary: Library
 for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
 markdown ## Cellar extractor This library contains two functions to get cellar
 case law data from eurlex. ## Version Python 3.9 ## Contributors
@@ -17,51 +17,60 @@
       that scrapes the eurlex websites to acquire the full text, keywords, case
       law directory code and eurovoc identifiers. If the user does have an
       eurlex account with access to the eurlex webservices, he can also pass
       his webservices login credentials to the method, in order to extract data
       about works citing work and works being cited by work. The full text is
       returned as a JSON file, rest of data as a CSV. Can be in-memory or as
       saved files.
+   5. get_nodes_and_edges_lists
+   6. Gets 2 dataframe objects, one for the nodes and edges of the citations
+      within the passed dataframe. Allows the creation of a network graph of
+      the citations. Can be saved in-memory or in the data folder as csv files.
+
 ## What are the parameters?
    1. get_cellar
    2. Parameters:
-          o max_ecli: int, optional
-          o Maximum number of ECLIs to retrieve
-            Default: 100
+          o max_ecli: int, optional, default 100
+          o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
-          o The start last modification date (yyyy-mm-dd)
+          o The start last modification date (yyyy-mm-dd).
           o ed: date, optional, default current date
-          o The end last modification date (yyyy-mm-dd)
+          o The end last modification date (yyyy-mm-dd).
           o save_file: ['y', 'n'],optional, default 'y'
-          o Save data in a data folder, or return in-memory
+          o Save data in a data folder, or return in-memory.
           o file_format: ['csv', 'json'],optional, default 'csv'
           o Returns the data as a JSON/dictionary, or as a CSV/Pandas Dataframe
             object.
    3. get_cellar_extra
-          o max_ecli: int, optional
-          o Maximum number of ECLIs to retrieve
-            Default: 100
+          o max_ecli: int, optional, default 100
+          o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
-          o The start last modification date (yyyy-mm-dd)
+          o The start last modification date (yyyy-mm-dd).
           o ed: date, optional, default current date
-          o The end last modification date (yyyy-mm-dd)
+          o The end last modification date (yyyy-mm-dd).
           o save_file: ['y', 'n'],optional, default 'y'
           o Save the full text of cases as JSON file / return as a dictionary
             and save the rest of the data as a CSV file / return as a Pandas
-            Dataframe object
+            Dataframe object.
           o threads: int ,optional, default 10
           o Extracting the additional data takes a lot of time. The use of
             multi-threading can cut down this time. Even with this, the method
             may take a couple of minutes for a couple of hundred cases. A
             maximum number of 10 recommended, as this method may also affect
             the device's internet connection.
           o username: string, optional, default empty string
           o The username to the eurlex webservices.
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
+   4. get_nodes_and_edges_lists
+          o df: DataFrame object, required, default None
+          o DataFrame of cellar metadata acquired from the get_cellar_extra
+            method.
+          o save_file: ['y', 'n'],optional, default 'y'
+          o Save data in a data folder, or return in-memory.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.44/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.45/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.44/setup.py` & `cellar_extractor-1.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.44',
+    version='1.0.45',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

