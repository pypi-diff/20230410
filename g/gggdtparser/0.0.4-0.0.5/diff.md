# Comparing `tmp/gggdtparser-0.0.4.tar.gz` & `tmp/gggdtparser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggdtparser-0.0.4.tar", last modified: Sun Apr  2 02:58:17 2023, max compression
+gzip compressed data, was "gggdtparser-0.0.5.tar", last modified: Mon Apr 10 04:26:42 2023, max compression
```

## Comparing `gggdtparser-0.0.4.tar` & `gggdtparser-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 02:58:17.798689 gggdtparser-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2791 2023-04-02 02:58:17.798689 gggdtparser-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2076 2023-04-01 07:04:24.000000 gggdtparser-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 02:58:17.793702 gggdtparser-0.0.4/gggdtparser/
--rw-rw-rw-   0        0        0      259 2023-03-28 10:39:47.000000 gggdtparser-0.0.4/gggdtparser/__init__.py
--rw-rw-rw-   0        0        0     8667 2023-04-02 02:55:57.000000 gggdtparser-0.0.4/gggdtparser/dtconfigs.py
--rw-rw-rw-   0        0        0    15978 2023-04-02 02:55:57.000000 gggdtparser-0.0.4/gggdtparser/dtparser.py
--rw-rw-rw-   0        0        0    39947 2023-04-02 02:55:57.000000 gggdtparser-0.0.4/gggdtparser/test.py
-drwxrwxrwx   0        0        0        0 2023-04-02 02:58:17.797691 gggdtparser-0.0.4/gggdtparser.egg-info/
--rw-rw-rw-   0        0        0     2791 2023-04-02 02:58:17.000000 gggdtparser-0.0.4/gggdtparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-02 02:58:17.000000 gggdtparser-0.0.4/gggdtparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 02:58:17.000000 gggdtparser-0.0.4/gggdtparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-02 02:58:17.000000 gggdtparser-0.0.4/gggdtparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-04-02 02:58:17.799687 gggdtparser-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:26:42.677419 gggdtparser-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-04-10 04:26:42.678417 gggdtparser-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 04:26:42.672432 gggdtparser-0.0.5/gggdtparser/
+-rw-rw-rw-   0        0        0      259 2023-03-28 10:39:47.000000 gggdtparser-0.0.5/gggdtparser/__init__.py
+-rw-rw-rw-   0        0        0    11660 2023-04-10 03:37:05.000000 gggdtparser-0.0.5/gggdtparser/dtconfigs.py
+-rw-rw-rw-   0        0        0    15931 2023-04-10 01:46:49.000000 gggdtparser-0.0.5/gggdtparser/dtparser.py
+-rw-rw-rw-   0        0        0    40554 2023-04-07 06:00:15.000000 gggdtparser-0.0.5/gggdtparser/test.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:26:42.676422 gggdtparser-0.0.5/gggdtparser.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-04-10 04:26:42.000000 gggdtparser-0.0.5/gggdtparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-10 04:26:42.000000 gggdtparser-0.0.5/gggdtparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 04:26:42.000000 gggdtparser-0.0.5/gggdtparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 04:26:42.000000 gggdtparser-0.0.5/gggdtparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-04-10 04:26:42.685483 gggdtparser-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.0.5/setup.py
```

### Comparing `gggdtparser-0.0.4/LICENSE` & `gggdtparser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.4/PKG-INFO` & `gggdtparser-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.4
+Version: 0.0.5
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
@@ -29,14 +29,19 @@
 
 ## 项目原理
 
 1. 采用正则的方式完成对时间的抽取，进一步对抽取到的时间进行解析，即抽取和解析一体，用户给与的时间文本可以有很多非时间内容，使得解析更加便捷。
 2. 对语义话时间进行计算，对其他语言进行支持。
 3. 使用正则规则，后续增加特殊时间格式较为方便。
 
+## 项目特色
+
+1. 文本时间内能包含一些噪音
+2. 解析速度快
+
 ## 使用方法
 
 ### 安装
 
     pip install gggdtparser
 
 ### 使用
@@ -58,13 +63,47 @@
 ### 详细案例
 
 1. 参考dtformat.md中支持的格式。
 2. 参考test.py中的测试案例。
 
 ### 特色案例
 
