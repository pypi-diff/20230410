# Comparing `tmp/ats_case-0.3.0.tar.gz` & `tmp/ats_case-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.3.0.tar", last modified: Fri Apr  7 01:45:58 2023, max compression
+gzip compressed data, was "ats_case-0.4.0.tar", last modified: Mon Apr 10 01:57:22 2023, max compression
```

## Comparing `ats_case-0.3.0.tar` & `ats_case-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 01:45:58.006032 ats_case-0.3.0/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.3.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-07 01:45:58.003041 ats_case-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 01:45:57.631967 ats_case-0.3.0/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.3.0/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 01:45:57.841351 ats_case-0.3.0/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.3.0/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    16892 2023-04-07 01:45:37.000000 ats_case-0.3.0/ats_case/case/command.py
--rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.3.0/ats_case/case/context.py
--rw-rw-rw-   0        0        0     4644 2023-04-07 01:42:05.000000 ats_case-0.3.0/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5448 2023-04-07 01:42:16.000000 ats_case-0.3.0/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-07 01:45:57.901303 ats_case-0.3.0/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.3.0/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      366 2023-02-21 08:40:11.000000 ats_case-0.3.0/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      203 2023-02-11 01:58:18.000000 ats_case-0.3.0/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-07 01:45:57.957111 ats_case-0.3.0/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.3.0/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.3.0/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2597 2023-04-07 01:42:53.000000 ats_case-0.3.0/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-07 01:45:57.995109 ats_case-0.3.0/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.3.0/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-02-23 05:48:08.000000 ats_case-0.3.0/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-07 01:45:57.734673 ats_case-0.3.0/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-07 01:45:57.000000 ats_case-0.3.0/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-07 01:45:57.000000 ats_case-0.3.0/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 01:45:57.000000 ats_case-0.3.0/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-07 01:45:57.000000 ats_case-0.3.0/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 01:45:57.000000 ats_case-0.3.0/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 01:45:58.006032 ats_case-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-04-07 01:44:02.000000 ats_case-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:57:22.018436 ats_case-0.4.0/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-10 01:57:22.014444 ats_case-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.455945 ats_case-0.4.0/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.0/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.738186 ats_case-0.4.0/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.0/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17006 2023-04-10 01:53:21.000000 ats_case-0.4.0/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.0/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     4644 2023-04-07 01:42:05.000000 ats_case-0.4.0/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5448 2023-04-07 01:42:16.000000 ats_case-0.4.0/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.851879 ats_case-0.4.0/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.0/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      366 2023-02-21 08:40:11.000000 ats_case-0.4.0/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      203 2023-02-11 01:58:18.000000 ats_case-0.4.0/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.935655 ats_case-0.4.0/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.0/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.0/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2584 2023-04-10 01:54:51.000000 ats_case-0.4.0/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.990506 ats_case-0.4.0/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.0/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-02-23 05:48:08.000000 ats_case-0.4.0/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.577618 ats_case-0.4.0/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 01:57:22.018436 ats_case-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      916 2023-04-10 01:56:57.000000 ats_case-0.4.0/setup.py
```

### Comparing `ats_case-0.3.0/PKG-INFO` & `ats_case-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.3.0
+Version: 0.4.0
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.3.0/README.md` & `ats_case-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.3.0/ats_case/case/command.py` & `ats_case-0.4.0/ats_case/case/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,23 +209,23 @@
                                                                                       self._operation,
                                                                                       self._element))
         if type(self._parameter) is dict:
             self._parameter = _replace(context, self._parameter)
 
         parse = pro.encode(func.to_dict(protocol=self._protocol.name, comm_addr=self._comm_addr,
                                         operation=self._operation, element=self._element, parameter=self._parameter,
-                                        addition=self._addition, security=self._security))
+                                        addition=self._addition, security=self._security, session_key=context.session.basename))
         logger.info('~ @PRO-ENCODE<- protocol:{} frame:{}'.format(self._protocol, parse.get('frame')))
 
         self._frame = parse.get('frame')
         return self._frame
 
     def decode(self, context: Context):
         logger.info('~ @PRO-DECODE-> protocol:{} frame:{}'.format(self._protocol, self._frame))
-        data = pro.decode(func.to_dict(protocol=self._protocol.name, frame=self._frame))
+        data = pro.decode(func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
         logger.info('~ @PRO-DECODE<- protocol:{} parse:{}'.format(self._protocol, data))
 
         self._handle_framing(context, data)
 
         self._parse = data.get('parse').get('link_data').get('mission').get('result')
         return self._parse
 
@@ -239,15 +239,15 @@
             part_frame = data['parse']['session']['part_frame']
             pfs = context.session.set('part_frame', str(index), part_frame)
 
             result = send(context,
                           todo={
                               'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': next_frame}})
             self._frame = result.get('result')
-            data = pro.decode(func.to_dict(protocol=self._protocol.name, frame=self._frame))
+            data = pro.decode(func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
 
             self.handle_framing(context, data, index + 1)
 
     def _flush(self, context: Context):
         context.runtime.steps.update({context.runtime.step: func.to_dict(obj='meter', op=self._operation
                                                                          , element=self._element
                                                                          , parameter=self._parameter,
```

### Comparing `ats_case-0.3.0/ats_case/case/context.py` & `ats_case-0.4.0/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.3.0/ats_case/case/executor.py` & `ats_case-0.4.0/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.3.0/ats_case/case/translator.py` & `ats_case-0.4.0/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.3.0/ats_case/manage/core.py` & `ats_case-0.4.0/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.3.0/ats_case/manage/start.py` & `ats_case-0.4.0/ats_case/manage/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def _save(self):
         pass
 
     def _build(self, work_mode: WorkMode, code: str = None):
         if code is None:
             code = 'case'
 
-        user_dir = func.makeDir(os.environ.get('PROJECT_DIR'), 'testcase', work_mode.value.lower(), self._username)
+        user_dir = func.makeDir(os.getenv('PWD'), 'testcase', work_mode.value.lower(), self._username)
         template_file = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'template', 'testcase_v1.tmp')
         script_file = os.path.join(user_dir, 'test_{}.py'.format(code))
 
         with open(template_file, 'r', encoding='UTF-8') as file:
             content = file.read()
             content = content.replace('{script}', code.upper())
         with open(script_file, 'w', encoding='UTF-8') as file:
```

### Comparing `ats_case-0.3.0/ats_case/template/testcase_v1.tmp` & `ats_case-0.4.0/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.3.0/ats_case.egg-info/PKG-INFO` & `ats_case-0.4.0/ats_case.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.3.0
+Version: 0.4.0
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.3.0/ats_case.egg-info/SOURCES.txt` & `ats_case-0.4.0/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.3.0/setup.py` & `ats_case-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.3.0",
+    version="0.4.0",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

