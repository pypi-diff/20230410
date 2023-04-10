# Comparing `tmp/encrypt256-1.6.tar.gz` & `tmp/encrypt256-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encrypt256-1.6.tar", last modified: Tue Feb 14 12:32:28 2023, max compression
+gzip compressed data, was "encrypt256-1.8.tar", last modified: Mon Apr 10 14:21:22 2023, max compression
```

## Comparing `encrypt256-1.6.tar` & `encrypt256-1.8.tar`

### file list

```diff
@@ -1,8 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-14 11:47:56.900367 encrypt256-1.6/LICENSE
--rw-r--r--   0        0        0     1967 2023-02-14 11:56:34.519141 encrypt256-1.6/README.md
--rw-r--r--   0        0        0       25 2022-11-12 19:25:42.000000 encrypt256-1.6/__init__.py
--rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 encrypt256-1.6/encrypt256/__init__.py
--rw-r--r--   0        0        0     4990 2023-02-14 11:32:44.328761 encrypt256-1.6/encrypt256/_encrypt256.py
--rw-r--r--   0        0        0      695 2023-02-14 12:25:50.582598 encrypt256-1.6/pyproject.toml
--rw-r--r--   0        0        0     1049 2023-02-14 11:15:11.325602 encrypt256-1.6/test.py
--rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 encrypt256-1.6/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-14 11:47:56.900367 encrypt256-1.8/LICENSE
+-rw-r--r--   0        0        0     2266 2023-04-06 03:55:17.481058 encrypt256-1.8/README.md
+-rw-r--r--   0        0        0       30 2023-04-10 04:00:30.884575 encrypt256-1.8/encrypt256.py
+-rw-r--r--   0        0        0      614 2023-04-10 09:20:22.910931 encrypt256-1.8/pyproject.toml
+-rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 encrypt256-1.8/PKG-INFO
```

### Comparing `encrypt256-1.6/LICENSE` & `encrypt256-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `encrypt256-1.6/README.md` & `encrypt256-1.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,80 @@
 # 项目描述
 
 一个用于加密str型和bytes型数据的加密器。
 
-* 此包是基于pycryptodome进行二次封装，底层加密算法为AES-CBC-256。
-* 加密时，会自动创建随机salt、随机iv、原始明文的校验值，并把校验值添加到密文中。
-* 解密时，会自动根据校验值校验“解密得到的明文”与“原始明文”是否一致。
+1、底层加密算法为AES-CBC-256。
 
-# 安装、文档与源码
+2、加密时，会自动创建随机salt、随机iv、原始明文的校验值，并把校验值添加到密文中。
 
-安装：`pip install encrypt256`
+3、解密时，会自动根据校验值校验“解密得到的明文”与“原始明文”是否一致。
 
-文档：[https://www.yuque.com/lcctoor/lcctopen/encrypt256](https://www.yuque.com/lcctoor/lcctopen/encrypt256)
+# 安装与教程
 
-源码：[https://github.com/lcctoor/lcctopen/tree/main/encrypt256](https://github.com/lcctoor/lcctopen/tree/main/encrypt256)
+安装：`pip install encrypt256`
 
-# 关于作者
+[教程](https://github.com/lcctoor/lccpy/blob/main/encrypt256/docs/doc.md)
 
-作者：许灿标，一个90后程序员。爱思考，爱钻研，善归纳。
+# Bug提交、功能提议
 
-更多信息：[关于作者](https://www.yuque.com/lcctoor/support/author)
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
-个人主页：[语雀](https://www.yuque.com/lcctoor)
+# 关于作者
 
-邮箱：lcctoor@outlook.com
+作者：许灿标
 
-微信：
+邮箱：lcctoor@outlook.com
 
-![微信二维码](https://raw.githubusercontent.com/lcctoor/support/main/author/WeChatQR200_200.jpg)
+[主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
-交流群：目前我们有微信交流群>高质量读书会、Python技术交流，若有兴趣加入，请与我联系后获取。
+开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
 
-# 语法预览
+# 教程预览
 
 导入：
 
-```
+```python
 from encrypt256 import Encrypt256
 ```
 
 创建加密器：
 
-```
+```python
 password1 = 123456789  # 支持int型密钥
 password2 = '黄河之水天上来'  # 支持str型密钥
 password3 = '床前明月光'.encode('utf8')  # 支持bytes型密钥
 
 enctool = Encrypt256(password1)  # 创建加密器
 ```
 
 加密：
 
-```
+```python
 # 加密str型数据
 p1 = '人生自古谁五死'
 c1 = enctool.encrypt(p1, checkSize=32)
 
 # 加密bytes型数据
 p2 = '莎士比亚'.encode('utf8')
 c2 = enctool.encrypt(p2, checkSize=64)
 ```
 
 解密：
 