+1. 语义时间的支持
+
+```
+   il y a 26 minutes
+   il y a 1 heure
+   Publié aujourd’hui à 10h34, modifié à 10h39
+   23分鐘前
+   ......      
+
+```
+
+2. 允许噪音
+
+```
+   发布于：2023/2/20
+   Hoje Macau - 4 Abr 2023 
+   2023年04月10日 07:46　来源：新闻网
+   ......
+```
+
+3. 支持多种语言
+
+```
+   31 март 2023  # 俄语
+   31 de marzo de 2023  # 西班牙语
+   27 Fev 2023  # 卡拜尔语
+   ......
+```
+
+## 待完善
+
+1. 兼容更多语言
+2. 对时区的解析
+
 ## 关于作者
 
 1. 邮箱：1194542196@qq.com
 2. 微信：hu1194542196
 3. 目前对常见的时间格式解析支持比较全，但是一些特殊的时间格式和其他语言的支持不够完善，如果遇到解析bug
    或不能解析的时间格式，可以私信作者，你们的提供越多，本库才能更完善。
```

### Comparing `gggdtparser-0.0.4/README.md` & `gggdtparser-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 ## 项目原理
 
 1. 采用正则的方式完成对时间的抽取，进一步对抽取到的时间进行解析，即抽取和解析一体，用户给与的时间文本可以有很多非时间内容，使得解析更加便捷。
 2. 对语义话时间进行计算，对其他语言进行支持。
 3. 使用正则规则，后续增加特殊时间格式较为方便。
 
+## 项目特色
+
+1. 文本时间内能包含一些噪音
+2. 解析速度快
+
 ## 使用方法
 
 ### 安装
 
     pip install gggdtparser
 
 ### 使用
@@ -40,13 +45,47 @@
 ### 详细案例
 
 1. 参考dtformat.md中支持的格式。
 2. 参考test.py中的测试案例。
 
 ### 特色案例
 
+1. 语义时间的支持
+
+```
+   il y a 26 minutes
+   il y a 1 heure
+   Publié aujourd’hui à 10h34, modifié à 10h39
+   23分鐘前
+   ......      
+
+```
+
+2. 允许噪音
+
+```
+   发布于：2023/2/20
+   Hoje Macau - 4 Abr 2023 
+   2023年04月10日 07:46　来源：新闻网
+   ......
+```
+
+3. 支持多种语言
+
+```
+   31 март 2023  # 俄语
+   31 de marzo de 2023  # 西班牙语
+   27 Fev 2023  # 卡拜尔语
+   ......
+```
+
+## 待完善
+
+1. 兼容更多语言
+2. 对时区的解析
+
 ## 关于作者
 
 1. 邮箱：1194542196@qq.com
 2. 微信：hu1194542196
 3. 目前对常见的时间格式解析支持比较全，但是一些特殊的时间格式和其他语言的支持不够完善，如果遇到解析bug
    或不能解析的时间格式，可以私信作者，你们的提供越多，本库才能更完善。
```

### Comparing `gggdtparser-0.0.4/gggdtparser/dtconfigs.py` & `gggdtparser-0.0.5/gggdtparser/dtconfigs.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 # date: 2023/3/24
 
 
 STRING_DATE_TIME_REGEX_LIST = [
     # 精准策略
     r"(?P<ts>\d{13})",
     r"(?P<ts>\d{10})",
-    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*T?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[:分]\s*(?P<S>\d{1,2})\s*[秒]?",
-    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s+T?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[分]?",
-    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s+(?P<H>\d{1,2})\s*[时]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{2})\s*[:时h]\s*(?P<M>\d{2})\s*[:分]\s*(?P<S>\d{2})\s*[秒]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{2})\s*[:时h]\s*(?P<M>\d{2})\s*[分]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{2})\s*[时]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[:分]\s*(?P<S>\d{1,2})\s*[秒]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[分]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{1,2})\s*[时]?",
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?",
 
 
     # before
     r"(?P<bd>\d+)\s*天\s*前",
     r"(?P<bM>\d+)\s*分钟\s*前",
     r"(?P<bH>\d+)\s*小时\s*前",
