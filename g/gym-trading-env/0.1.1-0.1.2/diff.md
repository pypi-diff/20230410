# Comparing `tmp/gym-trading-env-0.1.1.tar.gz` & `tmp/gym-trading-env-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.1.1.tar", last modified: Wed Apr  5 13:23:15 2023, max compression
+gzip compressed data, was "gym-trading-env-0.1.2.tar", last modified: Mon Apr 10 19:40:21 2023, max compression
```

## Comparing `gym-trading-env-0.1.1.tar` & `gym-trading-env-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 13:23:15.312158 gym-trading-env-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0    13015 2023-04-05 13:23:15.311162 gym-trading-env-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    11153 2023-04-02 17:44:50.000000 gym-trading-env-0.1.1/README.md
--rw-rw-rw-   0        0        0      816 2023-04-05 13:22:44.000000 gym-trading-env-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 13:23:15.312158 gym-trading-env-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 13:23:15.224393 gym-trading-env-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 13:23:15.244340 gym-trading-env-0.1.1/src/gym_trading_env/
--rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.1/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     8342 2023-04-05 10:11:44.000000 gym-trading-env-0.1.1/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2502 2023-04-05 09:57:31.000000 gym-trading-env-0.1.1/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-04-05 13:23:15.308169 gym-trading-env-0.1.1/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.1/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.1/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.1/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.1/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-04-05 13:23:15.294206 gym-trading-env-0.1.1/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0    13015 2023-04-05 13:23:15.000000 gym-trading-env-0.1.1/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-04-05 13:23:15.000000 gym-trading-env-0.1.1/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 13:23:15.000000 gym-trading-env-0.1.1/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-05 13:23:15.000000 gym-trading-env-0.1.1/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-05 13:23:15.000000 gym-trading-env-0.1.1/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.403118 gym-trading-env-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    14061 2023-04-10 19:40:21.401123 gym-trading-env-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12199 2023-04-10 19:39:58.000000 gym-trading-env-0.1.2/README.md
+-rw-rw-rw-   0        0        0      848 2023-04-10 19:19:49.000000 gym-trading-env-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 19:40:21.404119 gym-trading-env-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.302708 gym-trading-env-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.337043 gym-trading-env-0.1.2/src/gym_trading_env/
+-rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.2/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     3855 2023-04-10 19:15:33.000000 gym-trading-env-0.1.2/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.2/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2471 2023-04-05 13:55:23.000000 gym-trading-env-0.1.2/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.399128 gym-trading-env-0.1.2/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.2/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.2/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.2/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.2/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.375193 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0    14061 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.1.1/LICENSE.txt` & `gym-trading-env-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.1/PKG-INFO` & `gym-trading-env-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,7 @@
-Metadata-Version: 2.1
-Name: gym-trading-env
-Version: 0.1.1
-Summary: A simple, easy, customizable Open IA Gym environments for trading.
-Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
-License: MIT License
-        
-        Copyright (c) [year] [fullname]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/ClementPerroud/Gym-Trading-Env
-Project-URL: Bug Tracker, https://github.com/ClementPerroud/Gym-Trading-Env/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Crypto-Trading-Env
 
 
 <img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render.gif?raw=true" width = "800"/>
 
 An OpenAI Gym environment for simulating stocks and train Reinforcement Learning (RL) trading agents.
 
@@ -51,16 +16,18 @@
 ```
 
 ## Environment Properties
 
 ### Actions space : positions
 
 Github is full of environments that consider actions such as **BUY**, **SELL**. In my opinion, it is a real mistake to consider a reinforcement learning agent in the same way as a trader. Traders make trade and to do so, they place orders on the market (eg. Buy X of stock Y). But what really matter is the position reached. Now, imagine we labelled each position by a number :
-- ```1``` : All of our portfolio is converted into stock Y. *BUY ALL*
-- ```0``` : All of our portfolio is converted into our fiat currency. *SELL ALL*
+- ```1``` : All of our portfolio is converted into stock Y. (=*BUY ALL*)
+- ```0``` : All of our portfolio is converted into our fiat currency. (=*SELL ALL*)
+
+
 Now, we can imagine half position and other variants :
 - ```0.5``` : 50% in stock Y & 50% in currency
 - Even : ```0.1``` : 10% in stock Y & 90% in currency
 ....
 
 
 In fact, it is way simpler for a RL-agent to work with positions. This way, it can easily make complex operation with a simple action space.
@@ -79,15 +46,32 @@
 ```python
 # Available in the github repo : test/data/BTC_USD-Hourly.csv
 df = pd.read_csv("data/BTC_USD-Hourly.csv", parse_dates=["date"], index_col= "date")
 df.sort_index(inplace= True)
 df.dropna(inplace= True)
 df.drop_duplicates(inplace=True)
 ```
-**2 - Create your feature**. Your RL-agent will need some good, preprocessed features. It is your job to make sure it has everything it needs.
+**1.1 (Optional) Download data** : The package provide a easy way to download data (works with CCTX ans use asyncio to get FAST) :
+```python
+from gym_trading_env.downloader import download
+import datetime
+
+download(
+    exchange_names = ["binance", "bitfinex2", "huobi"],
+    symbols= ["BTC/USDT", "ETH/USDT"],
+    timeframe= "30m",
+    dir = "test/data",
+    since= datetime.datetime(year= 2019, month= 1, day=1),
+    until = datetime.datetime(year= 2023, month= 1, day=1),
+)
+```
+This function use pickle format to save the OHLCV data. You will need to import the dataset with ```pd.read_pickle('... .pkl', ...)```. The function supports exchange_names ```binance```, ```biftfinex2``` (API v2) and ```huobi```.
+
+
+**2 - Create your features**. Your RL-agent will need some good, preprocessed features. It is your job to make sure it has everything it needs.
 **The feature column names need to contain the keyword 'feature'. The environment will automatically detect them !**
 
 ```python
 df["feature_close"] = df["close"].pct_change()
 df["feature_open"] = df["open"]/df["close"]
 df["feature_high"] = df["high"]/df["close"]
 df["feature_low"] = df["low"]/df["close"]
