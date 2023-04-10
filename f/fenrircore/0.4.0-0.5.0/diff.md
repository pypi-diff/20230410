# Comparing `tmp/fenrircore-0.4.0.tar.gz` & `tmp/fenrircore-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenrircore-0.4.0.tar", last modified: Sun Apr  2 18:10:32 2023, max compression
+gzip compressed data, was "fenrircore-0.5.0.tar", last modified: Mon Apr 10 18:30:46 2023, max compression
```

## Comparing `fenrircore-0.4.0.tar` & `fenrircore-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-02 18:10:32.923353 fenrircore-0.4.0/
--rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-02-17 12:58:30.000000 fenrircore-0.4.0/LICENSE
--rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-02 18:10:32.919353 fenrircore-0.4.0/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)     1673 2023-04-01 22:01:01.000000 fenrircore-0.4.0/README.md
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-02 18:10:32.919353 fenrircore-0.4.0/fenrircore/
--rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-02 18:10:24.000000 fenrircore-0.4.0/fenrircore/__init__.py
--rw-r--r--   0 hannes    (1000) users      (100)    11033 2023-04-01 17:09:45.000000 fenrircore-0.4.0/fenrircore/arper.py
--rw-r--r--   0 hannes    (1000) users      (100)     6539 2023-04-01 17:09:45.000000 fenrircore-0.4.0/fenrircore/fenrir.py
--rw-r--r--   0 hannes    (1000) users      (100)     6706 2023-02-19 18:40:50.000000 fenrircore-0.4.0/fenrircore/filehandler.py
--rw-r--r--   0 hannes    (1000) users      (100)     4923 2023-04-01 17:09:45.000000 fenrircore-0.4.0/fenrircore/firewall.py
--rw-r--r--   0 hannes    (1000) users      (100)     2019 2023-02-17 12:58:30.000000 fenrircore-0.4.0/fenrircore/getmacvendors.py
--rw-r--r--   0 hannes    (1000) users      (100)     8258 2023-03-25 12:41:10.000000 fenrircore-0.4.0/fenrircore/scanner.py
--rw-r--r--   0 hannes    (1000) users      (100)    11899 2023-04-01 17:09:45.000000 fenrircore-0.4.0/fenrircore/vpn.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-02 18:10:32.919353 fenrircore-0.4.0/fenrircore.egg-info/
--rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-02 18:10:32.000000 fenrircore-0.4.0/fenrircore.egg-info/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      446 2023-04-02 18:10:32.000000 fenrircore-0.4.0/fenrircore.egg-info/SOURCES.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-02 18:10:32.000000 fenrircore-0.4.0/fenrircore.egg-info/dependency_links.txt
--rw-r--r--   0 hannes    (1000) users      (100)       54 2023-04-02 18:10:32.000000 fenrircore-0.4.0/fenrircore.egg-info/entry_points.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-02 11:09:58.000000 fenrircore-0.4.0/fenrircore.egg-info/not-zip-safe
--rw-r--r--   0 hannes    (1000) users      (100)       53 2023-04-02 18:10:32.000000 fenrircore-0.4.0/fenrircore.egg-info/requires.txt
--rw-r--r--   0 hannes    (1000) users      (100)       11 2023-04-02 18:10:32.000000 fenrircore-0.4.0/fenrircore.egg-info/top_level.txt
--rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-02 18:10:32.923353 fenrircore-0.4.0/setup.cfg
--rw-r--r--   0 hannes    (1000) users      (100)      900 2023-04-02 18:07:08.000000 fenrircore-0.4.0/setup.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 18:30:46.511050 fenrircore-0.5.0/
+-rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-02-17 12:58:30.000000 fenrircore-0.5.0/LICENSE
+-rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-10 18:30:46.511050 fenrircore-0.5.0/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)     1673 2023-04-01 22:01:01.000000 fenrircore-0.5.0/README.md
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 18:30:46.511050 fenrircore-0.5.0/fenrircore/
+-rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-10 17:51:42.000000 fenrircore-0.5.0/fenrircore/__init__.py
+-rw-r--r--   0 hannes    (1000) users      (100)       65 2023-04-10 17:56:19.000000 fenrircore-0.5.0/fenrircore/__main__.py
+-rw-r--r--   0 hannes    (1000) users      (100)    11033 2023-04-01 17:09:45.000000 fenrircore-0.5.0/fenrircore/arper.py
+-rw-r--r--   0 hannes    (1000) users      (100)     6868 2023-04-10 18:24:20.000000 fenrircore-0.5.0/fenrircore/fenrir.py
+-rw-r--r--   0 hannes    (1000) users      (100)     6706 2023-02-19 18:40:50.000000 fenrircore-0.5.0/fenrircore/filehandler.py
+-rw-r--r--   0 hannes    (1000) users      (100)     4923 2023-04-01 17:09:45.000000 fenrircore-0.5.0/fenrircore/firewall.py
+-rw-r--r--   0 hannes    (1000) users      (100)     2019 2023-02-17 12:58:30.000000 fenrircore-0.5.0/fenrircore/getmacvendors.py
+-rw-r--r--   0 hannes    (1000) users      (100)     8258 2023-03-25 12:41:10.000000 fenrircore-0.5.0/fenrircore/scanner.py
+-rw-r--r--   0 hannes    (1000) users      (100)    11899 2023-04-01 17:09:45.000000 fenrircore-0.5.0/fenrircore/vpn.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 18:30:46.511050 fenrircore-0.5.0/fenrircore.egg-info/
+-rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      469 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/SOURCES.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/dependency_links.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/entry_points.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-02 11:09:58.000000 fenrircore-0.5.0/fenrircore.egg-info/not-zip-safe
+-rw-r--r--   0 hannes    (1000) users      (100)       53 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/requires.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       11 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/top_level.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-10 18:30:46.511050 fenrircore-0.5.0/setup.cfg
+-rw-r--r--   0 hannes    (1000) users      (100)      896 2023-04-10 17:51:36.000000 fenrircore-0.5.0/setup.py
```

### Comparing `fenrircore-0.4.0/LICENSE` & `fenrircore-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenrircore-0.4.0/README.md` & `fenrircore-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fenrircore-0.4.0/fenrircore/arper.py` & `fenrircore-0.5.0/fenrircore/arper.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.4.0/fenrircore/fenrir.py` & `fenrircore-0.5.0/fenrircore/fenrir.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 from . firewall import Firewall
 from . arper import arper
 from . scanner import scan, printresults
 from . vpn import vpn
