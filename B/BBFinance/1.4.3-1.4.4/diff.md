# Comparing `tmp/BBFinance-1.4.3.tar.gz` & `tmp/BBFinance-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.4.3.tar", last modified: Mon Apr 10 14:48:15 2023, max compression
+gzip compressed data, was "BBFinance-1.4.4.tar", last modified: Mon Apr 10 15:24:50 2023, max compression
```

## Comparing `BBFinance-1.4.3.tar` & `BBFinance-1.4.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:51:38.976927 BBFinance-1.4.3/
-drwxrwxrwx   0        0        0        0 2023-04-10 14:51:35.757946 BBFinance-1.4.3/BBFinance/
--rw-rw-rw-   0        0        0    38829 2023-04-10 14:50:58.000000 BBFinance-1.4.3/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      325 2023-04-10 14:07:15.000000 BBFinance-1.4.3/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:51:37.898725 BBFinance-1.4.3/BBFinance/__pycache__/
--rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.3/BBFinance/__pycache__/BBFinance.cpython-311.pyc
--rw-rw-rw-   0        0        0    23221 2023-04-10 14:51:01.000000 BBFinance-1.4.3/BBFinance/__pycache__/BBFinance.cpython-39.pyc
--rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.3/BBFinance/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      433 2023-04-10 14:19:00.000000 BBFinance-1.4.3/BBFinance/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-10 14:51:37.023672 BBFinance-1.4.3/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     1997 2023-04-10 14:51:22.000000 BBFinance-1.4.3/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-04-10 14:51:32.000000 BBFinance-1.4.3/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:51:22.000000 BBFinance-1.4.3/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      255 2023-04-10 14:51:22.000000 BBFinance-1.4.3/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 14:51:23.000000 BBFinance-1.4.3/BBFinance.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 14:51:38.211248 BBFinance-1.4.3/Data/
--rw-rw-rw-   0        0        0    14286 2023-04-10 14:00:41.000000 BBFinance-1.4.3/Data/AtivosIbov.xlsx
--rw-rw-rw-   0        0        0     1099 2023-04-04 20:31:26.000000 BBFinance-1.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1997 2023-04-10 14:51:38.945688 BBFinance-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-04-06 20:03:42.000000 BBFinance-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:51:38.430014 BBFinance-1.4.3/__pycache__/
--rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.3/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.3/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0      300 2023-04-04 20:31:26.000000 BBFinance-1.4.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 14:51:39.008198 BBFinance-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1296 2023-04-10 14:44:39.000000 BBFinance-1.4.3/setup.py
--rw-rw-rw-   0        0        0       59 2023-04-10 14:27:20.000000 BBFinance-1.4.3/teste.py
+drwxrwxrwx   0        0        0        0 2023-04-10 15:28:13.870548 BBFinance-1.4.4/
+drwxrwxrwx   0        0        0        0 2023-04-10 15:28:09.740618 BBFinance-1.4.4/BBFinance/
+-rw-rw-rw-   0        0        0    38597 2023-04-10 15:24:18.000000 BBFinance-1.4.4/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      312 2023-04-10 15:24:35.000000 BBFinance-1.4.4/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 15:28:12.353636 BBFinance-1.4.4/BBFinance/__pycache__/
+-rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.4/BBFinance/__pycache__/BBFinance.cpython-311.pyc
+-rw-rw-rw-   0        0        0    23221 2023-04-10 14:51:01.000000 BBFinance-1.4.4/BBFinance/__pycache__/BBFinance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.4/BBFinance/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      433 2023-04-10 14:19:00.000000 BBFinance-1.4.4/BBFinance/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-04-10 15:28:11.413718 BBFinance-1.4.4/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     1997 2023-04-10 15:27:58.000000 BBFinance-1.4.4/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-04-10 15:28:06.000000 BBFinance-1.4.4/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 15:27:58.000000 BBFinance-1.4.4/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      255 2023-04-10 15:27:58.000000 BBFinance-1.4.4/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 15:27:58.000000 BBFinance-1.4.4/BBFinance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 15:28:12.838363 BBFinance-1.4.4/Data/
+-rw-rw-rw-   0        0        0    14286 2023-04-10 14:00:41.000000 BBFinance-1.4.4/Data/AtivosIbov.xlsx
+-rw-rw-rw-   0        0        0     1099 2023-04-04 20:31:26.000000 BBFinance-1.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1997 2023-04-10 15:28:13.823648 BBFinance-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-04-06 20:03:42.000000 BBFinance-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 15:28:13.448368 BBFinance-1.4.4/__pycache__/
+-rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.4/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.4/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0      300 2023-04-04 20:31:26.000000 BBFinance-1.4.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 15:28:13.901828 BBFinance-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2023-04-10 15:27:34.000000 BBFinance-1.4.4/setup.py
+-rw-rw-rw-   0        0        0       59 2023-04-10 14:27:20.000000 BBFinance-1.4.4/teste.py
```

### Comparing `BBFinance-1.4.3/BBFinance/BBFinance.py` & `BBFinance-1.4.4/BBFinance/BBFinance.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,16 @@
     """
     
     stock = yf.Ticker(symbol)
     info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO
     tipoInfo = type(info)
     if tipoInfo == dict:
         pass #SE FOR VAI SO PASSAR 
-    
+    else:
+        print('Ticker Invalido')
     # Obtenha o valor a mercado da açao
     current_price = stock.info['regularMarketPrice']
 
     # Obtenha o nome completo da empresa
     company_name = stock.info['longName']
 
     #Valor de Dividendos
@@ -117,23 +118,22 @@
     ## Parâmetros
     
     - symbol -> Nome do Ativo para a busca \n
     - period -> Data em ANOS para a busca das informaçoes do Ativo \n
     
     """
     
