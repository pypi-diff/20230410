# Comparing `tmp/ms-dataverse-0.1.3.tar.gz` & `tmp/ms-dataverse-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-dataverse-0.1.3.tar", last modified: Tue Apr  4 13:38:21 2023, max compression
+gzip compressed data, was "ms-dataverse-0.1.4.tar", last modified: Mon Apr 10 12:09:34 2023, max compression
```

## Comparing `ms-dataverse-0.1.3.tar` & `ms-dataverse-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 dennizsvens   (501) staff       (20)        0 2023-04-04 13:38:21.977163 ms-dataverse-0.1.3/
--rw-r--r--   0 dennizsvens   (501) staff       (20)     6114 2023-04-04 13:38:21.977017 ms-dataverse-0.1.3/PKG-INFO
--rw-r--r--   0 dennizsvens   (501) staff       (20)     5140 2023-04-04 13:02:53.000000 ms-dataverse-0.1.3/README.md
-drwxr-xr-x   0 dennizsvens   (501) staff       (20)        0 2023-04-04 13:38:21.976846 ms-dataverse-0.1.3/ms_dataverse.egg-info/
--rw-r--r--   0 dennizsvens   (501) staff       (20)     6114 2023-04-04 13:38:21.000000 ms-dataverse-0.1.3/ms_dataverse.egg-info/PKG-INFO
--rw-r--r--   0 dennizsvens   (501) staff       (20)      197 2023-04-04 13:38:21.000000 ms-dataverse-0.1.3/ms_dataverse.egg-info/SOURCES.txt
--rw-r--r--   0 dennizsvens   (501) staff       (20)        1 2023-04-04 13:38:21.000000 ms-dataverse-0.1.3/ms_dataverse.egg-info/dependency_links.txt
--rw-r--r--   0 dennizsvens   (501) staff       (20)        9 2023-04-04 13:38:21.000000 ms-dataverse-0.1.3/ms_dataverse.egg-info/requires.txt
--rw-r--r--   0 dennizsvens   (501) staff       (20)        1 2023-04-04 13:38:21.000000 ms-dataverse-0.1.3/ms_dataverse.egg-info/top_level.txt
--rw-r--r--   0 dennizsvens   (501) staff       (20)       38 2023-04-04 13:38:21.977199 ms-dataverse-0.1.3/setup.cfg
--rw-r--r--   0 dennizsvens   (501) staff       (20)     1311 2023-04-04 13:34:12.000000 ms-dataverse-0.1.3/setup.py
+drwxr-xr-x   0 dennizsvens   (501) staff       (20)        0 2023-04-10 12:09:34.458112 ms-dataverse-0.1.4/
+-rw-r--r--   0 dennizsvens   (501) staff       (20)     6314 2023-04-10 12:09:34.457901 ms-dataverse-0.1.4/PKG-INFO
+-rw-r--r--   0 dennizsvens   (501) staff       (20)     5340 2023-04-10 12:07:22.000000 ms-dataverse-0.1.4/README.md
+drwxr-xr-x   0 dennizsvens   (501) staff       (20)        0 2023-04-10 12:09:34.457732 ms-dataverse-0.1.4/ms_dataverse.egg-info/
+-rw-r--r--   0 dennizsvens   (501) staff       (20)     6314 2023-04-10 12:09:34.000000 ms-dataverse-0.1.4/ms_dataverse.egg-info/PKG-INFO
+-rw-r--r--   0 dennizsvens   (501) staff       (20)      197 2023-04-10 12:09:34.000000 ms-dataverse-0.1.4/ms_dataverse.egg-info/SOURCES.txt
+-rw-r--r--   0 dennizsvens   (501) staff       (20)        1 2023-04-10 12:09:34.000000 ms-dataverse-0.1.4/ms_dataverse.egg-info/dependency_links.txt
+-rw-r--r--   0 dennizsvens   (501) staff       (20)        9 2023-04-10 12:09:34.000000 ms-dataverse-0.1.4/ms_dataverse.egg-info/requires.txt
+-rw-r--r--   0 dennizsvens   (501) staff       (20)        1 2023-04-10 12:09:34.000000 ms-dataverse-0.1.4/ms_dataverse.egg-info/top_level.txt
+-rw-r--r--   0 dennizsvens   (501) staff       (20)       38 2023-04-10 12:09:34.458149 ms-dataverse-0.1.4/setup.cfg
+-rw-r--r--   0 dennizsvens   (501) staff       (20)     1311 2023-04-10 12:09:26.000000 ms-dataverse-0.1.4/setup.py
```

### Comparing `ms-dataverse-0.1.3/PKG-INFO` & `ms-dataverse-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-dataverse
-Version: 0.1.3
+Version: 0.1.4
 Summary: DataverseORM is a Python module that simplifies working with Microsoft Dataverse by providing a lightweight Object-Relational Mapper (ORM) for querying, creating, updating, and deleting entities. It uses the Dataverse Web API for communication and includes optional metadata validation to ensure that entities and properties exist in the connected Dataverse environment.
 Home-page: https://github.com/DennizSvens/ms-dataverse
 Author: Denniz Svens
 Author-email: denniz@liminity.se
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # DataverseORM
-DataverseORM is a Python module that simplifies working with Microsoft Dataverse by providing a lightweight Object-Relational Mapper (ORM) for querying, creating, updating, and deleting entities. It uses the Dataverse Web API for communication and includes optional metadata validation to ensure that entities and properties exist in the connected Dataverse environment.
+DataverseORM is a Python module that simplifies working with Microsoft Dataverse by providing a lightweight Object-Relational Mapper (ORM) for querying, creating, updating, and deleting entities. It uses the Dataverse Web API for communication. 
 
 ## Installation
 ```
 pip install ms-dataverse
 ```
 
 ## Dependencies
