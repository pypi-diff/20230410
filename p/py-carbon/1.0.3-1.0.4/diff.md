# Comparing `tmp/py-carbon-1.0.3.tar.gz` & `tmp/py-carbon-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-carbon-1.0.3.tar", last modified: Mon Apr 18 18:15:44 2022, max compression
+gzip compressed data, was "py-carbon-1.0.4.tar", last modified: Mon Apr 10 13:01:45 2023, max compression
```

## Comparing `py-carbon-1.0.3.tar` & `py-carbon-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-04-18 18:15:44.900366 py-carbon-1.0.3/
--rw-rw-rw-   0        0        0     1084 2021-05-29 19:45:14.000000 py-carbon-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2192 2022-04-18 18:15:44.898366 py-carbon-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2022-04-18 17:56:32.000000 py-carbon-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-04-18 18:15:44.879407 py-carbon-1.0.3/carbon/
--rw-rw-rw-   0        0        0      889 2022-04-18 17:57:28.000000 py-carbon-1.0.3/carbon/__init__.py
--rw-rw-rw-   0        0        0     2770 2022-04-18 17:56:31.000000 py-carbon-1.0.3/carbon/carbon.py
--rw-rw-rw-   0        0        0     1208 2021-05-29 21:06:14.000000 py-carbon-1.0.3/carbon/errors.py
--rw-rw-rw-   0        0        0     4607 2021-05-30 13:20:13.000000 py-carbon-1.0.3/carbon/opts.py
--rw-rw-rw-   0        0        0     1807 2021-05-29 20:24:10.000000 py-carbon-1.0.3/carbon/utils.py
-drwxrwxrwx   0        0        0        0 2022-04-18 18:15:44.894367 py-carbon-1.0.3/py_carbon.egg-info/
--rw-rw-rw-   0        0        0     2192 2022-04-18 18:15:44.000000 py-carbon-1.0.3/py_carbon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2022-04-18 18:15:44.000000 py-carbon-1.0.3/py_carbon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-18 18:15:44.000000 py-carbon-1.0.3/py_carbon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-04-18 18:15:44.000000 py-carbon-1.0.3/py_carbon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-05-30 13:25:10.000000 py-carbon-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-18 18:15:44.901370 py-carbon-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1034 2022-04-18 18:15:17.000000 py-carbon-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 13:01:45.060228 py-carbon-1.0.4/
+-rw-rw-rw-   0        0        0     1084 2021-05-29 19:45:14.000000 py-carbon-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2199 2023-04-10 13:01:45.057707 py-carbon-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1776 2023-04-10 12:57:43.000000 py-carbon-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 13:01:45.041156 py-carbon-1.0.4/carbon/
+-rw-rw-rw-   0        0        0      888 2023-04-10 12:56:13.000000 py-carbon-1.0.4/carbon/__init__.py
+-rw-rw-rw-   0        0        0     2764 2023-04-10 12:52:57.000000 py-carbon-1.0.4/carbon/carbon.py
+-rw-rw-rw-   0        0        0     1208 2021-05-29 21:06:14.000000 py-carbon-1.0.4/carbon/errors.py
+-rw-rw-rw-   0        0        0     4607 2021-05-30 13:20:13.000000 py-carbon-1.0.4/carbon/opts.py
+-rw-rw-rw-   0        0        0     1828 2023-04-10 12:52:57.000000 py-carbon-1.0.4/carbon/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 13:01:45.054434 py-carbon-1.0.4/py_carbon.egg-info/
+-rw-rw-rw-   0        0        0     2199 2023-04-10 13:01:44.000000 py-carbon-1.0.4/py_carbon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-10 13:01:45.000000 py-carbon-1.0.4/py_carbon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 13:01:44.000000 py-carbon-1.0.4/py_carbon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 13:01:44.000000 py-carbon-1.0.4/py_carbon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-05-30 13:25:10.000000 py-carbon-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 13:01:45.060228 py-carbon-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-04-10 12:56:13.000000 py-carbon-1.0.4/setup.py
```

### Comparing `py-carbon-1.0.3/LICENSE` & `py-carbon-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-carbon-1.0.3/PKG-INFO` & `py-carbon-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: py-carbon
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fully asynchronous Python library for carbon.now.sh
 Home-page: https://github.com/itsmewulf/py-carbon
