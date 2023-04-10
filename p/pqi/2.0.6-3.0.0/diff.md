# Comparing `tmp/pqi-2.0.6.tar.gz` & `tmp/pqi-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pqi-2.0.6.tar", last modified: Thu Aug  9 01:06:05 2018, max compression
+gzip compressed data, was "pqi-3.0.0.tar", last modified: Mon Apr 10 11:38:55 2023, max compression
```

## Comparing `pqi-2.0.6.tar` & `pqi-3.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2018-08-09 01:06:05.000000 pqi-2.0.6/
--rw-rw-rw-   0        0        0     4068 2018-08-09 01:06:05.000000 pqi-2.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2018-08-09 01:06:05.000000 pqi-2.0.6/PQI/
--rw-rw-rw-   0        0        0     4378 2018-08-09 01:03:16.000000 pqi-2.0.6/PQI/pqi.py
--rw-rw-rw-   0        0        0        0 2018-08-03 05:18:36.000000 pqi-2.0.6/PQI/__init__.py
-drwxrwxrwx   0        0        0        0 2018-08-09 01:06:05.000000 pqi-2.0.6/pqi.egg-info/
--rw-rw-rw-   0        0        0        1 2018-08-09 01:06:05.000000 pqi-2.0.6/pqi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2018-08-09 01:06:05.000000 pqi-2.0.6/pqi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     4068 2018-08-09 01:06:05.000000 pqi-2.0.6/pqi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        7 2018-08-09 01:06:05.000000 pqi-2.0.6/pqi.egg-info/requires.txt
--rw-rw-rw-   0        0        0      241 2018-08-09 01:06:05.000000 pqi-2.0.6/pqi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        4 2018-08-09 01:06:05.000000 pqi-2.0.6/pqi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2018-08-09 01:06:05.000000 pqi-2.0.6/pqi.egg-info/zip-safe
--rw-rw-rw-   0        0        0     2936 2018-08-03 05:18:36.000000 pqi-2.0.6/README.md
--rw-rw-rw-   0        0        0       85 2018-08-09 01:06:05.000000 pqi-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0      900 2018-08-09 01:02:41.000000 pqi-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:38:55.428377 pqi-3.0.0/
+-rw-rw-rw-   0        0        0     1069 2023-04-10 11:30:45.000000 pqi-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3401 2023-04-10 11:38:55.428377 pqi-3.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 11:38:55.391381 pqi-3.0.0/PQI/
+-rw-rw-rw-   0        0        0        0 2023-04-10 11:30:45.000000 pqi-3.0.0/PQI/__init__.py
+-rw-rw-rw-   0        0        0     4244 2023-04-10 11:30:45.000000 pqi-3.0.0/PQI/pqi.py
+-rw-rw-rw-   0        0        0     3070 2023-04-10 11:30:45.000000 pqi-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 11:38:55.426376 pqi-3.0.0/pqi.egg-info/
+-rw-rw-rw-   0        0        0     3401 2023-04-10 11:38:54.000000 pqi-3.0.0/pqi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-10 11:38:54.000000 pqi-3.0.0/pqi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 11:38:54.000000 pqi-3.0.0/pqi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-10 11:38:54.000000 pqi-3.0.0/pqi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 11:38:54.000000 pqi-3.0.0/pqi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-10 11:38:54.000000 pqi-3.0.0/pqi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-10 11:38:54.000000 pqi-3.0.0/pqi.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       85 2023-04-10 11:38:55.430380 pqi-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      870 2023-04-10 11:30:45.000000 pqi-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pqi-2.0.6/PQI/pqi.py` & `pqi-3.0.0/PQI/pqi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-"""PQI
-Usage:
-  pqi ls
-  pqi use <name>
-  pqi show
-  pqi add <name> <url>
-  pqi remove <name>
-  pqi (-h | --help)
-  pqi (-v | --version)
-Options:
-  -h --help        Show this screen.
-  -v --version     Show version.
-"""
-"""
-     _ __      _,.---._      .=-.-.
-  .-`." ,`.  ,-." - ,  `.   /==/_ /
- /==/, -   \/==/ ,    -  \ |==|, |
-|==| _ .=. |==| - .=.  ,  ||==|  |
-|==| , "=",|==|  : ;=:  - ||==|- |
-|==|-  ".."|==|,  "="  ,  ||==| ,|
-|==|,  |    \==\ _   -    ;|==|- |
-/==/ - |     ".=".  ,  ; -\/==/. /
-`--`---"       `--`--"" `--`--`-`
-                ---- A Terminal Tools For Python
-"""
-
-import os
-import re
-import sys
-import pickle
-import platform
-from docopt import docopt
-try:
-    import configparser
-except:
-    import ConfigParser as configparser
-
-FILE_NAME = "~\\pip\\pip.ini" if ("Windows" in platform.system()) else "~/.pip/pip.conf"
-FILE_PATH = os.path.expanduser(FILE_NAME)
-dir_path = os.path.dirname(FILE_PATH)
-if not os.path.exists(dir_path):
-    os.mkdir(dir_path)
-SOURCES_NAME = os.path.join(dir_path, "sources.dict")
-SOURCES = dict()
-
-if not os.path.exists(SOURCES_NAME):
-    with open(SOURCES_NAME, "wb") as fp:
-        pickle.dump({
-            "pypi": "https://pypi.python.org/simple/",
-            "tuna": "https://pypi.tuna.tsinghua.edu.cn/simple",
-            "douban": "http://pypi.douban.com/simple/",
-            "aliyun": "https://mirrors.aliyun.com/pypi/simple/",
-            "ustc": "https://mirrors.ustc.edu.cn/pypi/web/simple"
-        }, fp)
-with open(SOURCES_NAME, "rb") as fp:
-    SOURCES = pickle.load(fp)
-
-APP_DESC = """
-         PQI
-          ---- A Terminal Tools For Python
-          @author Hangfeng Yang (https:/github.com/Fenghuapiao)
-                        last_update 2018-01-28 15:41
-"""
-
-def list_all_source():
-    print('\n')
-    for key in SOURCES.keys():
-        print(key, '\t', SOURCES[key])
-    print('\n')
-
-def write_file(source_name):
-    with open(FILE_PATH, 'w') as fp:
-        str_ = "[global]\nindex-url = {0}\n[install]\ntrusted-host = {1}".format(
-            SOURCES[source_name], SOURCES[source_name].split('/')[2])
-        fp.write(str_)
-
-def select_source_name(source_name):
-    if source_name not in SOURCES.keys():
-        print("\n{} is not in the Source list.\n".format(source_name))
-    else:
-        write_file(source_name)
-        print("\nSource is changed to {}({}).\n".format(source_name, SOURCES[source_name]))
-
-def show_current_source():
-    if not os.path.exists(FILE_PATH):
-        print("\nCurrent source is pypi.\n")
-        return
-    config = configparser.ConfigParser()
-    config.read(FILE_PATH)
-    index_url = config.get("global", "index-url")
-    for key in SOURCES.keys():
-        if index_url == SOURCES[key]:
-            print("\nCurrent source is {}({}).\n".format(key, index_url))
-            break
-    else:
-         print("\nCurrent source is {}.\n".format(index_url))
-
-def check_url(url):
-    p = re.compile("^https?://.+?/simple/?$")
-    if p.match(url) == None:
-        return False    
-    return True
-
-def add_source(source_name, source_url):
-    if not check_url(source_url):
-        print("\nURL({}) does not conform to the rules.\n".format(source_url))
-        return
-    SOURCES[source_name] = source_url
-    with open(SOURCES_NAME, "wb") as fp:
-        pickle.dump(SOURCES, fp)
-    print("\n{}({}) is add to Source list.\n".format(source_name, source_url))
-
-def remove_source(source_name):
-    if source_name not in SOURCES.keys():
-        print("\n{} is not in the Source list.\n".format(source_name))
-    else:
-        source_url = SOURCES.pop(source_name)
-        with open(SOURCES_NAME, "wb") as fp:
-            pickle.dump(SOURCES, fp)
-        print("\n{}({}) is remove to Source list.\n".format(source_name, source_url))
-
-def main():
-    arguments = docopt(__doc__, version="2.0.6")
-    if arguments["ls"]:
-        list_all_source()
-    elif arguments["use"]:
-        select_source_name(arguments["<name>"])
-    elif arguments["show"]:
-        show_current_source()
-    elif arguments["add"]:
-        add_source(arguments["<name>"], arguments["<url>"])
-    elif arguments["remove"]:
-        remove_source(arguments["<name>"])
-    else:
-        print("input error!")
-
-if __name__ == "__main__":
-    print(APP_DESC)
-    main()
+"""PQI
+Usage:
+  pqi ls
+  pqi use <name>
+  pqi show
+  pqi add <name> <url>
+  pqi remove <name>
+  pqi (-h | --help)
+  pqi (-v | --version)
+Options:
+  -h --help        Show this screen.
+  -v --version     Show version.
+"""
+"""
+     _ __      _,.---._      .=-.-.
+  .-`." ,`.  ,-." - ,  `.   /==/_ /
+ /==/, -   \/==/ ,    -  \ |==|, |
+|==| _ .=. |==| - .=.  ,  ||==|  |
+|==| , "=",|==|  : ;=:  - ||==|- |
+|==|-  ".."|==|,  "="  ,  ||==| ,|
+|==|,  |    \==\ _   -    ;|==|- |
+/==/ - |     ".=".  ,  ; -\/==/. /
+`--`---"       `--`--"" `--`--`-`
+                ---- A Terminal Tools For Python
+"""
+
+import os
+import re
+import sys
+import pickle
+import platform
+from docopt import docopt
+try:
+    import configparser
+except:
+    import ConfigParser as configparser
+
+FILE_NAME = "~\\pip\\pip.ini" if ("Windows" in platform.system()) else "~/.config/pip/pip.conf"
+FILE_PATH = os.path.expanduser(FILE_NAME)
+dir_path = os.path.dirname(FILE_PATH)
+if not os.path.exists(dir_path):
+    os.mkdir(dir_path)
+SOURCES_NAME = os.path.join(dir_path, "sources.dict")
+SOURCES = dict()
+
+if not os.path.exists(SOURCES_NAME):
+    with open(SOURCES_NAME, "wb") as fp:
+        pickle.dump({
+            "pypi": "https://pypi.python.org/simple/",
+            "tuna": "https://pypi.tuna.tsinghua.edu.cn/simple",
+            "douban": "https://pypi.doubanio.com/simple/",
+            "aliyun": "https://mirrors.aliyun.com/pypi/simple/",
+            "ustc": "https://mirrors.ustc.edu.cn/pypi/web/simple"
+        }, fp)
+with open(SOURCES_NAME, "rb") as fp:
+    SOURCES = pickle.load(fp)
+
+APP_DESC = """
+         PQI
+          ---- A Terminal Tools For Python
+          @author Hangfeng Yang (https:/github.com/yhangf)
+                        last_update 2023-04-10 19:27
+"""
+
+def list_all_source():
+    print('\n')
+    for key in SOURCES.keys():
+        print(key, '\t', SOURCES[key])
+    print('\n')
+
+def write_file(source_name):
+    with open(FILE_PATH, 'w') as fp:
+        str_ = "[global]\nindex-url = {0}\n[install]\ntrusted-host = {1}".format(
+            SOURCES[source_name], SOURCES[source_name].split('/')[2])
+        fp.write(str_)
+
+def select_source_name(source_name):
+    if source_name not in SOURCES.keys():
+        print("\n{} is not in the Source list.\n".format(source_name))
+    else:
+        write_file(source_name)
+        print("\nSource is changed to {}({}).\n".format(source_name, SOURCES[source_name]))
+
+def show_current_source():
+    if not os.path.exists(FILE_PATH):
+        print("\nCurrent source is pypi.\n")
+        return
+    config = configparser.ConfigParser()
+    config.read(FILE_PATH)
+    index_url = config.get("global", "index-url")
+    for key in SOURCES.keys():
+        if index_url == SOURCES[key]:
+            print("\nCurrent source is {}({}).\n".format(key, index_url))
+            break
+    else:
+         print("\nCurrent source is {}.\n".format(index_url))
+
+def check_url(url):
+    p = re.compile("^https?://.+?/simple/?$")
+    if p.match(url) == None:
+        return False    
+    return True
+
+def add_source(source_name, source_url):
+    if not check_url(source_url):
+        print("\nURL({}) does not conform to the rules.\n".format(source_url))
+        return
+    SOURCES[source_name] = source_url
+    with open(SOURCES_NAME, "wb") as fp:
+        pickle.dump(SOURCES, fp)
+    print("\n{}({}) is add to Source list.\n".format(source_name, source_url))
+
+def remove_source(source_name):
+    if source_name not in SOURCES.keys():
+        print("\n{} is not in the Source list.\n".format(source_name))
+    else:
+        source_url = SOURCES.pop(source_name)
+        with open(SOURCES_NAME, "wb") as fp:
+            pickle.dump(SOURCES, fp)
+        print("\n{}({}) is remove to Source list.\n".format(source_name, source_url))
+
+def main():
+    arguments = docopt(__doc__, version="3.0.0")
+    if arguments["ls"]:
+        list_all_source()
+    elif arguments["use"]:
+        select_source_name(arguments["<name>"])
+    elif arguments["show"]:
+        show_current_source()
+    elif arguments["add"]:
+        add_source(arguments["<name>"], arguments["<url>"])
+    elif arguments["remove"]:
+        remove_source(arguments["<name>"])
+    else:
+        print("input error!")
+
+if __name__ == "__main__":
+    print(APP_DESC)
+    main()
```

### Comparing `pqi-2.0.6/README.md` & `pqi-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -44,141 +44,149 @@
 000002b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000002d0: 2020 2020 2020 2020 2d2d 2d2d 2062 7920          ---- by 
 000002e0: 4861 6e67 6665 6e67 2059 616e 670d 0a0d  Hangfeng Yang...
 000002f0: 0a60 6060 0d0a 2320 3c70 2061 6c69 676e  .```..# <p align
 00000300: 3d22 6365 6e74 6572 223e 7071 693a 2061  ="center">pqi: a
 00000310: 2074 6572 6d69 6e61 6c20 746f 6f6c 7320   terminal tools 
-00000320: 666f 7220 5079 7468 6f6e 3c2f 703e 0d0a  for Python</p>..
-00000330: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
-00000340: 6572 223e 0d0a 2020 2020 3c61 2068 7265  er">..    <a hre
-00000350: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000360: 622e 636f 6d2f 7968 616e 6766 2f50 7951  b.com/yhangf/PyQ
-00000370: 7569 636b 496e 7374 616c 6c2f 626c 6f62  uickInstall/blob
-00000380: 2f6d 6173 7465 722f 4c49 4345 4e53 4522  /master/LICENSE"
-00000390: 3e0d 0a20 2020 2020 2020 203c 696d 6720  >..        <img 
-000003a0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000003b0: 2e73 6869 656c 6473 2e69 6f2f 636f 636f  .shields.io/coco
-000003c0: 6170 6f64 732f 6c2f 4546 5152 436f 6465  apods/l/EFQRCode
-000003d0: 2e73 7667 3f73 7479 6c65 3d66 6c61 7422  .svg?style=flat"
-000003e0: 3e0d 0a20 2020 2020 2020 203c 2f61 3e0d  >..        </a>.
-000003f0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00000400: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
-00000410: 6e2e 6f72 672f 7079 7069 2f70 7169 223e  n.org/pypi/pqi">
-00000420: 0d0a 2020 2020 2020 2020 3c69 6d67 2073  ..        <img s
-00000430: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000440: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000450: 762f 7071 692e 7376 6722 3e0d 0a20 2020  v/pqi.svg">..   
-00000460: 2020 2020 203c 2f61 3e0d 0a20 2020 203c       </a>..    <
-00000470: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000480: 6769 7468 7562 2e63 6f6d 2f70 7974 686f  github.com/pytho
-00000490: 6e2f 6370 7974 686f 6e22 3e0d 0a20 2020  n/cpython">..   
-000004a0: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
-000004b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000004c0: 6473 2e69 6f2f 6261 6467 652f 6c61 6e67  ds.io/badge/lang
-000004d0: 7561 6765 2d70 7974 686f 6e2d 6666 3639  uage-python-ff69
-000004e0: 6234 2e73 7667 223e 0d0a 2020 2020 2020  b4.svg">..      
-000004f0: 2020 3c2f 613e 0d0a 2020 2020 3c61 2068    </a>..    <a h
-00000500: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000510: 6875 622e 636f 6d2f 7968 616e 6766 2f50  hub.com/yhangf/P
-00000520: 7951 7569 636b 496e 7374 616c 6c22 3e0d  yQuickInstall">.
-00000530: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00000540: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000550: 6473 2e69 6f2f 6769 7468 7562 2f73 7461  ds.io/github/sta
-00000560: 7273 2f79 6861 6e67 662f 5079 5175 6963  rs/yhangf/PyQuic
-00000570: 6b49 6e73 7461 6c6c 2e73 7667 3f73 7479  kInstall.svg?sty
-00000580: 6c65 3d73 6f63 6961 6c26 6c61 6265 6c3d  le=social&label=
-00000590: 5374 6172 223e 0d0a 2020 2020 2020 2020  Star">..        
-000005a0: 3c2f 613e 0d0a 2020 2020 3c61 2068 7265  </a>..    <a hre
-000005b0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-000005c0: 622e 636f 6d2f 7968 616e 6766 2f50 7951  b.com/yhangf/PyQ
-000005d0: 7569 636b 496e 7374 616c 6c22 3e0d 0a20  uickInstall">.. 
-000005e0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-000005f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000600: 2e69 6f2f 6769 7468 7562 2f66 6f72 6b73  .io/github/forks
-00000610: 2f79 6861 6e67 662f 5079 5175 6963 6b49  /yhangf/PyQuickI
-00000620: 6e73 7461 6c6c 2e73 7667 3f73 7479 6c65  nstall.svg?style
-00000630: 3d73 6f63 6961 6c26 6c61 6265 6c3d 466f  =social&label=Fo
-00000640: 726b 223e 0d0a 2020 2020 2020 2020 3c2f  rk">..        </
-00000650: 613e 0d0a 3c2f 703e 0d0a 0d0a e794 b1e4  a>..</p>........
-00000660: ba8e e59b bde5 8685 e980 9ae8 bf87 7069  ..............pi
-00000670: 70e4 b88b e8bd bd70 7974 686f 6ee5 8c85  p......python...
-00000680: e79a 84e9 809f e5ba a6e7 9c9f e79a 84e5  ................
-00000690: be88 e685 a2ef bc8c e5be 88e5 aeb9 e698  ................
-000006a0: 93e5 9ba0 e4b8 bae8 b685 e697 b6e8 808c  ................
-000006b0: e5a4 b1e8 b4a5 efbc 8ce8 808c 7071 69e5  ............pqi.
-000006c0: 8faf e4bb a5e6 8a8a 5079 5069 e6ba 90e8  ........PyPi....
-000006d0: bf85 e980 9fe5 8887 e68d a2e4 b8ba e59b  ................
-000006e0: bde5 8685 e6ba 9074 756e 612c 2064 6f75  .......tuna, dou
-000006f0: 6261 6e2c 2061 6c69 7975 6e2c 2075 7374  ban, aliyun, ust
-00000700: 63e4 bb8e e880 8ce5 8aa0 e5bf ab70 7974  c............pyt
-00000710: 686f 6ee5 8c85 e79a 84e5 ae89 e8a3 85e9  hon.............
-00000720: 809f e5ba a6e3 8082 0d0a 0d0a 0d0a 2323  ..............##
-00000730: 20e6 808e e4b9 88e4 bdbf e794 a828 e585   ............(..
-00000740: bce5 aeb9 7079 322f 7079 332f 6c69 6e75  ....py2/py3/linu
-00000750: 782f 7769 6e64 6f77 732f 4d61 634f 5329  x/windows/MacOS)
-00000760: 0d0a 2323 2320 312e e5ae 89e8 a385 0d0a  ..### 1.........
-00000770: 2323 2323 20e6 96b9 e6b3 95e4 b880 efbc  #### ...........
-00000780: 88e6 8ea8 e88d 90ef bc89 0d0a 6060 600d  ............```.
-00000790: 0a3e 3e3e 2070 6970 2069 6e73 7461 6c6c  .>>> pip install
-000007a0: 2070 7169 0d0a 6060 600d 0a0d 0a23 2323   pqi..```....###
-000007b0: 2320 e696 b9e6 b395 e4ba 8c0d 0a60 6060  # ...........```
-000007c0: 0d0a 3e3e 3e20 6769 7420 636c 6f6e 6520  ..>>> git clone 
-000007d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000007e0: 6f6d 2f79 6861 6e67 662f 5079 5175 6963  om/yhangf/PyQuic
-000007f0: 6b49 6e73 7461 6c6c 2e67 6974 0d0a 3e3e  kInstall.git..>>
-00000800: 3e20 7079 7468 6f6e 3320 7365 7475 702e  > python3 setup.
-00000810: 7079 2069 6e73 7461 6c6c 0d0a 6060 600d  py install..```.
-00000820: 0a0d 0a0d 0a23 2323 2032 2e20 e591 bde4  .....### 2. ....
-00000830: bba4 e8a1 8ce8 be93 e585 a520 6070 7169  ........... `pqi
-00000840: 6020 e59b 9ee8 bda6 0d0a 6060 600d 0a3e  ` ........```..>
-00000850: 3e3e 2070 7169 0d0a 5573 6167 653a 0d0a  >> pqi..Usage:..
-00000860: 2020 7071 6920 6c73 0d0a 2020 7071 6920    pqi ls..  pqi 
-00000870: 7573 6520 3c6e 616d 653e 0d0a 2020 7071  use <name>..  pq
-00000880: 6920 7368 6f77 0d0a 2020 7071 6920 6164  i show..  pqi ad
-00000890: 6420 3c6e 616d 653e 203c 7572 6c3e 0d0a  d <name> <url>..
-000008a0: 2020 7071 6920 7265 6d6f 7665 203c 6e61    pqi remove <na
-000008b0: 6d65 3e0d 0a20 2070 7169 2028 2d68 207c  me>..  pqi (-h |
-000008c0: 202d 2d68 656c 7029 0d0a 2020 7071 6920   --help)..  pqi 
-000008d0: 282d 7620 7c20 2d2d 7665 7273 696f 6e29  (-v | --version)
-000008e0: 0d0a 4f70 7469 6f6e 733a 0d0a 2020 2d68  ..Options:..  -h
-000008f0: 202d 2d68 656c 7020 2020 2020 2020 2053   --help        S
-00000900: 686f 7720 7468 6973 2073 6372 6565 6e2e  how this screen.
-00000910: 0d0a 2020 2d76 202d 2d76 6572 7369 6f6e  ..  -v --version
-00000920: 2020 2020 2053 686f 7720 7665 7273 696f       Show versio
-00000930: 6e2e 0d0a 6060 600d 0a2a 20e5 8897 e4b8  n...```..* .....
-00000940: bee6 8980 e69c 89e6 94af e68c 81e7 9a84  ................
-00000950: 5079 5069 e6ba 900d 0a60 6060 0d0a 3e3e  PyPi.....```..>>
-00000960: 3e20 7071 6920 6c73 0d0a 6060 600d 0a0d  > pqi ls..```...
-00000970: 0a2a 20e6 94b9 e58f 9850 7950 69e6 ba90  .* ......PyPi...
-00000980: 0d0a 6060 600d 0a3e 3e3e 2070 7169 2075  ..```..>>> pqi u
-00000990: 7365 203c 6e61 6d65 3e0d 0a60 6060 0d0a  se <name>..```..
-000009a0: e4be 8be5 ad90 efbc 8ce6 af94 e5a6 82e8  ................
-000009b0: bf90 e8a1 8c60 7071 6920 7573 6520 7475  .....`pqi use tu
-000009c0: 6e61 60e5 8db3 e68a 8ae5 bd93 e589 8d50  na`............P
-000009d0: 7950 69e6 ba90 e694 b9e4 b8ba e6b8 85e5  yPi.............
-000009e0: 8d8e e79a 8450 7950 69e6 ba90 0d0a 0d0a  .....PyPi.......
-000009f0: 2a20 e698 bee7 a4ba e5bd 93e5 898d 5079  * ............Py
-00000a00: 5069 e6ba 900d 0a60 6060 0d0a 3e3e 3e20  Pi.....```..>>> 
-00000a10: 7071 6920 7368 6f77 0d0a 6060 600d 0a0d  pqi show..```...
-00000a20: 0a2a 20e6 b7bb e58a a0e6 96b0 e79a 8470  .* ............p
-00000a30: 6970 e6ba 9028 e5a6 82e6 b7bb e58a a055  ip...(.........U
-00000a40: 5354 43e6 ba90 efbc 890d 0a60 6060 0d0a  STC........```..
-00000a50: 3e3e 3e20 7071 6920 6164 6420 7573 7463  >>> pqi add ustc
-00000a60: 2068 7474 7073 3a2f 2f6d 6972 726f 7273   https://mirrors
-00000a70: 2e75 7374 632e 6564 752e 636e 2f70 7970  .ustc.edu.cn/pyp
-00000a80: 692f 7765 622f 7369 6d70 6c65 0d0a 6060  i/web/simple..``
-00000a90: 600d 0a0d 0a2a 20e7 a7bb e999 a470 6970  `....* ......pip
-00000aa0: e6ba 90ef bc88 e5a6 82e5 ae98 e696 b950  ...............P
-00000ab0: 7950 69e6 ba90 efbc 890d 0a60 6060 0d0a  yPi........```..
-00000ac0: 3e3e 3e20 7071 6920 7265 6d6f 7665 2070  >>> pqi remove p
-00000ad0: 7970 690d 0a60 6060 0d0a 0d0a 2323 2320  ypi..```....### 
-00000ae0: 332e 20e5 8d87 e7ba a7e5 88b0 e69c 80e6  3. .............
-00000af0: 96b0 e789 8860 7071 6960 0d0a 6060 600d  .....`pqi`..```.
-00000b00: 0a3e 3e3e 2070 6970 2069 6e73 7461 6c6c  .>>> pip install
-00000b10: 202d 2d75 7067 7261 6465 2070 7169 0d0a   --upgrade pqi..
-00000b20: 6060 600d 0a0d 0a23 2320 4c49 4345 4e53  ```....## LICENS
-00000b30: 450d 0a5b 4d49 545d 2868 7474 7073 3a2f  E..[MIT](https:/
-00000b40: 2f67 6974 6875 622e 636f 6d2f 7968 616e  /github.com/yhan
-00000b50: 6766 2f50 7951 7569 636b 496e 7374 616c  gf/PyQuickInstal
-00000b60: 6c2f 626c 6f62 2f6d 6173 7465 722f 4c49  l/blob/master/LI
-00000b70: 4345 4e53 4529 0d0a                      CENSE)..
+00000320: 666f 7220 5079 7468 6f6e 3a67 6c6f 6265  for Python:globe
+00000330: 5f77 6974 685f 6d65 7269 6469 616e 733a  _with_meridians:
+00000340: 3c2f 703e 0d0a 0d0a 3c70 2061 6c69 676e  </p>....<p align
+00000350: 3d22 6365 6e74 6572 223e 0d0a 2020 2020  ="center">..    
+00000360: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000370: 2f67 6974 6875 622e 636f 6d2f 7968 616e  /github.com/yhan
+00000380: 6766 2f50 7951 7569 636b 496e 7374 616c  gf/PyQuickInstal
+00000390: 6c2f 626c 6f62 2f6d 6173 7465 722f 4c49  l/blob/master/LI
+000003a0: 4345 4e53 4522 3e0d 0a20 2020 2020 2020  CENSE">..       
+000003b0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+000003c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000003d0: 6f2f 636f 636f 6170 6f64 732f 6c2f 4546  o/cocoapods/l/EF
+000003e0: 5152 436f 6465 2e73 7667 3f73 7479 6c65  QRCode.svg?style
+000003f0: 3d66 6c61 7422 3e0d 0a20 2020 2020 2020  =flat">..       
+00000400: 203c 2f61 3e0d 0a20 2020 203c 6120 6872   </a>..    <a hr
+00000410: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00000420: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
+00000430: 2f70 7169 223e 0d0a 2020 2020 2020 2020  /pqi">..        
+00000440: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000450: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000460: 2f70 7970 692f 762f 7071 692e 7376 6722  /pypi/v/pqi.svg"
+00000470: 3e0d 0a20 2020 2020 2020 203c 2f61 3e0d  >..        </a>.
+00000480: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000490: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000004a0: 2f70 7974 686f 6e2f 6370 7974 686f 6e22  /python/cpython"
+000004b0: 3e0d 0a20 2020 2020 2020 203c 696d 6720  >..        <img 
+000004c0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000004d0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000004e0: 652f 6c61 6e67 7561 6765 2d70 7974 686f  e/language-pytho
+000004f0: 6e2d 6666 3639 6234 2e73 7667 223e 0d0a  n-ff69b4.svg">..
+00000500: 2020 2020 2020 2020 3c2f 613e 0d0a 2020          </a>..  
+00000510: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000520: 3a2f 2f67 6974 6875 622e 636f 6d2f 7968  ://github.com/yh
+00000530: 616e 6766 2f50 7951 7569 636b 496e 7374  angf/PyQuickInst
+00000540: 616c 6c22 3e0d 0a20 2020 203c 696d 6720  all">..    <img 
+00000550: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000560: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000570: 7562 2f73 7461 7273 2f79 6861 6e67 662f  ub/stars/yhangf/
+00000580: 5079 5175 6963 6b49 6e73 7461 6c6c 2e73  PyQuickInstall.s
+00000590: 7667 3f73 7479 6c65 3d73 6f63 6961 6c26  vg?style=social&
+000005a0: 6c61 6265 6c3d 5374 6172 223e 0d0a 2020  label=Star">..  
+000005b0: 2020 2020 2020 3c2f 613e 0d0a 2020 2020        </a>..    
+000005c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000005d0: 2f67 6974 6875 622e 636f 6d2f 7968 616e  /github.com/yhan
+000005e0: 6766 2f50 7951 7569 636b 496e 7374 616c  gf/PyQuickInstal
+000005f0: 6c22 3e0d 0a20 2020 203c 696d 6720 7372  l">..    <img sr
+00000600: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000610: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00000620: 2f66 6f72 6b73 2f79 6861 6e67 662f 5079  /forks/yhangf/Py
+00000630: 5175 6963 6b49 6e73 7461 6c6c 2e73 7667  QuickInstall.svg
+00000640: 3f73 7479 6c65 3d73 6f63 6961 6c26 6c61  ?style=social&la
+00000650: 6265 6c3d 466f 726b 223e 0d0a 2020 2020  bel=Fork">..    
+00000660: 2020 2020 3c2f 613e 0d0a 3c2f 703e 0d0a      </a>..</p>..
+00000670: e794 b1e4 ba8e e59b bde5 8685 e980 9ae8  ................
+00000680: bf87 7069 70e4 b88b e8bd bd70 7974 686f  ..pip......pytho
+00000690: 6ee5 8c85 e79a 84e9 809f e5ba a6e7 9c9f  n...............
+000006a0: e79a 84e5 be88 e685 a2ef bc8c e5be 88e5  ................
+000006b0: aeb9 e698 93e5 9ba0 e4b8 bae8 b685 e697  ................
+000006c0: b6e8 808c e5a4 b1e8 b4a5 efbc 8ce8 808c  ................
+000006d0: 7071 69e5 8faf e4bb a5e6 8a8a 5079 5069  pqi.........PyPi
+000006e0: e6ba 90e8 bf85 e980 9fe5 8887 e68d a2e4  ................
+000006f0: b8ba e59b bde5 8685 e6ba 9074 756e 612c  ...........tuna,
+00000700: 2064 6f75 6261 6e2c 2061 6c69 7975 6e2c   douban, aliyun,
+00000710: 2075 7374 63e4 bb8e e880 8ce5 a4a7 e5a4   ustc...........
+00000720: a7e5 8aa0 e5bf ab70 7974 686f 6ee5 8c85  .......python...
+00000730: e79a 84e5 ae89 e8a3 85e9 809f e5ba a6ef  ................
+00000740: bc8c e68f 90e9 809f e695 88e6 9e9c e8a7  ................
+00000750: 81e4 b88b e59b bee6 8980 e7a4 bae3 8082  ................
+00000760: 0d0a 0d0a 215b 5d28 6874 7470 733a 2f2f  ....![](https://
+00000770: 6769 7468 7562 2e63 6f6d 2f79 6861 6e67  github.com/yhang
+00000780: 662f 5079 5175 6963 6b49 6e73 7461 6c6c  f/PyQuickInstall
+00000790: 2f62 6c6f 622f 6d61 7374 6572 2f70 6963  /blob/master/pic
+000007a0: 7475 7265 2f64 622e 706e 6729 0d0a 0d0a  ture/db.png)....
+000007b0: 2323 20e6 808e e4b9 88e4 bdbf e794 a828  ## ............(
+000007c0: e585 bce5 aeb9 7079 322f 7079 332f 6c69  ......py2/py3/li
+000007d0: 6e75 782f 7769 6e64 6f77 732f 4d61 634f  nux/windows/MacO
+000007e0: 5329 0d0a 0d0a 2323 2320 312e e5ae 89e8  S)....### 1.....
+000007f0: a385 0d0a 2323 2323 20e6 96b9 e6b3 95e4  ....#### .......
+00000800: b880 efbc 88e6 8ea8 e88d 90ef bc89 0d0a  ................
+00000810: 0d0a 6060 600d 0a3e 3e3e 2070 6970 2069  ..```..>>> pip i
+00000820: 6e73 7461 6c6c 2070 7169 0d0a 6060 600d  nstall pqi..```.
+00000830: 0a0d 0a23 2323 2320 e696 b9e6 b395 e4ba  ...#### ........
+00000840: 8c0d 0a60 6060 0d0a 3e3e 3e20 6769 7420  ...```..>>> git 
+00000850: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
+00000860: 7468 7562 2e63 6f6d 2f79 6861 6e67 662f  thub.com/yhangf/
+00000870: 5079 5175 6963 6b49 6e73 7461 6c6c 2e67  PyQuickInstall.g
+00000880: 6974 0d0a 3e3e 3e20 7079 7468 6f6e 3320  it..>>> python3 
+00000890: 7365 7475 702e 7079 2069 6e73 7461 6c6c  setup.py install
+000008a0: 0d0a 6060 600d 0a0d 0a0d 0a23 2323 2032  ..```......### 2
+000008b0: 2e20 e591 bde4 bba4 e8a1 8ce8 be93 e585  . ..............
+000008c0: a520 6070 7169 6020 e59b 9ee8 bda6 0d0a  . `pqi` ........
+000008d0: 6060 600d 0a3e 3e3e 2070 7169 0d0a 5573  ```..>>> pqi..Us
+000008e0: 6167 653a 0d0a 2020 7071 6920 6c73 0d0a  age:..  pqi ls..
+000008f0: 2020 7071 6920 7573 6520 3c6e 616d 653e    pqi use <name>
+00000900: 0d0a 2020 7071 6920 7368 6f77 0d0a 2020  ..  pqi show..  
+00000910: 7071 6920 6164 6420 3c6e 616d 653e 203c  pqi add <name> <
+00000920: 7572 6c3e 0d0a 2020 7071 6920 7265 6d6f  url>..  pqi remo
+00000930: 7665 203c 6e61 6d65 3e0d 0a20 2070 7169  ve <name>..  pqi
+00000940: 2028 2d68 207c 202d 2d68 656c 7029 0d0a   (-h | --help)..
+00000950: 2020 7071 6920 282d 7620 7c20 2d2d 7665    pqi (-v | --ve
+00000960: 7273 696f 6e29 0d0a 4f70 7469 6f6e 733a  rsion)..Options:
+00000970: 0d0a 2020 2d68 202d 2d68 656c 7020 2020  ..  -h --help   
+00000980: 2020 2020 2053 686f 7720 7468 6973 2073       Show this s
+00000990: 6372 6565 6e2e 0d0a 2020 2d76 202d 2d76  creen...  -v --v
+000009a0: 6572 7369 6f6e 2020 2020 2053 686f 7720  ersion     Show 
+000009b0: 7665 7273 696f 6e2e 0d0a 6060 600d 0a2a  version...```..*
+000009c0: 20e5 8897 e4b8 bee6 8980 e69c 89e6 94af   ...............
+000009d0: e68c 81e7 9a84 5079 5069 e6ba 900d 0a60  ......PyPi.....`
+000009e0: 6060 0d0a 3e3e 3e20 7071 6920 6c73 0d0a  ``..>>> pqi ls..
+000009f0: 6060 600d 0a0d 0a2a 20e6 94b9 e58f 9850  ```....* ......P
+00000a00: 7950 69e6 ba90 0d0a 6060 600d 0a3e 3e3e  yPi.....```..>>>
+00000a10: 2070 7169 2075 7365 203c 6e61 6d65 3e0d   pqi use <name>.
+00000a20: 0a60 6060 0d0a e4be 8be5 ad90 efbc 8ce6  .```............
+00000a30: af94 e5a6 82e8 bf90 e8a1 8c60 7071 6920  ...........`pqi 
+00000a40: 7573 6520 7475 6e61 60e5 8db3 e68a 8ae5  use tuna`.......
+00000a50: bd93 e589 8d50 7950 69e6 ba90 e694 b9e4  .....PyPi.......
+00000a60: b8ba e6b8 85e5 8d8e e79a 8450 7950 69e6  ...........PyPi.
+00000a70: ba90 0d0a 0d0a 2a20 e698 bee7 a4ba e5bd  ......* ........
+00000a80: 93e5 898d 5079 5069 e6ba 900d 0a60 6060  ....PyPi.....```
+00000a90: 0d0a 3e3e 3e20 7071 6920 7368 6f77 0d0a  ..>>> pqi show..
+00000aa0: 6060 600d 0a0d 0a2a 20e6 b7bb e58a a0e6  ```....* .......
+00000ab0: 96b0 e79a 8470 6970 e6ba 9028 e5a6 82e6  .....pip...(....
+00000ac0: b7bb e58a a055 5354 43e6 ba90 efbc 890d  .....USTC.......
+00000ad0: 0a60 6060 0d0a 3e3e 3e20 7071 6920 6164  .```..>>> pqi ad
+00000ae0: 6420 7573 7463 2068 7474 7073 3a2f 2f6d  d ustc https://m
+00000af0: 6972 726f 7273 2e75 7374 632e 6564 752e  irrors.ustc.edu.
+00000b00: 636e 2f70 7970 692f 7765 622f 7369 6d70  cn/pypi/web/simp
+00000b10: 6c65 0d0a 6060 600d 0a0d 0a2a 20e7 a7bb  le..```....* ...
+00000b20: e999 a470 6970 e6ba 90ef bc88 e5a6 82e5  ...pip..........
+00000b30: ae98 e696 b950 7950 69e6 ba90 efbc 890d  .....PyPi.......
+00000b40: 0a60 6060 0d0a 3e3e 3e20 7071 6920 7265  .```..>>> pqi re
+00000b50: 6d6f 7665 2070 7970 690d 0a60 6060 0d0a  move pypi..```..
+00000b60: 0d0a 2323 2320 332e 20e5 8d87 e7ba a7e5  ..### 3. .......
+00000b70: 88b0 e69c 80e6 96b0 e789 8860 7071 6960  ...........`pqi`
+00000b80: 0d0a 6060 600d 0a3e 3e3e 2070 6970 2069  ..```..>>> pip i
+00000b90: 6e73 7461 6c6c 202d 2d75 7067 7261 6465  nstall --upgrade
+00000ba0: 2070 7169 0d0a 6060 600d 0a0d 0a23 2320   pqi..```....## 
+00000bb0: 4c49 4345 4e53 450d 0a5b 4d49 545d 2868  LICENSE..[MIT](h
+00000bc0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000bd0: 6d2f 7968 616e 6766 2f50 7951 7569 636b  m/yhangf/PyQuick
+00000be0: 496e 7374 616c 6c2f 626c 6f62 2f6d 6173  Install/blob/mas
+00000bf0: 7465 722f 4c49 4345 4e53 4529 0d0a       ter/LICENSE)..
```

