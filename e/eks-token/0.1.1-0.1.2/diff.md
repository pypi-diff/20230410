# Comparing `tmp/eks_token-0.1.1.tar.gz` & `tmp/eks_token-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eks_token-0.1.1.tar", last modified: Wed Mar 10 08:59:44 2021, max compression
+gzip compressed data, was "eks_token-0.1.2.tar", last modified: Mon Apr 10 05:35:50 2023, max compression
```

## Comparing `eks_token-0.1.1.tar` & `eks_token-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 08:59:44.781589 eks_token-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2021-03-10 08:59:44.781589 eks_token-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2021-03-10 08:59:31.000000 eks_token-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 08:59:44.781589 eks_token-0.1.1/eks_token/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-03-10 08:59:31.000000 eks_token-0.1.1/eks_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2021-03-10 08:59:31.000000 eks_token-0.1.1/eks_token/logics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 08:59:44.781589 eks_token-0.1.1/eks_token.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2021-03-10 08:59:44.000000 eks_token-0.1.1/eks_token.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-03-10 08:59:44.000000 eks_token-0.1.1/eks_token.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-10 08:59:44.000000 eks_token-0.1.1/eks_token.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-10 08:59:44.000000 eks_token-0.1.1/eks_token.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-10 08:59:44.000000 eks_token-0.1.1/eks_token.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-10 08:59:44.781589 eks_token-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      715 2021-03-10 08:59:31.000000 eks_token-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:35:50.572330 eks_token-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-10 05:35:37.000000 eks_token-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-10 05:35:50.572330 eks_token-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-10 05:35:37.000000 eks_token-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:35:50.568329 eks_token-0.1.2/eks_token/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 05:35:37.000000 eks_token-0.1.2/eks_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-10 05:35:37.000000 eks_token-0.1.2/eks_token/logics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:35:50.572330 eks_token-0.1.2/eks_token.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-10 05:35:50.000000 eks_token-0.1.2/eks_token.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-10 05:35:50.000000 eks_token-0.1.2/eks_token.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 05:35:50.000000 eks_token-0.1.2/eks_token.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 05:35:50.000000 eks_token-0.1.2/eks_token.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 05:35:50.000000 eks_token-0.1.2/eks_token.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 05:35:50.572330 eks_token-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-10 05:35:37.000000 eks_token-0.1.2/setup.py
```

### Comparing `eks_token-0.1.1/PKG-INFO` & `eks_token-0.1.2/eks_token.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 Metadata-Version: 2.1
-Name: eks_token
-Version: 0.1.1
+Name: eks-token
+Version: 0.1.2
 Summary: EKS Token package, an alternate to "aws eks get-token ..." CLI
 Home-page: https://github.com/peak-ai/eks-token
 Author: Peak AI
 Author-email: support@peak.ai
