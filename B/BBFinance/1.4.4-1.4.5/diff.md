# Comparing `tmp/BBFinance-1.4.4.tar.gz` & `tmp/BBFinance-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.4.4.tar", last modified: Mon Apr 10 15:24:50 2023, max compression
+gzip compressed data, was "BBFinance-1.4.5.tar", last modified: Mon Apr 10 17:27:19 2023, max compression
```

## Comparing `BBFinance-1.4.4.tar` & `BBFinance-1.4.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 15:28:13.870548 BBFinance-1.4.4/
-drwxrwxrwx   0        0        0        0 2023-04-10 15:28:09.740618 BBFinance-1.4.4/BBFinance/
--rw-rw-rw-   0        0        0    38597 2023-04-10 15:24:18.000000 BBFinance-1.4.4/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      312 2023-04-10 15:24:35.000000 BBFinance-1.4.4/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:28:12.353636 BBFinance-1.4.4/BBFinance/__pycache__/
--rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.4/BBFinance/__pycache__/BBFinance.cpython-311.pyc
--rw-rw-rw-   0        0        0    23221 2023-04-10 14:51:01.000000 BBFinance-1.4.4/BBFinance/__pycache__/BBFinance.cpython-39.pyc
--rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.4/BBFinance/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      433 2023-04-10 14:19:00.000000 BBFinance-1.4.4/BBFinance/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-10 15:28:11.413718 BBFinance-1.4.4/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     1997 2023-04-10 15:27:58.000000 BBFinance-1.4.4/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-04-10 15:28:06.000000 BBFinance-1.4.4/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 15:27:58.000000 BBFinance-1.4.4/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      255 2023-04-10 15:27:58.000000 BBFinance-1.4.4/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 15:27:58.000000 BBFinance-1.4.4/BBFinance.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 15:28:12.838363 BBFinance-1.4.4/Data/
--rw-rw-rw-   0        0        0    14286 2023-04-10 14:00:41.000000 BBFinance-1.4.4/Data/AtivosIbov.xlsx
--rw-rw-rw-   0        0        0     1099 2023-04-04 20:31:26.000000 BBFinance-1.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1997 2023-04-10 15:28:13.823648 BBFinance-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-04-06 20:03:42.000000 BBFinance-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 15:28:13.448368 BBFinance-1.4.4/__pycache__/
--rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.4/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.4/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0      300 2023-04-04 20:31:26.000000 BBFinance-1.4.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 15:28:13.901828 BBFinance-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1296 2023-04-10 15:27:34.000000 BBFinance-1.4.4/setup.py
--rw-rw-rw-   0        0        0       59 2023-04-10 14:27:20.000000 BBFinance-1.4.4/teste.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:30:41.306390 BBFinance-1.4.5/
+drwxrwxrwx   0        0        0        0 2023-04-10 17:30:41.415828 BBFinance-1.4.5/BBFinance/
+-rw-rw-rw-   0        0        0    38822 2023-04-10 17:27:31.000000 BBFinance-1.4.5/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      312 2023-04-10 15:30:26.000000 BBFinance-1.4.5/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:30:42.353818 BBFinance-1.4.5/BBFinance/__pycache__/
+-rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.5/BBFinance/__pycache__/BBFinance.cpython-311.pyc
+-rw-rw-rw-   0        0        0    23221 2023-04-10 14:51:01.000000 BBFinance-1.4.5/BBFinance/__pycache__/BBFinance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.5/BBFinance/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      433 2023-04-10 14:19:00.000000 BBFinance-1.4.5/BBFinance/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-04-10 17:30:42.025523 BBFinance-1.4.5/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-04-10 17:30:33.000000 BBFinance-1.4.5/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-04-10 17:30:39.000000 BBFinance-1.4.5/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 17:30:33.000000 BBFinance-1.4.5/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      255 2023-04-10 17:30:33.000000 BBFinance-1.4.5/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 17:30:33.000000 BBFinance-1.4.5/BBFinance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 17:30:42.431992 BBFinance-1.4.5/Data/
+-rw-rw-rw-   0        0        0    14286 2023-04-10 14:00:41.000000 BBFinance-1.4.5/Data/AtivosIbov.xlsx
+-rw-rw-rw-   0        0        0      589 2023-04-10 16:16:08.000000 BBFinance-1.4.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2023 2023-04-10 17:30:42.698568 BBFinance-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-04-06 20:03:42.000000 BBFinance-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 17:30:42.573456 BBFinance-1.4.5/__pycache__/
+-rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.5/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.5/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1204 2023-04-10 17:22:53.000000 BBFinance-1.4.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 17:30:42.714195 BBFinance-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1322 2023-04-10 17:29:58.000000 BBFinance-1.4.5/setup.py
+-rw-rw-rw-   0        0        0       59 2023-04-10 14:27:20.000000 BBFinance-1.4.5/teste.py
```

### Comparing `BBFinance-1.4.4/BBFinance/BBFinance.py` & `BBFinance-1.4.5/BBFinance/BBFinance.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,14 +561,25 @@
 responseHistory = Response(media_type="application/json")
 
 
 ## BUSCA INFO DE FUNDOS ##
 
 @app.get("/infoFunds", response_model=None)
 def get_funds(symbol: str) -> pd.DataFrame:
+
+    """
+    ## Usabilidade
+    Funçao utilizada para adquirir as principais caracteristicas e informações do fundo selecionado
+
+    ## Parâmetros
+
+    - symbol -> Nome do Fundo para fazer a busca \n
+
+    """
+
     url = "https://www.fundsexplorer.com.br/ranking"
     response = requests.get(url)
     soup = BeautifulSoup(response.content, "html.parser")
     table = soup.find_all("table")[0]
     fundsDF = pd.read_html(str(table))[0]    
     fundsDF['Código do fundo'] = fundsDF['Código do fundo'].apply(lambda x: x+'.SA')
```

### Comparing `BBFinance-1.4.4/BBFinance/__pycache__/BBFinance.cpython-311.pyc` & `BBFinance-1.4.5/BBFinance/__pycache__/BBFinance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.4/BBFinance/__pycache__/BBFinance.cpython-39.pyc` & `BBFinance-1.4.5/BBFinance/__pycache__/BBFinance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.4/BBFinance.egg-info/PKG-INFO` & `BBFinance-1.4.5/BBFinance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4.4
+Version: 1.4.5
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # BBFinance
 
 Biblioteca de análise financeira
```

### Comparing `BBFinance-1.4.4/BBFinance.egg-info/SOURCES.txt` & `BBFinance-1.4.5/BBFinance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.4/Data/AtivosIbov.xlsx` & `BBFinance-1.4.5/Data/AtivosIbov.xlsx`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.4/PKG-INFO` & `BBFinance-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4.4
+Version: 1.4.5
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # BBFinance
 
 Biblioteca de análise financeira
```

### Comparing `BBFinance-1.4.4/README.md` & `BBFinance-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.4/__pycache__/main.cpython-39.pyc` & `BBFinance-1.4.5/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.4/setup.py` & `BBFinance-1.4.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.4.4',
+    version='1.4.5',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
     license='MIT',
     packages=['BBFinance'],
     long_description= long_description,
@@ -31,11 +31,11 @@
         'Unicode>=1.3.6',
         'typing_extensions>=4.5.0'
         
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.9',
     ],
 )
```

