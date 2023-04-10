# Comparing `tmp/fuckvkeypad-0.1.0.tar.gz` & `tmp/fuckvkeypad-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuckvkeypad-0.1.0.tar", last modified: Mon Apr 10 14:07:30 2023, max compression
+gzip compressed data, was "fuckvkeypad-0.2.0.tar", last modified: Mon Apr 10 16:42:10 2023, max compression
```

## Comparing `fuckvkeypad-0.1.0.tar` & `fuckvkeypad-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:07:30.821942 fuckvkeypad-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-04-09 15:21:23.000000 fuckvkeypad-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2084 2023-04-10 14:07:30.821942 fuckvkeypad-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2023-04-10 13:46:31.000000 fuckvkeypad-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:07:30.815877 fuckvkeypad-0.1.0/fuckvkeypad/
--rw-rw-rw-   0        0        0       37 2023-04-10 13:28:30.000000 fuckvkeypad-0.1.0/fuckvkeypad/__init__.py
--rw-rw-rw-   0        0        0     1452 2023-04-10 13:28:30.000000 fuckvkeypad-0.1.0/fuckvkeypad/fuckvkeypad.py
--rw-rw-rw-   0        0        0     1781 2023-04-10 10:31:04.000000 fuckvkeypad-0.1.0/fuckvkeypad/studio.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:07:30.820944 fuckvkeypad-0.1.0/fuckvkeypad.egg-info/
--rw-rw-rw-   0        0        0     2084 2023-04-10 14:07:30.000000 fuckvkeypad-0.1.0/fuckvkeypad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-04-10 14:07:30.000000 fuckvkeypad-0.1.0/fuckvkeypad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:07:30.000000 fuckvkeypad-0.1.0/fuckvkeypad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-10 14:07:30.000000 fuckvkeypad-0.1.0/fuckvkeypad.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      258 2023-04-10 14:07:30.000000 fuckvkeypad-0.1.0/fuckvkeypad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 14:07:30.000000 fuckvkeypad-0.1.0/fuckvkeypad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 14:07:30.823022 fuckvkeypad-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      805 2023-04-10 10:27:27.000000 fuckvkeypad-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:42:10.534284 fuckvkeypad-0.2.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-09 15:21:23.000000 fuckvkeypad-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2801 2023-04-10 16:42:10.534284 fuckvkeypad-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2461 2023-04-10 16:18:24.000000 fuckvkeypad-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 16:42:10.527283 fuckvkeypad-0.2.0/fuckvkeypad/
+-rw-rw-rw-   0        0        0       37 2023-04-10 13:28:30.000000 fuckvkeypad-0.2.0/fuckvkeypad/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-04-10 16:11:28.000000 fuckvkeypad-0.2.0/fuckvkeypad/fuckvkeypad.py
+-rw-rw-rw-   0        0        0     1794 2023-04-10 16:02:37.000000 fuckvkeypad-0.2.0/fuckvkeypad/studio.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:42:10.533286 fuckvkeypad-0.2.0/fuckvkeypad.egg-info/
+-rw-rw-rw-   0        0        0     2801 2023-04-10 16:42:10.000000 fuckvkeypad-0.2.0/fuckvkeypad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-04-10 16:42:10.000000 fuckvkeypad-0.2.0/fuckvkeypad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 16:42:10.000000 fuckvkeypad-0.2.0/fuckvkeypad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-10 16:42:10.000000 fuckvkeypad-0.2.0/fuckvkeypad.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      214 2023-04-10 16:42:10.000000 fuckvkeypad-0.2.0/fuckvkeypad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 16:42:10.000000 fuckvkeypad-0.2.0/fuckvkeypad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 16:42:10.534284 fuckvkeypad-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-04-10 16:41:45.000000 fuckvkeypad-0.2.0/setup.py
```

### Comparing `fuckvkeypad-0.1.0/LICENSE` & `fuckvkeypad-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuckvkeypad-0.1.0/PKG-INFO` & `fuckvkeypad-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,75 @@
 Metadata-Version: 2.1
 Name: fuckvkeypad
