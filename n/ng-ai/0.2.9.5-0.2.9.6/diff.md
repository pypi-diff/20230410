# Comparing `tmp/ng_ai-0.2.9.5-py3-none-any.whl.zip` & `tmp/ng_ai-0.2.9.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 20417 bytes, number of entries: 15
+Zip file size: 20603 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      616 b- defN 16-Jan-01 00:00 ng_ai/__init__.py
 -rw-r--r--  2.0 unx      966 b- defN 16-Jan-01 00:00 ng_ai/config.py
 -rw-r--r--  2.0 unx     3911 b- defN 16-Jan-01 00:00 ng_ai/engines.py
 -rw-r--r--  2.0 unx    13009 b- defN 16-Jan-01 00:00 ng_ai/nebula_algo.py
 -rw-r--r--  2.0 unx     4371 b- defN 16-Jan-01 00:00 ng_ai/nebula_data.py
 -rw-r--r--  2.0 unx      238 b- defN 16-Jan-01 00:00 ng_ai/nebula_gnn.py
 -rw-r--r--  2.0 unx     6925 b- defN 16-Jan-01 00:00 ng_ai/nebula_reader.py
 -rw-r--r--  2.0 unx    11319 b- defN 16-Jan-01 00:00 ng_ai/nebula_writer.py
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 ng_ai/ng_ai_api/__init__.py
 -rw-r--r--  2.0 unx      157 b- defN 16-Jan-01 00:00 ng_ai/ng_ai_api/__main__.py
 -rw-r--r--  2.0 unx     4914 b- defN 16-Jan-01 00:00 ng_ai/ng_ai_api/app.py
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 ng_ai-0.2.9.5.dist-info/WHEEL
-?rw-------  2.0 unx    12657 b- defN 16-Jan-01 00:00 ng_ai-0.2.9.5.dist-info/METADATA
--rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 ng_ai-0.2.9.5.dist-info/licenses/LICENSE
-?rw-------  2.0 unx     1154 b- defN 16-Jan-01 00:00 ng_ai-0.2.9.5.dist-info/RECORD
-15 files, 71681 bytes uncompressed, 18539 bytes compressed:  74.1%
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 ng_ai-0.2.9.6.dist-info/WHEEL
+?rw-------  2.0 unx    13437 b- defN 16-Jan-01 00:00 ng_ai-0.2.9.6.dist-info/METADATA
+-rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 ng_ai-0.2.9.6.dist-info/licenses/LICENSE
+?rw-------  2.0 unx     1154 b- defN 16-Jan-01 00:00 ng_ai-0.2.9.6.dist-info/RECORD
+15 files, 72461 bytes uncompressed, 18725 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: ng_ai/ng_ai_api/__main__.py
 Comment: 
 
 Filename: ng_ai/ng_ai_api/app.py
 Comment: 
 
-Filename: ng_ai-0.2.9.5.dist-info/WHEEL
+Filename: ng_ai-0.2.9.6.dist-info/WHEEL
 Comment: 
 
-Filename: ng_ai-0.2.9.5.dist-info/METADATA
+Filename: ng_ai-0.2.9.6.dist-info/METADATA
 Comment: 
 
-Filename: ng_ai-0.2.9.5.dist-info/licenses/LICENSE
+Filename: ng_ai-0.2.9.6.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: ng_ai-0.2.9.5.dist-info/RECORD
+Filename: ng_ai-0.2.9.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ng_ai-0.2.9.5.dist-info/METADATA` & `ng_ai-0.2.9.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: ng_ai
-Version: 0.2.9.5
+Version: 0.2.9.6
 Summary: NebulaGraph AI Suite
 License: Apache-2.0
 Author-email: Wey Gu <weyl.gu@gmail.com>
 Requires-Python: >=3.7,<3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: flask>=2.0.3
 Requires-Dist: nebula3-python
 Requires-Dist: networkx>=2.5.1
 Provides-Extra: all
 Requires-Dist: ng_ai[networkx,spark]; extra == "all"
 Provides-Extra: dev
 Requires-Dist: ng_ai[all,lint,test]; extra == "dev"
@@ -20,14 +23,18 @@
 Requires-Dist: networkx>=2.5.1; extra == "networkx"
 Provides-Extra: spark
 Requires-Dist: pyspark>=3.2.3; extra == "spark"
 Provides-Extra: test
 Requires-Dist: pytest>=7.2.2; extra == "test"
 Requires-Dist: chispa; extra == "test"
 Requires-Dist: requests; extra == "test"
