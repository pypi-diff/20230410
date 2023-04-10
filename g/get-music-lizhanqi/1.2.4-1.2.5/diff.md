# Comparing `tmp/get-music-lizhanqi-1.2.4.tar.gz` & `tmp/get-music-lizhanqi-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\???\Desktop\get_music\dist\.tmp-uq2o1w9i\get-music-lizhanqi-1.2.4.tar", last modified: Mon Jan 16 12:35:18 2023, max compression
+gzip compressed data, was "C:\Users\???\Desktop\get_music\dist\.tmp-0ydxs70x\get-music-lizhanqi-1.2.5.tar", last modified: Mon Apr 10 09:52:40 2023, max compression
```

## Comparing `get-music-lizhanqi-1.2.4.tar` & `get-music-lizhanqi-1.2.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/
--rw-rw-rw-   0        0        0     1091 2022-04-09 10:07:52.000000 get-music-lizhanqi-1.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1767 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1353 2023-01-16 12:34:53.000000 get-music-lizhanqi-1.2.4/README.md
--rw-rw-rw-   0        0        0       86 2022-04-09 10:04:03.000000 get-music-lizhanqi-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      952 2023-01-16 12:32:14.000000 get-music-lizhanqi-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/tests/
-drwxrwxrwx   0        0        0        0 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/tests/get_music/
--rw-rw-rw-   0        0        0      757 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/__init__.py
--rw-rw-rw-   0        0        0     3092 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/baidu.py
--rw-rw-rw-   0        0        0     1938 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/download.py
--rw-rw-rw-   0        0        0     2892 2023-01-16 12:15:24.000000 get-music-lizhanqi-1.2.4/tests/get_music/downloads.py
--rw-rw-rw-   0        0        0     3222 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/fivesing.py
--rw-rw-rw-   0        0        0    10140 2023-01-16 12:29:42.000000 get-music-lizhanqi-1.2.4/tests/get_music/get_music.py
--rw-rw-rw-   0        0        0    11725 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/gui.py
--rw-rw-rw-   0        0        0     2391 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/kg_playerlist.py
--rw-rw-rw-   0        0        0     5305 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/kugou.py
--rw-rw-rw-   0        0        0     3985 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/kuwo.py
--rw-rw-rw-   0        0        0     2655 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/kw_playerlist.py
--rw-rw-rw-   0        0        0     2861 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/migu.py
--rw-rw-rw-   0        0        0     3763 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/netease.py
--rw-rw-rw-   0        0        0     2090 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/oneting.py
--rw-rw-rw-   0        0        0     3304 2023-01-16 12:19:05.000000 get-music-lizhanqi-1.2.4/tests/get_music/playerlist.py
--rw-rw-rw-   0        0        0     4293 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/qq.py
--rw-rw-rw-   0        0        0     2504 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/qq_playerlist.py
--rw-rw-rw-   0        0        0     2562 2023-01-16 12:04:51.000000 get-music-lizhanqi-1.2.4/tests/get_music/singbz.py
--rw-rw-rw-   0        0        0     6826 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/top.py
--rw-rw-rw-   0        0        0     1702 2023-01-16 12:31:58.000000 get-music-lizhanqi-1.2.4/tests/get_music/ver.py
--rw-rw-rw-   0        0        0     3089 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/wy_playerlist.py
--rw-rw-rw-   0        0        0     3692 2023-01-14 10:18:32.000000 get-music-lizhanqi-1.2.4/tests/get_music/zhidao.py
-drwxrwxrwx   0        0        0        0 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/tests/get_music_lizhanqi.egg-info/
--rw-rw-rw-   0        0        0     1767 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/tests/get_music_lizhanqi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/tests/get_music_lizhanqi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/tests/get_music_lizhanqi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/tests/get_music_lizhanqi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/tests/get_music_lizhanqi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-16 12:35:18.000000 get-music-lizhanqi-1.2.4/tests/get_music_lizhanqi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/
+-rw-rw-rw-   0        0        0     1091 2022-04-09 10:07:52.000000 get-music-lizhanqi-1.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1869 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1455 2023-04-10 09:51:35.000000 get-music-lizhanqi-1.2.5/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-09 10:04:03.000000 get-music-lizhanqi-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      952 2023-04-10 09:43:27.000000 get-music-lizhanqi-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/
+drwxrwxrwx   0        0        0        0 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/tests/get_music/
+-rw-rw-rw-   0        0        0      266 2023-04-09 14:18:18.000000 get-music-lizhanqi-1.2.5/tests/get_music/__init__.py
+-rw-rw-rw-   0        0        0     3092 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/baidu.py
+-rw-rw-rw-   0        0        0     1938 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/download.py
+-rw-rw-rw-   0        0        0     2892 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/downloads.py
+-rw-rw-rw-   0        0        0     3222 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/fivesing.py
+-rw-rw-rw-   0        0        0    10379 2023-04-10 09:41:28.000000 get-music-lizhanqi-1.2.5/tests/get_music/get_music.py
+-rw-rw-rw-   0        0        0    11725 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/gui.py
+-rw-rw-rw-   0        0        0     2613 2023-04-10 09:28:35.000000 get-music-lizhanqi-1.2.5/tests/get_music/kg_one_playerlist.py
+-rw-rw-rw-   0        0        0     2570 2023-04-10 09:22:32.000000 get-music-lizhanqi-1.2.5/tests/get_music/kg_playerlist.py
+-rw-rw-rw-   0        0        0     5305 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/kugou.py
+-rw-rw-rw-   0        0        0     3985 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/kuwo.py
+-rw-rw-rw-   0        0        0     2685 2023-04-10 09:47:01.000000 get-music-lizhanqi-1.2.5/tests/get_music/kw_playerlist.py
+-rw-rw-rw-   0        0        0     2861 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/migu.py
+-rw-rw-rw-   0        0        0     3763 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/netease.py
+-rw-rw-rw-   0        0        0     2090 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/oneting.py
+-rw-rw-rw-   0        0        0     3306 2023-04-10 09:21:26.000000 get-music-lizhanqi-1.2.5/tests/get_music/playerlist.py
+-rw-rw-rw-   0        0        0     4293 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/qq.py
+-rw-rw-rw-   0        0        0     2534 2023-04-10 09:46:23.000000 get-music-lizhanqi-1.2.5/tests/get_music/qq_playerlist.py
+-rw-rw-rw-   0        0        0     2562 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/singbz.py
+-rw-rw-rw-   0        0        0     6826 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/top.py
+-rw-rw-rw-   0        0        0     2100 2023-04-09 14:37:17.000000 get-music-lizhanqi-1.2.5/tests/get_music/ver.py
+-rw-rw-rw-   0        0        0     3119 2023-04-10 09:46:07.000000 get-music-lizhanqi-1.2.5/tests/get_music/wy_playerlist.py
+-rw-rw-rw-   0        0        0     3692 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/zhidao.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/
+-rw-rw-rw-   0        0        0     1869 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/top_level.txt
```

### Comparing `get-music-lizhanqi-1.2.4/LICENSE.txt` & `get-music-lizhanqi-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/PKG-INFO` & `get-music-lizhanqi-1.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-music-lizhanqi
-Version: 1.2.4
+Version: 1.2.5
 Summary: 可以下载音乐的包哦
 Home-page: 
 Author: Li Zhan Qi
 Author-email: 3101978435@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,19 +16,15 @@
 - 这是一个可以下载和搜索音乐的python命令行工具，支持，酷狗，酷我，百度，网易云，咪咕，qq音乐，5sing，欢迎前来学习的指点
 
 ## 使用方法
 - 长话短说**get-music -help**或**get-music-lizhanqi -help**打开帮助，帮助里面有全部命令的介绍，或者前往github地址:<https://github.com/lzq-hopego/get-music-lizhanqi>
 
 
 ## 更新记录
