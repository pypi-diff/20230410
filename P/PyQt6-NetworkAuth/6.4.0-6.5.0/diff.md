# Comparing `tmp/PyQt6_NetworkAuth-6.4.0.tar.gz` & `tmp/PyQt6_NetworkAuth-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_NetworkAuth-6.4.0.tar", last modified: Fri Sep 30 10:27:36 2022, max compression
+gzip compressed data, was "PyQt6_NetworkAuth-6.5.0.tar", last modified: Tue Apr  4 15:22:32 2023, max compression
```

## Comparing `PyQt6_NetworkAuth-6.4.0.tar` & `PyQt6_NetworkAuth-6.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:36.387956 PyQt6_NetworkAuth-6.4.0/
--rw-r--r--   0 phil       (501) staff       (20)     4959 2022-09-30 10:27:35.982809 PyQt6_NetworkAuth-6.4.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2022-09-30 10:27:35.814360 PyQt6_NetworkAuth-6.4.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      632 2022-09-30 10:27:13.518021 PyQt6_NetworkAuth-6.4.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1663 2022-09-30 10:27:36.388119 PyQt6_NetworkAuth-6.4.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1315 2022-09-30 10:27:35.983784 PyQt6_NetworkAuth-6.4.0/README
--rw-r--r--   0 phil       (501) staff       (20)      852 2022-09-30 10:27:35.984094 PyQt6_NetworkAuth-6.4.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:36.384194 PyQt6_NetworkAuth-6.4.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:36.387632 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/
--rw-r--r--   0 phil       (501) staff       (20)     2568 2022-09-30 10:27:36.218673 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/QtNetworkAuthmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     8253 2022-09-30 10:27:36.216273 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qabstractoauth.sip
--rw-r--r--   0 phil       (501) staff       (20)     3446 2022-09-30 10:27:36.217362 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qabstractoauth2.sip
--rw-r--r--   0 phil       (501) staff       (20)     1567 2022-09-30 10:27:36.217801 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qabstractoauthreplyhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     4170 2022-09-30 10:27:36.214278 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauth1.sip
--rw-r--r--   0 phil       (501) staff       (20)     2829 2022-09-30 10:27:36.214989 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauth1signature.sip
--rw-r--r--   0 phil       (501) staff       (20)     2386 2022-09-30 10:27:36.216742 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauth2authorizationcodeflow.sip
--rw-r--r--   0 phil       (501) staff       (20)     1967 2022-09-30 10:27:36.219128 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauthhttpserverreplyhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1289 2022-09-30 10:27:36.218198 PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauthoobreplyhandler.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:32.880464 PyQt6_NetworkAuth-6.5.0/
+-rw-r--r--   0 phil       (501) staff       (20)     5173 2023-04-04 15:22:32.448360 PyQt6_NetworkAuth-6.5.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2023-04-04 15:22:32.243611 PyQt6_NetworkAuth-6.5.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      687 2023-04-04 15:22:08.530599 PyQt6_NetworkAuth-6.5.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1663 2023-04-04 15:22:32.880674 PyQt6_NetworkAuth-6.5.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1315 2023-04-04 15:22:32.449422 PyQt6_NetworkAuth-6.5.0/README
+-rw-r--r--   0 phil       (501) staff       (20)      852 2023-04-04 15:22:32.449808 PyQt6_NetworkAuth-6.5.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:32.877121 PyQt6_NetworkAuth-6.5.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:32.880180 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/
+-rw-r--r--   0 phil       (501) staff       (20)     2588 2023-04-04 15:22:32.706021 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/QtNetworkAuthmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8253 2023-04-04 15:22:32.703235 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qabstractoauth.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3807 2023-04-04 15:22:32.704513 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qabstractoauth2.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1567 2023-04-04 15:22:32.705016 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qabstractoauthreplyhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4170 2023-04-04 15:22:32.701069 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauth1.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2829 2023-04-04 15:22:32.701762 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauth1signature.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2386 2023-04-04 15:22:32.703782 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauth2authorizationcodeflow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1967 2023-04-04 15:22:32.706535 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauthhttpserverreplyhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1289 2023-04-04 15:22:32.705491 PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauthoobreplyhandler.sip
```

### Comparing `PyQt6_NetworkAuth-6.4.0/ChangeLog` & `PyQt6_NetworkAuth-6.5.0/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+2023-03-31  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-NetworkAuth.msp:
+	Updated for Qt v6.5.0rc.
+	[b75be9d64045] [6.5.0]
+
 2022-09-30  Phil Thompson  <phil@riverbankcomputing.com>
 
+	* .hgtags:
+	Added tag 6.4.0 for changeset 7e49c36be25b
+	[9a95e3488eff]
+
 	* NEWS:
 	Updated for Qt v6.4.0.
 	[7e49c36be25b] [6.4.0]
 
 2022-09-21  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-NetworkAuth.msp:
```

### Comparing `PyQt6_NetworkAuth-6.4.0/LICENSE` & `PyQt6_NetworkAuth-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_NetworkAuth-6.4.0/NEWS` & `PyQt6_NetworkAuth-6.5.0/NEWS`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+v6.5.0 31st March 2023
+  - Added support for Qt v6.5.
+
 v6.4.0 30th September 2022
   - Added support for Qt v6.4.
 
 v6.3.0 31st March 2022
   - Added support for Qt v6.3.
 
 v6.2.0 30th September 2021
```

