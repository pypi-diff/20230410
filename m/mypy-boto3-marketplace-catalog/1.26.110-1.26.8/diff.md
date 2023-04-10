# Comparing `tmp/mypy-boto3-marketplace-catalog-1.26.110.tar.gz` & `tmp/mypy-boto3-marketplace-catalog-1.26.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-marketplace-catalog-1.26.110.tar", last modified: Mon Apr 10 19:32:48 2023, max compression
+gzip compressed data, was "mypy-boto3-marketplace-catalog-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
```

## Comparing `mypy-boto3-marketplace-catalog-1.26.110.tar` & `mypy-boto3-marketplace-catalog-1.26.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:32:48.684928 mypy-boto3-marketplace-catalog-1.26.110/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-04-10 19:32:48.684928 mypy-boto3-marketplace-catalog-1.26.110/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:32:48.672927 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-04-10 19:32:12.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-04-10 19:32:12.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-10 19:32:12.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-10 19:32:12.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:32:48.684928 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-04-10 19:32:48.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-10 19:32:48.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:32:48.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:32:48.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:32:48.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 19:32:48.000000 mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:32:48.684928 mypy-boto3-marketplace-catalog-1.26.110/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-10 19:32:11.000000 mypy-boto3-marketplace-catalog-1.26.110/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    13287 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11805 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9814 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9799 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7238 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7236 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     8466 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8456 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13287 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/setup.py
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/LICENSE` & `mypy-boto3-marketplace-catalog-1.26.8/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.26.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.26.110
-Summary: Type annotations for boto3.MarketplaceCatalog 1.26.110 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.8
+Summary: Type annotations for boto3.MarketplaceCatalog 1.26.8 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-marketplace-catalog"></a>
 
 # mypy-boto3-marketplace-catalog
 
 [![PyPI - mypy-boto3-marketplace-catalog](https://img.shields.io/pypi/v/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-marketplace-catalog?color=blue)](https://pypistats.org/packages/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.26.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,15 +278,14 @@
 `mypy_boto3_marketplace_catalog.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.literals import (
     ChangeStatusType,
     FailureCodeType,
-    OwnershipTypeType,
     SortOrderType,
     MarketplaceCatalogServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -307,27 +305,23 @@
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
     ErrorDetailTypeDef,
     TagTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CancelChangeSetResponseTypeDef,
     DescribeEntityResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
     StartChangeSetResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
@@ -345,42 +339,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/README.md` & `mypy-boto3-marketplace-catalog-1.26.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-marketplace-catalog"></a>
 
 # mypy-boto3-marketplace-catalog
 
 [![PyPI - mypy-boto3-marketplace-catalog](https://img.shields.io/pypi/v/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-marketplace-catalog?color=blue)](https://pypistats.org/packages/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.26.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -247,15 +247,14 @@
 `mypy_boto3_marketplace_catalog.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.literals import (
     ChangeStatusType,
     FailureCodeType,
-    OwnershipTypeType,
     SortOrderType,
     MarketplaceCatalogServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -275,27 +274,23 @@
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
     ErrorDetailTypeDef,
     TagTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CancelChangeSetResponseTypeDef,
     DescribeEntityResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
     StartChangeSetResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
@@ -313,42 +308,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/__main__.py` & `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceCatalog 1.26.110\nVersion:         1.26.110\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MarketplaceCatalog 1.26.8\nVersion:         1.26.8\nBuilder"
+        " version: 7.11.10\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.110")
+    print("1.26.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/client.py` & `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,20 @@
     client: MarketplaceCatalogClient = session.client("marketplace-catalog")
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import OwnershipTypeType
 from .type_defs import (
     CancelChangeSetResponseTypeDef,
     ChangeTypeDef,
     DescribeChangeSetResponseTypeDef,
     DescribeEntityResponseTypeDef,
     FilterTypeDef,
-    GetResourcePolicyResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SortTypeDef,
     StartChangeSetResponseTypeDef,
     TagTypeDef,
 )
@@ -95,23 +93,14 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#close)
         """
 
-    def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
-        """
-        Deletes a resource-based policy on an Entity that is identified by its resource
-        ARN.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.delete_resource_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#delete_resource_policy)
-        """
-
     def describe_change_set(
         self, *, Catalog: str, ChangeSetId: str
     ) -> DescribeChangeSetResponseTypeDef:
         """
         Provides information about a given change set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.describe_change_set)
@@ -136,23 +125,14 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#generate_presigned_url)
         """
 
-    def get_resource_policy(self, *, ResourceArn: str) -> GetResourcePolicyResponseTypeDef:
-        """
-        Gets a resource-based policy of an Entity that is identified by its resource
-        ARN.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.get_resource_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#get_resource_policy)
-        """
-
     def list_change_sets(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         MaxResults: int = ...,
@@ -170,16 +150,15 @@
         self,
         *,
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...,
-        OwnershipType: OwnershipTypeType = ...
+        MaxResults: int = ...
     ) -> ListEntitiesResponseTypeDef:
         """
         Provides the list of entities of a given type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#list_entities)
         """
@@ -192,22 +171,14 @@
         <https://docs.aws.amazon.com/marketplace-catalog/latest/api-
         reference/welcome.html#working-with-change-se...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#list_tags_for_resource)
         """
 
-    def put_resource_policy(self, *, ResourceArn: str, Policy: str) -> Dict[str, Any]:
-        """
-        Attaches a resource-based policy to an Entity.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.put_resource_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#put_resource_policy)
-        """
-
     def start_change_set(
         self,
         *,
         Catalog: str,
         ChangeSet: Sequence[ChangeTypeDef],
         ChangeSetName: str = ...,
         ClientRequestToken: str = ...,
@@ -221,15 +192,15 @@
         """
 
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tags a resource (either an [entity](https://docs.aws.amazon.com/marketplace-
         catalog/latest/api-reference/welcome.html#catalog-api-entities)_ or [change
         set](https://docs.aws.amazon.com/marketplace-catalog/latest/api-
-        reference/welcome.html#working-with-change-sets)_).
+        reference/welcome.html#working-with-change-sets)_ ).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#tag_resource)
         """
 
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/client.pyi` & `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/client.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,20 @@
     client: MarketplaceCatalogClient = session.client("marketplace-catalog")
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import OwnershipTypeType
 from .type_defs import (
     CancelChangeSetResponseTypeDef,
     ChangeTypeDef,
     DescribeChangeSetResponseTypeDef,
     DescribeEntityResponseTypeDef,
     FilterTypeDef,
-    GetResourcePolicyResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SortTypeDef,
     StartChangeSetResponseTypeDef,
     TagTypeDef,
 )
@@ -88,22 +86,14 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#close)
         """
-    def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
-        """
-        Deletes a resource-based policy on an Entity that is identified by its resource
-        ARN.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.delete_resource_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#delete_resource_policy)
-        """
     def describe_change_set(
         self, *, Catalog: str, ChangeSetId: str
     ) -> DescribeChangeSetResponseTypeDef:
         """
         Provides information about a given change set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.describe_change_set)
@@ -125,22 +115,14 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#generate_presigned_url)
         """
-    def get_resource_policy(self, *, ResourceArn: str) -> GetResourcePolicyResponseTypeDef:
-        """
-        Gets a resource-based policy of an Entity that is identified by its resource
-        ARN.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.get_resource_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#get_resource_policy)
-        """
     def list_change_sets(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         MaxResults: int = ...,
@@ -157,16 +139,15 @@
         self,
         *,
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...,
-        OwnershipType: OwnershipTypeType = ...
+        MaxResults: int = ...
     ) -> ListEntitiesResponseTypeDef:
         """
         Provides the list of entities of a given type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#list_entities)
         """
@@ -177,21 +158,14 @@
         reference/welcome.html#catalog-api-entities)_ or `change set
         <https://docs.aws.amazon.com/marketplace-catalog/latest/api-
         reference/welcome.html#working-with-change-se...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#list_tags_for_resource)
         """
-    def put_resource_policy(self, *, ResourceArn: str, Policy: str) -> Dict[str, Any]:
-        """
-        Attaches a resource-based policy to an Entity.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.put_resource_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#put_resource_policy)
-        """
     def start_change_set(
         self,
         *,
         Catalog: str,
         ChangeSet: Sequence[ChangeTypeDef],
         ChangeSetName: str = ...,
         ClientRequestToken: str = ...,
@@ -204,15 +178,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#start_change_set)
         """
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tags a resource (either an [entity](https://docs.aws.amazon.com/marketplace-
         catalog/latest/api-reference/welcome.html#catalog-api-entities)_ or [change
         set](https://docs.aws.amazon.com/marketplace-catalog/latest/api-
-        reference/welcome.html#working-with-change-sets)_).
+        reference/welcome.html#working-with-change-sets)_ ).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#tag_resource)
         """
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag or list of tags from a resource (either an
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/literals.py` & `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,26 +18,24 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "ChangeStatusType",
     "FailureCodeType",
-    "OwnershipTypeType",
     "SortOrderType",
     "MarketplaceCatalogServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
 ChangeStatusType = Literal["APPLYING", "CANCELLED", "FAILED", "PREPARING", "SUCCEEDED"]
 FailureCodeType = Literal["CLIENT_ERROR", "SERVER_FAULT"]
-OwnershipTypeType = Literal["SELF", "SHARED"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
 MarketplaceCatalogServiceName = Literal["marketplace-catalog"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -56,15 +54,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -74,31 +71,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -127,15 +120,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -180,57 +172,51 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -262,32 +248,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -315,63 +297,56 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/literals.pyi` & `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,23 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ChangeStatusType",
     "FailureCodeType",
-    "OwnershipTypeType",
     "SortOrderType",
     "MarketplaceCatalogServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 ChangeStatusType = Literal["APPLYING", "CANCELLED", "FAILED", "PREPARING", "SUCCEEDED"]
 FailureCodeType = Literal["CLIENT_ERROR", "SERVER_FAULT"]
-OwnershipTypeType = Literal["SELF", "SHARED"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
 MarketplaceCatalogServiceName = Literal["marketplace-catalog"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -54,15 +52,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -72,31 +69,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -125,15 +118,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -178,57 +170,51 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -260,32 +246,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -313,63 +295,56 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/type_defs.py` & `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,42 +10,38 @@
 
     data: CancelChangeSetRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
-from .literals import ChangeStatusType, FailureCodeType, OwnershipTypeType, SortOrderType
+from .literals import ChangeStatusType, FailureCodeType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChangeSetSummaryListItemTypeDef",
     "EntityTypeDef",
     "ErrorDetailTypeDef",
     "TagTypeDef",
-    "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
-    "GetResourcePolicyRequestRequestTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PutResourcePolicyRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CancelChangeSetResponseTypeDef",
     "DescribeEntityResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "StartChangeSetResponseTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
@@ -121,21 +117,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
-    "DeleteResourcePolicyRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-
 DescribeChangeSetRequestRequestTypeDef = TypedDict(
     "DescribeChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
@@ -166,21 +155,14 @@
     {
         "Name": str,
         "ValueList": Sequence[str],
     },
     total=False,
 )
 
-GetResourcePolicyRequestRequestTypeDef = TypedDict(
-    "GetResourcePolicyRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -189,22 +171,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PutResourcePolicyRequestRequestTypeDef = TypedDict(
-    "PutResourcePolicyRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Policy": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -226,22 +200,14 @@
         "EntityArn": str,
         "LastModifiedDate": str,
         "Details": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 StartChangeSetResponseTypeDef = TypedDict(
     "StartChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -350,15 +316,14 @@
 _OptionalListEntitiesRequestRequestTypeDef = TypedDict(
     "_OptionalListEntitiesRequestRequestTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "NextToken": str,
         "MaxResults": int,
-        "OwnershipType": OwnershipTypeType,
     },
     total=False,
 )
 
 
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog/type_defs.pyi` & `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,41 +10,37 @@
 
     data: CancelChangeSetRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
-from .literals import ChangeStatusType, FailureCodeType, OwnershipTypeType, SortOrderType
+from .literals import ChangeStatusType, FailureCodeType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChangeSetSummaryListItemTypeDef",
     "EntityTypeDef",
     "ErrorDetailTypeDef",
     "TagTypeDef",
-    "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
-    "GetResourcePolicyRequestRequestTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PutResourcePolicyRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CancelChangeSetResponseTypeDef",
     "DescribeEntityResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "StartChangeSetResponseTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
@@ -118,21 +114,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
-    "DeleteResourcePolicyRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-
 DescribeChangeSetRequestRequestTypeDef = TypedDict(
     "DescribeChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
@@ -163,21 +152,14 @@
     {
         "Name": str,
         "ValueList": Sequence[str],
     },
     total=False,
 )
 
-GetResourcePolicyRequestRequestTypeDef = TypedDict(
-    "GetResourcePolicyRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -186,22 +168,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PutResourcePolicyRequestRequestTypeDef = TypedDict(
-    "PutResourcePolicyRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Policy": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -223,22 +197,14 @@
         "EntityArn": str,
         "LastModifiedDate": str,
         "Details": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 StartChangeSetResponseTypeDef = TypedDict(
     "StartChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -343,15 +309,14 @@
 _OptionalListEntitiesRequestRequestTypeDef = TypedDict(
     "_OptionalListEntitiesRequestRequestTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "NextToken": str,
         "MaxResults": int,
-        "OwnershipType": OwnershipTypeType,
     },
     total=False,
 )
 
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.26.110
-Summary: Type annotations for boto3.MarketplaceCatalog 1.26.110 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.8
+Summary: Type annotations for boto3.MarketplaceCatalog 1.26.8 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-marketplace-catalog"></a>
 
 # mypy-boto3-marketplace-catalog
 
 [![PyPI - mypy-boto3-marketplace-catalog](https://img.shields.io/pypi/v/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-marketplace-catalog?color=blue)](https://pypistats.org/packages/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.26.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,15 +278,14 @@
 `mypy_boto3_marketplace_catalog.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.literals import (
     ChangeStatusType,
     FailureCodeType,
-    OwnershipTypeType,
     SortOrderType,
     MarketplaceCatalogServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -307,27 +305,23 @@
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
     ErrorDetailTypeDef,
     TagTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CancelChangeSetResponseTypeDef,
     DescribeEntityResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
     StartChangeSetResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
@@ -345,42 +339,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt` & `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.26.110/setup.py` & `mypy-boto3-marketplace-catalog-1.26.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 """
 Setup script for mypy-boto3-marketplace-catalog.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-marketplace-catalog",
-    version="1.26.110",
+    version="1.26.8",
     packages=["mypy_boto3_marketplace_catalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceCatalog 1.26.110 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MarketplaceCatalog 1.26.8 service generated with"
+        " mypy-boto3-builder 7.11.10"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 marketplace-catalog type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_marketplace_catalog": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_marketplace_catalog": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