-Version: 0.1.0
+Version: 0.2.0
 Summary: Bypassing vKeyboard using OpenCV
 Home-page: https://github.com/soulee-dev/fuckvkeypad
 Author: Soul Lee
-License: UNKNOWN
-Platform: UNKNOWN
+License: MIT License
+Platform: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🖕⌨️ fuckvkeypad
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Lint](https://github.com/soulee-dev/FuckVkeyPad/actions/workflows/black.yml/badge.svg)](https://github.com/soulee-dev/FuckVkeyPad/actions/workflows/black.yml)
 [![codecov](https://codecov.io/gh/soulee-dev/FuckVkeyPad/branch/main/graph/badge.svg?token=V3MK4N5X5X)](https://codecov.io/gh/soulee-dev/FuckVkeyPad)
 
 금융, 정부 웹사이트등에 널리 쓰이는 보안 프로그램인 가상키보드(vKeyboard)를 우회합니다
 
 미리 캡쳐된 이미지와 유사도를 분석하는 방식으로 우회가 이루어집니다
 
+![vKeypad1](images/img1.png)
+![vKeypad2](images/img2.png)
+
+
 # 사용 방법
 ## vKeypad-Studio
 [사용 방법 영상 - YouTube](https://www.youtube.com/watch?v=4kE4m3oMGX8)
 1. 가상키보드 이미지를 준비합니다
 2. Figma에서 가상 키보드 이미지를 업로드 합니다
 3. Figma에서 사각형으로 가상 키보드 각각의 키를 덮어줍니다
 4. Figma에서 svg 파일로 Export 합니다
 5. 터미널에서 ``vkeypad-studio [이미지 파일] [svg 파일]`` 을 입력합니다
 6. 새로 뜬 창에서, 이미지에 해당되는 키보드 키를 눌러줍니다
 7. assets 폴더 속 사진들과, data.json을 따로 보관 해둡니다
 
 ## fuckvkeypad
+### 설치
+```
+pip install fuckvkeypad
+```
+
+### 예제
+assets의 폴더 위치와, data.json 위치를 매개변수로 넘겨줍니다
 ```python
 import cv2
 from fuckvkeypad import get_keymap
 
 img = cv2.imread("test_assets/vKeypad.png")
 keymap = get_keymap(
     img, asset_path="test_assets/", data_path="test_assets/data.json"
 )
 
 print(keymap)
 ```
-```shell
-> ["1", "2", "3", "4", "5", "6", "7", "8", "9", "0"]
-```
 
+바운딩 박스의 좌표와 키코드를 순서대로 출력합니다
+```python
+[
+  {"box": [0, 0, 55, 55], "key_code": 49},
+  {"box": [58, 0, 113, 55], "key_code": 50},
+  {"box": [116, 0, 171, 55], "key_code": 51},
+  {"box": [0, 58, 55, 113], "key_code": 52},
+  {"box": [58, 58, 113, 113], "key_code": 53},
+  {"box": [116, 58, 171, 113], "key_code": 54},
+  {"box": [0, 116, 55, 171], "key_code": 55},
+  {"box": [58, 116, 113, 171], "key_code": 56},
+  {"box": [116, 116, 171, 171], "key_code": 57},
+  {"box": [58, 174, 113, 229], "key_code": 48},
+]
+```
 
 # Special Thanks
-이 라이브러리는 [simple_bank_korea](https://github.com/Beomi/simple_bank_korea)에서 영감을 받아 제작하였습니다
+이 라이브러리는[simple_bank_korea](https://github.com/Beomi/simple_bank_korea)에서 영감을 받아 제작하였습니다
```

### Comparing `fuckvkeypad-0.1.0/fuckvkeypad/fuckvkeypad.py` & `fuckvkeypad-0.2.0/fuckvkeypad/fuckvkeypad.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import json
 import cv2
 import numpy as np
 
 
 def diff_img(img1, img2):
     img1 = cv2.cvtColor(img1, cv2.COLOR_BGR2GRAY)
@@ -14,41 +15,62 @@
 
 
 def get_keymap(
     img,
     asset_path: str,
     data_path: str,
     threshold: float = 100,
-    debug: bool = False,
+    verbose: bool = False,
 ):
     with open(data_path, "r") as f:
         data = json.load(f)
     boxes = data["boxes"]
     assets = data["assets"]
     keymap = []
     for box in boxes:
         crop = img[box[1] : box[3], box[0] : box[2]]
         for key, asset in assets.items():
-            img_asset = cv2.imread(asset_path + asset)
+            img_asset = cv2.imread(os.path.join(asset_path, asset))
             h1, w1 = crop.shape[:2]
             h2, w2 = img_asset.shape[:2]
             if (h1 != h2) or (w1 != w2):
                 continue
             try:
                 diff = diff_img(crop, img_asset)
-                if debug:
-                    print(diff)
+                if verbose:
+                    print(f"{key}: {diff:.2f}")
                 if diff >= threshold:
-                    keymap.append(key)
+                    keymap.append({"key_code": int(key), "box": box})
             except Exception as e:
                 print(e)
     return keymap
 
 
 def main():
     image_path = input("Enter image path: ")
     img = cv2.imread(image_path)
-    print(get_keymap(img, threshold=100))
+    keymap = get_keymap(
+        img,
+        threshold=100,
+        asset_path="../test_assets",
+        data_path="../test_assets/data.json",
+    )
+    for key in keymap:
+        print(key["key_code"], key["box"])
+        x_center = int((key["box"][0] + key["box"][2]) / 2)
+        y_center = int((key["box"][1] + key["box"][3]) / 2)
+        cv2.putText(
+            img,
+            str(chr(key["key_code"] % 256)),
+            (x_center, y_center),
+            cv2.FONT_HERSHEY_SIMPLEX,
+            1,
+            (0, 0, 255),
+            2,
+        )
+    cv2.imwrite("img2.png", img)
+    # cv2.imshow("img", img)
+    # cv2.waitKey(0)
 
 
 if __name__ == "__main__":
     main()  # pragma: no cover
```

### Comparing `fuckvkeypad-0.1.0/fuckvkeypad/studio.py` & `fuckvkeypad-0.2.0/fuckvkeypad/studio.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     coordinates = interpret_svg(svg_path)
     print("Press the key that corresponds on the keypad on image")
     if not os.path.exists("assets"):
         os.makedirs("assets")
     for i, coordinate in enumerate(coordinates):
         crop = img[coordinate[1] : coordinate[3], coordinate[0] : coordinate[2]]
         cv2.imshow("crop", crop)
-        key = chr(cv2.waitKey(0))
-        print(f"Key: {key}")
+        key = cv2.waitKey(0)
+        print(f"Key: {chr(key % 256)}({key})")
         boxes.append(coordinate)
         assets[key] = f"{i}.png"
         cv2.imwrite(f"assets/{i}.png", crop)
     cv2.destroyAllWindows()
     boxes.sort(key=lambda box: (box[1], box[0]))
     json_data = {"boxes": boxes, "assets": assets}
     with open("data.json", "w") as f:
```

### Comparing `fuckvkeypad-0.1.0/fuckvkeypad.egg-info/PKG-INFO` & `fuckvkeypad-0.2.0/fuckvkeypad.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,75 @@
 Metadata-Version: 2.1
 Name: fuckvkeypad
-Version: 0.1.0
+Version: 0.2.0
 Summary: Bypassing vKeyboard using OpenCV
 Home-page: https://github.com/soulee-dev/fuckvkeypad
 Author: Soul Lee
-License: UNKNOWN
-Platform: UNKNOWN
+License: MIT License
+Platform: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🖕⌨️ fuckvkeypad
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Lint](https://github.com/soulee-dev/FuckVkeyPad/actions/workflows/black.yml/badge.svg)](https://github.com/soulee-dev/FuckVkeyPad/actions/workflows/black.yml)
 [![codecov](https://codecov.io/gh/soulee-dev/FuckVkeyPad/branch/main/graph/badge.svg?token=V3MK4N5X5X)](https://codecov.io/gh/soulee-dev/FuckVkeyPad)
 
 금융, 정부 웹사이트등에 널리 쓰이는 보안 프로그램인 가상키보드(vKeyboard)를 우회합니다
 
 미리 캡쳐된 이미지와 유사도를 분석하는 방식으로 우회가 이루어집니다
 
+![vKeypad1](images/img1.png)
+![vKeypad2](images/img2.png)
+
+
 # 사용 방법
 ## vKeypad-Studio
 [사용 방법 영상 - YouTube](https://www.youtube.com/watch?v=4kE4m3oMGX8)
 1. 가상키보드 이미지를 준비합니다
 2. Figma에서 가상 키보드 이미지를 업로드 합니다
 3. Figma에서 사각형으로 가상 키보드 각각의 키를 덮어줍니다
 4. Figma에서 svg 파일로 Export 합니다
 5. 터미널에서 ``vkeypad-studio [이미지 파일] [svg 파일]`` 을 입력합니다
 6. 새로 뜬 창에서, 이미지에 해당되는 키보드 키를 눌러줍니다
 7. assets 폴더 속 사진들과, data.json을 따로 보관 해둡니다
 
 ## fuckvkeypad
+### 설치
+```
+pip install fuckvkeypad
+```
+
+### 예제
+assets의 폴더 위치와, data.json 위치를 매개변수로 넘겨줍니다
 ```python
 import cv2
 from fuckvkeypad import get_keymap
 
 img = cv2.imread("test_assets/vKeypad.png")
 keymap = get_keymap(
     img, asset_path="test_assets/", data_path="test_assets/data.json"
 )
 
 print(keymap)
 ```
-```shell
-> ["1", "2", "3", "4", "5", "6", "7", "8", "9", "0"]
-```
 
+바운딩 박스의 좌표와 키코드를 순서대로 출력합니다
+```python
+[
+  {"box": [0, 0, 55, 55], "key_code": 49},
+  {"box": [58, 0, 113, 55], "key_code": 50},
+  {"box": [116, 0, 171, 55], "key_code": 51},
+  {"box": [0, 58, 55, 113], "key_code": 52},
+  {"box": [58, 58, 113, 113], "key_code": 53},
+  {"box": [116, 58, 171, 113], "key_code": 54},
+  {"box": [0, 116, 55, 171], "key_code": 55},
+  {"box": [58, 116, 113, 171], "key_code": 56},
+  {"box": [116, 116, 171, 171], "key_code": 57},
+  {"box": [58, 174, 113, 229], "key_code": 48},
+]
+```
 
 # Special Thanks
-이 라이브러리는 [simple_bank_korea](https://github.com/Beomi/simple_bank_korea)에서 영감을 받아 제작하였습니다
+이 라이브러리는[simple_bank_korea](https://github.com/Beomi/simple_bank_korea)에서 영감을 받아 제작하였습니다
```

### Comparing `fuckvkeypad-0.1.0/setup.py` & `fuckvkeypad-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 from setuptools import setup, find_packages
 
 
 def get_requires():
     this_dir = os.path.dirname(__file__)
     req_path = os.path.join(this_dir, "requirements.txt")
-    return [line.rstrip("\n") for line in open(req_path, encoding="utf-16")]
+    return [line.rstrip("\n") for line in open(req_path)]
 
 
 setup(
     name="fuckvkeypad",
-    version="0.1.0",
+    version="0.2.0",
     description="Bypassing vKeyboard using OpenCV",
     author="Soul Lee",
     url="https://github.com/soulee-dev/fuckvkeypad",
     packages=find_packages(),
     install_requires=get_requires(),
-    long_description=open("README.md", "r", encoding="utf-8").read(),
+    long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
+    platforms="OS Independent",
+    license="MIT License",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     entry_points={"console_scripts": ["vkeypad-studio = fuckvkeypad.studio:main"]},
 )
```

