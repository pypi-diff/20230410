# Comparing `tmp/rstyleslice-1.1.tar.gz` & `tmp/rstyleslice-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstyleslice-1.1.tar", last modified: Tue Feb 14 12:31:48 2023, max compression
+gzip compressed data, was "rstyleslice-1.4.tar", last modified: Mon Apr 10 14:16:31 2023, max compression
```

## Comparing `rstyleslice-1.1.tar` & `rstyleslice-1.4.tar`

### file list

```diff
@@ -1,8 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 rstyleslice-1.1/LICENSE
--rw-r--r--   0        0        0     3548 2023-02-14 02:27:24.987834 rstyleslice-1.1/README.md
--rw-r--r--   0        0        0       26 2023-02-13 16:21:20.491336 rstyleslice-1.1/__init__.py
--rw-r--r--   0        0        0      674 2023-02-14 12:26:46.765056 rstyleslice-1.1/pyproject.toml
--rw-r--r--   0        0        0       40 2023-02-14 01:31:45.064435 rstyleslice-1.1/rstyleslice/__init__.py
--rw-r--r--   0        0        0     5483 2023-02-05 08:54:32.021022 rstyleslice-1.1/rstyleslice/_rstyleslice.py
--rw-r--r--   0        0        0    11806 2023-02-12 15:34:56.450005 rstyleslice-1.1/test.py
--rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 rstyleslice-1.1/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 rstyleslice-1.4/LICENSE
+-rw-r--r--   0        0        0     3293 2023-04-09 11:36:38.368832 rstyleslice-1.4/README.md
+-rw-r--r--   0        0        0      571 2023-04-10 09:28:33.061542 rstyleslice-1.4/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4/rstyleslice.py
+-rw-r--r--   0        0        0     3606 1970-01-01 00:00:00.000000 rstyleslice-1.4/PKG-INFO
```

### Comparing `rstyleslice-1.1/LICENSE` & `rstyleslice-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rstyleslice-1.1/README.md` & `rstyleslice-1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,82 @@
 # 项目描述
 
-让Python容器（如：list）可以使用R语言风格的索引和切片。
+一套符合直觉的索引和切片语法。
 
-R语言风格索引：从1开始，1表示第1个元素，-1表示倒数第1个元素。
+|                                        | **Python**                                               | **rstyleslice**                                          |
+| -------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
+| **索引**                         | 从 0 开始<br />0 表示第 1 个元素<br />-1 表示倒数第 1 个元素（相同点） | 从 1 开始<br />1 表示第 1 个元素<br />-1 表示倒数第 1 个元素（相同点）   |
+| **切片**                         | 左闭右开区间，例如：<br />[3: 5] 表示提取第 4、5 这 2 个元素           | 双闭区间，例如：<br />[3: 5] 表示提取第 3、4、5 这 3 个元素              |
+| **从右往**<br />**左切片** | step（步长）为负值，例如：<br />[9: 1: -1] 表示提取第 9~3 这 7 个元素  | step（步长）始终为正值，例如：<br />[9: 1: 1] 表示提取第 9~1 这 9 个元素 |
 
-R语言风格切片：双闭区间。如：[3: 5]表示提取第3、4、5三个元素。
+切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>1  时表示间隔式切片。
 
-# 安装、文档与源码
+# 安装与教程
 
 安装：`pip install rstyleslice`
 
