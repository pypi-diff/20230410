# Comparing `tmp/dcentralab_qa_infra_automation-0.0.7.tar.gz` & `tmp/dcentralab_qa_infra_automation-0.0.8.tar.gz`

## Comparing `dcentralab_qa_infra_automation-0.0.7.tar` & `dcentralab_qa_infra_automation-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.0.8/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-0.0.7/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.0.8/.idea/workspace.xml`

 * *Files 9% similar despite different names*

#### Comparing `dcentralab_qa_infra_automation-0.0.7/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.0.8/.idea/workspace.xml`

```diff
@@ -2,14 +2,16 @@
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="ce720036-d8eb-462b-9d8d-e560b75fc3e8" name="Changes" comment="change package name">
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/__init__.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/Loggers.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/Loggers.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/seleniumPythonFramework_VeriSoft/__init__.py" beforeDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
```

### Comparing `dcentralab_qa_infra_automation-0.0.7/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-0.0.8/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,26 +6,63 @@
 init brave browser driver
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 
-def initBraveDriver():
+def addBraveToChrome():
     """
-    init brave driver, using ChromeDriverManager for chromeDriver installation
-    :return: driver - driver instance
+    add brave to chrome based on OS type
+    :return: binary_location
     """
-    option = webdriver.ChromeOptions()
-
+    binary_location = None
     # On macOS - use mac brave path
     if pytest.data_driven.get("OS") == "windows":
-        option.binary_location = pytest.properties.get("brave.windows.path")
+        binary_location = pytest.properties.get("brave.windows.path")
     # On windowsOS - use windows brave path
     elif pytest.data_driven.get("OS") == "mac":
-        option.binary_location = pytest.properties.get("brave.mac.path")
+        binary_location = pytest.properties.get("brave.mac.path")
     # If no OS injected
     else:
         pytest.logger.info("no OS type injected, brave did not add to chrome.")
 
-    driver = webdriver.Chrome(ChromeDriverManager().install(), options=option)
+    return binary_location
+
+
+def addExtensionToChrome():
+    """
+    add CRX extension to chrome
+    :return: add_extension - current extension crx file
+    """
+    add_extension = None
+    # In metamask wallet type
+    if pytest.data_driven.get("wallet_type") == 'MetaMask':
+        add_extension = pytest.user_dir + pytest.properties.get("metamask.extension.crx")
+    elif pytest.data_driven.get("wallet_type") == 'Coinbase':
+        add_extension = pytest.user_dir + pytest.properties.get("coinbase.extension.crx")
+
+    return add_extension
+
+
+def initBraveDriver():
+    """
+    init brave driver, using ChromeDriverManager for chromeDriver installation
+    :return: driver - driver instance
+    """
+    options = webdriver.ChromeOptions()
+    options.binary_location = addBraveToChrome()
+
+    driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
+    return driver
+
+
+def initBraveDriverWithExtension():
+    """
+    init brave driver with CRX extension, using ChromeDriverManager for chromeDriver installation
+    :return: driver - driver instance
+    """
+    options = webdriver.ChromeOptions()
+    options.binary_location = addBraveToChrome()
+    options.add_extension(addExtensionToChrome())
+    driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
     return driver
```

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,7 +14,14 @@
     """
     init chrome driver, using ChromeDriverManager for chromeDriver installation
     :return: driver - driver instance
     """
     pytest.logger.info("chrome driver type injected, initialize chrome browser")
     driver = webdriver.Chrome(ChromeDriverManager().install())
     return driver
+
+
+def initChromeDriverWithExtension():
+    """
+    init chrome driver with CRX extension, using ChromeDriverManager for chromeDriver installation
+    :return: driver - driver instance
+    """
```

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-0.0.8/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/LICENSE` & `dcentralab_qa_infra_automation-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.0.7/pyproject.toml` & `dcentralab_qa_infra_automation-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-0.0.7/PKG-INFO` & `dcentralab_qa_infra_automation-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 0.0.7
+Version: 0.0.8
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

