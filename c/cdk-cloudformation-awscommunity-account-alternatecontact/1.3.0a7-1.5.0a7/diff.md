# Comparing `tmp/cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7.tar.gz` & `tmp/cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-account-alternatecontact/dist/python/cdk-c", last modified: Fri Feb  3 16:13:21 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-account-alternatecontact/dist/python/cdk-c", last modified: Mon Apr 10 06:14:10 2023, max compression
```

## Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7.tar` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:21.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-02-03 16:13:12.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-02-03 16:13:12.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3051 2023-02-03 16:13:21.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2108 2023-02-03 16:13:12.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      236 2023-02-03 16:13:12.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-02-03 16:13:21.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1970 2023-02-03 16:13:12.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:21.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:21.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11839 2023-02-03 16:13:12.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:21.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      490 2023-02-03 16:13:12.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    18450 2023-02-03 16:13:12.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/awscommunity-account-alternatecontact@1.3.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:13:12.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:21.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3051 2023-02-03 16:13:20.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      822 2023-02-03 16:13:20.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:13:20.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-02-03 16:13:20.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       57 2023-02-03 16:13:20.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-04-10 06:14:04.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-10 06:14:04.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3082 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2108 2023-04-10 06:14:04.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-04-10 06:14:04.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2020 2023-04-10 06:14:04.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11596 2023-04-10 06:14:04.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      490 2023-04-10 06:14:04.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    18351 2023-04-10 06:14:04.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/awscommunity-account-alternatecontact@1.5.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-10 06:14:04.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3082 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      822 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       57 2023-04-10 06:14:10.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/LICENSE` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/PKG-INFO` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-account-alternatecontact
-Version: 1.3.0a7
+Version: 1.5.0a7
 Summary: An alternate contact attached to an Amazon Web Services account.
 Home-page: https://github.com/aws-cloudformation/community-registry-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # awscommunity-account-alternatecontact
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.5.0.
 
 ## Description
 
 An alternate contact attached to an Amazon Web Services account.
 
 ## References
 
@@ -55,15 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Account::AlternateContact`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.5.0).
 * Issues related to `AwsCommunity::Account::AlternateContact` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/README.md` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # awscommunity-account-alternatecontact
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.5.0.
 
 ## Description
 
 An alternate contact attached to an Amazon Web Services account.
 
 ## References
 
@@ -32,13 +32,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Account::AlternateContact`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.5.0).
 * Issues related to `AwsCommunity::Account::AlternateContact` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/setup.py` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-awscommunity-account-alternatecontact",
-    "version": "1.3.0.a7",
+    "version": "1.5.0.a7",
     "description": "An alternate contact attached to an Amazon Web Services account.",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-cloudformation/community-registry-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_cloudformation_awscommunity_account_alternatecontact",
         "cdk_cloudformation_awscommunity_account_alternatecontact._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_awscommunity_account_alternatecontact._jsii": [
-            "awscommunity-account-alternatecontact@1.3.0-alpha.7.jsii.tgz"
+            "awscommunity-account-alternatecontact@1.5.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_awscommunity_account_alternatecontact": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.63.0, <3.0.0",
-        "constructs>=10.1.239, <11.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "aws-cdk-lib>=2.72.1, <3.0.0",
+        "constructs>=10.1.302, <11.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
 )
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/__init__.py` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # awscommunity-account-alternatecontact
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.5.0.
 
 ## Description
 
 An alternate contact attached to an Amazon Web Services account.
 
 ## References
 
@@ -33,15 +33,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Account::AlternateContact`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.5.0).
 * Issues related to `AwsCommunity::Account::AlternateContact` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
@@ -85,15 +85,15 @@
         phone_number: builtins.str,
         title: builtins.str,
     ) -> None:
         '''Create a new ``AwsCommunity::Account::AlternateContact``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
-        :param account_id: The account ID of the AWS account that you want to add an alternate contact to. If you do not specify this parameter, it defaults to the current AWS account.
+        :param account_id: The account ID of the AWS account that you want to add an alternate contact to.
         :param alternate_contact_type: The type of alternate contact you want to create.
         :param email_address: The email address for the alternate contact.
         :param name: The name for the alternate contact.
         :param phone_number: The phone number for the alternate contact.
         :param title: The title for the alternate contact.
         '''
         if __debug__:
@@ -145,15 +145,15 @@
         email_address: builtins.str,
         name: builtins.str,
         phone_number: builtins.str,
         title: builtins.str,
     ) -> None:
         '''An alternate contact attached to an Amazon Web Services account.
 
-        :param account_id: The account ID of the AWS account that you want to add an alternate contact to. If you do not specify this parameter, it defaults to the current AWS account.
+        :param account_id: The account ID of the AWS account that you want to add an alternate contact to.
         :param alternate_contact_type: The type of alternate contact you want to create.
         :param email_address: The email address for the alternate contact.
         :param name: The name for the alternate contact.
         :param phone_number: The phone number for the alternate contact.
         :param title: The title for the alternate contact.
 
         :schema: CfnAlternateContactProps
@@ -175,16 +175,14 @@
             "title": title,
         }
 
     @builtins.property
     def account_id(self) -> builtins.str:
         '''The account ID of the AWS account that you want to add an alternate contact to.
 
-        If you do not specify this parameter, it defaults to the current AWS account.
-
         :schema: CfnAlternateContactProps#AccountId
         '''
         result = self._values.get("account_id")
         assert result is not None, "Required property 'account_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-account-alternatecontact
-Version: 1.3.0a7
+Version: 1.5.0a7
 Summary: An alternate contact attached to an Amazon Web Services account.
 Home-page: https://github.com/aws-cloudformation/community-registry-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # awscommunity-account-alternatecontact
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.5.0.
 
 ## Description
 
 An alternate contact attached to an Amazon Web Services account.
 
 ## References
 
@@ -55,15 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Account::AlternateContact`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.5.0).
 * Issues related to `AwsCommunity::Account::AlternateContact` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.3.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.5.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_awscommunity_account_alternatecontact/py.typed
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/dependency_links.txt
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/requires.txt
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/top_level.txt
 src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/__init__.py
-src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/awscommunity-account-alternatecontact@1.3.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/awscommunity-account-alternatecontact@1.5.0-alpha.7.jsii.tgz
```