@@ -103,43 +87,51 @@
 The history object is similar to a DataFrame. It uses timestep and/or columns to access its values. You can use it this way :
 - ```history['column name', t]``` returns the a *scalar* value of the metrics 'column name' at time step t.
 - ```history['column name']``` returns a *numpy array* with all the values from timestep 0 to current timestep.
 - ```history[t]``` returns a *dictionnary* with of the metrics as keys with the associated values.
 
 
 Accessible columns of history object :
-- ```step```: ...,# Step = t
-- ```date```: ...,# Date at step t, datetime
-- ```reward```: ..., # Reward at step t
-- ```position_index```: ..., # Index of the position at step t amoung your position argument
-- ```position``` : ..., # Portfolio position at step t
+- ```step``` : Step = t.
+- ```date``` : Date at step t, datetime.
+- ```reward``` : Reward at step t.
+- ```position_index``` : Index of the position at step t amoung your position argument.
+- ```position``` : Portfolio position at step t.
+- ```portfolio_valuation```: Global valuation of the portfolio.
 
     *It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :*
-- ```data_close```: Close price,
-- ```data_open```: Open price,
-- ```data_high```:Hight price,
+- ```data_close``` : Close price.
+- ```data_open``` : Open price.
+- ```data_high``` : High price.
 
     *......*
 
-- ```portfolio_valuation```: Global valuation of the portfolio
-
-
     *It stores the distribution of the portfolio :*
-- ```portfolio_distribution_asset``` : The amount of owned asset (stock),
-- ```portfolio_distribution_fiat``` : The amount of owned fiat currency,
-- ```portfolio_distribution_borrowed_asset```: The amount of borrowed asset,
-- ```portfolio_distribution_borrowed_fiat```: The amount of borrowed fiat currency,
-- ```portfolio_distribution_interest_asset```: The total of cumalated interest generated by the borrowed asset.
-- ```portfolio_distribution_interest_fiat```: The total of cumalated interest generated by the borrowed fiat currency.
-
-
-**4 - Create the environment**
-
-```python
-env = TradingEnv(...)
+- ```portfolio_distribution_asset``` : The amount of owned asset (stock).
+- ```portfolio_distribution_fiat``` : The amount of owned fiat currency.
+- ```portfolio_distribution_borrowed_asset``` : The amount of borrowed asset.
+- ```portfolio_distribution_borrowed_fiat``` : The amount of borrowed fiat currency.
+- ```portfolio_distribution_interest_asset``` : The total of cumalated interest generated by the borrowed asset.
+- ```portfolio_distribution_interest_fiat``` : The total of cumalated interest generated by the borrowed fiat currency.
+
+
+**4 - Initiate the environment**
+
+```python
+env = TradingEnv(
+        name= "BTCUSD",
+        df = df,
+        windows= 5,
+        positions = [ -1, -0.5, 0, 0.5, 1], # From -1 (=SHORT), to +1 (=LONG)
+        initial_position = 0,
+        trading_fees = 0.01/100, # 0.01% per stock buy / sell (Binance fees)
+        borrow_interest_rate= 0.0003/100, # 0.0003% per timestep (= 1h here)
+        reward_function = reward_function,
+        portfolio_initial_value = 1000, # here, in USDT
+    )
 ```
 Parameters :
 - ```name``` (required) : Name of your asset / symbol
 - ```df``` (required) : DataFrame containing technical indicators ```open```, ```high```, ```low```, ```close```, ```volume```, and the features you want to be returned as observations (containing ```feature``` in their column names).
 - ```windows```(optional, default : None), If None, observation at t are the features at step t  (classic mode). If windows = i (int),  observation at t are the features from steps [t-i+1 :  t] (useful for reccurent models)
 - ```positions``` (optional, default : [0, 1]). Positions that the agent can choose (Explained in "Actions space : positions")
 - ```initial_position``` (optional, default : 0). Initial position of the portfolio
@@ -171,68 +163,60 @@
 
 For the render not to perturb the training, the render needs to be performed in a separate python script. This way you have plenty of time to perform analysis on your results. 
 
 First, you need to save your results at the end of every episode you want to render with ```env.save_for_render(...)```. And decide which file you want your logs to be stored in with paramter ```dir```. For example :
 
 ```python
 ...
