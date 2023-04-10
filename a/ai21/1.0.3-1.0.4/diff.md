# Comparing `tmp/ai21-1.0.3.tar.gz` & `tmp/ai21-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ai21-1.0.3.tar", last modified: Mon Mar 27 13:09:01 2023, max compression
+gzip compressed data, was "dist/ai21-1.0.4.tar", last modified: Mon Apr 10 09:45:55 2023, max compression
```

## Comparing `ai21-1.0.3.tar` & `ai21-1.0.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-03-27 13:09:01.000000 ai21-1.0.3/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      204 2023-03-27 13:09:01.000000 ai21-1.0.3/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2598 2023-03-25 06:53:34.000000 ai21-1.0.3/README.md
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      576 2023-03-27 12:47:23.000000 ai21-1.0.3/setup.py
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      107 2023-03-27 13:09:01.000000 ai21-1.0.3/setup.cfg
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-03-27 13:09:01.000000 ai21-1.0.3/ai21/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      971 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/ai21_object.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       22 2023-03-27 13:08:20.000000 ai21-1.0.3/ai21/version.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3868 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/http_client.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      104 2023-03-27 12:35:08.000000 ai21-1.0.3/ai21/constants.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      700 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2590 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/ai21_studio_client.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2100 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/SM_utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/api_resources.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1875 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2823 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/errors.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-03-27 13:09:01.000000 ai21-1.0.3/ai21/modules/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1375 2023-03-27 12:35:43.000000 ai21-1.0.3/ai21/modules/completion.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1174 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/experimantal.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      856 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/custom_model.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-03-27 13:09:01.000000 ai21-1.0.3/ai21/modules/resources/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1208 2023-03-27 12:30:48.000000 ai21-1.0.3/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/resources/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      352 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      371 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      387 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      476 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/resources/upload_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      585 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      461 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/tokenization.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      678 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/improvements.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      795 2023-03-27 12:35:43.000000 ai21-1.0.3/ai21/modules/summarize.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      536 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/gec.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      646 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/dataset.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/paraphrase.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      611 2023-03-25 06:53:34.000000 ai21-1.0.3/ai21/modules/segmentation.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-03-27 13:09:01.000000 ai21-1.0.3/ai21.egg-info/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      204 2023-03-27 13:09:01.000000 ai21-1.0.3/ai21.egg-info/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      933 2023-03-27 13:09:01.000000 ai21-1.0.3/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       21 2023-03-27 13:09:01.000000 ai21-1.0.3/ai21.egg-info/requires.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        5 2023-03-27 13:09:01.000000 ai21-1.0.3/ai21.egg-info/top_level.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        1 2023-03-27 13:09:01.000000 ai21-1.0.3/ai21.egg-info/dependency_links.txt
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      204 2023-04-10 09:45:55.000000 ai21-1.0.4/PKG-INFO
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2600 2023-04-10 09:05:28.000000 ai21-1.0.4/README.md
+-rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      576 2023-03-27 12:47:23.000000 ai21-1.0.4/setup.py
+-rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      107 2023-04-10 09:45:55.000000 ai21-1.0.4/setup.cfg
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/ai21/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      971 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/ai21_object.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)       22 2023-04-10 09:39:56.000000 ai21-1.0.4/ai21/version.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3868 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/http_client.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      104 2023-04-10 09:05:28.000000 ai21-1.0.4/ai21/constants.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      751 2023-04-10 09:33:18.000000 ai21-1.0.4/ai21/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2590 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/ai21_studio_client.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2100 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/SM_utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/api_resources.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1875 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2823 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/errors.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/ai21/modules/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      771 2023-04-10 09:33:08.000000 ai21-1.0.4/ai21/modules/question_answering.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1375 2023-04-10 09:05:28.000000 ai21-1.0.4/ai21/modules/completion.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1823 2023-04-10 09:18:41.000000 ai21-1.0.4/ai21/modules/experimantal.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      856 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/custom_model.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/ai21/modules/resources/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1208 2023-04-10 09:05:28.000000 ai21-1.0.4/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      352 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      371 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      387 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      476 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/upload_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      585 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      461 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/tokenization.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      678 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/improvements.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      795 2023-04-10 09:35:40.000000 ai21-1.0.4/ai21/modules/summarize.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      536 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/gec.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      646 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/dataset.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/paraphrase.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      611 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/segmentation.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/ai21.egg-info/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      204 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      968 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)       21 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/requires.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        5 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/top_level.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        1 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/dependency_links.txt
```

### Comparing `ai21-1.0.3/README.md` & `ai21-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
 print(response)
 ```
 
 ### SageMaker Endpoint
 This python SDK can also be used to invoke Jurassic-1 models as a SageMaker (SM) endpoint. To activate this option, make sure to install with the extra SM dependencies:
 
-`pip install -U ai21[SM]`
+`pip install -U ai21['SM']`
 
 You can then generate a completion by running:
 ```python
 response = ai21.Completion.execute(sm_endpoint="<your_endpoint_name>", prompt="hello world", maxTokens=20)
 print(response)
 ```
```

