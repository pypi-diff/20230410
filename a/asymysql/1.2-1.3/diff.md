# Comparing `tmp/asymysql-1.2.tar.gz` & `tmp/asymysql-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymysql-1.2.tar", last modified: Thu Mar 30 12:15:55 2023, max compression
+gzip compressed data, was "asymysql-1.3.tar", last modified: Mon Apr 10 14:24:22 2023, max compression
```

## Comparing `asymysql-1.2.tar` & `asymysql-1.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymysql-1.2/LICENSE
--rw-r--r--   0        0        0     6720 2023-03-30 06:12:11.347878 asymysql-1.2/README.md
--rw-r--r--   0        0        0       72 2023-03-11 14:46:21.808074 asymysql-1.2/asymysql/__init__.py
--rw-r--r--   0        0        0    20186 2023-03-11 14:46:52.936569 asymysql-1.2/asymysql/_asymysql.py
--rw-r--r--   0        0        0      570 2023-03-30 12:15:44.942643 asymysql-1.2/pyproject.toml
--rw-r--r--   0        0        0     6960 1970-01-01 00:00:00.000000 asymysql-1.2/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymysql-1.3/LICENSE
+-rw-r--r--   0        0        0     4862 2023-04-09 11:16:24.511029 asymysql-1.3/README.md
+-rw-r--r--   0        0        0       28 2023-04-10 03:48:57.281686 asymysql-1.3/asymysql.py
+-rw-r--r--   0        0        0      562 2023-04-10 09:20:03.028976 asymysql-1.3/pyproject.toml
+-rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 asymysql-1.3/PKG-INFO
```

### Comparing `asymysql-1.2/LICENSE` & `asymysql-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asymysql-1.2/README.md` & `asymysql-1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # 项目描述
 
 异步的 mysql ORM 。
 
-# 安装与文档
+# 安装与教程
 
 安装：`pip install asymysql`
 