@@ -46,14 +50,16 @@
     r"(?P<sd>前天)\s*(?P<H>\d+):(?P<M>\d+)",
     r"(?P<sd>前天)\s*(?P<H>\d+)",
     r"(?P<sd>前天)",
     r"(?P<so>刚刚)",
 ]
 
 STRING_DATE_TIME_REGEX_LIST_FUZZY = [  # 模糊时间
+    # 2010 7月19日
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]?\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?",
     # 14 March 2023
     r"(?P<d>\d{1,2})[\.]?\s*(?P<m>\d{1,2})\s*[月]\s*(?P<Y>\d{4})",
     # 2023/0329
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})(?P<d>\d{2})",
     # 2012.9
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})",
     r"(?P<m>\d{1,2})\s*[\-\|/\.月]?\s*(?P<d>\d{1,2})\s*[\-\|/\.日]?\s*?(?P<Y>\d{4})\s*[\-\|/\.年]?",
@@ -78,14 +84,15 @@
     # Feb 5
     r"(?P<m>\d{1,2})\s*[月]\s*(?P<d>\d{1,2})",
     # 2022年
     r"(?P<Y>\d{4})\s*年",
     # 02月
     r"(?P<m>\d{1,2})\s*[月]",
 
+
 ]
 
 OTHER_STRING_DATE_TIME_REGEX_LIST = {
     'EN': [
         # Thu February 02 02:02:02 2022
         r"(?P<m>\d{1,2})\s*[\-\|/\.月]?\s*(?P<d>\d{1,2})\s*[\-\|/\.日]?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[:分]\s*(?P<S>\d{1,2})\s*[秒]?\s*(?P<Y>\d{4})\s*[\-\|/\.年]?",
         # 04:28, 13 Feb 2023
@@ -119,31 +126,53 @@
 
 
     ],
     'ZH_TW': [
         r"民国\s*(?P<mgY>\d+)[\-\|/\.年]\s*(?P<m>\d+)[\-\|/\.月]\s*(?P<d>\d+)[日]?",
         r"民国\s*(?P<mgY>\d+)[\-\|/\.年]\s*(?P<m>\d+)[\-\|/\.月]?",
         r"民国(?P<mgY>\d+)[年]?",
+
+        r"(?P<bH>\d+)\s*时间前",
     ],
     'FRA': [
         # 31/03/23 à 12h03
         r"(?P<d>\d{1,2})\s*[\-\|/\.日]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<Y>\d{2,4})\s*[,]?\s*(?P<H>\d{1,2})\s*[:时h\.]\s*(?P<M>\d{1,2})\s*[:分]?",
 
         # before
         r"(il y a)?\s*(?P<bH>\d+)\s*heures?\s*(ago)?",
+    ],
+    "SWE": [
+        r"(?P<bS>\d+)\s*segundos?\s*",
+        r"(?P<bM>\d+)\s*minutos?\s*",
+        r"(?P<bH>\d+)\s*horas?\s*",
+        r"(?P<bd>\d+)\s*dias?\s*",
+        r"(?P<bm>\d+)\s*meses?\s*",
+        r"(?P<ba>\d+)\s*semanas?\s*",
+        r"(?P<bY>\d+)\s*anos?\s*",
+    ],
+    "SOM": [
+        r"(?P<bH>\d+)\s*Saacadood?\s*",
+    ],
+    "IR": [
+        r"(?P<bS>\d+)\s*секунда?\s*",
+        r"(?P<bM>\d+)\s*минута?\s*",
+        r"(?P<bH>\d+)\s*час?\s*",
+    ],
+    "MAR": [
+        r"(?P<bM>\d+)\s*तासांपूर्वी",
     ]
 }
 
 # 替换翻译
 SUB_TRANSLATE = {
     'EN': [
         (r"January|JANUARY|Jan\.|Jan", "1月"),
         (r"February|FEBRUARY|Feb\.", "2月"),
-        (r"March|MARCH|Mar\.|Mar", "3月"),
-        (r"April|APRIL|Apr\.|Apr", "4月"),
+        (r"March|MARCH|Mar\.|Mar|Mai", "3月"),
+        (r"April|APRIL|Apr\.|Apr|Abr", "4月"),
         (r"May\.|May|MAY", "5月"),
         (r"June|JUNE|Jun\.|Jun", "6月"),
         (r"July|JULY|Jul\.|Jul", "7月"),
         (r"August|AUGUST|Aug\.|Aug", "8月"),
         (r"September|SEPTEMBER|Sept\.|Sept|Sep\.|Sep", "9月"),
         (r"October|OCTOBER|Oct\.|Oct", "10月"),
         (r"November|NOVEMBER|Nov\.|Nov", "11月"),
@@ -178,17 +207,20 @@
         (r"四", "4"),
         (r"五", "5"),
         (r"六", "6"),
         (r"七", "7"),
         (r"八", "8"),
         (r"九", "9"),
         (r"零", "0"),
+        (r"上午", "am"),
+        (r"下午", "pm"),
     ],
     'ZH_TW': [
         (r'時', '时'),
+        (r'間', '间'),
         (r'國', '国'),
         (r'鐘', '钟'),
     ],
     'DE': [
         (r"Januar|Jan", "1月"),
         (r"Februar|Feb\.", "2月"),
         (r"März|Mär", "3月"),
@@ -219,14 +251,60 @@
         (r"aujourd’hui à", ""),
         (r"à l’instant", "刚刚"),
         (r"à", ""),
     ],
     'VIE': [
         (r"phút", "分钟"),
         (r"trước", "前"),
+        (r"giờ", "小时"),
+    ],
+    'KAB': [
+        (r"Fev", "2月"),
+    ],
+    'KOR': [
+        (r"(de)?\s*enero\s*(de)?", "1月"),
+        (r"(de)?\s*febrero\s*(de)?", "2月"),
+        (r"(de)?\s*marzo\s*(de)?", "3月"),
+        (r"(de)?\s*abril\s*(de)?", "4月"),
+        (r"(de)?\s*mayo\s*(de)?", "5月"),
+        (r"(de)?\s*junio\s*(de)?", "6月"),
+        (r"(de)?\s*julio\s*(de)?", "7月"),
+        (r"(de)?\s*agosto\s*(de)?", "8月"),
+        (r"(de)?\s*septiembre\s*(de)?", "9月"),
+        (r"(de)?\s*octubre\s*(de)?", "10月"),
+        (r"(de)?\s*noviembre\s*(de)?", "11月"),
+        (r"(de)?\s*diciembre\s*(de)?", "12月"),
+    ],
+    'IR': [
+        (r"январь", "1月"),
+        (r"февраль", "2月"),
+        (r"март", "3月"),
+        (r"апрель", "4月"),
+        (r"май", "5月"),
+        (r"июнь", "6月"),
+        (r"июль", "7月"),
+        (r"август", "8月"),
+        (r"сентябрь", "9月"),
+        (r"октябрь", "10月"),
+        (r"ноябрь", "11月"),
+        (r"декабрь", "12月"),
+    ],
+    'SWE': [
+        (r"janeiro", "1月"),
+        (r"fevereiro", "2月"),
+        (r"março", "3月"),
+        (r"abril", "4月"),
+        (r"maio", "5月"),
+        (r"junho", "6月"),
+        (r"julho", "7月"),
+        (r"agosto", "8月"),
+        (r"setembro", "9月"),
+        (r"outubro", "10月"),
+        (r"novembro", "11月"),
+        (r"dezembro", "12月"),
     ],
     # 最后
     'END': [
         (r"Feb", "2月"),
     ]
 
 }
