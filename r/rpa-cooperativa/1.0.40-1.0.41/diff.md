# Comparing `tmp/rpa_cooperativa-1.0.40.tar.gz` & `tmp/rpa_cooperativa-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.40.tar", last modified: Thu Apr  6 20:21:33 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.41.tar", last modified: Mon Apr 10 14:01:59 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.40.tar` & `rpa_cooperativa-1.0.41.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 20:21:33.201758 rpa_cooperativa-1.0.40/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.40/LICENSE
--rw-rw-rw-   0        0        0     5326 2023-04-06 20:21:33.195152 rpa_cooperativa-1.0.40/PKG-INFO
--rw-rw-rw-   0        0        0     4181 2023-03-24 13:54:04.000000 rpa_cooperativa-1.0.40/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 20:21:32.951345 rpa_cooperativa-1.0.40/rpa_coop/
--rw-rw-rw-   0        0        0      507 2023-03-24 17:45:39.000000 rpa_cooperativa-1.0.40/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 20:21:33.130796 rpa_cooperativa-1.0.40/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.40/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.40/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.40/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.40/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.40/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.40/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      347 2023-02-28 19:51:44.000000 rpa_cooperativa-1.0.40/rpa_coop/img/siac_verde.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.40/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0      336 2023-02-28 19:52:19.000000 rpa_cooperativa-1.0.40/rpa_coop/img/siat_verde.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.40/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.40/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    63570 2023-04-06 20:20:32.000000 rpa_cooperativa-1.0.40/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-04-06 20:21:33.186142 rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     5326 2023-04-06 20:21:32.000000 rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-04-06 20:21:32.000000 rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 20:21:32.000000 rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-06 20:21:32.000000 rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      544 2023-04-06 20:21:32.000000 rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 20:21:32.000000 rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 20:21:33.202758 rpa_cooperativa-1.0.40/setup.cfg
--rw-rw-rw-   0        0        0     2305 2023-04-06 20:20:46.000000 rpa_cooperativa-1.0.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:01:59.747887 rpa_cooperativa-1.0.41/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.41/LICENSE
+-rw-rw-rw-   0        0        0     5578 2023-04-10 14:01:59.742065 rpa_cooperativa-1.0.41/PKG-INFO
+-rw-rw-rw-   0        0        0     4429 2023-04-10 13:24:59.000000 rpa_cooperativa-1.0.41/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 14:01:59.410355 rpa_cooperativa-1.0.41/rpa_coop/
+-rw-rw-rw-   0        0        0      528 2023-04-10 13:18:19.000000 rpa_cooperativa-1.0.41/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:01:59.651274 rpa_cooperativa-1.0.41/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.41/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.41/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.41/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.41/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.41/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.41/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      347 2023-02-28 19:51:44.000000 rpa_cooperativa-1.0.41/rpa_coop/img/siac_verde.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.41/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0      336 2023-02-28 19:52:19.000000 rpa_cooperativa-1.0.41/rpa_coop/img/siat_verde.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.41/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.41/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    65069 2023-04-10 14:00:48.000000 rpa_cooperativa-1.0.41/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:01:59.723355 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     5578 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      544 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:01:59.750886 rpa_cooperativa-1.0.41/setup.cfg
+-rw-rw-rw-   0        0        0     2305 2023-04-10 12:54:19.000000 rpa_cooperativa-1.0.41/setup.py
```

### Comparing `rpa_cooperativa-1.0.40/LICENSE` & `rpa_cooperativa-1.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.40/PKG-INFO` & `rpa_cooperativa-1.0.41/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.40
+Version: 1.0.41
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -36,14 +36,28 @@
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
 ```
 
+## manipulacao selenium: automaÃ§Ã£o web
+```python
+from rpa_coop import selenium
+import time
+
+driver = selenium.driver_edge()
+url = 'http://www.google.com.br'
+
+time.sleep(1)
+driver.get(url)
+time.sleep(1)
+driver.maximize_window()
+```
+
 
 ## manipulacao da ferramenta de fluxo de trabalho: fluid
 ```python
 ########################################################
 from rpa_coop import fluid
 
 # Variaveis
