# Comparing `tmp/qesdk-0.1.1.tar.gz` & `tmp/qesdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qesdk-0.1.1.tar", last modified: Sat Mar 18 15:23:40 2023, max compression
+gzip compressed data, was "qesdk-0.1.3.tar", last modified: Mon Apr 10 16:43:13 2023, max compression
```

## Comparing `qesdk-0.1.1.tar` & `qesdk-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 15:23:40.628787 qesdk-0.1.1/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       36 2022-09-22 03:32:43.000000 qesdk-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6225 2023-03-18 15:23:40.628787 qesdk-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.1/README.md
--rw-rw-rw-   0        0        0      751 2023-03-18 15:22:52.000000 qesdk-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-18 15:23:40.628787 qesdk-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-18 15:23:40.611788 qesdk-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-18 15:23:40.618788 qesdk-0.1.1/src/qesdk/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.1/src/qesdk/__init__.py
--rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.1/src/qesdk/aio_api.py
--rw-rw-rw-   0        0        0    25690 2023-03-14 02:20:42.000000 qesdk-0.1.1/src/qesdk/api.py
--rw-rw-rw-   0        0        0     4915 2023-03-18 15:22:41.000000 qesdk-0.1.1/src/qesdk/client.py
--rw-rw-rw-   0        0        0      183 2022-09-19 13:40:24.000000 qesdk-0.1.1/src/qesdk/config.py
--rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.1/src/qesdk/qedata.thrift
--rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.1/src/qesdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-18 15:23:40.622787 qesdk-0.1.1/src/qesdk.egg-info/
--rw-rw-rw-   0        0        0     6225 2023-03-18 15:23:40.000000 qesdk-0.1.1/src/qesdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-03-18 15:23:40.000000 qesdk-0.1.1/src/qesdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 15:23:40.000000 qesdk-0.1.1/src/qesdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-03-18 15:23:40.000000 qesdk-0.1.1/src/qesdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-03-18 15:23:40.000000 qesdk-0.1.1/src/qesdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-18 15:23:40.627787 qesdk-0.1.1/src/qesdk2/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.1/src/qesdk2/__init__.py
--rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.1/src/qesdk2/aio_api.py
--rw-rw-rw-   0        0        0    25580 2023-03-01 05:53:03.000000 qesdk-0.1.1/src/qesdk2/api.py
--rw-rw-rw-   0        0        0     4812 2023-02-14 10:32:25.000000 qesdk-0.1.1/src/qesdk2/client.py
--rw-rw-rw-   0        0        0      178 2022-11-30 10:59:44.000000 qesdk-0.1.1/src/qesdk2/config.py
--rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.1/src/qesdk2/utils.py
--rw-rw-rw-   0        0        0     1020 2023-03-16 12:44:25.000000 qesdk-0.1.1/src/test.py
--rw-rw-rw-   0        0        0     1628 2023-03-07 07:21:37.000000 qesdk-0.1.1/src/test2.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:43:13.750422 qesdk-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       36 2022-09-22 03:32:43.000000 qesdk-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6225 2023-04-10 16:43:13.750422 qesdk-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.3/README.md
+-rw-rw-rw-   0        0        0      751 2023-04-10 16:40:33.000000 qesdk-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 16:43:13.750924 qesdk-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 16:43:13.732923 qesdk-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 16:43:13.739424 qesdk-0.1.3/src/qesdk/
+-rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.3/src/qesdk/__init__.py
+-rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.3/src/qesdk/aio_api.py
+-rw-rw-rw-   0        0        0    29118 2023-04-10 16:39:22.000000 qesdk-0.1.3/src/qesdk/api.py
+-rw-rw-rw-   0        0        0     4929 2023-04-10 16:40:24.000000 qesdk-0.1.3/src/qesdk/client.py
+-rw-rw-rw-   0        0        0      183 2022-09-19 13:40:24.000000 qesdk-0.1.3/src/qesdk/config.py
+-rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.3/src/qesdk/qedata.thrift
+-rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.3/src/qesdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:43:13.744423 qesdk-0.1.3/src/qesdk.egg-info/
+-rw-rw-rw-   0        0        0     6225 2023-04-10 16:43:13.000000 qesdk-0.1.3/src/qesdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-04-10 16:43:13.000000 qesdk-0.1.3/src/qesdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 16:43:13.000000 qesdk-0.1.3/src/qesdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-10 16:43:13.000000 qesdk-0.1.3/src/qesdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-10 16:43:13.000000 qesdk-0.1.3/src/qesdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 16:43:13.749424 qesdk-0.1.3/src/qesdk2/
+-rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.3/src/qesdk2/__init__.py
+-rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.3/src/qesdk2/aio_api.py
+-rw-rw-rw-   0        0        0    25580 2023-03-01 05:53:03.000000 qesdk-0.1.3/src/qesdk2/api.py
+-rw-rw-rw-   0        0        0     4812 2023-02-14 10:32:25.000000 qesdk-0.1.3/src/qesdk2/client.py
+-rw-rw-rw-   0        0        0      178 2022-11-30 10:59:44.000000 qesdk-0.1.3/src/qesdk2/config.py
+-rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.3/src/qesdk2/utils.py
+-rw-rw-rw-   0        0        0     1056 2023-04-10 16:39:06.000000 qesdk-0.1.3/src/test.py
+-rw-rw-rw-   0        0        0     1628 2023-03-07 07:21:37.000000 qesdk-0.1.3/src/test2.py
```

### Comparing `qesdk-0.1.1/LICENSE` & `qesdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.1/PKG-INFO` & `qesdk-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.1
+Version: 0.1.3
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qesdk-0.1.1/README.md` & `qesdk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.1/pyproject.toml` & `qesdk-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qesdk"
-version = "0.1.1"
+version = "0.1.3"
 authors = [
   { name="Scott Zhang", email="scott2011@qq.com" },
 ]
 description = "Quantease SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `qesdk-0.1.1/src/qesdk/aio_api.py` & `qesdk-0.1.3/src/qesdk/aio_api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.1/src/qesdk/api.py` & `qesdk-0.1.3/src/qesdk2/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,18 +282,14 @@
     if len(instid) < 2:
         return instid
     if prod[1].isdigit():
         prod = prod[:1]
     return prod
 
 @assert_auth
