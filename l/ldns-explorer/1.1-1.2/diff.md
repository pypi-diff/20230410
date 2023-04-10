# Comparing `tmp/ldns-explorer-1.1.tar.gz` & `tmp/ldns-explorer-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/CD/Desktop/first/DNS/dist/.tmp-hpcgkveo/ldns-explorer-1.1.tar", last modified: Tue Apr  4 20:21:32 2023, max compression
+gzip compressed data, was "/Users/CD/Desktop/first/DNS/dist/.tmp-cc0kzenk/ldns-explorer-1.2.tar", last modified: Mon Apr 10 19:41:08 2023, max compression
```

## Comparing `ldns-explorer-1.1.tar` & `ldns-explorer-1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-04 20:21:32.190449 ldns-explorer-1.1/
--rw-r--r--   0 CD         (501) staff       (20)     1550 2023-04-04 20:21:32.190014 ldns-explorer-1.1/PKG-INFO
--rw-r--r--   0 CD         (501) staff       (20)     1290 2023-04-04 20:21:12.000000 ldns-explorer-1.1/README.md
--rw-r--r--   0 CD         (501) staff       (20)      403 2023-04-04 20:21:17.000000 ldns-explorer-1.1/pyproject.toml
--rw-r--r--   0 CD         (501) staff       (20)       38 2023-04-04 20:21:32.190602 ldns-explorer-1.1/setup.cfg
--rw-r--r--   0 CD         (501) staff       (20)      157 2023-03-28 20:00:36.000000 ldns-explorer-1.1/setup.py
-drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-04 20:21:32.183551 ldns-explorer-1.1/src/
--rw-r--r--   0 CD         (501) staff       (20)        0 2023-03-15 19:25:14.000000 ldns-explorer-1.1/src/__init__.py
--rw-r--r--   0 CD         (501) staff       (20)       67 2023-03-24 21:07:54.000000 ldns-explorer-1.1/src/envplay.py
-drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-04 20:21:32.185115 ldns-explorer-1.1/src/ldns_explorer.egg-info/
--rw-r--r--   0 CD         (501) staff       (20)     1550 2023-04-04 20:21:32.000000 ldns-explorer-1.1/src/ldns_explorer.egg-info/PKG-INFO
--rw-r--r--   0 CD         (501) staff       (20)      489 2023-04-04 20:21:32.000000 ldns-explorer-1.1/src/ldns_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 CD         (501) staff       (20)        1 2023-04-04 20:21:32.000000 ldns-explorer-1.1/src/ldns_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 CD         (501) staff       (20)       21 2023-04-04 20:21:32.000000 ldns-explorer-1.1/src/ldns_explorer.egg-info/requires.txt
--rw-r--r--   0 CD         (501) staff       (20)       30 2023-04-04 20:21:32.000000 ldns-explorer-1.1/src/ldns_explorer.egg-info/top_level.txt
-drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-04 20:21:32.189169 ldns-explorer-1.1/src/ldnsexplorer/
--rw-r--r--   0 CD         (501) staff       (20)     9841 2023-03-29 02:08:40.000000 ldns-explorer-1.1/src/ldnsexplorer/DNS_APP.py
--rw-r--r--   0 CD         (501) staff       (20)        0 2023-03-14 21:01:01.000000 ldns-explorer-1.1/src/ldnsexplorer/__init__.py
--rw-r--r--   0 CD         (501) staff       (20)       40 2023-03-28 16:23:49.000000 ldns-explorer-1.1/src/ldnsexplorer/__main__.py
--rw-r--r--   0 CD         (501) staff       (20)      303 2023-02-27 20:24:11.000000 ldns-explorer-1.1/src/ldnsexplorer/find_local_resolver.py
--rw-r--r--   0 CD         (501) staff       (20)     1439 2023-03-14 04:37:46.000000 ldns-explorer-1.1/src/ldnsexplorer/measure_dns.py
--rw-r--r--   0 CD         (501) staff       (20)      352 2023-03-14 04:52:05.000000 ldns-explorer-1.1/src/ldnsexplorer/measure_tcp.py
--rw-r--r--   0 CD         (501) staff       (20)     1584 2023-03-29 02:06:34.000000 ldns-explorer-1.1/src/ldnsexplorer/tcp_client.py
+drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 19:41:08.340955 ldns-explorer-1.2/
+-rw-r--r--   0 CD         (501) staff       (20)     2238 2023-04-10 19:41:08.340588 ldns-explorer-1.2/PKG-INFO
+-rw-r--r--   0 CD         (501) staff       (20)     1978 2023-04-10 19:39:49.000000 ldns-explorer-1.2/README.md
+-rw-r--r--   0 CD         (501) staff       (20)      403 2023-04-10 19:37:23.000000 ldns-explorer-1.2/pyproject.toml
+-rw-r--r--   0 CD         (501) staff       (20)       38 2023-04-10 19:41:08.341029 ldns-explorer-1.2/setup.cfg
+-rw-r--r--   0 CD         (501) staff       (20)      157 2023-03-28 20:00:36.000000 ldns-explorer-1.2/setup.py
+drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 19:41:08.333689 ldns-explorer-1.2/src/
+-rw-r--r--   0 CD         (501) staff       (20)        0 2023-03-15 19:25:14.000000 ldns-explorer-1.2/src/__init__.py
+-rw-r--r--   0 CD         (501) staff       (20)       67 2023-03-24 21:07:54.000000 ldns-explorer-1.2/src/envplay.py
+drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 19:41:08.336022 ldns-explorer-1.2/src/ldns_explorer.egg-info/
+-rw-r--r--   0 CD         (501) staff       (20)     2238 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 CD         (501) staff       (20)      489 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 CD         (501) staff       (20)        1 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 CD         (501) staff       (20)       21 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/requires.txt
+-rw-r--r--   0 CD         (501) staff       (20)       30 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 19:41:08.339727 ldns-explorer-1.2/src/ldnsexplorer/
+-rw-r--r--   0 CD         (501) staff       (20)     9852 2023-04-10 19:40:55.000000 ldns-explorer-1.2/src/ldnsexplorer/DNS_APP.py
+-rw-r--r--   0 CD         (501) staff       (20)        0 2023-03-14 21:01:01.000000 ldns-explorer-1.2/src/ldnsexplorer/__init__.py
+-rw-r--r--   0 CD         (501) staff       (20)       40 2023-03-28 16:23:49.000000 ldns-explorer-1.2/src/ldnsexplorer/__main__.py
+-rw-r--r--   0 CD         (501) staff       (20)      303 2023-02-27 20:24:11.000000 ldns-explorer-1.2/src/ldnsexplorer/find_local_resolver.py
+-rw-r--r--   0 CD         (501) staff       (20)     1439 2023-03-14 04:37:46.000000 ldns-explorer-1.2/src/ldnsexplorer/measure_dns.py
+-rw-r--r--   0 CD         (501) staff       (20)      352 2023-03-14 04:52:05.000000 ldns-explorer-1.2/src/ldnsexplorer/measure_tcp.py
+-rw-r--r--   0 CD         (501) staff       (20)     1584 2023-03-29 02:06:34.000000 ldns-explorer-1.2/src/ldnsexplorer/tcp_client.py
```

### Comparing `ldns-explorer-1.1/PKG-INFO` & `ldns-explorer-1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldns-explorer
-Version: 1.1
+Version: 1.2
 Summary: A public DNS resolver explorer
 Author: cwru
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
@@ -28,15 +28,15 @@
 ```python
 python3 -m ldns-explorer
 ```
 
 
 ## Customized Test Case
 
