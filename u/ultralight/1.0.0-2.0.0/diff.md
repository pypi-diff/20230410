# Comparing `tmp/ultralight-1.0.0.tar.gz` & `tmp/ultralight-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralight-1.0.0.tar", last modified: Sat Jan 21 17:54:20 2023, max compression
+gzip compressed data, was "ultralight-2.0.0.tar", last modified: Mon Apr 10 17:17:27 2023, max compression
```

## Comparing `ultralight-1.0.0.tar` & `ultralight-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-01-21 17:54:20.307813 ultralight-1.0.0/
--rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 ultralight-1.0.0/LICENSE.txt
--rw-r--r--   0 abionics   (501) staff       (20)     1950 2023-01-21 17:54:20.307880 ultralight-1.0.0/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)      760 2023-01-21 17:18:17.000000 ultralight-1.0.0/README.md
--rw-r--r--   0 abionics   (501) staff       (20)       79 2023-01-21 17:54:20.308101 ultralight-1.0.0/setup.cfg
--rw-r--r--   0 abionics   (501) staff       (20)     1866 2023-01-21 17:14:47.000000 ultralight-1.0.0/setup.py
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-01-21 17:54:20.307090 ultralight-1.0.0/ultralight/
--rw-r--r--   0 abionics   (501) staff       (20)      166 2023-01-20 20:10:33.000000 ultralight-1.0.0/ultralight/__init__.py
--rw-r--r--   0 abionics   (501) staff       (20)     7587 2023-01-21 17:47:54.000000 ultralight-1.0.0/ultralight/ultralight.py
--rw-r--r--   0 abionics   (501) staff       (20)     1362 2023-01-21 17:47:54.000000 ultralight-1.0.0/ultralight/utils.py
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-01-21 17:54:20.307713 ultralight-1.0.0/ultralight.egg-info/
--rw-r--r--   0 abionics   (501) staff       (20)     1950 2023-01-21 17:54:20.000000 ultralight-1.0.0/ultralight.egg-info/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)      310 2023-01-21 17:54:20.000000 ultralight-1.0.0/ultralight.egg-info/SOURCES.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-01-21 17:54:20.000000 ultralight-1.0.0/ultralight.egg-info/dependency_links.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-01-21 17:53:59.000000 ultralight-1.0.0/ultralight.egg-info/not-zip-safe
--rw-r--r--   0 abionics   (501) staff       (20)       41 2023-01-21 17:54:20.000000 ultralight-1.0.0/ultralight.egg-info/requires.txt
--rw-r--r--   0 abionics   (501) staff       (20)       11 2023-01-21 17:54:20.000000 ultralight-1.0.0/ultralight.egg-info/top_level.txt
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-04-10 17:17:27.157510 ultralight-2.0.0/
+-rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 ultralight-2.0.0/LICENSE.txt
+-rw-r--r--   0 abionics   (501) staff       (20)     2235 2023-04-10 17:17:27.157574 ultralight-2.0.0/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)     1118 2023-04-06 17:02:58.000000 ultralight-2.0.0/README.md
+-rw-r--r--   0 abionics   (501) staff       (20)       79 2023-04-10 17:17:27.157793 ultralight-2.0.0/setup.cfg
+-rw-r--r--   0 abionics   (501) staff       (20)     1829 2023-04-05 13:57:36.000000 ultralight-2.0.0/setup.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-04-10 17:17:27.156768 ultralight-2.0.0/ultralight/
+-rw-r--r--   0 abionics   (501) staff       (20)      166 2023-04-07 13:03:47.000000 ultralight-2.0.0/ultralight/__init__.py
+-rw-r--r--   0 abionics   (501) staff       (20)      174 2023-04-06 16:44:43.000000 ultralight-2.0.0/ultralight/exceptions.py
+-rw-r--r--   0 abionics   (501) staff       (20)     1514 2023-04-07 13:14:59.000000 ultralight-2.0.0/ultralight/loader.py
+-rw-r--r--   0 abionics   (501) staff       (20)      188 2023-04-06 17:02:58.000000 ultralight-2.0.0/ultralight/types.py
+-rw-r--r--   0 abionics   (501) staff       (20)     8345 2023-04-07 13:07:42.000000 ultralight-2.0.0/ultralight/ultralight.py
+-rw-r--r--   0 abionics   (501) staff       (20)     3225 2023-04-06 16:52:40.000000 ultralight-2.0.0/ultralight/utils.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-04-10 17:17:27.157419 ultralight-2.0.0/ultralight.egg-info/
+-rw-r--r--   0 abionics   (501) staff       (20)     2235 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)      376 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/SOURCES.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/dependency_links.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/not-zip-safe
+-rw-r--r--   0 abionics   (501) staff       (20)       54 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/requires.txt
+-rw-r--r--   0 abionics   (501) staff       (20)       11 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/top_level.txt
```

### Comparing `ultralight-1.0.0/LICENSE.txt` & `ultralight-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ultralight-1.0.0/setup.py` & `ultralight-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,16 +30,18 @@
     author='Alex Ermolaev',
     author_email='abionics.dev@gmail.com',
     url=URL,
     license='MIT',
     keywords='face detection ai ultra light',
     install_requires=[
         'numpy',
+        'numexpr',
         'opencv-python',
         'requests',
+        'tqdm',
         'onnxruntime',
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
@@ -48,13 +50,12 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
         'Topic :: Scientific/Engineering :: Image Recognition',
         'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Software Development :: Libraries :: Python Modules',
         'Typing :: Typed',
     ],
     packages=find_packages(exclude=['models', 'samples']),
     zip_safe=False,
 )