-# At the end of episode you want to render
+# At the end of the episode you want to render
 env.save_for_render(dir = "render_logs")
 ```
 
 Then in the separated render script. You can import and initiate a render object, and run the render in a localhost web app :
 ```python
 from gym_trading_env.renderer import Renderer
-renderer = Renderer(render_dir="render_logs")
+renderer = Renderer(render_logs_dir="render_logs")
 renderer.run()
 ```
 
 You can add **metrics** and plot **lines** with :
 ```python
-# Add lines
-# - Simple Moving Average - 10
-renderer.add_scatter(
-        name = "sma10",
-        function = lambda df : df["close"].rolling(10).mean(),
-        scatter_args = {
-            "line": {"color":'blue'}
-        })
-# - Simple Moving Average - 40
-renderer.add_scatter(
-        name = "sma40",
-        function = lambda df : df["close"].rolling(40).mean(),
-        scatter_args = {
-            "line": {"color": "purple"}
-        })
-
-# Add metrics 
-def max_drawdown(df):
-    current_max = df["portfolio_valuation"].iloc[0]
-    max_drawdown = 0
-    for i in range(len(df)):
-        current_max = max(df["portfolio_valuation"].iloc[i], current_max)
-        max_drawdown = min(max_drawdown, (df["portfolio_valuation"].iloc[i] - current_max)/current_max)
-    return f"{max_drawdown*100:0.2f}%"
+renderer = Renderer(render_logs_dir="render_logs")
 
-renderer.add_metric("Max drawdown", max_drawdown)
+# Add Custom Lines (Simple Moving Average)
+renderer.add_line( name= "sma10", function= lambda df : df["close"].rolling(10).mean(), line_options ={"width" : 1, "color": "purple"})
+renderer.add_line( name= "sma20", function= lambda df : df["close"].rolling(20).mean(), line_options ={"width" : 1, "color": "blue"})
+
+# Add Custom Metrics (Annualized metrics)
+renderer.add_metric(
+    name = "Annual Market Return",
+    function = lambda df : f"{ ((df['close'].iloc[-1] / df['close'].iloc[0])**(pd.Timedelta(days=365)/(df.index.values[-1] - df.index.values[0]))-1)*100:0.2f}%"
+)
+
+renderer.add_metric(
+        name = "Annual Portfolio Return",
+        function = lambda df : f"{((df['portfolio_valuation'].iloc[-1] / df['portfolio_valuation'].iloc[0])**(pd.Timedelta(days=365)/(df.index.values[-1] - df.index.values[0]))-1)*100:0.2f}%"
+)
+
+renderer.run()
 ```
 
 <img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render_customization.gif?raw=true" width = "800"/>
 
 
 
-```.add_scatter``` takes arguments :
-- ```name``` : The name of the scatter
-- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
-- ```scatter_args``` : Paramaters added to the go.Scatter object during the process. It can be used to customize your plots. The [documentation of the go.Scatter object](https://plotly.com/python-api-reference/generated/plotly.graph_objects.Scatter.html) might help you.
+```.add_line``` takes arguments :
+- ```name``` (*required*): The name of the scatter
+- ```function``` (*required*): The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
+- ```line_options``` : Can contain a dict with keys ```color``` and ```width```
 
 
 ```.add_metric``` takes arguments :
 - ```name``` : The name of the metric
-- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a scalar.
+- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a **string** !
 
 
 Enjoy :)
```

### Comparing `gym-trading-env-0.1.1/README.md` & `gym-trading-env-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: gym-trading-env
+Version: 0.1.2
+Summary: A simple, easy, customizable Open IA Gym environments for trading.
+Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
+License: MIT License
+        
+        Copyright (c) [year] [fullname]
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/ClementPerroud/Gym-Trading-Env
+Project-URL: Bug Tracker, https://github.com/ClementPerroud/Gym-Trading-Env/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Crypto-Trading-Env
 
 
 <img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render.gif?raw=true" width = "800"/>
 
 An OpenAI Gym environment for simulating stocks and train Reinforcement Learning (RL) trading agents.
 