### Comparing `PyQt6_NetworkAuth-6.4.0/PKG-INFO` & `PyQt6_NetworkAuth-6.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-NetworkAuth
-Version: 6.4.0
+Version: 6.5.0
 Requires-Python: >=3.7
 Summary: Python bindings for the Qt Network Authorization library
 Home-Page: https://www.riverbankcomputing.com/software/pyqtnetworkauth/
 Author: Riverbank Computing Limited
 Author-Email: info@riverbankcomputing.com
 License: GPL v3
 Requires-Dist: PyQt6 (>=6.2.0)
```

### Comparing `PyQt6_NetworkAuth-6.4.0/README` & `PyQt6_NetworkAuth-6.5.0/README`

 * *Files identical despite different names*

### Comparing `PyQt6_NetworkAuth-6.4.0/pyproject.toml` & `PyQt6_NetworkAuth-6.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["sip >=6, <7", "PyQt-builder >=1.9, <2"]
 build-backend = "sipbuild.api"
 
 # Specify the PEP 566 metadata for the project.
 [tool.sip.metadata]
 name = "PyQt6-NetworkAuth"
-version = "6.4.0"
+version = "6.5.0"
 summary = "Python bindings for the Qt Network Authorization library"
 home-page = "https://www.riverbankcomputing.com/software/pyqtnetworkauth/"
 author = "Riverbank Computing Limited"
 author-email = "info@riverbankcomputing.com"
 license = "GPL v3"
 description-file = "README"
 requires-dist = "PyQt6 (>=6.2.0)"
```

### Comparing `PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/QtNetworkAuthmod.sip` & `PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/QtNetworkAuthmod.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtNetworkAuthmod.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -21,18 +21,18 @@
 
 
 %Module(name=PyQt6.QtNetworkAuth, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtCore/QtCoremod.sip
 %Import QtNetwork/QtNetworkmod.sip
 
-%Timeline {QtNetworkAuth_6_0_0 QtNetworkAuth_6_1_0 QtNetworkAuth_6_2_0 QtNetworkAuth_6_3_0 QtNetworkAuth_6_4_0}
+%Timeline {QtNetworkAuth_6_0_0 QtNetworkAuth_6_1_0 QtNetworkAuth_6_2_0 QtNetworkAuth_6_3_0 QtNetworkAuth_6_4_0 QtNetworkAuth_6_5_0}
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-NetworkAuth.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -48,16 +48,16 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_NETWORKAUTH_VERSION;
 const char *PYQT_NETWORKAUTH_VERSION_STR;
 
 %ModuleCode
-static int PYQT_NETWORKAUTH_VERSION = 0x060400;
-static const char *PYQT_NETWORKAUTH_VERSION_STR = "6.4.0";
+static int PYQT_NETWORKAUTH_VERSION = 0x060500;
+static const char *PYQT_NETWORKAUTH_VERSION_STR = "6.5.0";
 %End
 
 %Include qabstractoauth.sip
 %Include qabstractoauth2.sip
 %Include qabstractoauthreplyhandler.sip
 %Include qoauth1.sip
 %Include qoauth1signature.sip
```

### Comparing `PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qabstractoauth.sip` & `PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qabstractoauth.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractoauth.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qabstractoauth2.sip` & `PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qabstractoauth2.sip`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractoauth2.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -65,8 +65,25 @@
 
 public:
     virtual QNetworkReply *post(const QUrl &url, const QByteArray &data);
     virtual QNetworkReply *post(const QUrl &url, QHttpMultiPart *multiPart);
     virtual QNetworkReply *put(const QUrl &url, const QByteArray &data);
     virtual QNetworkReply *put(const QUrl &url, QHttpMultiPart *multiPart);
     virtual void prepareRequest(QNetworkRequest *request, const QByteArray &verb, const QByteArray &body = QByteArray());
+%If (QtNetworkAuth_6_5_0 -)
+%If (PyQt_SSL)
+    QSslConfiguration sslConfiguration() const;
+%End
+%End
+%If (QtNetworkAuth_6_5_0 -)
+%If (PyQt_SSL)
+    void setSslConfiguration(const QSslConfiguration &configuration);
+%End
+%End
+
+signals:
+%If (QtNetworkAuth_6_5_0 -)
+%If (PyQt_SSL)
+    void sslConfigurationChanged(const QSslConfiguration &configuration);
+%End
+%End
 };
```

### Comparing `PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qabstractoauthreplyhandler.sip` & `PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qabstractoauthreplyhandler.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractoauthreplyhandler.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauth1.sip` & `PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauth1.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauth1.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauth1signature.sip` & `PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauth1signature.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauth1signature.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauth2authorizationcodeflow.sip` & `PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauth2authorizationcodeflow.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauth2authorizationcodeflow.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauthhttpserverreplyhandler.sip` & `PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauthhttpserverreplyhandler.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauthhttpserverreplyhandler.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_NetworkAuth-6.4.0/sip/QtNetworkAuth/qoauthoobreplyhandler.sip` & `PyQt6_NetworkAuth-6.5.0/sip/QtNetworkAuth/qoauthoobreplyhandler.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauthoobreplyhandler.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