-    try:
-        stock = yf.Ticker(symbol)
-        info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO
-        tipoInfo = type(info)
-        if tipoInfo == dict:
-            pass #SE FOR VAI SO PASSAR 
-    except:
-        return {"error": print("Invalid ticker symbol")}
-    
+    stock = yf.Ticker(symbol)
+    info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO
+    tipoInfo = type(info)
+    if tipoInfo == dict:
+        pass #SE FOR VAI SO PASSAR 
+    else:
+        print('Ticker Invalido')
+
     history = stock.history(period=period)
     
     if history.empty:
         return {"error": print("No data found")}
     else:
         history_dict = history.to_dict(orient="list")
         history_df = pd.DataFrame.from_dict(history_dict).reset_index(drop=False)
@@ -163,22 +163,21 @@
     
     ## Parâmetros
     
     - symbol -> Nome do Ativo para a busca \n
     
     """
     
-    try:
-        stock = yf.Ticker(symbol)
-        info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO
-        tipoInfo = type(info)
-        if tipoInfo == dict:
-            pass #SE FOR VAI SO PASSAR 
-    except:
-        return {"error": print("Invalid ticker symbol")}
+    stock = yf.Ticker(symbol)
+    info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO
+    tipoInfo = type(info)
+    if tipoInfo == dict:
+        pass #SE FOR VAI SO PASSAR 
+    else:
+        print('Ticker Invalido')
 
     history = stock.history(period='1d')
     close_prices = history['Close']
     trend = 'up' if close_prices.iloc[-1] > close_prices.iloc[0] else 'down'
     
     json_data = { "symbol": symbol,
                 "trend": trend,
@@ -207,22 +206,21 @@
     Quando o RSI está abaixo de 30, o ativo é considerado sobrevendido, o que significa que pode estar prestes a subir novamente. \n 
     
     ## Parâmetros
     - symbol -> Nome do Ativo para a busca \n
     
     """
     
-    try:
-        stock = yf.Ticker(symbol)
-        info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO, SENAO VAI PASSAR
-        tipoInfo = type(info)
-        if tipoInfo == dict:
-            pass 
-    except:
-        return {"error": print("Invalid ticker symbol")}
+    stock = yf.Ticker(symbol)
+    info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO, SENAO VAI PASSAR
+    tipoInfo = type(info)
+    if tipoInfo == dict:
+        pass 
+    else:
+        print('Ticker Invalido')
 
     history = stock.history(period='max')
     close_prices = history['Close']
     
     # Calcula as médias móveis
     sma_50 = close_prices.rolling(window=50).mean().iloc[-1] #calcula as médias móveis de 50 períodos
     sma_200 = close_prices.rolling(window=200).mean().iloc[-1]  #calcula as médias móveis de 200 períodos
