# Comparing `tmp/kat_bulgaria-0.6.1.tar.gz` & `tmp/kat_bulgaria-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kat_bulgaria-0.6.1.tar", last modified: Mon Apr 10 17:31:10 2023, max compression
+gzip compressed data, was "kat_bulgaria-0.6.2.tar", last modified: Mon Apr 10 17:58:39 2023, max compression
```

## Comparing `kat_bulgaria-0.6.1.tar` & `kat_bulgaria-0.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:31:10.052554 kat_bulgaria-0.6.1/kat_bulgaria/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/kat_bulgaria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/kat_bulgaria/obligations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/tests/test_obligations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:58:39.788977 kat_bulgaria-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-10 17:58:39.788977 kat_bulgaria-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-10 17:58:23.000000 kat_bulgaria-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:58:39.784977 kat_bulgaria-0.6.2/kat_bulgaria/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 17:58:23.000000 kat_bulgaria-0.6.2/kat_bulgaria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-04-10 17:58:23.000000 kat_bulgaria-0.6.2/kat_bulgaria/obligations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:58:39.788977 kat_bulgaria-0.6.2/kat_bulgaria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-10 17:58:39.000000 kat_bulgaria-0.6.2/kat_bulgaria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 17:58:39.000000 kat_bulgaria-0.6.2/kat_bulgaria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:58:39.000000 kat_bulgaria-0.6.2/kat_bulgaria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 17:58:39.000000 kat_bulgaria-0.6.2/kat_bulgaria.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 17:58:39.000000 kat_bulgaria-0.6.2/kat_bulgaria.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:58:39.788977 kat_bulgaria-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-10 17:58:23.000000 kat_bulgaria-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:58:39.788977 kat_bulgaria-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-10 17:58:23.000000 kat_bulgaria-0.6.2/tests/test_obligations.py
```

### Comparing `kat_bulgaria-0.6.1/PKG-INFO` & `kat_bulgaria-0.6.2/kat_bulgaria.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kat_bulgaria
-Version: 0.6.1
+Name: kat-bulgaria
+Version: 0.6.2
 Summary: A library to check for existing obligations to KAT Bulgaria
 Home-page: https://github.com/Nedevski/py_kat_bulgaria
 Author: Nikola Nedevski
 Author-email: nikola.nedevski@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `kat_bulgaria-0.6.1/README.md` & `kat_bulgaria-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `kat_bulgaria-0.6.1/kat_bulgaria/obligations.py` & `kat_bulgaria-0.6.2/kat_bulgaria/obligations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Obligations module"""
 
-import array
 from dataclasses import dataclass
 from enum import Enum
 from typing import Generic, TypeVar
 
 import re
 import httpx
 
@@ -40,14 +39,46 @@
     VALIDATION_ERROR = 1
     API_UNAVAILABLE = 2
     TIMEOUT = 3
 
 
 # endregion
 
+# region ----- Data types
+
+
+class KatObligation:
+    """Obligation model."""
+
+    description: str
+    document_number: str
+    person_name: str
+    person_identifier: str
+    date_created: str
+    date_served: str
+    amount: float
+    discount: int
+
+    def __init__(self, obligation: any):
+        """Parse the data."""
+        self.description = obligation["paymentReason"]
+        self.document_number = obligation["additionalData"]["documentNumber"]
+
+        self.person_name = obligation["obligedPersonName"]
+        self.person_identifier = obligation["obligedPersonIdent"]
+
+        self.date_created = obligation["additionalData"]["fishCreateDate"]
+        self.date_served = obligation["obligationDate"]
+
+        self.amount = float(obligation["amount"])
+        self.discount = int(obligation["additionalData"]["discount"])
+
+
+# endregion
+
 # region ----- Responses
 
 
 @dataclass
 class KatObligationsSimpleResponse:
     """The obligations response object."""
 
@@ -59,39 +90,26 @@
 
 @dataclass
 class KatObligationsResponse:
     """The obligations response object."""
 
     has_non_handed_slip: bool
     has_obligations: bool
-    obligations: array.array
+    obligations: list[KatObligation]
 
     def __init__(self, data: any) -> None:
         self.obligations = []
         self.has_non_handed_slip = data[_RESP_HAS_NON_HANDED_SLIP]
         self.has_obligations = (
             data[_RESP_HAS_NON_HANDED_SLIP] or len(data[_RESP_OBLIGATIONS]) > 0
         )
 
         if len(data[_RESP_OBLIGATIONS]) > 0:
             for obligation in data[_RESP_OBLIGATIONS]:
-                self.obligations.append(
-                    {
-                        "amount": obligation["amount"],
-                        "description": obligation["paymentReason"],
-                        "documentNumber": obligation["additionalData"][
-                            "documentNumber"
-                        ],
-                        "date_created": obligation["additionalData"]["fishCreateDate"],
-                        "date_served": obligation["obligationDate"],
-                        "person_name": obligation["obligedPersonName"],
-                        "person_identifier": obligation["obligedPersonIdent"],
-                        "discount": obligation["additionalData"]["discount"],
-                    }
-                )
+                self.obligations.append(KatObligation(obligation))
 
 
 T = TypeVar("T", KatObligationsResponse, KatObligationsSimpleResponse, bool)
 
 
 @dataclass
 class KatApiResponse(Generic[T]):
```

### Comparing `kat_bulgaria-0.6.1/kat_bulgaria.egg-info/PKG-INFO` & `kat_bulgaria-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kat-bulgaria
-Version: 0.6.1
+Name: kat_bulgaria
+Version: 0.6.2
 Summary: A library to check for existing obligations to KAT Bulgaria
 Home-page: https://github.com/Nedevski/py_kat_bulgaria
 Author: Nikola Nedevski
 Author-email: nikola.nedevski@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `kat_bulgaria-0.6.1/setup.py` & `kat_bulgaria-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from setuptools import find_packages, setup
 
 long_description = Path("README.md").read_text("utf-8")
 
 setup(
     name="kat_bulgaria",
-    version="0.6.1",
+    version="0.6.2",
     description="A library to check for existing obligations to KAT Bulgaria",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nedevski/py_kat_bulgaria",
     author="Nikola Nedevski",
     author_email="nikola.nedevski@gmail.com",
     license="MIT",
```

### Comparing `kat_bulgaria-0.6.1/tests/test_obligations.py` & `kat_bulgaria-0.6.2/tests/test_obligations.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     KatErrorType,
 )
 
 from .conftest import EGN, LICENSE, INVALID_EGN, INVALID_LICENSE
 
 
 # region verify_credentials
+
+
 @pytest.mark.asyncio
 async def test_verify_credentials(
     httpx_mock: HTTPXMock, s200_no_obligations: pytest.fixture
 ) -> None:
     """Verify credentials - success."""
 
     httpx_mock.add_response(json=s200_no_obligations)
@@ -299,19 +301,28 @@
     assert len(httpx_mock.get_requests()) == 1
     assert resp.success is True
 
     assert resp.data.has_obligations is True
     assert resp.data.has_non_handed_slip is False
     assert len(resp.data.obligations) == 1
 
+    oblig = resp.data.obligations[0]
+    assert oblig.description == "НП 22-1085-002609 14.10.2022"
+    assert oblig.document_number == "22-1085-002609"
+    assert oblig.person_name == "ИМЕ ПРЕЗИМЕ ФАМИЛИЯ"
+    assert oblig.person_identifier == "1234567890"
+    assert oblig.date_created == "2022-10-14"
+    assert oblig.date_served == "2023-04-06T00:00:00"
+    assert oblig.amount == 100.0
+    assert oblig.discount == 20
+
     assert not resp.error_message
     assert not resp.error_type
 
 
-
 @pytest.mark.asyncio
 async def test_get_obligations_invalid_egn(httpx_mock: HTTPXMock) -> None:
     """Get obligations - local EGN validation failed."""
 
     resp = await KatApi().async_get_obligations(INVALID_EGN, LICENSE)
 
     assert len(httpx_mock.get_requests()) == 0
@@ -329,14 +340,15 @@
 
     assert len(httpx_mock.get_requests()) == 0
     assert resp.success is False
     assert resp.data is None
     assert resp.error_message == ERR_INVALID_LICENSE
     assert resp.error_type is KatErrorType.VALIDATION_ERROR
 
+
 @pytest.mark.asyncio
 async def test_get_obligations_api_invalid_data_sent(
     httpx_mock: HTTPXMock, s400_invalid_user_details: pytest.fixture
 ) -> None:
     """Get obligations - remote KAT API validation failed."""
 
     httpx_mock.add_response(json=s400_invalid_user_details, status_code=400)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

