# Comparing `tmp/essentials_configuration_keyvault-1.0.0.tar.gz` & `tmp/essentials_configuration_keyvault-1.0.1.tar.gz`

## Comparing `essentials_configuration_keyvault-1.0.0.tar` & `essentials_configuration_keyvault-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/MANIFEST.in
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/config/keyvault/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/config/keyvault/py.typed
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/LICENSE
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/README.md
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.1/config/keyvault/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.1/config/keyvault/py.typed
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.1/README.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.1/PKG-INFO
```

### Comparing `essentials_configuration_keyvault-1.0.0/config/keyvault/__init__.py` & `essentials_configuration_keyvault-1.0.1/config/keyvault/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration_keyvault-1.0.0/.gitignore` & `essentials_configuration_keyvault-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `essentials_configuration_keyvault-1.0.0/LICENSE` & `essentials_configuration_keyvault-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `essentials_configuration_keyvault-1.0.0/README.md` & `essentials_configuration_keyvault-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `essentials_configuration_keyvault-1.0.0/pyproject.toml` & `essentials_configuration_keyvault-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "essentials-configuration-keyvault"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ name = "Roberto Prevato", email = "roberto.prevato@gmail.com" }]
 description = "Azure Key Vault source for essentials-configuration."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
@@ -19,29 +19,19 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 keywords = ["Azure Key Vault", "secrets", "configuration", "environment"]
 
 dependencies = ["essentials-configuration~=2.0.0", "azure-identity~=1.12.0", "azure-keyvault-secrets~=4.7.0"]
 
+[tool.hatch.build.targets.wheel]
+packages = ["config"]
+
 [tool.hatch.build.targets.sdist]
-exclude = [
-    "/.github",
-    "/docs",
-    "/deps",
-    "/htmlcov",
-    "/tests",
-    "Makefile",
-    "CODE_OF_CONDUCT.md",
-    ".isort.cfg",
-    ".gitignore",
-    ".flake8",
-    "junit",
-    "requirements.txt",
-    "mypy.ini",
-    "pytest.ini",
-    "venv",
-]
+exclude = ["tests"]
+
+[tool.hatch.build]
+only-packages = true
 
 [project.urls]
 "Homepage" = "https://github.com/Neoteroi/essentials-configuration-keyvault"
 "Bug Tracker" = "https://github.com/Neoteroi/essentials-configuration-keyvault/issues"
```

### Comparing `essentials_configuration_keyvault-1.0.0/PKG-INFO` & `essentials_configuration_keyvault-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: essentials-configuration-keyvault
-Version: 1.0.0
+Version: 1.0.1
 Summary: Azure Key Vault source for essentials-configuration.
 Project-URL: Homepage, https://github.com/Neoteroi/essentials-configuration-keyvault
 Project-URL: Bug Tracker, https://github.com/Neoteroi/essentials-configuration-keyvault/issues
 Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 License-File: LICENSE
 Keywords: Azure Key Vault,configuration,environment,secrets
 Classifier: Development Status :: 5 - Production/Stable
```