-We support customized test domains and resolves beside our
+We support customized lists of test domains and resolvers beside our
 sample test cases.
 
 If you would like to add domains, please create a 
 txt file called `domains.txt` under the directory you invoke the 
 explorer.
 
 **The file structure is one domain per line.**
@@ -55,14 +55,20 @@
 `resolvers.txt`:
 ```text
 0.0.0.0
 1.1.1.1
 ```
 
 
-## Clarification
-
-The explorer will send the result of the measurement to us. You can disable
-this functionality by typing `NO` when the script prompt up the choice. 
-
+## Disclaimer
 
+The purpose of this project is twofold. On one hand, we hope it will help Internet
+users choose a DNS resolver that would improve their own Web browsing experience.  
+On the other hand, we would like to obtain general insights about performance 
+of DNS resolution infrastructures, which may lead to improvements of the Internet 
+for everybody. For the latter purpose, the DNS Explorer will send the result 
+of the measurement to us. No personally identifiable information is collected 
+or accessed by the application -- only the public IP address and the performance metrics. You can disable this 
+functionality by typing `NO` to the corresponding prompt during the application 
+execution; however, we hope you choose to participate in this crowdsources data collection 
+in recognition of our effort in creating this application.
```

### Comparing `ldns-explorer-1.1/src/ldns_explorer.egg-info/PKG-INFO` & `ldns-explorer-1.2/src/ldns_explorer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldns-explorer
-Version: 1.1
+Version: 1.2
 Summary: A public DNS resolver explorer
 Author: cwru
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
@@ -28,15 +28,15 @@
 ```python
 python3 -m ldns-explorer
 ```
 
 
 ## Customized Test Case
 