+from . getmacvendors import updatemacvendors
 from signal import signal, SIGINT, SIGTERM
 from time import sleep
 from os import kill, makedirs, path
 from sys import stdout
 from logging import info, basicConfig, INFO, DEBUG
 from multiprocessing import Process
 from argparse import ArgumentParser
@@ -140,18 +141,22 @@
     parser = ArgumentParser()
     parser.add_argument('--vpninterface', help='interface for VPN traffic', default='tun0')
     parser.add_argument('--inputinterface', help='interface for network scanning/intercepting', default='eth0')
     parser.add_argument('--dbpath', help='path to vpnconfig database', default='/var/cache/fenrir/fenrir.sqlite')
     parser.add_argument('--debug', help='activate debug logging', action='store_true')
     parser.add_argument('--scanonly', help='do network scan and print results', action='store_true')
     parser.add_argument('--password', help='use given password for vpnconfig encryption/decryption', default=None)
+    parser.add_argument('--updatemacvendors', const='/var/cache/fenrir/macvendors.sqlite',
+                        help='update macvendors and store to given path', default=None, nargs='?')
     args = parser.parse_args()
     loglevel = DEBUG if args.debug else INFO
     basicConfig(stream=stdout, level=loglevel)
     if args.scanonly:
         return printresults(args.inputinterface)
+    elif args.updatemacvendors:
+        return updatemacvendors(dbpath=args.updatemacvendors)
     Fenrir(inputinterface=args.inputinterface, vpninterface=args.vpninterface,
            dbpath=args.dbpath, password=args.password).run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fenrircore-0.4.0/fenrircore/filehandler.py` & `fenrircore-0.5.0/fenrircore/filehandler.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.4.0/fenrircore/firewall.py` & `fenrircore-0.5.0/fenrircore/firewall.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.4.0/fenrircore/getmacvendors.py` & `fenrircore-0.5.0/fenrircore/getmacvendors.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.4.0/fenrircore/scanner.py` & `fenrircore-0.5.0/fenrircore/scanner.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.4.0/fenrircore/vpn.py` & `fenrircore-0.5.0/fenrircore/vpn.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.4.0/setup.py` & `fenrircore-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 This is done via ARP Spoofing. Determined default GW on inputinterface is spoofed to configured device.
     """,
     authors=['Hannes Hofer <Hannes.Hofer@gmail.com>'],
     packages=['fenrircore'],
     include_package_data=True,
     zip_safe=False,
     install_requires=['cryptography', 'pyroute2', 'python_iptables', 'requests', 'scapy'],
-    entry_points={'console_scripts': ['fenrir = fenrircore.fenrircore:main', ]},
+    entry_points={'console_scripts': ['fenrir = fenrircore.fenrir:main', ]},
     project_urls={
         'Source': 'https://github.com/HannesHofer/fenrir',
         'Tracker': 'https://github.com/HannesHofer/fenrir/issues'
     }
 )
```

