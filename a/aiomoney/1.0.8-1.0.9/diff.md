# Comparing `tmp/aiomoney-1.0.8.tar.gz` & `tmp/aiomoney-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomoney-1.0.8.tar", last modified: Fri Mar 10 07:12:21 2023, max compression
+gzip compressed data, was "aiomoney-1.0.9.tar", last modified: Fri Mar 10 07:22:28 2023, max compression
```

## Comparing `aiomoney-1.0.8.tar` & `aiomoney-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 07:12:21.504238 aiomoney-1.0.8/
--rw-rw-rw-   0        0        0     3809 2023-03-10 07:12:21.504238 aiomoney-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3238 2023-03-10 06:47:08.000000 aiomoney-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-10 07:12:21.504238 aiomoney-1.0.8/aiomoney/
--rw-rw-rw-   0        0        0       78 2023-03-10 04:38:35.000000 aiomoney-1.0.8/aiomoney/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-03-09 14:31:45.000000 aiomoney-1.0.8/aiomoney/authorization.py
--rw-rw-rw-   0        0        0       96 2023-03-09 14:24:49.000000 aiomoney-1.0.8/aiomoney/exceptions.py
--rw-rw-rw-   0        0        0     1559 2023-03-10 04:18:32.000000 aiomoney-1.0.8/aiomoney/request.py
-drwxrwxrwx   0        0        0        0 2023-03-10 07:12:21.504238 aiomoney-1.0.8/aiomoney/types/
--rw-rw-rw-   0        0        0      179 2023-03-10 04:07:21.000000 aiomoney-1.0.8/aiomoney/types/__init__.py
--rw-rw-rw-   0        0        0      823 2023-03-10 03:51:21.000000 aiomoney-1.0.8/aiomoney/types/account_info.py
--rw-rw-rw-   0        0        0      821 2023-03-10 03:55:47.000000 aiomoney-1.0.8/aiomoney/types/operation_details.py
--rw-rw-rw-   0        0        0      574 2023-03-10 03:52:58.000000 aiomoney-1.0.8/aiomoney/types/operation_history.py
--rw-rw-rw-   0        0        0      261 2023-03-10 04:06:54.000000 aiomoney-1.0.8/aiomoney/types/payment.py
--rw-rw-rw-   0        0        0     3452 2023-03-10 05:11:11.000000 aiomoney-1.0.8/aiomoney/wallet.py
-drwxrwxrwx   0        0        0        0 2023-03-10 07:12:21.504238 aiomoney-1.0.8/aiomoney.egg-info/
--rw-rw-rw-   0        0        0     3809 2023-03-10 07:12:21.000000 aiomoney-1.0.8/aiomoney.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-03-10 07:12:21.000000 aiomoney-1.0.8/aiomoney.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 07:12:21.000000 aiomoney-1.0.8/aiomoney.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-03-10 07:12:21.000000 aiomoney-1.0.8/aiomoney.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-10 07:12:21.000000 aiomoney-1.0.8/aiomoney.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-10 07:12:21.504238 aiomoney-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-03-10 07:12:18.000000 aiomoney-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-10 07:22:28.700929 aiomoney-1.0.9/
+-rw-rw-rw-   0        0        0     3809 2023-03-10 07:22:28.700929 aiomoney-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3238 2023-03-10 06:47:08.000000 aiomoney-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-10 07:22:28.685305 aiomoney-1.0.9/aiomoney/
+-rw-rw-rw-   0        0        0       78 2023-03-10 04:38:35.000000 aiomoney-1.0.9/aiomoney/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-03-09 14:31:45.000000 aiomoney-1.0.9/aiomoney/authorization.py
+-rw-rw-rw-   0        0        0       96 2023-03-09 14:24:49.000000 aiomoney-1.0.9/aiomoney/exceptions.py
+-rw-rw-rw-   0        0        0     1559 2023-03-10 04:18:32.000000 aiomoney-1.0.9/aiomoney/request.py
+drwxrwxrwx   0        0        0        0 2023-03-10 07:22:28.700929 aiomoney-1.0.9/aiomoney/types/
+-rw-rw-rw-   0        0        0      179 2023-03-10 04:07:21.000000 aiomoney-1.0.9/aiomoney/types/__init__.py
+-rw-rw-rw-   0        0        0      823 2023-03-10 03:51:21.000000 aiomoney-1.0.9/aiomoney/types/account_info.py
+-rw-rw-rw-   0        0        0      821 2023-03-10 03:55:47.000000 aiomoney-1.0.9/aiomoney/types/operation_details.py
+-rw-rw-rw-   0        0        0      574 2023-03-10 03:52:58.000000 aiomoney-1.0.9/aiomoney/types/operation_history.py
+-rw-rw-rw-   0        0        0      261 2023-03-10 04:06:54.000000 aiomoney-1.0.9/aiomoney/types/payment.py
+-rw-rw-rw-   0        0        0     3452 2023-03-10 05:11:11.000000 aiomoney-1.0.9/aiomoney/wallet.py
+drwxrwxrwx   0        0        0        0 2023-03-10 07:22:28.685305 aiomoney-1.0.9/aiomoney.egg-info/
+-rw-rw-rw-   0        0        0     3809 2023-03-10 07:22:28.000000 aiomoney-1.0.9/aiomoney.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-03-10 07:22:28.000000 aiomoney-1.0.9/aiomoney.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-10 07:22:28.000000 aiomoney-1.0.9/aiomoney.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-03-10 07:22:28.000000 aiomoney-1.0.9/aiomoney.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-03-10 07:22:28.000000 aiomoney-1.0.9/aiomoney.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-10 07:22:28.700929 aiomoney-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2023-03-10 07:22:02.000000 aiomoney-1.0.9/setup.py
```

### Comparing `aiomoney-1.0.8/PKG-INFO` & `aiomoney-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomoney
-Version: 1.0.8
+Version: 1.0.9
 Summary: Простая асинхронная библиотека для работы с API ЮMoney
 Home-page: https://github.com/fofmow/aiomoney
 Download-URL: https://github.com/fofmow/aiomoney
 Author: fofmow
 Author-email: fofmow@gmail.com
 License: MIT
 Keywords: yoomoney python async