```

### Comparing `ultralight-1.0.0/ultralight/ultralight.py` & `ultralight-2.0.0/ultralight/ultralight.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,134 +1,155 @@
-import os.path
-from typing import Literal, Sequence
+from typing import Sequence
 
 import cv2
+import numexpr as ne
 import numpy as np
-import onnxruntime as ort
-import requests
+from onnxruntime import InferenceSession
 
-MODEL_DEFAULT_PATH = '.models'
-MODEL_URL_TEMPLATE = 'https://github.com/abionics/UltraLight/releases/download/v1.0.0/{}'
-
-SizeType = Literal[320, 640]
+from ultralight.exceptions import InvalidModelParamException, InvalidInputException
+from ultralight.loader import UltraLightLoader
+from ultralight.types import SizeType, BoxesType, ScoresType
 
 
 class UltraLightDetector:
-    IMAGE_MEAN = np.asarray([127, 127, 127])
 
     def __init__(
             self,
             size: SizeType = 640,
+            batched: bool = True,
             path: str = None,
             providers: Sequence[str] = None,
             score_threshold: float = 0.9,
             iou_threshold: float = 0.3,
             keep_top_k: int = 1024,
             top_k: int = 256,
     ):
         """
         :param size: size of model input (640x480 or 320x240)
+        :param batched: should model use batched input
         :param path: path to ONNX file of model
         :param providers: ONNX providers (devices) as CPUExecutionProvider/CUDAExecutionProvider/CoreMLExecutionProvider
         :param score_threshold: confidence score threshold
         :param iou_threshold: intersection over union threshold
         :param top_k: keep K results before NMS, if k <= 0 than keep all the results
         :param top_k: keep K results after NMS, if k <= 0 than keep all the results
         """
+        self._batched = batched
         self._model_shape = (640, 480) if size == 640 else (320, 240)
-        self._ort_session = self._create_ort_session(size, path, providers)
-        ort_session_input = self._ort_session.get_inputs()[0]
-        self._input_name = ort_session_input.name
+        self._session = self._create_session(size, batched, path, providers)
+        session_input = self._session.get_inputs()[0]
+        self._input_name = session_input.name
         self._score_threshold = score_threshold
         self._iou_threshold = iou_threshold
         self._keep_top_k = keep_top_k
         self._top_k = top_k
-        onnx_model_shape = tuple(ort_session_input.shape[3:1:-1])
+        onnx_model_shape = tuple(session_input.shape[3:1:-1])
         if onnx_model_shape != self._model_shape:
