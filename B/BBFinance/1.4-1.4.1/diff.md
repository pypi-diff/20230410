# Comparing `tmp/BBFinance-1.4.tar.gz` & `tmp/BBFinance-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.4.tar", last modified: Mon Apr 10 01:07:53 2023, max compression
+gzip compressed data, was "BBFinance-1.4.1.tar", last modified: Mon Apr 10 14:04:40 2023, max compression
```

## Comparing `BBFinance-1.4.tar` & `BBFinance-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 01:07:53.456663 BBFinance-1.4/
-drwxrwxrwx   0        0        0        0 2023-04-10 01:07:53.427662 BBFinance-1.4/BBFinance/
--rw-rw-rw-   0        0        0    38911 2023-04-10 01:06:27.000000 BBFinance-1.4/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      289 2023-04-07 23:16:39.000000 BBFinance-1.4/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:07:53.454686 BBFinance-1.4/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     1995 2023-04-10 01:07:53.000000 BBFinance-1.4/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-04-10 01:07:53.000000 BBFinance-1.4/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:07:53.000000 BBFinance-1.4/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      275 2023-04-10 01:07:53.000000 BBFinance-1.4/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 01:07:53.000000 BBFinance-1.4/BBFinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1099 2023-04-07 01:44:35.000000 BBFinance-1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1995 2023-04-10 01:07:53.456663 BBFinance-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-04-07 01:44:35.000000 BBFinance-1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 01:07:53.457661 BBFinance-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1326 2023-04-10 01:06:48.000000 BBFinance-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:08:03.823386 BBFinance-1.4.1/
+drwxrwxrwx   0        0        0        0 2023-04-10 14:08:01.416781 BBFinance-1.4.1/BBFinance/
+-rw-rw-rw-   0        0        0    39408 2023-04-10 14:06:03.000000 BBFinance-1.4.1/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      325 2023-04-10 14:07:15.000000 BBFinance-1.4.1/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:08:02.885811 BBFinance-1.4.1/BBFinance/__pycache__/
+-rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.1/BBFinance/__pycache__/BBFinance.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8391 2023-04-06 19:36:07.000000 BBFinance-1.4.1/BBFinance/__pycache__/BBFinance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.1/BBFinance/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      306 2023-04-06 19:20:52.000000 BBFinance-1.4.1/BBFinance/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-04-10 14:08:02.166840 BBFinance-1.4.1/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     1997 2023-04-10 14:07:50.000000 BBFinance-1.4.1/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-04-10 14:07:59.000000 BBFinance-1.4.1/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:07:50.000000 BBFinance-1.4.1/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      255 2023-04-10 14:07:50.000000 BBFinance-1.4.1/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 14:07:50.000000 BBFinance-1.4.1/BBFinance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 14:08:03.151448 BBFinance-1.4.1/Data/
+-rw-rw-rw-   0        0        0    14286 2023-04-10 14:00:41.000000 BBFinance-1.4.1/Data/AtivosIbov.xlsx
+-rw-rw-rw-   0        0        0     1099 2023-04-04 20:31:26.000000 BBFinance-1.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1997 2023-04-10 14:08:03.807761 BBFinance-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-04-06 20:03:42.000000 BBFinance-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 14:08:03.573370 BBFinance-1.4.1/__pycache__/
+-rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.1/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.1/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0      300 2023-04-04 20:31:26.000000 BBFinance-1.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:08:03.839011 BBFinance-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2023-04-10 14:07:14.000000 BBFinance-1.4.1/setup.py
+-rw-rw-rw-   0        0        0       66 2023-04-10 11:52:03.000000 BBFinance-1.4.1/teste.py
```

### Comparing `BBFinance-1.4/BBFinance/BBFinance.py` & `BBFinance-1.4.1/BBFinance/BBFinance.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     Outros = 'Outros'
 
 class TipoPerfis(str, Enum):
     Agressivo = 'Agressivo'
     Moderado = 'Moderado'
     Conservador = 'Conservador'
 
