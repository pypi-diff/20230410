# Comparing `tmp/TerminalPrinter-2.1.0.tar.gz` & `tmp/TerminalPrinter-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TerminalPrinter-2.1.0.tar", last modified: Sun Apr  9 00:38:39 2023, max compression
+gzip compressed data, was "dist/TerminalPrinter-2.2.0.tar", last modified: Mon Apr 10 14:16:20 2023, max compression
```

## Comparing `TerminalPrinter-2.1.0.tar` & `TerminalPrinter-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/PKG-INFO
--rw-r--r--   0 hellflame   (501) staff       (20)     1077 2021-05-18 14:35:42.000000 TerminalPrinter-2.1.0/LICENSE
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/printer/
--rw-r--r--   0 hellflame   (501) staff       (20)     4265 2023-04-09 00:20:29.000000 TerminalPrinter-2.1.0/printer/run.py
--rw-r--r--   0 hellflame   (501) staff       (20)      105 2023-04-09 00:36:47.000000 TerminalPrinter-2.1.0/printer/version.py
--rw-r--r--   0 hellflame   (501) staff       (20)     6542 2023-04-07 00:00:47.000000 TerminalPrinter-2.1.0/printer/painter.py
--rw-r--r--   0 hellflame   (501) staff       (20)     2523 2023-04-07 15:03:33.000000 TerminalPrinter-2.1.0/printer/resource.py
--rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.1.0/printer/__init__.py
--rw-r--r--   0 hellflame   (501) staff       (20)      589 2023-04-09 00:27:18.000000 TerminalPrinter-2.1.0/printer/utils.py
--rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.1.0/printer/http.py
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/PKG-INFO
--rw-r--r--   0 hellflame   (501) staff       (20)      412 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/SOURCES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/entry_points.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/requires.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/top_level.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/dependency_links.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.1.0/MANIFEST.in
--rw-r--r--   0 hellflame   (501) staff       (20)     8153 2023-04-09 00:35:29.000000 TerminalPrinter-2.1.0/README.md
--rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.1.0/CHANGES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.1.0/setup.py
--rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/setup.cfg
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/PKG-INFO
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/printer/
+-rw-r--r--   0 hellflame   (501) staff       (20)     4265 2023-04-10 13:33:12.000000 TerminalPrinter-2.2.0/printer/run.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      106 2023-04-10 14:14:27.000000 TerminalPrinter-2.2.0/printer/version.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     5378 2023-04-10 14:11:54.000000 TerminalPrinter-2.2.0/printer/painter.py
+-rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.2.0/printer/__init__.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      753 2023-04-09 15:24:51.000000 TerminalPrinter-2.2.0/printer/utils.py
+-rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.2.0/printer/http.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     3466 2023-04-09 15:33:02.000000 TerminalPrinter-2.2.0/printer/font_helper.py
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/PKG-INFO
+-rw-r--r--   0 hellflame   (501) staff       (20)      407 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/SOURCES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/entry_points.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/requires.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/top_level.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/TerminalPrinter.egg-info/dependency_links.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.2.0/MANIFEST.in
+-rw-r--r--   0 hellflame   (501) staff       (20)     8528 2023-04-10 14:15:48.000000 TerminalPrinter-2.2.0/README.md
+-rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.2.0/CHANGES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.2.0/setup.py
+-rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-10 14:16:20.000000 TerminalPrinter-2.2.0/setup.cfg
```

### Comparing `TerminalPrinter-2.1.0/PKG-INFO` & `TerminalPrinter-2.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.1.0
+Version: 2.2.0
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.1.0/printer/run.py` & `TerminalPrinter-2.2.0/printer/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # coding=utf8
 
 import os
 import argparse
 
 from printer.version import __url__
-from printer.painter import MESS_FILTERS, FONT_LIST, FONT_DIR, \
-    FONT_URL, make_terminal_img, text_drawer, get_img
-from printer.resource import font_handle
+from printer.painter import MESS_FILTERS, make_terminal_img, text_drawer, get_img
+from printer.font_helper import font_init, choose_font
 from printer.utils import print_version, print_debug
 
 __all__ = ['parser']
 
 
 def command(args, parse):
     if args.debug:
         print_debug(args)
     if args.init:
