# Comparing `tmp/getSourceCode-1.0.3.tar.gz` & `tmp/getSourceCode-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getSourceCode-1.0.3.tar", last modified: Mon Nov 14 14:46:00 2022, max compression
+gzip compressed data, was "getSourceCode-1.0.4.tar", last modified: Mon Apr 10 08:17:09 2023, max compression
```

## Comparing `getSourceCode-1.0.3.tar` & `getSourceCode-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-11-14 14:46:00.960814 getSourceCode-1.0.3/
--rw-rw-rw-   0        0        0     7232 2022-11-14 14:46:00.959815 getSourceCode-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5610 2022-11-14 14:44:56.000000 getSourceCode-1.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-14 14:46:00.938298 getSourceCode-1.0.3/getSourceCode/
--rw-rw-rw-   0        0        0    28370 2022-11-14 14:43:34.000000 getSourceCode-1.0.3/getSourceCode/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-14 14:46:00.957812 getSourceCode-1.0.3/getSourceCode.egg-info/
--rw-rw-rw-   0        0        0     7232 2022-11-14 14:46:00.000000 getSourceCode-1.0.3/getSourceCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2022-11-14 14:46:00.000000 getSourceCode-1.0.3/getSourceCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-14 14:46:00.000000 getSourceCode-1.0.3/getSourceCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-11-14 14:46:00.000000 getSourceCode-1.0.3/getSourceCode.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2022-11-14 14:46:00.000000 getSourceCode-1.0.3/getSourceCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-14 14:46:00.960814 getSourceCode-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      505 2022-11-14 14:39:21.000000 getSourceCode-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:17:09.963257 getSourceCode-1.0.4/
+-rw-rw-rw-   0        0        0     7236 2023-04-10 08:17:09.951721 getSourceCode-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5614 2023-04-10 08:16:44.000000 getSourceCode-1.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 08:17:09.918842 getSourceCode-1.0.4/getSourceCode/
+-rw-rw-rw-   0        0        0    28636 2023-04-10 08:16:33.000000 getSourceCode-1.0.4/getSourceCode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:17:09.944703 getSourceCode-1.0.4/getSourceCode.egg-info/
+-rw-rw-rw-   0        0        0     7236 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 08:17:09.964768 getSourceCode-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-04-10 08:16:50.000000 getSourceCode-1.0.4/setup.py
```

### Comparing `getSourceCode-1.0.3/PKG-INFO` & `getSourceCode-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: getSourceCode
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple way to get contract source code.
 Home-page: https://hxzy.me
 Author: hxzy
 Author-email: hxzy0220@gmail.com
 License: UNKNOWN
 Description: getSourceCode
         =============
@@ -17,15 +17,15 @@
         
         Supported Chain Platforms:
         
         ::
         
             Heco|ETH|BSC|Fantom|Poly|AVAX|ARBI|Tron
         
-            Cronos|moonbeam|moonriver|boba|okex
+            Cronos|moonbeam|moonriver|boba|okex|opt
         
             avax-testnet|arbi-testnet|poly-testnet
         
             bsc-testnet|heco-testnet|ftm-testnet
         
             Goerli|Kovan|Rinkeby|Ropsten
```

### Comparing `getSourceCode-1.0.3/README.rst` & `getSourceCode-1.0.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Supported Chain Platforms:
 
 ::
 
     Heco|ETH|BSC|Fantom|Poly|AVAX|ARBI|Tron
 
-    Cronos|moonbeam|moonriver|boba|okex
+    Cronos|moonbeam|moonriver|boba|okex|opt
 
     avax-testnet|arbi-testnet|poly-testnet
 
     bsc-testnet|heco-testnet|ftm-testnet
 
     Goerli|Kovan|Rinkeby|Ropsten