-- 2023-1-16 完成v1.2.4版本,支持搜索5sing的伴奏数据
-> 可以搭配"get-music -r"进行批量搜索，第三个参数是bz代表着5sing伴奏
-```
-爱人错过,1,bz
-```
+- 2023-04-10 完成v1.2.5版本,支持手机kugou的歌单链接进行获取歌单中的信息,优化导入模块时会打印的logo导致pyinstaller -w参数打包时会失败的问题，由此取消导入模块时打印logo,只有在命令行执行命令时会打印logo,优化细节
 
 
 
 
 ## THE END
 - 本脚本仅支持学习使用，如有发现有任何商业用途，一经发现您将受到法律责任。
 - 本程序使用的接口全部来源于网络，切不可有任何商业用途，或我程序中有涉及你公司利益的，你可以联系我，我会及时删除源代码，并不再更新。
```

### Comparing `get-music-lizhanqi-1.2.4/README.md` & `get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,35 @@
+Metadata-Version: 2.1
+Name: get-music-lizhanqi
+Version: 1.2.5
+Summary: 可以下载音乐的包哦
+Home-page: 
+Author: Li Zhan Qi
+Author-email: 3101978435@qq.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # get-music-lizhanqi
 - 这是一个可以下载和搜索音乐的python命令行工具，支持，酷狗，酷我，百度，网易云，咪咕，qq音乐，5sing，欢迎前来学习的指点
 
 ## 使用方法
 - 长话短说**get-music -help**或**get-music-lizhanqi -help**打开帮助，帮助里面有全部命令的介绍，或者前往github地址:<https://github.com/lzq-hopego/get-music-lizhanqi>
 
 
 ## 更新记录
