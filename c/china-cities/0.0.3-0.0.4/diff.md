# Comparing `tmp/china_cities-0.0.3.tar.gz` & `tmp/china_cities-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/china_cities-0.0.3.tar", last modified: Thu Nov 28 03:56:23 2019, max compression
+gzip compressed data, was "china_cities-0.0.4.tar", last modified: Mon Apr 10 11:09:56 2023, max compression
```

## Comparing `china_cities-0.0.3.tar` & `china_cities-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 vanbos   (215453377) 1437522721        0 2019-11-28 03:56:23.000000 china_cities-0.0.3/
--rw-r--r--   0 vanbos   (215453377) 1437522721       41 2019-11-28 01:52:50.000000 china_cities-0.0.3/MANIFEST.in
--rw-r--r--   0 vanbos   (215453377) 1437522721     2326 2019-11-28 03:56:23.000000 china_cities-0.0.3/PKG-INFO
--rw-r--r--   0 vanbos   (215453377) 1437522721     1077 2019-11-28 01:52:50.000000 china_cities-0.0.3/README.md
-drwxr-xr-x   0 vanbos   (215453377) 1437522721        0 2019-11-28 03:56:23.000000 china_cities-0.0.3/china_cities/
--rw-r--r--   0 vanbos   (215453377) 1437522721      286 2019-11-28 03:55:50.000000 china_cities-0.0.3/china_cities/__init__.py
--rw-r--r--   0 vanbos   (215453377) 1437522721    17849 2019-11-28 03:53:43.000000 china_cities-0.0.3/china_cities/cities.csv
--rw-r--r--   0 vanbos   (215453377) 1437522721     1677 2019-11-28 03:55:00.000000 china_cities-0.0.3/china_cities/cities.py
-drwxr-xr-x   0 vanbos   (215453377) 1437522721        0 2019-11-28 03:56:23.000000 china_cities-0.0.3/china_cities.egg-info/
--rw-r--r--   0 vanbos   (215453377) 1437522721     2326 2019-11-28 03:56:22.000000 china_cities-0.0.3/china_cities.egg-info/PKG-INFO
--rw-r--r--   0 vanbos   (215453377) 1437522721      291 2019-11-28 03:56:22.000000 china_cities-0.0.3/china_cities.egg-info/SOURCES.txt
--rw-r--r--   0 vanbos   (215453377) 1437522721        1 2019-11-28 03:56:22.000000 china_cities-0.0.3/china_cities.egg-info/dependency_links.txt
--rw-r--r--   0 vanbos   (215453377) 1437522721        1 2019-11-28 03:56:22.000000 china_cities-0.0.3/china_cities.egg-info/not-zip-safe
--rw-r--r--   0 vanbos   (215453377) 1437522721       13 2019-11-28 03:56:22.000000 china_cities-0.0.3/china_cities.egg-info/top_level.txt
--rw-r--r--   0 vanbos   (215453377) 1437522721       67 2019-11-28 03:56:23.000000 china_cities-0.0.3/setup.cfg
--rw-r--r--   0 vanbos   (215453377) 1437522721     1355 2019-11-28 01:52:50.000000 china_cities-0.0.3/setup.py
+drwxrwxr-x   0 boeboe    (1000) boeboe    (1000)        0 2023-04-10 11:09:56.417755 china_cities-0.0.4/
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)     1069 2023-04-10 10:47:24.000000 china_cities-0.0.4/LICENSE
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)       41 2023-04-10 10:47:24.000000 china_cities-0.0.4/MANIFEST.in
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)     1837 2023-04-10 11:09:56.417755 china_cities-0.0.4/PKG-INFO
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)     1077 2023-04-10 10:47:24.000000 china_cities-0.0.4/README.md
+drwxrwxr-x   0 boeboe    (1000) boeboe    (1000)        0 2023-04-10 11:09:56.417755 china_cities-0.0.4/china_cities/
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)      286 2023-04-10 11:09:38.000000 china_cities-0.0.4/china_cities/__init__.py
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)    17849 2023-04-10 10:47:24.000000 china_cities-0.0.4/china_cities/cities.csv
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)     1695 2023-04-10 11:03:15.000000 china_cities-0.0.4/china_cities/cities.py
+drwxrwxr-x   0 boeboe    (1000) boeboe    (1000)        0 2023-04-10 11:09:56.417755 china_cities-0.0.4/china_cities.egg-info/
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)     1837 2023-04-10 11:09:56.000000 china_cities-0.0.4/china_cities.egg-info/PKG-INFO
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)      320 2023-04-10 11:09:56.000000 china_cities-0.0.4/china_cities.egg-info/SOURCES.txt
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)        1 2023-04-10 11:09:56.000000 china_cities-0.0.4/china_cities.egg-info/dependency_links.txt
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)        1 2023-04-10 11:09:54.000000 china_cities-0.0.4/china_cities.egg-info/not-zip-safe
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)       13 2023-04-10 11:09:56.000000 china_cities-0.0.4/china_cities.egg-info/top_level.txt
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)       67 2023-04-10 11:09:56.421755 china_cities-0.0.4/setup.cfg
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)     1296 2023-04-10 11:08:57.000000 china_cities-0.0.4/setup.py
+drwxrwxr-x   0 boeboe    (1000) boeboe    (1000)        0 2023-04-10 11:09:56.417755 china_cities-0.0.4/tests/
+-rw-rw-r--   0 boeboe    (1000) boeboe    (1000)     1954 2023-04-10 10:47:24.000000 china_cities-0.0.4/tests/test_cities.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `china_cities-0.0.3/PKG-INFO` & `china_cities-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: china_cities
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package to get the names of Chinese cities and provinces
 Home-page: https://github.com/boeboe/china-cities
 Author: Bart Van Bos
 Author-email: bartvanbos@gmail.com
 License: MIT
-Description: # china_cities
-        
-        ## Introduction
-        
-        `china_cities` is a python package to list Chinese cities and provinces. The cities 
-        can be retrieved in English or Chinese language.
-        
-        The data is based on [`wikipedia`](https://en.wikipedia.org/wiki/List_of_cities_in_China) as a source
-        
-        ## Installation
-        
-        ### Install with pip
-        
-        Run `pip install china-cities`
-        
-        ### Install from source
-        
-        `git clone https://github.com/boeboe/china-cities.git`
-        
-        Run `python setup.py install`
-        
-        ### Run tests
-        
-        Run `make tests`
-        
-        ### Update source when wikipedia changed
-        
-        Run `make generate`
-        
-        ## Usage
-        
-        Some examples on how to use this package.
-        
-        ```python
-        from china_cities import *
-        
-        for city in cities.get_cities():
-            print("english name:", city.name_en)
-            print("chinese name:", city.name_cn)
-            print("province:    ", city.province)
-        
-        for city_en in cities.get_cities_en():
-            print(city_en)
-        
-        for city_cn in cities.get_cities_cn():
-            print(city_cn)
-        
-        for province in cities.get_provinces():
-            print(province)
-        
-        for province_city in cities.get_cities_by_province("Anhui"):
-            print(province_city.name_en)
-        
-        ```
-        
 Keywords: china chinese cities provinces
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Software Distribution
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# china_cities
+
+## Introduction
+
+`china_cities` is a python package to list Chinese cities and provinces. The cities 
+can be retrieved in English or Chinese language.
+
+The data is based on [`wikipedia`](https://en.wikipedia.org/wiki/List_of_cities_in_China) as a source
+
+## Installation
+
+### Install with pip
+
+Run `pip install china-cities`
+
+### Install from source
+
+`git clone https://github.com/boeboe/china-cities.git`
+
+Run `python setup.py install`
+
+### Run tests
+
+Run `make tests`
+
+### Update source when wikipedia changed
+
+Run `make generate`
+
+## Usage
+
+Some examples on how to use this package.
+
+```python
+from china_cities import *
+
+for city in cities.get_cities():
+    print("english name:", city.name_en)
+    print("chinese name:", city.name_cn)
+    print("province:    ", city.province)
+
+for city_en in cities.get_cities_en():
+    print(city_en)
+
+for city_cn in cities.get_cities_cn():
+    print(city_cn)
+
+for province in cities.get_provinces():
+    print(province)
+
+for province_city in cities.get_cities_by_province("Anhui"):
+    print(province_city.name_en)
+
+```
```

### Comparing `china_cities-0.0.3/README.md` & `china_cities-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `china_cities-0.0.3/china_cities/cities.csv` & `china_cities-0.0.4/china_cities/cities.csv`

 * *Files identical despite different names*

### Comparing `china_cities-0.0.3/china_cities/cities.py` & `china_cities-0.0.4/china_cities/cities.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return str(self.__class__) + ": " + str(self.__dict__)
 
     def __repr__(self):
         return str(self.__class__) + ": " + str(self.__dict__)
 
 CITIES = []
 
-with open(os.path.join(__location__, 'cities.csv')) as fileHandler:
+with open(os.path.join(__location__, 'cities.csv'), encoding='utf-8') as fileHandler:
     for line in fileHandler:
         split = line.strip().split(",")
         CITIES.append(City(name_en=split[0], name_cn=split[1], province=split[2]))
 
 def get_cities():
     """Return a list of all Chinese Cities (City objects) """
     return CITIES
```

### Comparing `china_cities-0.0.3/china_cities.egg-info/PKG-INFO` & `china_cities-0.0.4/china_cities.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: china-cities
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package to get the names of Chinese cities and provinces
 Home-page: https://github.com/boeboe/china-cities
 Author: Bart Van Bos
 Author-email: bartvanbos@gmail.com
 License: MIT
-Description: # china_cities
-        
-        ## Introduction
-        
-        `china_cities` is a python package to list Chinese cities and provinces. The cities 
-        can be retrieved in English or Chinese language.
-        
-        The data is based on [`wikipedia`](https://en.wikipedia.org/wiki/List_of_cities_in_China) as a source
-        
-        ## Installation
-        
-        ### Install with pip
-        
-        Run `pip install china-cities`
-        
-        ### Install from source
-        
-        `git clone https://github.com/boeboe/china-cities.git`
-        
-        Run `python setup.py install`
-        
-        ### Run tests
-        
-        Run `make tests`
-        
-        ### Update source when wikipedia changed
-        
-        Run `make generate`
-        
-        ## Usage
-        
-        Some examples on how to use this package.
-        
-        ```python
-        from china_cities import *
-        
-        for city in cities.get_cities():
-            print("english name:", city.name_en)
-            print("chinese name:", city.name_cn)
-            print("province:    ", city.province)
-        
-        for city_en in cities.get_cities_en():
-            print(city_en)
-        
-        for city_cn in cities.get_cities_cn():
-            print(city_cn)
-        
-        for province in cities.get_provinces():
-            print(province)
-        
-        for province_city in cities.get_cities_by_province("Anhui"):
-            print(province_city.name_en)
-        
-        ```
-        
 Keywords: china chinese cities provinces
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Software Distribution
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# china_cities
+
+## Introduction
+
+`china_cities` is a python package to list Chinese cities and provinces. The cities 
+can be retrieved in English or Chinese language.
+
+The data is based on [`wikipedia`](https://en.wikipedia.org/wiki/List_of_cities_in_China) as a source
+
+## Installation
+
+### Install with pip
+
+Run `pip install china-cities`
+
+### Install from source
+
+`git clone https://github.com/boeboe/china-cities.git`
+
+Run `python setup.py install`
+
+### Run tests
+
+Run `make tests`
+
+### Update source when wikipedia changed
+
+Run `make generate`
+
+## Usage
+
+Some examples on how to use this package.
+
+```python
+from china_cities import *
+
+for city in cities.get_cities():
+    print("english name:", city.name_en)
+    print("chinese name:", city.name_cn)
+    print("province:    ", city.province)
+
+for city_en in cities.get_cities_en():
+    print(city_en)
+
+for city_cn in cities.get_cities_cn():
+    print(city_cn)
+
+for province in cities.get_provinces():
+    print(province)
+
+for province_city in cities.get_cities_by_province("Anhui"):
+    print(province_city.name_en)
+
+```
```

### Comparing `china_cities-0.0.3/setup.py` & `china_cities-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
       zip_safe=False,
       classifiers=[
                     'Development Status :: 5 - Production/Stable',
                     'Intended Audience :: Developers',
                     'Natural Language :: English',
                     'License :: OSI Approved :: MIT License',
                     'Programming Language :: Python',
-                    'Programming Language :: Python :: 2',
                     'Programming Language :: Python :: 3',
                     "Topic :: Software Development :: Libraries :: Python Modules",
                     "Topic :: System :: Software Distribution"
       ],
       test_suite='tests',
       tests_require=['unittest']
       )
```