@@ -16,16 +51,18 @@
 ```
 
 ## Environment Properties
 
 ### Actions space : positions
 
 Github is full of environments that consider actions such as **BUY**, **SELL**. In my opinion, it is a real mistake to consider a reinforcement learning agent in the same way as a trader. Traders make trade and to do so, they place orders on the market (eg. Buy X of stock Y). But what really matter is the position reached. Now, imagine we labelled each position by a number :
-- ```1``` : All of our portfolio is converted into stock Y. *BUY ALL*
-- ```0``` : All of our portfolio is converted into our fiat currency. *SELL ALL*
+- ```1``` : All of our portfolio is converted into stock Y. (=*BUY ALL*)
+- ```0``` : All of our portfolio is converted into our fiat currency. (=*SELL ALL*)
+
+
 Now, we can imagine half position and other variants :
 - ```0.5``` : 50% in stock Y & 50% in currency
 - Even : ```0.1``` : 10% in stock Y & 90% in currency
 ....
 
 
 In fact, it is way simpler for a RL-agent to work with positions. This way, it can easily make complex operation with a simple action space.
@@ -44,15 +81,32 @@
 ```python
 # Available in the github repo : test/data/BTC_USD-Hourly.csv
 df = pd.read_csv("data/BTC_USD-Hourly.csv", parse_dates=["date"], index_col= "date")
 df.sort_index(inplace= True)
 df.dropna(inplace= True)
 df.drop_duplicates(inplace=True)
 ```
-**2 - Create your feature**. Your RL-agent will need some good, preprocessed features. It is your job to make sure it has everything it needs.
+**1.1 (Optional) Download data** : The package provide a easy way to download data (works with CCTX ans use asyncio to get FAST) :
+```python
+from gym_trading_env.downloader import download
+import datetime
+
+download(
+    exchange_names = ["binance", "bitfinex2", "huobi"],
+    symbols= ["BTC/USDT", "ETH/USDT"],
+    timeframe= "30m",
+    dir = "test/data",
+    since= datetime.datetime(year= 2019, month= 1, day=1),
+    until = datetime.datetime(year= 2023, month= 1, day=1),
+)
+```
+This function use pickle format to save the OHLCV data. You will need to import the dataset with ```pd.read_pickle('... .pkl', ...)```. The function supports exchange_names ```binance```, ```biftfinex2``` (API v2) and ```huobi```.
+
+
+**2 - Create your features**. Your RL-agent will need some good, preprocessed features. It is your job to make sure it has everything it needs.
 **The feature column names need to contain the keyword 'feature'. The environment will automatically detect them !**
 
 ```python
 df["feature_close"] = df["close"].pct_change()
 df["feature_open"] = df["open"]/df["close"]
 df["feature_high"] = df["high"]/df["close"]
 df["feature_low"] = df["low"]/df["close"]
@@ -68,43 +122,51 @@
 The history object is similar to a DataFrame. It uses timestep and/or columns to access its values. You can use it this way :
 - ```history['column name', t]``` returns the a *scalar* value of the metrics 'column name' at time step t.
 - ```history['column name']``` returns a *numpy array* with all the values from timestep 0 to current timestep.
 - ```history[t]``` returns a *dictionnary* with of the metrics as keys with the associated values.
 
 
 Accessible columns of history object :
-- ```step```: ...,# Step = t
-- ```date```: ...,# Date at step t, datetime
-- ```reward```: ..., # Reward at step t
-- ```position_index```: ..., # Index of the position at step t amoung your position argument
-- ```position``` : ..., # Portfolio position at step t
+- ```step``` : Step = t.
+- ```date``` : Date at step t, datetime.
+- ```reward``` : Reward at step t.
+- ```position_index``` : Index of the position at step t amoung your position argument.
+- ```position``` : Portfolio position at step t.
+- ```portfolio_valuation```: Global valuation of the portfolio.
 
     *It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :*
-- ```data_close```: Close price,
-- ```data_open```: Open price,
-- ```data_high```:Hight price,
+- ```data_close``` : Close price.
+- ```data_open``` : Open price.
+- ```data_high``` : High price.
 
     *......*
 
-- ```portfolio_valuation```: Global valuation of the portfolio
-
-
     *It stores the distribution of the portfolio :*
