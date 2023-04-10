# Comparing `tmp/fairmaterials-0.3.0.tar.gz` & `tmp/fairmaterials-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fairmaterials-0.3.0.tar", last modified: Fri Feb 10 18:18:48 2023, max compression
+gzip compressed data, was "dist/fairmaterials-0.4.0.tar", last modified: Mon Apr 10 19:04:38 2023, max compression
```

## Comparing `fairmaterials-0.3.0.tar` & `fairmaterials-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nice.j     (501) staff       (20)        0 2023-02-10 18:18:48.000000 fairmaterials-0.3.0/
--rw-r--r--   0 nice.j     (501) staff       (20)     4474 2023-02-10 18:18:48.000000 fairmaterials-0.3.0/PKG-INFO
-drwxr-xr-x   0 nice.j     (501) staff       (20)        0 2023-02-10 18:18:48.000000 fairmaterials-0.3.0/fairmaterials/
--rw-r--r--   0 nice.j     (501) staff       (20)        0 2022-12-08 11:02:28.000000 fairmaterials-0.3.0/fairmaterials/__init__.py
--rw-r--r--   0 nice.j     (501) staff       (20)    28083 2023-02-10 17:40:43.000000 fairmaterials-0.3.0/fairmaterials/fairify_data.py
-drwxr-xr-x   0 nice.j     (501) staff       (20)        0 2023-02-10 18:18:48.000000 fairmaterials-0.3.0/fairmaterials.egg-info/
--rw-r--r--   0 nice.j     (501) staff       (20)     4474 2023-02-10 18:18:48.000000 fairmaterials-0.3.0/fairmaterials.egg-info/PKG-INFO
--rw-r--r--   0 nice.j     (501) staff       (20)      234 2023-02-10 18:18:48.000000 fairmaterials-0.3.0/fairmaterials.egg-info/SOURCES.txt
--rw-r--r--   0 nice.j     (501) staff       (20)       14 2023-02-10 18:18:48.000000 fairmaterials-0.3.0/fairmaterials.egg-info/top_level.txt
--rw-r--r--   0 nice.j     (501) staff       (20)        1 2023-02-10 18:18:48.000000 fairmaterials-0.3.0/fairmaterials.egg-info/dependency_links.txt
--rw-r--r--   0 nice.j     (501) staff       (20)     3034 2023-02-10 18:11:11.000000 fairmaterials-0.3.0/README.md
--rw-r--r--   0 nice.j     (501) staff       (20)     1925 2023-02-10 18:11:37.000000 fairmaterials-0.3.0/setup.py
--rw-r--r--   0 nice.j     (501) staff       (20)       38 2023-02-10 18:18:48.000000 fairmaterials-0.3.0/setup.cfg
--rw-r--r--   0 nice.j     (501) staff       (20)     1520 2022-12-10 05:08:09.000000 fairmaterials-0.3.0/LICENSE.txt
+drwxr-xr-x   0 nice.j     (501) staff       (20)        0 2023-04-10 19:04:38.000000 fairmaterials-0.4.0/
+-rw-r--r--   0 nice.j     (501) staff       (20)     5559 2023-04-10 19:04:38.000000 fairmaterials-0.4.0/PKG-INFO
+drwxr-xr-x   0 nice.j     (501) staff       (20)        0 2023-04-10 19:04:38.000000 fairmaterials-0.4.0/fairmaterials/
+-rw-r--r--   0 nice.j     (501) staff       (20)        0 2022-12-08 11:02:28.000000 fairmaterials-0.4.0/fairmaterials/__init__.py
+-rw-r--r--   0 nice.j     (501) staff       (20)    11710 2023-04-10 18:38:14.000000 fairmaterials-0.4.0/fairmaterials/fairify_data.py
+drwxr-xr-x   0 nice.j     (501) staff       (20)        0 2023-04-10 19:04:38.000000 fairmaterials-0.4.0/fairmaterials.egg-info/
+-rw-r--r--   0 nice.j     (501) staff       (20)     5559 2023-04-10 19:04:37.000000 fairmaterials-0.4.0/fairmaterials.egg-info/PKG-INFO
+-rw-r--r--   0 nice.j     (501) staff       (20)      234 2023-04-10 19:04:37.000000 fairmaterials-0.4.0/fairmaterials.egg-info/SOURCES.txt
+-rw-r--r--   0 nice.j     (501) staff       (20)       14 2023-04-10 19:04:37.000000 fairmaterials-0.4.0/fairmaterials.egg-info/top_level.txt
+-rw-r--r--   0 nice.j     (501) staff       (20)        1 2023-04-10 19:04:37.000000 fairmaterials-0.4.0/fairmaterials.egg-info/dependency_links.txt
+-rw-r--r--   0 nice.j     (501) staff       (20)     4157 2023-04-10 18:54:26.000000 fairmaterials-0.4.0/README.md
+-rw-r--r--   0 nice.j     (501) staff       (20)     1888 2023-04-10 18:58:50.000000 fairmaterials-0.4.0/setup.py
+-rw-r--r--   0 nice.j     (501) staff       (20)       38 2023-04-10 19:04:38.000000 fairmaterials-0.4.0/setup.cfg
+-rw-r--r--   0 nice.j     (501) staff       (20)     1520 2022-12-10 05:08:09.000000 fairmaterials-0.4.0/LICENSE.txt
```

### Comparing `fairmaterials-0.3.0/PKG-INFO` & `fairmaterials-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: fairmaterials
-Version: 0.3.0
-Summary: Generate  JSON-LD format file based on FAIRification standard
+Version: 0.4.0
+Summary: Make Materials Data FAIR
 Home-page: UNKNOWN