-- 2023-1-16 完成v1.2.4版本,支持搜索5sing的伴奏数据
-> 可以搭配"get-music -r"进行批量搜索，第三个参数是bz代表着5sing伴奏
-```
-爱人错过,1,bz
-```
+- 2023-04-10 完成v1.2.5版本,支持手机kugou的歌单链接进行获取歌单中的信息,优化导入模块时会打印的logo导致pyinstaller -w参数打包时会失败的问题，由此取消导入模块时打印logo,只有在命令行执行命令时会打印logo,优化细节
 
 
 
 
 ## THE END
 - 本脚本仅支持学习使用，如有发现有任何商业用途，一经发现您将受到法律责任。
 - 本程序使用的接口全部来源于网络，切不可有任何商业用途，或我程序中有涉及你公司利益的，你可以联系我，我会及时删除源代码，并不再更新。
 - **禁止将本工具用于商业用途**，如产生法律纠纷与本人无关，如有侵权，请联系我删除。
 - 如果你对界面设计感兴趣可以去看我的另一篇pyqt5对接的get-music-lizhanqi做的音乐下载播放ui，地址：https://github.com/lzq-hopego/get-music-lizhanqi-gui
 - 项目创建者：李先生
 - 项目维护者：李先生
-- 维护者邮箱：3101978435@qq.com
+- 维护者邮箱：3101978435@qq.com
```

### Comparing `get-music-lizhanqi-1.2.4/setup.py` & `get-music-lizhanqi-1.2.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="get-music-lizhanqi",
-    version="1.2.4",
+    version="1.2.5",
     author="Li Zhan Qi",
     author_email="3101978435@qq.com",
     description="可以下载音乐的包哦",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/baidu.py` & `get-music-lizhanqi-1.2.5/tests/get_music/baidu.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/download.py` & `get-music-lizhanqi-1.2.5/tests/get_music/download.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/downloads.py` & `get-music-lizhanqi-1.2.5/tests/get_music/downloads.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/fivesing.py` & `get-music-lizhanqi-1.2.5/tests/get_music/fivesing.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/get_music.py` & `get-music-lizhanqi-1.2.5/tests/get_music/get_music.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,26 @@
 from get_music import singbz
 from get_music import download
 from rich.console import Console
 from rich.table import Table
 import sys
 
 console = Console()