-- ```portfolio_distribution_asset``` : The amount of owned asset (stock),
-- ```portfolio_distribution_fiat``` : The amount of owned fiat currency,
-- ```portfolio_distribution_borrowed_asset```: The amount of borrowed asset,
-- ```portfolio_distribution_borrowed_fiat```: The amount of borrowed fiat currency,
-- ```portfolio_distribution_interest_asset```: The total of cumalated interest generated by the borrowed asset.
-- ```portfolio_distribution_interest_fiat```: The total of cumalated interest generated by the borrowed fiat currency.
+- ```portfolio_distribution_asset``` : The amount of owned asset (stock).
+- ```portfolio_distribution_fiat``` : The amount of owned fiat currency.
+- ```portfolio_distribution_borrowed_asset``` : The amount of borrowed asset.
+- ```portfolio_distribution_borrowed_fiat``` : The amount of borrowed fiat currency.
+- ```portfolio_distribution_interest_asset``` : The total of cumalated interest generated by the borrowed asset.
+- ```portfolio_distribution_interest_fiat``` : The total of cumalated interest generated by the borrowed fiat currency.
 
 
-**4 - Create the environment**
+**4 - Initiate the environment**
 
 ```python
-env = TradingEnv(...)
+env = TradingEnv(
+        name= "BTCUSD",
+        df = df,
+        windows= 5,
+        positions = [ -1, -0.5, 0, 0.5, 1], # From -1 (=SHORT), to +1 (=LONG)
+        initial_position = 0,
+        trading_fees = 0.01/100, # 0.01% per stock buy / sell (Binance fees)
+        borrow_interest_rate= 0.0003/100, # 0.0003% per timestep (= 1h here)
+        reward_function = reward_function,
+        portfolio_initial_value = 1000, # here, in USDT
+    )
 ```
 Parameters :
 - ```name``` (required) : Name of your asset / symbol
 - ```df``` (required) : DataFrame containing technical indicators ```open```, ```high```, ```low```, ```close```, ```volume```, and the features you want to be returned as observations (containing ```feature``` in their column names).
 - ```windows```(optional, default : None), If None, observation at t are the features at step t  (classic mode). If windows = i (int),  observation at t are the features from steps [t-i+1 :  t] (useful for reccurent models)
 - ```positions``` (optional, default : [0, 1]). Positions that the agent can choose (Explained in "Actions space : positions")
 - ```initial_position``` (optional, default : 0). Initial position of the portfolio
@@ -136,68 +198,60 @@
 
 For the render not to perturb the training, the render needs to be performed in a separate python script. This way you have plenty of time to perform analysis on your results. 
 
 First, you need to save your results at the end of every episode you want to render with ```env.save_for_render(...)```. And decide which file you want your logs to be stored in with paramter ```dir```. For example :
 
 ```python
 ...
-# At the end of episode you want to render
+# At the end of the episode you want to render
 env.save_for_render(dir = "render_logs")
 ```
 
 Then in the separated render script. You can import and initiate a render object, and run the render in a localhost web app :
 ```python
 from gym_trading_env.renderer import Renderer
-renderer = Renderer(render_dir="render_logs")
+renderer = Renderer(render_logs_dir="render_logs")
 renderer.run()
 ```
 
 You can add **metrics** and plot **lines** with :
 ```python
-# Add lines
-# - Simple Moving Average - 10
-renderer.add_scatter(
-        name = "sma10",
-        function = lambda df : df["close"].rolling(10).mean(),
-        scatter_args = {
-            "line": {"color":'blue'}
-        })
-# - Simple Moving Average - 40
-renderer.add_scatter(
-        name = "sma40",
-        function = lambda df : df["close"].rolling(40).mean(),
-        scatter_args = {
-            "line": {"color": "purple"}
-        })
-
-# Add metrics 
-def max_drawdown(df):
-    current_max = df["portfolio_valuation"].iloc[0]
-    max_drawdown = 0
-    for i in range(len(df)):
-        current_max = max(df["portfolio_valuation"].iloc[i], current_max)
-        max_drawdown = min(max_drawdown, (df["portfolio_valuation"].iloc[i] - current_max)/current_max)
-    return f"{max_drawdown*100:0.2f}%"
+renderer = Renderer(render_logs_dir="render_logs")
+
+# Add Custom Lines (Simple Moving Average)
+renderer.add_line( name= "sma10", function= lambda df : df["close"].rolling(10).mean(), line_options ={"width" : 1, "color": "purple"})
+renderer.add_line( name= "sma20", function= lambda df : df["close"].rolling(20).mean(), line_options ={"width" : 1, "color": "blue"})
+
+# Add Custom Metrics (Annualized metrics)
+renderer.add_metric(
+    name = "Annual Market Return",
+    function = lambda df : f"{ ((df['close'].iloc[-1] / df['close'].iloc[0])**(pd.Timedelta(days=365)/(df.index.values[-1] - df.index.values[0]))-1)*100:0.2f}%"
+)
+
+renderer.add_metric(
+        name = "Annual Portfolio Return",
+        function = lambda df : f"{((df['portfolio_valuation'].iloc[-1] / df['portfolio_valuation'].iloc[0])**(pd.Timedelta(days=365)/(df.index.values[-1] - df.index.values[0]))-1)*100:0.2f}%"
+)
 
-renderer.add_metric("Max drawdown", max_drawdown)
+renderer.run()
 ```
 
 <img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render_customization.gif?raw=true" width = "800"/>
 
 
 
-```.add_scatter``` takes arguments :
-- ```name``` : The name of the scatter
-- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
-- ```scatter_args``` : Paramaters added to the go.Scatter object during the process. It can be used to customize your plots. The [documentation of the go.Scatter object](https://plotly.com/python-api-reference/generated/plotly.graph_objects.Scatter.html) might help you.
+```.add_line``` takes arguments :
+- ```name``` (*required*): The name of the scatter
+- ```function``` (*required*): The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
+- ```line_options``` : Can contain a dict with keys ```color``` and ```width```
 
 
 ```.add_metric``` takes arguments :
 - ```name``` : The name of the metric
-- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a scalar.
+- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a **string** !
 
 
 Enjoy :)
