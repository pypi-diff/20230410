# Comparing `tmp/napari-sam-0.1.9.tar.gz` & `tmp/napari-sam-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.1.9.tar", last modified: Thu Apr  6 13:26:58 2023, max compression
+gzip compressed data, was "napari-sam-0.2.0.tar", last modified: Mon Apr 10 09:35:35 2023, max compression
```

## Comparing `napari-sam-0.1.9.tar` & `napari-sam-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:26:58.601552 napari-sam-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-06 13:26:36.000000 napari-sam-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-06 13:26:36.000000 napari-sam-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-06 13:26:58.601552 napari-sam-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-06 13:26:36.000000 napari-sam-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-06 13:26:36.000000 napari-sam-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-06 13:26:58.601552 napari-sam-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:26:58.597552 napari-sam-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:26:58.601552 napari-sam-0.1.9/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-06 13:26:36.000000 napari-sam-0.1.9/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-06 13:26:36.000000 napari-sam-0.1.9/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-06 13:26:36.000000 napari-sam-0.1.9/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-06 13:26:36.000000 napari-sam-0.1.9/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:26:58.601552 napari-sam-0.1.9/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-06 13:26:58.000000 napari-sam-0.1.9/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-06 13:26:58.000000 napari-sam-0.1.9/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:26:58.000000 napari-sam-0.1.9/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-06 13:26:58.000000 napari-sam-0.1.9/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-06 13:26:58.000000 napari-sam-0.1.9/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 13:26:58.000000 napari-sam-0.1.9/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:35:35.359510 napari-sam-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 09:35:16.000000 napari-sam-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-10 09:35:16.000000 napari-sam-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-10 09:35:35.359510 napari-sam-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-10 09:35:16.000000 napari-sam-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-10 09:35:16.000000 napari-sam-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-10 09:35:35.359510 napari-sam-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:35:35.355510 napari-sam-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:35:35.359510 napari-sam-0.2.0/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 09:35:16.000000 napari-sam-0.2.0/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-04-10 09:35:16.000000 napari-sam-0.2.0/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-10 09:35:16.000000 napari-sam-0.2.0/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-10 09:35:16.000000 napari-sam-0.2.0/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:35:35.359510 napari-sam-0.2.0/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-10 09:35:35.000000 napari-sam-0.2.0/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-10 09:35:35.000000 napari-sam-0.2.0/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:35:35.000000 napari-sam-0.2.0/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 09:35:35.000000 napari-sam-0.2.0/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 09:35:35.000000 napari-sam-0.2.0/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 09:35:35.000000 napari-sam-0.2.0/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.1.9/LICENSE` & `napari-sam-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.1.9/PKG-INFO` & `napari-sam-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,241 +1,215 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6e61 7061  : 2.1.Name: napa
-00000020: 7269 2d73 616d 0a56 6572 7369 6f6e 3a20  ri-sam.Version: 
-00000030: 302e 312e 390a 5375 6d6d 6172 793a 2053  0.1.9.Summary: S
-00000040: 6567 6d65 6e74 2061 6e79 7468 696e 6720  egment anything 
-00000050: 7769 7468 204d 6574 6120 4149 2773 206e  with Meta AI's n
-00000060: 6577 2053 414d 206d 6f64 656c 210a 486f  ew SAM model!.Ho
-00000070: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-00000080: 2f67 6974 6875 622e 636f 6d2f 4d49 432d  /github.com/MIC-
-00000090: 444b 465a 2f6e 6170 6172 692d 7361 6d0a  DKFZ/napari-sam.
-000000a0: 4175 7468 6f72 3a20 4b61 726f 6c20 476f  Author: Karol Go
-000000b0: 746b 6f77 736b 690a 4175 7468 6f72 2d65  tkowski.Author-e
-000000c0: 6d61 696c 3a20 6b61 726f 6c2e 676f 746b  mail: karol.gotk
-000000d0: 6f77 736b 6940 646b 667a 2e64 650a 4c69  owski@dkfz.de.Li
-000000e0: 6365 6e73 653a 2041 7061 6368 652d 322e  cense: Apache-2.
-000000f0: 300a 5072 6f6a 6563 742d 5552 4c3a 2042  0.Project-URL: B
-00000100: 7567 2054 7261 636b 6572 2c20 6874 7470  ug Tracker, http
-00000110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
-00000120: 4943 2d44 4b46 5a2f 6e61 7061 7269 2d73  IC-DKFZ/napari-s
-00000130: 616d 2f69 7373 7565 730a 5072 6f6a 6563  am/issues.Projec
-00000140: 742d 5552 4c3a 2044 6f63 756d 656e 7461  t-URL: Documenta
-00000150: 7469 6f6e 2c20 6874 7470 733a 2f2f 6769  tion, https://gi
-00000160: 7468 7562 2e63 6f6d 2f4d 4943 2d44 4b46  thub.com/MIC-DKF
-00000170: 5a2f 6e61 7061 7269 2d73 616d 2352 4541  Z/napari-sam#REA
-00000180: 444d 452e 6d64 0a50 726f 6a65 6374 2d55  DME.md.Project-U
-00000190: 524c 3a20 536f 7572 6365 2043 6f64 652c  RL: Source Code,
-000001a0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000001b0: 636f 6d2f 4d49 432d 444b 465a 2f6e 6170  com/MIC-DKFZ/nap
-000001c0: 6172 692d 7361 6d0a 5072 6f6a 6563 742d  ari-sam.Project-
-000001d0: 5552 4c3a 2055 7365 7220 5375 7070 6f72  URL: User Suppor
-000001e0: 742c 2068 7474 7073 3a2f 2f67 6974 6875  t, https://githu
-000001f0: 622e 636f 6d2f 4d49 432d 444b 465a 2f6e  b.com/MIC-DKFZ/n
-00000200: 6170 6172 692d 7361 6d2f 6973 7375 6573  apari-sam/issues
-00000210: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-00000220: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000230: 3a3a 2032 202d 2050 7265 2d41 6c70 6861  :: 2 - Pre-Alpha
-00000240: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
-00000250: 6d65 776f 726b 203a 3a20 6e61 7061 7269  mework :: napari
-00000260: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
-00000270: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000280: 3a20 4465 7665 6c6f 7065 7273 0a43 6c61  : Developers.Cla
-00000290: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-000002a0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000002b0: 203a 3a20 4170 6163 6865 2053 6f66 7477   :: Apache Softw
-000002c0: 6172 6520 4c69 6365 6e73 650a 436c 6173  are License.Clas
-000002d0: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-000002e0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-000002f0: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
-00000300: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000310: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000320: 7974 686f 6e0a 436c 6173 7369 6669 6572  ython.Classifier
-00000330: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000340: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000350: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
-00000360: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000370: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000380: 203a 3a20 3320 3a3a 204f 6e6c 790a 436c   :: 3 :: Only.Cl
-00000390: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000003a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000003b0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-000003c0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-000003d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000003e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000003f0: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
-00000400: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000410: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000420: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
-00000430: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
-00000440: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
-00000450: 203a 3a20 496d 6167 6520 5072 6f63 6573   :: Image Proces
-00000460: 7369 6e67 0a52 6571 7569 7265 732d 5079  sing.Requires-Py
-00000470: 7468 6f6e 3a20 3e3d 332e 380a 4465 7363  thon: >=3.8.Desc
-00000480: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00000490: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-000004a0: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
-000004b0: 7261 3a20 7465 7374 696e 670a 4c69 6365  ra: testing.Lice
-000004c0: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-000004d0: 450a 0a23 206e 6170 6172 692d 7361 6d0a  E..# napari-sam.
-000004e0: 0a5b 215b 4c69 6365 6e73 6520 4170 6163  .[![License Apac
-000004f0: 6865 2053 6f66 7477 6172 6520 4c69 6365  he Software Lice
-00000500: 6e73 6520 322e 305d 2868 7474 7073 3a2f  nse 2.0](https:/
-00000510: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000520: 7079 7069 2f6c 2f6e 6170 6172 692d 7361  pypi/l/napari-sa
-00000530: 6d2e 7376 673f 636f 6c6f 723d 6772 6565  m.svg?color=gree
-00000540: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
-00000550: 7562 2e63 6f6d 2f4d 4943 2d44 4b46 5a2f  ub.com/MIC-DKFZ/
-00000560: 6e61 7061 7269 2d73 616d 2f72 6177 2f6d  napari-sam/raw/m
-00000570: 6169 6e2f 4c49 4345 4e53 4529 0a5b 215b  ain/LICENSE).[![
-00000580: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
-00000590: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000005a0: 692f 762f 6e61 7061 7269 2d73 616d 2e73  i/v/napari-sam.s
-000005b0: 7667 3f63 6f6c 6f72 3d67 7265 656e 295d  vg?color=green)]
-000005c0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-000005d0: 672f 7072 6f6a 6563 742f 6e61 7061 7269  g/project/napari
-000005e0: 2d73 616d 290a 5b21 5b50 7974 686f 6e20  -sam).[![Python 
-000005f0: 5665 7273 696f 6e5d 2868 7474 7073 3a2f  Version](https:/
-00000600: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000610: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
-00000620: 6e61 7061 7269 2d73 616d 2e73 7667 3f63  napari-sam.svg?c
-00000630: 6f6c 6f72 3d67 7265 656e 295d 2868 7474  olor=green)](htt
-00000640: 7073 3a2f 2f70 7974 686f 6e2e 6f72 6729  ps://python.org)
-00000650: 0a5b 215b 7465 7374 735d 2868 7474 7073  .[![tests](https
-00000660: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d49  ://github.com/MI
-00000670: 432d 444b 465a 2f6e 6170 6172 692d 7361  C-DKFZ/napari-sa
-00000680: 6d2f 776f 726b 666c 6f77 732f 7465 7374  m/workflows/test
-00000690: 732f 6261 6467 652e 7376 6729 5d28 6874  s/badge.svg)](ht
-000006a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000006b0: 2f4d 4943 2d44 4b46 5a2f 6e61 7061 7269  /MIC-DKFZ/napari
-000006c0: 2d73 616d 2f61 6374 696f 6e73 290a 5b21  -sam/actions).[!
-000006d0: 5b63 6f64 6563 6f76 5d28 6874 7470 733a  [codecov](https:
-000006e0: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
-000006f0: 4d49 432d 444b 465a 2f6e 6170 6172 692d  MIC-DKFZ/napari-
-00000700: 7361 6d2f 6272 616e 6368 2f6d 6169 6e2f  sam/branch/main/
-00000710: 6772 6170 682f 6261 6467 652e 7376 6729  graph/badge.svg)
-00000720: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
-00000730: 762e 696f 2f67 682f 4d49 432d 444b 465a  v.io/gh/MIC-DKFZ
-00000740: 2f6e 6170 6172 692d 7361 6d29 0a5b 215b  /napari-sam).[![
-00000750: 6e61 7061 7269 2068 7562 5d28 6874 7470  napari hub](http
-00000760: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000770: 696f 2f65 6e64 706f 696e 743f 7572 6c3d  io/endpoint?url=
-00000780: 6874 7470 733a 2f2f 6170 692e 6e61 7061  https://api.napa
-00000790: 7269 2d68 7562 2e6f 7267 2f73 6869 656c  ri-hub.org/shiel
-000007a0: 6473 2f6e 6170 6172 692d 7361 6d29 5d28  ds/napari-sam)](
-000007b0: 6874 7470 733a 2f2f 6e61 7061 7269 2d68  https://napari-h
-000007c0: 7562 2e6f 7267 2f70 6c75 6769 6e73 2f6e  ub.org/plugins/n
-000007d0: 6170 6172 692d 7361 6d29 0a0a 5365 676d  apari-sam)..Segm
-000007e0: 656e 7420 616e 7974 6869 6e67 2077 6974  ent anything wit
-000007f0: 6820 4d65 7461 2041 4927 7320 6e65 7720  h Meta AI's new 
-00000800: 5341 4d20 6d6f 6465 6c21 0a0a 2d2d 2d2d  SAM model!..----
-00000810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00000830: 5468 6973 205b 6e61 7061 7269 5d20 706c  This [napari] pl
-00000840: 7567 696e 2077 6173 2067 656e 6572 6174  ugin was generat
-00000850: 6564 2077 6974 6820 5b43 6f6f 6b69 6563  ed with [Cookiec
-00000860: 7574 7465 725d 2075 7369 6e67 205b 406e  utter] using [@n
-00000870: 6170 6172 695d 2773 205b 636f 6f6b 6965  apari]'s [cookie
-00000880: 6375 7474 6572 2d6e 6170 6172 692d 706c  cutter-napari-pl
-00000890: 7567 696e 5d20 7465 6d70 6c61 7465 2e0a  ugin] template..
-000008a0: 0a3c 212d 2d0a 446f 6e27 7420 6d69 7373  .<!--.Don't miss
-000008b0: 2074 6865 2066 756c 6c20 6765 7474 696e   the full gettin
-000008c0: 6720 7374 6172 7465 6420 6775 6964 6520  g started guide 
-000008d0: 746f 2073 6574 2075 7020 796f 7572 206e  to set up your n
-000008e0: 6577 2070 6163 6b61 6765 3a0a 6874 7470  ew package:.http
-000008f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
-00000900: 6170 6172 692f 636f 6f6b 6965 6375 7474  apari/cookiecutt
-00000910: 6572 2d6e 6170 6172 692d 706c 7567 696e  er-napari-plugin
-00000920: 2367 6574 7469 6e67 2d73 7461 7274 6564  #getting-started
-00000930: 0a0a 616e 6420 7265 7669 6577 2074 6865  ..and review the
-00000940: 206e 6170 6172 6920 646f 6373 2066 6f72   napari docs for
-00000950: 2070 6c75 6769 6e20 6465 7665 6c6f 7065   plugin develope
-00000960: 7273 3a0a 6874 7470 733a 2f2f 6e61 7061  rs:.https://napa
-00000970: 7269 2e6f 7267 2f73 7461 626c 652f 706c  ri.org/stable/pl
-00000980: 7567 696e 732f 696e 6465 782e 6874 6d6c  ugins/index.html
-00000990: 0a2d 2d3e 0a0a 2323 2049 6e73 7461 6c6c  .-->..## Install
-000009a0: 6174 696f 6e0a 0a59 6f75 2063 616e 2069  ation..You can i
-000009b0: 6e73 7461 6c6c 2060 6e61 7061 7269 2d73  nstall `napari-s
-000009c0: 616d 6020 7669 6120 5b70 6970 5d3a 0a0a  am` via [pip]:..
-000009d0: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
-000009e0: 6e61 7061 7269 2d73 616d 0a0a 0a0a 546f  napari-sam....To
-000009f0: 2069 6e73 7461 6c6c 206c 6174 6573 7420   install latest 
-00000a00: 6465 7665 6c6f 706d 656e 7420 7665 7273  development vers
-00000a10: 696f 6e20 3a0a 0a20 2020 2070 6970 2069  ion :..    pip i
-00000a20: 6e73 7461 6c6c 2067 6974 2b68 7474 7073  nstall git+https
-00000a30: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d49  ://github.com/MI
-00000a40: 432d 444b 465a 2f6e 6170 6172 692d 7361  C-DKFZ/napari-sa
-00000a50: 6d2e 6769 740a 0a0a 2323 2043 6f6e 7472  m.git...## Contr
-00000a60: 6962 7574 696e 670a 0a43 6f6e 7472 6962  ibuting..Contrib
-00000a70: 7574 696f 6e73 2061 7265 2076 6572 7920  utions are very 
-00000a80: 7765 6c63 6f6d 652e 2054 6573 7473 2063  welcome. Tests c
-00000a90: 616e 2062 6520 7275 6e20 7769 7468 205b  an be run with [
-00000aa0: 746f 785d 2c20 706c 6561 7365 2065 6e73  tox], please ens
-00000ab0: 7572 650a 7468 6520 636f 7665 7261 6765  ure.the coverage
-00000ac0: 2061 7420 6c65 6173 7420 7374 6179 7320   at least stays 
-00000ad0: 7468 6520 7361 6d65 2062 6566 6f72 6520  the same before 
-00000ae0: 796f 7520 7375 626d 6974 2061 2070 756c  you submit a pul
-00000af0: 6c20 7265 7175 6573 742e 0a0a 2323 204c  l request...## L
-00000b00: 6963 656e 7365 0a0a 4469 7374 7269 6275  icense..Distribu
-00000b10: 7465 6420 756e 6465 7220 7468 6520 7465  ted under the te
-00000b20: 726d 7320 6f66 2074 6865 205b 4170 6163  rms of the [Apac
-00000b30: 6865 2053 6f66 7477 6172 6520 4c69 6365  he Software Lice
-00000b40: 6e73 6520 322e 305d 206c 6963 656e 7365  nse 2.0] license
-00000b50: 2c0a 226e 6170 6172 692d 7361 6d22 2069  ,."napari-sam" i
-00000b60: 7320 6672 6565 2061 6e64 206f 7065 6e20  s free and open 
-00000b70: 736f 7572 6365 2073 6f66 7477 6172 650a  source software.
-00000b80: 0a23 2320 4973 7375 6573 0a0a 4966 2079  .## Issues..If y
-00000b90: 6f75 2065 6e63 6f75 6e74 6572 2061 6e79  ou encounter any
-00000ba0: 2070 726f 626c 656d 732c 2070 6c65 6173   problems, pleas
-00000bb0: 6520 5b66 696c 6520 616e 2069 7373 7565  e [file an issue
-00000bc0: 5d20 616c 6f6e 6720 7769 7468 2061 2064  ] along with a d
-00000bd0: 6574 6169 6c65 6420 6465 7363 7269 7074  etailed descript
-00000be0: 696f 6e2e 0a0a 5b6e 6170 6172 695d 3a20  ion...[napari]: 
-00000bf0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c00: 6f6d 2f6e 6170 6172 692f 6e61 7061 7269  om/napari/napari
-00000c10: 0a5b 436f 6f6b 6965 6375 7474 6572 5d3a  .[Cookiecutter]:
-00000c20: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000c30: 636f 6d2f 6175 6472 6579 722f 636f 6f6b  com/audreyr/cook
-00000c40: 6965 6375 7474 6572 0a5b 406e 6170 6172  iecutter.[@napar
-00000c50: 695d 3a20 6874 7470 733a 2f2f 6769 7468  i]: https://gith
-00000c60: 7562 2e63 6f6d 2f6e 6170 6172 690a 5b4d  ub.com/napari.[M
-00000c70: 4954 5d3a 2068 7474 703a 2f2f 6f70 656e  IT]: http://open
-00000c80: 736f 7572 6365 2e6f 7267 2f6c 6963 656e  source.org/licen
-00000c90: 7365 732f 4d49 540a 5b42 5344 2d33 5d3a  ses/MIT.[BSD-3]:
-00000ca0: 2068 7474 703a 2f2f 6f70 656e 736f 7572   http://opensour
-00000cb0: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
-00000cc0: 4253 442d 332d 436c 6175 7365 0a5b 474e  BSD-3-Clause.[GN
-00000cd0: 5520 4750 4c20 7633 2e30 5d3a 2068 7474  U GPL v3.0]: htt
-00000ce0: 703a 2f2f 7777 772e 676e 752e 6f72 672f  p://www.gnu.org/
-00000cf0: 6c69 6365 6e73 6573 2f67 706c 2d33 2e30  licenses/gpl-3.0
-00000d00: 2e74 7874 0a5b 474e 5520 4c47 504c 2076  .txt.[GNU LGPL v
-00000d10: 332e 305d 3a20 6874 7470 3a2f 2f77 7777  3.0]: http://www
-00000d20: 2e67 6e75 2e6f 7267 2f6c 6963 656e 7365  .gnu.org/license
-00000d30: 732f 6c67 706c 2d33 2e30 2e74 7874 0a5b  s/lgpl-3.0.txt.[
-00000d40: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
-00000d50: 4c69 6365 6e73 6520 322e 305d 3a20 6874  License 2.0]: ht
-00000d60: 7470 3a2f 2f77 7777 2e61 7061 6368 652e  tp://www.apache.
-00000d70: 6f72 672f 6c69 6365 6e73 6573 2f4c 4943  org/licenses/LIC
-00000d80: 454e 5345 2d32 2e30 0a5b 4d6f 7a69 6c6c  ENSE-2.0.[Mozill
-00000d90: 6120 5075 626c 6963 204c 6963 656e 7365  a Public License
-00000da0: 2032 2e30 5d3a 2068 7474 7073 3a2f 2f77   2.0]: https://w
-00000db0: 7777 2e6d 6f7a 696c 6c61 2e6f 7267 2f6d  ww.mozilla.org/m
-00000dc0: 6564 6961 2f4d 504c 2f32 2e30 2f69 6e64  edia/MPL/2.0/ind
-00000dd0: 6578 2e74 7874 0a5b 636f 6f6b 6965 6375  ex.txt.[cookiecu
-00000de0: 7474 6572 2d6e 6170 6172 692d 706c 7567  tter-napari-plug
-00000df0: 696e 5d3a 2068 7474 7073 3a2f 2f67 6974  in]: https://git
-00000e00: 6875 622e 636f 6d2f 6e61 7061 7269 2f63  hub.com/napari/c
-00000e10: 6f6f 6b69 6563 7574 7465 722d 6e61 7061  ookiecutter-napa
-00000e20: 7269 2d70 6c75 6769 6e0a 0a5b 6669 6c65  ri-plugin..[file
-00000e30: 2061 6e20 6973 7375 655d 3a20 6874 7470   an issue]: http
-00000e40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
-00000e50: 4943 2d44 4b46 5a2f 6e61 7061 7269 2d73  IC-DKFZ/napari-s
-00000e60: 616d 2f69 7373 7565 730a 0a5b 6e61 7061  am/issues..[napa
-00000e70: 7269 5d3a 2068 7474 7073 3a2f 2f67 6974  ri]: https://git
-00000e80: 6875 622e 636f 6d2f 6e61 7061 7269 2f6e  hub.com/napari/n
-00000e90: 6170 6172 690a 5b74 6f78 5d3a 2068 7474  apari.[tox]: htt
-00000ea0: 7073 3a2f 2f74 6f78 2e72 6561 6474 6865  ps://tox.readthe
-00000eb0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00000ec0: 742f 0a5b 7069 705d 3a20 6874 7470 733a  t/.[pip]: https:
-00000ed0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000ee0: 6374 2f70 6970 2f0a 5b50 7950 495d 3a20  ct/pip/.[PyPI]: 
-00000ef0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000f00: 2f0a                                     /.
+00000000: 2320 5365 676d 656e 7420 416e 7974 6869  # Segment Anythi
+00000010: 6e67 204d 6f64 656c 2028 5341 4d29 2069  ng Model (SAM) i
+00000020: 6e20 4e61 7061 7269 0a0a 5b21 5b4c 6963  n Napari..[![Lic
+00000030: 656e 7365 2041 7061 6368 6520 536f 6674  ense Apache Soft
+00000040: 7761 7265 204c 6963 656e 7365 2032 2e30  ware License 2.0
+00000050: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000060: 6965 6c64 732e 696f 2f70 7970 692f 6c2f  ields.io/pypi/l/
+00000070: 6e61 7061 7269 2d73 616d 2e73 7667 3f63  napari-sam.svg?c
+00000080: 6f6c 6f72 3d67 7265 656e 295d 2868 7474  olor=green)](htt
+00000090: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000000a0: 4d49 432d 444b 465a 2f6e 6170 6172 692d  MIC-DKFZ/napari-
+000000b0: 7361 6d2f 7261 772f 6d61 696e 2f4c 4943  sam/raw/main/LIC
+000000c0: 454e 5345 290a 5b21 5b50 7950 495d 2868  ENSE).[![PyPI](h
+000000d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000000e0: 6473 2e69 6f2f 7079 7069 2f76 2f6e 6170  ds.io/pypi/v/nap
+000000f0: 6172 692d 7361 6d2e 7376 673f 636f 6c6f  ari-sam.svg?colo
+00000100: 723d 6772 6565 6e29 5d28 6874 7470 733a  r=green)](https:
+00000110: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000120: 6374 2f6e 6170 6172 692d 7361 6d29 0a5b  ct/napari-sam).[
+00000130: 215b 5079 7468 6f6e 2056 6572 7369 6f6e  ![Python Version
+00000140: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000150: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
+00000160: 7665 7273 696f 6e73 2f6e 6170 6172 692d  versions/napari-
+00000170: 7361 6d2e 7376 673f 636f 6c6f 723d 6772  sam.svg?color=gr
+00000180: 6565 6e29 5d28 6874 7470 733a 2f2f 7079  een)](https://py
+00000190: 7468 6f6e 2e6f 7267 290a 5b21 5b74 6573  thon.org).[![tes
+000001a0: 7473 5d28 6874 7470 733a 2f2f 6769 7468  ts](https://gith
+000001b0: 7562 2e63 6f6d 2f4d 4943 2d44 4b46 5a2f  ub.com/MIC-DKFZ/
+000001c0: 6e61 7061 7269 2d73 616d 2f77 6f72 6b66  napari-sam/workf
+000001d0: 6c6f 7773 2f74 6573 7473 2f62 6164 6765  lows/tests/badge
+000001e0: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+000001f0: 6974 6875 622e 636f 6d2f 4d49 432d 444b  ithub.com/MIC-DK
+00000200: 465a 2f6e 6170 6172 692d 7361 6d2f 6163  FZ/napari-sam/ac
+00000210: 7469 6f6e 7329 0a5b 215b 636f 6465 636f  tions).[![codeco
+00000220: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
+00000230: 6f76 2e69 6f2f 6768 2f4d 4943 2d44 4b46  ov.io/gh/MIC-DKF
+00000240: 5a2f 6e61 7061 7269 2d73 616d 2f62 7261  Z/napari-sam/bra
+00000250: 6e63 682f 6d61 696e 2f67 7261 7068 2f62  nch/main/graph/b
+00000260: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00000270: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00000280: 2f4d 4943 2d44 4b46 5a2f 6e61 7061 7269  /MIC-DKFZ/napari
+00000290: 2d73 616d 290a 5b21 5b6e 6170 6172 6920  -sam).[![napari 
+000002a0: 6875 625d 2868 7474 7073 3a2f 2f69 6d67  hub](https://img
+000002b0: 2e73 6869 656c 6473 2e69 6f2f 656e 6470  .shields.io/endp
+000002c0: 6f69 6e74 3f75 726c 3d68 7474 7073 3a2f  oint?url=https:/
+000002d0: 2f61 7069 2e6e 6170 6172 692d 6875 622e  /api.napari-hub.
+000002e0: 6f72 672f 7368 6965 6c64 732f 6e61 7061  org/shields/napa
+000002f0: 7269 2d73 616d 295d 2868 7474 7073 3a2f  ri-sam)](https:/
+00000300: 2f6e 6170 6172 692d 6875 622e 6f72 672f  /napari-hub.org/
+00000310: 706c 7567 696e 732f 6e61 7061 7269 2d73  plugins/napari-s
+00000320: 616d 290a 0a53 6567 6d65 6e74 2061 6e79  am)..Segment any
+00000330: 7468 696e 6720 7769 7468 204d 6574 6120  thing with Meta 
+00000340: 4149 2773 206e 6577 2053 414d 206d 6f64  AI's new SAM mod
+00000350: 656c 2077 6974 6820 7468 6920 4e61 7061  el with thi Napa
+00000360: 7269 2070 6c75 6769 6e21 0a0a 5341 4d20  ri plugin!..SAM 
+00000370: 6973 2074 6865 206e 6577 2073 6567 6d65  is the new segme
+00000380: 6e74 6174 696f 6e20 7379 7374 656d 2066  ntation system f
+00000390: 726f 6d20 4d65 7461 2041 4920 6361 7061  rom Meta AI capa
+000003a0: 626c 6520 6f66 202a 2a6f 6e65 2d63 6c69  ble of **one-cli
+000003b0: 636b 2073 6567 6d65 6e74 6174 696f 6e20  ck segmentation 
+000003c0: 6f66 2061 6e79 206f 626a 6563 742a 2a20  of any object** 
+000003d0: 616e 6420 6e6f 7720 6f75 7220 706c 7567  and now our plug
+000003e0: 696e 206e 6561 746c 7920 696e 7465 6772  in neatly integr
+000003f0: 6174 6573 2074 6869 7320 696e 746f 204e  ates this into N
+00000400: 6170 6172 692e 0a0a 5765 2061 6c72 6561  apari...We alrea
+00000410: 6479 202a 2a65 7874 656e 6465 642a 2a20  dy **extended** 
+00000420: 5341 4d73 2063 6c69 636b 2d62 6173 6564  SAMs click-based
+00000430: 2066 6f72 6567 726f 756e 6420 7365 7061   foreground sepa
+00000440: 7261 7469 6f6e 2074 6f20 6675 6c6c 202a  ration to full *
+00000450: 2a63 6c69 636b 2d62 6173 6564 2073 656d  *click-based sem
+00000460: 616e 7469 6320 7365 676d 656e 7461 7469  antic segmentati
+00000470: 6f6e 2026 2069 6e73 7461 6e63 6520 7365  on & instance se
+00000480: 676d 656e 7461 7469 6f6e 2a2a 2077 696c  gmentation** wil
+00000490: 6c20 736f 6f6e 2066 6f6c 6c6f 7721 0a0a  l soon follow!..
+000004a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004c0: 2d2d 0a0a 5341 4d27 7320 6576 6572 7974  --..SAM's everyt
+000004d0: 6869 6e67 206d 6f64 6520 2020 2020 2020  hing mode       
+000004e0: 2020 2020 2020 7c20 204f 7572 2063 6c69        |  Our cli
+000004f0: 636b 2d62 6173 6564 2073 656d 616e 7469  ck-based semanti
+00000500: 6320 7365 676d 656e 7461 7469 6f6e 206d  c segmentation m
+00000510: 6f64 650a 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ode.:-----------
+00000520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
+00000530: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 3a0a 215b 5d28  ----------:.![](
+00000550: 6361 7473 5f69 6e73 7461 6e63 652e 706e  cats_instance.pn
+00000560: 6729 2020 7c20 2021 5b5d 2863 6174 735f  g)  |  ![](cats_
+00000570: 7365 6d61 6e74 6963 2e70 6e67 290a 0a2d  semantic.png)..-
+00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000005a0: 2d0a 3c68 3220 616c 6967 6e3d 2263 656e  -.<h2 align="cen
+000005b0: 7465 7222 3e53 414d 2069 6e20 4e61 7061  ter">SAM in Napa
+000005c0: 7269 2064 656d 6f3c 2f68 323e 0a3c 7020  ri demo</h2>.<p 
+000005d0: 616c 6967 6e3d 2263 656e 7465 7222 3e3c  align="center"><
+000005e0: 656d 3e43 6c69 636b 2074 6f20 706c 6179  em>Click to play
+000005f0: 2074 6865 2076 6964 656f 3c2f 656d 3e3c   the video</em><
+00000600: 2f70 3e0a 3c64 6976 2061 6c69 676e 3d22  /p>.<div align="
+00000610: 6365 6e74 6572 223e 0a20 203c 6120 6872  center">.  <a hr
+00000620: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
+00000630: 796f 7574 7562 652e 636f 6d2f 7761 7463  youtube.com/watc
+00000640: 683f 763d 4f50 4531 586e 7734 3837 4522  h?v=OPE1Xnw487E"
+00000650: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00000660: 7468 756d 706e 6169 6c2e 6a70 6567 2220  thumpnail.jpeg" 
+00000670: 616c 743d 2253 414d 2044 656d 6f22 3e0a  alt="SAM Demo">.
+00000680: 2020 3c2f 613e 0a3c 2f64 6976 3e0a 0a0a    </a>.</div>...
+00000690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006b0: 2d2d 0a0a 2323 2049 6e73 7461 6c6c 6174  --..## Installat
+000006c0: 696f 6e0a 0a54 6865 2070 6c75 6769 6e20  ion..The plugin 
+000006d0: 7265 7175 6972 6573 2060 7079 7468 6f6e  requires `python
+000006e0: 3e3d 332e 3860 2c20 6173 2077 656c 6c20  >=3.8`, as well 
+000006f0: 6173 2060 7079 746f 7263 683e 3d31 2e37  as `pytorch>=1.7
+00000700: 6020 616e 6420 6074 6f72 6368 7669 7369  ` and `torchvisi
+00000710: 6f6e 3e3d 302e 3860 2e20 506c 6561 7365  on>=0.8`. Please
+00000720: 2066 6f6c 6c6f 7720 7468 6520 696e 7374   follow the inst
+00000730: 7275 6374 696f 6e73 2068 6572 6520 746f  ructions here to
+00000740: 2069 6e73 7461 6c6c 2062 6f74 6820 5079   install both Py
+00000750: 546f 7263 6820 616e 6420 546f 7263 6856  Torch and TorchV
+00000760: 6973 696f 6e20 6465 7065 6e64 656e 6369  ision dependenci
+00000770: 6573 2e20 496e 7374 616c 6c69 6e67 2062  es. Installing b
+00000780: 6f74 6820 5079 546f 7263 6820 616e 6420  oth PyTorch and 
+00000790: 546f 7263 6856 6973 696f 6e20 7769 7468  TorchVision with
+000007a0: 2043 5544 4120 7375 7070 6f72 7420 6973   CUDA support is
+000007b0: 2073 7472 6f6e 676c 7920 7265 636f 6d6d   strongly recomm
+000007c0: 656e 6465 642e 0a0a 596f 7520 6361 6e20  ended...You can 
+000007d0: 696e 7374 616c 6c20 606e 6170 6172 692d  install `napari-
+000007e0: 7361 6d60 2076 6961 205b 7069 705d 3a0a  sam` via [pip]:.
+000007f0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00000800: 2067 6974 2b68 7474 7073 3a2f 2f67 6974   git+https://git
+00000810: 6875 622e 636f 6d2f 6661 6365 626f 6f6b  hub.com/facebook
+00000820: 7265 7365 6172 6368 2f73 6567 6d65 6e74  research/segment
+00000830: 2d61 6e79 7468 696e 672e 6769 740a 2020  -anything.git.  
+00000840: 2020 7069 7020 696e 7374 616c 6c20 6e61    pip install na
+00000850: 7061 7269 2d73 616d 0a0a 0a0a 546f 2069  pari-sam....To i
+00000860: 6e73 7461 6c6c 206c 6174 6573 7420 6465  nstall latest de
+00000870: 7665 6c6f 706d 656e 7420 7665 7273 696f  velopment versio
+00000880: 6e20 3a0a 0a20 2020 2070 6970 2069 6e73  n :..    pip ins
+00000890: 7461 6c6c 2067 6974 2b68 7474 7073 3a2f  tall git+https:/
+000008a0: 2f67 6974 6875 622e 636f 6d2f 4d49 432d  /github.com/MIC-
+000008b0: 444b 465a 2f6e 6170 6172 692d 7361 6d2e  DKFZ/napari-sam.
+000008c0: 6769 740a 0a0a 2323 2043 6f6e 7472 6962  git...## Contrib
+000008d0: 7574 696e 670a 0a43 6f6e 7472 6962 7574  uting..Contribut
+000008e0: 696f 6e73 2061 7265 2076 6572 7920 7765  ions are very we
+000008f0: 6c63 6f6d 652e 2054 6573 7473 2063 616e  lcome. Tests can
+00000900: 2062 6520 7275 6e20 7769 7468 205b 746f   be run with [to
+00000910: 785d 2c20 706c 6561 7365 2065 6e73 7572  x], please ensur
+00000920: 650a 7468 6520 636f 7665 7261 6765 2061  e.the coverage a
+00000930: 7420 6c65 6173 7420 7374 6179 7320 7468  t least stays th
+00000940: 6520 7361 6d65 2062 6566 6f72 6520 796f  e same before yo
+00000950: 7520 7375 626d 6974 2061 2070 756c 6c20  u submit a pull 
+00000960: 7265 7175 6573 742e 0a0a 2323 204c 6963  request...## Lic
+00000970: 656e 7365 0a0a 4469 7374 7269 6275 7465  ense..Distribute
+00000980: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
+00000990: 7320 6f66 2074 6865 205b 4170 6163 6865  s of the [Apache
+000009a0: 2053 6f66 7477 6172 6520 4c69 6365 6e73   Software Licens
+000009b0: 6520 322e 305d 206c 6963 656e 7365 2c0a  e 2.0] license,.
+000009c0: 226e 6170 6172 692d 7361 6d22 2069 7320  "napari-sam" is 
+000009d0: 6672 6565 2061 6e64 206f 7065 6e20 736f  free and open so
+000009e0: 7572 6365 2073 6f66 7477 6172 650a 0a23  urce software..#
+000009f0: 2320 4973 7375 6573 0a0a 4966 2079 6f75  # Issues..If you
+00000a00: 2065 6e63 6f75 6e74 6572 2061 6e79 2070   encounter any p
+00000a10: 726f 626c 656d 732c 2070 6c65 6173 6520  roblems, please 
+00000a20: 5b66 696c 6520 616e 2069 7373 7565 5d20  [file an issue] 
+00000a30: 616c 6f6e 6720 7769 7468 2061 2064 6574  along with a det
+00000a40: 6169 6c65 6420 6465 7363 7269 7074 696f  ailed descriptio
+00000a50: 6e2e 0a0a 5b6e 6170 6172 695d 3a20 6874  n...[napari]: ht
+00000a60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000a70: 2f6e 6170 6172 692f 6e61 7061 7269 0a5b  /napari/napari.[
+00000a80: 436f 6f6b 6965 6375 7474 6572 5d3a 2068  Cookiecutter]: h
+00000a90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000aa0: 6d2f 6175 6472 6579 722f 636f 6f6b 6965  m/audreyr/cookie
+00000ab0: 6375 7474 6572 0a5b 406e 6170 6172 695d  cutter.[@napari]
+00000ac0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000ad0: 2e63 6f6d 2f6e 6170 6172 690a 5b4d 4954  .com/napari.[MIT
+00000ae0: 5d3a 2068 7474 703a 2f2f 6f70 656e 736f  ]: http://openso
+00000af0: 7572 6365 2e6f 7267 2f6c 6963 656e 7365  urce.org/license
+00000b00: 732f 4d49 540a 5b42 5344 2d33 5d3a 2068  s/MIT.[BSD-3]: h
+00000b10: 7474 703a 2f2f 6f70 656e 736f 7572 6365  ttp://opensource
+00000b20: 2e6f 7267 2f6c 6963 656e 7365 732f 4253  .org/licenses/BS
+00000b30: 442d 332d 436c 6175 7365 0a5b 474e 5520  D-3-Clause.[GNU 
+00000b40: 4750 4c20 7633 2e30 5d3a 2068 7474 703a  GPL v3.0]: http:
+00000b50: 2f2f 7777 772e 676e 752e 6f72 672f 6c69  //www.gnu.org/li
+00000b60: 6365 6e73 6573 2f67 706c 2d33 2e30 2e74  censes/gpl-3.0.t
+00000b70: 7874 0a5b 474e 5520 4c47 504c 2076 332e  xt.[GNU LGPL v3.
+00000b80: 305d 3a20 6874 7470 3a2f 2f77 7777 2e67  0]: http://www.g
+00000b90: 6e75 2e6f 7267 2f6c 6963 656e 7365 732f  nu.org/licenses/
+00000ba0: 6c67 706c 2d33 2e30 2e74 7874 0a5b 4170  lgpl-3.0.txt.[Ap
+00000bb0: 6163 6865 2053 6f66 7477 6172 6520 4c69  ache Software Li
+00000bc0: 6365 6e73 6520 322e 305d 3a20 6874 7470  cense 2.0]: http
+00000bd0: 3a2f 2f77 7777 2e61 7061 6368 652e 6f72  ://www.apache.or
+00000be0: 672f 6c69 6365 6e73 6573 2f4c 4943 454e  g/licenses/LICEN
+00000bf0: 5345 2d32 2e30 0a5b 4d6f 7a69 6c6c 6120  SE-2.0.[Mozilla 
+00000c00: 5075 626c 6963 204c 6963 656e 7365 2032  Public License 2
+00000c10: 2e30 5d3a 2068 7474 7073 3a2f 2f77 7777  .0]: https://www
+00000c20: 2e6d 6f7a 696c 6c61 2e6f 7267 2f6d 6564  .mozilla.org/med
+00000c30: 6961 2f4d 504c 2f32 2e30 2f69 6e64 6578  ia/MPL/2.0/index
+00000c40: 2e74 7874 0a5b 636f 6f6b 6965 6375 7474  .txt.[cookiecutt
+00000c50: 6572 2d6e 6170 6172 692d 706c 7567 696e  er-napari-plugin
+00000c60: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
+00000c70: 622e 636f 6d2f 6e61 7061 7269 2f63 6f6f  b.com/napari/coo
+00000c80: 6b69 6563 7574 7465 722d 6e61 7061 7269  kiecutter-napari
+00000c90: 2d70 6c75 6769 6e0a 0a5b 6669 6c65 2061  -plugin..[file a
+00000ca0: 6e20 6973 7375 655d 3a20 6874 7470 733a  n issue]: https:
+00000cb0: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 4943  //github.com/MIC
+00000cc0: 2d44 4b46 5a2f 6e61 7061 7269 2d73 616d  -DKFZ/napari-sam
+00000cd0: 2f69 7373 7565 730a 0a5b 6e61 7061 7269  /issues..[napari
+00000ce0: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
+00000cf0: 622e 636f 6d2f 6e61 7061 7269 2f6e 6170  b.com/napari/nap
+00000d00: 6172 690a 5b74 6f78 5d3a 2068 7474 7073  ari.[tox]: https
+00000d10: 3a2f 2f74 6f78 2e72 6561 6474 6865 646f  ://tox.readthedo
+00000d20: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000d30: 0a5b 7069 705d 3a20 6874 7470 733a 2f2f  .[pip]: https://
+00000d40: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000d50: 2f70 6970 2f0a 5b50 7950 495d 3a20 6874  /pip/.[PyPI]: ht
+00000d60: 7470 733a 2f2f 7079 7069 2e6f 7267 2f0a  tps://pypi.org/.
```

### Comparing `napari-sam-0.1.9/setup.cfg` & `napari-sam-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	qtpy
 	napari
 	vispy
+	tqdm
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `napari-sam-0.1.9/src/napari_sam/utils.py` & `napari-sam-0.2.0/src/napari_sam/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 import urllib.request
 from pathlib import Path
 import os
 import os.path
 from os.path import join
+from tqdm import tqdm
 
 SAM_WEIGHTS_URL = {
     "default": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
     "vit_h": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
     "vit_l": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
     "vit_b": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
 }
 
 
-def _report_hook(block_num: int, block_size: int, total_size: int) -> None:
-    downloaded = block_num * block_size
-    percent = downloaded * 100 / total_size
-    downloaded_mb = downloaded / 1024 / 1024
-    total_size_mb = total_size / 1024 / 1024
-    print(
-        f"Download progress: {percent:.1f}% ({downloaded_mb:.1f}/{total_size_mb:.1f} MB)",
-        end="\r",
-    )
+def download_with_progress(url, output_file):
+    # Open the URL and get the content length
+    req = urllib.request.urlopen(url)
+    content_length = int(req.headers.get('Content-Length'))
+
+    # Set up the progress bar
+    progress_bar = tqdm(total=content_length, unit='B', unit_scale=True)
+
+    # Download the file and update the progress bar
+    with open(output_file, 'wb') as f:
+        downloaded_bytes = 0
+        while True:
+            buffer = req.read(8192)
+            if not buffer:
+                break
+            downloaded_bytes += len(buffer)
+            f.write(buffer)
+            progress_bar.update(len(buffer))
+
+    # Close the progress bar and the URL
+    progress_bar.close()
+    req.close()
 
 
-def get_weights_path(model_type: str) -> Path:
-    """Returns the path to the weight of a given model architecture."""
+def get_weights_path(model_type):
     weight_url = SAM_WEIGHTS_URL[model_type]
 
     cache_dir = Path.home() / ".cache/napari-segment-anything"
     cache_dir.mkdir(parents=True, exist_ok=True)
 
     weight_path = cache_dir / weight_url.split("/")[-1]
 
-    # Download the weights if they don't exist
     if not weight_path.exists():
-        print(f"Downloading {weight_url} to {weight_path} ...")
-        urllib.request.urlretrieve(
-            weight_url, str(weight_path), reporthook=_report_hook
-        )
-        print("\rDownload complete.                           ")
+        print("Downloading {} to {} ...".format(weight_url, weight_path))
+        download_with_progress(weight_url, weight_path)
 
     return weight_path
 
 
 def get_cached_weight_types(model_types):
     cached_weight_types = {}
     cache_dir = str(Path.home() / ".cache/napari-segment-anything")
```

### Comparing `napari-sam-0.1.9/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e61 7061  : 2.1.Name: napa
 00000020: 7269 2d73 616d 0a56 6572 7369 6f6e 3a20  ri-sam.Version: 
-00000030: 302e 312e 390a 5375 6d6d 6172 793a 2053  0.1.9.Summary: S
+00000030: 302e 322e 300a 5375 6d6d 6172 793a 2053  0.2.0.Summary: S
 00000040: 6567 6d65 6e74 2061 6e79 7468 696e 6720  egment anything 
 00000050: 7769 7468 204d 6574 6120 4149 2773 206e  with Meta AI's n
 00000060: 6577 2053 414d 206d 6f64 656c 210a 486f  ew SAM model!.Ho
 00000070: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000080: 2f67 6974 6875 622e 636f 6d2f 4d49 432d  /github.com/MIC-
 00000090: 444b 465a 2f6e 6170 6172 692d 7361 6d0a  DKFZ/napari-sam.
 000000a0: 4175 7468 6f72 3a20 4b61 726f 6c20 476f  Author: Karol Go
@@ -71,171 +71,223 @@
 00000460: 7369 6e67 0a52 6571 7569 7265 732d 5079  sing.Requires-Py
 00000470: 7468 6f6e 3a20 3e3d 332e 380a 4465 7363  thon: >=3.8.Desc
 00000480: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
 00000490: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
 000004a0: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
 000004b0: 7261 3a20 7465 7374 696e 670a 4c69 6365  ra: testing.Lice
 000004c0: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-000004d0: 450a 0a23 206e 6170 6172 692d 7361 6d0a  E..# napari-sam.
-000004e0: 0a5b 215b 4c69 6365 6e73 6520 4170 6163  .[![License Apac
-000004f0: 6865 2053 6f66 7477 6172 6520 4c69 6365  he Software Lice
-00000500: 6e73 6520 322e 305d 2868 7474 7073 3a2f  nse 2.0](https:/
-00000510: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000520: 7079 7069 2f6c 2f6e 6170 6172 692d 7361  pypi/l/napari-sa
-00000530: 6d2e 7376 673f 636f 6c6f 723d 6772 6565  m.svg?color=gree
-00000540: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
-00000550: 7562 2e63 6f6d 2f4d 4943 2d44 4b46 5a2f  ub.com/MIC-DKFZ/
-00000560: 6e61 7061 7269 2d73 616d 2f72 6177 2f6d  napari-sam/raw/m
-00000570: 6169 6e2f 4c49 4345 4e53 4529 0a5b 215b  ain/LICENSE).[![
-00000580: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
-00000590: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000005a0: 692f 762f 6e61 7061 7269 2d73 616d 2e73  i/v/napari-sam.s
-000005b0: 7667 3f63 6f6c 6f72 3d67 7265 656e 295d  vg?color=green)]
-000005c0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-000005d0: 672f 7072 6f6a 6563 742f 6e61 7061 7269  g/project/napari
-000005e0: 2d73 616d 290a 5b21 5b50 7974 686f 6e20  -sam).[![Python 
-000005f0: 5665 7273 696f 6e5d 2868 7474 7073 3a2f  Version](https:/
-00000600: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000610: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
-00000620: 6e61 7061 7269 2d73 616d 2e73 7667 3f63  napari-sam.svg?c
-00000630: 6f6c 6f72 3d67 7265 656e 295d 2868 7474  olor=green)](htt
-00000640: 7073 3a2f 2f70 7974 686f 6e2e 6f72 6729  ps://python.org)
-00000650: 0a5b 215b 7465 7374 735d 2868 7474 7073  .[![tests](https
-00000660: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d49  ://github.com/MI
-00000670: 432d 444b 465a 2f6e 6170 6172 692d 7361  C-DKFZ/napari-sa
-00000680: 6d2f 776f 726b 666c 6f77 732f 7465 7374  m/workflows/test
-00000690: 732f 6261 6467 652e 7376 6729 5d28 6874  s/badge.svg)](ht
-000006a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000006b0: 2f4d 4943 2d44 4b46 5a2f 6e61 7061 7269  /MIC-DKFZ/napari
-000006c0: 2d73 616d 2f61 6374 696f 6e73 290a 5b21  -sam/actions).[!
-000006d0: 5b63 6f64 6563 6f76 5d28 6874 7470 733a  [codecov](https:
-000006e0: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
-000006f0: 4d49 432d 444b 465a 2f6e 6170 6172 692d  MIC-DKFZ/napari-
-00000700: 7361 6d2f 6272 616e 6368 2f6d 6169 6e2f  sam/branch/main/
-00000710: 6772 6170 682f 6261 6467 652e 7376 6729  graph/badge.svg)
-00000720: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
-00000730: 762e 696f 2f67 682f 4d49 432d 444b 465a  v.io/gh/MIC-DKFZ
-00000740: 2f6e 6170 6172 692d 7361 6d29 0a5b 215b  /napari-sam).[![
-00000750: 6e61 7061 7269 2068 7562 5d28 6874 7470  napari hub](http
-00000760: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000770: 696f 2f65 6e64 706f 696e 743f 7572 6c3d  io/endpoint?url=
-00000780: 6874 7470 733a 2f2f 6170 692e 6e61 7061  https://api.napa
-00000790: 7269 2d68 7562 2e6f 7267 2f73 6869 656c  ri-hub.org/shiel
-000007a0: 6473 2f6e 6170 6172 692d 7361 6d29 5d28  ds/napari-sam)](
-000007b0: 6874 7470 733a 2f2f 6e61 7061 7269 2d68  https://napari-h
-000007c0: 7562 2e6f 7267 2f70 6c75 6769 6e73 2f6e  ub.org/plugins/n
-000007d0: 6170 6172 692d 7361 6d29 0a0a 5365 676d  apari-sam)..Segm
-000007e0: 656e 7420 616e 7974 6869 6e67 2077 6974  ent anything wit
-000007f0: 6820 4d65 7461 2041 4927 7320 6e65 7720  h Meta AI's new 
-00000800: 5341 4d20 6d6f 6465 6c21 0a0a 2d2d 2d2d  SAM model!..----
-00000810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00000830: 5468 6973 205b 6e61 7061 7269 5d20 706c  This [napari] pl
-00000840: 7567 696e 2077 6173 2067 656e 6572 6174  ugin was generat
-00000850: 6564 2077 6974 6820 5b43 6f6f 6b69 6563  ed with [Cookiec
-00000860: 7574 7465 725d 2075 7369 6e67 205b 406e  utter] using [@n
-00000870: 6170 6172 695d 2773 205b 636f 6f6b 6965  apari]'s [cookie
-00000880: 6375 7474 6572 2d6e 6170 6172 692d 706c  cutter-napari-pl
-00000890: 7567 696e 5d20 7465 6d70 6c61 7465 2e0a  ugin] template..
-000008a0: 0a3c 212d 2d0a 446f 6e27 7420 6d69 7373  .<!--.Don't miss
-000008b0: 2074 6865 2066 756c 6c20 6765 7474 696e   the full gettin
-000008c0: 6720 7374 6172 7465 6420 6775 6964 6520  g started guide 
-000008d0: 746f 2073 6574 2075 7020 796f 7572 206e  to set up your n
-000008e0: 6577 2070 6163 6b61 6765 3a0a 6874 7470  ew package:.http
-000008f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
-00000900: 6170 6172 692f 636f 6f6b 6965 6375 7474  apari/cookiecutt
-00000910: 6572 2d6e 6170 6172 692d 706c 7567 696e  er-napari-plugin
-00000920: 2367 6574 7469 6e67 2d73 7461 7274 6564  #getting-started
-00000930: 0a0a 616e 6420 7265 7669 6577 2074 6865  ..and review the
-00000940: 206e 6170 6172 6920 646f 6373 2066 6f72   napari docs for
-00000950: 2070 6c75 6769 6e20 6465 7665 6c6f 7065   plugin develope
-00000960: 7273 3a0a 6874 7470 733a 2f2f 6e61 7061  rs:.https://napa
-00000970: 7269 2e6f 7267 2f73 7461 626c 652f 706c  ri.org/stable/pl
-00000980: 7567 696e 732f 696e 6465 782e 6874 6d6c  ugins/index.html
-00000990: 0a2d 2d3e 0a0a 2323 2049 6e73 7461 6c6c  .-->..## Install
-000009a0: 6174 696f 6e0a 0a59 6f75 2063 616e 2069  ation..You can i
-000009b0: 6e73 7461 6c6c 2060 6e61 7061 7269 2d73  nstall `napari-s
-000009c0: 616d 6020 7669 6120 5b70 6970 5d3a 0a0a  am` via [pip]:..
-000009d0: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
-000009e0: 6e61 7061 7269 2d73 616d 0a0a 0a0a 546f  napari-sam....To
-000009f0: 2069 6e73 7461 6c6c 206c 6174 6573 7420   install latest 
-00000a00: 6465 7665 6c6f 706d 656e 7420 7665 7273  development vers
-00000a10: 696f 6e20 3a0a 0a20 2020 2070 6970 2069  ion :..    pip i
-00000a20: 6e73 7461 6c6c 2067 6974 2b68 7474 7073  nstall git+https
-00000a30: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d49  ://github.com/MI
-00000a40: 432d 444b 465a 2f6e 6170 6172 692d 7361  C-DKFZ/napari-sa
-00000a50: 6d2e 6769 740a 0a0a 2323 2043 6f6e 7472  m.git...## Contr
-00000a60: 6962 7574 696e 670a 0a43 6f6e 7472 6962  ibuting..Contrib
-00000a70: 7574 696f 6e73 2061 7265 2076 6572 7920  utions are very 
-00000a80: 7765 6c63 6f6d 652e 2054 6573 7473 2063  welcome. Tests c
-00000a90: 616e 2062 6520 7275 6e20 7769 7468 205b  an be run with [
-00000aa0: 746f 785d 2c20 706c 6561 7365 2065 6e73  tox], please ens
-00000ab0: 7572 650a 7468 6520 636f 7665 7261 6765  ure.the coverage
-00000ac0: 2061 7420 6c65 6173 7420 7374 6179 7320   at least stays 
-00000ad0: 7468 6520 7361 6d65 2062 6566 6f72 6520  the same before 
-00000ae0: 796f 7520 7375 626d 6974 2061 2070 756c  you submit a pul
-00000af0: 6c20 7265 7175 6573 742e 0a0a 2323 204c  l request...## L
-00000b00: 6963 656e 7365 0a0a 4469 7374 7269 6275  icense..Distribu
-00000b10: 7465 6420 756e 6465 7220 7468 6520 7465  ted under the te
-00000b20: 726d 7320 6f66 2074 6865 205b 4170 6163  rms of the [Apac
-00000b30: 6865 2053 6f66 7477 6172 6520 4c69 6365  he Software Lice
-00000b40: 6e73 6520 322e 305d 206c 6963 656e 7365  nse 2.0] license
-00000b50: 2c0a 226e 6170 6172 692d 7361 6d22 2069  ,."napari-sam" i
-00000b60: 7320 6672 6565 2061 6e64 206f 7065 6e20  s free and open 
-00000b70: 736f 7572 6365 2073 6f66 7477 6172 650a  source software.
-00000b80: 0a23 2320 4973 7375 6573 0a0a 4966 2079  .## Issues..If y
-00000b90: 6f75 2065 6e63 6f75 6e74 6572 2061 6e79  ou encounter any
-00000ba0: 2070 726f 626c 656d 732c 2070 6c65 6173   problems, pleas
-00000bb0: 6520 5b66 696c 6520 616e 2069 7373 7565  e [file an issue
-00000bc0: 5d20 616c 6f6e 6720 7769 7468 2061 2064  ] along with a d
-00000bd0: 6574 6169 6c65 6420 6465 7363 7269 7074  etailed descript
-00000be0: 696f 6e2e 0a0a 5b6e 6170 6172 695d 3a20  ion...[napari]: 
-00000bf0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c00: 6f6d 2f6e 6170 6172 692f 6e61 7061 7269  om/napari/napari
-00000c10: 0a5b 436f 6f6b 6965 6375 7474 6572 5d3a  .[Cookiecutter]:
-00000c20: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000c30: 636f 6d2f 6175 6472 6579 722f 636f 6f6b  com/audreyr/cook
-00000c40: 6965 6375 7474 6572 0a5b 406e 6170 6172  iecutter.[@napar
-00000c50: 695d 3a20 6874 7470 733a 2f2f 6769 7468  i]: https://gith
-00000c60: 7562 2e63 6f6d 2f6e 6170 6172 690a 5b4d  ub.com/napari.[M
-00000c70: 4954 5d3a 2068 7474 703a 2f2f 6f70 656e  IT]: http://open
-00000c80: 736f 7572 6365 2e6f 7267 2f6c 6963 656e  source.org/licen
-00000c90: 7365 732f 4d49 540a 5b42 5344 2d33 5d3a  ses/MIT.[BSD-3]:
-00000ca0: 2068 7474 703a 2f2f 6f70 656e 736f 7572   http://opensour
-00000cb0: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
-00000cc0: 4253 442d 332d 436c 6175 7365 0a5b 474e  BSD-3-Clause.[GN
-00000cd0: 5520 4750 4c20 7633 2e30 5d3a 2068 7474  U GPL v3.0]: htt
-00000ce0: 703a 2f2f 7777 772e 676e 752e 6f72 672f  p://www.gnu.org/
-00000cf0: 6c69 6365 6e73 6573 2f67 706c 2d33 2e30  licenses/gpl-3.0
-00000d00: 2e74 7874 0a5b 474e 5520 4c47 504c 2076  .txt.[GNU LGPL v
-00000d10: 332e 305d 3a20 6874 7470 3a2f 2f77 7777  3.0]: http://www
-00000d20: 2e67 6e75 2e6f 7267 2f6c 6963 656e 7365  .gnu.org/license
-00000d30: 732f 6c67 706c 2d33 2e30 2e74 7874 0a5b  s/lgpl-3.0.txt.[
-00000d40: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
-00000d50: 4c69 6365 6e73 6520 322e 305d 3a20 6874  License 2.0]: ht
-00000d60: 7470 3a2f 2f77 7777 2e61 7061 6368 652e  tp://www.apache.
-00000d70: 6f72 672f 6c69 6365 6e73 6573 2f4c 4943  org/licenses/LIC
-00000d80: 454e 5345 2d32 2e30 0a5b 4d6f 7a69 6c6c  ENSE-2.0.[Mozill
-00000d90: 6120 5075 626c 6963 204c 6963 656e 7365  a Public License
-00000da0: 2032 2e30 5d3a 2068 7474 7073 3a2f 2f77   2.0]: https://w
-00000db0: 7777 2e6d 6f7a 696c 6c61 2e6f 7267 2f6d  ww.mozilla.org/m
-00000dc0: 6564 6961 2f4d 504c 2f32 2e30 2f69 6e64  edia/MPL/2.0/ind
-00000dd0: 6578 2e74 7874 0a5b 636f 6f6b 6965 6375  ex.txt.[cookiecu
-00000de0: 7474 6572 2d6e 6170 6172 692d 706c 7567  tter-napari-plug
-00000df0: 696e 5d3a 2068 7474 7073 3a2f 2f67 6974  in]: https://git
-00000e00: 6875 622e 636f 6d2f 6e61 7061 7269 2f63  hub.com/napari/c
-00000e10: 6f6f 6b69 6563 7574 7465 722d 6e61 7061  ookiecutter-napa
-00000e20: 7269 2d70 6c75 6769 6e0a 0a5b 6669 6c65  ri-plugin..[file
-00000e30: 2061 6e20 6973 7375 655d 3a20 6874 7470   an issue]: http
-00000e40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
-00000e50: 4943 2d44 4b46 5a2f 6e61 7061 7269 2d73  IC-DKFZ/napari-s
-00000e60: 616d 2f69 7373 7565 730a 0a5b 6e61 7061  am/issues..[napa
-00000e70: 7269 5d3a 2068 7474 7073 3a2f 2f67 6974  ri]: https://git
-00000e80: 6875 622e 636f 6d2f 6e61 7061 7269 2f6e  hub.com/napari/n
-00000e90: 6170 6172 690a 5b74 6f78 5d3a 2068 7474  apari.[tox]: htt
-00000ea0: 7073 3a2f 2f74 6f78 2e72 6561 6474 6865  ps://tox.readthe
-00000eb0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00000ec0: 742f 0a5b 7069 705d 3a20 6874 7470 733a  t/.[pip]: https:
-00000ed0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000ee0: 6374 2f70 6970 2f0a 5b50 7950 495d 3a20  ct/pip/.[PyPI]: 
-00000ef0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000f00: 2f0a                                     /.
+000004d0: 450a 0a23 2053 6567 6d65 6e74 2041 6e79  E..# Segment Any
+000004e0: 7468 696e 6720 4d6f 6465 6c20 2853 414d  thing Model (SAM
+000004f0: 2920 696e 204e 6170 6172 690a 0a5b 215b  ) in Napari..[![
+00000500: 4c69 6365 6e73 6520 4170 6163 6865 2053  License Apache S
+00000510: 6f66 7477 6172 6520 4c69 6365 6e73 6520  oftware License 
+00000520: 322e 305d 2868 7474 7073 3a2f 2f69 6d67  2.0](https://img
+00000530: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000540: 2f6c 2f6e 6170 6172 692d 7361 6d2e 7376  /l/napari-sam.sv
+00000550: 673f 636f 6c6f 723d 6772 6565 6e29 5d28  g?color=green)](
+00000560: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000570: 6f6d 2f4d 4943 2d44 4b46 5a2f 6e61 7061  om/MIC-DKFZ/napa
+00000580: 7269 2d73 616d 2f72 6177 2f6d 6169 6e2f  ri-sam/raw/main/
+00000590: 4c49 4345 4e53 4529 0a5b 215b 5079 5049  LICENSE).[![PyPI
+000005a0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000005b0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+000005c0: 6e61 7061 7269 2d73 616d 2e73 7667 3f63  napari-sam.svg?c
+000005d0: 6f6c 6f72 3d67 7265 656e 295d 2868 7474  olor=green)](htt
+000005e0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+000005f0: 6f6a 6563 742f 6e61 7061 7269 2d73 616d  oject/napari-sam
+00000600: 290a 5b21 5b50 7974 686f 6e20 5665 7273  ).[![Python Vers
+00000610: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
+00000620: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000630: 2f70 7976 6572 7369 6f6e 732f 6e61 7061  /pyversions/napa
+00000640: 7269 2d73 616d 2e73 7667 3f63 6f6c 6f72  ri-sam.svg?color
+00000650: 3d67 7265 656e 295d 2868 7474 7073 3a2f  =green)](https:/
+00000660: 2f70 7974 686f 6e2e 6f72 6729 0a5b 215b  /python.org).[![
+00000670: 7465 7374 735d 2868 7474 7073 3a2f 2f67  tests](https://g
+00000680: 6974 6875 622e 636f 6d2f 4d49 432d 444b  ithub.com/MIC-DK
+00000690: 465a 2f6e 6170 6172 692d 7361 6d2f 776f  FZ/napari-sam/wo
+000006a0: 726b 666c 6f77 732f 7465 7374 732f 6261  rkflows/tests/ba
+000006b0: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+000006c0: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 4943  //github.com/MIC
+000006d0: 2d44 4b46 5a2f 6e61 7061 7269 2d73 616d  -DKFZ/napari-sam
+000006e0: 2f61 6374 696f 6e73 290a 5b21 5b63 6f64  /actions).[![cod
+000006f0: 6563 6f76 5d28 6874 7470 733a 2f2f 636f  ecov](https://co
+00000700: 6465 636f 762e 696f 2f67 682f 4d49 432d  decov.io/gh/MIC-
+00000710: 444b 465a 2f6e 6170 6172 692d 7361 6d2f  DKFZ/napari-sam/
+00000720: 6272 616e 6368 2f6d 6169 6e2f 6772 6170  branch/main/grap
+00000730: 682f 6261 6467 652e 7376 6729 5d28 6874  h/badge.svg)](ht
+00000740: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000750: 2f67 682f 4d49 432d 444b 465a 2f6e 6170  /gh/MIC-DKFZ/nap
+00000760: 6172 692d 7361 6d29 0a5b 215b 6e61 7061  ari-sam).[![napa
+00000770: 7269 2068 7562 5d28 6874 7470 733a 2f2f  ri hub](https://
+00000780: 696d 672e 7368 6965 6c64 732e 696f 2f65  img.shields.io/e
+00000790: 6e64 706f 696e 743f 7572 6c3d 6874 7470  ndpoint?url=http
+000007a0: 733a 2f2f 6170 692e 6e61 7061 7269 2d68  s://api.napari-h
+000007b0: 7562 2e6f 7267 2f73 6869 656c 6473 2f6e  ub.org/shields/n
+000007c0: 6170 6172 692d 7361 6d29 5d28 6874 7470  apari-sam)](http
+000007d0: 733a 2f2f 6e61 7061 7269 2d68 7562 2e6f  s://napari-hub.o
+000007e0: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
+000007f0: 692d 7361 6d29 0a0a 5365 676d 656e 7420  i-sam)..Segment 
+00000800: 616e 7974 6869 6e67 2077 6974 6820 4d65  anything with Me
+00000810: 7461 2041 4927 7320 6e65 7720 5341 4d20  ta AI's new SAM 
+00000820: 6d6f 6465 6c20 7769 7468 2074 6869 204e  model with thi N
+00000830: 6170 6172 6920 706c 7567 696e 210a 0a53  apari plugin!..S
+00000840: 414d 2069 7320 7468 6520 6e65 7720 7365  AM is the new se
+00000850: 676d 656e 7461 7469 6f6e 2073 7973 7465  gmentation syste
+00000860: 6d20 6672 6f6d 204d 6574 6120 4149 2063  m from Meta AI c
+00000870: 6170 6162 6c65 206f 6620 2a2a 6f6e 652d  apable of **one-
+00000880: 636c 6963 6b20 7365 676d 656e 7461 7469  click segmentati
+00000890: 6f6e 206f 6620 616e 7920 6f62 6a65 6374  on of any object
+000008a0: 2a2a 2061 6e64 206e 6f77 206f 7572 2070  ** and now our p
+000008b0: 6c75 6769 6e20 6e65 6174 6c79 2069 6e74  lugin neatly int
+000008c0: 6567 7261 7465 7320 7468 6973 2069 6e74  egrates this int
+000008d0: 6f20 4e61 7061 7269 2e0a 0a57 6520 616c  o Napari...We al
+000008e0: 7265 6164 7920 2a2a 6578 7465 6e64 6564  ready **extended
+000008f0: 2a2a 2053 414d 7320 636c 6963 6b2d 6261  ** SAMs click-ba
+00000900: 7365 6420 666f 7265 6772 6f75 6e64 2073  sed foreground s
+00000910: 6570 6172 6174 696f 6e20 746f 2066 756c  eparation to ful
+00000920: 6c20 2a2a 636c 6963 6b2d 6261 7365 6420  l **click-based 
+00000930: 7365 6d61 6e74 6963 2073 6567 6d65 6e74  semantic segment
+00000940: 6174 696f 6e20 2620 696e 7374 616e 6365  ation & instance
+00000950: 2073 6567 6d65 6e74 6174 696f 6e2a 2a20   segmentation** 
+00000960: 7769 6c6c 2073 6f6f 6e20 666f 6c6c 6f77  will soon follow
+00000970: 210a 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  !..-------------
+00000980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000990: 2d2d 2d2d 2d0a 0a53 414d 2773 2065 7665  -----..SAM's eve
+000009a0: 7279 7468 696e 6720 6d6f 6465 2020 2020  rything mode    
+000009b0: 2020 2020 2020 2020 207c 2020 4f75 7220           |  Our 
+000009c0: 636c 6963 6b2d 6261 7365 6420 7365 6d61  click-based sema
+000009d0: 6e74 6963 2073 6567 6d65 6e74 6174 696f  ntic segmentatio
+000009e0: 6e20 6d6f 6465 0a3a 2d2d 2d2d 2d2d 2d2d  n mode.:--------
+000009f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a00: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
+00000a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 0a21  -------------:.!
+00000a20: 5b5d 2863 6174 735f 696e 7374 616e 6365  [](cats_instance
+00000a30: 2e70 6e67 2920 207c 2020 215b 5d28 6361  .png)  |  ![](ca
+00000a40: 7473 5f73 656d 616e 7469 632e 706e 6729  ts_semantic.png)
+00000a50: 0a0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..--------------
+00000a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a70: 2d2d 2d2d 0a3c 6832 2061 6c69 676e 3d22  ----.<h2 align="
+00000a80: 6365 6e74 6572 223e 5341 4d20 696e 204e  center">SAM in N
+00000a90: 6170 6172 6920 6465 6d6f 3c2f 6832 3e0a  apari demo</h2>.
+00000aa0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000ab0: 223e 3c65 6d3e 436c 6963 6b20 746f 2070  "><em>Click to p
+00000ac0: 6c61 7920 7468 6520 7669 6465 6f3c 2f65  lay the video</e
+00000ad0: 6d3e 3c2f 703e 0a3c 6469 7620 616c 6967  m></p>.<div alig
+00000ae0: 6e3d 2263 656e 7465 7222 3e0a 2020 3c61  n="center">.  <a
+00000af0: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
+00000b00: 7777 2e79 6f75 7475 6265 2e63 6f6d 2f77  ww.youtube.com/w
+00000b10: 6174 6368 3f76 3d4f 5045 3158 6e77 3438  atch?v=OPE1Xnw48
+00000b20: 3745 223e 0a20 2020 203c 696d 6720 7372  7E">.    <img sr
+00000b30: 633d 2274 6875 6d70 6e61 696c 2e6a 7065  c="thumpnail.jpe
+00000b40: 6722 2061 6c74 3d22 5341 4d20 4465 6d6f  g" alt="SAM Demo
+00000b50: 223e 0a20 203c 2f61 3e0a 3c2f 6469 763e  ">.  </a>.</div>
+00000b60: 0a0a 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ...-------------
+00000b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b80: 2d2d 2d2d 2d0a 0a23 2320 496e 7374 616c  -----..## Instal
+00000b90: 6c61 7469 6f6e 0a0a 5468 6520 706c 7567  lation..The plug
+00000ba0: 696e 2072 6571 7569 7265 7320 6070 7974  in requires `pyt
+00000bb0: 686f 6e3e 3d33 2e38 602c 2061 7320 7765  hon>=3.8`, as we
+00000bc0: 6c6c 2061 7320 6070 7974 6f72 6368 3e3d  ll as `pytorch>=
+00000bd0: 312e 3760 2061 6e64 2060 746f 7263 6876  1.7` and `torchv
+00000be0: 6973 696f 6e3e 3d30 2e38 602e 2050 6c65  ision>=0.8`. Ple
+00000bf0: 6173 6520 666f 6c6c 6f77 2074 6865 2069  ase follow the i
+00000c00: 6e73 7472 7563 7469 6f6e 7320 6865 7265  nstructions here
+00000c10: 2074 6f20 696e 7374 616c 6c20 626f 7468   to install both
+00000c20: 2050 7954 6f72 6368 2061 6e64 2054 6f72   PyTorch and Tor
+00000c30: 6368 5669 7369 6f6e 2064 6570 656e 6465  chVision depende
+00000c40: 6e63 6965 732e 2049 6e73 7461 6c6c 696e  ncies. Installin
+00000c50: 6720 626f 7468 2050 7954 6f72 6368 2061  g both PyTorch a
+00000c60: 6e64 2054 6f72 6368 5669 7369 6f6e 2077  nd TorchVision w
+00000c70: 6974 6820 4355 4441 2073 7570 706f 7274  ith CUDA support
+00000c80: 2069 7320 7374 726f 6e67 6c79 2072 6563   is strongly rec
+00000c90: 6f6d 6d65 6e64 6564 2e0a 0a59 6f75 2063  ommended...You c
+00000ca0: 616e 2069 6e73 7461 6c6c 2060 6e61 7061  an install `napa
+00000cb0: 7269 2d73 616d 6020 7669 6120 5b70 6970  ri-sam` via [pip
+00000cc0: 5d3a 0a0a 2020 2020 7069 7020 696e 7374  ]:..    pip inst
+00000cd0: 616c 6c20 6769 742b 6874 7470 733a 2f2f  all git+https://
+00000ce0: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
+00000cf0: 6f6f 6b72 6573 6561 7263 682f 7365 676d  ookresearch/segm
+00000d00: 656e 742d 616e 7974 6869 6e67 2e67 6974  ent-anything.git
+00000d10: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00000d20: 206e 6170 6172 692d 7361 6d0a 0a0a 0a54   napari-sam....T
+00000d30: 6f20 696e 7374 616c 6c20 6c61 7465 7374  o install latest
+00000d40: 2064 6576 656c 6f70 6d65 6e74 2076 6572   development ver
+00000d50: 7369 6f6e 203a 0a0a 2020 2020 7069 7020  sion :..    pip 
+00000d60: 696e 7374 616c 6c20 6769 742b 6874 7470  install git+http
+00000d70: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
+00000d80: 4943 2d44 4b46 5a2f 6e61 7061 7269 2d73  IC-DKFZ/napari-s
+00000d90: 616d 2e67 6974 0a0a 0a23 2320 436f 6e74  am.git...## Cont
+00000da0: 7269 6275 7469 6e67 0a0a 436f 6e74 7269  ributing..Contri
+00000db0: 6275 7469 6f6e 7320 6172 6520 7665 7279  butions are very
+00000dc0: 2077 656c 636f 6d65 2e20 5465 7374 7320   welcome. Tests 
+00000dd0: 6361 6e20 6265 2072 756e 2077 6974 6820  can be run with 
+00000de0: 5b74 6f78 5d2c 2070 6c65 6173 6520 656e  [tox], please en
+00000df0: 7375 7265 0a74 6865 2063 6f76 6572 6167  sure.the coverag
+00000e00: 6520 6174 206c 6561 7374 2073 7461 7973  e at least stays
+00000e10: 2074 6865 2073 616d 6520 6265 666f 7265   the same before
+00000e20: 2079 6f75 2073 7562 6d69 7420 6120 7075   you submit a pu
+00000e30: 6c6c 2072 6571 7565 7374 2e0a 0a23 2320  ll request...## 
+00000e40: 4c69 6365 6e73 650a 0a44 6973 7472 6962  License..Distrib
+00000e50: 7574 6564 2075 6e64 6572 2074 6865 2074  uted under the t
+00000e60: 6572 6d73 206f 6620 7468 6520 5b41 7061  erms of the [Apa
+00000e70: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
+00000e80: 656e 7365 2032 2e30 5d20 6c69 6365 6e73  ense 2.0] licens
+00000e90: 652c 0a22 6e61 7061 7269 2d73 616d 2220  e,."napari-sam" 
+00000ea0: 6973 2066 7265 6520 616e 6420 6f70 656e  is free and open
+00000eb0: 2073 6f75 7263 6520 736f 6674 7761 7265   source software
+00000ec0: 0a0a 2323 2049 7373 7565 730a 0a49 6620  ..## Issues..If 
+00000ed0: 796f 7520 656e 636f 756e 7465 7220 616e  you encounter an
+00000ee0: 7920 7072 6f62 6c65 6d73 2c20 706c 6561  y problems, plea
+00000ef0: 7365 205b 6669 6c65 2061 6e20 6973 7375  se [file an issu
+00000f00: 655d 2061 6c6f 6e67 2077 6974 6820 6120  e] along with a 
+00000f10: 6465 7461 696c 6564 2064 6573 6372 6970  detailed descrip
+00000f20: 7469 6f6e 2e0a 0a5b 6e61 7061 7269 5d3a  tion...[napari]:
+00000f30: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000f40: 636f 6d2f 6e61 7061 7269 2f6e 6170 6172  com/napari/napar
+00000f50: 690a 5b43 6f6f 6b69 6563 7574 7465 725d  i.[Cookiecutter]
+00000f60: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000f70: 2e63 6f6d 2f61 7564 7265 7972 2f63 6f6f  .com/audreyr/coo
+00000f80: 6b69 6563 7574 7465 720a 5b40 6e61 7061  kiecutter.[@napa
+00000f90: 7269 5d3a 2068 7474 7073 3a2f 2f67 6974  ri]: https://git
+00000fa0: 6875 622e 636f 6d2f 6e61 7061 7269 0a5b  hub.com/napari.[
+00000fb0: 4d49 545d 3a20 6874 7470 3a2f 2f6f 7065  MIT]: http://ope
+00000fc0: 6e73 6f75 7263 652e 6f72 672f 6c69 6365  nsource.org/lice
+00000fd0: 6e73 6573 2f4d 4954 0a5b 4253 442d 335d  nses/MIT.[BSD-3]
+00000fe0: 3a20 6874 7470 3a2f 2f6f 7065 6e73 6f75  : http://opensou
+00000ff0: 7263 652e 6f72 672f 6c69 6365 6e73 6573  rce.org/licenses
+00001000: 2f42 5344 2d33 2d43 6c61 7573 650a 5b47  /BSD-3-Clause.[G
+00001010: 4e55 2047 504c 2076 332e 305d 3a20 6874  NU GPL v3.0]: ht
+00001020: 7470 3a2f 2f77 7777 2e67 6e75 2e6f 7267  tp://www.gnu.org
+00001030: 2f6c 6963 656e 7365 732f 6770 6c2d 332e  /licenses/gpl-3.
+00001040: 302e 7478 740a 5b47 4e55 204c 4750 4c20  0.txt.[GNU LGPL 
+00001050: 7633 2e30 5d3a 2068 7474 703a 2f2f 7777  v3.0]: http://ww
+00001060: 772e 676e 752e 6f72 672f 6c69 6365 6e73  w.gnu.org/licens
+00001070: 6573 2f6c 6770 6c2d 332e 302e 7478 740a  es/lgpl-3.0.txt.
+00001080: 5b41 7061 6368 6520 536f 6674 7761 7265  [Apache Software
+00001090: 204c 6963 656e 7365 2032 2e30 5d3a 2068   License 2.0]: h
+000010a0: 7474 703a 2f2f 7777 772e 6170 6163 6865  ttp://www.apache
+000010b0: 2e6f 7267 2f6c 6963 656e 7365 732f 4c49  .org/licenses/LI
+000010c0: 4345 4e53 452d 322e 300a 5b4d 6f7a 696c  CENSE-2.0.[Mozil
+000010d0: 6c61 2050 7562 6c69 6320 4c69 6365 6e73  la Public Licens
+000010e0: 6520 322e 305d 3a20 6874 7470 733a 2f2f  e 2.0]: https://
+000010f0: 7777 772e 6d6f 7a69 6c6c 612e 6f72 672f  www.mozilla.org/
+00001100: 6d65 6469 612f 4d50 4c2f 322e 302f 696e  media/MPL/2.0/in
+00001110: 6465 782e 7478 740a 5b63 6f6f 6b69 6563  dex.txt.[cookiec
+00001120: 7574 7465 722d 6e61 7061 7269 2d70 6c75  utter-napari-plu
+00001130: 6769 6e5d 3a20 6874 7470 733a 2f2f 6769  gin]: https://gi
+00001140: 7468 7562 2e63 6f6d 2f6e 6170 6172 692f  thub.com/napari/
+00001150: 636f 6f6b 6965 6375 7474 6572 2d6e 6170  cookiecutter-nap
+00001160: 6172 692d 706c 7567 696e 0a0a 5b66 696c  ari-plugin..[fil
+00001170: 6520 616e 2069 7373 7565 5d3a 2068 7474  e an issue]: htt
+00001180: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001190: 4d49 432d 444b 465a 2f6e 6170 6172 692d  MIC-DKFZ/napari-
+000011a0: 7361 6d2f 6973 7375 6573 0a0a 5b6e 6170  sam/issues..[nap
+000011b0: 6172 695d 3a20 6874 7470 733a 2f2f 6769  ari]: https://gi
+000011c0: 7468 7562 2e63 6f6d 2f6e 6170 6172 692f  thub.com/napari/
+000011d0: 6e61 7061 7269 0a5b 746f 785d 3a20 6874  napari.[tox]: ht
+000011e0: 7470 733a 2f2f 746f 782e 7265 6164 7468  tps://tox.readth
+000011f0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00001200: 7374 2f0a 5b70 6970 5d3a 2068 7474 7073  st/.[pip]: https
+00001210: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00001220: 6563 742f 7069 702f 0a5b 5079 5049 5d3a  ect/pip/.[PyPI]:
+00001230: 2068 7474 7073 3a2f 2f70 7970 692e 6f72   https://pypi.or
+00001240: 672f 0a                                  g/.
```

