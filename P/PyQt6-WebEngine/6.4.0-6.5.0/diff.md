# Comparing `tmp/PyQt6_WebEngine-6.4.0.tar.gz` & `tmp/PyQt6_WebEngine-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_WebEngine-6.4.0.tar", last modified: Fri Sep 30 10:29:56 2022, max compression
+gzip compressed data, was "PyQt6_WebEngine-6.5.0.tar", last modified: Tue Apr  4 15:25:07 2023, max compression
```

## Comparing `PyQt6_WebEngine-6.4.0.tar` & `PyQt6_WebEngine-6.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:29:56.243795 PyQt6_WebEngine-6.4.0/
--rw-r--r--   0 phil       (501) staff       (20)     4025 2022-09-30 10:29:55.681202 PyQt6_WebEngine-6.4.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2022-09-30 10:29:55.520176 PyQt6_WebEngine-6.4.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      403 2022-09-30 10:27:37.363176 PyQt6_WebEngine-6.4.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1787 2022-09-30 10:29:56.243899 PyQt6_WebEngine-6.4.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1453 2022-09-30 10:29:55.682166 PyQt6_WebEngine-6.4.0/README
--rw-r--r--   0 phil       (501) staff       (20)      959 2022-09-30 10:29:55.682508 PyQt6_WebEngine-6.4.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:29:56.232224 PyQt6_WebEngine-6.4.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:29:56.243496 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/
--rw-r--r--   0 phil       (501) staff       (20)     3428 2022-09-30 10:29:56.025116 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/QtWebEngineCoremod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1284 2022-09-30 10:29:56.064562 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qtwebenginecoreglobal.sip
--rw-r--r--   0 phil       (501) staff       (20)     2140 2022-09-30 10:29:56.025675 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginecertificateerror.sip
--rw-r--r--   0 phil       (501) staff       (20)     1425 2022-09-30 10:29:56.023094 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineclientcertificateselection.sip
--rw-r--r--   0 phil       (501) staff       (20)     1397 2022-09-30 10:29:56.016109 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineclientcertificatestore.sip
--rw-r--r--   0 phil       (501) staff       (20)     2535 2022-09-30 10:29:56.061333 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginecontextmenurequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     4428 2022-09-30 10:29:56.057765 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginecookiestore.sip
--rw-r--r--   0 phil       (501) staff       (20)     3408 2022-09-30 10:29:56.018705 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginedownloadrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2069 2022-09-30 10:29:56.022156 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginefilesystemaccessrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1282 2022-09-30 10:29:56.023513 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginefindtextresult.sip
--rw-r--r--   0 phil       (501) staff       (20)     1296 2022-09-30 10:29:56.062497 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginefullscreenrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2995 2022-09-30 10:29:56.020087 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginehistory.sip
--rw-r--r--   0 phil       (501) staff       (20)     2156 2022-09-30 10:29:56.027052 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginehttprequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2091 2022-09-30 10:29:56.063209 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineloadinginfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1741 2022-09-30 10:29:56.020588 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginenavigationrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1495 2022-09-30 10:29:56.021053 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginenewwindowrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1526 2022-09-30 10:29:56.056467 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginenotification.sip
--rw-r--r--   0 phil       (501) staff       (20)    14679 2022-09-30 10:29:56.060545 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginepage.sip
--rw-r--r--   0 phil       (501) staff       (20)     8324 2022-09-30 10:29:56.017897 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineprofile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1333 2022-09-30 10:29:56.024518 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginequotarequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1435 2022-09-30 10:29:56.026543 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineregisterprotocolhandlerrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2015 2022-09-30 10:29:56.021605 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginescript.sip
--rw-r--r--   0 phil       (501) staff       (20)     1522 2022-09-30 10:29:56.026108 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginescriptcollection.sip
--rw-r--r--   0 phil       (501) staff       (20)     3701 2022-09-30 10:29:56.064070 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginesettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     2606 2022-09-30 10:29:56.019373 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlrequestinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1270 2022-09-30 10:29:56.016535 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlrequestinterceptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1615 2022-09-30 10:29:56.022636 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlrequestjob.sip
--rw-r--r--   0 phil       (501) staff       (20)     2340 2022-09-30 10:29:56.024091 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlscheme.sip
--rw-r--r--   0 phil       (501) staff       (20)     1277 2022-09-30 10:29:56.061837 PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlschemehandler.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:29:56.231845 PyQt6_WebEngine-6.4.0/sip/QtWebEngineQuick/
--rw-r--r--   0 phil       (501) staff       (20)     2077 2022-09-30 10:29:56.014337 PyQt6_WebEngine-6.4.0/sip/QtWebEngineQuick/QtWebEngineQuickmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     4363 2022-09-30 10:29:56.015183 PyQt6_WebEngine-6.4.0/sip/QtWebEngineQuick/qquickwebengineprofile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1094 2022-09-30 10:29:56.015573 PyQt6_WebEngine-6.4.0/sip/QtWebEngineQuick/qtwebenginequickglobal.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:29:56.230470 PyQt6_WebEngine-6.4.0/sip/QtWebEngineWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2225 2022-09-30 10:29:56.013879 PyQt6_WebEngine-6.4.0/sip/QtWebEngineWidgets/QtWebEngineWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     7637 2022-09-30 10:29:56.013344 PyQt6_WebEngine-6.4.0/sip/QtWebEngineWidgets/qwebengineview.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:25:07.309769 PyQt6_WebEngine-6.5.0/
+-rw-r--r--   0 phil       (501) staff       (20)     4237 2023-04-04 15:25:06.752939 PyQt6_WebEngine-6.5.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2023-04-04 15:25:06.571606 PyQt6_WebEngine-6.5.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      458 2023-04-04 15:22:33.896329 PyQt6_WebEngine-6.5.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1787 2023-04-04 15:25:07.309887 PyQt6_WebEngine-6.5.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1453 2023-04-04 15:25:06.753937 PyQt6_WebEngine-6.5.0/README
+-rw-r--r--   0 phil       (501) staff       (20)      959 2023-04-04 15:25:06.754313 PyQt6_WebEngine-6.5.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:25:07.298929 PyQt6_WebEngine-6.5.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:25:07.309551 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/
+-rw-r--r--   0 phil       (501) staff       (20)     3446 2023-04-04 15:25:07.124042 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/QtWebEngineCoremod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1352 2023-04-04 15:25:07.133484 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qtwebenginecoreglobal.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2140 2023-04-04 15:25:07.124607 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginecertificateerror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1425 2023-04-04 15:25:07.121919 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineclientcertificateselection.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1397 2023-04-04 15:25:07.114445 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineclientcertificatestore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2535 2023-04-04 15:25:07.130869 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginecontextmenurequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4428 2023-04-04 15:25:07.127705 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginecookiestore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3408 2023-04-04 15:25:07.117276 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginedownloadrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2069 2023-04-04 15:25:07.120925 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginefilesystemaccessrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1282 2023-04-04 15:25:07.122357 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginefindtextresult.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1296 2023-04-04 15:25:07.131736 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginefullscreenrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2995 2023-04-04 15:25:07.118727 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginehistory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2156 2023-04-04 15:25:07.126178 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginehttprequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2091 2023-04-04 15:25:07.132276 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineloadinginfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1741 2023-04-04 15:25:07.119258 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginenavigationrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1495 2023-04-04 15:25:07.119764 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginenewwindowrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1526 2023-04-04 15:25:07.126715 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginenotification.sip
+-rw-r--r--   0 phil       (501) staff       (20)    14679 2023-04-04 15:25:07.130143 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginepage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8472 2023-04-04 15:25:07.116404 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineprofile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1333 2023-04-04 15:25:07.123412 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginequotarequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1435 2023-04-04 15:25:07.125527 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineregisterprotocolhandlerrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2015 2023-04-04 15:25:07.120344 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginescript.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1522 2023-04-04 15:25:07.125080 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginescriptcollection.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3701 2023-04-04 15:25:07.133041 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginesettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2692 2023-04-04 15:25:07.117988 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlrequestinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1270 2023-04-04 15:25:07.114900 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlrequestinterceptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1615 2023-04-04 15:25:07.121447 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlrequestjob.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2340 2023-04-04 15:25:07.122965 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlscheme.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1277 2023-04-04 15:25:07.131295 PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlschemehandler.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:25:07.298620 PyQt6_WebEngine-6.5.0/sip/QtWebEngineQuick/
+-rw-r--r--   0 phil       (501) staff       (20)     2077 2023-04-04 15:25:07.112374 PyQt6_WebEngine-6.5.0/sip/QtWebEngineQuick/QtWebEngineQuickmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4597 2023-04-04 15:25:07.113376 PyQt6_WebEngine-6.5.0/sip/QtWebEngineQuick/qquickwebengineprofile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1094 2023-04-04 15:25:07.113842 PyQt6_WebEngine-6.5.0/sip/QtWebEngineQuick/qtwebenginequickglobal.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:25:07.297301 PyQt6_WebEngine-6.5.0/sip/QtWebEngineWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2225 2023-04-04 15:25:07.111832 PyQt6_WebEngine-6.5.0/sip/QtWebEngineWidgets/QtWebEngineWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7637 2023-04-04 15:25:07.111263 PyQt6_WebEngine-6.5.0/sip/QtWebEngineWidgets/qwebengineview.sip
```

### Comparing `PyQt6_WebEngine-6.4.0/ChangeLog` & `PyQt6_WebEngine-6.5.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+2023-03-31  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-WebEngine.msp:
+	Updated for Qt v6.5.0rc.
+	[105702805a7a] [6.5.0]
+
 2022-09-30  Phil Thompson  <phil@riverbankcomputing.com>
 