+Project-URL: Changelog, https://github.com/wey-gu/nebulagraph-ai/releases
+Project-URL: Documentation, https://github.com/wey-gu/nebulagraph-ai#documentation
+Project-URL: Homepage, https://github.com/wey-gu/nebulagraph-ai
+Project-URL: Repository, https://github.com/wey-gu/nebulagraph-ai
 Description-Content-Type: text/markdown
 
 <img alt="NebulaGraph AI Suite(ng_ai)" src="https://user-images.githubusercontent.com/1651790/226242809-fe488ff2-bb4a-4e7d-b23a-70865a7b3228.png">
 
 <p align="center">
     <em>NebulaGraph AI Suite with 4 line code to run Graph Algo on NebulaGraph</em>
 </p>
@@ -37,22 +44,28 @@
     <img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" alt="License">
 </a>
 
 <a href="https://badge.fury.io/py/ng_ai" target="_blank">
     <img src="https://badge.fury.io/py/ng_ai.svg" alt="PyPI version">
 </a>
 
-<a href="https://www.python.org/downloads/release/python-360/" target="_blank">
+<!-- <a href="https://www.python.org/downloads/release/python-360/" target="_blank">
     <img src="https://img.shields.io/badge/python-3.6%2B-blue.svg" alt="Python">
-</a>
+</a> -->
 
 <a href="https://pdm.fming.dev" target="_blank">
     <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
 
+<a href="https://github.com/wey-gu/nebulagraph-ai/actions/workflows/ci.yml">
+  <img src="https://github.com/wey-gu/nebulagraph-ai/actions/workflows/ci.yml/badge.svg" alt="Tests">
+</a>
+
+<img src="https://img.shields.io/badge/Python-3.9-blue.svg" alt="Python 3.9">
+
 </p>
 
 ---
 
 **Documentation**: <a href="https://github.com/wey-gu/nebulagraph-ai#documentation" target="_blank">https://github.com/wey-gu/nebulagraph-ai#documentation</a>
 
 **Source Code**: <a href="https://github.com/wey-gu/nebulagraph-ai" target="_blank">https://github.com/wey-gu/nebulagraph-ai</a>