```

### Comparing `gggdtparser-0.0.4/gggdtparser/dtparser.py` & `gggdtparser-0.0.5/gggdtparser/dtparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             if not match_obj:
                 continue
             group_dict = match_obj.groupdict()
             if group_dict:
                 try:
                     result = cls._parse_group_dict(
                         group_dict, accurately, max_datetime)
-                    # print(regex)
+                    print(regex)
                     return result
                 except Exception:
                     continue
 
     @classmethod
     def _parse_group_dict(cls, group_dict, accurately, max_datetime):
         un_accurately = not accurately
@@ -278,17 +278,15 @@
             accurately, use_now_config['second'], now.second, second)
         month = 1 if not month else month
         day = 1 if not day else day
         parse_datetime = datetime.datetime(
             year=year, month=month,
             day=day, hour=hour,
             minute=minute, second=second) - change_timedelta
-        if not max_datetime:
-            max_datetime = now
-        if parse_datetime > max_datetime:
+        if max_datetime and parse_datetime > max_datetime:
             raise Exception('解析时间超出最大时间')
         return parse_datetime
 
     @classmethod
     def _update_use_now_config(cls, use_now_config, year=False, month=False,
                                day=False, hour=False, minute=False,
                                second=False):
```

### Comparing `gggdtparser-0.0.4/gggdtparser/test.py` & `gggdtparser-0.0.5/gggdtparser/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,22 @@
         'accurately': datetime.datetime(
             year=2022, month=2, day=2,
             hour=2, minute=2),
         'un_accurately': datetime.datetime(
             year=2022, month=2, day=2,
             hour=2, minute=2, second=now.second),
     },
