# Comparing `tmp/kat_bulgaria-0.6.0.tar.gz` & `tmp/kat_bulgaria-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kat_bulgaria-0.6.0.tar", last modified: Mon Apr 10 17:04:04 2023, max compression
+gzip compressed data, was "kat_bulgaria-0.6.1.tar", last modified: Mon Apr 10 17:31:10 2023, max compression
```

## Comparing `kat_bulgaria-0.6.0.tar` & `kat_bulgaria-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:04.461662 kat_bulgaria-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-10 17:04:04.461662 kat_bulgaria-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-10 17:03:51.000000 kat_bulgaria-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:04.461662 kat_bulgaria-0.6.0/kat_bulgaria/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 17:03:51.000000 kat_bulgaria-0.6.0/kat_bulgaria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-10 17:03:51.000000 kat_bulgaria-0.6.0/kat_bulgaria/obligations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:04.461662 kat_bulgaria-0.6.0/kat_bulgaria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-10 17:04:04.000000 kat_bulgaria-0.6.0/kat_bulgaria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 17:04:04.000000 kat_bulgaria-0.6.0/kat_bulgaria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:04:04.000000 kat_bulgaria-0.6.0/kat_bulgaria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 17:04:04.000000 kat_bulgaria-0.6.0/kat_bulgaria.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 17:04:04.000000 kat_bulgaria-0.6.0/kat_bulgaria.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:04:04.461662 kat_bulgaria-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-10 17:03:51.000000 kat_bulgaria-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:04.461662 kat_bulgaria-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-04-10 17:03:51.000000 kat_bulgaria-0.6.0/tests/test_obligations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:31:10.052554 kat_bulgaria-0.6.1/kat_bulgaria/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/kat_bulgaria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/kat_bulgaria/obligations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 17:31:10.000000 kat_bulgaria-0.6.1/kat_bulgaria.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:31:10.056554 kat_bulgaria-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-04-10 17:30:55.000000 kat_bulgaria-0.6.1/tests/test_obligations.py
```

### Comparing `kat_bulgaria-0.6.0/PKG-INFO` & `kat_bulgaria-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kat_bulgaria
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library to check for existing obligations to KAT Bulgaria
 Home-page: https://github.com/Nedevski/py_kat_bulgaria
 Author: Nikola Nedevski
 Author-email: nikola.nedevski@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `kat_bulgaria-0.6.0/README.md` & `kat_bulgaria-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `kat_bulgaria-0.6.0/kat_bulgaria/obligations.py` & `kat_bulgaria-0.6.1/kat_bulgaria/obligations.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,71 +145,75 @@
 
 class KatApi:
     """KAT API manager"""
 
     def __init__(self):
         """Constructor"""
 
-    async def async_verify_credentials(
-        self, egn: str, license_number: str
-    ) -> KatApiResponse[bool]:
-        """Confirm that the credentials are correct."""
+    def __validate_credentials(self, egn: str, license_number: str) -> str | None:
+        """Validate EGN/License locally."""
 
+        # Validate EGN
         if egn is None:
-            return KatApiResponse(
-                None,
-                f"{_ERR_PREFIX} EGN is missing or emtpy",
-                KatErrorType.VALIDATION_ERROR,
-            )
+            return f"{_ERR_PREFIX} EGN is missing or emtpy"
         else:
             egn_match = re.search(REGEX_EGN, egn)
             if egn_match is None:
-                return KatApiResponse(
-                    None,
-                    ERR_INVALID_EGN,
-                    KatErrorType.VALIDATION_ERROR,
-                )
+                return ERR_INVALID_EGN
 
+        # Validate License Number
         if license_number is None:
-            return KatApiResponse(
-                None,
-                f"{_ERR_PREFIX} Driving License Number missing",
-                KatErrorType.VALIDATION_ERROR,
-            )
+            return f"{_ERR_PREFIX} Driving License Number missing"
         else:
             license_match = re.search(REGEX_DRIVING_LICENSE, license_number)
             if license_match is None:
-                return KatApiResponse(
-                    None,
-                    ERR_INVALID_LICENSE,
-                    KatErrorType.VALIDATION_ERROR,
-                )
+                return ERR_INVALID_LICENSE
+
+        # If everything is valid - return None
+        return None
+
+    async def async_verify_credentials(
+        self, egn: str, license_number: str
+    ) -> KatApiResponse[bool]:
+        """Confirm that the credentials are correct."""
+
+        validation_msg = self.__validate_credentials(egn, license_number)
+        if validation_msg is not None:
+            return KatApiResponse(None, validation_msg, KatErrorType.VALIDATION_ERROR)
 
         res = await self.__get_obligations_request(egn, license_number)
 
         return KatApiResponse(res.success, res.error_message, res.error_type)
 
     async def async_check_obligations(
         self, egn: str, license_number: str
     ) -> KatApiResponse[bool]:
         """Check if the person has obligations"""
 