+
 def formataValoresNumero(df, nomeColuna):
     df[nomeColuna] = df[nomeColuna].replace('[.]', '', regex=True)
     df[nomeColuna] = df[nomeColuna].replace('[%]', '', regex=True)
     df[nomeColuna] = df[nomeColuna].replace('[,]', '.', regex=True)
     df[nomeColuna] = df[nomeColuna].astype(float)
 
     return df
@@ -113,22 +114,24 @@
     
     # Crie um objeto JSON com as informações da ação
     json_data = {'symbol': symbol, 
                  'current_price': current_price, 
                  'company_name': company_name,
                  'dividends' : dividend}
     
-    formatted_json = json.dumps(json_data, indent=5)
-    print(formatted_json)
+    # formatted_json = json.dumps(json_data, indent=4)
+
+    return json_data
 
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/info")
 response = Response(media_type="application/json")
 
 
+
 ## HISTORICO DAS AÇOES ##
 
 @app.get("/stocks/{symbol}/history", response_model=None)
 def get_stock_history(symbol: str, period: str = '1y') -> pd.DataFrame:
     
     """
     ## Usabilidade 
@@ -152,16 +155,18 @@
     
     history = stock.history(period=period)
     
     if history.empty:
         return {"error": print("No data found")}
     else:
         history_dict = history.to_dict(orient="list")
-        history_df = pd.DataFrame.from_dict(history_dict).reset_index(drop=False)     
-        return print(history_df)
+        history_df = pd.DataFrame.from_dict(history_dict).reset_index(drop=False)
+
+        return history_df
+    
         # json_data = {'symbol': symbol,
         # "history":  history_df.to_dict(orient="records"),
         # }
 
         # formatted_json = json.dumps(json_data, indent=2)
         # print(formatted_json)
 
@@ -198,16 +203,17 @@
     close_prices = history['Close']
     trend = 'up' if close_prices.iloc[-1] > close_prices.iloc[0] else 'down'
     
     json_data = { "symbol": symbol,
                 "trend": trend,
     }
     
-    formatted_json = json.dumps(json_data, indent=2)
-    print(formatted_json)
+    # formatted_json = json.dumps(json_data, indent=2)
+
+    return json_data
 
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/trend")
 responseHistory = Response(media_type="application/json")
 
 
 ## RSI ##
@@ -262,22 +268,22 @@
         "symbol": symbol,
         "sma_50": sma_50,
         "sma_200": sma_200,
         "rsi": rsi,
         "tendency" : status
     }
 
-    formatted_json = json.dumps(json_data, indent=4)
-    print(formatted_json)
+    # formatted_json = json.dumps(json_data, indent=4)
+
+    return json_data
 
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/technical")
 responseHistory = Response(media_type="application/json")
 
-
 ## VOLATILIDADE ##
 
 @app.get("stocks/{symbol}/volatility", response_model=None)
 def get_volatility(symbol: str, start_date: str, end_date: str) -> str:
     
     """
     ## Usabilidade 
@@ -294,21 +300,21 @@
         if stock_data.empty:
             return {"error": print("Nao foi encontrado o historico nesse periodo, verificar.")}
     except:
         pass
     
     log_returns = np.log(stock_data['Close']/stock_data['Close'].shift(1))
     volatility = np.sqrt(252*log_returns.var())
-    return {'volatility': print(volatility)}
+
+    return volatility
 
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/volatility")
 responseHistory = Response(media_type="application/json")
 
-
 ## BETA ##
 
 @app.get("stocks/{symbol}/beta", response_model=None)
 def get_beta(symbol: str) -> dict:
     
     """
     ## Usabilidade 
@@ -318,20 +324,20 @@
     ## Parâmetros
     - symbol -> Nome do Ativo para a busca \n
     - market -> Como padrao, Mercado: IBOVESPA / BVSP
     """
     
     # Obter os dados do ativo e do mercado
     try:
-        asset = yf.Ticker(symbol)
+        asset = yf.Ticker('PETR4.SA')
         market = yf.Ticker("^BVSP") # Índice Bovespa como mercado de referência
         info = asset.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO, SENAO VAI PASSAR
         infoMarket = market.info
         tipoInfo = type(info)
-        if tipoInfo == dict | infoMarket == dict:
+        if tipoInfo == dict or infoMarket == dict:
             pass 
     except:
         return {"error": print("Invalid ticker symbol")}
 
     asset_history = asset.history(period="max")
     market_history = market.history(period="max")
 
