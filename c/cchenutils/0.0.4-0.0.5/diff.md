# Comparing `tmp/cchenutils-0.0.4-py3-none-any.whl.zip` & `tmp/cchenutils-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 121063 bytes, number of entries: 101
+Zip file size: 121079 bytes, number of entries: 101
 -rw-rw-rw-  2.0 fat       83 b- defN 23-Apr-10 09:19 cchenutils/__init__.py
 -rw-rw-rw-  2.0 fat      613 b- defN 23-Mar-31 11:06 cchenutils/dict.py
--rw-rw-rw-  2.0 fat     1900 b- defN 23-Apr-10 09:34 cchenutils/session.py
+-rw-rw-rw-  2.0 fat     1936 b- defN 23-Apr-10 09:39 cchenutils/session.py
 -rw-rw-rw-  2.0 fat      150 b- defN 20-Mar-21 19:46 wanghong/__init__.py
 -rw-rw-rw-  2.0 fat     1372 b- defN 20-Mar-24 05:56 wanghong/async.py
 -rw-rw-rw-  2.0 fat     1347 b- defN 20-Mar-23 22:38 wanghong/dataprep.py
 -rw-rw-rw-  2.0 fat      784 b- defN 20-Apr-06 03:33 wanghong/opts.py
 -rw-rw-rw-  2.0 fat     1717 b- defN 21-Mar-06 19:19 wanghong/test.py
 -rw-rw-rw-  2.0 fat     4258 b- defN 21-Mar-23 02:17 wanghong/utils.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-21 23:45 wanghong/3rdparty/__init__.py
@@ -91,13 +91,13 @@
 -rw-rw-rw-  2.0 fat     3312 b- defN 20-Mar-24 00:35 wanghong/video/prep/wav_split.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/__init__.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/taobao/__init__.py
 -rw-rw-rw-  2.0 fat     4548 b- defN 20-Apr-05 03:47 wanghong/webscraping/taobao/items_cover.py
 -rw-rw-rw-  2.0 fat     4874 b- defN 20-Mar-27 20:44 wanghong/webscraping/taobao/taobao_shopinfo_manual.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/yizhibo/__init__.py
 -rw-rw-rw-  2.0 fat     8389 b- defN 20-Mar-26 19:40 wanghong/webscraping/yizhibo/ts_downbind.py
--rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-10 09:34 cchenutils-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 09:34 cchenutils-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-10 09:34 cchenutils-0.0.4.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.0.4.dist-info/zip-safe
--rw-rw-r--  2.0 fat     8962 b- defN 23-Apr-10 09:34 cchenutils-0.0.4.dist-info/RECORD
-101 files, 345745 bytes uncompressed, 106779 bytes compressed:  69.1%
+-rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-10 09:40 cchenutils-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 09:40 cchenutils-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-10 09:40 cchenutils-0.0.5.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.0.5.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     8962 b- defN 23-Apr-10 09:40 cchenutils-0.0.5.dist-info/RECORD
+101 files, 345781 bytes uncompressed, 106795 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -282,23 +282,23 @@
 
 Filename: wanghong/webscraping/yizhibo/__init__.py
 Comment: 
 
 Filename: wanghong/webscraping/yizhibo/ts_downbind.py
 Comment: 
 
-Filename: cchenutils-0.0.4.dist-info/METADATA
+Filename: cchenutils-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: cchenutils-0.0.4.dist-info/WHEEL
+Filename: cchenutils-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: cchenutils-0.0.4.dist-info/top_level.txt
+Filename: cchenutils-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: cchenutils-0.0.4.dist-info/zip-safe
+Filename: cchenutils-0.0.5.dist-info/zip-safe
 Comment: 
 
-Filename: cchenutils-0.0.4.dist-info/RECORD
+Filename: cchenutils-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cchenutils/session.py