-Author: statch
-Author-email: paul@przybyszewski.me
+Author: wulf
+Author-email: paul@przybyszew.ski
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-carbon [![Badge](https://img.shields.io/pypi/v/py-carbon?color=3776AB&logo=python&style=for-the-badge)](https://pypi.org/project/py-carbon/)  [![Badge 2](https://img.shields.io/pypi/dm/py-carbon?color=3776AB&logo=python&style=for-the-badge)](https://pypi.org/project/py-carbon/)
@@ -23,29 +22,31 @@
 
 ## A quick example
 In this example we'll create a carbon image and save it to disk.
 ```py
 import carbon
 import asyncio
 
-loop = asyncio.get_event_loop()  # Setting up asyncio
-
 code = """
 defmodule Something do
     def anything() do
         IO.puts "Hello, World"
     end
 end
 """  # Any kind of code-block in any language
 
-options = carbon.CarbonOptions(code)
 
-cb = carbon.Carbon()
-image = loop.run_until_complete(cb.generate(options))  # Returns a CarbonImage object
-loop.run_until_complete(image.save('something-script'))
+async def main():
+    cb = carbon.Carbon()  # Create a Carbon instance
+    opts = carbon.CarbonOptions(code=code)  # Set the options for the image
+    image = await cb.generate(opts)  # Generate the image
+    await image.save('hello')  # Save the image in png format
+
+
+asyncio.run(main())
 ```
 
 And it'll output something like this:  
   
 <img src="https://github.com/itsmewulf/py-carbon/blob/main/examples/something-script.png?raw=true" alt="Carbon Image" width="400"/>
 
 ### Contributing
@@ -56,11 +57,9 @@
 it [here.](https://github.com/itsmewulf/py-carbon/issues)
 
 ### Fixing/Editing Content
 If you want to contribute to this package, fork the repository, make your changes and then simply create a Pull Request!
 
 ### Contact
 If you want to contact me:  
-**Mail -** ```paul@przybyszewski.me```  
+**Mail -** ```paul@przybyszew.ski```  
 **Discord -** [wulf](https://dsc.bio/wulf)
-
-
```

### Comparing `py-carbon-1.0.3/README.md` & `py-carbon-1.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 
 ## A quick example
 In this example we'll create a carbon image and save it to disk.
 ```py
 import carbon
 import asyncio
 
-loop = asyncio.get_event_loop()  # Setting up asyncio
-
 code = """
 defmodule Something do
     def anything() do
         IO.puts "Hello, World"
     end
 end
 """  # Any kind of code-block in any language
 
-options = carbon.CarbonOptions(code)
 
-cb = carbon.Carbon()
-image = loop.run_until_complete(cb.generate(options))  # Returns a CarbonImage object
-loop.run_until_complete(image.save('something-script'))
+async def main():
+    cb = carbon.Carbon()  # Create a Carbon instance
+    opts = carbon.CarbonOptions(code=code)  # Set the options for the image
+    image = await cb.generate(opts)  # Generate the image
+    await image.save('hello')  # Save the image in png format
+
+
+asyncio.run(main())
 ```
 
 And it'll output something like this:  
   
 <img src="https://github.com/itsmewulf/py-carbon/blob/main/examples/something-script.png?raw=true" alt="Carbon Image" width="400"/>
 
 ### Contributing
@@ -41,9 +43,9 @@
 it [here.](https://github.com/itsmewulf/py-carbon/issues)
 
 ### Fixing/Editing Content
 If you want to contribute to this package, fork the repository, make your changes and then simply create a Pull Request!
 
 ### Contact
 If you want to contact me:  
-**Mail -** ```paul@przybyszewski.me```  
+**Mail -** ```paul@przybyszew.ski```  
 **Discord -** [wulf](https://dsc.bio/wulf)
```

### Comparing `py-carbon-1.0.3/carbon/__init__.py` & `py-carbon-1.0.4/carbon/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from . import utils
 from .carbon import *
 from .errors import CarbonError
 from .opts import *
 
 VersionInfo = namedtuple('VersionInfo', 'major minor micro releaselevel serial')
 
-version_info = VersionInfo(major=1, minor=0, micro=3, releaselevel='final', serial=0)
+version_info = VersionInfo(major=1, minor=0, micro=4, releaselevel='final', serial=0)
 
 __version__ = f'{version_info.major}.{version_info.minor}.{version_info.micro}'
 __title__ = 'py-carbon'
 __license__ = 'MIT'
 __author__ = 'wulf'
-__email__ = 'paul@przybyszewski.me'
+__email__ = 'paul@przybyszew.skie'
 __uri__ = "https://github.com/statch/py-carbon"
-__copyright__ = 'Copyright 2021-2022 %s' % __author__
+__copyright__ = 'Copyright 2021-2023 %s' % __author__
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
```

### Comparing `py-carbon-1.0.3/carbon/carbon.py` & `py-carbon-1.0.4/carbon/carbon.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,26 @@
         self.bytes: bytes = _bytes
 
     async def save(self, filename: str) -> AnyStr:
         async with aiofiles.open(sanitize_filename(filename), 'wb') as fp:
             await fp.write(self.bytes)
         return os.path.realpath(filename)
 
-    async def memorize(self, filename: Optional[str] = None) -> io.BytesIO:
+    async def memoize(self, filename: Optional[str] = None) -> io.BytesIO:
         io_obj: io.BytesIO = io.BytesIO(self.bytes)
         if filename:
             setattr(io_obj, 'name', sanitize_filename(filename))
         return io_obj
 
     def __bytes__(self) -> bytes:
         return self.bytes
 
 
 class Carbon:
-    __url__: str = 'https://carbonara-42.herokuapp.com/api/cook'
+    __url__: str = 'https://carbonara.solopov.dev/api/cook'
 
     def __init__(self, session: Optional[aiohttp.ClientSession] = None):
         self._ses: aiohttp.ClientSession = session or aiohttp.ClientSession()
 
     async def generate(self, options: CarbonOptions) -> CarbonImage:
         res: aiohttp.ClientResponse = await self._ses.post(self.__url__,
                                                            json=options.request_format(),
```

### Comparing `py-carbon-1.0.3/carbon/errors.py` & `py-carbon-1.0.4/carbon/errors.py`

 * *Files identical despite different names*

### Comparing `py-carbon-1.0.3/carbon/opts.py` & `py-carbon-1.0.4/carbon/opts.py`

 * *Files identical despite different names*

### Comparing `py-carbon-1.0.3/carbon/utils.py` & `py-carbon-1.0.4/carbon/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,7 +54,8 @@
 
 
 def sanitize_filename(filename: str) -> str:
     if not filename.endswith('.png'):
         if '.' in filename:
             return filename[:filename.rindex('.', 1)] + '.png'
         return filename + '.png'
+    return filename
```

### Comparing `py-carbon-1.0.3/py_carbon.egg-info/PKG-INFO` & `py-carbon-1.0.4/py_carbon.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: py-carbon
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fully asynchronous Python library for carbon.now.sh
 Home-page: https://github.com/itsmewulf/py-carbon
-Author: statch
-Author-email: paul@przybyszewski.me
+Author: wulf
+Author-email: paul@przybyszew.ski
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-carbon [![Badge](https://img.shields.io/pypi/v/py-carbon?color=3776AB&logo=python&style=for-the-badge)](https://pypi.org/project/py-carbon/)  [![Badge 2](https://img.shields.io/pypi/dm/py-carbon?color=3776AB&logo=python&style=for-the-badge)](https://pypi.org/project/py-carbon/)
@@ -23,29 +22,31 @@
 
 ## A quick example
 In this example we'll create a carbon image and save it to disk.
 ```py
 import carbon
 import asyncio
 
-loop = asyncio.get_event_loop()  # Setting up asyncio
-
 code = """
 defmodule Something do
     def anything() do
         IO.puts "Hello, World"
     end
 end
 """  # Any kind of code-block in any language
 
-options = carbon.CarbonOptions(code)
 
-cb = carbon.Carbon()
-image = loop.run_until_complete(cb.generate(options))  # Returns a CarbonImage object
-loop.run_until_complete(image.save('something-script'))
+async def main():
+    cb = carbon.Carbon()  # Create a Carbon instance
+    opts = carbon.CarbonOptions(code=code)  # Set the options for the image
+    image = await cb.generate(opts)  # Generate the image
+    await image.save('hello')  # Save the image in png format
+
+
+asyncio.run(main())
 ```
 
 And it'll output something like this:  
   
 <img src="https://github.com/itsmewulf/py-carbon/blob/main/examples/something-script.png?raw=true" alt="Carbon Image" width="400"/>
 
 ### Contributing
@@ -56,11 +57,9 @@
 it [here.](https://github.com/itsmewulf/py-carbon/issues)
 
 ### Fixing/Editing Content
 If you want to contribute to this package, fork the repository, make your changes and then simply create a Pull Request!
 
 ### Contact
 If you want to contact me:  
-**Mail -** ```paul@przybyszewski.me```  
+**Mail -** ```paul@przybyszew.ski```  
 **Discord -** [wulf](https://dsc.bio/wulf)
-
-
```

### Comparing `py-carbon-1.0.3/setup.py` & `py-carbon-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     name='py-carbon',
     version=version,
     description='Fully asynchronous Python library for carbon.now.sh',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     license='MIT',
-    author='statch',
-    author_email='paul@przybyszewski.me',
+    author='wulf',
+    author_email='paul@przybyszew.ski',
     url='https://github.com/itsmewulf/py-carbon',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License'
     ],
     python_requires='>=3.9',
```