```

### Comparing `gym-trading-env-0.1.1/pyproject.toml` & `gym-trading-env-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.1.1"
+version = "0.1.2"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["pandas>=1.5.3", "numpy>=1.23.1", "gym>=0.26.2", "flask>=2.2.3", "pyecharts>=2.0.2",]
+dependencies = ["pandas>=1.5.3", "numpy>=1.23.1", "gym>=0.26.2", "flask>=2.2.3", "pyecharts>=2.0.2", "ccxt>=3.0.59", "numpy>=1.24.2"]
 
 [project.urls]
 "Homepage" = "https://github.com/ClementPerroud/Gym-Trading-Env"
 "Bug Tracker" = "https://github.com/ClementPerroud/Gym-Trading-Env/issues"
```

### Comparing `gym-trading-env-0.1.1/src/gym_trading_env/environments.py` & `gym-trading-env-0.1.2/src/gym_trading_env/environments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import gym
-from gym import spaces
+import gymnasium as gym
+from gymnasium import spaces
 import pandas as pd
 import numpy as np
 import datetime
 import glob
+from pathlib import Path    
 
 from collections import Counter
 from .utils.history import History
 from .utils.portfolio import Portfolio, TargetPortfolio
 
 import tempfile, os
 import warnings
@@ -77,17 +78,16 @@
         if self.windows is None: _step_index = self._step
         else: _step_index = np.arange(self._step + 1 - self.windows , self._step + 1)
         return {
             "features" : self._obs_array[_step_index],
             "position" : self._position
             }
     
-    def reset(self, seed = None, df = None):
+    def reset(self, seed = None):
         super().reset(seed = seed)