-[文档](https://github.com/lcctoor/lccpy/blob/main/asymysql/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/asymysql/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
 
@@ -18,15 +18,15 @@
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
 开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
 
-# 语法预览
+# 教程预览
 
 导入：
 
 ```python
 from aiomysql import connect
 from asymysql import ORM, mc, mf
 ```
@@ -53,15 +53,15 @@
 line1 = {'姓名': '小一', '年龄':11, '签到日期':'2023-01-11'}
 line2 = {'姓名': '小二', '年龄':12, '签到日期':'2023-01-12'}
 line3 = {'姓名': '小三', '年龄':13, '签到日期':'2023-01-13'}
 line4 = {'姓名': '小四', '年龄':14, '签到日期':'2023-01-14'}
 line5 = {'姓名': '小五', '年龄':15, '签到日期':'2023-01-15'}
 line6 = {'姓名': '小六', '年龄':16, '签到日期':'2023-01-16'}
 
-await sheet.insert(line1)  # 单条添加
+await sheet.insert(line1)  # 添加1条数据
 await sheet.insert([ line2, line3, line4, line5, line6 ])  # 批量添加
 ```
 
 查询：
 
 ```python
 await sheet[:]  # 查询所有数据
@@ -92,36 +92,36 @@
 # 删除年龄大于10、且喜欢足球的第2条数据
 await sheet[mc.年龄>10][mc.爱好.re('足球')].delete()[2]
 
 # 删除所有数据
 await sheet.delete()[:]
 ```
 
-过滤器：
+比较运算：
 
 | **代码** |
 | -------------- |
 | mc.年龄 > 10   |
 | mc.年龄 >= 10  |
 | mc.年龄 < 10   |
 | ...            |
 
+成员运算：
+
 | **代码**               | **解释**                   |
 | ---------------------------- | -------------------------------- |
 | mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
 | mc.年级.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
 
-| **代码**   |
-| ---------------- |
-| mc.姓名.re('小') |
+过滤器的集合运算：
 
 | **代码**                                                                  | **解释** |
 | ------------------------------------------------------------------------------- | -------------- |
 | [ mc.年龄>3 ][ mc.年龄<100 ]                                                    | 交集           |
-| [ (mc.年龄==30)&#124; (mc.年龄>30) &#124; (mc.年龄<30) &#124; (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄==30) \| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集           |
 | [ (mc.年龄>3) - (mc.年龄>100) ]                                                 | 差集           |
 | [ ~(mc.年龄>100) ]                                                              | 补集           |
 
 只返回姓名、年龄这2个字段：
 
 ```python
 await sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
@@ -129,51 +129,14 @@
 
 优先按年龄降序，其次按姓名升序，排序后返回第2~4条数据：
 
 ```python
 await sheet[mc.年龄>12].order(年龄=False, 姓名=True)[2:4]
 ```
 
-统计：
-
-| **项目**  | **语法**                 | **返回**                                          |
-| --------------- | ------------------------------ | ------------------------------------------------------- |
-| 主键            | await sheet.getPK( )           | 'id'                                                    |
-| 所有字段        | await sheet.getColumns( )      | [{'name':'id', 'comment':'', 'type':'int'}, {...}, ...] |
-| 数据总量        | await sheet.len( )             | 0                                                       |
-| 年龄>10的数据量 | await sheet[mc.年龄>10].len( ) | 0                                                       |
-
-orm（账户ORM）：
-
-| **功能**   | **语法**          | **返回**                                                         |
-| ---------------- | ----------------------- | ---------------------------------------------------------------------- |
-| 获取所有库的名称 | await orm.getDbNames( ) | ['information_schema', 'mysql', 'performance_schema', 'sys', '泉州市'] |
-| 统计库的数量     | await orm.len( )        | 5                                                                      |
-
-db（库ORM）：
-
-| **功能**   | **语法**            | **返回** |
-| ---------------- | ------------------------- | -------------- |
-| 获取所有表的名称 | await db.getSheetNames( ) | ['希望小学']   |
-| 统计表的数量     | await db.len( )           | 1              |
-
-调用mysql函数：
-
-```python
-# 在查询、删除、修改的条件中使用
-await sheet[mf.year('签到日期') == 2023][:]
-await sheet[mf.year('签到日期') == 2029].delete()[:]
-await sheet[mf.year('签到日期') == 2023].update({'性别':'女'})[2:5]
-
-# 在修改中使用
-await sheet.update({'备注': '签到日期'})[:]  # 修改为'签到日期'这个字符串
-await sheet.update({'备注': mc.签到日期})[:]  # 修改为各自的'签到日期'字段的值
-await sheet.update({'备注': mf.year('签到日期')})[:]  # 修改为各自的'签到日期'字段的值经year处理后的值
-```
-
 执行原生SQL语句：
 
 ```python
 data, cursor = await sheet.execute('select 姓名 from 希望小学 limit 1')
 data
 # >>> [{'姓名': '小一'}]
 
@@ -187,7 +150,15 @@
 
 sql = 'insert into 希望小学(姓名, 年龄) values (%s, %s)'
 students = [('小七', 17), ('小八', 18)]
 data, cursor = await sheet.executemany(sql, students)
 cursor.lastrowid
 # >>> 8
 ```
+
+# 支持作者1元
+
+asymysql 是一个免费的开源项目，由个人维护。
+
+每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
+
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
```

### Comparing `asymysql-1.2/pyproject.toml` & `asymysql-1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymysql"
-version = "1.2"
+version = "1.3"
 description = "异步的 mysql ORM"
-dependencies = ["aiomysql", "vtype", "coolfunc"]
+dependencies = ["lccpy >=1.3"]
 keywords = ["asymysql", "aiomysql", "mysql", "pymysql"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
+requires-python = ">=3.7"
 
 [project.urls]
-Documentation = "https://github.com/lcctoor/lccpy/blob/main/asymysql/docs/doc.md"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/asymysql"
```

### Comparing `asymysql-1.2/PKG-INFO` & `asymysql-1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: asymysql
-Version: 1.2
+Version: 1.3
 Summary: 异步的 mysql ORM
 Keywords: asymysql,aiomysql,mysql,pymysql
 Author-email: 许灿标 <lcctoor@outlook.com>
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: aiomysql
-Requires-Dist: vtype
-Requires-Dist: coolfunc
-Project-URL: Documentation, https://github.com/lcctoor/lccpy/blob/main/asymysql/docs/doc.md
+Requires-Dist: lccpy >=1.3
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/asymysql
 
 # 项目描述
 
 异步的 mysql ORM 。
 
-# 安装与文档
+# 安装与教程
 
 安装：`pip install asymysql`
 
-[文档](https://github.com/lcctoor/lccpy/blob/main/asymysql/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/asymysql/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
 
@@ -31,15 +30,15 @@
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
 开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
 
-# 语法预览
+# 教程预览
 
 导入：
 
 ```python
 from aiomysql import connect
 from asymysql import ORM, mc, mf
 ```
@@ -66,15 +65,15 @@
 line1 = {'姓名': '小一', '年龄':11, '签到日期':'2023-01-11'}
 line2 = {'姓名': '小二', '年龄':12, '签到日期':'2023-01-12'}
 line3 = {'姓名': '小三', '年龄':13, '签到日期':'2023-01-13'}
 line4 = {'姓名': '小四', '年龄':14, '签到日期':'2023-01-14'}
 line5 = {'姓名': '小五', '年龄':15, '签到日期':'2023-01-15'}
 line6 = {'姓名': '小六', '年龄':16, '签到日期':'2023-01-16'}
 
-await sheet.insert(line1)  # 单条添加
+await sheet.insert(line1)  # 添加1条数据
 await sheet.insert([ line2, line3, line4, line5, line6 ])  # 批量添加
 ```
 
 查询：
 
 ```python
 await sheet[:]  # 查询所有数据
@@ -105,36 +104,36 @@
 # 删除年龄大于10、且喜欢足球的第2条数据
 await sheet[mc.年龄>10][mc.爱好.re('足球')].delete()[2]
 
 # 删除所有数据
 await sheet.delete()[:]
 ```
 
-过滤器：
+比较运算：
 
 | **代码** |
 | -------------- |
 | mc.年龄 > 10   |
 | mc.年龄 >= 10  |
 | mc.年龄 < 10   |
 | ...            |
 
+成员运算：
+
 | **代码**               | **解释**                   |
 | ---------------------------- | -------------------------------- |
 | mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
 | mc.年级.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
 
-| **代码**   |
-| ---------------- |
-| mc.姓名.re('小') |
+过滤器的集合运算：
 
 | **代码**                                                                  | **解释** |
 | ------------------------------------------------------------------------------- | -------------- |
 | [ mc.年龄>3 ][ mc.年龄<100 ]                                                    | 交集           |
-| [ (mc.年龄==30)&#124; (mc.年龄>30) &#124; (mc.年龄<30) &#124; (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄==30) \| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集           |
 | [ (mc.年龄>3) - (mc.年龄>100) ]                                                 | 差集           |
 | [ ~(mc.年龄>100) ]                                                              | 补集           |
 
 只返回姓名、年龄这2个字段：
 
 ```python
 await sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
@@ -142,51 +141,14 @@
 
 优先按年龄降序，其次按姓名升序，排序后返回第2~4条数据：
 
 ```python
 await sheet[mc.年龄>12].order(年龄=False, 姓名=True)[2:4]
 ```
 
-统计：
-
-| **项目**  | **语法**                 | **返回**                                          |
-| --------------- | ------------------------------ | ------------------------------------------------------- |
-| 主键            | await sheet.getPK( )           | 'id'                                                    |
-| 所有字段        | await sheet.getColumns( )      | [{'name':'id', 'comment':'', 'type':'int'}, {...}, ...] |
-| 数据总量        | await sheet.len( )             | 0                                                       |
-| 年龄>10的数据量 | await sheet[mc.年龄>10].len( ) | 0                                                       |
-
-orm（账户ORM）：
-
-| **功能**   | **语法**          | **返回**                                                         |
-| ---------------- | ----------------------- | ---------------------------------------------------------------------- |
-| 获取所有库的名称 | await orm.getDbNames( ) | ['information_schema', 'mysql', 'performance_schema', 'sys', '泉州市'] |
-| 统计库的数量     | await orm.len( )        | 5                                                                      |
-
-db（库ORM）：
-
-| **功能**   | **语法**            | **返回** |
-| ---------------- | ------------------------- | -------------- |
-| 获取所有表的名称 | await db.getSheetNames( ) | ['希望小学']   |
-| 统计表的数量     | await db.len( )           | 1              |
-
-调用mysql函数：
-
-```python
-# 在查询、删除、修改的条件中使用
-await sheet[mf.year('签到日期') == 2023][:]
-await sheet[mf.year('签到日期') == 2029].delete()[:]
-await sheet[mf.year('签到日期') == 2023].update({'性别':'女'})[2:5]
-
-# 在修改中使用
-await sheet.update({'备注': '签到日期'})[:]  # 修改为'签到日期'这个字符串
-await sheet.update({'备注': mc.签到日期})[:]  # 修改为各自的'签到日期'字段的值
-await sheet.update({'备注': mf.year('签到日期')})[:]  # 修改为各自的'签到日期'字段的值经year处理后的值
-```
-
 执行原生SQL语句：
 
 ```python
 data, cursor = await sheet.execute('select 姓名 from 希望小学 limit 1')
 data
 # >>> [{'姓名': '小一'}]
 
@@ -201,7 +163,14 @@
 sql = 'insert into 希望小学(姓名, 年龄) values (%s, %s)'
 students = [('小七', 17), ('小八', 18)]
 data, cursor = await sheet.executemany(sql, students)
 cursor.lastrowid
 # >>> 8
 ```
 
+# 支持作者1元
+
+asymysql 是一个免费的开源项目，由个人维护。
+
+每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
+
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
```