@@ -43,22 +43,28 @@
 ## Authentication
 You can obtain an access token using the MSAL Python package available at:
 https://github.com/AzureAD/microsoft-authentication-library-for-python
 
 Both `PublicClientApplication` and `ConfidentialClientApplication` classes work effectively with this package and the Dataverse Web API.
 
 
-## Fetching metadata
-If you want to enable metadata validation (recommended during development), pass metadata_validation=True when creating an instance of DataverseORM:
+## Refresh token callback
+The refresh_token_callback parameter is an optional function that you can provide to handle token expiration. When the access token expires, the callback function will be called automatically to refresh the token. The callback function should return a new access token. To use the refresh_token_callback, pass it when creating an instance of DataverseORM:
 
 ``` python
-orm = DataverseORM(dynamics_url="https://your_environment.crm.dynamics.com", access_token="your_access_token", metadata_validation=True)
+
+def refresh_access_token():
+    # Your token refresh logic here
+    return new_access_token
+
+orm = DataverseORM(dynamics_url="https://your_environment.crm.dynamics.com", access_token="your_access_token", refresh_token_callback=refresh_access_token)
+
 ```
 
-Metadata validation verifies the existence of entities and properties prior to issuing API requests, which results in improved error handling and messaging.
+By providing a refresh_token_callback, you can ensure seamless operation of the DataverseORM instance, even when the access token expires during its usage.
 
 ## Working with entities
 To work with a specific entity, get an instance of the Entity class:
 
 ``` python
 account = orm.entity("accounts")
 ```
```

### Comparing `ms-dataverse-0.1.3/README.md` & `ms-dataverse-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DataverseORM
-DataverseORM is a Python module that simplifies working with Microsoft Dataverse by providing a lightweight Object-Relational Mapper (ORM) for querying, creating, updating, and deleting entities. It uses the Dataverse Web API for communication and includes optional metadata validation to ensure that entities and properties exist in the connected Dataverse environment.
+DataverseORM is a Python module that simplifies working with Microsoft Dataverse by providing a lightweight Object-Relational Mapper (ORM) for querying, creating, updating, and deleting entities. It uses the Dataverse Web API for communication. 
 
 ## Installation
 ```
 pip install ms-dataverse
 ```
 
 ## Dependencies
@@ -26,22 +26,28 @@
 ## Authentication
 You can obtain an access token using the MSAL Python package available at:
 https://github.com/AzureAD/microsoft-authentication-library-for-python
 
 Both `PublicClientApplication` and `ConfidentialClientApplication` classes work effectively with this package and the Dataverse Web API.
 
 