@@ -351,16 +357,17 @@
     if beta == 1:
         status =  'Acao com a mesma Volatilidade que o mercado em geral'
 
 
     json_data =  {"beta": beta,
                   "status" : status}
     
-    formatted_json = json.dumps(json_data, indent=2)
-    print(formatted_json)
+    # formatted_json = json.dumps(json_data, indent=2)
+
+    return json_data
 
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/beta")
 responseHistory = Response(media_type="application/json")
 
 
 ## VAR ##
@@ -394,16 +401,17 @@
 
     # Calcular o retorno diário da ação
     returns = np.log(prices / prices.shift(1))
 
     # Calcular o desvio padrão e o VaR histórico
     std_dev = returns.std()
     var = std_dev * norm.ppf(1 - confidence_level)
-
-    return print({"VaR": round(var * prices[-1], 2)})
+    print({"VaR": round(var * prices[-1], 2)})
+    Var = round(var * prices[-1], 2)
+    return Var
 
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/VaR")
 responseHistory = Response(media_type="application/json")
 
 
 ## CARTEIRA DE ATIVOS ##
@@ -457,16 +465,16 @@
                 'Ativo' : symbols,
                 'Preço a Mercado' : valueMarket,
                 'Retorno anual': retorno_anual,
                 'Desvio padrão anual': desvio_padrao_anual,
                 'Retorno total': retorno_total
             }, index=[1])
             
-            print(valueSymbols)
-
+            return valueSymbols
+        
         except:
             print("Ticker inválido")
   
     elif isinstance(symbols, list):
         valueDF = pd.DataFrame()
         print(f"Você digitou uma lista: {symbols}")
         for simbolo in symbols:
@@ -498,16 +506,16 @@
                 'Ativo' : simbolo,
                 'Retorno anual': retorno_anual,
                 'Desvio padrão anual': desvio_padrao_anual,
                 'Retorno total': retorno_total
             }, index=[len(symbols)])
             
             valueDF = pd.concat([returnSymbols, valueDF])
-        print(valueDF)
 
+        return valueDF
     else:
         print("Tipo inválido. Digite uma string ou uma lista.")
 
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="stocks/{symbol}/AnnualReturn")
 responseHistory = Response(media_type="application/json")
 
@@ -565,18 +573,17 @@
     for i in range(len(symbols)):
         taxas = f"O ativo {symbols[i]} deve ser alocado em {w_markowitz[i] * 100:.2f}% da carteira"
         markowitzList.append(taxas)
     json_data = {'Retorno Esperado' : retorno_esperado,
                  'Risco da Carteira' : risco,
                  'Alocacao Markowitz' : markowitzList}
     
-    formatted_json = json.dumps(json_data, indent=4, sort_keys=True)
-    print(formatted_json)
+    # formatted_json = json.dumps(json_data, indent=4, sort_keys=True)
     
-    return formatted_json
+    return json_data
     
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="stocks/{symbol}/MarkowitzAllocation")
 responseHistory = Response(media_type="application/json")
 
 
 ## BUSCA INFO DE FUNDOS ##
@@ -588,26 +595,26 @@
     soup = BeautifulSoup(response.content, "html.parser")
     table = soup.find_all("table")[0]
     fundsDF = pd.read_html(str(table))[0]    
     fundsDF['Código do fundo'] = fundsDF['Código do fundo'].apply(lambda x: x+'.SA')
         
     valuesFI = fundsDF.loc[(fundsDF['Código do fundo'] == symbol)]
     valuesFI = valuesFI[['Código do fundo', 'Setor', 'Preço Atual', 'Dividendo', 'Variação Preço', "Rentab. Período"]]
-    print(valuesFI)
+
     return valuesFI
 
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="/infoFunds")
 responseHistory = Response(media_type="application/json")
 
 
 ## COMPARADOR DE FUNDOS COM BASE NO SETOR ##
 
 @app.get("/compareSetorFunds", response_model=None)