-License: UNKNOWN
-Description: # eks-token
-        EKS Token package, an alternate to "aws eks get-token ..." CLI
-        
-        ![CodeQuality](https://github.com/peak-ai/eks-token/workflows/CodeQL/badge.svg) ![Publish](https://github.com/peak-ai/eks-token/workflows/Upload%20Python%20Package/badge.svg) ![stable](https://img.shields.io/github/v/release/peak-ai/eks-token) ![](https://img.shields.io/github/v/release/peak-ai/eks-token?include_prereleases) ![](https://img.shields.io/github/license/peak-ai/eks-token) ![](https://img.shields.io/github/languages/count/peak-ai/eks-token) ![](https://img.shields.io/github/languages/top/peak-ai/eks-token) ![](https://img.shields.io/github/issues-raw/peak-ai/eks-token) ![](https://img.shields.io/github/issues-pr-raw/peak-ai/eks-token) ![](https://img.shields.io/github/languages/code-size/peak-ai/eks-token) ![](https://img.shields.io/github/repo-size/peak-ai/eks-token)
-        
-        ![logo](https://raw.githubusercontent.com/peak-ai/eks-token/master/eks-iam.png)
-        
-        ## Usage
-        
-        ### Installation
-        
-        ```shell
-        pip install eks-token
-        ```
-        
-        ### Basic usage
-        
-        ```python
-        from eks_token import get_token
-        from pprint import pprint
-        
-        response = get_token(cluster_name='<value>')
-        pprint(response)
-        ```
-        Expected Output
-        ```python
-        {'apiVersion': 'client.authentication.k8s.io/v1alpha1',
-         'kind': 'ExecCredential',
-         'spec': {},
-         'status': {'expirationTimestamp': '2020-10-01T15:05:17Z',
-                    'token': 'k8s-aws-v1.<token_value>'}}
-        ```
-        
-        ### Extract token from response
-        
-        ```python
-        from eks_token import get_token
-        
-        token = get_token(cluster_name='value')['status']['token']
-        print(token)
-        ```
-        
-        ### Get Token signed for particular IAM role
-        
-        Pass `role_arn`  argument to the function
-        ```python
-        from eks_token import get_token
-        
-        token = get_token(cluster_name='<value>', role_arn='<value>')['status']['token']
-        print(token)
-        ```
-        
-        ## Contribution
-        Check our guidelines [here](CONTRIBUTING.md)
-        
 Keywords: eks k8s boto3 awscli python aws
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# eks-token
+EKS Token package, an alternate to "aws eks get-token ..." CLI
+
+![CodeQuality](https://github.com/peak-ai/eks-token/workflows/CodeQL/badge.svg) ![Publish](https://github.com/peak-ai/eks-token/workflows/Upload%20Python%20Package/badge.svg) ![stable](https://img.shields.io/github/v/release/peak-ai/eks-token) ![](https://img.shields.io/github/v/release/peak-ai/eks-token?include_prereleases) ![](https://img.shields.io/github/license/peak-ai/eks-token) ![](https://img.shields.io/github/languages/count/peak-ai/eks-token) ![](https://img.shields.io/github/languages/top/peak-ai/eks-token) ![](https://img.shields.io/github/issues-raw/peak-ai/eks-token) ![](https://img.shields.io/github/issues-pr-raw/peak-ai/eks-token) ![](https://img.shields.io/github/languages/code-size/peak-ai/eks-token) ![](https://img.shields.io/github/repo-size/peak-ai/eks-token)
+
+![logo](https://raw.githubusercontent.com/peak-ai/eks-token/main/eks-iam.png)
+
+## Usage
+
+### Installation
+
+```shell
+pip install eks-token
+```
+
+### Basic usage
+
+```python
+from eks_token import get_token
+from pprint import pprint
+
+response = get_token(cluster_name='<value>')
+pprint(response)
+```
+Expected Output
+```python
+{'apiVersion': 'client.authentication.k8s.io/v1alpha1',
+ 'kind': 'ExecCredential',
+ 'spec': {},
+ 'status': {'expirationTimestamp': '2020-10-01T15:05:17Z',
+            'token': 'k8s-aws-v1.<token_value>'}}
+```
+
+### Extract token from response
+
+```python
+from eks_token import get_token
+
+token = get_token(cluster_name='value')['status']['token']
+print(token)
+```
+
+### Get Token signed for particular IAM role
+
+Pass `role_arn`  argument to the function
+```python
+from eks_token import get_token
+
+token = get_token(cluster_name='<value>', role_arn='<value>')['status']['token']
+print(token)
+```
+
+## Contribution
+Check our guidelines [here](CONTRIBUTING.md)
```

### Comparing `eks_token-0.1.1/README.md` & `eks_token-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # eks-token
 EKS Token package, an alternate to "aws eks get-token ..." CLI
 
 ![CodeQuality](https://github.com/peak-ai/eks-token/workflows/CodeQL/badge.svg) ![Publish](https://github.com/peak-ai/eks-token/workflows/Upload%20Python%20Package/badge.svg) ![stable](https://img.shields.io/github/v/release/peak-ai/eks-token) ![](https://img.shields.io/github/v/release/peak-ai/eks-token?include_prereleases) ![](https://img.shields.io/github/license/peak-ai/eks-token) ![](https://img.shields.io/github/languages/count/peak-ai/eks-token) ![](https://img.shields.io/github/languages/top/peak-ai/eks-token) ![](https://img.shields.io/github/issues-raw/peak-ai/eks-token) ![](https://img.shields.io/github/issues-pr-raw/peak-ai/eks-token) ![](https://img.shields.io/github/languages/code-size/peak-ai/eks-token) ![](https://img.shields.io/github/repo-size/peak-ai/eks-token)
 
-![logo](https://raw.githubusercontent.com/peak-ai/eks-token/master/eks-iam.png)
+![logo](https://raw.githubusercontent.com/peak-ai/eks-token/main/eks-iam.png)
 
 ## Usage
 
 ### Installation
 
 ```shell
 pip install eks-token
```

### Comparing `eks_token-0.1.1/eks_token/logics.py` & `eks_token-0.1.2/eks_token/logics.py`

 * *Files identical despite different names*

### Comparing `eks_token-0.1.1/eks_token.egg-info/PKG-INFO` & `eks_token-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 Metadata-Version: 2.1
-Name: eks-token
-Version: 0.1.1
+Name: eks_token
+Version: 0.1.2
 Summary: EKS Token package, an alternate to "aws eks get-token ..." CLI
 Home-page: https://github.com/peak-ai/eks-token
 Author: Peak AI
 Author-email: support@peak.ai
-License: UNKNOWN
-Description: # eks-token
-        EKS Token package, an alternate to "aws eks get-token ..." CLI
-        
-        ![CodeQuality](https://github.com/peak-ai/eks-token/workflows/CodeQL/badge.svg) ![Publish](https://github.com/peak-ai/eks-token/workflows/Upload%20Python%20Package/badge.svg) ![stable](https://img.shields.io/github/v/release/peak-ai/eks-token) ![](https://img.shields.io/github/v/release/peak-ai/eks-token?include_prereleases) ![](https://img.shields.io/github/license/peak-ai/eks-token) ![](https://img.shields.io/github/languages/count/peak-ai/eks-token) ![](https://img.shields.io/github/languages/top/peak-ai/eks-token) ![](https://img.shields.io/github/issues-raw/peak-ai/eks-token) ![](https://img.shields.io/github/issues-pr-raw/peak-ai/eks-token) ![](https://img.shields.io/github/languages/code-size/peak-ai/eks-token) ![](https://img.shields.io/github/repo-size/peak-ai/eks-token)
-        
-        ![logo](https://raw.githubusercontent.com/peak-ai/eks-token/master/eks-iam.png)
-        
-        ## Usage
-        
-        ### Installation
-        
-        ```shell
-        pip install eks-token
-        ```
-        
-        ### Basic usage
-        
-        ```python
-        from eks_token import get_token
-        from pprint import pprint
-        
-        response = get_token(cluster_name='<value>')
-        pprint(response)
-        ```
-        Expected Output
-        ```python
-        {'apiVersion': 'client.authentication.k8s.io/v1alpha1',
-         'kind': 'ExecCredential',
-         'spec': {},
-         'status': {'expirationTimestamp': '2020-10-01T15:05:17Z',
-                    'token': 'k8s-aws-v1.<token_value>'}}
-        ```
-        
-        ### Extract token from response
-        
-        ```python
-        from eks_token import get_token
-        
-        token = get_token(cluster_name='value')['status']['token']
-        print(token)
-        ```
-        
-        ### Get Token signed for particular IAM role
-        
-        Pass `role_arn`  argument to the function
-        ```python
-        from eks_token import get_token
-        
-        token = get_token(cluster_name='<value>', role_arn='<value>')['status']['token']
-        print(token)
-        ```
-        
-        ## Contribution
-        Check our guidelines [here](CONTRIBUTING.md)
-        
 Keywords: eks k8s boto3 awscli python aws
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# eks-token
+EKS Token package, an alternate to "aws eks get-token ..." CLI
+
+![CodeQuality](https://github.com/peak-ai/eks-token/workflows/CodeQL/badge.svg) ![Publish](https://github.com/peak-ai/eks-token/workflows/Upload%20Python%20Package/badge.svg) ![stable](https://img.shields.io/github/v/release/peak-ai/eks-token) ![](https://img.shields.io/github/v/release/peak-ai/eks-token?include_prereleases) ![](https://img.shields.io/github/license/peak-ai/eks-token) ![](https://img.shields.io/github/languages/count/peak-ai/eks-token) ![](https://img.shields.io/github/languages/top/peak-ai/eks-token) ![](https://img.shields.io/github/issues-raw/peak-ai/eks-token) ![](https://img.shields.io/github/issues-pr-raw/peak-ai/eks-token) ![](https://img.shields.io/github/languages/code-size/peak-ai/eks-token) ![](https://img.shields.io/github/repo-size/peak-ai/eks-token)
+
+![logo](https://raw.githubusercontent.com/peak-ai/eks-token/main/eks-iam.png)
+
+## Usage
+
+### Installation
+
+```shell
+pip install eks-token
+```
+
+### Basic usage
+
+```python
+from eks_token import get_token
+from pprint import pprint
+
+response = get_token(cluster_name='<value>')
+pprint(response)
+```
+Expected Output
+```python
+{'apiVersion': 'client.authentication.k8s.io/v1alpha1',
+ 'kind': 'ExecCredential',
+ 'spec': {},
+ 'status': {'expirationTimestamp': '2020-10-01T15:05:17Z',
+            'token': 'k8s-aws-v1.<token_value>'}}
+```
+
+### Extract token from response
+
+```python
+from eks_token import get_token
+
+token = get_token(cluster_name='value')['status']['token']
+print(token)
+```
+
+### Get Token signed for particular IAM role
+
+Pass `role_arn`  argument to the function
+```python
+from eks_token import get_token
+
+token = get_token(cluster_name='<value>', role_arn='<value>')['status']['token']
+print(token)
+```
+
+## Contribution
+Check our guidelines [here](CONTRIBUTING.md)
```

### Comparing `eks_token-0.1.1/setup.py` & `eks_token-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='eks_token',
-    version='0.1.1',
+    version='0.1.2',
     author='Peak AI',
     author_email='support@peak.ai',
     description='EKS Token package, an alternate to "aws eks get-token ..." CLI',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/peak-ai/eks-token',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     keywords='eks k8s boto3 awscli python aws',
-    install_requires=["awscli==1.18.150"],
+    install_requires=["awscli==1.27.8"],
 )
```