-```
+```python
 p11 = enctool.decrypt(c1)
 p22 = enctool.decrypt(c2)
 
 assert p1 == p11
 assert p2 == p22
 
 assert type(p1) is type(p11)
 assert type(p2) is type(p22)
 ```
+
+# 支持作者1元
+
+encrypt256 是一个免费的开源项目，由个人维护。
+
+每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
+
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
```

### Comparing `encrypt256-1.6/PKG-INFO` & `encrypt256-1.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,92 @@
 Metadata-Version: 2.1
 Name: encrypt256
-Version: 1.6
+Version: 1.8
 Summary: 一个用于加密str型和bytes型数据的加密器
 Keywords: encrypt256,encrypt,AES,pycryptodome,Crypto
 Author-email: 许灿标 <lcctoor@outlook.com>
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: pycryptodome
-Project-URL: Documentation, https://www.yuque.com/lcctoor/lcctopen/encrypt256
-Project-URL: Source, https://github.com/lcctoor/lcctopen/tree/main/encrypt256
+Requires-Dist: lccpy >=1.3
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/encrypt256
 
 # 项目描述
 
 一个用于加密str型和bytes型数据的加密器。
 
-* 此包是基于pycryptodome进行二次封装，底层加密算法为AES-CBC-256。
-* 加密时，会自动创建随机salt、随机iv、原始明文的校验值，并把校验值添加到密文中。
-* 解密时，会自动根据校验值校验“解密得到的明文”与“原始明文”是否一致。
+1、底层加密算法为AES-CBC-256。
 
-# 安装、文档与源码
+2、加密时，会自动创建随机salt、随机iv、原始明文的校验值，并把校验值添加到密文中。
 
-安装：`pip install encrypt256`
+3、解密时，会自动根据校验值校验“解密得到的明文”与“原始明文”是否一致。
 
-文档：[https://www.yuque.com/lcctoor/lcctopen/encrypt256](https://www.yuque.com/lcctoor/lcctopen/encrypt256)
+# 安装与教程
 
-源码：[https://github.com/lcctoor/lcctopen/tree/main/encrypt256](https://github.com/lcctoor/lcctopen/tree/main/encrypt256)
+安装：`pip install encrypt256`
 
-# 关于作者
+[教程](https://github.com/lcctoor/lccpy/blob/main/encrypt256/docs/doc.md)
 
-作者：许灿标，一个90后程序员。爱思考，爱钻研，善归纳。
+# Bug提交、功能提议
 
-更多信息：[关于作者](https://www.yuque.com/lcctoor/support/author)
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
-个人主页：[语雀](https://www.yuque.com/lcctoor)
+# 关于作者
 
-邮箱：lcctoor@outlook.com
+作者：许灿标
 
-微信：
+邮箱：lcctoor@outlook.com
 
-![微信二维码](https://raw.githubusercontent.com/lcctoor/support/main/author/WeChatQR200_200.jpg)
+[主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
-交流群：目前我们有微信交流群>高质量读书会、Python技术交流，若有兴趣加入，请与我联系后获取。
+开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
 
-# 语法预览
+# 教程预览
 
 导入：
 
-```
+```python
 from encrypt256 import Encrypt256
 ```
 
 创建加密器：
 
-```
+```python
 password1 = 123456789  # 支持int型密钥
 password2 = '黄河之水天上来'  # 支持str型密钥
 password3 = '床前明月光'.encode('utf8')  # 支持bytes型密钥
 
 enctool = Encrypt256(password1)  # 创建加密器
 ```
 
 加密：
 
-```
+```python
 # 加密str型数据
 p1 = '人生自古谁五死'
 c1 = enctool.encrypt(p1, checkSize=32)
 
 # 加密bytes型数据
 p2 = '莎士比亚'.encode('utf8')
 c2 = enctool.encrypt(p2, checkSize=64)
 ```
 
 解密：
 
-```
+```python
 p11 = enctool.decrypt(c1)
 p22 = enctool.decrypt(c2)
 
 assert p1 == p11
 assert p2 == p22
 
 assert type(p1) is type(p11)
 assert type(p2) is type(p22)
 ```
 
+# 支持作者1元
+
+encrypt256 是一个免费的开源项目，由个人维护。
+
+每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
+
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
```