-def compare_setor_funds(setor= TipoSetores, rentabilidade_min = 0) -> pd.DataFrame:
+def compare_setor_funds(setor: str, rentabilidade_min = 0) -> pd.DataFrame:
     
     """
     ## Usabilidade
     
     - Funçao que utiliza as metricas e medias dos fundo com base no seu Setor para uma analise mais restrita
     
     ## Parâmetros
@@ -616,69 +623,74 @@
     - setor -> Setores de fundos que poderam ser escolhidos, segue a lista:
     
     ```
     TiposSetores:
     - Corporativas = "Lajes Corporativas" 
     - Mobiliarios = "Títulos e Val. Mob."
     - Shoppings = "Shoppings"
-    - Hibridos = 'Híbrido'
+    - Híbrido = 'Híbrido'
     - Renda = 'Renda'
-    - Logistica = 'Logística'
+    - Logística = 'Logística'
     - Hospital = 'Hospital'
     - Residencial = 'Residencial'
     - Outros = 'Outros'
 
     ```
-    
     ## Exemplo:
     
     ```
     >>> bb.compare_setor_funds(setor='Corporativas', rentabilidade_min = 3)
     ```
-    
-    
+
     """
     
     url = "https://www.fundsexplorer.com.br/ranking"
     response = requests.get(url)
     soup = BeautifulSoup(response.content, "html.parser")
     table = soup.find_all("table")[0]
     fundsDF = pd.read_html(str(table))[0]
 
     formataValoresNumero(fundsDF, "Rentab. Período")
     rentabilidade_min = rentabilidade_min / 100
     valuesFI = fundsDF.loc[(fundsDF["Rentab. Período"]/100) > rentabilidade_min]
     valuesFI = valuesFI[['Código do fundo', 'Setor', 'Preço Atual', 'Dividendo', 'Variação Preço', "Rentab. Período"]]
     valuesFI = valuesFI.dropna()
     rentabilidade_media = valuesFI['Rentab. Período'].mean()
-    rentabilidade_mercado = valuesFI.loc[valuesFI["Setor"] == setor]["Rentab. Período"].mean()
-    
+    if setor == 'Corporativas':
+        setor = 'Lajes Corporativas'
+        rentabilidade_mercado = valuesFI.loc[valuesFI["Setor"] == setor]["Rentab. Período"].mean()
+    elif setor == 'Mobiliarios': 
+        setor = 'Títulos e Val. Mob.'
+        rentabilidade_mercado = valuesFI.loc[valuesFI["Setor"] == setor]["Rentab. Período"].mean()
+    else:
+        rentabilidade_mercado = valuesFI.loc[valuesFI["Setor"] == setor]["Rentab. Período"].mean()
+
     desvio_padrao = valuesFI["Rentab. Período"].std()
     
     resultados = pd.DataFrame({
         "Rentabilidade Média dos FIIs Selecionados": [rentabilidade_media],
         "Rentabilidade Média do Mercado": [rentabilidade_mercado],
         "Desvio Padrão das Rentabilidades dos FIIs Selecionados": [desvio_padrao]
     })
     
     resultados = resultados.fillna('O setor/valor nao foi encontrado')
