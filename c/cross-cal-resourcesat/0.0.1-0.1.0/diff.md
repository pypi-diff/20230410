# Comparing `tmp/cross_cal_resourcesat-0.0.1.tar.gz` & `tmp/cross_cal_resourcesat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cross_cal_resourcesat-0.0.1.tar", last modified: Sun Apr  9 18:40:13 2023, max compression
+gzip compressed data, was "cross_cal_resourcesat-0.1.0.tar", last modified: Mon Apr 10 21:11:06 2023, max compression
```

## Comparing `cross_cal_resourcesat-0.0.1.tar` & `cross_cal_resourcesat-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 18:40:13.988977 cross_cal_resourcesat-0.0.1/
--rw-rw-rw-   0        0        0     1095 2023-04-09 17:18:12.000000 cross_cal_resourcesat-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-09 17:18:12.000000 cross_cal_resourcesat-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1595 2023-04-09 18:40:13.988977 cross_cal_resourcesat-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-04-09 17:18:12.000000 cross_cal_resourcesat-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 18:40:13.977680 cross_cal_resourcesat-0.0.1/cross_cal_resourcesat/
--rw-rw-rw-   0        0        0      149 2023-04-09 17:18:12.000000 cross_cal_resourcesat-0.0.1/cross_cal_resourcesat/__init__.py
--rw-rw-rw-   0        0        0       20 2023-04-09 17:18:12.000000 cross_cal_resourcesat-0.0.1/cross_cal_resourcesat/cross_cal_resourcesat.py
-drwxrwxrwx   0        0        0        0 2023-04-09 18:40:13.977680 cross_cal_resourcesat-0.0.1/cross_cal_resourcesat.egg-info/
--rw-rw-rw-   0        0        0     1595 2023-04-09 18:40:13.000000 cross_cal_resourcesat-0.0.1/cross_cal_resourcesat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-04-09 18:40:13.000000 cross_cal_resourcesat-0.0.1/cross_cal_resourcesat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 18:40:13.000000 cross_cal_resourcesat-0.0.1/cross_cal_resourcesat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 18:40:13.000000 cross_cal_resourcesat-0.0.1/cross_cal_resourcesat.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2023-04-09 18:40:13.000000 cross_cal_resourcesat-0.0.1/cross_cal_resourcesat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:12.000000 cross_cal_resourcesat-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      429 2023-04-09 18:40:13.990538 cross_cal_resourcesat-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1920 2023-04-09 17:18:12.000000 cross_cal_resourcesat-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:11:06.670409 cross_cal_resourcesat-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-10 21:11:06.670409 cross_cal_resourcesat-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:11:06.666409 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat/cross_cal_resourcesat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:11:06.670409 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-10 21:11:06.670409 cross_cal_resourcesat-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/setup.py
```

### Comparing `cross_cal_resourcesat-0.0.1/LICENSE` & `cross_cal_resourcesat-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Akhilesh Kumar
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Akhilesh Kumar
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `cross_cal_resourcesat-0.0.1/setup.py` & `cross_cal_resourcesat-0.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = [ ]
-
-test_requirements = [ ]
-
-setup(
-    author="Akhilesh Kumar",
-    author_email='akhiraj9661@gmail.com',
-    python_requires='>=3.7',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
-    description="A python package to cross calibrate ResourceSat 2 sensors like LISS III, AWiFS or LISS IV.",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='cross_cal_resourcesat',
-    name='cross_cal_resourcesat',
-    packages=find_packages(include=['cross_cal_resourcesat', 'cross_cal_resourcesat.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/akhi9661/cross_cal_resourcesat',
-    version='0.0.1',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = [ ]
+
+test_requirements = [ ]
+
+setup(
+    author="Akhilesh Kumar",
+    author_email='akhiraj9661@gmail.com',
+    python_requires='>=3.7',
+    classifiers=[
+        'Development Status :: 2 - Pre-Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+    ],
+    description="A python package to cross calibrate ResourceSat 2 sensors like LISS III, AWiFS or LISS IV.",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='cross_cal_resourcesat',
+    name='cross_cal_resourcesat',
+    packages=find_packages(include=['cross_cal_resourcesat', 'cross_cal_resourcesat.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/akhi9661/cross_cal_resourcesat',
+    version='0.1.0',
+    zip_safe=False,
+)
```