-            raise Exception(
+            raise InvalidModelParamException(
                 f'ONNX model\'s shape is {onnx_model_shape}, while detector shape is {self._model_shape}! '
                 'Change `size` param or use another model file',
             )
         if self._score_threshold < 0 or self._score_threshold > 1:
-            raise Exception(f'Invalid score threshold: {self._score_threshold}, it should be in range [0..1]')
+            raise InvalidModelParamException(
+                f'Invalid score threshold: {self._score_threshold}, it should be in range [0..1]'
+            )
         if self._iou_threshold < 0 or self._iou_threshold > 1:
-            raise Exception(f'Invalid iou threshold: {self._iou_threshold}, it should be in range [0..1]')
+            raise InvalidModelParamException(
+                f'Invalid iou threshold: {self._iou_threshold}, it should be in range [0..1]'
+            )
 
     @classmethod
-    def _create_ort_session(cls, size: SizeType, path: str, providers: Sequence[str]) -> ort.InferenceSession:
+    def _create_session(
+            cls,
+            size: SizeType,
+            batched: bool,
+            path: str,
+            providers: Sequence[str],
+    ) -> InferenceSession:
         if path is None:
-            path = cls._download_model(size)
-        return ort.InferenceSession(path, providers=providers)
-
-    @staticmethod
-    def _download_model(size: SizeType) -> str:
-        if not os.path.exists(MODEL_DEFAULT_PATH):
-            os.mkdir(MODEL_DEFAULT_PATH)
-        filename = f'ultra_light_{size}.onnx'
-        path = os.path.join(MODEL_DEFAULT_PATH, filename)
-        if os.path.exists(path):
-            return path
-        url = MODEL_URL_TEMPLATE.format(filename)
-        print(f'Downloading model "{filename}" from {url}...')
-        response = requests.get(url)
-        print(f'Downloaded model "{filename}"')
-        with open(path, 'wb') as file:
-            file.write(response.content)
-        print(f'Saved model "{filename}" to "{path}"')
-        return path
+            loader = UltraLightLoader()
+            path = loader.load(size, batched)
+        return InferenceSession(path, providers=providers)
 
-    def detect(self, image: np.ndarray, fit_to_image: bool = False) -> tuple[np.ndarray, list[float]]:
+    def detect_one(self, image: np.ndarray, fit_to_image: bool = False) -> tuple[BoxesType, ScoresType]:
         if image is None:
-            raise Exception('Image is None')
-        height, width, _ = image.shape
-        image = self._preprocess_image(image)
-        scores_out, boxes_out = self._ort_session.run(None, {self._input_name: image})
-        return self._extract(boxes_out[0], scores_out[0], width, height, fit_to_image)
-
-    def _preprocess_image(self, image: np.ndarray) -> np.ndarray:
-        image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-        image = cv2.resize(image, self._model_shape)
-        image = (image - self.IMAGE_MEAN) / 128
-        image = np.transpose(image, [2, 0, 1])
-        return np.expand_dims(image, axis=0).astype(np.float32)
+            raise InvalidInputException('Image is None')
+        return self.detect_batch(np.asarray([image]), fit_to_image)[0]
+
+    def detect_batch(
+            self,
+            images: Sequence[np.ndarray],
+            fit_to_image: bool = False,
+    ) -> list[tuple[BoxesType, ScoresType]]:
+        if images is None or len(images) == 0:
+            return list()
+        for i, image in enumerate(images):
+            if image is None:
+                raise InvalidInputException(f'Image with index {i} is None')
+        if len(images) > 1 and not self._batched:
+            raise InvalidInputException(
+                f'Current detector is not batched, but images count is more than 1 (count is {len(images)}), '
+                f'use `batched=True` param in detector\'s constructor to fix this'
+            )
+        images_input = self._preprocess_images(images)
+        outputs = self._session.run(None, {self._input_name: images_input})
+        results = list()
+        for image, scores, boxes, *_ in zip(images, *outputs):
+            height, width, _ = image.shape
+            boxes, scores = self._postprocess(boxes, scores, width, height, fit_to_image)
+            results.append((boxes, scores))
+        return results
+
+    def _preprocess_images(self, images: Sequence[np.ndarray]) -> np.ndarray:
+        images = np.asarray([
+            cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+            for image in images
+        ])
+        images = np.asarray([
+            cv2.resize(image, self._model_shape)
+            for image in images
+        ])
+        images = images.astype(np.float32)  # noqa used in numexpr
+        images = ne.evaluate('(images - 127) / 128')
+        return np.transpose(images, [0, 3, 1, 2])
 
-    def _extract(
+    def _postprocess(
             self,
             boxes: np.ndarray,
             scores: np.ndarray,
             width: int,
             height: int,
             fit_to_image: bool = False,
-    ) -> tuple[np.ndarray, list[float]]:
+    ) -> tuple[BoxesType, ScoresType]:
         """
         Select boxes that contain human faces (function `predict` in original implementation)
         Parameters:
             boxes (N, 4): boxes array in corner-form
             scores (N, 2): scores array
             width: original image width
             height: original image height
             fit_to_image: should boxes fit to image borders
         Returns:
-            boxes (K, 4): an array of boxes kept
-            scores (K): a list of scores for each boxes
+            faces (K, 4): an array of faces
+            scores (K): an array of scores for each face
         """
         scores = scores[:, 1]
         mask = scores > self._score_threshold
         boxes = boxes[mask]
         scores = scores[mask]
         picked = self._hard_nms(boxes, scores)
         if len(picked) == 0:
-            return np.asarray([]), list()
+            return np.asarray([]), np.asarray([], dtype=np.float32)
         boxes = boxes[picked]
         scores = scores[picked]
         boxes *= np.asarray([width, height, width, height])
         if fit_to_image:
             boxes[:, 0::2] = np.clip(boxes[:, 0::2], 0, width - 1)
             boxes[:, 1::2] = np.clip(boxes[:, 1::2], 0, height - 1)
-        return boxes.astype(np.int32), scores.tolist()
+        return boxes.astype(np.int32), scores
 
     def _hard_nms(self, boxes: np.ndarray, scores: np.ndarray) -> list[int]:
         """
         Perform hard non-maximum-suppression to filter out boxes with iou greater than threshold
         Parameters:
             boxes (N, 4): boxes array in corner-form
             scores (N, 2): scores array
```