```

### Comparing `getSourceCode-1.0.3/getSourceCode/__init__.py` & `getSourceCode-1.0.4/getSourceCode/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 import base64
 import json
 import os
 import re
 
 apiKeys = {
     "cronos": [],
+    "opt":[
+        "M88PMFFAS2KAAT71X6UP491MHWA9VMU6V6",
+        "NW3G4BUUVFD1D1YRFQSYGDWFZ81KY9K758",
+        "2CEAVWSQMGTSTA4A6QS95NHYBPU6SDWMMK"
+    ],
     "heco": [
         "JCTU517KN68FM9APHJWPQ7FVPHKFIAUCZB",
         "GWB1A9WKKFVQCE572YH8TA6CHRNVE42R41",
         "ZD6TXYMR7CPM2AVR8I2CNKVF3TMHIQRTKF",
         "MTZUEG344W46RK9HU8ZI8G2HQB91RU474Q",
         "RQ6ZMRWVSE33BEKZ999AYDKX1HU1A2Z5V2",
         "IG8YQGB4ZZCRXNDB7RY3H2SIYPM6SSB67F",
@@ -172,14 +177,15 @@
     "boba-testnet": ["", "", ""],
 }
 
 defaultFolder = "contract"
 
 reqUrl = {
     "heco": "https://api.hecoinfo.com/api?module=contract&action=getsourcecode&address=",
+    "opt": "https://api-optimistic.etherscan.io/api?module=contract&action=getsourcecode&address=",
     "eth": "https://api.etherscan.io/api?module=contract&action=getsourcecode&address=",
     "bsc": "https://api.bscscan.com/api?module=contract&action=getsourcecode&address=",
     "fantom": "https://api.ftmscan.com/api?module=contract&action=getsourcecode&address=",
     "poly": "https://api.polygonscan.com/api?module=contract&action=getsourcecode&address=",
     "avax": "https://api.snowtrace.io/api?module=contract&action=getsourcecode&address=",
     "arbi": "https://api.arbiscan.io/api?module=contract&action=getsourcecode&address=",
     "goerli": "https://api-goerli.etherscan.io/api?module=contract&action=getsourcecode&address=",
@@ -264,15 +270,15 @@
 
 contractInfo = {}
 
 proxyContract = {}
 
 def _argparse():
     parser = argparse.ArgumentParser(
-        description="To get contract source code. \n\nSupport network: \nHeco|ETH|BSC|Fantom|Poly|AVAX|ARBI|Tron\nCronos|moonbeam|moonriver|boba|okex\navax-testnet|arbi-testnet|poly-testnet\nbsc-testnet|heco-testnet|ftm-testnet\nGoerli|Kovan|Rinkeby|Ropsten\nmoonbase|boba-testnet\n\nGet code by tx only supports:\nBSC|ETH|BOBA|ARBI|HECO",
+        description="To get contract source code. \n\nSupport network: \nHeco|ETH|BSC|Fantom|Poly|AVAX|ARBI|Tron\nCronos|moonbeam|moonriver|boba|okex|opt\navax-testnet|arbi-testnet|poly-testnet\nbsc-testnet|heco-testnet|ftm-testnet\nGoerli|Kovan|Rinkeby|Ropsten\nmoonbase|boba-testnet\n\nGet code by tx only supports:\nBSC|ETH|BOBA|ARBI|HECO",
         formatter_class=RawTextHelpFormatter)
     parser.add_argument('-i', default='', dest='inputFile', help='Input file path including contract addresses.')
     parser.add_argument('-o', default='', dest='outputFolder', help='Choose a folder to export.')
     parser.add_argument('-a', default='', dest='address', help='A string including contract addresses.')
     parser.add_argument('-n', default='', dest='network', help='Which network to get source code.')
     parser.add_argument('-k', action="store_true", dest='key', help='Provide some api keys.')
     parser.add_argument('-p', default='', dest='proxy', help='Use a proxy.')
```

### Comparing `getSourceCode-1.0.3/getSourceCode.egg-info/PKG-INFO` & `getSourceCode-1.0.4/getSourceCode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: getSourceCode
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple way to get contract source code.
 Home-page: https://hxzy.me
 Author: hxzy
 Author-email: hxzy0220@gmail.com
 License: UNKNOWN
 Description: getSourceCode
         =============
@@ -17,15 +17,15 @@
         
         Supported Chain Platforms:
         
         ::
         
             Heco|ETH|BSC|Fantom|Poly|AVAX|ARBI|Tron
         
-            Cronos|moonbeam|moonriver|boba|okex
+            Cronos|moonbeam|moonriver|boba|okex|opt
         
             avax-testnet|arbi-testnet|poly-testnet
         
             bsc-testnet|heco-testnet|ftm-testnet
         
             Goerli|Kovan|Rinkeby|Ropsten
```