-        font_handle(FONT_DIR, FONT_URL)
+        font_init()
     elif args.version:
         print_version()
     elif args.picture:
         pic_path = args.picture
         if os.path.exists(pic_path) and os.path.isfile(pic_path):
             print(make_terminal_img(
                 get_img(pic_path, gray=args.gray),
@@ -43,50 +42,50 @@
     parse = argparse.ArgumentParser(description="Terminal Printer",
                                     formatter_class=argparse.RawTextHelpFormatter,
                                     epilog="首次进行文字处理\r\n"
                                            "需要执行 terminalprint -i 初始化或指定字体\r\n"
                                            "更多帮助信息请参考: " + __url__)
 
     def usable_color(s):
+        _COLOR_MAP = {'black': 30, 'red': 31, 'green': 32, 'yellow': 33, 'blue': 34,
+                      'magenta': 35, 'cyan': 36, 'white': 37}
+        for k, v in _COLOR_MAP.items():
+            _COLOR_MAP['bg-' + k] = v + 10
         if s.isdigit():
             if 30 <= int(s) <= 50:
                 return int(s)
             raise argparse.ArgumentTypeError("颜色值若为数字，应在30～50之间")
         else:
-            return s
+            return _COLOR_MAP.get(s, s)
 
     def usable_filter(s):
         if s.isdigit() and 1 <= int(s) <= len(MESS_FILTERS) - 1:
             return int(s)
         raise argparse.ArgumentTypeError("填充方式索引值应在1～{}之间".format(len(MESS_FILTERS) - 1))
 
     def usable_font(s):
-        if s.isdigit():
-            if 0 <= int(s) <= len(FONT_LIST) - 1:
-                return int(s)
-            raise argparse.ArgumentTypeError("字体若为数字，应在0～{}之间".format(len(FONT_LIST) - 1))
-        else:
-            if os.path.exists(s):
-                return s
+        f, exist = choose_font(s)
+        if not exist:
             raise argparse.ArgumentTypeError("字体路径不存在，请检查路径或使用数字")
+        return f
 
     basic = parse.add_argument_group("basics")
     basic.add_argument("-i", "--init", action="store_true", help="初始化程序，下载字体")
     basic.add_argument("-v", '--version', action="store_true", help="输出版本信息")
     basic.add_argument("--debug", action="store_true", help="输出调试信息")
 
     picture = parse.add_argument_group("pictures")
     picture.add_argument("picture", nargs="?", help="可选的图片")
     picture.add_argument("-kr", '--keep-ratio', action="store_true", help="保持图片比例")
 
     text = parse.add_argument_group("text")
     text.add_argument("-t", '--text', default="HellFlame", help="设置将要处理的文本内容，默认为 HellFlame")
     text.add_argument("-c", '--color', type=usable_color, metavar="i", help="设置颜色")
     text.add_argument("-g", '--gray', action="store_true", help="图像转换为灰度图(若指定图)")
-    text.add_argument("-F", '--font', metavar="path", type=usable_font, help="设置书写字体")
+    text.add_argument("-F", '--font', metavar="path", type=usable_font, default='0', help="设置书写字体")
     text.add_argument("-r", '--reverse', action="store_true", help="反色(对彩色输出无效)")
 
     common = parse.add_argument_group("common")
     common.add_argument('-W', "--width", metavar="w", type=int, help="设置输出宽度，需要与高度一起设置")
     common.add_argument('-H', "--height", metavar="h", type=int, help="设置输出高度，需要与宽度一起设置")
     common.add_argument("-f", '--filter', type=usable_filter, metavar="i", default=73, help="设置打印填充方式")
```

### Comparing `TerminalPrinter-2.1.0/printer/painter.py` & `TerminalPrinter-2.2.0/printer/painter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,17 @@
 # coding=utf8
 import sys
 import random
 import subprocess
-from os import popen, path
+from os import popen
 
-from PIL import Image, ImageFont, ImageDraw
+from PIL import Image, ImageDraw
 
+from printer.font_helper import initiate_true_type
 
-FONT_LIST = ['shuyan.ttf',
-             'letter.ttf',
-             'Haibaoyuanyuan.ttf',
-             'fengyun.ttf',
-             'huakangbold.otf']
-
-_font_prefix = "https://raw.githubusercontent.com/hellflame/terminal_printer/" \
-               "808004a7cd41b4383bfe6aa310c491c69d9b2556/fonts/"
-
-FONT_URL = {
-    f: _font_prefix + f for f in FONT_LIST
-}
-
-FONT_DIR = path.join(path.expanduser('~'), ".terminal_fonts")
 DEFAULT_SIZE = 50, 30  # width, height
 _SIZE_CMD = "stty size"
 
 if sys.version_info.major == 2:
     reload(sys)
     sys.setdefaultencoding('utf8')
     MESS_FILTERS = ''.join([unichr(i) for i in range(32, 256)])
@@ -70,18 +57,15 @@
     :param strip_white: 是否删除(文字打印)模式下的空白行
     :return: 图像字符
     """
     if not img:
         # 如果文字画布生成失败，img为空
         return ''
     if not keep_ratio:
-        if width is None or height is None:
-            img = img.resize(DEFAULT_SIZE)
-        else:
-            img = img.resize((width, height))
+        img = img.resize((width or DEFAULT_SIZE[0], height or DEFAULT_SIZE[1]))
     else:
         size = img.size
         if width is None or height is None:
             ratio = min(float(DEFAULT_SIZE[0]) / size[0], float(DEFAULT_SIZE[1]) / size[1])
             img = img.resize((int(size[0] * ratio), int(size[1] * ratio)))
         else:
             ratio = min(float(width) / size[0], float(height) / size[1])
@@ -124,30 +108,31 @@
     else:
         def render_pix(x, y):
             # 如果这里也用和灰度图一样的处理方法的话，会显得很乱，终端中的颜色也难以显示出来
             return '\033[0;38;2;%s;%s;%sm' % pix[x, y][:3] + MESS_FILTERS[filter_type]
 
     if type(dye) is int:
         # 特定颜色绘制
-        result = '\033[01;{}m'.format(dye) + '\n'.join([''.join([render_pix(w, h) for w in range(width)])
-                                                        for h in range(height)])
+        result = '\033[01;{}m'.format(dye) + \
+                 '\n'.join([''.join([render_pix(w, h) for w in range(width)])
+                            for h in range(height)]) + '\033[00m'
     elif type(dye) is str:
         # 随机颜色绘制
         result = '\n'.join([''.join(["\033[01;{}m{}".format(random.randrange(30, 40),
                                                             render_pix(w, h))
                                      for w in range(width)])
-                            for h in range(height)])
+                            for h in range(height)]) + '\033[00m'
 
     else:
         # 黑白
         result = '\n'.join([''.join([render_pix(w, h)
                                      for w in range(width)])
                             for h in range(height)])
     img.close()
-    return result + '\033[00m'
+    return result
 
 
 def get_img(file_path, gray=False):
     """
     获取输入图片
     :param file_path: 图片文件位置
     :param gray: 是否转换为灰度图
@@ -168,38 +153,17 @@
     将文字书写在白色画布上
     :param text: 要书写的文字
     :param fonts: 字体选择，索引或路径
     :return: img
     """
     im = Image.new("1", (1, 1), 'white')  # 初始画布大小没有关系
     draw = ImageDraw.Draw(im)
-    if type(fonts) is int:
-        font = path.join(FONT_DIR, FONT_LIST[fonts if len(FONT_LIST) - 1 >= fonts >= 0 else 0])
-        # print(font)
-    elif fonts is None:
-        font = path.join(FONT_DIR, FONT_LIST[0])
-    else:
-        font = fonts
-
-    if not path.exists(font) and path.isfile(font):
-        print("字体文件不存在({})，请使用其他字体".format(font))
-        return None
-    try:
-        font = ImageFont.truetype(font, 20)
-    except IOError:
-        print("字体文件损坏，请使用其他字体")
+    font = initiate_true_type(fonts, 20)
+    if not font:
         return None
-    except:
-        target = path.join(FONT_DIR, FONT_LIST[0])
-        if path.exists(target):
-            font = ImageFont.truetype(target, 20)
-        else:
-            print("字体缺失，请初始化字体!")
-            return None
-
     text_size = draw.textsize(unicode(text), font=font)
     im = im.resize(text_size)
 
     draw = ImageDraw.Draw(im)
     draw.text((0, 0), unicode(text), font=font)
     return im
```

### Comparing `TerminalPrinter-2.1.0/printer/resource.py` & `TerminalPrinter-2.2.0/printer/font_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,62 @@
 # coding=utf8
 
 import os
 import sys
 import time
 import shutil
+from os import path
+
+from PIL import ImageFont
 
 from printer.http import HTTPCons, SockFeed, unit_change
 
 if sys.version_info.major == 2:
     reload(sys)
     sys.setdefaultencoding("utf8")
 
-__all__ = ['font_downloader', 'font_handle']
+# __all__ = ['font_downloader', 'font_handle']
+
+FONT_LIST = ['shuyan.ttf',
+             'letter.ttf',
+             'Haibaoyuanyuan.ttf',
+             'fengyun.ttf',
+             'huakangbold.otf']
+
+_font_prefix = "https://raw.githubusercontent.com/hellflame/terminal_printer/" \
+               "808004a7cd41b4383bfe6aa310c491c69d9b2556/fonts/"
+
+FONT_URL = {
+    f: _font_prefix + f for f in FONT_LIST
+}
+
+FONT_DIR = path.join(path.expanduser('~'), ".terminal_fonts")
+
+
+def choose_font(choice):
+    if choice.isdigit():
+        choice = int(choice)
+        font = path.join(FONT_DIR, FONT_LIST[choice if len(FONT_LIST) - 1 >= choice >= 0 else 0])
+    else:
+        font = choice
+    if not path.exists(font) and path.isfile(font):
+        return font, False
+    return font, True
+
+
+def initiate_true_type(choice, size=20):
+    font_path, exist = choose_font(choice)
+    if not exist:
+        print("字体文件不存在({})，请使用其他字体".format(font_path))
+        return None
+    try:
+        return ImageFont.truetype(font_path, size)
+    except IOError:
+        print("字体文件损坏({})，请使用其他字体".format(font_path))
+        return None
 
 
 def font_downloader(font_link, font_dir):
     """
     字体下载
     :param font_link: 字体名称
     :param font_dir: 字体保存路径
@@ -35,49 +76,41 @@
               .format(font_name,
                       unit_change(size / (end - start))))
     else:
         print("\033[01;31m{}\033[00m 下载失败".format(font_name))
     return True
 
 
-def font_handle(font_dir, fonts_url, show_prompt=True):
+def font_init(show_prompt=True):
     """
     字体下载管理，如果没有缺失字体依然执行，将提示重新下载所有字体
-    :param font_dir: 字体路径
-    :param fonts_url: 字体链接
     :param show_prompt: 显示提示信息
     :return:
     """
-    target = [fonts_url[f] for f in fonts_url if not os.path.exists(os.path.join(font_dir, f))]
+    target = [FONT_URL[f] for f in FONT_URL if not os.path.exists(os.path.join(FONT_DIR, f))]
     if not target:
         # 如果字体完整依然执行初始化，则提示删除原有字体目录
         if show_prompt:
             # 如果不显示提示信息，则直接删除
             prompt = "当前字体数据完整，是否删除后继续初始化? y/n "
             try:
                 if sys.version_info.major == 2:
                     if not raw_input(prompt).lower().startswith('y'):
                         return False
                 else:
                     if not input(prompt).lower().startswith('y'):
                         return False
             except KeyboardInterrupt:
                 exit(0)
-        shutil.rmtree(font_dir)
-        target = fonts_url.values()
+        shutil.rmtree(FONT_DIR)
+        target = FONT_URL.values()
 
-    if not os.path.exists(font_dir):
+    if not os.path.exists(FONT_DIR):
         # 创建字体目录
-        os.makedirs(font_dir)
+        os.makedirs(FONT_DIR)
 
     print("Start Downloading {} fonts".format(len(target)))
     for font in target:
-        font_downloader(font, font_dir)
+        font_downloader(font, FONT_DIR)
 
     print("下载完成")
 
-
-if __name__ == '__main__':
-    from printer import painter
-    font_handle(painter.FONT_DIR, painter.FONT_URL, show_prompt=False)
-
-
```

### Comparing `TerminalPrinter-2.1.0/printer/utils.py` & `TerminalPrinter-2.2.0/printer/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import os
 import platform
 
 from printer.version import __version__
 from printer.painter import DEFAULT_SIZE
+from printer.font_helper import choose_font
 
 
 def print_version():
     print("TerminalPrinter v{}".format(__version__))
 
 
 def print_debug(args):
     print_version()
     print("Shell: {}".format(os.getenv("SHELL")))
     print("Term: {}".format(os.getenv("TERM")))
     print("Platform: {}".format("/".join(platform.uname())))
     print("Given Size: {}/{} Default Size: {}/{}".format(args.width, args.height, *DEFAULT_SIZE))
     print("Arguments: {}".format(" ".join(["{}:{}".format(k, v) for k, v in args.__dict__.items()])))
-
+    if args.text:
+        font, exist = choose_font(args.font)
+        print("Font: {} (exist? {})".format(font, exist))
```

### Comparing `TerminalPrinter-2.1.0/printer/http.py` & `TerminalPrinter-2.2.0/printer/http.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.1.0/TerminalPrinter.egg-info/PKG-INFO` & `TerminalPrinter-2.2.0/TerminalPrinter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.1.0
+Version: 2.2.0
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.1.0/README.md` & `TerminalPrinter-2.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 $ terminalprint -v # terminalprint --version
 ```
 
 #### iii. 初始化字体库
 
 > 选择的字体都是可以支持大部分中文的字体，这5个字体是大多数系统没有安装的第三方字体，所以把这5个字体放在了用户目录下的一个隐藏文件目录，`~/.terminal_fonts/` ，5个字体的下载路径分别为：(可以手动下载保存在指定路径)
 
-由于GFW和域名审核等问题，现在将字体资源放在 [fonts](./fonts)
+现在字体资源放在 [fonts](./fonts) ，也可点击 [下载完整字体包](./images/fonts.tar.gz)，解压将5个字体文件放到 `~/.terminal_fonts/` 即可
 
 当然，可以直接通过以下命令初始化字体库:
 
 ```bash
 $ terminalprint -i # terminalprint --init
 ```
 
@@ -118,15 +118,19 @@
 
 ```bash
 $ terminalprint -c [color]
 ```
 
 color值范围30～50，覆盖终端基本的16色
 
-也可以使用随机颜色，只要颜色值是一个非数字字符串即可
+可以使用部分颜色名称如：`red`, `black`, `green`, `yellow`, `blue`, `magenta`, `cyan`, `white`
+
+在上述颜色名称添加前缀 `bg-` 即可设置为对应背景色，如可设置背景蓝色：`bg-blue`
+
+也可以使用随机颜色，只要颜色值是一个非颜色名称的字符串即可
 
 ```bash
 $ terminalprint -c auto
 ```
 
 ![random](./images/sample-4.png)
 
@@ -250,10 +254,15 @@
 
   易用性更新
 
 - v2.1.0
 
   新增调试入口
 
+- v2.2.0
+
+  新增颜色名称支持
+
+  输出长宽更自由
 ------
 
 嗯，以上，Just For Fun!
```

### Comparing `TerminalPrinter-2.1.0/setup.py` & `TerminalPrinter-2.2.0/setup.py`

 * *Files identical despite different names*