### Comparing `pqi-2.0.6/setup.py` & `pqi-3.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import setup, find_packages
-
-VERSION = '2.0.6'
-
-with open("README.md", "r", encoding="utf-8") as fp:
-    long_description = fp.read()
-
-setup(name='pqi',
-      version=VERSION,
-      description="Fast switching PyPi mirror image source",
-      classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
-      keywords='python、PyPi source、terminal',
-      author='HangfengYang',
-      author_email='yhf5fhy@gmail.com',
-      url='https://github.com/yhangf/PyQuickInstall',
-      license='MIT',
-      packages=["PQI"],
-      long_description=long_description,
-      long_description_content_type="text/markdown",
-      include_package_data=True,
-      zip_safe=True,
-      install_requires=[
-        'docopt',
-      ],
-      entry_points={
-        'console_scripts':[
-            'pqi = PQI.pqi:main'
-        ]
-      },
-)
+from setuptools import setup, find_packages
+
+VERSION = '3.0.0'
+
+with open("README.md", "r", encoding="utf-8") as fp:
+    long_description = fp.read()
+
+setup(name='pqi',
+      version=VERSION,
+      description="Fast switching PyPi mirror image source",
+      classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
+      keywords='python、PyPi source、terminal',
+      author='HangfengYang',
+      author_email='yhf5fhy@gmail.com',
+      url='https://github.com/yhangf/PyQuickInstall',
+      license='MIT',
+      packages=["PQI"],
+      long_description=long_description,
+      long_description_content_type="text/markdown",
+      include_package_data=True,
+      zip_safe=True,
+      install_requires=[
+        'docopt',
+      ],
+      entry_points={
+        'console_scripts':[
+            'pqi = PQI.pqi:main'
+        ]
+      },
+)
```