+    '2022年2月02日，上午02:02': {
+            'accurately': datetime.datetime(
+                year=2022, month=2, day=2, hour=2,
+                minute=2, second=0),
+            'un_accurately': datetime.datetime(
+                year=2022, month=2, day=2, hour=2,
+                minute=2, second=now.second)
+        },
     '2022-02-02 02:02': {
         'accurately': datetime.datetime(
             year=2022, month=2, day=2,
             hour=2, minute=2),
         'un_accurately': datetime.datetime(
             year=2022, month=2, day=2,
             hour=2, minute=2, second=now.second),
@@ -118,14 +126,21 @@
         'accurately': datetime.datetime(
             year=2022, month=2, day=2, hour=0,
             minute=0, second=0),
         'un_accurately': datetime.datetime(
             year=2022, month=2, day=2, hour=now.hour,
             minute=now.minute, second=now.second)
     },
+    '2022 02月02日': {
+        'accurately': datetime.datetime(
+            year=2022, month=2, day=2, ),
+        'un_accurately': datetime.datetime(
+            year=2022, month=2, day=2,
+            hour=now.hour, minute=now.minute, second=now.second),
+    },
     '2022年02月': {
         'accurately': datetime.datetime(
             year=2022, month=2, day=1),
         'un_accurately': datetime.datetime(
             year=2022, month=2, day=now.day,
             hour=now.hour, minute=now.minute, second=now.second),
     },
```

### Comparing `gggdtparser-0.0.4/gggdtparser.egg-info/PKG-INFO` & `gggdtparser-0.0.5/gggdtparser.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.4
+Version: 0.0.5
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
@@ -29,14 +29,19 @@
 
 ## 项目原理
 
 1. 采用正则的方式完成对时间的抽取，进一步对抽取到的时间进行解析，即抽取和解析一体，用户给与的时间文本可以有很多非时间内容，使得解析更加便捷。
 2. 对语义话时间进行计算，对其他语言进行支持。
 3. 使用正则规则，后续增加特殊时间格式较为方便。
 
+## 项目特色
+
+1. 文本时间内能包含一些噪音
+2. 解析速度快
+
 ## 使用方法
 
 ### 安装
 
     pip install gggdtparser
 
 ### 使用
@@ -58,13 +63,47 @@
 ### 详细案例
 
 1. 参考dtformat.md中支持的格式。
 2. 参考test.py中的测试案例。
 
 ### 特色案例
 
+1. 语义时间的支持
+
+```
+   il y a 26 minutes
+   il y a 1 heure
+   Publié aujourd’hui à 10h34, modifié à 10h39
+   23分鐘前
+   ......      
+
+```
+
+2. 允许噪音
+
+```
+   发布于：2023/2/20
+   Hoje Macau - 4 Abr 2023 
+   2023年04月10日 07:46　来源：新闻网
+   ......
+```
+
+3. 支持多种语言
+
+```
+   31 март 2023  # 俄语
+   31 de marzo de 2023  # 西班牙语
+   27 Fev 2023  # 卡拜尔语
+   ......
+```
+
+## 待完善
+
+1. 兼容更多语言
+2. 对时区的解析
+
 ## 关于作者
 
 1. 邮箱：1194542196@qq.com
 2. 微信：hu1194542196
 3. 目前对常见的时间格式解析支持比较全，但是一些特殊的时间格式和其他语言的支持不够完善，如果遇到解析bug
    或不能解析的时间格式，可以私信作者，你们的提供越多，本库才能更完善。
```

### Comparing `gggdtparser-0.0.4/setup.cfg` & `gggdtparser-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6474 7061 7273 6572 0d0a   = gggdtparser..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 340d  version = 0.0.4.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 350d  version = 0.0.5.
 00000030: 0a61 7574 686f 7220 3d20 6b75 7365 6e0d  .author = kusen.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6875 3131 3934 3534 3231 3936 4071 712e  hu1194542196@qq.
 00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000070: 203d 20cd a8d3 c3a1 a2b1 e3bd dda1 a2d7   = .............
 00000080: bcc8 b7b5 c4d7 d6b7 fbb4 aeca b1bc e4bd  ................
 00000090: e2ce f6b9 a4be df0d 0a6c 6f6e 675f 6465  .........long_de
```