```

### Comparing `rpa_cooperativa-1.0.40/README.md` & `rpa_cooperativa-1.0.41/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,28 @@
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
 ```
 
+## manipulacao selenium: automação web
+```python
+from rpa_coop import selenium
+import time
+
+driver = selenium.driver_edge()
+url = 'http://www.google.com.br'
+
+time.sleep(1)
+driver.get(url)
+time.sleep(1)
+driver.maximize_window()
+```
+
 
 ## manipulacao da ferramenta de fluxo de trabalho: fluid
 ```python
 ########################################################
 from rpa_coop import fluid
 
 # Variaveis
```

### Comparing `rpa_cooperativa-1.0.40/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.41/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.40/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.41/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.40/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.41/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.40/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.41/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.40/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.41/rpa_coop/rpa_coop.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,14 @@
         self.senha_fluid = str(gerador_pwd('usuario_fluid', 'senha'))
         
         self.ip_planning = str(os.getenv('ip_planning'))
         self.user_planning = str(os.getenv('user_planning'))
         self.pw_bd_planning = str(urllib.parse.quote_plus(os.getenv('pw_bd_planning'))) 
         
         
- 
     def anexar_arquivo_fluid(self, cod_processo:str, path_file:str, tipo_arquivo:str):
         '''
             num_processo = '497305'\n
             path_file = 'C:\\Temp\\teste.xlsx'\n
             id_doc_fluid = '417'\n
             api_upload_anexo_fluid( num_processo, path_file, id_doc_fluid )
         '''
@@ -1380,23 +1379,60 @@
 print(df2)'''
         
         file = open(script_file_path, 'a')
         file.write(txt)
         file.close()        
         self.comentar_linha(script_file_path, 'gerador_de_codigo.')
         
+           
+  
+class Selenium:
+    
+    def __init__(self):
+        pass
+    
+    from selenium import webdriver
+    from selenium.webdriver.common.by import By
+    from selenium.webdriver.support.ui import WebDriverWait
+    from selenium.webdriver.common.action_chains import ActionChains
+    from selenium.webdriver.support import expected_conditions as ec
+    from selenium.webdriver.support.ui import Select
+    from selenium.webdriver.common.keys import Keys
+    from selenium.webdriver.common.alert import Alert
+    
+    from selenium.webdriver.chrome.service import Service as ChromeService 
+    from webdriver_manager.chrome import ChromeDriverManager
+    from selenium.webdriver.chrome.options import Options as chrome_options
+    
+    from selenium.webdriver.edge.service import Service as EdgeService
+    from webdriver_manager.microsoft import EdgeChromiumDriverManager
+    from selenium.webdriver.edge.options import Options as edge_options
+    
+    
+    def driver_chrome(self):
+        driver = self.webdriver.Chrome(service=(self.ChromeService(self.ChromeDriverManager().install())))
+        return driver
+    
+    
+    def driver_edge(self):
+        driver = self.webdriver.Edge(service=(self.EdgeService(self.EdgeChromiumDriverManager().install())))
+        return driver
+    
+    
+    def aguardar_elemento(self, driver, xpath, espera_em_segundos=60):
+        '''Espera por um elemento até o tempo máximo definido, interrompe a espera assim que encontrar o elemento'''
+        elemento_esperado = self.WebDriverWait(driver, espera_em_segundos).until(self.ec.visibility_of_element_located((self.By.XPATH, xpath)))
+        encontrou = str(elemento_esperado.is_displayed())
+        return encontrou
+        
         
-     
-
-url_api_whats = str(gerador_pwd('url_api_whats', 'sistema'))
-token_api_whats = str(gerador_pwd('url_api_whats', 'senha'))
 
-# url_api_sms = str(gerador_pwd('url_api_sms', 'sistema'))
-# token_api_sms = str(gerador_pwd('url_api_sms', 'senha'))
-# print(token_api_whats)      
-  
+    
+    
+    
+
```

### Comparing `rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.40
+Version: 1.0.41
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -36,14 +36,28 @@
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
 ```
 
+## manipulacao selenium: automaÃ§Ã£o web
+```python
+from rpa_coop import selenium
+import time
+
+driver = selenium.driver_edge()
+url = 'http://www.google.com.br'
+
+time.sleep(1)
+driver.get(url)
+time.sleep(1)
+driver.maximize_window()
+```
+
 
 ## manipulacao da ferramenta de fluxo de trabalho: fluid
 ```python
 ########################################################
 from rpa_coop import fluid
 
 # Variaveis
```

### Comparing `rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.40/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.40/setup.py` & `rpa_cooperativa-1.0.41/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.40",
+    version="1.0.41",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