### Comparing `ai21-1.0.3/setup.py` & `ai21-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/ai21_object.py` & `ai21-1.0.4/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/http_client.py` & `ai21-1.0.4/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/__init__.py` & `ai21-1.0.4/ai21/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ai21.modules.tokenization import Tokenization
 from ai21.modules.custom_model import CustomModel
 from ai21.modules.experimantal import Experimental
 from ai21.modules.paraphrase import Paraphrase
 from ai21.modules.summarize import Summarize
 from ai21.modules.segmentation import Segmentation
 from ai21.modules.improvements import Improvements
+from ai21.modules.question_answering import Answer
 from ai21.modules.gec import GEC
 
 
 api_key = None
 organization = None
 application = None
 api_version = DEFAULT_API_VERSION
```

### Comparing `ai21-1.0.3/ai21/ai21_studio_client.py` & `ai21-1.0.4/ai21/ai21_studio_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/SM_utils.py` & `ai21-1.0.4/ai21/SM_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/utils.py` & `ai21-1.0.4/ai21/utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/errors.py` & `ai21-1.0.4/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/modules/completion.py` & `ai21-1.0.4/ai21/modules/completion.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/modules/experimantal.py` & `ai21-1.0.4/ai21/modules/experimantal.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ai21 import Completion
+from ai21.constants import SAGEMAKER_ENDPOINT_KEY
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
 class Experimental(NLPTask):
 
     @classmethod
@@ -24,7 +25,18 @@
         url = f'{url}/experimental/summarize'
         return super().execute(task_url=url, **params)
 
     @classmethod
     def j1_grande_instruct(cls, **params):
         params["model"] = "j1-grande-instruct"
         return Completion.execute(experimental_mode=True, **params)
+
+    @classmethod
+    def answer(cls, **params):
+        validate_mandatory_field(key='context', call_name="answer_experimental", params=params, validate_type=True, expected_type=str)
+        validate_mandatory_field(key='question', call_name="answer_experimental", params=params, validate_type=True, expected_type=str)
+        use_sm_endpoint = SAGEMAKER_ENDPOINT_KEY in params
+        if use_sm_endpoint:
+            return cls.execute_sm_endpoint(**params)
+        url = cls.get_base_url(**params)
+        url = f'{url}/experimental/answer'
+        return super().execute(task_url=url, **params)
```

### Comparing `ai21-1.0.3/ai21/modules/custom_model.py` & `ai21-1.0.4/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/modules/resources/nlp_task.py` & `ai21-1.0.4/ai21/modules/resources/nlp_task.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/modules/resources/ai21_module.py` & `ai21-1.0.4/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/modules/improvements.py` & `ai21-1.0.4/ai21/modules/improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/modules/summarize.py` & `ai21-1.0.4/ai21/modules/summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/modules/gec.py` & `ai21-1.0.4/ai21/modules/gec.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/modules/dataset.py` & `ai21-1.0.4/ai21/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21/modules/segmentation.py` & `ai21-1.0.4/ai21/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.3/ai21.egg-info/SOURCES.txt` & `ai21-1.0.4/ai21.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ai21/modules/completion.py
 ai21/modules/custom_model.py
 ai21/modules/dataset.py
 ai21/modules/experimantal.py
 ai21/modules/gec.py
 ai21/modules/improvements.py
 ai21/modules/paraphrase.py
+ai21/modules/question_answering.py
 ai21/modules/segmentation.py
 ai21/modules/summarize.py
 ai21/modules/tokenization.py
 ai21/modules/resources/__init__.py
 ai21/modules/resources/ai21_module.py
 ai21/modules/resources/creatable_resource.py
 ai21/modules/resources/listable_resource.py
```