-    print(resultados)
+
     return resultados
 
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="/compareSetorFunds")
 responseHistory = Response(media_type="application/json")
 
 
 ## COMPARADOR DE FUNDOS ##
 
 @app.get("/compareFunds", response_model=None)
 def compare_funds(listfund= None, fund_1= str, fund_2= str) -> pd.DataFrame:
     """
-    ## Usabilidade 
+    ## Usabilidade
     
     - Funçao que realiza a comparaçao entre dois fundos, seja feita a requisiçao dos fundos via lista ou unicos 
     - Requisiçao Listas: Retorna o fundo com maior porcentagem de risco (a variação percentual dos preços dos ativos, calculo realizado com base no desvio padrão)
     - Requisiçao Unica: Retorna um Dataframe com as principais informaçoes dos fundos, afim de uma comparaçao entre seus valores \n
     
     ## Parâmetros
     
@@ -709,15 +721,15 @@
         fund1 = fundsDF.loc[fundsDF["Código do fundo"] == fund_1]
         fund2 = fundsDF.loc[fundsDF["Código do fundo"] == fund_2]
 
         unit = pd.concat([fund1, fund2])
         if unit.empty:
             print('Nao foram apresentado dados dos fundos para verificaçao unica')
         else:
-            print(unit)
+            return unit
         
     if listfund is None:
         listfund = []
     else:
         max_risco = -1
         ticker_max_risco = ''
         for ticker in listfund:
@@ -730,27 +742,25 @@
             
         valuerisk = pd.DataFrame({'Fund' : ticker_max_risco,
                     'Max risk (%)' : max_risco * 100}, index=[len(listfund)])
         
         if valuerisk.empty:
             print('Nao foram apresentado dados dos fundos para verificaçao múltipla')
         else:
-            print(valuerisk)
-            
-    return valuerisk, unit
-            
+            return valuerisk
+                        
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="/compareFunds")
 responseHistory = Response(media_type="application/json")
 
 
 ## SIMULADOR DE AÇOES ##
 
 @app.get("/bestAssets", response_model=None)
-def best_assets(perfil= TipoPerfis) -> pd.DataFrame:
+def best_assets(perfil= str) -> pd.DataFrame:
     
     """
     ## Usabilidade
     - Função que analisa os principais ativos listados no mercado que com base no perfil escolhido mostra quais podem ser suas escolhas e quantos porcento se deve ter na carteira
     
     ## Parâmetros
     
@@ -813,19 +823,20 @@
             for ativo in precos.columns:
                 if retorno[ativo] > 0.0001 and risco[ativo] > 0.01:
                     agressivo.append(ativo)
             # print('Para um cliente agressivo, Ativos selecionados:', agressivo)
             DfAgressivo = pd.DataFrame(agressivo, columns=['Ativos P/Agressivo'])
             print('Realizando calculos para a sua carteira com base no seu perfil.')
             alocation_Agressive = markowitz_allocation(agressivo, star_date= oneY, end_date= currently )
-            dataAlocation_Agressive = json.loads(alocation_Agressive)
-            dataAlocation_Agressive = pd.DataFrame(dataAlocation_Agressive)
+            alocation_Agressive = [alocation_Agressive]
+            dataAlocation_Agressive = pd.DataFrame(alocation_Agressive)
+            dataAlocation_Agressive = dataAlocation_Agressive.explode('Alocacao Markowitz')
 
             # adiciona as quebras de linha na coluna "Alocacao Markowitz"
-            dataAlocation_Agressive['Alocacao Markowitz'] = dataAlocation_Agressive['Alocacao Markowitz'].replace('\n', '\\n', regex=True)
+            # dataAlocation_Agressive['Alocacao Markowitz'] = dataAlocation_Agressive['Alocacao Markowitz'].replace('\n', '\\n', regex=True)
             dataAlocation_Agressive['Retorno Esperado'] = dataAlocation_Agressive['Retorno Esperado'].drop_duplicates().dropna()
             dataAlocation_Agressive['Risco da Carteira'] = dataAlocation_Agressive['Risco da Carteira'].drop_duplicates().dropna()
             
             if dataAlocation_Agressive.empty:
                 pass
             else:
                 return dataAlocation_Agressive
@@ -836,19 +847,20 @@
             for ativo in precos.columns:
                 if retorno[ativo] > 0.0003 and risco[ativo] < 0.03:
                     moderado.append(ativo)
             # print('Para um cliente moderado, Ativos selecionados:', moderado)
             DfModerado = pd.DataFrame(moderado, columns=['Ativos P/Moderado'])
             print('Realizando calculos para a sua carteira com base no seu perfil.')
             alocation_Moderade = markowitz_allocation(moderado, star_date= oneY, end_date= currently )
-            dataAlocation_Moderade = json.loads(alocation_Moderade)
-            dataAlocation_Moderade = pd.DataFrame(dataAlocation_Moderade)
+            alocation_Moderade = [alocation_Moderade]
+            dataAlocation_Moderade = pd.DataFrame(alocation_Moderade)
+            dataAlocation_Moderade = dataAlocation_Moderade.explode('Alocacao Markowitz')
 
             # adiciona as quebras de linha na coluna "Alocacao Markowitz"