-Author: Mingjian Lu,Liangyi Huang, Will Oltjen,Xuanji Yu,Arafath Nihar, Tommy Ciardi, Erika Barcelos,Pawan Tripathi,Abhishek Daundkar,Deepa Bhuvanagiri,Hope Omodolor,Hein Htet Aung,Kristen Hernandez,Mirra Rasmussen,Raymond Wieser, Sameera Nalin Venkat,Tian Wang, Weiqi Yue, Yangxin Fan,Rounak Chawla,Leean Jo,Olatunde Akanbi,Zelin Li,Jiqi Liu, Justin Glynn, Kehley Coleman,Jeffery Yarus, Mengjie Li,Kristopher.Davis, Laura Bruckman,Yinghui Wu,Roger French
-Author-email: mxl1171@case.edu,lxh442@case.edu, wco3@case.edu,xxy530@case.edu ,arafath@case.edu,tgc17@case.edu,eib14@case.edu,pkt19@case.edu,aad157@case.edu,dcb117@case.edu,hxo76@case.edu,hxh483@case.edu,kjh125@case.edu,mmr125@case.edu,rxw497@case.edu,sxn440@case.edu,txw387@case.edu,wxy215@case.edu,yxf451@case.edu,rxc542@case.edu,yxj414@case.edu,oda10@case.edu,zxl1080@case.edu,jxl1763@case.edu,jpg90@case.edu,kac196@case.edu,jmy41@case.edu,Mengjie.Li@ucf.edu,Kristopher.Davis@ucf.edu,lsh41@case.edu,yxw1650@case.edu,rxf131@case.edu
+Author: Mingjian Lu, Will Oltjen,Xuanji Yu,Liangyi Huang,Arafath Nihar, Tommy Ciardi, Erika Barcelos,Pawan Tripathi,Abhishek Daundkar,Deepa Bhuvanagiri,Hope Omodolor,Hein Htet Aung,Kristen Hernandez,Mirra Rasmussen,Raymond Wieser, Sameera Nalin Venkat,Tian Wang, Weiqi Yue, Yangxin Fan,Rounak Chawla,Leean Jo,Olatunde Akanbi,Zelin Li,Jiqi Liu, Justin Glynn, Kehley Coleman,Jeffery Yarus, Mengjie Li,Kristopher.Davis, Laura Bruckman,Yinghui Wu,Roger French
+Author-email: mxl1171@case.edu,wco3@case.edu,xxy530@case.edu ,lxh442@case.edu,arafath@case.edu,tgc17@case.edu,eib14@case.edu,pkt19@case.edu,aad157@case.edu,dcb117@case.edu,hxo76@case.edu,hxh483@case.edu,kjh125@case.edu,mmr125@case.edu,rxw497@case.edu,sxn440@case.edu,txw387@case.edu,wxy215@case.edu,yxf451@case.edu,rxc542@case.edu,yxj414@case.edu,oda10@case.edu,zxl1080@case.edu,jxl1763@case.edu,jpg90@case.edu,kac196@case.edu,jmy41@case.edu,Mengjie.Li@ucf.edu,Kristopher.Davis@ucf.edu,lsh41@case.edu,yxw1650@case.edu,rxf131@case.edu
 License: BSD License (BSD-3)
 Project-URL: HomePage, https://cwrusdle.bitbucket.io
 Project-URL: Documentation, https://cwrusdle.bitbucket.io/fairmaterials-py/index.html
 Keywords: FAIRification,PowerPlant,Engineering
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 ![logo](https://i.imgur.com/pqR2OBe.png)
 
 # Fairmaterials
 Fairmaterials is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland OH.
-Fairmaterials is a tool for fairing data. It reads a template JSON-LD file to get the preset data. The user can edit the data by manually inputting or by importing a csv file or dataframe. The output will be a sequence of JSON-LD files with the fairified data inside. 
-
+We provide here tools used by the Solar Durability and Lifetime Extension Center (SDLE) for FAIRifying data from materials science projects. Functions have been created for numerous tools common in the field in order to make the metadata more Findable, Accessible, Interoperable, and Reproducible.
 
 # Features
  -  Importing JSON template as JSON-LD.
  -   Modify JSON data.
 		- Based on CSV file.
 		- Based on dataframe file
  -   Output fairiried data as standard JSON-LD format file.
@@ -42,14 +41,55 @@
 ```python
 fairify_data(dataframe,"polymerAdditiveManufacturing")
 ``` 
 ***Output will be series of json-ld format file***
 
 #  Versions
 All notable changes to this project will be documented in this file.
+## [0.4.0] - 2023-04-10
+### Added
+- Expand the domain to 33 
+- Rename domain names
+- Fairify data from different domains,data from different domains inside one dataframe(or CSV)can be fairify to different JSON-LD output according to the JSON-LD template. 
+- Add synonym function which can fairify data according to the synonym inside JSON-LD template  
+#### Domains
+-opticalProfilometry
+-streamWater
+-opticalSpectroscopy
+-metalAdditiveManufacturing
+-environmentalExposure
+-photovoltaicModule
+-asterGdem
+-sample-metadata
+-photovoltaicInverter
+-caryUvVis-instrument-metadata
+-capillaryEletrophoresis-Measurement-metadata
+-waterMetaDataUSGS
+-spectramaxUvVis-results
+-spectramaxUvVis-instrument-metadata
+-photovoltaicCell
+-soilWoSis
+-currentVoltage
+-computedTomographyXRay
+-photovoltaicSystem
+-soil
+-diffractionXRay
+-polymerFormulation
+-photovoltaicBacksheet
+-gasFlux
+-caryUvVis-results
+-caryUvVis-measurement-metadata
+-polymerAdditiveManufacturing
+-spectramaxUvVis-measurement-metadata
+-materials-processing
+-geospatialWell
+-buildings
+-capillaryElectrophoresis-calibration-results
+-waterDataUSGS'
+
 ## [0.3.0] - 2023-02-10
 ### Added
 - Expand the domain to 20 
 - Rename domain names 
 #### Domains
 - diffractionXRay
 - capillaryElectrophoresis
```

### Comparing `fairmaterials-0.3.0/fairmaterials.egg-info/PKG-INFO` & `fairmaterials-0.4.0/fairmaterials.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: fairmaterials
-Version: 0.3.0
-Summary: Generate  JSON-LD format file based on FAIRification standard
+Version: 0.4.0
+Summary: Make Materials Data FAIR
 Home-page: UNKNOWN
-Author: Mingjian Lu,Liangyi Huang, Will Oltjen,Xuanji Yu,Arafath Nihar, Tommy Ciardi, Erika Barcelos,Pawan Tripathi,Abhishek Daundkar,Deepa Bhuvanagiri,Hope Omodolor,Hein Htet Aung,Kristen Hernandez,Mirra Rasmussen,Raymond Wieser, Sameera Nalin Venkat,Tian Wang, Weiqi Yue, Yangxin Fan,Rounak Chawla,Leean Jo,Olatunde Akanbi,Zelin Li,Jiqi Liu, Justin Glynn, Kehley Coleman,Jeffery Yarus, Mengjie Li,Kristopher.Davis, Laura Bruckman,Yinghui Wu,Roger French
-Author-email: mxl1171@case.edu,lxh442@case.edu, wco3@case.edu,xxy530@case.edu ,arafath@case.edu,tgc17@case.edu,eib14@case.edu,pkt19@case.edu,aad157@case.edu,dcb117@case.edu,hxo76@case.edu,hxh483@case.edu,kjh125@case.edu,mmr125@case.edu,rxw497@case.edu,sxn440@case.edu,txw387@case.edu,wxy215@case.edu,yxf451@case.edu,rxc542@case.edu,yxj414@case.edu,oda10@case.edu,zxl1080@case.edu,jxl1763@case.edu,jpg90@case.edu,kac196@case.edu,jmy41@case.edu,Mengjie.Li@ucf.edu,Kristopher.Davis@ucf.edu,lsh41@case.edu,yxw1650@case.edu,rxf131@case.edu
+Author: Mingjian Lu, Will Oltjen,Xuanji Yu,Liangyi Huang,Arafath Nihar, Tommy Ciardi, Erika Barcelos,Pawan Tripathi,Abhishek Daundkar,Deepa Bhuvanagiri,Hope Omodolor,Hein Htet Aung,Kristen Hernandez,Mirra Rasmussen,Raymond Wieser, Sameera Nalin Venkat,Tian Wang, Weiqi Yue, Yangxin Fan,Rounak Chawla,Leean Jo,Olatunde Akanbi,Zelin Li,Jiqi Liu, Justin Glynn, Kehley Coleman,Jeffery Yarus, Mengjie Li,Kristopher.Davis, Laura Bruckman,Yinghui Wu,Roger French
+Author-email: mxl1171@case.edu,wco3@case.edu,xxy530@case.edu ,lxh442@case.edu,arafath@case.edu,tgc17@case.edu,eib14@case.edu,pkt19@case.edu,aad157@case.edu,dcb117@case.edu,hxo76@case.edu,hxh483@case.edu,kjh125@case.edu,mmr125@case.edu,rxw497@case.edu,sxn440@case.edu,txw387@case.edu,wxy215@case.edu,yxf451@case.edu,rxc542@case.edu,yxj414@case.edu,oda10@case.edu,zxl1080@case.edu,jxl1763@case.edu,jpg90@case.edu,kac196@case.edu,jmy41@case.edu,Mengjie.Li@ucf.edu,Kristopher.Davis@ucf.edu,lsh41@case.edu,yxw1650@case.edu,rxf131@case.edu
 License: BSD License (BSD-3)
 Project-URL: HomePage, https://cwrusdle.bitbucket.io
 Project-URL: Documentation, https://cwrusdle.bitbucket.io/fairmaterials-py/index.html
 Keywords: FAIRification,PowerPlant,Engineering
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 ![logo](https://i.imgur.com/pqR2OBe.png)
 
 # Fairmaterials
 Fairmaterials is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland OH.
-Fairmaterials is a tool for fairing data. It reads a template JSON-LD file to get the preset data. The user can edit the data by manually inputting or by importing a csv file or dataframe. The output will be a sequence of JSON-LD files with the fairified data inside. 
-
+We provide here tools used by the Solar Durability and Lifetime Extension Center (SDLE) for FAIRifying data from materials science projects. Functions have been created for numerous tools common in the field in order to make the metadata more Findable, Accessible, Interoperable, and Reproducible.
 
 # Features
  -  Importing JSON template as JSON-LD.
  -   Modify JSON data.
 		- Based on CSV file.
 		- Based on dataframe file
  -   Output fairiried data as standard JSON-LD format file.
@@ -42,14 +41,55 @@
 ```python
 fairify_data(dataframe,"polymerAdditiveManufacturing")
 ``` 
 ***Output will be series of json-ld format file***
 
 #  Versions
 All notable changes to this project will be documented in this file.
+## [0.4.0] - 2023-04-10
+### Added
+- Expand the domain to 33 
+- Rename domain names
+- Fairify data from different domains,data from different domains inside one dataframe(or CSV)can be fairify to different JSON-LD output according to the JSON-LD template. 
+- Add synonym function which can fairify data according to the synonym inside JSON-LD template  
+#### Domains
+-opticalProfilometry
+-streamWater
+-opticalSpectroscopy
+-metalAdditiveManufacturing
+-environmentalExposure
+-photovoltaicModule
+-asterGdem
+-sample-metadata
+-photovoltaicInverter
+-caryUvVis-instrument-metadata
+-capillaryEletrophoresis-Measurement-metadata
+-waterMetaDataUSGS
+-spectramaxUvVis-results
+-spectramaxUvVis-instrument-metadata
+-photovoltaicCell
+-soilWoSis
+-currentVoltage
+-computedTomographyXRay
+-photovoltaicSystem
+-soil
+-diffractionXRay
+-polymerFormulation
+-photovoltaicBacksheet
+-gasFlux
+-caryUvVis-results
+-caryUvVis-measurement-metadata
+-polymerAdditiveManufacturing
+-spectramaxUvVis-measurement-metadata
+-materials-processing
+-geospatialWell
+-buildings
+-capillaryElectrophoresis-calibration-results
+-waterDataUSGS'
+
 ## [0.3.0] - 2023-02-10
 ### Added
 - Expand the domain to 20 
 - Rename domain names 
 #### Domains
 - diffractionXRay
 - capillaryElectrophoresis
```

### Comparing `fairmaterials-0.3.0/README.md` & `fairmaterials-0.4.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 ![logo](https://i.imgur.com/pqR2OBe.png)
 
 # Fairmaterials
 Fairmaterials is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland OH.
-Fairmaterials is a tool for fairing data. It reads a template JSON-LD file to get the preset data. The user can edit the data by manually inputting or by importing a csv file or dataframe. The output will be a sequence of JSON-LD files with the fairified data inside. 
-
+We provide here tools used by the Solar Durability and Lifetime Extension Center (SDLE) for FAIRifying data from materials science projects. Functions have been created for numerous tools common in the field in order to make the metadata more Findable, Accessible, Interoperable, and Reproducible.
 
 # Features
  -  Importing JSON template as JSON-LD.
  -   Modify JSON data.
 		- Based on CSV file.
 		- Based on dataframe file
  -   Output fairiried data as standard JSON-LD format file.
@@ -27,14 +26,55 @@
 ```python
 fairify_data(dataframe,"polymerAdditiveManufacturing")
 ``` 
 ***Output will be series of json-ld format file***
 
 #  Versions
 All notable changes to this project will be documented in this file.
+## [0.4.0] - 2023-04-10
+### Added
+- Expand the domain to 33 
+- Rename domain names
+- Fairify data from different domains,data from different domains inside one dataframe(or CSV)can be fairify to different JSON-LD output according to the JSON-LD template. 
+- Add synonym function which can fairify data according to the synonym inside JSON-LD template  
+#### Domains
+-opticalProfilometry
+-streamWater
+-opticalSpectroscopy
+-metalAdditiveManufacturing
+-environmentalExposure
+-photovoltaicModule
+-asterGdem
+-sample-metadata
+-photovoltaicInverter
+-caryUvVis-instrument-metadata
+-capillaryEletrophoresis-Measurement-metadata
+-waterMetaDataUSGS
+-spectramaxUvVis-results
+-spectramaxUvVis-instrument-metadata
+-photovoltaicCell
+-soilWoSis
+-currentVoltage
+-computedTomographyXRay
+-photovoltaicSystem
+-soil
+-diffractionXRay
+-polymerFormulation
+-photovoltaicBacksheet
+-gasFlux
+-caryUvVis-results
+-caryUvVis-measurement-metadata
+-polymerAdditiveManufacturing
+-spectramaxUvVis-measurement-metadata
+-materials-processing
+-geospatialWell
+-buildings
+-capillaryElectrophoresis-calibration-results
+-waterDataUSGS'
+
 ## [0.3.0] - 2023-02-10
 ### Added
 - Expand the domain to 20 
 - Rename domain names 
 #### Domains
 - diffractionXRay
 - capillaryElectrophoresis
```

### Comparing `fairmaterials-0.3.0/setup.py` & `fairmaterials-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,24 @@
   'HomePage': 'https://cwrusdle.bitbucket.io',
     'Documentation':'https://cwrusdle.bitbucket.io/fairmaterials-py/index.html'
 }
 
 
 setup(
     name='fairmaterials',
-    version='0.3.0',
+    version='0.4.0',
     keywords=['FAIRification','PowerPlant','Engineering'],
-    description='Generate  JSON-LD format file based on FAIRification standard',
+    description='Make Materials Data FAIR',
     long_description=long_description,
     long_description_content_type='text/markdown',
     project_urls=project_urls,
-    author='Mingjian Lu,Liangyi Huang, Will Oltjen,Xuanji Yu,Arafath Nihar, Tommy Ciardi, Erika Barcelos,Pawan Tripathi,Abhishek Daundkar,Deepa Bhuvanagiri,Hope Omodolor,Hein Htet Aung,Kristen Hernandez,Mirra Rasmussen,Raymond Wieser, Sameera Nalin Venkat,Tian Wang, Weiqi Yue, Yangxin Fan,Rounak Chawla,Leean Jo,Olatunde Akanbi,Zelin Li,Jiqi Liu, Justin Glynn, Kehley Coleman,Jeffery Yarus, Mengjie Li,Kristopher.Davis, Laura Bruckman,Yinghui Wu,Roger French',
-    author_email='mxl1171@case.edu,lxh442@case.edu, wco3@case.edu,xxy530@case.edu ,arafath@case.edu,tgc17@case.edu,eib14@case.edu,pkt19@case.edu,aad157@case.edu,dcb117@case.edu,hxo76@case.edu,hxh483@case.edu,kjh125@case.edu,mmr125@case.edu,rxw497@case.edu,sxn440@case.edu,txw387@case.edu,wxy215@case.edu,yxf451@case.edu,rxc542@case.edu,yxj414@case.edu,oda10@case.edu,zxl1080@case.edu,jxl1763@case.edu,jpg90@case.edu,kac196@case.edu,jmy41@case.edu,Mengjie.Li@ucf.edu,Kristopher.Davis@ucf.edu,lsh41@case.edu,yxw1650@case.edu,rxf131@case.edu',
+    author='Mingjian Lu, Will Oltjen,Xuanji Yu,Liangyi Huang,Arafath Nihar, Tommy Ciardi, Erika Barcelos,Pawan Tripathi,Abhishek Daundkar,Deepa Bhuvanagiri,Hope Omodolor,Hein Htet Aung,Kristen Hernandez,Mirra Rasmussen,Raymond Wieser, Sameera Nalin Venkat,Tian Wang, Weiqi Yue, Yangxin Fan,Rounak Chawla,Leean Jo,Olatunde Akanbi,Zelin Li,Jiqi Liu, Justin Glynn, Kehley Coleman,Jeffery Yarus, Mengjie Li,Kristopher.Davis, Laura Bruckman,Yinghui Wu,Roger French',
+    author_email='mxl1171@case.edu,wco3@case.edu,xxy530@case.edu ,lxh442@case.edu,arafath@case.edu,tgc17@case.edu,eib14@case.edu,pkt19@case.edu,aad157@case.edu,dcb117@case.edu,hxo76@case.edu,hxh483@case.edu,kjh125@case.edu,mmr125@case.edu,rxw497@case.edu,sxn440@case.edu,txw387@case.edu,wxy215@case.edu,yxf451@case.edu,rxc542@case.edu,yxj414@case.edu,oda10@case.edu,zxl1080@case.edu,jxl1763@case.edu,jpg90@case.edu,kac196@case.edu,jmy41@case.edu,Mengjie.Li@ucf.edu,Kristopher.Davis@ucf.edu,lsh41@case.edu,yxw1650@case.edu,rxf131@case.edu',
 
 
     # BSD 3-Clause License:
     # - http://choosealicense.com/licenses/bsd-3-clause
     # - http://opensource.org/licenses/BSD-3-Clause
     license='BSD License (BSD-3)',
     packages=find_packages(),
     include_package_data=True,
-)
+)
```

### Comparing `fairmaterials-0.3.0/LICENSE.txt` & `fairmaterials-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

