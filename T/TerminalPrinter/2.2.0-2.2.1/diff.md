# Comparing `tmp/TerminalPrinter-2.2.0.tar.gz` & `tmp/TerminalPrinter-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TerminalPrinter-2.2.0.tar", last modified: Mon Apr 10 14:16:20 2023, max compression
+gzip compressed data, was "dist/TerminalPrinter-2.2.1.tar", last modified: Mon Apr 10 14:52:31 2023, max compression
```

## Comparing `TerminalPrinter-2.2.0.tar` & `TerminalPrinter-2.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/PKG-INFO
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/printer/
--rw-r--r--   0 hellflame   (501) staff       (20)     4265 2023-04-10 13:33:12.000000 TerminalPrinter-2.2.0/printer/run.py
--rw-r--r--   0 hellflame   (501) staff       (20)      106 2023-04-10 14:14:27.000000 TerminalPrinter-2.2.0/printer/version.py
--rw-r--r--   0 hellflame   (501) staff       (20)     5378 2023-04-10 14:11:54.000000 TerminalPrinter-2.2.0/printer/painter.py
--rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.2.0/printer/__init__.py
--rw-r--r--   0 hellflame   (501) staff       (20)      753 2023-04-09 15:24:51.000000 TerminalPrinter-2.2.0/printer/utils.py
--rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.2.0/printer/http.py
--rw-r--r--   0 hellflame   (501) staff       (20)     3466 2023-04-09 15:33:02.000000 TerminalPrinter-2.2.0/printer/font_helper.py
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/PKG-INFO
--rw-r--r--   0 hellflame   (501) staff       (20)      407 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/SOURCES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/entry_points.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/requires.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/top_level.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/dependency_links.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.2.0/MANIFEST.in
--rw-r--r--   0 hellflame   (501) staff       (20)     8528 2023-04-10 14:15:48.000000 TerminalPrinter-2.2.0/README.md
--rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.2.0/CHANGES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.2.0/setup.py
--rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/setup.cfg
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/PKG-INFO
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/printer/
+-rw-r--r--   0 hellflame   (501) staff       (20)     4280 2023-04-10 14:48:28.000000 TerminalPrinter-2.2.1/printer/run.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      106 2023-04-10 14:51:28.000000 TerminalPrinter-2.2.1/printer/version.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     5378 2023-04-10 14:11:54.000000 TerminalPrinter-2.2.1/printer/painter.py
+-rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.2.1/printer/__init__.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      753 2023-04-09 15:24:51.000000 TerminalPrinter-2.2.1/printer/utils.py
+-rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.2.1/printer/http.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     3466 2023-04-09 15:33:02.000000 TerminalPrinter-2.2.1/printer/font_helper.py
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/PKG-INFO
+-rw-r--r--   0 hellflame   (501) staff       (20)      407 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/SOURCES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/entry_points.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/requires.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/top_level.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/dependency_links.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.2.1/MANIFEST.in
+-rw-r--r--   0 hellflame   (501) staff       (20)     8643 2023-04-10 14:45:40.000000 TerminalPrinter-2.2.1/README.md
+-rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.2.1/CHANGES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.2.1/setup.py
+-rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/setup.cfg
```

### Comparing `TerminalPrinter-2.2.0/PKG-INFO` & `TerminalPrinter-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.2.0
+Version: 2.2.1
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.2.0/printer/run.py` & `TerminalPrinter-2.2.1/printer/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
                                     epilog="首次进行文字处理\r\n"
                                            "需要执行 terminalprint -i 初始化或指定字体\r\n"
                                            "更多帮助信息请参考: " + __url__)
 
     def usable_color(s):
         _COLOR_MAP = {'black': 30, 'red': 31, 'green': 32, 'yellow': 33, 'blue': 34,
                       'magenta': 35, 'cyan': 36, 'white': 37}
-        for k, v in _COLOR_MAP.items():
-            _COLOR_MAP['bg-' + k] = v + 10
+        for k in tuple(_COLOR_MAP.keys()):
+            _COLOR_MAP['bg-' + k] = _COLOR_MAP[k] + 10
         if s.isdigit():
             if 30 <= int(s) <= 50:
                 return int(s)
             raise argparse.ArgumentTypeError("颜色值若为数字，应在30～50之间")
         else:
             return _COLOR_MAP.get(s, s)
```

### Comparing `TerminalPrinter-2.2.0/printer/painter.py` & `TerminalPrinter-2.2.1/printer/painter.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.2.0/printer/utils.py` & `TerminalPrinter-2.2.1/printer/utils.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.2.0/printer/http.py` & `TerminalPrinter-2.2.1/printer/http.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.2.0/printer/font_helper.py` & `TerminalPrinter-2.2.1/printer/font_helper.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.2.0/TerminalPrinter.egg-info/PKG-INFO` & `TerminalPrinter-2.2.1/TerminalPrinter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.2.0
+Version: 2.2.1
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.2.0/README.md` & `TerminalPrinter-2.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,18 @@
 # terminalprint [pic] -g -c 34 -f 4
 ```
 
 ![](./images/sample-3.png)
 
 这里的填充字符索引会多义为使用不超过ANSI中可打印字符码值不超过4的字符来表示不同的灰度级别，索引值越大，灰度的符号越多，看上去也会更杂乱。实际上，如果将索引调到最大的话，还是依稀可以看到原图的影子的，不过实际效果嘛，，，灰阶较少的图片也没有问题。
 
+> windows cmd 虽然支持不多，但也基本能用，但颜色等特性无法使用
+
+![](./images/windows.png)
+
 ### 版本日志
 
 好吧，`v1.3.0` 之前的版本都是在几年前写的，当时也没有想过要记录什么的问题，所以版本日志从 `v1.3.3` 开始
 
 - v1.3.0 ～ v1.3.2
 
 从1.3.0开始，代码开始写的认真一点了，曾经的代码到现在看来真的完全不能入目的感觉=。=完全不知道在想什么，虽然也不确定现在重写之后会不会被更久之后吐槽。
```

### Comparing `TerminalPrinter-2.2.0/setup.py` & `TerminalPrinter-2.2.1/setup.py`

 * *Files identical despite different names*