+	* .hgtags:
+	Added tag 6.4.0 for changeset 1514ce956b1e
+	[0eff8a16b8ef]
+
 	* NEWS:
 	Updated for Qt v6.4.0.
 	[1514ce956b1e] [6.4.0]
 
 2022-09-21  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-WebEngine.msp:
```

### Comparing `PyQt6_WebEngine-6.4.0/LICENSE` & `PyQt6_WebEngine-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_WebEngine-6.4.0/PKG-INFO` & `PyQt6_WebEngine-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-WebEngine
-Version: 6.4.0
+Version: 6.5.0
 Requires-Python: >=3.7
 Summary: Python bindings for the Qt WebEngine framework
 Home-Page: https://www.riverbankcomputing.com/software/pyqtwebengine/
 Author: Riverbank Computing Limited
 Author-Email: info@riverbankcomputing.com
 License: GPL v3
 Requires-Dist: PyQt6 (>=6.2.0)
```

### Comparing `PyQt6_WebEngine-6.4.0/README` & `PyQt6_WebEngine-6.5.0/README`

 * *Files identical despite different names*

### Comparing `PyQt6_WebEngine-6.4.0/pyproject.toml` & `PyQt6_WebEngine-6.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["sip >=6, <7", "PyQt-builder >=1.11, <2"]
 build-backend = "sipbuild.api"
 
 # Specify the PEP 566 metadata for the project.
 [tool.sip.metadata]
 name = "PyQt6-WebEngine"