```diff
@@ -1,14 +1,15 @@
 import time
 
 import requests
 from bs4 import BeautifulSoup
 from requests.adapters import HTTPAdapter, Retry
 from requests.exceptions import ConnectionError, ProxyError, JSONDecodeError
 
+from .dict import dict
 
 HEADERS = {
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36'
 }
 
 
 class Session(requests.Session):
@@ -35,18 +36,18 @@
         except (ProxyError, ConnectionError):
             pass
         time.sleep(self.sleep)
         kwargs['_retry'] = kwargs.setdefault('_retry', 0) + 1
         return self.get(url, **kwargs)
 
     def get_json(self, url, **kwargs):
-        return self.get(url, **kwargs).json()
+        return dict(self.get(url, **kwargs).json())
 
     def get_soup(self, url, **kwargs):
         return BeautifulSoup(self.get(url, **kwargs).text, features='lxml')
 
     def get_json_or_soup(self, url, **kwargs):
         r = self.get(url, **kwargs)
         try:
-            return r.json()
+            return dict(r.json())
         except JSONDecodeError:
             return BeautifulSoup(r.text, features='lxml')
```

## Comparing `cchenutils-0.0.4.dist-info/RECORD` & `cchenutils-0.0.5.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cchenutils/__init__.py,sha256=IK9pz6X2d8NS15ctzrl0-Ek_rXrve5dDaN_Ugcw0sGg,83
 cchenutils/dict.py,sha256=IO_6WLY3xZB8huHpwgKCbYEL3d31TllDWdhoSF8Kz6c,613
-cchenutils/session.py,sha256=1aOiFm5ifvQSusgq-GWU6XbJ6x2ddvMFXgel8RS26lo,1900
+cchenutils/session.py,sha256=7k67EyOxZFBhEB4Mr4sj7PS8IZeb5Whiic4de2g540c,1936
 wanghong/__init__.py,sha256=nNr59H3MLTTN-oZoTCUhyOXw0282nv2lzsyom0EbEi0,150
 wanghong/async.py,sha256=5Mb-lTfhRaSYtBHcw4-PT9iV3ohu3aRNaC33okI9Pb8,1372
 wanghong/dataprep.py,sha256=8UEMnrbuPhQ8_ts_HAF9L6FQCj3Rhm3YFjIQFlI5zwY,1347
 wanghong/opts.py,sha256=T5pwfVsmma7B8OKVycfL5ddsapTpvzpNU4bOCtSccNs,784
 wanghong/test.py,sha256=jCN-cUTttNazLmN1tQb1OquGygddmwrsbZ2Gjpej4y0,1717
 wanghong/utils.py,sha256=MgPrC6cJoxon8ooopYx8BvN17GEbAW7TOTPs61RsER0,4258
 wanghong/3rdparty/__init__.py,sha256=7XnItt31RApVDO03DMqxuIVRpnNkhiBmpB8Ue5Nwm-8,152
@@ -90,12 +90,12 @@
 wanghong/video/prep/wav_split.py,sha256=UJ6iKDszpjRtpxGfE_-h_GAa_uT1dXd0ll_7zJ_2Icc,3312
 wanghong/webscraping/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/items_cover.py,sha256=xt1swF6RCnpR0eLJMsuhEkyLqw9M9GGa4BZfoPI-Egs,4548
 wanghong/webscraping/taobao/taobao_shopinfo_manual.py,sha256=wYjqTHCW4NcU8Qy8eLIi-ZpNgsXsNYeXeP7-eyMtVTw,4874
 wanghong/webscraping/yizhibo/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/yizhibo/ts_downbind.py,sha256=u-VOJl_EAsoA4Ep81XdF0GXeSc3Vr1QkmXnLDBca79o,8389
-cchenutils-0.0.4.dist-info/METADATA,sha256=hexaEg2iLNu8V-3xoMU6Qw67afxCODPGzOAbgo4SCAg,196
-cchenutils-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cchenutils-0.0.4.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
-cchenutils-0.0.4.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-cchenutils-0.0.4.dist-info/RECORD,,
+cchenutils-0.0.5.dist-info/METADATA,sha256=YQG5nPD7QMm3NHF_hiyJIJBm-VLOd6Uj8e3K82o7w7I,196
+cchenutils-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cchenutils-0.0.5.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
+cchenutils-0.0.5.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+cchenutils-0.0.5.dist-info/RECORD,,
```