-## Fetching metadata
-If you want to enable metadata validation (recommended during development), pass metadata_validation=True when creating an instance of DataverseORM:
+## Refresh token callback
+The refresh_token_callback parameter is an optional function that you can provide to handle token expiration. When the access token expires, the callback function will be called automatically to refresh the token. The callback function should return a new access token. To use the refresh_token_callback, pass it when creating an instance of DataverseORM:
 
 ``` python
-orm = DataverseORM(dynamics_url="https://your_environment.crm.dynamics.com", access_token="your_access_token", metadata_validation=True)
+
+def refresh_access_token():
+    # Your token refresh logic here
+    return new_access_token
+
+orm = DataverseORM(dynamics_url="https://your_environment.crm.dynamics.com", access_token="your_access_token", refresh_token_callback=refresh_access_token)
+
 ```
 
-Metadata validation verifies the existence of entities and properties prior to issuing API requests, which results in improved error handling and messaging.
+By providing a refresh_token_callback, you can ensure seamless operation of the DataverseORM instance, even when the access token expires during its usage.
 
 ## Working with entities
 To work with a specific entity, get an instance of the Entity class:
 
 ``` python
 account = orm.entity("accounts")
 ```
```

### Comparing `ms-dataverse-0.1.3/ms_dataverse.egg-info/PKG-INFO` & `ms-dataverse-0.1.4/ms_dataverse.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-dataverse
-Version: 0.1.3
+Version: 0.1.4
 Summary: DataverseORM is a Python module that simplifies working with Microsoft Dataverse by providing a lightweight Object-Relational Mapper (ORM) for querying, creating, updating, and deleting entities. It uses the Dataverse Web API for communication and includes optional metadata validation to ensure that entities and properties exist in the connected Dataverse environment.
 Home-page: https://github.com/DennizSvens/ms-dataverse
 Author: Denniz Svens
 Author-email: denniz@liminity.se
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # DataverseORM
-DataverseORM is a Python module that simplifies working with Microsoft Dataverse by providing a lightweight Object-Relational Mapper (ORM) for querying, creating, updating, and deleting entities. It uses the Dataverse Web API for communication and includes optional metadata validation to ensure that entities and properties exist in the connected Dataverse environment.
+DataverseORM is a Python module that simplifies working with Microsoft Dataverse by providing a lightweight Object-Relational Mapper (ORM) for querying, creating, updating, and deleting entities. It uses the Dataverse Web API for communication. 
 
 ## Installation
 ```
 pip install ms-dataverse
 ```
 
 ## Dependencies
@@ -43,22 +43,28 @@
 ## Authentication
 You can obtain an access token using the MSAL Python package available at:
 https://github.com/AzureAD/microsoft-authentication-library-for-python
 
 Both `PublicClientApplication` and `ConfidentialClientApplication` classes work effectively with this package and the Dataverse Web API.
 
 
-## Fetching metadata
-If you want to enable metadata validation (recommended during development), pass metadata_validation=True when creating an instance of DataverseORM:
+## Refresh token callback
+The refresh_token_callback parameter is an optional function that you can provide to handle token expiration. When the access token expires, the callback function will be called automatically to refresh the token. The callback function should return a new access token. To use the refresh_token_callback, pass it when creating an instance of DataverseORM:
 
 ``` python
-orm = DataverseORM(dynamics_url="https://your_environment.crm.dynamics.com", access_token="your_access_token", metadata_validation=True)
+
+def refresh_access_token():
+    # Your token refresh logic here
+    return new_access_token
+
+orm = DataverseORM(dynamics_url="https://your_environment.crm.dynamics.com", access_token="your_access_token", refresh_token_callback=refresh_access_token)
+
 ```
 
-Metadata validation verifies the existence of entities and properties prior to issuing API requests, which results in improved error handling and messaging.
+By providing a refresh_token_callback, you can ensure seamless operation of the DataverseORM instance, even when the access token expires during its usage.
 
 ## Working with entities
 To work with a specific entity, get an instance of the Entity class:
 
 ``` python
 account = orm.entity("accounts")
 ```
```

### Comparing `ms-dataverse-0.1.3/setup.py` & `ms-dataverse-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ms-dataverse",
-    version="0.1.3",
+    version="0.1.4",
     description="DataverseORM is a Python module that simplifies working with Microsoft Dataverse by providing a lightweight Object-Relational Mapper (ORM) for querying, creating, updating, and deleting entities. It uses the Dataverse Web API for communication and includes optional metadata validation to ensure that entities and properties exist in the connected Dataverse environment.",
     author="Denniz Svens",
     author_email="denniz@liminity.se",
     url="https://github.com/DennizSvens/ms-dataverse",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