-def get_all_products():
-    return qedataClient().instance()('get_all_products',**locals())
-
-@assert_auth
 def get_realtime_minute_prices(insts):
     if isinstance(insts, str):
         insts = [insts]
     if not isinstance(insts,list) :
         print('insts必须是合法合约的list')
         return None
     instids = json.dumps(insts)
```

### Comparing `qesdk-0.1.1/src/qesdk/client.py` & `qesdk-0.1.3/src/qesdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     server_config = outside_server_config
 except ImportError:
     server_config = {'host' : '192.168.123.13',
                      'port' : 6001}    
 
 
 
-__version__='0.1.1'
+__version__='0.1.3'
 
 thrift_path = path.join(sys.modules["ROOT_DIR"], "qedata.thrift")
 thrift_path = path.abspath(thrift_path)
 #print(thrift_path)
 qedata_thrift = thriftpy2.load(thrift_path, module_name="qedata_thrift")
 loop = asyncio.get_event_loop()
 def setTimeout(client, timeout):
@@ -142,18 +142,18 @@
             return True
         else:
             print(f'AUTH FAILED : {result.msg}')
             return False
             
     
 def auth(username, authcode):
-    asyncio.run(qedataClient.auth(username, authcode))
+    return asyncio.run(qedataClient.auth(username, authcode))
 
 def login(username, password):
-    asyncio.run(qedataClient.login(username, password))
+    return asyncio.run(qedataClient.login(username, password))
 
 def check_auth():
     return qedataClient.check_auth()
     
     
 def testClient():
     #loop.run_until_complete(qedataClient.instance().auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.'))
