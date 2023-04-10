# Comparing `tmp/sinergym-2.2.9.tar.gz` & `tmp/sinergym-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinergym-2.2.9.tar", last modified: Fri Mar 24 15:36:01 2023, max compression
+gzip compressed data, was "sinergym-2.3.0.tar", last modified: Mon Apr 10 18:19:39 2023, max compression
```

## Comparing `sinergym-2.2.9.tar` & `sinergym-2.3.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.701079 sinergym-2.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-24 15:35:59.000000 sinergym-2.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-24 15:35:59.000000 sinergym-2.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-03-24 15:36:01.701079 sinergym-2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-03-24 15:35:59.000000 sinergym-2.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 15:36:01.000000 sinergym-2.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-24 15:36:01.701079 sinergym-2.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-03-24 15:36:01.000000 sinergym-2.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.673079 sinergym-2.2.9/sinergym/
--rw-r--r--   0 runner    (1001) docker     (123)    94684 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.673079 sinergym-2.2.9/sinergym/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.677079 sinergym-2.2.9/sinergym/data/buildings/
--rw-r--r--   0 runner    (1001) docker     (123)   168677 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
--rw-r--r--   0 runner    (1001) docker     (123)   140099 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/buildings/5ZoneAutoDXVAV.idf
--rw-r--r--   0 runner    (1001) docker     (123)   586238 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   373188 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   475269 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/buildings/OfficeGridStorageSmoothing.idf
--rw-r--r--   0 runner    (1001) docker     (123)   265862 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/buildings/ShopWithVandBattery.idf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.677079 sinergym-2.2.9/sinergym/data/variables/
--rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/variables/5ZoneAutoDXVAV.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/variables/ShopWithVandBattery.rdd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.697079 sinergym-2.2.9/sinergym/data/weather/
--rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.697079 sinergym-2.2.9/sinergym/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/envs/eplus_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.697079 sinergym-2.2.9/sinergym/simulators/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/simulators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/simulators/eplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/simulators/eplus_alpha.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.701079 sinergym-2.2.9/sinergym/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39240 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:36:01.673079 sinergym-2.2.9/sinergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-24 15:36:01.000000 sinergym-2.2.9/sinergym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.264739 sinergym-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 18:19:36.000000 sinergym-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-10 18:19:36.000000 sinergym-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-10 18:19:39.264739 sinergym-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-04-10 18:19:36.000000 sinergym-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 18:19:38.000000 sinergym-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-10 18:19:39.264739 sinergym-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-10 18:19:38.000000 sinergym-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.232739 sinergym-2.3.0/sinergym/
+-rw-r--r--   0 runner    (1001) docker     (123)    94684 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.232739 sinergym-2.3.0/sinergym/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.236739 sinergym-2.3.0/sinergym/data/buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)   168677 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   140099 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/5ZoneAutoDXVAV.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   586238 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   373188 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   475269 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/OfficeGridStorageSmoothing.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   265862 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/ShopWithVandBattery.idf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.236739 sinergym-2.3.0/sinergym/data/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/5ZoneAutoDXVAV.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/ShopWithVandBattery.rdd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.260739 sinergym-2.3.0/sinergym/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.260739 sinergym-2.3.0/sinergym/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/envs/eplus_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.260739 sinergym-2.3.0/sinergym/simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/simulators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/simulators/eplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/simulators/eplus_alpha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.264739 sinergym-2.3.0/sinergym/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39240 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.236739 sinergym-2.3.0/sinergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/top_level.txt
```

### Comparing `sinergym-2.2.9/LICENSE` & `sinergym-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/PKG-INFO` & `sinergym-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.2.9
+Version: 2.3.0
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 2.2.9 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.3.0 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.2.9/README.md` & `sinergym-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/setup.py` & `sinergym-2.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       keywords='control reinforcement-learning buildings reinforcement-learning-environments',
       install_requires=reqs,
       include_package_data=True,
       extras_require={
           'extras': [
               'matplotlib',  # visualization
               # DRL with pytorch
-              'stable-baselines3',
+              'stable-baselines3 @ git+https://github.com/DLR-RM/stable-baselines3@feat/gymnasium-support#egg=stable-baselines3',
               'wandb',
               'pytest',
               'pytest-cov',
               'pytest-xdist',  # Unit test repository
               'sphinx',  # documentation
               'sphinx-rtd-theme',  # documentation theme
               'sphinxcontrib-spelling',  # documentation spelling
@@ -43,19 +43,19 @@
               'google-cloud-storage==2.5.0',
               'IPython'
           ],
           'test': [
               'pytest',
               'pytest-cov',
               'pytest-xdist',
-              'stable-baselines3',
+              'stable-baselines3 @ git+https://github.com/DLR-RM/stable-baselines3@feat/gymnasium-support#egg=stable-baselines3',
               'wandb'
           ],
           'DRL': [
-              'stable-baselines3',
+              'stable-baselines3 @ git+https://github.com/DLR-RM/stable-baselines3@feat/gymnasium-support#egg=stable-baselines3',
               'wandb'
           ],
           'doc': [
               'sphinx',
               'sphinx-rtd-theme',
               'sphinxcontrib-spelling',
               'sphinx-multiversion @ git+https://github.com/Holzhaus/sphinx-multiversion#egg=sphinx-multiversion',
```

### Comparing `sinergym-2.2.9/sinergym/__init__.py` & `sinergym-2.3.0/sinergym/__init__.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf` & `sinergym-2.3.0/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/buildings/5ZoneAutoDXVAV.idf` & `sinergym-2.3.0/sinergym/data/buildings/5ZoneAutoDXVAV.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf` & `sinergym-2.3.0/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf` & `sinergym-2.3.0/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/buildings/OfficeGridStorageSmoothing.idf` & `sinergym-2.3.0/sinergym/data/buildings/OfficeGridStorageSmoothing.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/buildings/ShopWithVandBattery.idf` & `sinergym-2.3.0/sinergym/data/buildings/ShopWithVandBattery.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd` & `sinergym-2.3.0/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/variables/5ZoneAutoDXVAV.rdd` & `sinergym-2.3.0/sinergym/data/variables/5ZoneAutoDXVAV.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd` & `sinergym-2.3.0/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd` & `sinergym-2.3.0/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/variables/OfficeGridStorageSmoothing.rdd` & `sinergym-2.3.0/sinergym/data/variables/OfficeGridStorageSmoothing.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/variables/ShopWithVandBattery.rdd` & `sinergym-2.3.0/sinergym/data/variables/ShopWithVandBattery.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy` & `sinergym-2.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw` & `sinergym-2.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy` & `sinergym-2.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/COL_Bogota.802220_IWEC.epw` & `sinergym-2.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy` & `sinergym-2.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/ESP_Granada.084190_SWEC.epw` & `sinergym-2.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy` & `sinergym-2.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw` & `sinergym-2.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy` & `sinergym-2.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw` & `sinergym-2.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy` & `sinergym-2.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw` & `sinergym-2.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy` & `sinergym-2.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw` & `sinergym-2.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy` & `sinergym-2.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw` & `sinergym-2.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy` & `sinergym-2.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw` & `sinergym-2.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy` & `sinergym-2.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw` & `sinergym-2.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy` & `sinergym-2.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw` & `sinergym-2.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy` & `sinergym-2.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw` & `sinergym-2.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy` & `sinergym-2.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw` & `sinergym-2.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/envs/eplus_env.py` & `sinergym-2.3.0/sinergym/envs/eplus_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,18 @@
         # ---------------------------------------------------------------------------- #
         #                             Variables definition                             #
         # ---------------------------------------------------------------------------- #
         self.variables = {}
         self.variables['observation'] = observation_variables
         self.variables['action'] = action_variables
 
+        # Copy to use original variables in step.obs_dict for reward
+        self.original_obs = observation_variables
+        self.original_act = action_variables
+
         self.name = env_name
 
         # ---------------------------------------------------------------------------- #
         #                                   Simulator                                  #
         # ---------------------------------------------------------------------------- #
         self.simulator = EnergyPlus(
             env_name=env_name,
@@ -108,14 +112,16 @@
 
         # ---------------------------------------------------------------------------- #
         #        Adding simulation date to observation (not needed in simulator)       #
         # ---------------------------------------------------------------------------- #
 
         self.variables['observation'] = ['year', 'month',
                                          'day', 'hour'] + self.variables['observation']
+        self.original_obs = ['year', 'month',
+                             'day', 'hour'] + self.original_obs
 
         # ---------------------------------------------------------------------------- #
         #                          reset default options                               #
         # ---------------------------------------------------------------------------- #
         self.default_options = {}
         # Weather Variability
         if weather_variability:
@@ -153,16 +159,15 @@
                     np.repeat(1, action_space.shape[0]), dtype=np.float32),
                 dtype=action_space.dtype
             )
 
         # ---------------------------------------------------------------------------- #
         #                                    Reward                                    #
         # ---------------------------------------------------------------------------- #
-        self.reward_fn = reward(self, **reward_kwargs)
-        self.obs_dict = None
+        self.reward_fn = reward(**reward_kwargs)
 
         # ---------------------------------------------------------------------------- #
         #                        Environment definition checker                        #
         # ---------------------------------------------------------------------------- #
 
         self._check_eplus_env()
 
@@ -220,19 +225,18 @@
 
         # Get action
         action_ = self._get_action(action)
         # Send action to the simulator
         self.simulator.logger_main.debug(action_)
         # Execute action in simulation
         obs, terminated, truncated, info = self.simulator.step(action_)
-        # Create dictionary with observation
-        self.obs_dict = dict(zip(self.variables['observation'], obs))
+        obs_dict = dict(zip(self.original_obs, obs))
 
         # Calculate reward
-        reward, terms = self.reward_fn()
+        reward, terms = self.reward_fn(obs_dict)
 
         # info update with reward information
         info.update({'reward': reward})
         info.update(terms)
 
         return np.array(
             obs, dtype=np.float32), reward, terminated, truncated, info
```

### Comparing `sinergym-2.2.9/sinergym/simulators/base.py` & `sinergym-2.3.0/sinergym/simulators/base.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/simulators/eplus.py` & `sinergym-2.3.0/sinergym/simulators/eplus.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/simulators/eplus_alpha.py` & `sinergym-2.3.0/sinergym/simulators/eplus_alpha.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/callbacks.py` & `sinergym-2.3.0/sinergym/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/common.py` & `sinergym-2.3.0/sinergym/utils/common.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/config.py` & `sinergym-2.3.0/sinergym/utils/config.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/constants.py` & `sinergym-2.3.0/sinergym/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/controllers.py` & `sinergym-2.3.0/sinergym/utils/controllers.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/env_checker.py` & `sinergym-2.3.0/sinergym/utils/env_checker.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/evaluation.py` & `sinergym-2.3.0/sinergym/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/gcloud.py` & `sinergym-2.3.0/sinergym/utils/gcloud.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/logger.py` & `sinergym-2.3.0/sinergym/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym/utils/rewards.py` & `sinergym-2.3.0/sinergym/utils/rewards.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,34 @@
 from typing import Any, Dict, List, Tuple, Union
 
 from gymnasium import Env
 
 
 class BaseReward(object):
 
-    def __init__(self, env):
+    def __init__(self):
         """
         Base reward class.
 
         All reward functions should inherit from this class.
 
         Args:
             env (Env): Gym environment.
         """
-        self.env = env
 
     def __call__(self):
         """Method for calculating the reward function."""
         raise NotImplementedError(
             "Reward class must have a `__call__` method.")
 
 
 class LinearReward(BaseReward):
 
     def __init__(
         self,
-        env: Env,
         temperature_variable: Union[str, list],
         energy_variable: str,
         range_comfort_winter: Tuple[int, int],
         range_comfort_summer: Tuple[int, int],
         summer_start: Tuple[int, int] = (6, 1),
         summer_final: Tuple[int, int] = (9, 30),
         energy_weight: float = 0.5,
@@ -47,27 +45,26 @@
 
         It considers the energy consumption and the absolute difference to temperature comfort.
 
         .. math::
             R = - W * lambda_E * power - (1 - W) * lambda_T * (max(T - T_{low}, 0) + max(T_{up} - T, 0))
 
         Args:
-            env (Env): Gym environment.
             temperature_variable (Union[str, list]): Name(s) of the temperature variable(s).
             energy_variable (str): Name of the energy/power variable.
             range_comfort_winter (Tuple[int,int]): Temperature comfort range for cold season. Depends on environment you are using.
             range_comfort_summer (Tuple[int,int]): Temperature comfort range for hot season. Depends on environment you are using.
             summer_start (Tuple[int,int]): Summer session tuple with month and day start. Defaults to (6,1).
             summer_final (Tuple[int,int]): Summer session tuple with month and day end. defaults to (9,30).
             energy_weight (float, optional): Weight given to the energy term. Defaults to 0.5.
             lambda_energy (float, optional): Constant for removing dimensions from power(1/W). Defaults to 1e-4.
             lambda_temperature (float, optional): Constant for removing dimensions from temperature(1/C). Defaults to 1.0.
         """
 
-        super(LinearReward, self).__init__(env)
+        super(LinearReward, self).__init__()
 
         # Name of the variables
         self.temp_name = temperature_variable
         self.energy_name = energy_variable
 
         # Reward parameters
         self.range_comfort_winter = range_comfort_winter
@@ -76,23 +73,24 @@
         self.lambda_energy = lambda_energy
         self.lambda_temp = lambda_temperature
 
         # Summer period
         self.summer_start = summer_start  # (month,day)
         self.summer_final = summer_final  # (month,day)
 
-    def __call__(self) -> Tuple[float, Dict[str, Any]]:
-        """
-        Calculate the reward function.
+    def __call__(self, obs_dict: Dict[str, Any]
+                 ) -> Tuple[float, Dict[str, Any]]:
+        """Calculate the reward function.
+
+        Args:
+            obs_dict (Dict[str, Any]): Dict with observation variable name (key) and observation variable value (value)
 
         Returns:
             Tuple[float, Dict[str, Any]]: Reward value and dictionary with their individual components.
         """
-        # Current observation
-        obs_dict = self.env.obs_dict.copy()
 
         # Energy term
         reward_energy = - self.lambda_energy * obs_dict[self.energy_name]
 
         # Comfort
         comfort, temps = self._get_comfort(obs_dict)
         reward_comfort = - self.lambda_temp * comfort
@@ -120,23 +118,23 @@
         Returns:
             Tuple[float, List[float]]: comfort penalty and List with temperatures used.
         """
 
         month = obs_dict['month']
         day = obs_dict['day']
         year = obs_dict['year']
-        current_dt = datetime(year, month, day)
+        current_dt = datetime(int(year), int(month), int(day))
 
         # Periods
         summer_start_date = datetime(
-            year,
+            int(year),
             self.summer_start[0],
             self.summer_start[1])
         summer_final_date = datetime(
-            year,
+            int(year),
             self.summer_final[0],
             self.summer_final[1])
 
         if current_dt >= summer_start_date and current_dt <= summer_final_date:
             temp_range = self.range_comfort_summer
         else:
             temp_range = self.range_comfort_winter
@@ -150,15 +148,14 @@
         return comfort, temps
 
 
 class ExpReward(LinearReward):
 
     def __init__(
         self,
-        env: Env,
         temperature_variable: Union[str, list],
         energy_variable: str,
         range_comfort_winter: Tuple[int, int],
         range_comfort_summer: Tuple[int, int],
         summer_start: Tuple[int, int] = (6, 1),
         summer_final: Tuple[int, int] = (9, 30),
         energy_weight: float = 0.5,
@@ -168,28 +165,26 @@
         """
         Reward considering exponential absolute difference to temperature comfort.
 
         .. math::
             R = - W * lambda_E * power - (1 - W) * lambda_T * exp( (max(T - T_{low}, 0) + max(T_{up} - T, 0)) )
 
         Args:
-            env (Env): Gym environment.
             temperature_variable (Union[str, list]): Name(s) of the temperature variable(s).
             energy_variable (str): Name of the energy/power variable.
             range_comfort_winter (Tuple[int,int]): Temperature comfort range for cold season. Depends on environment you are using.
             range_comfort_summer (Tuple[int,int]): Temperature comfort range for hot season. Depends on environment you are using.
             summer_start (Tuple[int,int]): Summer session tuple with month and day start. Defaults to (6,1).
             summer_final (Tuple[int,int]): Summer session tuple with month and day end. defaults to (9,30).
             energy_weight (float, optional): Weight given to the energy term. Defaults to 0.5.
             lambda_energy (float, optional): Constant for removing dimensions from power(1/W). Defaults to 1e-4.
             lambda_temperature (float, optional): Constant for removing dimensions from temperature(1/C). Defaults to 1.0.
         """
 
         super(ExpReward, self).__init__(
-            env,
             temperature_variable,
             energy_variable,
             range_comfort_winter,
             range_comfort_summer,
             summer_start,
             summer_final,
             energy_weight,
@@ -206,23 +201,23 @@
         Returns:
             Tuple[float, List[float]]: comfort penalty and List with temperatures used.
         """
 
         month = obs_dict['month']
         day = obs_dict['day']
         year = obs_dict['year']
-        current_dt = datetime(year, month, day)
+        current_dt = datetime(int(year), int(month), int(day))
 
         # Periods
         summer_start_date = datetime(
-            year,
+            int(year),
             self.summer_start[0],
             self.summer_start[1])
         summer_final_date = datetime(
-            year,
+            int(year),
             self.summer_final[0],
             self.summer_final[1])
 
         if current_dt >= summer_start_date and current_dt <= summer_final_date:
             temp_range = self.range_comfort_summer
         else:
             temp_range = self.range_comfort_winter
@@ -237,15 +232,14 @@
         return comfort, temps
 
 
 class HourlyLinearReward(LinearReward):
 
     def __init__(
         self,
-        env: Env,
         temperature_variable: Union[str, list],
         energy_variable: str,
         range_comfort_winter: Tuple[int, int],
         range_comfort_summer: Tuple[int, int],
         summer_start: Tuple[int, int] = (6, 1),
         summer_final: Tuple[int, int] = (9, 30),
         min_energy_weight: float = 0.5,
@@ -253,52 +247,51 @@
         lambda_temperature: float = 1.0,
         range_comfort_hours: tuple = (9, 19),
     ):
         """
         Linear reward function with a time-dependent weight for consumption and energy terms.
 
         Args:
-            env (Env): Gym environment.
             temperature_variable (Union[str, list]): Name(s) of the temperature variable(s).
             energy_variable (str): Name of the energy/power variable.
             range_comfort_winter (Tuple[int,int]): Temperature comfort range for cold season. Depends on environment you are using.
             range_comfort_summer (Tuple[int,int]): Temperature comfort range for hot season. Depends on environment you are using.
             summer_start (Tuple[int,int]): Summer session tuple with month and day start. Defaults to (6,1).
             summer_final (Tuple[int,int]): Summer session tuple with month and day end. defaults to (9,30).
             min_energy_weight (float, optional): Minimum weight given to the energy term. Defaults to 0.5.
             lambda_energy (float, optional): Constant for removing dimensions from power(1/W). Defaults to 1e-4.
             lambda_temperature (float, optional): Constant for removing dimensions from temperature(1/C). Defaults to 1.0.
             range_comfort_hours (tuple, optional): Hours where thermal comfort is considered. Defaults to (9, 19).
         """
 
         super(HourlyLinearReward, self).__init__(
-            env,
             temperature_variable,
             energy_variable,
             range_comfort_winter,
             range_comfort_summer,
             summer_start,
             summer_final,
             min_energy_weight,
             lambda_energy,
             lambda_temperature
         )
 
         # Reward parameters
         self.range_comfort_hours = range_comfort_hours
 
-    def __call__(self) -> Tuple[float, Dict[str, Any]]:
+    def __call__(self, obs_dict: Dict[str, Any]
+                 ) -> Tuple[float, Dict[str, Any]]:
         """Calculate the reward function.
 
-        Returns:
-            Tuple[float, Dict[str, Any]]: Reward and dict with reward terms.
-            """
-        # Current observation
-        obs_dict = self.env.obs_dict.copy()
+        Args:
+            obs_dict (Dict[str, Any]): Dict with observation variable name (key) and observation variable value (value)
 
+        Returns:
+            Tuple[float, Dict[str, Any]]: Reward value and dictionary with their individual components.
+        """
         # Energy term
         reward_energy = - self.lambda_energy * obs_dict[self.energy_name]
 
         # Comfort
         comfort, temps = self._get_comfort(obs_dict)
         reward_comfort = - self.lambda_temp * comfort
```

### Comparing `sinergym-2.2.9/sinergym/utils/wrappers.py` & `sinergym-2.3.0/sinergym/utils/wrappers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Implementation of custom Gym environments."""
 
 import random
 from collections import deque
+from copy import deepcopy
+from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import gymnasium as gym
 import numpy as np
 
 from sinergym.utils.common import is_wrapped
 from sinergym.utils.logger import CSVLogger
@@ -325,15 +327,199 @@
         self.logger.activate_flag()
 
     def deactivate_logger(self) -> None:
         """Deactivate logger if its flag True.
         """
         self.logger.deactivate_flag()
 
-# ---------------------- Specific environment wrappers ---------------------#
+
+class DatetimeWrapper(gym.ObservationWrapper):
+    """Wrapper to substitute day value by is_weekend flag, and hour and month by sin and cos values.
+       Observation space is updated automatically."""
+
+    def __init__(self,
+                 env: Any):
+        super(DatetimeWrapper, self).__init__(env)
+        # Update new shape
+        new_shape = env.observation_space.shape[0] + 2
+        self.observation_space = gym.spaces.Box(
+            low=-5e6, high=5e6, shape=(new_shape,), dtype=np.float32)
+        # Update observation variables
+        day_index = self.variables['observation'].index('day')
+        self.variables['observation'][day_index] = 'is_weekend'
+        hour_index = self.variables['observation'].index('hour')
+        self.variables['observation'][hour_index] = 'hour_cos'
+        self.variables['observation'].insert(hour_index + 1, 'hour_sin')
+        month_index = self.variables['observation'].index('month')
+        self.variables['observation'][month_index] = 'month_cos'
+        self.variables['observation'].insert(month_index + 1, 'month_sin')
+
+    def observation(self, obs: np.ndarray) -> np.ndarray:
+        """Applies calculation in is_weekend flag, and sen and cos in hour and month
+
+        Args:
+            obs (np.ndarray): Original observation.
+
+        Returns:
+            np.ndarray: Transformed observation.
+        """
+        obs_dict = dict(zip(self.original_obs, obs))
+        # New obs dict with same values than obs_dict but with new fields with
+        # None
+        new_obs = dict.fromkeys(self.variables['observation'])
+        for key, value in obs_dict.items():
+            if key in new_obs.keys():
+                new_obs[key] = value
+        dt = datetime(
+            int(obs_dict['year']),
+            int(obs_dict['month']),
+            int(obs_dict['day']),
+            int(obs_dict['hour']))
+        # Update obs
+        new_obs['is_weekend'] = 1.0 if dt.isoweekday() in [6, 7] else 0.0
+        new_obs['hour_cos'] = np.cos(obs_dict['hour'])
+        new_obs['hour_sin'] = np.sin(obs_dict['hour'])
+        new_obs['month_cos'] = np.cos(obs_dict['month'])
+        new_obs['month_sin'] = np.sin(obs_dict['month'])
+
+        return np.array(list(new_obs.values()))
+
+
+class PreviousObservationWrapper(gym.ObservationWrapper):
+    """Wrapper to add observation values from previous timestep to
+    current environment observation"""
+
+    def __init__(self,
+                 env: Any,
+                 previous_variables: List[str]):
+        super(PreviousObservationWrapper, self).__init__(env)
+        # Check and apply previous variables to observation space and variables
+        # names
+        self.original_variable_index = []
+        for obs_var in previous_variables:
+            assert obs_var in self.variables['observation'], '{} variable is not defined in observation space, revise the name.'.format(
+                obs_var)
+            self.original_variable_index.append(
+                self.variables['observation'].index(obs_var))
+            self.variables['observation'].append(obs_var + '_previous')
+        # Update new shape
+        new_shape = env.observation_space.shape[0] + len(previous_variables)
+        self.observation_space = gym.spaces.Box(
+            low=-5e6, high=5e6, shape=(new_shape,), dtype=np.float32)
+
+        # previous observation initialization
+        self.previous_observation = np.zeros(
+            shape=len(previous_variables), dtype=np.float32)
+
+    def observation(self, obs: np.ndarray) -> np.ndarray:
+        """Add previous observation to the current one
+
+        Args:
+            obs (np.ndarray): Original observation.
+
+        Returns:
+            np.ndarray: observation with
+        """
+
+        new_obs = np.concatenate((obs, self.previous_observation))
+        # Aquí tengo que seleccionar las variables que se correponden con lo
+        # que son
+        self.previous_observation = obs[self.original_variable_index]
+
+        return new_obs
+
+
+class DiscreteIncrementalWrapper(gym.ActionWrapper):
+    """A wrapper for an incremental setpoint discrete action space environment.
+    WARNING: A environment with only temperature setpoints control must be used
+    with this wrapper."""
+
+    def __init__(
+        self,
+        env: gym.Env,
+        max_values: List[float],
+        min_values: List[float],
+        delta_temp: float = 2.0,
+        step_temp: float = 0.5,
+    ):
+        """
+        Args:
+            env: The original Sinergym env.
+            action_names: Name of the action variables with the setpoint control you want to do incremental.
+            initial_values: Initial values of the setpoints. One list per zone: [[heating zone 1, cooling zone 1], [heating zone 2, cooling zone 2], ...]
+            heating_range: Acceptable values for the heating setpoint.
+            cooling_range: Acceptable values for the cooling setpoint.
+            delta_temp: Maximum temperature variation in the setpoints in one step.
+            step_temp: Minimum temperature variation in the setpoints in one step.
+        """
+
+        super().__init__(env)
+
+        # Params
+        self.env = env
+        self.current_setpoints = []
+        self.max_values = max_values
+        self.min_values = min_values
+
+        # calculate initial values for setpoints
+        for external_schedule in self.env.simulator._config.building.ExternalInterface_Schedule:
+            self.current_setpoints.append(external_schedule.initial_value)
+
+        # Check environment is valid
+        assert len(
+            self.current_setpoints) == len(
+            self.env.variables['action']), 'IncrementalWrapper: Number of variables is different from environment'
+        assert len(
+            self.current_setpoints) == len(
+            self.max_values), 'IncrementalWrapper: max_values specified is incorrect for the number of action variables'
+        assert len(
+            self.current_setpoints) == len(
+            self.min_values), 'IncrementalWrapper: min_values specified is incorrect for the number of action variables'
+        assert self.env.flag_discrete, 'IncrementalWrapper: Environment wrapped must be discrete'
+
+        # Define all posible setpoint variations
+        values = np.arange(step_temp, delta_temp + step_temp / 10, step_temp)
+        values = [v for v in [*values, *-values]]
+
+        # Reset default environment action_mapping
+        self.action_mapping = {}
+        do_nothing = [0.0 for _ in range(
+            len(self.env.variables['action']))]  # do nothing
+        self.action_mapping[0] = do_nothing
+        n = 1
+
+        # Generate all posible actions
+        for k in range(len(self.env.variables['action'])):
+            for v in values:
+                x = do_nothing.copy()
+                x[k] = v
+                self.action_mapping[n] = x
+                n += 1
+
+        self.action_space = gym.spaces.Discrete(n)
+        print(f'New incremental action mapping: {n}')
+        print(self.action_mapping)
+
+    def action(self, action):
+        """Takes the discrete action and transforms it to setpoints tuple."""
+        action_ = self.action_mapping[action]
+        # Update current setpoints values with incremental action
+        self.current_setpoints = [
+            sum(i) for i in zip(
+                self.current_setpoints,
+                action_)]
+
+        setpoints = np.clip(
+            np.array(self.current_setpoints),
+            self.min_values,
+            self.max_values
+        )
+        return list(setpoints)
+
+    # ---------------------- Specific environment wrappers ---------------------#
 
 
 class OfficeGridStorageSmoothingActionConstraintsWrapper(
         gym.ActionWrapper):  # pragma: no cover
     def __init__(self, env):
         assert env.idf_path.split(
             '/')[-1] == 'OfficeGridStorageSmoothing.idf', 'OfficeGridStorageSmoothingActionConstraintsWrapper: This wrapper is not valid for this environment.'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sinergym-2.2.9/sinergym.egg-info/PKG-INFO` & `sinergym-2.3.0/sinergym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.2.9
+Version: 2.3.0
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 2.2.9 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.3.0 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.2.9/sinergym.egg-info/SOURCES.txt` & `sinergym-2.3.0/sinergym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinergym-2.2.9/sinergym.egg-info/requires.txt` & `sinergym-2.3.0/sinergym.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 opyplus
 pandas
 pytype
 twine
 xlsxwriter
 
 [DRL]
-stable-baselines3
+stable-baselines3@ git+https://github.com/DLR-RM/stable-baselines3@feat/gymnasium-support#egg=stable-baselines3
 wandb
 
 [doc]
 IPython
 nbsphinx
 nbsphinx_link
 pyenchant
@@ -37,24 +37,24 @@
 pytest-cov
 pytest-xdist
 sphinx
 sphinx-multitoc-numbering
 sphinx-multiversion@ git+https://github.com/Holzhaus/sphinx-multiversion#egg=sphinx-multiversion
 sphinx-rtd-theme
 sphinxcontrib-spelling
-stable-baselines3
+stable-baselines3@ git+https://github.com/DLR-RM/stable-baselines3@feat/gymnasium-support#egg=stable-baselines3
 wandb
 
 [gcloud]
 google-api-python-client==2.58.0
 google-cloud-storage==2.5.0
 oauth2client==4.1.3
 
 [test]
 pytest
 pytest-cov
 pytest-xdist
-stable-baselines3
+stable-baselines3@ git+https://github.com/DLR-RM/stable-baselines3@feat/gymnasium-support#egg=stable-baselines3
 wandb
 
 [visualization]
 matplotlib
```

