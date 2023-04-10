# Comparing `tmp/aiosmartpost-0.4.0b1-py3-none-any.whl.zip` & `tmp/aiosmartpost-0.4.0b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8699 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       82 b- defN 23-Apr-03 18:28 smartpost/__init__.py
--rw-rw-r--  2.0 unx     6088 b- defN 23-Apr-03 18:38 smartpost/client.py
+Zip file size: 8681 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       82 b- defN 23-Apr-10 19:06 smartpost/__init__.py
+-rw-rw-r--  2.0 unx     6000 b- defN 23-Apr-10 19:06 smartpost/client.py
 -rw-rw-r--  2.0 unx     2435 b- defN 23-Apr-03 18:31 smartpost/errors.py
 -rw-rw-r--  2.0 unx     4639 b- defN 23-Apr-03 18:35 smartpost/models.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-28 17:14 smartpost/py.typed
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-28 17:14 smartpost/sync/__init__.py
 -rw-rw-r--  2.0 unx     1211 b- defN 23-Apr-03 18:25 smartpost/sync/client.py
--rw-rw-r--  2.0 unx     1210 b- defN 23-Apr-03 19:25 aiosmartpost-0.4.0b1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2751 b- defN 23-Apr-03 19:25 aiosmartpost-0.4.0b1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-03 19:25 aiosmartpost-0.4.0b1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Apr-03 19:25 aiosmartpost-0.4.0b1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      958 b- defN 23-Apr-03 19:25 aiosmartpost-0.4.0b1.dist-info/RECORD
-12 files, 19476 bytes uncompressed, 7085 bytes compressed:  63.6%
+-rw-rw-r--  2.0 unx     1210 b- defN 23-Apr-10 19:08 aiosmartpost-0.4.0b2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2751 b- defN 23-Apr-10 19:08 aiosmartpost-0.4.0b2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-10 19:08 aiosmartpost-0.4.0b2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Apr-10 19:08 aiosmartpost-0.4.0b2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      958 b- defN 23-Apr-10 19:08 aiosmartpost-0.4.0b2.dist-info/RECORD
+12 files, 19388 bytes uncompressed, 7067 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: smartpost/sync/__init__.py
 Comment: 
 
 Filename: smartpost/sync/client.py
 Comment: 
 
-Filename: aiosmartpost-0.4.0b1.dist-info/LICENSE
+Filename: aiosmartpost-0.4.0b2.dist-info/LICENSE
 Comment: 
 
-Filename: aiosmartpost-0.4.0b1.dist-info/METADATA
+Filename: aiosmartpost-0.4.0b2.dist-info/METADATA
 Comment: 
 
-Filename: aiosmartpost-0.4.0b1.dist-info/WHEEL
+Filename: aiosmartpost-0.4.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: aiosmartpost-0.4.0b1.dist-info/top_level.txt
+Filename: aiosmartpost-0.4.0b2.dist-info/top_level.txt
 Comment: 
 
-Filename: aiosmartpost-0.4.0b1.dist-info/RECORD
+Filename: aiosmartpost-0.4.0b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smartpost/__init__.py

```diff
@@ -1,4 +1,4 @@
 from smartpost.client import Client
 
-__version__ = "0.4.0b1"
+__version__ = "0.4.0b2"
 __all__ = ["Client"]
```

## smartpost/client.py

```diff
@@ -135,19 +135,17 @@
                 key: value for key, value in asdict(order).items() if value is not None
             }
             request_data["orders"]["item"].append(order_dict)
 
         response = await self.post("/api/ext/v1/orders", dict(request_data))
         if response.status_code == 400:
             errors = response.json()
-            print(errors)
             raise ShipmentOrderError(errors["error"])
 
         data = response.json()
-        print(data)
         orders: list[SmartPostOrder] = data["orders"]["item"]
         return [Order(**order) for order in orders]
 
     async def get_labels_pdf(
         self,
         format: Literal["A5", "A6", "A6-4", "A7", "A7-8"],
         barcodes: list[str],
@@ -167,12 +165,11 @@
 
         Raises:
             httpx.ReadTimeout:
                 SmartPost API did not manage to send PDF file in time.
         """
         response = await self.get("/api/ext/v1/labels", format=format, barcode=barcodes)
         data = response.read()
-        print(data)
         if response.status_code != 200:
-            raise ShipmentLabelsError(response.read(), response.status_code)
+            raise ShipmentLabelsError(data, response.status_code)
 
-        return response.read()
+        return data
```

## Comparing `aiosmartpost-0.4.0b1.dist-info/LICENSE` & `aiosmartpost-0.4.0b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiosmartpost-0.4.0b1.dist-info/METADATA` & `aiosmartpost-0.4.0b2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosmartpost
-Version: 0.4.0b1
+Version: 0.4.0b2
 Summary: Itella SmartPost API wrapper for humans 📦
 Home-page: https://github.com/HarrySky/aiosmartpost
 Author: Igor Nehoroshev
 Author-email: mail@neigor.me
 License: Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