```

### Comparing `qesdk-0.1.1/src/qesdk/qedata.thrift` & `qesdk-0.1.3/src/qesdk/qedata.thrift`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.1/src/qesdk/utils.py` & `qesdk-0.1.3/src/qesdk/utils.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.1/src/qesdk.egg-info/PKG-INFO` & `qesdk-0.1.3/src/qesdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.1
+Version: 0.1.3
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qesdk-0.1.1/src/qesdk2/aio_api.py` & `qesdk-0.1.3/src/qesdk2/aio_api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.1/src/qesdk2/api.py` & `qesdk-0.1.3/src/qesdk/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -282,14 +282,18 @@
     if len(instid) < 2:
         return instid
     if prod[1].isdigit():
         prod = prod[:1]
     return prod
 
 @assert_auth
+def get_all_products():
+    return qedataClient().instance()('get_all_products',**locals())
+
+@assert_auth
 def get_realtime_minute_prices(insts):
     if isinstance(insts, str):
         insts = [insts]
     if not isinstance(insts,list) :
         print('insts必须是合法合约的list')
         return None
     instids = json.dumps(insts)
@@ -401,27 +405,85 @@
             dbname = "futures_daily" if freqtype == 1 else "futures_minu"
         del dfcols
         return qedataClient.instance()('get_price',**locals())
     except Exception as e:
         print("get_price Error:", e.__traceback__.tb_lineno,e)
         return None
 
+
+
 @assert_auth
-def get_bar_data(instids, tradingday, count=0):
+def get_bar_data(instids, tradingday, count=0, freq=1):
     try:
         assert isinstance(instids, list),'instids 必须是合约名list'
         #tnames = [inst2tablename(inst) for inst in instids]
         if isinstance(tradingday, str):
             tday = tradingday.replace('-','')
+            if tday == '':
+                tday = datetime.now().strftime('%Y%m%d')
         elif isinstance(tradingday, datetime) or isinstance(tradingday, date):
             tday = tradingday.strftime('%Ym%d')
         else:
             raise TypeError
         instids = json.dumps(instids)    
-        return qedataClient.instance()('get_bar_data', **locals())    
+        lcount = count
+        if freq != 1:
+            count = 0
+        data = qedataClient.instance()('get_bar_data', **locals())
+       #print(data)
+        if data:
+                f=str(freq)+'min'
+                for instid in data.keys():  
+                    df=data[instid]
+                    if len(df) > 0:
+                        #print(df.time)
+                        df['runtime']= pd.to_datetime(df.time, format='%Y%m%d%H%M%S',errors='ignore')
+                        #for i in range(len(df['time'])):
+                        #    df['runtime'].loc[i]=datetime.datetime.strptime(str(df['time'].loc[i]), "%Y%m%d%H%M%S")
+                        df.set_index(["runtime"], inplace=True)
+                        #print(df)
+                        if f=='1min':
+                            del data[instid]['time']
+                        else:
+                            df2 = pd.DataFrame(columns=df.columns)
+                            #print('111',df2)
+                            for col in df.columns:
+                                tmp = pd.Series(index=df.index, data=df.loc[:,col])
+                                if col == "open":
+                                    tmp=df[col].resample(f, label='right', closed='right').first()
+                                elif col =="close":
+                                    tmp=df[col].resample(f, label='right', closed='right').last()
+                                elif col == 'high':
+                                    tmp=df[col].resample(f, label='right', closed='right').max()
+                                elif col == 'low':
+                                    tmp=df[col].resample(f, label='right', closed='right').min()
+                                elif col == 'volume':
+                                    tmp=df[col].resample(f, label='right', closed='right').sum()
+                                elif col == 'money':
+                                    tmp=df[col].resample(f, label='right', closed='right').sum()
+                                elif col == 'position':
+                                    tmp = df[col].resample(f, label='right', closed='right').last()
+                                elif col == 'presett':
+                                    tmp=df[col].resample(f, label='right', closed='right').last()
+                                elif col == 'preclose':
+                                    tmp=df[col].resample(f, label='right', closed='right').last()
+                                elif col == 'lowerlimit':
+                                    tmp=df[col].resample(f, label='right', closed='right').last()
+                                elif col == 'upperlimit':
+                                    tmp=df[col].resample(f, label='right', closed='right').last()
+                                elif col == 'tradingday':
+                                    tmp=df[col].resample(f, label='right', closed='right').last()
+                                df2.loc[:,col] = tmp
+                            #print(df2)
+                            del df2['time']
+                            if isinstance(lcount, int) and lcount > 0:
+                                data[instid]=df2.dropna(how='any').iloc[-lcount:,]
+                            else:
+                                data[instid]=df2.dropna(how='any')
+        return data
     except Exception as e:
         print("get_bar_data Error:", e.__traceback__.tb_lineno,e)
         return None
 
 @assert_auth
 def get_broker_info(broker):
     try:
```

### Comparing `qesdk-0.1.1/src/qesdk2/client.py` & `qesdk-0.1.3/src/qesdk2/client.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.1/src/qesdk2/utils.py` & `qesdk-0.1.3/src/qesdk2/utils.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.1/src/test.py` & `qesdk-0.1.3/src/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 Created on Fri Sep 23 21:41:10 2022
 
 @author: ScottStation
 """
 
 
 import qesdk
-#qesdk.auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.')
-qesdk.auth('qestratmarket','$1$$BbR4MSZT9isFx3PBepvxd/')
+qesdk.auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.')
+#qesdk.auth('qestratmarket','$1$$BbR4MSZT9isFx3PBepvxd/')
 #qesdk.auth('Scott_1665208401','$1$$oaWXYSWPp1jpTQmndXJcK/')
 #print(qesdk.check_auth())
-
+'''
 qesdk.login('scott','12345678')
 stratlist=(qesdk.sm_get_clone_strat_list())
 print('strats',stratlist)
 if stratlist and isinstance(stratlist,list) and len(stratlist) > 0:
     print(qesdk.sm_get_clone_strat_position(stratlist))
-
+'''
 #df = qesdk.get_instrument_broker_pnl('东证期货','AU2306.SFE','2023-02-24','2023-02-28')
 #df = qesdk.get_product_invent_orders('CU', '2023-02-01','2023-02-14')
-df = qesdk.get_bar_data(['510300.SSE'], '',1)
+inst = 'AU2312.SFE'
+data = qesdk.get_bar_data([inst], '',5,freq=5)
 #df = qesdk.get_realtime_minute_prices(['AU2312.SFE','AG2401.SFE'])
-print(df)
+print(data[inst])
 #print(df['510300.SSE'].columns)
     
 #qesdk.auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.')
 #
 #print(df)
 #print(qesdk2.get_price('AG2212.SFE','2022-09-01','2022-09-22'))
```

### Comparing `qesdk-0.1.1/src/test2.py` & `qesdk-0.1.3/src/test2.py`

 * *Files identical despite different names*