-        if df is not None: self._set_df(df)
         self._step = 0
         self._limit_orders = {}
         if self.windows is not None: self._step = self.windows
 
         self._portfolio  = TargetPortfolio(
             position=self.initial_position,
             value= self.portfolio_initial_value,
@@ -174,23 +174,32 @@
         history_df.sort_index(inplace = True)
         render_df = self.df.join(history_df, how = "inner")
         
         if not os.path.exists(dir):os.makedirs(dir)
         render_df.to_pickle(f"{dir}/{self.name}_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}.pkl")
 
 class MultiDatasetTradingEnv(TradingEnv):
-    def __init(self, dataset_dir, *args, **kwargs):
+    def __init__(self, dataset_dir, preprocess, *args, **kwargs):
         self.dataset_dir = dataset_dir
+        self.preprocess = preprocess
         self.dataset_pathes = glob.glob(self.dataset_dir)
         self.dataset_nb_uses = np.zeros(shape=(len(self.dataset_pathes), ))
-        df = self.pick_dataset()
-        super().__init__(df, *args, **kwargs)
+        super().__init__(self.next_dataset(), *args, **kwargs)
 
-    def pick_dataset(self):
+    def next_dataset(self):
         # Find the indexes of the less explored dataset
         potential_dataset_pathes = np.where(self.dataset_nb_uses == self.dataset_nb_uses.min())[0]
         # Pick one of them
         random_int = np.random.randint(potential_dataset_pathes.size)
         dataset_path = self.dataset_pathes[random_int]
         self.dataset_nb_uses[random_int] += 1 # Update nb use counts
-        return pd.read_pickle(dataset_path)
+
+        self.name = Path(dataset_path).name
+        return self.preprocess(pd.read_pickle(dataset_path))
+
+    def reset(self, seed=None):
+        self._set_df(
+            self.next_dataset()
+        )
+        print(f"Selected dataset {self.name} ...")
+        return super().reset(seed)
```

### Comparing `gym-trading-env-0.1.1/src/gym_trading_env/renderer.py` & `gym-trading-env-0.1.2/src/gym_trading_env/renderer.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import glob
 import pandas as pd
 
 
 class Renderer():
     def __init__(self, render_logs_dir):
         self.app = Flask(__name__, static_folder="./templates/")
-        self.app.debug = True
         self.app.config["EXPLAIN_TEMPLATE_LOADING"] = True
         self.df = None
         self.render_logs_dir = render_logs_dir
         self.metrics = [
             {
                 "name": "Market Return",
                 "function" : lambda df : f"{(df['close'].iloc[-1] / df['close'].iloc[0] - 1)*100:0.2f}%",
```

### Comparing `gym-trading-env-0.1.1/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.1.2/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.1/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.1.2/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.1/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.1.2/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.1/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.1.2/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,16 +51,18 @@
 ```
 
 ## Environment Properties
 
 ### Actions space : positions
 
 Github is full of environments that consider actions such as **BUY**, **SELL**. In my opinion, it is a real mistake to consider a reinforcement learning agent in the same way as a trader. Traders make trade and to do so, they place orders on the market (eg. Buy X of stock Y). But what really matter is the position reached. Now, imagine we labelled each position by a number :
-- ```1``` : All of our portfolio is converted into stock Y. *BUY ALL*
-- ```0``` : All of our portfolio is converted into our fiat currency. *SELL ALL*
+- ```1``` : All of our portfolio is converted into stock Y. (=*BUY ALL*)
+- ```0``` : All of our portfolio is converted into our fiat currency. (=*SELL ALL*)
+
+
 Now, we can imagine half position and other variants :
 - ```0.5``` : 50% in stock Y & 50% in currency
 - Even : ```0.1``` : 10% in stock Y & 90% in currency
 ....
 
 
 In fact, it is way simpler for a RL-agent to work with positions. This way, it can easily make complex operation with a simple action space.
@@ -79,15 +81,32 @@
 ```python
 # Available in the github repo : test/data/BTC_USD-Hourly.csv
 df = pd.read_csv("data/BTC_USD-Hourly.csv", parse_dates=["date"], index_col= "date")
 df.sort_index(inplace= True)
 df.dropna(inplace= True)
 df.drop_duplicates(inplace=True)
 ```
-**2 - Create your feature**. Your RL-agent will need some good, preprocessed features. It is your job to make sure it has everything it needs.
+**1.1 (Optional) Download data** : The package provide a easy way to download data (works with CCTX ans use asyncio to get FAST) :
+```python
+from gym_trading_env.downloader import download
+import datetime
+
+download(
+    exchange_names = ["binance", "bitfinex2", "huobi"],
+    symbols= ["BTC/USDT", "ETH/USDT"],
+    timeframe= "30m",
+    dir = "test/data",
+    since= datetime.datetime(year= 2019, month= 1, day=1),
+    until = datetime.datetime(year= 2023, month= 1, day=1),
+)
+```
+This function use pickle format to save the OHLCV data. You will need to import the dataset with ```pd.read_pickle('... .pkl', ...)```. The function supports exchange_names ```binance```, ```biftfinex2``` (API v2) and ```huobi```.
+
+
+**2 - Create your features**. Your RL-agent will need some good, preprocessed features. It is your job to make sure it has everything it needs.
 **The feature column names need to contain the keyword 'feature'. The environment will automatically detect them !**
 
 ```python
 df["feature_close"] = df["close"].pct_change()
 df["feature_open"] = df["open"]/df["close"]
 df["feature_high"] = df["high"]/df["close"]
 df["feature_low"] = df["low"]/df["close"]
@@ -103,43 +122,51 @@
 The history object is similar to a DataFrame. It uses timestep and/or columns to access its values. You can use it this way :
 - ```history['column name', t]``` returns the a *scalar* value of the metrics 'column name' at time step t.
 - ```history['column name']``` returns a *numpy array* with all the values from timestep 0 to current timestep.
 - ```history[t]``` returns a *dictionnary* with of the metrics as keys with the associated values.
 
 
 Accessible columns of history object :
-- ```step```: ...,# Step = t
-- ```date```: ...,# Date at step t, datetime
-- ```reward```: ..., # Reward at step t
-- ```position_index```: ..., # Index of the position at step t amoung your position argument
-- ```position``` : ..., # Portfolio position at step t
+- ```step``` : Step = t.
+- ```date``` : Date at step t, datetime.
+- ```reward``` : Reward at step t.
+- ```position_index``` : Index of the position at step t amoung your position argument.
+- ```position``` : Portfolio position at step t.
+- ```portfolio_valuation```: Global valuation of the portfolio.
 
     *It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :*
-- ```data_close```: Close price,
-- ```data_open```: Open price,
-- ```data_high```:Hight price,
+- ```data_close``` : Close price.
+- ```data_open``` : Open price.
+- ```data_high``` : High price.
 
     *......*
 
-- ```portfolio_valuation```: Global valuation of the portfolio
-
-
     *It stores the distribution of the portfolio :*
-- ```portfolio_distribution_asset``` : The amount of owned asset (stock),
-- ```portfolio_distribution_fiat``` : The amount of owned fiat currency,
-- ```portfolio_distribution_borrowed_asset```: The amount of borrowed asset,
-- ```portfolio_distribution_borrowed_fiat```: The amount of borrowed fiat currency,
-- ```portfolio_distribution_interest_asset```: The total of cumalated interest generated by the borrowed asset.
-- ```portfolio_distribution_interest_fiat```: The total of cumalated interest generated by the borrowed fiat currency.
+- ```portfolio_distribution_asset``` : The amount of owned asset (stock).
+- ```portfolio_distribution_fiat``` : The amount of owned fiat currency.
+- ```portfolio_distribution_borrowed_asset``` : The amount of borrowed asset.
+- ```portfolio_distribution_borrowed_fiat``` : The amount of borrowed fiat currency.
+- ```portfolio_distribution_interest_asset``` : The total of cumalated interest generated by the borrowed asset.
+- ```portfolio_distribution_interest_fiat``` : The total of cumalated interest generated by the borrowed fiat currency.
 
 
-**4 - Create the environment**
+**4 - Initiate the environment**
 
 ```python
-env = TradingEnv(...)
+env = TradingEnv(
+        name= "BTCUSD",
+        df = df,
+        windows= 5,
+        positions = [ -1, -0.5, 0, 0.5, 1], # From -1 (=SHORT), to +1 (=LONG)
+        initial_position = 0,
+        trading_fees = 0.01/100, # 0.01% per stock buy / sell (Binance fees)
+        borrow_interest_rate= 0.0003/100, # 0.0003% per timestep (= 1h here)
+        reward_function = reward_function,
+        portfolio_initial_value = 1000, # here, in USDT
+    )
 ```
 Parameters :
 - ```name``` (required) : Name of your asset / symbol
 - ```df``` (required) : DataFrame containing technical indicators ```open```, ```high```, ```low```, ```close```, ```volume```, and the features you want to be returned as observations (containing ```feature``` in their column names).
 - ```windows```(optional, default : None), If None, observation at t are the features at step t  (classic mode). If windows = i (int),  observation at t are the features from steps [t-i+1 :  t] (useful for reccurent models)
 - ```positions``` (optional, default : [0, 1]). Positions that the agent can choose (Explained in "Actions space : positions")
 - ```initial_position``` (optional, default : 0). Initial position of the portfolio
@@ -171,68 +198,60 @@
 
 For the render not to perturb the training, the render needs to be performed in a separate python script. This way you have plenty of time to perform analysis on your results. 
 
 First, you need to save your results at the end of every episode you want to render with ```env.save_for_render(...)```. And decide which file you want your logs to be stored in with paramter ```dir```. For example :
 
 ```python
 ...
-# At the end of episode you want to render
+# At the end of the episode you want to render
 env.save_for_render(dir = "render_logs")
 ```
 
 Then in the separated render script. You can import and initiate a render object, and run the render in a localhost web app :
 ```python
 from gym_trading_env.renderer import Renderer
-renderer = Renderer(render_dir="render_logs")
+renderer = Renderer(render_logs_dir="render_logs")
 renderer.run()
 ```
 
 You can add **metrics** and plot **lines** with :
 ```python
-# Add lines
-# - Simple Moving Average - 10
-renderer.add_scatter(
-        name = "sma10",
-        function = lambda df : df["close"].rolling(10).mean(),
-        scatter_args = {
-            "line": {"color":'blue'}
-        })
-# - Simple Moving Average - 40
-renderer.add_scatter(
-        name = "sma40",
-        function = lambda df : df["close"].rolling(40).mean(),
-        scatter_args = {
-            "line": {"color": "purple"}
-        })
-
-# Add metrics 
-def max_drawdown(df):
-    current_max = df["portfolio_valuation"].iloc[0]
-    max_drawdown = 0
-    for i in range(len(df)):
-        current_max = max(df["portfolio_valuation"].iloc[i], current_max)
-        max_drawdown = min(max_drawdown, (df["portfolio_valuation"].iloc[i] - current_max)/current_max)
-    return f"{max_drawdown*100:0.2f}%"
+renderer = Renderer(render_logs_dir="render_logs")
 
-renderer.add_metric("Max drawdown", max_drawdown)
+# Add Custom Lines (Simple Moving Average)
+renderer.add_line( name= "sma10", function= lambda df : df["close"].rolling(10).mean(), line_options ={"width" : 1, "color": "purple"})
+renderer.add_line( name= "sma20", function= lambda df : df["close"].rolling(20).mean(), line_options ={"width" : 1, "color": "blue"})
+
+# Add Custom Metrics (Annualized metrics)
+renderer.add_metric(
+    name = "Annual Market Return",
+    function = lambda df : f"{ ((df['close'].iloc[-1] / df['close'].iloc[0])**(pd.Timedelta(days=365)/(df.index.values[-1] - df.index.values[0]))-1)*100:0.2f}%"
+)
+
+renderer.add_metric(
+        name = "Annual Portfolio Return",
+        function = lambda df : f"{((df['portfolio_valuation'].iloc[-1] / df['portfolio_valuation'].iloc[0])**(pd.Timedelta(days=365)/(df.index.values[-1] - df.index.values[0]))-1)*100:0.2f}%"
+)
+
+renderer.run()
 ```
 
 <img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render_customization.gif?raw=true" width = "800"/>
 
 
 
-```.add_scatter``` takes arguments :
-- ```name``` : The name of the scatter
-- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
-- ```scatter_args``` : Paramaters added to the go.Scatter object during the process. It can be used to customize your plots. The [documentation of the go.Scatter object](https://plotly.com/python-api-reference/generated/plotly.graph_objects.Scatter.html) might help you.
+```.add_line``` takes arguments :
+- ```name``` (*required*): The name of the scatter
+- ```function``` (*required*): The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
+- ```line_options``` : Can contain a dict with keys ```color``` and ```width```
 
 
 ```.add_metric``` takes arguments :
 - ```name``` : The name of the metric
-- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a scalar.
+- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a **string** !
 
 
 Enjoy :)
```