+txt='''
+                __                                  __        
+   ____   _____/  |_            _____  __ __  _____|__| ____  
+  / ___\_/ __ \   __\  ______  /     \|  |  \/  ___/  |/ ___\ 
+ / /_/  >  ___/|  |   /_____/ |  Y Y  \  |  /\___ \|  \  \___ 
+ \___  / \___  >__|           |__|_|  /____//____  >__|\___  >
+/_____/      \/                     \/           \/        \/
+
+'''
+console=Console()
+console.print(txt,style='bold green')
+
 def zhuti(songname = '',p = False,l = False):
     d={1:kugou.kugou(p,l),
        2:netease.netease(p,l),
        3:qq.qq(p,l),
        4:kuwo.kuwo(p,l),
        5:migu.migu(p,l),
        6:baidu.baidu(p,l),
@@ -48,15 +60,15 @@
 
 
 def main_help():    
     txt='''
     关于本脚本的使用：\n
     \t\t1.1,“[b red]get-music -v[/]”查看当前版本，同时程序也会检查一下新版本的版本号是否更新看您个人\n
     \t\t1.2,“[b red]get-music -l[/]”下载歌曲的同时也下载歌曲的歌词，直接敲就行了后面的搜索步骤和“get-music”的操作基本一致\n
-    \t\t1.3,“[b red]get-music -p[/]”下载歌曲的同时也下载歌曲的封面，这九个接口中只有“1ting”不支持下载歌词，其他的功能都能正常使用\n
+    \t\t1.3,“[b red]get-music -p[/]”下载歌曲的同时也下载歌曲的封面，这十个接口中只有“1ting”不支持下载歌词，其他的功能都能正常使用\n
     \t\t1.4,“[b red]get-music -lp[/]”或者“get-music -pl”它俩都是同一个意思，下载歌曲的同时也下载封面和歌词\n
     \t\t1.5,“[b red]get-music -t[/]”打开本脚本的GUI界面，相比命令行对小白更友好\n
     \t\t1.6，“[b red]get-music -help[/]”查看帮助文档\n
     \t\t1.7，“[b red]get-music -hot[/]”查看热歌榜单\n
     \t\t1.8，“[b red]get-music -r[/]”批量下载\n
     \t\t1.9，“[b red]get-music -s[/]”在网络中查找歌曲的网盘链接\n
     \t\t1.10, “[b red]get-music -playerlist[/]”下载歌单中的歌曲,只支持,酷狗,网易云,QQ,酷我,四个平台\n
@@ -107,18 +119,15 @@
                     except:
                         console.print('[b red]接口无反应您可重试！')
                 elif sys.argv[1] == '-playerlist':
                     try:
                         from get_music.playerlist import player_list
                         player_list(sys.argv[2:])
                     except:
-                        console.print('[b red]注意使用规范！')
-                        from get_music.playerlist import y_help
-                        y_help()
-                        console.print('[b red]出现错误！请联系维护者！')
+                        sys.exit()
                 elif sys.argv[1] in ['-t','-T']:
                     try:
                         from get_music import gui
                     except:
                         console.print('[b red]您的设备暂不支持该命令！')
                 elif sys.argv[1] in ['-s','-S']:
                     try:
```

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/gui.py` & `get-music-lizhanqi-1.2.5/tests/get_music/gui.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/kg_playerlist.py` & `get-music-lizhanqi-1.2.5/tests/get_music/kg_playerlist.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-import requests,re
+import requests,re,sys
 from get_music.kugou import kugou
 from get_music.download import download
 import ast
+from get_music import kg_one_playerlist
 
 def kg_playerlist(url,pic=False,lrc=False):
     kg=kugou()
     headers={'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36 Edg/108.0.1462.54'
              }
 
     page_url='https://t1.kugou.com/'
+    if 'm.kugou.com' in url:
+        kg_one_playerlist.kg_one_playerlist(url=url)
+        sys.exit()
     if ('t1.kugou.com' in url) or ('wwwapi.kugou.com' in url):
         page_url=url
     else:
         page_url+=url
     
     s=requests.session()
 
@@ -36,17 +40,17 @@
     for i in range(len(hashlist)):
         print("序号:{}\t{}\t{}\t".format(i+1,song_name[i],singer[i]))
     songs=input('请选择您要下载哪一首歌，直接输入序号就行\n如需下载多个不连续的请用英文逗号分割即可，例如1,2\n如需下载多个连续的请用-分割即可，例如1-3\n如需全部下载，请输入all\n如果不需要下载多个，请直接输入序号就行:')
     if songs=='':
         print('\n\n\n——您未做出选择！程序即将自动退出！！！')
         return
     if songs=='all':
-        song_list=range(len(song_name))
+        song_list=[x+1 for x in range(len(song_name))]
     elif '-' in songs:
-        song_list=range(int(songs.split('-')[0]),int(songs.split('-')[-1])+1)
+        song_list=[x+1 for x in range(int(songs.split('-')[0]),int(songs.split('-')[-1])+1)]
     else:
         song_list=songs.split(",")
         if len(song_list)==1:
             song_list=songs.split("，")
 
     for i in song_list:
         i=int(i)-1
```

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/kugou.py` & `get-music-lizhanqi-1.2.5/tests/get_music/kugou.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/kuwo.py` & `get-music-lizhanqi-1.2.5/tests/get_music/kuwo.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/kw_playerlist.py` & `get-music-lizhanqi-1.2.5/tests/get_music/kw_playerlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
 
     songs=input('请选择您要下载哪一首歌，直接输入序号就行\n如需下载多个不连续的请用英文逗号分割即可，例如1,2\n如需下载多个连续的请用-分割即可，例如1-3\n如需全部下载，请输入all\n如果不需要下载多个，请直接输入序号就行:')
     if songs=='':
         print('\n\n\n——您未做出选择！程序即将自动退出！！！')
         return
     if songs=='all':
-        song_list=range(len(song_name))
+        song_list=[x+1 for x in range(len(song_name))]
     elif '-' in songs:
-        song_list=range(int(songs.split('-')[0]),int(songs.split('-')[-1])+1)
+        song_list=[x+1 for x in range(int(songs.split('-')[0]),int(songs.split('-')[-1])+1)]
     else:
         song_list=songs.split(",")
         if len(song_list)==1:
             song_list=songs.split("，")
 
 
     for i in song_list:
```

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/migu.py` & `get-music-lizhanqi-1.2.5/tests/get_music/migu.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/netease.py` & `get-music-lizhanqi-1.2.5/tests/get_music/netease.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/oneting.py` & `get-music-lizhanqi-1.2.5/tests/get_music/oneting.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/playerlist.py` & `get-music-lizhanqi-1.2.5/tests/get_music/playerlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import getopt
 from rich.console import Console
 
 con = Console()
 def player_list(argv):
     opts=getopt.getopt(argv,"i:-l-p",["api="])[0]
-    print(opts)
+##    print(opts)
     api=''
     url=''
     lrc=False
     pic=False
     for i in opts:
         if ('-i' in i) and (i[-1] !=''):
             url=i[-1]
```

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/qq.py` & `get-music-lizhanqi-1.2.5/tests/get_music/qq.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/qq_playerlist.py` & `get-music-lizhanqi-1.2.5/tests/get_music/qq_playerlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
     for i in range(len(songid)):
             print("序号:{}\t{}\t{}".format(i+1,songs_ls[i],singer[i]))
     songs=input('请选择您要下载哪一首歌，直接输入序号就行\n如需下载多个不连续的请用英文逗号分割即可，例如1,2\n如需下载多个连续的请用-分割即可，例如1-3\n如需全部下载，请输入all\n如果不需要下载多个，请直接输入序号就行:')
     if songs=='':
         print('\n\n\n——您未做出选择！程序即将自动退出！！！')
         return
     if songs=='all':
-        song_list=range(len(song_name))
+        song_list=[x+1 for x in range(len(song_name))]
     elif '-' in songs:
-        song_list=range(int(songs.split('-')[0]),int(songs.split('-')[-1])+1)
+        song_list=[x+1 for x in range(int(songs.split('-')[0]),int(songs.split('-')[-1])+1)]
     else:
         song_list=songs.split(",")
         if len(song_list)==1:
             song_list=songs.split("，")
 
     for i in song_list:
         i=int(i)-1
```

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/singbz.py` & `get-music-lizhanqi-1.2.5/tests/get_music/singbz.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/top.py` & `get-music-lizhanqi-1.2.5/tests/get_music/top.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/ver.py` & `get-music-lizhanqi-1.2.5/tests/get_music/ver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 import requests,re
 from rich.console import Console
 def ver(ip=True):
     console=Console()
-    version = '1.2.4'
+    
+    if ip==True:
+            try:
+                txt=requests.get('http://ip.tool.lu',timeout=1).text.split()
+                ip=txt[1]
+                area=' '.join(txt[3:])
+                console.print('\n[b green]信息一:本机外网ip地址为:[b red]{}[/]，归属:[b red]{}[/]'.format(ip,area))
+
+                url = 'http://api.ip33.com/ip/search?s='                     
+                d = requests.get(url,timeout=1).json()                                                       
+                console.print('\n[b green]信息二:本机外网ip地址为:[b red]{}[/]，归属:[b red]{}[/]'.format(d['ip'],d['area']))
+                return
+            except:
+                console.print("\n[b red]ip地址查询失败！")
+                return
+    
+    version = '1.2.5'
     console.print("[green]当前版本:"+"v"+version)
     url = 'https://pypi.org/project/get-music-lizhanqi/#history'
     try:
         with console.status("[b green]检查最新版中..."):
-            html = requests.get(url,timeout = 1)
+            html = requests.get(url,timeout = 5)
             txt = html.text
             crad = re.findall(r' <a class="card release__card" href="/project/get-music-lizhanqi/(.*?)/">',txt,re.S)
             ver = crad[0]
             ver1 = version.split('.')
             ver2 = ver.split('.')
             ls= []
             for i in range(3):
@@ -23,18 +39,12 @@
                     ls.append(True)
                 else:
                     ls.append(False)
         if False in ls:
             console.print('[b red]最新版本是:v'+ver+',你可以用"pip install --upgrade get-music-lizhanqi"命令进行更新')
         else:
            console.print('[b red]最新版本是:v'+ver+',您已是最新版本')
-        if ip==True:
-            try:
-                url = 'http://api.ip33.com/ip/search?s='                     
-                d = requests.get(url,timeout=1).json()                                                       
-                console.print('\n[b green]本机外网ip地址为:[b red]{}[/]，归属:[b red]{}[/]'.format(d['ip'],d['area']))
-            except:
-                pass
+        
     except:
         console.print("[b red]获取最新版本信息失败！请检查是否是网络的问题！")
```

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/wy_playerlist.py` & `get-music-lizhanqi-1.2.5/tests/get_music/wy_playerlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         print("序号:{}\t{}".format(i+1,song_name[i]))
 
     songs=input('请选择您要下载哪一首歌，直接输入序号就行\n如需下载多个不连续的请用英文逗号分割即可，例如1,2\n如需下载多个连续的请用-分割即可，例如1-3\n如需全部下载，请输入all\n如果不需要下载多个，请直接输入序号就行:')
     if songs=='':
         print('\n\n\n——您未做出选择！程序即将自动退出！！！')
         return
     if songs=='all':
-        song_list=range(len(song_name))
+        song_list=[x+1 for x in range(len(song_name))]
     elif '-' in songs:
-        song_list=range(int(songs.split('-')[0]),int(songs.split('-')[-1])+1)
+        song_list=[x+1 for x in range(int(songs.split('-')[0]),int(songs.split('-')[-1])+1)]
     else:
         song_list=songs.split(",")
         if len(song_list)==1:
             song_list=songs.split("，")
 
     for i in song_list:
         i=int(i)-1
```

#### html2text {}

```diff
@@ -16,20 +16,20 @@
       print("å¹³å°éå¶ï¼åªè½æå°åº10é¦å¦")_for_i_in_range(len
       (urls)):_print("åºå·:{}\t{}".format(i+1,song_name[i]))_songs=input
       ('è¯·éæ©æ¨è¦ä¸è½½åªä¸é¦æ­ï¼ç´æ¥è¾å¥åºå·å°±è¡\nå¦éä¸è½½å¤ä¸ªä¸è¿ç»­çè¯·ç¨è±æéå·åå²å³å¯ï¼ä¾å¦1,2\nå¦éä¸è½½å¤ä¸ªè¿ç»­çè¯·ç¨-
       åå²å³å¯ï¼ä¾å¦1-
       3\nå¦éå¨é¨ä¸è½½ï¼è¯·è¾å¥all\nå¦æä¸éè¦ä¸è½½å¤ä¸ªï¼è¯·ç´æ¥è¾å¥åºå·å°±è¡:
       ')_if_songs=='':_print
       ('\n\n\nââæ¨æªååºéæ©ï¼ç¨åºå³å°èªå¨éåºï¼ï¼ï¼')
-      return_if_songs=='all':_song_list=range(len(song_name))_elif_'-'_in
-      songs:_song_list=range(int(songs.split('-')[0]),int(songs.split('-')[-
-      1])+1)_else:_song_list=songs.split(",")_if_len(song_list)==1:
-      song_list=songs.split("ï¼")_for_i_in_song_list:_i=int(i)-1_try:
-      html=s.get(netease_url+urls[i],timeout=1)_html.encoding='utf-8'
-      txt=html.text_song_id=urls[i].split('=')[-1]_song_url=(song_id).join
+      return_if_songs=='all':_song_list=[x+1_for_x_in_range(len(song_name))]
+      elif_'-'_in_songs:_song_list=[x+1_for_x_in_range(int(songs.split('-')
+      [0]),int(songs.split('-')[-1])+1)]_else:_song_list=songs.split(",")_if
+      len(song_list)==1:_song_list=songs.split("ï¼")_for_i_in_song_list:_i=int
+      (i)-1_try:_html=s.get(netease_url+urls[i],timeout=1)_html.encoding='utf-
+      8'_txt=html.text_song_id=urls[i].split('=')[-1]_song_url=(song_id).join
       (songs_url)_p=re.findall(r'
       (.*?)<\/p>',txt)[0]_singer=(re.findall(r'',p)[0]).replace('amp;','')
       download(song_url,song_name[i]+"-"+singer+".mp3")_if_pic:
       img_url=re.findall('[.*]',txt)[0]_download(img_url,song_name[i]+"-
       "+singer+".jpg")_if_lrc:_txt=wy.get_music_lrc(song_id)_with_open
       (song_name[i]+"-"+singer+".txt",'w')_as_f:_f.write(txt)_except:_print
       ('\n\n\nââæ æ³ä¸è½½æè§£ææ­æ²ï¼ï¼ï¼')
```

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music/zhidao.py` & `get-music-lizhanqi-1.2.5/tests/get_music/zhidao.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.4/tests/get_music_lizhanqi.egg-info/SOURCES.txt` & `get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 tests/get_music/__init__.py
 tests/get_music/baidu.py
 tests/get_music/download.py
 tests/get_music/downloads.py
 tests/get_music/fivesing.py
 tests/get_music/get_music.py
 tests/get_music/gui.py
+tests/get_music/kg_one_playerlist.py
 tests/get_music/kg_playerlist.py
 tests/get_music/kugou.py
 tests/get_music/kuwo.py
 tests/get_music/kw_playerlist.py
 tests/get_music/migu.py
 tests/get_music/netease.py
 tests/get_music/oneting.py
```