-            dataAlocation_Moderade['Alocacao Markowitz'] = dataAlocation_Moderade['Alocacao Markowitz'].replace('\n', '\\n', regex=True)
+            # dataAlocation_Moderade['Alocacao Markowitz'] = dataAlocation_Moderade['Alocacao Markowitz'].replace('\n', '\\n', regex=True)
             dataAlocation_Moderade['Retorno Esperado'] = dataAlocation_Moderade['Retorno Esperado'].drop_duplicates().dropna()
             dataAlocation_Moderade['Risco da Carteira'] = dataAlocation_Moderade['Risco da Carteira'].drop_duplicates().dropna()
             
             if dataAlocation_Moderade.empty:
                 pass
             else:
                 return dataAlocation_Moderade
@@ -859,19 +871,19 @@
             for ativo in precos.columns:
                 if risco[ativo] < 0.01:
                     conservador.append(ativo)
             DfConservador = pd.DataFrame(conservador, columns=['Ativos P/Conservador'])
             # print('Para um cliente conservador, Ativos selecionados:', conservador)
             print('Realizando calculos para a sua carteira com base no seu perfil.')
             alocation_Conservative = markowitz_allocation(conservador, star_date= oneY, end_date= currently )
-            dataAlocation_Conservative = json.loads(alocation_Conservative)
-            dataAlocation_Conservative = pd.DataFrame(dataAlocation_Conservative)
-
+            alocation_Conservative = [alocation_Conservative]
+            dataAlocation_Conservative = pd.DataFrame(alocation_Conservative)
+            dataAlocation_Conservative = dataAlocation_Conservative.explode('Alocacao Markowitz')
             # adiciona as quebras de linha na coluna "Alocacao Markowitz"
-            dataAlocation_Conservative['Alocacao Markowitz'] = dataAlocation_Conservative['Alocacao Markowitz'].replace('\n', '\\n', regex=True)
+            # dataAlocation_Conservative['Alocacao Markowitz'] = dataAlocation_Conservative['Alocacao Markowitz'].replace('\n', '\\n', regex=True)
             dataAlocation_Conservative['Retorno Esperado'] = dataAlocation_Conservative['Retorno Esperado'].drop_duplicates().dropna()
             dataAlocation_Conservative['Risco da Carteira'] = dataAlocation_Conservative['Risco da Carteira'].drop_duplicates().dropna()
             
             if dataAlocation_Conservative.empty:
                 pass
             else:
                 return dataAlocation_Conservative
@@ -893,15 +905,15 @@
     ## Parâmetros
     
     - valor -> Valor do investimento, por padrão 0
 
     """
     
     # Lista de ativos
-    ativos = pd.read_excel(r'C:\Users\Luis\ProjetoFin\BBFinance\Data\AtivosIbov.xlsx')
+    ativos = pd.read_excel(r'Q:\Risco\Novo Risco\pythonrisco\BBFinance\Data\AtivosIbov.xlsx')
     ativos['Código'] = ativos['Código'].apply(lambda x: x+'.SA')
 
     # Baixa os dados históricos dos ativos nos últimos 12 meses
     precos = yf.download(ativos['Código'].tolist(), period='1y')['Close']
 
     # Remove colunas com valores ausentes
     precos = precos.dropna(axis=1)
```

### Comparing `BBFinance-1.4/BBFinance.egg-info/PKG-INFO` & `BBFinance-1.4.1/BBFinance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4
+Version: 1.4.1
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.4/LICENSE.txt` & `BBFinance-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4/PKG-INFO` & `BBFinance-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4
+Version: 1.4.1
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.4/README.md` & `BBFinance-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4/setup.py` & `BBFinance-1.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.4',
+    version='1.4.1',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
     license='MIT',
     packages=['BBFinance'],
     long_description= long_description,
@@ -25,16 +25,15 @@
         'fastapi>=0.95.0',
         'scipy>=1.10.1',
         'requests>=2.28.2',
         'bs4>=0.0.1',
         'beautifulsoup4>=4.11.2',
         'pydantic>=1.10.7',
         'Unicode>=1.3.6',
-        'typing_extensions>=4.5.0',
-        'scikit-learn>=1.2.2'
+        'typing_extensions>=4.5.0'
         
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
```