-We support customized test domains and resolves beside our
+We support customized lists of test domains and resolvers beside our
 sample test cases.
 
 If you would like to add domains, please create a 
 txt file called `domains.txt` under the directory you invoke the 
 explorer.
 
 **The file structure is one domain per line.**
@@ -55,14 +55,20 @@
 `resolvers.txt`:
 ```text
 0.0.0.0
 1.1.1.1
 ```
 
 
-## Clarification
-
-The explorer will send the result of the measurement to us. You can disable
-this functionality by typing `NO` when the script prompt up the choice. 
-
+## Disclaimer
 
+The purpose of this project is twofold. On one hand, we hope it will help Internet
+users choose a DNS resolver that would improve their own Web browsing experience.  
+On the other hand, we would like to obtain general insights about performance 
+of DNS resolution infrastructures, which may lead to improvements of the Internet 
+for everybody. For the latter purpose, the DNS Explorer will send the result 
+of the measurement to us. No personally identifiable information is collected 
+or accessed by the application -- only the public IP address and the performance metrics. You can disable this 
+functionality by typing `NO` to the corresponding prompt during the application 
+execution; however, we hope you choose to participate in this crowdsources data collection 
+in recognition of our effort in creating this application.
```

### Comparing `ldns-explorer-1.1/src/ldnsexplorer/DNS_APP.py` & `ldns-explorer-1.2/src/ldnsexplorer/DNS_APP.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
                 cur_tcp_delay = sorted(cur_tcp_delay)
                 cum_tcp_delay += cur_tcp_delay[int(len(cur_tcp_delay) / 2)]
 
             domains[domain][2].append(cum_tcp_delay / len(ip_addresses))
 
         progress += 1
-        print('Current progress:', progress, '/', total)
+        print('Current progress:', progress, '/', total, 'domains')
 
     # Output report file
     output_file = open("output.txt", "a+")
 
     # This will write the local resolver address to the output file
     local_resolver_address = find_local_resolver.find_local_resolver()
     output_file.write(local_resolver_address)
```

### Comparing `ldns-explorer-1.1/src/ldnsexplorer/measure_dns.py` & `ldns-explorer-1.2/src/ldnsexplorer/measure_dns.py`

 * *Files identical despite different names*

### Comparing `ldns-explorer-1.1/src/ldnsexplorer/tcp_client.py` & `ldns-explorer-1.2/src/ldnsexplorer/tcp_client.py`

 * *Files identical despite different names*