-version = "6.4.0"
+version = "6.5.0"
 summary = "Python bindings for the Qt WebEngine framework"
 home-page = "https://www.riverbankcomputing.com/software/pyqtwebengine/"
 author = "Riverbank Computing Limited"
 author-email = "info@riverbankcomputing.com"
 license = "GPL v3"
 description-file = "README"
 requires-dist = "PyQt6 (>=6.2.0)"
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/QtWebEngineCoremod.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/QtWebEngineCoremod.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtWebEngineCoremod.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -23,18 +23,18 @@
 %Module(name=PyQt6.QtWebEngineCore, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 %Import QtNetwork/QtNetworkmod.sip
 %Import QtWebChannel/QtWebChannelmod.sip
 
-%Timeline {QtWebEngine_6_0_0 QtWebEngine_6_1_0 QtWebEngine_6_2_0 QtWebEngine_6_3_0 QtWebEngine_6_4_0}
+%Timeline {QtWebEngine_6_0_0 QtWebEngine_6_1_0 QtWebEngine_6_2_0 QtWebEngine_6_3_0 QtWebEngine_6_4_0 QtWebEngine_6_5_0}
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-WebEngine.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -50,16 +50,16 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_WEBENGINE_VERSION;
 const char *PYQT_WEBENGINE_VERSION_STR;
 
 %ModuleCode
-static int PYQT_WEBENGINE_VERSION = 0x060400;
-static const char *PYQT_WEBENGINE_VERSION_STR = "6.4.0";
+static int PYQT_WEBENGINE_VERSION = 0x060500;
+static const char *PYQT_WEBENGINE_VERSION_STR = "6.5.0";
 %End
 
 %Include qtwebenginecoreglobal.sip
 %Include qwebenginecertificateerror.sip
 %Include qwebengineclientcertificateselection.sip
 %Include qwebengineclientcertificatestore.sip
 %Include qwebenginecontextmenurequest.sip
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qtwebenginecoreglobal.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qtwebenginecoreglobal.sip`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtwebenginecoreglobal.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -31,7 +31,10 @@
 %End
 %If (QtWebEngine_6_2_0 -)
 const char *qWebEngineChromiumVersion();
 %End
 %If (QtWebEngine_6_3_0 -)
 const char *qWebEngineChromiumSecurityPatchVersion();
 %End
+%If (QtWebEngine_6_5_0 -)
+const char *qWebEngineProcessName();
+%End
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginecertificateerror.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginecertificateerror.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginecertificateerror.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineclientcertificateselection.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineclientcertificateselection.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineclientcertificateselection.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineclientcertificatestore.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineclientcertificatestore.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineclientcertificatestore.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginecontextmenurequest.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginecontextmenurequest.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginecontextmenurequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginecookiestore.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginecookiestore.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginecookiestore.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginedownloadrequest.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginedownloadrequest.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginedownloadrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginefilesystemaccessrequest.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginefilesystemaccessrequest.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginefilesystemaccessrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginefindtextresult.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginefindtextresult.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginefindtextresult.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginefullscreenrequest.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginefullscreenrequest.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginefullscreenrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginehistory.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginehistory.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginehistory.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginehttprequest.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginehttprequest.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginehttprequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineloadinginfo.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineloadinginfo.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineloadinginfo.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginenavigationrequest.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginenavigationrequest.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginenavigationrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginenewwindowrequest.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginenewwindowrequest.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginenewwindowrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginenotification.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginenotification.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginenotification.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginepage.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginepage.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginepage.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineprofile.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineprofile.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineprofile.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -224,8 +224,15 @@
         
         
             SIP_UNBLOCK_THREADS
         });
         
         Py_END_ALLOW_THREADS
 %End
+
+%If (QtWebEngine_6_5_0 -)
+    bool isPushServiceEnabled() const;
+%End
+%If (QtWebEngine_6_5_0 -)
+    void setPushServiceEnabled(bool enabled);
+%End
 };
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginequotarequest.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginequotarequest.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginequotarequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineregisterprotocolhandlerrequest.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineregisterprotocolhandlerrequest.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineregisterprotocolhandlerrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginescript.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginescript.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginescript.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginescriptcollection.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginescriptcollection.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginescriptcollection.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebenginesettings.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebenginesettings.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginesettings.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlrequestinfo.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlrequestinfo.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlrequestinfo.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -71,12 +71,15 @@
     QUrl requestUrl() const;
     QUrl firstPartyUrl() const;
     QByteArray requestMethod() const;
     void block(bool shouldBlock);
     void redirect(const QUrl &url);
     void setHttpHeader(const QByteArray &name, const QByteArray &value);
     QUrl initiator() const;
+%If (QtWebEngine_6_5_0 -)
+    QHash<QByteArray, QByteArray> httpHeaders() const;
+%End
 
 private:
     QWebEngineUrlRequestInfo();
     ~QWebEngineUrlRequestInfo();
 };
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlrequestinterceptor.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlrequestinterceptor.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlrequestinterceptor.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlrequestjob.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlrequestjob.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlrequestjob.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlscheme.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlscheme.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlscheme.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineCore/qwebengineurlschemehandler.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineCore/qwebengineurlschemehandler.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlschemehandler.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineQuick/QtWebEngineQuickmod.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineQuick/QtWebEngineQuickmod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtWebEngineQuickmod.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineQuick Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 %Module(name=PyQt6.QtWebEngineQuick, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtQml/QtQmlmod.sip
 %Import QtWebEngineCore/QtWebEngineCoremod.sip
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-WebEngine.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineQuick/qquickwebengineprofile.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineQuick/qquickwebengineprofile.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qquickwebengineprofile.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineQuick Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -127,8 +127,21 @@
 %If (PyQt_SSL)
     QWebEngineClientCertificateStore *clientCertificateStore();
 %End
 
 signals:
     void downloadPathChanged();
     void presentNotification(QWebEngineNotification *notification);
+
+public:
+%If (QtWebEngine_6_5_0 -)
+    bool isPushServiceEnabled() const;
+%End
+%If (QtWebEngine_6_5_0 -)
+    void setPushServiceEnabled(bool enable);
+%End
+
+signals:
+%If (QtWebEngine_6_5_0 -)
+    void pushServiceEnabledChanged();
+%End
 };
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineQuick/qtwebenginequickglobal.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineQuick/qtwebenginequickglobal.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtwebenginequickglobal.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineQuick Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineWidgets/QtWebEngineWidgetsmod.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineWidgets/QtWebEngineWidgetsmod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtWebEngineWidgetsmod.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineWidgets Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -25,15 +25,15 @@
 %Import QtCore/QtCoremod.sip
 %Import QtNetwork/QtNetworkmod.sip
 %Import QtPrintSupport/QtPrintSupportmod.sip
 %Import QtWebEngineCore/QtWebEngineCoremod.sip
 %Import QtWidgets/QtWidgetsmod.sip
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-WebEngine.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.4.0/sip/QtWebEngineWidgets/qwebengineview.sip` & `PyQt6_WebEngine-6.5.0/sip/QtWebEngineWidgets/qwebengineview.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineview.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineWidgets Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