```

### Comparing `aiomoney-1.0.8/README.md` & `aiomoney-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aiomoney-1.0.8/aiomoney/authorization.py` & `aiomoney-1.0.9/aiomoney/authorization.py`

 * *Files identical despite different names*

### Comparing `aiomoney-1.0.8/aiomoney/request.py` & `aiomoney-1.0.9/aiomoney/request.py`

 * *Files identical despite different names*

### Comparing `aiomoney-1.0.8/aiomoney/types/account_info.py` & `aiomoney-1.0.9/aiomoney/types/account_info.py`

 * *Files identical despite different names*

### Comparing `aiomoney-1.0.8/aiomoney/types/operation_details.py` & `aiomoney-1.0.9/aiomoney/types/operation_details.py`

 * *Files identical despite different names*

### Comparing `aiomoney-1.0.8/aiomoney/types/operation_history.py` & `aiomoney-1.0.9/aiomoney/types/operation_history.py`

 * *Files identical despite different names*

### Comparing `aiomoney-1.0.8/aiomoney/wallet.py` & `aiomoney-1.0.9/aiomoney/wallet.py`

 * *Files identical despite different names*

### Comparing `aiomoney-1.0.8/aiomoney.egg-info/PKG-INFO` & `aiomoney-1.0.9/aiomoney.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomoney
-Version: 1.0.8
+Version: 1.0.9
 Summary: Простая асинхронная библиотека для работы с API ЮMoney
 Home-page: https://github.com/fofmow/aiomoney
 Download-URL: https://github.com/fofmow/aiomoney
 Author: fofmow
 Author-email: fofmow@gmail.com
 License: MIT
 Keywords: yoomoney python async
```

### Comparing `aiomoney-1.0.8/setup.py` & `aiomoney-1.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 """
 :authors: fofmow
 :license: MIT
 """
 
-version = "1.0.8"
+version = "1.0.9"
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 
 if __name__ == "__main__":
     setup(
@@ -24,15 +24,15 @@
         long_description=long_description,
         long_description_content_type="text/markdown",
         
         url="https://github.com/fofmow/aiomoney",
         download_url="https://github.com/fofmow/aiomoney",
         license="MIT",
         packages=find_packages(),
-        install_requires=["aiohttp==3.8.3"],
+        install_requires=["aiohttp>=3.8.3"],
         classifiers=[
             "Programming Language :: Python :: 3.10",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent"
         ],
         keywords="yoomoney python async",
         python_requires=">=3.10"
```