@@ -220,13 +233,13 @@
 - [NebulaGraph 3.4+](https://github.com/vesoft-inc/nebula)
 - [NebulaGraph Python Client 3.4+](https://github.com/vesoft-inc/nebula-python)
 - [NetworkX](https://networkx.org/)
 
 
 ## Contributing
 
-See HACKING.md for details.
+See [HACKING.md](https://github.com/wey-gu/nebulagraph-ai/blob/main/HACKING.md) for details.
 
 ## License
 
 This project is licensed under the terms of the Apache License 2.0.
```

### html2text {}

```diff
@@ -1,22 +1,28 @@
-Metadata-Version: 2.1 Name: ng_ai Version: 0.2.9.5 Summary: NebulaGraph AI
+Metadata-Version: 2.1 Name: ng_ai Version: 0.2.9.6 Summary: NebulaGraph AI
 Suite License: Apache-2.0 Author-email: Wey Gu
-gu@gmail.com> Requires-Python: >=3.7,<3.10 Requires-Dist: flask>=2.0.3
-Requires-Dist: nebula3-python Requires-Dist: networkx>=2.5.1 Provides-Extra:
-all Requires-Dist: ng_ai[networkx,spark]; extra == "all" Provides-Extra: dev
+gu@gmail.com> Requires-Python: >=3.7,<3.10 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic
+:: Software Development :: Build Tools Requires-Dist: flask>=2.0.3 Requires-
+Dist: nebula3-python Requires-Dist: networkx>=2.5.1 Provides-Extra: all
+Requires-Dist: ng_ai[networkx,spark]; extra == "all" Provides-Extra: dev
 Requires-Dist: ng_ai[all,lint,test]; extra == "dev" Provides-Extra: lint
 Requires-Dist: flake8>=4.0.1; extra == "lint" Requires-Dist: black
 [jupyter]>=23.1.0; extra == "lint" Requires-Dist: isort>=5.11.5; extra ==
 "lint" Provides-Extra: networkx Requires-Dist: networkx>=2.5.1; extra ==
 "networkx" Provides-Extra: spark Requires-Dist: pyspark>=3.2.3; extra ==
 "spark" Provides-Extra: test Requires-Dist: pytest>=7.2.2; extra == "test"
 Requires-Dist: chispa; extra == "test" Requires-Dist: requests; extra == "test"
+Project-URL: Changelog, https://github.com/wey-gu/nebulagraph-ai/releases
+Project-URL: Documentation, https://github.com/wey-gu/nebulagraph-
+ai#documentation Project-URL: Homepage, https://github.com/wey-gu/nebulagraph-
+ai Project-URL: Repository, https://github.com/wey-gu/nebulagraph-ai
 Description-Content-Type: text/markdown [NebulaGraph AI Suite(ng_ai)]
     NebulaGraph AI Suite with 4 line code to run Graph Algo on NebulaGraph
-                [License] [PyPI_version] [Python] [pdm-managed]
+         [License] [PyPI_version]  [pdm-managed] [Tests] [Python 3.9]
 --- **Documentation**: https://github.com/wey-gu/nebulagraph-ai#documentation
 **Source Code**: https://github.com/wey-gu/nebulagraph-ai --- NebulaGraph AI
 Suite for Python (ng_ai) is a powerful Python library that offers APIs for data
 scientists to effectively read, write, analyze, and compute data in
 NebulaGraph. With the support of single-machine engine(NetworkX), or
 distributed computing environment using Spark we could perform Graph Analysis
 and Algorithms on top of NebulaGraph in less than 10 lines of code, in unified
@@ -111,9 +117,10 @@
 ``` ### Spark Engine Prerequisites - Spark 2.4, 3.0(not yet tested) -
 [NebulaGraph 3.4+](https://github.com/vesoft-inc/nebula) - [NebulaGraph Spark
 Connector 3.4+](https://repo1.maven.org/maven2/com/vesoft/nebula-spark-
 connector/) - [NebulaGraph Algorithm 3.1+](https://repo1.maven.org/maven2/com/
 vesoft/nebula-algorithm/) ### NebulaGraph Engine Prerequisites - [NebulaGraph
 3.4+](https://github.com/vesoft-inc/nebula) - [NebulaGraph Python Client 3.4+]
 (https://github.com/vesoft-inc/nebula-python) - [NetworkX](https://
-networkx.org/) ## Contributing See HACKING.md for details. ## License This
-project is licensed under the terms of the Apache License 2.0.
+networkx.org/) ## Contributing See [HACKING.md](https://github.com/wey-gu/
+nebulagraph-ai/blob/main/HACKING.md) for details. ## License This project is
+licensed under the terms of the Apache License 2.0.
```

## Comparing `ng_ai-0.2.9.5.dist-info/licenses/LICENSE` & `ng_ai-0.2.9.6.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `ng_ai-0.2.9.5.dist-info/RECORD` & `ng_ai-0.2.9.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 ng_ai/nebula_data.py,sha256=OyK_DravgaVjA_p3bPp87vepfJXb1NqMWlhawt1bojU,4371
 ng_ai/nebula_gnn.py,sha256=EH1wvNcyqg3KjM2vZI0gBXnSRzxK3CQZt9W4yvTwDCY,238
 ng_ai/nebula_reader.py,sha256=XRkQdZ6IB6MqopYR2JqSh74DpH-W1uS93lCaI4Yx6yI,6925
 ng_ai/nebula_writer.py,sha256=4dybqpdPq_7yf4wW6IAmk7lx5hcCv5ih2gadFI2uh74,11319
 ng_ai/ng_ai_api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ng_ai/ng_ai_api/__main__.py,sha256=9_63HbEI1A507UOnWohgms9jOg3HHVLxLFttNtxMRJg,157
 ng_ai/ng_ai_api/app.py,sha256=x2qZwwyR2d6ehuKHKoycGb-k84-fHfzVLDEY2BLFTuM,4914
-ng_ai-0.2.9.5.dist-info/WHEEL,sha256=JtIceljpZF_3FlF7JEESqvYUELdenaIGNR7wSL2mRl0,87
-ng_ai-0.2.9.5.dist-info/METADATA,sha256=OGIN2Z8FbvWOgud8H4ZShZuqZ1lZBayXUMeuMQcRrmc,12657
-ng_ai-0.2.9.5.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-ng_ai-0.2.9.5.dist-info/RECORD,,
+ng_ai-0.2.9.6.dist-info/WHEEL,sha256=JtIceljpZF_3FlF7JEESqvYUELdenaIGNR7wSL2mRl0,87
+ng_ai-0.2.9.6.dist-info/METADATA,sha256=6yXITlJdGkGChuoqBXg4qt5Zbcz6otx8V1prePRjVYA,13437
+ng_ai-0.2.9.6.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+ng_ai-0.2.9.6.dist-info/RECORD,,
```