+        validation_msg = self.__validate_credentials(egn, license_number)
+        if validation_msg is not None:
+            return KatApiResponse(None, validation_msg, KatErrorType.VALIDATION_ERROR)
+
         res = await self.__get_obligations_request(egn, license_number)
 
         if res.success:
             has_obligations = KatObligationsSimpleResponse(res.raw_data).has_obligations
             return KatApiResponse(has_obligations)
         else:
             return KatApiResponse(None, res.error_message, res.error_type)
 
     async def async_get_obligations(
         self, egn: str, license_number: str
     ) -> KatApiResponse[KatObligationsResponse]:
         """Get all obligations"""
 
+        validation_msg = self.__validate_credentials(egn, license_number)
+        if validation_msg is not None:
+            return KatApiResponse(None, validation_msg, KatErrorType.VALIDATION_ERROR)
+
         res = await self.__get_obligations_request(egn, license_number)
 
         if res.success:
             return KatApiResponse(KatObligationsResponse(res.raw_data))
         else:
             return KatApiResponse(None, res.error_message, res.error_type)
```

### Comparing `kat_bulgaria-0.6.0/kat_bulgaria.egg-info/PKG-INFO` & `kat_bulgaria-0.6.1/kat_bulgaria.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kat-bulgaria
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library to check for existing obligations to KAT Bulgaria
 Home-page: https://github.com/Nedevski/py_kat_bulgaria
 Author: Nikola Nedevski
 Author-email: nikola.nedevski@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `kat_bulgaria-0.6.0/setup.py` & `kat_bulgaria-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from setuptools import find_packages, setup
 
 long_description = Path("README.md").read_text("utf-8")
 
 setup(
     name="kat_bulgaria",
-    version="0.6.0",
+    version="0.6.1",
     description="A library to check for existing obligations to KAT Bulgaria",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nedevski/py_kat_bulgaria",
     author="Nikola Nedevski",
     author_email="nikola.nedevski@gmail.com",
     license="MIT",
```

### Comparing `kat_bulgaria-0.6.0/tests/test_obligations.py` & `kat_bulgaria-0.6.1/tests/test_obligations.py`

 * *Files 12% similar despite different names*

```diff
@@ -161,14 +161,40 @@
     assert resp.success is True
     assert resp.data is True
     assert not resp.error_message
     assert not resp.error_type
 
 
 @pytest.mark.asyncio
+async def test_check_obligations_invalid_egn(httpx_mock: HTTPXMock) -> None:
+    """Check obligations - local EGN validation failed."""
+
+    resp = await KatApi().async_check_obligations(INVALID_EGN, LICENSE)
+
+    assert len(httpx_mock.get_requests()) == 0
+    assert resp.success is False
+    assert resp.data is None
+    assert resp.error_message == ERR_INVALID_EGN
+    assert resp.error_type is KatErrorType.VALIDATION_ERROR
+
+
+@pytest.mark.asyncio
+async def test_check_obligations_invalid_driver_license(httpx_mock: HTTPXMock) -> None:
+    """Check obligations - local Driver License validation failed."""
+
+    resp = await KatApi().async_check_obligations(EGN, INVALID_LICENSE)
+
+    assert len(httpx_mock.get_requests()) == 0
+    assert resp.success is False
+    assert resp.data is None
+    assert resp.error_message == ERR_INVALID_LICENSE
+    assert resp.error_type is KatErrorType.VALIDATION_ERROR
+
+
+@pytest.mark.asyncio
 async def test_check_obligations_api_invalid_data_sent(
     httpx_mock: HTTPXMock, s400_invalid_user_details: pytest.fixture
 ) -> None:
     """Check obligations - remote KAT API validation failed."""
 
     httpx_mock.add_response(json=s400_invalid_user_details, status_code=400)
 
@@ -277,14 +303,40 @@
     assert resp.data.has_non_handed_slip is False
     assert len(resp.data.obligations) == 1
 
     assert not resp.error_message
     assert not resp.error_type
 
 
+
+@pytest.mark.asyncio
+async def test_get_obligations_invalid_egn(httpx_mock: HTTPXMock) -> None:
+    """Get obligations - local EGN validation failed."""
+
+    resp = await KatApi().async_get_obligations(INVALID_EGN, LICENSE)
+
+    assert len(httpx_mock.get_requests()) == 0
+    assert resp.success is False
+    assert resp.data is None
+    assert resp.error_message == ERR_INVALID_EGN
+    assert resp.error_type is KatErrorType.VALIDATION_ERROR
+
+
+@pytest.mark.asyncio
+async def test_get_obligations_invalid_driver_license(httpx_mock: HTTPXMock) -> None:
+    """Get obligations - local Driver License validation failed."""
+
+    resp = await KatApi().async_get_obligations(EGN, INVALID_LICENSE)
+
+    assert len(httpx_mock.get_requests()) == 0
+    assert resp.success is False
+    assert resp.data is None
+    assert resp.error_message == ERR_INVALID_LICENSE
+    assert resp.error_type is KatErrorType.VALIDATION_ERROR
+
 @pytest.mark.asyncio
 async def test_get_obligations_api_invalid_data_sent(
     httpx_mock: HTTPXMock, s400_invalid_user_details: pytest.fixture
 ) -> None:
     """Get obligations - remote KAT API validation failed."""
 
     httpx_mock.add_response(json=s400_invalid_user_details, status_code=400)
```