@@ -253,14 +251,15 @@
 
     return json_data
 
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/technical")
 responseHistory = Response(media_type="application/json")
 
+
 ## VOLATILIDADE ##
 
 @app.get("stocks/{symbol}/volatility", response_model=None)
 def get_volatility(symbol: str, start_date: str, end_date: str) -> str:
     
     """
     ## Usabilidade 
@@ -284,14 +283,15 @@
 
     return volatility
 
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/volatility")
 responseHistory = Response(media_type="application/json")
 
+
 ## BETA ##
 
 @app.get("stocks/{symbol}/beta", response_model=None)
 def get_beta(symbol: str) -> dict:
     
     """
     ## Usabilidade 
@@ -300,24 +300,23 @@
     
     ## Parâmetros
     - symbol -> Nome do Ativo para a busca \n
     - market -> Como padrao, Mercado: IBOVESPA / BVSP
     """
     
     # Obter os dados do ativo e do mercado
-    try:
-        asset = yf.Ticker('PETR4.SA')
-        market = yf.Ticker("^BVSP") # Índice Bovespa como mercado de referência
-        info = asset.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO, SENAO VAI PASSAR
-        infoMarket = market.info
-        tipoInfo = type(info)
-        if tipoInfo == dict or infoMarket == dict:
-            pass 
-    except:
-        return {"error": print("Invalid ticker symbol")}
+    asset = yf.Ticker('PETR4.SA')
+    market = yf.Ticker("^BVSP") # Índice Bovespa como mercado de referência
+    info = asset.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO, SENAO VAI PASSAR
+    infoMarket = market.info
+    tipoInfo = type(info)
+    if tipoInfo == dict or infoMarket == dict:
+        pass 
+    else:
+        print('Ticker Invalido')
 
     asset_history = asset.history(period="max")
     market_history = market.history(period="max")
 
     # Calcular os retornos diários
     asset_returns = asset_history['Close'].pct_change()
     market_returns = market_history['Close'].pct_change()
@@ -360,22 +359,21 @@
     
     - symbol -> Nome do Ativo para fazer a busca \n
     - confidence_level -> Nivel de confiança para o VAR (0 a 1), normalmente usado em 0.95 \n
     - lookback_period -> Periodo EM DIAS a ser considerado para o cálculo do VaR
 
     """
     
-    try:
-        stock = yf.Ticker(symbol)
-        info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO, SENAO VAI PASSAR
-        tipoInfo = type(info)
-        if tipoInfo == dict:
-            pass
-    except:
-         print("Invalid ticker symbol")
+    stock = yf.Ticker(symbol)
+    info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO, SENAO VAI PASSAR
+    tipoInfo = type(info)
+    if tipoInfo == dict:
+        pass
+    else:
+        print('Ticker Invalido')
 
     # Obter os dados de preços do ativo
     prices = stock.history(period=f"{lookback_period}d")["Close"]
 
     # Calcular o retorno diário da ação
     returns = np.log(prices / prices.shift(1))
```

### Comparing `BBFinance-1.4.3/BBFinance/__pycache__/BBFinance.cpython-311.pyc` & `BBFinance-1.4.4/BBFinance/__pycache__/BBFinance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.3/BBFinance/__pycache__/BBFinance.cpython-39.pyc` & `BBFinance-1.4.4/BBFinance/__pycache__/BBFinance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.3/BBFinance.egg-info/PKG-INFO` & `BBFinance-1.4.4/BBFinance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4.3
+Version: 1.4.4
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.4.3/BBFinance.egg-info/SOURCES.txt` & `BBFinance-1.4.4/BBFinance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.3/Data/AtivosIbov.xlsx` & `BBFinance-1.4.4/Data/AtivosIbov.xlsx`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.3/LICENSE.txt` & `BBFinance-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.3/PKG-INFO` & `BBFinance-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4.3
+Version: 1.4.4
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.4.3/README.md` & `BBFinance-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.3/__pycache__/main.cpython-39.pyc` & `BBFinance-1.4.4/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.3/setup.py` & `BBFinance-1.4.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.4.3',
+    version='1.4.4',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
     license='MIT',
     packages=['BBFinance'],
     long_description= long_description,
```

