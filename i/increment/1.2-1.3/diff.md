# Comparing `tmp/increment-1.2.tar.gz` & `tmp/increment-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increment-1.2.tar", last modified: Sat Apr  8 16:18:29 2023, max compression
+gzip compressed data, was "increment-1.3.tar", last modified: Mon Apr 10 14:19:46 2023, max compression
```

## Comparing `increment-1.2.tar` & `increment-1.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 increment-1.2/LICENSE
--rw-r--r--   0        0        0     1735 2023-04-08 16:07:56.686123 increment-1.2/README.md
--rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 increment-1.2/increment/__init__.py
--rw-r--r--   0        0        0     1512 2023-04-08 15:57:17.331903 increment-1.2/increment/_increment.py
--rw-r--r--   0        0        0      569 2023-04-08 16:10:43.684141 increment-1.2/pyproject.toml
--rw-r--r--   0        0        0     2056 1970-01-01 00:00:00.000000 increment-1.2/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 increment-1.3/LICENSE
+-rw-r--r--   0        0        0     1691 2023-04-08 16:28:37.947596 increment-1.3/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 04:01:47.110396 increment-1.3/increment.py
+-rw-r--r--   0        0        0      582 2023-04-10 09:20:39.407916 increment-1.3/pyproject.toml
+-rw-r--r--   0        0        0     2042 1970-01-01 00:00:00.000000 increment-1.3/PKG-INFO
```

### Comparing `increment-1.2/LICENSE` & `increment-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `increment-1.2/README.md` & `increment-1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,28 +50,25 @@
 
 使用当前时间：
 
 ```python
 inc.pk2()
 # >>> 'lg8657cj_gsdo_258_0_3'
 
-inc.pk2()
-# >>> 'lg8657cj_gsdo_258_0_4'
-
 # 'lg8657cj'是当前时间
 ```
 
-只返回递增主键：
+只返回自增主键：
 
 ```python
 inc.pk3()
-# >>> '0_5'
+# >>> '0_4'
 
 inc.pk3()
-# >>> '0_6'
+# >>> '0_5'
 ```
 
 # 支持作者1元
 
 increment 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
```

### Comparing `increment-1.2/pyproject.toml` & `increment-1.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "increment"
-version = "1.2"
+version = "1.3"
 description = "主键生成器，支持多机器|多进程|多线程高并发生成"
-dependencies = []
+dependencies = ["lccpy >=1.3"]
 keywords = ["increment"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `increment-1.2/PKG-INFO` & `increment-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: increment
-Version: 1.2
+Version: 1.3
 Summary: 主键生成器，支持多机器|多进程|多线程高并发生成
 Keywords: increment
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Dist: lccpy >=1.3
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/increment
 
 # 项目描述
 
 主键生成器，支持多机器|多进程|多线程高并发生成。
 
 # 安装
@@ -61,28 +62,25 @@
 
 使用当前时间：
 
 ```python
 inc.pk2()
 # >>> 'lg8657cj_gsdo_258_0_3'
 
-inc.pk2()
-# >>> 'lg8657cj_gsdo_258_0_4'
-
 # 'lg8657cj'是当前时间
 ```
 
-只返回递增主键：
+只返回自增主键：
 
 ```python
 inc.pk3()
-# >>> '0_5'
+# >>> '0_4'
 
 inc.pk3()
-# >>> '0_6'
+# >>> '0_5'
 ```
 
 # 支持作者1元
 
 increment 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
```