-文档：[https://www.yuque.com/lcctoor/lcctopen/rstyleslic](https://www.yuque.com/lcctoor/lcctopen/rstyleslice)
+[教程](https://github.com/lcctoor/lccpy/blob/main/rstyleslice/docs/doc.md)
 
-源码：[https://github.com/lcctoor/lcctopen/tree/main/rstyleslice](https://github.com/lcctoor/lcctopen/tree/main/rstyleslice)
+# Bug提交、功能提议
 
-# 关于作者
-
-作者：许灿标，一个90后程序员。爱思考，爱钻研，善归纳。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
-更多信息：[关于作者](https://www.yuque.com/lcctoor/support/author)
+# 关于作者
 
-个人主页：[语雀](https://www.yuque.com/lcctoor)
+作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-微信：
-
-![微信二维码](https://raw.githubusercontent.com/lcctoor/support/main/author/WeChatQR200_200.jpg)
+[主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
-交流群：目前我们有微信交流群>高质量读书会、Python技术交流，若有兴趣加入，请与我联系后获取。
+开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
 
-# 语法预览
+# 教程预览
 
 导入：
 
-```
-from rstyleslice import rslice, rindex
+```python
+from rstyleslice import rslice
 ```
 
 创建R风格容器：
 
-```
-obj = rslice([1, 2, 3, 4, 5, 6, 7, 8, 9])
-# 理论上，Python中任何可以索引和切片的对象都可以转化成R风格容器
+```python
+obj = rslice([1,2,3,4,5,6,7,8,9])
+
+# Python中任何可以索引和切片的对象（如list、str、tuple）都可以转化成R风格容器。
 ```
 
 索引取值：
 
-```
+```python
 obj[1]
 # >>> 1
 ```
 
 索引赋值：
 
-```
+```python
 obj[1] = 111
 obj[:]
 # >>> [111, 2, 3, 4, 5, 6, 7, 8, 9]
 ```
 
 切片取值：
 
-```
+```python
 obj[3:7]  # >>> [3, 4, 5, 6, 7]
 obj[7:3]  # >>> [7, 6, 5, 4, 3]
 obj[3:7:2]  # >>> [3, 5, 7]
 obj[8:2:3]  # >>> [8, 5, 2]
 ```
 
 切片赋值：
 
-```
+```python
 obj[4:6] = [44, 55]
 obj[:]
 # >>> [111, 2, 3, 44, 55, 7, 8, 9]
 
 obj[4:6] = []
 obj[:]
 # >>> [111, 2, 3, 8, 9]
@@ -85,23 +86,14 @@
 # >>> [111, 2, 3, 1, 2, 3, 4, 5]
 
 obj[4:100] = ['1', 2, 3, 4, 5]
 obj[:]
 # >>> [111, 2, 3, '1', 2, 3, 4, 5]
 ```
 
-调用Python容器的原生方法：
+# 支持作者1元
+
+rstyleslice 是一个免费的开源项目，由个人维护。
+
+每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-| 代码                              |  结果  |                  解释                  |
-| :-------------------------------- | :----: | :------------------------------------: |
-| rslice('abcd').count('a')         |   1   |                                        |
-| rslice('abcd').index('b')         |   1   |  原生index方法返回Python风格的索引值  |
-| rslice('abcd').index_('b')        |   2   | 在原生方法后加"_"表示将返回值+1, 1+1=2 |
-| rslice('ABCd').lower()            | 'abcd' |                                        |
-| rslice('ABCd').lower().count('a') |   1   |                                        |
-
-| 代码                                | 结果 |                                           解释                                           |
-| :---------------------------------- | :--: | :--------------------------------------------------------------------------------------: |
-| rslice([6,7,8,9]).pop(1)            |  7  |                               原生pop方法按Python索引取值                               |
-| rslice([6,7,8,9]).pop( rindex(1) )  |  6  |                         使用rindex将R风格的索引转化成Python索引                         |
-| rslice([6,7,8,9]).pop_(1)           |  8  |                          在原生方法后加"_"表示将返回值+1, 7+1=8                          |
-| rslice([6,7,8,9]).pop_( rindex(1) ) |  7  | 先用rindex将R索引转化为Python索引, 然后再将返回值+1<br />相当于: [6, 7, 8, 9].pop(0) + 1 |
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
```

### Comparing `rstyleslice-1.1/PKG-INFO` & `rstyleslice-1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,94 @@
 Metadata-Version: 2.1
 Name: rstyleslice
-Version: 1.1
-Summary: 让Python容器（如：list）可以使用R语言风格的索引和切片。
+Version: 1.4
+Summary: 一套符合直觉的索引和切片语法
 Keywords: rstyleslice,slice
 Author-email: 许灿标 <lcctoor@outlook.com>
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Project-URL: Documentation, https://www.yuque.com/lcctoor/lcctopen/rstyleslice
-Project-URL: Source, https://github.com/lcctoor/lcctopen/tree/main/rstyleslice
+Requires-Dist: lccpy >=1.3
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/rstyleslice
 
 # 项目描述
 
-让Python容器（如：list）可以使用R语言风格的索引和切片。
+一套符合直觉的索引和切片语法。
 
-R语言风格索引：从1开始，1表示第1个元素，-1表示倒数第1个元素。
+|                                        | **Python**                                               | **rstyleslice**                                          |
+| -------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
+| **索引**                         | 从 0 开始<br />0 表示第 1 个元素<br />-1 表示倒数第 1 个元素（相同点） | 从 1 开始<br />1 表示第 1 个元素<br />-1 表示倒数第 1 个元素（相同点）   |
+| **切片**                         | 左闭右开区间，例如：<br />[3: 5] 表示提取第 4、5 这 2 个元素           | 双闭区间，例如：<br />[3: 5] 表示提取第 3、4、5 这 3 个元素              |
+| **从右往**<br />**左切片** | step（步长）为负值，例如：<br />[9: 1: -1] 表示提取第 9~3 这 7 个元素  | step（步长）始终为正值，例如：<br />[9: 1: 1] 表示提取第 9~1 这 9 个元素 |
 
-R语言风格切片：双闭区间。如：[3: 5]表示提取第3、4、5三个元素。
+切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>1  时表示间隔式切片。
 
-# 安装、文档与源码
+# 安装与教程
 
 安装：`pip install rstyleslice`
 
-文档：[https://www.yuque.com/lcctoor/lcctopen/rstyleslic](https://www.yuque.com/lcctoor/lcctopen/rstyleslice)
+[教程](https://github.com/lcctoor/lccpy/blob/main/rstyleslice/docs/doc.md)
 
-源码：[https://github.com/lcctoor/lcctopen/tree/main/rstyleslice](https://github.com/lcctoor/lcctopen/tree/main/rstyleslice)
+# Bug提交、功能提议
 
-# 关于作者
-
-作者：许灿标，一个90后程序员。爱思考，爱钻研，善归纳。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
-更多信息：[关于作者](https://www.yuque.com/lcctoor/support/author)
+# 关于作者
 
-个人主页：[语雀](https://www.yuque.com/lcctoor)
+作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-微信：
-
-![微信二维码](https://raw.githubusercontent.com/lcctoor/support/main/author/WeChatQR200_200.jpg)
+[主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
-交流群：目前我们有微信交流群>高质量读书会、Python技术交流，若有兴趣加入，请与我联系后获取。
+开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
 
-# 语法预览
+# 教程预览
 
 导入：
 
-```
-from rstyleslice import rslice, rindex
+```python
+from rstyleslice import rslice
 ```
 
 创建R风格容器：
 
-```
-obj = rslice([1, 2, 3, 4, 5, 6, 7, 8, 9])
-# 理论上，Python中任何可以索引和切片的对象都可以转化成R风格容器
+```python
+obj = rslice([1,2,3,4,5,6,7,8,9])
+
+# Python中任何可以索引和切片的对象（如list、str、tuple）都可以转化成R风格容器。
 ```
 
 索引取值：
 
-```
+```python
 obj[1]
 # >>> 1
 ```
 
 索引赋值：
 
-```
+```python
 obj[1] = 111
 obj[:]
 # >>> [111, 2, 3, 4, 5, 6, 7, 8, 9]
 ```
 
 切片取值：
 
-```
+```python
 obj[3:7]  # >>> [3, 4, 5, 6, 7]
 obj[7:3]  # >>> [7, 6, 5, 4, 3]
 obj[3:7:2]  # >>> [3, 5, 7]
 obj[8:2:3]  # >>> [8, 5, 2]
 ```
 
 切片赋值：
 
-```
+```python
 obj[4:6] = [44, 55]
 obj[:]
 # >>> [111, 2, 3, 44, 55, 7, 8, 9]
 
 obj[4:6] = []
 obj[:]
 # >>> [111, 2, 3, 8, 9]
@@ -96,24 +98,15 @@
 # >>> [111, 2, 3, 1, 2, 3, 4, 5]
 
 obj[4:100] = ['1', 2, 3, 4, 5]
 obj[:]
 # >>> [111, 2, 3, '1', 2, 3, 4, 5]
 ```
 
-调用Python容器的原生方法：
+# 支持作者1元
+
+rstyleslice 是一个免费的开源项目，由个人维护。
+
+每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-| 代码                              |  结果  |                  解释                  |
-| :-------------------------------- | :----: | :------------------------------------: |
-| rslice('abcd').count('a')         |   1   |                                        |
-| rslice('abcd').index('b')         |   1   |  原生index方法返回Python风格的索引值  |
-| rslice('abcd').index_('b')        |   2   | 在原生方法后加"_"表示将返回值+1, 1+1=2 |
-| rslice('ABCd').lower()            | 'abcd' |                                        |
-| rslice('ABCd').lower().count('a') |   1   |                                        |
-
-| 代码                                | 结果 |                                           解释                                           |
-| :---------------------------------- | :--: | :--------------------------------------------------------------------------------------: |
-| rslice([6,7,8,9]).pop(1)            |  7  |                               原生pop方法按Python索引取值                               |
-| rslice([6,7,8,9]).pop( rindex(1) )  |  6  |                         使用rindex将R风格的索引转化成Python索引                         |
-| rslice([6,7,8,9]).pop_(1)           |  8  |                          在原生方法后加"_"表示将返回值+1, 7+1=8                          |
-| rslice([6,7,8,9]).pop_( rindex(1) ) |  7  | 先用rindex将R索引转化为Python索引, 然后再将返回值+1<br />相当于: [6, 7, 8, 9].pop(0) + 1 |
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
```

