# Comparing `tmp/Kekik-1.2.4.tar.gz` & `tmp/Kekik-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kekik-1.2.4.tar", last modified: Sun Apr  2 15:35:30 2023, max compression
+gzip compressed data, was "Kekik-1.2.5.tar", last modified: Mon Apr 10 14:50:35 2023, max compression
```

## Comparing `Kekik-1.2.4.tar` & `Kekik-1.2.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:35:30.783941 Kekik-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:35:30.775941 Kekik-1.2.4/Kekik/
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/Nesne.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/csv2dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/dict2csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/dict2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/dosya2set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/dosya_indir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/hwid_kontrol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:35:30.783941 Kekik-1.2.4/Kekik/kisi_ver/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/kisi_ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189486 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/kisi_ver/biyografiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    88066 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/kisi_ver/isimler.py
--rw-r--r--   0 runner    (1001) docker     (123)    78485 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/kisi_ver/soyisimler.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/link_islemleri.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/list2html.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/liste_fetis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/mail_gonder.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/okunabilir_byte.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/proxy_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/qr_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/ses_fetis.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/slugify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/txt_fetis.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-02 15:35:08.000000 Kekik-1.2.4/Kekik/zaman_donustur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:35:30.775941 Kekik-1.2.4/Kekik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-02 15:35:30.000000 Kekik-1.2.4/Kekik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-02 15:35:30.000000 Kekik-1.2.4/Kekik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 15:35:30.000000 Kekik-1.2.4/Kekik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-02 15:35:30.000000 Kekik-1.2.4/Kekik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-02 15:35:30.000000 Kekik-1.2.4/Kekik.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-02 15:35:08.000000 Kekik-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-02 15:35:08.000000 Kekik-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-02 15:35:30.783941 Kekik-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-02 15:35:08.000000 Kekik-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 15:35:30.783941 Kekik-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-02 15:35:08.000000 Kekik-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:50:35.174618 Kekik-1.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:50:35.170618 Kekik-1.2.5/Kekik/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/BIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/Nesne.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/csv2dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/dict2csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/dict2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/dosya2set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/dosya_indir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/hwid_kontrol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:50:35.174618 Kekik-1.2.5/Kekik/kisi_ver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/kisi_ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189486 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/kisi_ver/biyografiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88066 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/kisi_ver/isimler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78485 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/kisi_ver/soyisimler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/link_islemleri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/list2html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/liste_fetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/mail_gonder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/okunabilir_byte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/proxy_ver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/qr_ver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/ses_fetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/slugify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/txt_fetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-10 14:50:15.000000 Kekik-1.2.5/Kekik/zaman_donustur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:50:35.170618 Kekik-1.2.5/Kekik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-04-10 14:50:35.000000 Kekik-1.2.5/Kekik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 14:50:35.000000 Kekik-1.2.5/Kekik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:50:35.000000 Kekik-1.2.5/Kekik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-10 14:50:35.000000 Kekik-1.2.5/Kekik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 14:50:35.000000 Kekik-1.2.5/Kekik.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 14:50:15.000000 Kekik-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 14:50:15.000000 Kekik-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-04-10 14:50:35.174618 Kekik-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-04-10 14:50:15.000000 Kekik-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 14:50:35.174618 Kekik-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-10 14:50:15.000000 Kekik-1.2.5/setup.py
```

### Comparing `Kekik-1.2.4/Kekik/Nesne.py` & `Kekik-1.2.5/Kekik/Nesne.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/__init__.py` & `Kekik-1.2.5/Kekik/__init__.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/cli.py` & `Kekik-1.2.5/Kekik/cli.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/dict2csv.py` & `Kekik-1.2.5/Kekik/dict2csv.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/dict2json.py` & `Kekik-1.2.5/Kekik/dict2json.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/dosya_indir.py` & `Kekik-1.2.5/Kekik/dosya_indir.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/hwid_kontrol.py` & `Kekik-1.2.5/Kekik/hwid_kontrol.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/kisi_ver/__init__.py` & `Kekik-1.2.5/Kekik/kisi_ver/__init__.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/kisi_ver/biyografiler.py` & `Kekik-1.2.5/Kekik/kisi_ver/biyografiler.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/kisi_ver/isimler.py` & `Kekik-1.2.5/Kekik/kisi_ver/isimler.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/kisi_ver/soyisimler.py` & `Kekik-1.2.5/Kekik/kisi_ver/soyisimler.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/link_islemleri.py` & `Kekik-1.2.5/Kekik/link_islemleri.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/list2html.py` & `Kekik-1.2.5/Kekik/list2html.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/mail_gonder.py` & `Kekik-1.2.5/Kekik/mail_gonder.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/okunabilir_byte.py` & `Kekik-1.2.5/Kekik/okunabilir_byte.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/proxy_ver.py` & `Kekik-1.2.5/Kekik/proxy_ver.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/qr_ver.py` & `Kekik-1.2.5/Kekik/qr_ver.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/ses_fetis.py` & `Kekik-1.2.5/Kekik/ses_fetis.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/slugify.py` & `Kekik-1.2.5/Kekik/slugify.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/txt_fetis.py` & `Kekik-1.2.5/Kekik/txt_fetis.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik/zaman_donustur.py` & `Kekik-1.2.5/Kekik/zaman_donustur.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/Kekik.egg-info/PKG-INFO` & `Kekik-1.2.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: Kekik
-Version: 1.2.4
-Summary: İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..
-Home-page: https://github.com/keyiflerolsun/Kekik
-Author: keyiflerolsun
-Author-email: keyiflerolsun@gmail.com
-License: GPLv3+
-Keywords: Kekik,KekikAkademi,keyiflerolsun
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # <img src="https://www.akashtrehan.com/assets/images/emoji/terminal.png" height="42" align="center"> Kekik
 
 ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/Kekik?logo=git&logoColor=white)
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/Kekik&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 ![Python Version](https://img.shields.io/pypi/pyversions/Kekik?logo=python&logoColor=white)
@@ -199,14 +183,25 @@
 liste_fetis.n_adete_bol(liste, adet=3)
 # [[1, 4, 7, 10], [2, 5, 8], [3, 6, 9]]
 
 liste_fetis.n_er_hale_getir(liste, adet=3)
 # [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10]]
 ```
 
+### **[BIST](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/BIST.py)**
+```python
+from Kekik import BIST
+
+print(BIST.marketler)
+# {'XU100': ['AEFES', 'AGHOL', 'AKBNK', 'AKFGY', 'AKSA', 'AKSEN', 'ALARK', 'ALBRK', 'ALFAS', 'ALKIM', 'ARCLK', 'ASELS', 'ASUZU', 'AYDEM', 'BAGFS', 'BASGZ', 'BERA', 'BIMAS', 'BIOEN', 'BRYAT', 'BUCIM', 'CCOLA', 'CEMTS', 'CIMSA', 'DOAS', 'DOHOL', 'ECILC', 'EGEEN', 'EKGYO', 'ENJSA', 'ENKAI', 'ERBOS', 'EREGL', 'EUREN', 'FENER', 'FROTO', 'GARAN', 'GENIL', 'GESAN', 'GLYHO', 'GSDHO', 'GUBRF', 'GWIND', 'HALKB', 'HEKTS', 'IPEKE', 'ISCTR', 'ISDMR', 'ISGYO', 'IZMDC', 'KARSN', 'KCAER', 'KCHOL', 'KERVT', 'KLRHO', 'KMPUR', 'KONTR', 'KONYA', 'KORDS', 'KOZAA', 'KOZAL', 'KRDMD', 'KZBGY', 'MAVI', 'MGROS', 'ODAS', 'OTKAR', 'OYAKC', 'PETKM', 'PGSUS', 'PSGYO', 'SAHOL', 'SASA', 'SELEC', 'SISE', 'SKBNK', 'SMRTG', 'SNGYO', 'SOKM', 'TAVHL', 'TCELL', 'THYAO', 'TKFEN', 'TKNSA', 'TMSN', 'TOASO', 'TSKB', 'TTKOM', 'TTRAK', 'TUKAS', 'TUPRS', 'TURSG', 'ULKER', 'ULUUN', 'VAKBN', 'VESBE', 'VESTL', 'YKBNK', 'YYLGD', 'ZOREN'], 'XU050': ['AEFES', 'AKBNK', 'AKSA', 'AKSEN', 'ALARK', 'ARCLK', 'ASELS', 'BERA', 'BIMAS', 'DOHOL', 'EGEEN', 'EKGYO', 'ENJSA', 'ENKAI', 'EREGL', 'FROTO', 'GARAN', 'GESAN', 'GUBRF', 'HALKB', 'HEKTS', 'ISCTR', 'ISGYO', 'KCHOL', 'KONTR', 'KORDS', 'KOZAA', 'KOZAL', 'KRDMD', 'MGROS', 'ODAS', 'OYAKC', 'PETKM', 'PGSUS', 'SAHOL', 'SASA', 'SISE', 'SMRTG', 'SOKM', 'TAVHL', 'TCELL', 'THYAO', 'TKFEN', 'TOASO', 'TSKB', 'TTKOM', 'TUPRS', 'VAKBN', 'VESTL', 'YKBNK'], 'XU030': ['AKBNK', 'AKSEN', 'ALARK', 'ARCLK', 'ASELS', 'BIMAS', 'EKGYO', 'ENKAI', 'EREGL', 'FROTO', 'GARAN', 'GUBRF', 'HEKTS', 'ISCTR', 'KCHOL', 'KOZAA', 'KOZAL', 'KRDMD', 'ODAS', 'PETKM', 'PGSUS', 'SAHOL', 'SASA', 'SISE', 'TAVHL', 'TCELL', 'THYAO', 'TOASO', 'TUPRS', 'YKBNK']}
+
+print(BIST.sembol_sorgu("VESBE"))
+# {'VESBE': ['XU100']}
+```
+
 ### **[dict2json](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/dict2json.py)**
 ### **[dosya_indir](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/dosya_indir.py)**
 ### **[benim_hwid](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/hwid_kontrol.py)**
 ### **[hwid_kontrol](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/hwid_kontrol.py)**
 ### **[satir_ekle](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)**
 ### **[satirlar_ekle](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)**
 ### **[satir_sil](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)**
@@ -224,8 +219,8 @@
 
 ## ♻️ İletişim
 
 *Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ##
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,17 +1,9 @@
-Metadata-Version: 2.1 Name: Kekik Version: 1.2.4 Summary: Ä°Ålerimizi
-kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda durduÄu kÃ¼tÃ¼phane.. Home-page:
-https://github.com/keyiflerolsun/Kekik Author: keyiflerolsun Author-email:
-keyiflerolsun@gmail.com License: GPLv3+ Keywords:
-Kekik,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
-Production/Stable Classifier: License :: OSI Approved :: GNU General Public
-License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE # [https://www.akashtrehan.com/assets/images/emoji/terminal.png] Kekik
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/
+# [https://www.akashtrehan.com/assets/images/emoji/terminal.png] Kekik ![Repo
+Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/
 Kekik?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/
 api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/
 Kekik&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/âï¸-Kahve
 Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/pyversions/
 Kekik?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
 Kekik?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
 Kekik?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
@@ -86,26 +78,51 @@
 import Nesne nesne = Nesne({"Merhaba": "DÃ¼nya"}) print(nesne) # Nesne
 (Merhaba=DÃ¼nya) nesne.gorsel(girinti=0, kademe=1) ''' Nesne( Merhaba=... ) '''
 print(nesne.Merhaba) # DÃ¼nya ``` ### **[liste_fetis](https://github.com/
 keyiflerolsun/Kekik/blob/main/Kekik/liste_fetis.py)** ```python from Kekik
 import liste_fetis liste = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
 liste_fetis.n_adete_bol(liste, adet=3) # [[1, 4, 7, 10], [2, 5, 8], [3, 6, 9]]
 liste_fetis.n_er_hale_getir(liste, adet=3) # [[1, 2, 3], [4, 5, 6], [7, 8, 9],
-[10]] ``` ### **[dict2json](https://github.com/keyiflerolsun/Kekik/blob/main/
-Kekik/dict2json.py)** ### **[dosya_indir](https://github.com/keyiflerolsun/
-Kekik/blob/main/Kekik/dosya_indir.py)** ### **[benim_hwid](https://github.com/
-keyiflerolsun/Kekik/blob/main/Kekik/hwid_kontrol.py)** ### **[hwid_kontrol]
-(https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/hwid_kontrol.py)** ###
-**[satir_ekle](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
-txt_fetis.py)** ### **[satirlar_ekle](https://github.com/keyiflerolsun/Kekik/
-blob/main/Kekik/txt_fetis.py)** ### **[satir_sil](https://github.com/
-keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)** ### **[list2html](https://
-github.com/keyiflerolsun/Kekik/blob/main/Kekik/list2html.py)** ### **
-[mail_gonder](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
-mail_gonder.py)** ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://
-KekikAkademi.org/Kahve)** ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2022
-by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/Kekik/
-blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸
-Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj
-gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## > **
-[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+[10]] ``` ### **[BIST](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
+BIST.py)** ```python from Kekik import BIST print(BIST.marketler) # {'XU100':
+['AEFES', 'AGHOL', 'AKBNK', 'AKFGY', 'AKSA', 'AKSEN', 'ALARK', 'ALBRK',
+'ALFAS', 'ALKIM', 'ARCLK', 'ASELS', 'ASUZU', 'AYDEM', 'BAGFS', 'BASGZ', 'BERA',
+'BIMAS', 'BIOEN', 'BRYAT', 'BUCIM', 'CCOLA', 'CEMTS', 'CIMSA', 'DOAS', 'DOHOL',
+'ECILC', 'EGEEN', 'EKGYO', 'ENJSA', 'ENKAI', 'ERBOS', 'EREGL', 'EUREN',
+'FENER', 'FROTO', 'GARAN', 'GENIL', 'GESAN', 'GLYHO', 'GSDHO', 'GUBRF',
+'GWIND', 'HALKB', 'HEKTS', 'IPEKE', 'ISCTR', 'ISDMR', 'ISGYO', 'IZMDC',
+'KARSN', 'KCAER', 'KCHOL', 'KERVT', 'KLRHO', 'KMPUR', 'KONTR', 'KONYA',
+'KORDS', 'KOZAA', 'KOZAL', 'KRDMD', 'KZBGY', 'MAVI', 'MGROS', 'ODAS', 'OTKAR',
+'OYAKC', 'PETKM', 'PGSUS', 'PSGYO', 'SAHOL', 'SASA', 'SELEC', 'SISE', 'SKBNK',
+'SMRTG', 'SNGYO', 'SOKM', 'TAVHL', 'TCELL', 'THYAO', 'TKFEN', 'TKNSA', 'TMSN',
+'TOASO', 'TSKB', 'TTKOM', 'TTRAK', 'TUKAS', 'TUPRS', 'TURSG', 'ULKER', 'ULUUN',
+'VAKBN', 'VESBE', 'VESTL', 'YKBNK', 'YYLGD', 'ZOREN'], 'XU050': ['AEFES',
+'AKBNK', 'AKSA', 'AKSEN', 'ALARK', 'ARCLK', 'ASELS', 'BERA', 'BIMAS', 'DOHOL',
+'EGEEN', 'EKGYO', 'ENJSA', 'ENKAI', 'EREGL', 'FROTO', 'GARAN', 'GESAN',
+'GUBRF', 'HALKB', 'HEKTS', 'ISCTR', 'ISGYO', 'KCHOL', 'KONTR', 'KORDS',
+'KOZAA', 'KOZAL', 'KRDMD', 'MGROS', 'ODAS', 'OYAKC', 'PETKM', 'PGSUS', 'SAHOL',
+'SASA', 'SISE', 'SMRTG', 'SOKM', 'TAVHL', 'TCELL', 'THYAO', 'TKFEN', 'TOASO',
+'TSKB', 'TTKOM', 'TUPRS', 'VAKBN', 'VESTL', 'YKBNK'], 'XU030': ['AKBNK',
+'AKSEN', 'ALARK', 'ARCLK', 'ASELS', 'BIMAS', 'EKGYO', 'ENKAI', 'EREGL',
+'FROTO', 'GARAN', 'GUBRF', 'HEKTS', 'ISCTR', 'KCHOL', 'KOZAA', 'KOZAL',
+'KRDMD', 'ODAS', 'PETKM', 'PGSUS', 'SAHOL', 'SASA', 'SISE', 'TAVHL', 'TCELL',
+'THYAO', 'TOASO', 'TUPRS', 'YKBNK']} print(BIST.sembol_sorgu("VESBE")) #
+{'VESBE': ['XU100']} ``` ### **[dict2json](https://github.com/keyiflerolsun/
+Kekik/blob/main/Kekik/dict2json.py)** ### **[dosya_indir](https://github.com/
+keyiflerolsun/Kekik/blob/main/Kekik/dosya_indir.py)** ### **[benim_hwid](https:
+//github.com/keyiflerolsun/Kekik/blob/main/Kekik/hwid_kontrol.py)** ### **
+[hwid_kontrol](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
+hwid_kontrol.py)** ### **[satir_ekle](https://github.com/keyiflerolsun/Kekik/
+blob/main/Kekik/txt_fetis.py)** ### **[satirlar_ekle](https://github.com/
+keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)** ### **[satir_sil](https://
+github.com/keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)** ### **
+[list2html](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
+list2html.py)** ### **[mail_gonder](https://github.com/keyiflerolsun/Kekik/
+blob/main/Kekik/mail_gonder.py)** ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla]
+(https://KekikAkademi.org/Kahve)** ## ð Telif HakkÄ± ve Lisans * *Copyright
+(C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
+GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
+keyiflerolsun/Kekik/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
+lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
+isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
+(https://t.me/KekikKahve) ## > **[@KekikAkademi](https://t.me/KekikAkademi)**
+*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `Kekik-1.2.4/Kekik.egg-info/SOURCES.txt` & `Kekik-1.2.5/Kekik.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+Kekik/BIST.py
 Kekik/Nesne.py
 Kekik/__init__.py
 Kekik/cli.py
 Kekik/csv2dict.py
 Kekik/dict2csv.py
 Kekik/dict2json.py
 Kekik/dosya2set.py
```

### Comparing `Kekik-1.2.4/LICENSE` & `Kekik-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.4/setup.py` & `Kekik-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     packages     = ["Kekik"],
 
     name         = "Kekik",
-    version      = "1.2.4",
+    version      = "1.2.5",
     url          = "https://github.com/keyiflerolsun/Kekik",
     description  = "İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..",
     keywords     = ["Kekik", "KekikAkademi", "keyiflerolsun"],
 
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True,
```

