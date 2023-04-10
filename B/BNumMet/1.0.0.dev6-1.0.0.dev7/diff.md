# Comparing `tmp/BNumMet-1.0.0.dev6.tar.gz` & `tmp/BNumMet-1.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BNumMet-1.0.0.dev6.tar", last modified: Wed Apr  5 16:10:21 2023, max compression
+gzip compressed data, was "BNumMet-1.0.0.dev7.tar", last modified: Mon Apr 10 12:35:26 2023, max compression
```

## Comparing `BNumMet-1.0.0.dev6.tar` & `BNumMet-1.0.0.dev7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:10:21.802520 BNumMet-1.0.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50060 2023-04-05 16:10:21.806520 BNumMet-1.0.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-05 16:10:21.806520 BNumMet-1.0.0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:10:21.798520 BNumMet-1.0.0.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:10:21.802520 BNumMet-1.0.0.dev6/src/BNumMet/
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/Interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/LinearSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/NonLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/Random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:10:21.802520 BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/InterpolationVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/LUVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/LeastSquaresVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25959 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/NonLinearVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/RandomVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/src/BNumMet/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:10:21.802520 BNumMet-1.0.0.dev6/src/BNumMet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50060 2023-04-05 16:10:21.000000 BNumMet-1.0.0.dev6/src/BNumMet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-05 16:10:21.000000 BNumMet-1.0.0.dev6/src/BNumMet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 16:10:21.000000 BNumMet-1.0.0.dev6/src/BNumMet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 16:10:21.000000 BNumMet-1.0.0.dev6/src/BNumMet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-05 16:10:21.000000 BNumMet-1.0.0.dev6/src/BNumMet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 16:10:21.000000 BNumMet-1.0.0.dev6/src/BNumMet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:10:21.802520 BNumMet-1.0.0.dev6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/tests/test_General.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/tests/test_Interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/tests/test_LeastSquares.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/tests/test_LinealSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/tests/test_NonLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/tests/test_Random.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-05 16:10:03.000000 BNumMet-1.0.0.dev6/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50394 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.679077 BNumMet-1.0.0.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.679077 BNumMet-1.0.0.dev7/src/BNumMet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/LinearSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/NonLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/InterpolationVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/LUVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/LeastSquaresVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/NonLinearVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/RandomVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50394 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_General.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_Interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_LeastSquares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_LinealSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_NonLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_Random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_module.py
```

### Comparing `BNumMet-1.0.0.dev6/LICENSE` & `BNumMet-1.0.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/PKG-INFO` & `BNumMet-1.0.0.dev7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BNumMet
-Version: 1.0.0.dev6
+Version: 1.0.0.dev7
 Summary: Basic Numerical Methods for Python 3
 Home-page: https://github.com/fbpazos/Trabajo-Fin-Master/tree/main/Python_BNumMet
 Author: Fernando Bellido Pazos
 Author-email: fbellidopazos@gmail.com
 License: AGPL-3.0
 Platform: unix
 Platform: linux
@@ -227,15 +227,15 @@
 # Plotting using Matplotlib
 plt.plot(u, v, "b-", label="Interpolated")
 plt.plot(x, y, "ro", label="Original Points")
 plt.legend()
 plt.show()
 ```
 
-![Interpolation](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Interpolation/PCHIP%20Example%201.png?token=GHSAT0AAAAAAB4UDLTP2QAM3MIK5XNV3UQ2ZBKWKMQ)
+![Interpolation](https://dub07pap002files.storage.live.com/y4m52-hsxWxH8zjFakW7db0zDr1AGGI4j3VL3PTT_g5KO0AiotCnUBwwO5I9sSXIToLvJnfWtCBaOyZLukE_JBryO-JNNkodo2W0xjneL0cDoDy3CZaoFC-d8N0XbkOAWYjZgcu3M1K-j74BgEXUL5-oV6S_yLayyCtUl30xP6BPlC6bio1ZqPtqs2mARBgEP7e?encodeFailures=1&width=543&height=413)
 
 ### Non-Linear
 
 ```python
 from BNumMet.NonLinear import zBrentDekker
 fun = lambda x: x**2 - 2
 interval = [1, 2]
@@ -256,60 +256,60 @@
         marsaglia_rand(base=41, lag_r=2, lag_s=1, carry=0, seed_tuple=(0, 1)),
     )
     for i in range(100000)
 ]
 plt.scatter(*zip(*fail), s=1, c="black")
 plt.show()
 ```
-![Randomness](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Randomness/Marsaglia%20Rand%20Example%203.png?token=GHSAT0AAAAAAB4UDLTPNUUF6YTR75GHN7CCZBKWMCQ)
+![Randomness](https://dub07pap002files.storage.live.com/y4mzE0abSi6MSC6wlcNO6cc7HkixFGCybt2guF2nrsuJevEeYJ01VOcaZ244FjFpN27PlSrAUucq_62p8wlyPdlkW1hEGJTD2ngxsI5DX8KtFOGtFqfHSyijZiYvKO4D2QoeURctNgIbgg75bzDNkiYWIjcJhXbwdipgxoLEuQItQBXjEX3vGcH134768ZZXfF_?encodeFailures=1&width=547&height=413)
 
 ### Visualizers
 #### Linear Systems
 ```python
 from BNumMet.Visualizers.LUVisualizer import LUVisualizer
 luVisualizer = LUVisualizer()
 display(luVisualizer.run())
 ```
-![LUVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/LUVisualizer/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTPYKFM4QBOJKB4RDGQZBKWNDQ)
+![LUVisualizer](https://dub07pap002files.storage.live.com/y4m1q7uSd3dG2sMftf0YKDwNnz7aLGBnXeclboMbvU5un83LIpfX4Pw-8MJCHRzYcwLocDkZ1BeeAEx3qaowz7GUROV2rDzAYvmCcDEMw-X9P2HzXU9U3BzSMAQISEyUxxvVp3aNi46blEf1c1Liw_cADasxsqjOaZwwrrwTP7x7awPTudf0z4GwEmO2RH_akoB?encodeFailures=1&width=1080&height=404)
 
 #### Interpolation
 ```python
 from BNumMet.Visualizers.InterpolationVisualizer import InterpolVisualizer
 interpolVisualizer = InterpolVisualizer()
 display(interpolVisualizer.run())
 ```
-![interpolVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/Interpolation/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTOLYUOFN2JCWWDMMNWZBKWNPA)
+![interpolVisualizer](https://dub07pap002files.storage.live.com/y4mIg9iw5xzbHxOkHF5tfZGqdjS2yob1Zzd6LXkedOdQE8RBt54lqqfLUX8XB2113dOYLKqzjph5GDzoYvp-Qf7uaqL8NQ_GH0CBYfTQNT1FIqB6Yn-KO4dT78rau9Ka1FfR5zsbToR24NJnkJX5jy-xymWato5cUJ4aDJqAz_ENPJA2n1nNkCaFQ7WX58tmqzz?encodeFailures=1&width=952&height=551)
 
 
 #### Non-Linear
 ```python
 from BNumMet.Visualizers.NonLinearVisualizer import NonLinearVisualizer
 zerosVisualizer = NonLinearVisualizer()
 zerosVisualizer.run()
 ```
-![zerosVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/NonLinear/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTONMMPKCLJ6ESNJKC4ZBKWOXA)
+![zerosVisualizer](https://dub07pap002files.storage.live.com/y4m1UJWkc5j50NF4KZd1w9VENgIqMT-GMjhE-qhKLIdF3K-ymR4Rttav5ZwUjSaCDFzuz0mYyDPS-5MBo89JEyTOO-P5PdwXoJN4rCO1vlrn_MxwTHLsscwHGFITW_0KwLW1cWi0u5EAtXphyBQf_tCH-OT5aqPQT8TS6urP1bgeHDrmAm6twsn0E2AqWKhbMpX?encodeFailures=1&width=864&height=711)
 
 
 #### Least Squares
 ```python
 from BNumMet.Visualizers.LeastSquaresVisualizer import LSPVisualizer
 xData = np.array([0, 1, 2, 3, 4, 5])
 yData = np.array([4.5, 2.4, 1.5, 1, 1.5, 2.4])
 lspVisualizer = LSPVisualizer(xData, yData)
 lspVisualizer.run()
 ```
-![lspVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/LeastSquares/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTOGS7TTRSRNDBCS4KCZBKWPSA)
+![lspVisualizer](https://dub07pap002files.storage.live.com/y4mJQgX2hkcE5PU_vExDNiJb3-xPapyxDQqf7yZbw1uJ3kkxv5gxwsmYb13hUqf_IYyxdp9cZJHUP4UPYCuXzXs_hh27XFdwF5e6DsQSr0JGfKQhxivPBD6B_90wSpatlXWFG47NPzC5SxsDcM8Mj0u50hQUCGdXsbpGHHY5eDnB-CL_E2I1F0F0CkNPnAna5XW?encodeFailures=1&width=794&height=465)
 
 #### Randomness
 ```python
 from BNumMet.Visualizers.RandomVisualizer import RandomVisualizer
 randomVisualizer = RandomVisualizer()
 randomVisualizer.run()
 ```
-![randomVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/Randomness/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTPTJFHTKTPLC43VJQAZBKWQHQ)
+![randomVisualizer](https://dub07pap002files.storage.live.com/y4mE3vUbK5Q6OnxGwiw3aQCfp8TrjYyo9mNdVMs1qjLWA3hNpGcLtisRHQZRXQEOEmdU3b3LLH4OLDgfgUFT2GrO4ktOIa6nyKB10ICQR_WIEyS-LPyM1NDXdEmKhe8uafPjJdJy8-fJI9y9t-tiuOaDZFGedaHBDfFZCvTZbYKvHgDmRrqycXAp7vx1lesvPLv?encodeFailures=1&width=722&height=758)
```

### Comparing `BNumMet-1.0.0.dev6/Readme.md` & `BNumMet-1.0.0.dev7/Readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 # Plotting using Matplotlib
 plt.plot(u, v, "b-", label="Interpolated")
 plt.plot(x, y, "ro", label="Original Points")
 plt.legend()
 plt.show()
 ```
 
-![Interpolation](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Interpolation/PCHIP%20Example%201.png?token=GHSAT0AAAAAAB4UDLTP2QAM3MIK5XNV3UQ2ZBKWKMQ)
+![Interpolation](https://dub07pap002files.storage.live.com/y4m52-hsxWxH8zjFakW7db0zDr1AGGI4j3VL3PTT_g5KO0AiotCnUBwwO5I9sSXIToLvJnfWtCBaOyZLukE_JBryO-JNNkodo2W0xjneL0cDoDy3CZaoFC-d8N0XbkOAWYjZgcu3M1K-j74BgEXUL5-oV6S_yLayyCtUl30xP6BPlC6bio1ZqPtqs2mARBgEP7e?encodeFailures=1&width=543&height=413)
 
 ### Non-Linear
 
 ```python
 from BNumMet.NonLinear import zBrentDekker
 fun = lambda x: x**2 - 2
 interval = [1, 2]
@@ -217,60 +217,60 @@
         marsaglia_rand(base=41, lag_r=2, lag_s=1, carry=0, seed_tuple=(0, 1)),
     )
     for i in range(100000)
 ]
 plt.scatter(*zip(*fail), s=1, c="black")
 plt.show()
 ```
-![Randomness](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Randomness/Marsaglia%20Rand%20Example%203.png?token=GHSAT0AAAAAAB4UDLTPNUUF6YTR75GHN7CCZBKWMCQ)
+![Randomness](https://dub07pap002files.storage.live.com/y4mzE0abSi6MSC6wlcNO6cc7HkixFGCybt2guF2nrsuJevEeYJ01VOcaZ244FjFpN27PlSrAUucq_62p8wlyPdlkW1hEGJTD2ngxsI5DX8KtFOGtFqfHSyijZiYvKO4D2QoeURctNgIbgg75bzDNkiYWIjcJhXbwdipgxoLEuQItQBXjEX3vGcH134768ZZXfF_?encodeFailures=1&width=547&height=413)
 
 ### Visualizers
 #### Linear Systems
 ```python
 from BNumMet.Visualizers.LUVisualizer import LUVisualizer
 luVisualizer = LUVisualizer()
 display(luVisualizer.run())
 ```
-![LUVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/LUVisualizer/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTPYKFM4QBOJKB4RDGQZBKWNDQ)
+![LUVisualizer](https://dub07pap002files.storage.live.com/y4m1q7uSd3dG2sMftf0YKDwNnz7aLGBnXeclboMbvU5un83LIpfX4Pw-8MJCHRzYcwLocDkZ1BeeAEx3qaowz7GUROV2rDzAYvmCcDEMw-X9P2HzXU9U3BzSMAQISEyUxxvVp3aNi46blEf1c1Liw_cADasxsqjOaZwwrrwTP7x7awPTudf0z4GwEmO2RH_akoB?encodeFailures=1&width=1080&height=404)
 
 #### Interpolation
 ```python
 from BNumMet.Visualizers.InterpolationVisualizer import InterpolVisualizer
 interpolVisualizer = InterpolVisualizer()
 display(interpolVisualizer.run())
 ```
-![interpolVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/Interpolation/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTOLYUOFN2JCWWDMMNWZBKWNPA)
+![interpolVisualizer](https://dub07pap002files.storage.live.com/y4mIg9iw5xzbHxOkHF5tfZGqdjS2yob1Zzd6LXkedOdQE8RBt54lqqfLUX8XB2113dOYLKqzjph5GDzoYvp-Qf7uaqL8NQ_GH0CBYfTQNT1FIqB6Yn-KO4dT78rau9Ka1FfR5zsbToR24NJnkJX5jy-xymWato5cUJ4aDJqAz_ENPJA2n1nNkCaFQ7WX58tmqzz?encodeFailures=1&width=952&height=551)
 
 
 #### Non-Linear
 ```python
 from BNumMet.Visualizers.NonLinearVisualizer import NonLinearVisualizer
 zerosVisualizer = NonLinearVisualizer()
 zerosVisualizer.run()
 ```
-![zerosVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/NonLinear/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTONMMPKCLJ6ESNJKC4ZBKWOXA)
+![zerosVisualizer](https://dub07pap002files.storage.live.com/y4m1UJWkc5j50NF4KZd1w9VENgIqMT-GMjhE-qhKLIdF3K-ymR4Rttav5ZwUjSaCDFzuz0mYyDPS-5MBo89JEyTOO-P5PdwXoJN4rCO1vlrn_MxwTHLsscwHGFITW_0KwLW1cWi0u5EAtXphyBQf_tCH-OT5aqPQT8TS6urP1bgeHDrmAm6twsn0E2AqWKhbMpX?encodeFailures=1&width=864&height=711)
 
 
 #### Least Squares
 ```python
 from BNumMet.Visualizers.LeastSquaresVisualizer import LSPVisualizer
 xData = np.array([0, 1, 2, 3, 4, 5])
 yData = np.array([4.5, 2.4, 1.5, 1, 1.5, 2.4])
 lspVisualizer = LSPVisualizer(xData, yData)
 lspVisualizer.run()
 ```
-![lspVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/LeastSquares/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTOGS7TTRSRNDBCS4KCZBKWPSA)
+![lspVisualizer](https://dub07pap002files.storage.live.com/y4mJQgX2hkcE5PU_vExDNiJb3-xPapyxDQqf7yZbw1uJ3kkxv5gxwsmYb13hUqf_IYyxdp9cZJHUP4UPYCuXzXs_hh27XFdwF5e6DsQSr0JGfKQhxivPBD6B_90wSpatlXWFG47NPzC5SxsDcM8Mj0u50hQUCGdXsbpGHHY5eDnB-CL_E2I1F0F0CkNPnAna5XW?encodeFailures=1&width=794&height=465)
 
 #### Randomness
 ```python
 from BNumMet.Visualizers.RandomVisualizer import RandomVisualizer
 randomVisualizer = RandomVisualizer()
 randomVisualizer.run()
 ```
-![randomVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/Randomness/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTPTJFHTKTPLC43VJQAZBKWQHQ)
+![randomVisualizer](https://dub07pap002files.storage.live.com/y4mE3vUbK5Q6OnxGwiw3aQCfp8TrjYyo9mNdVMs1qjLWA3hNpGcLtisRHQZRXQEOEmdU3b3LLH4OLDgfgUFT2GrO4ktOIa6nyKB10ICQR_WIEyS-LPyM1NDXdEmKhe8uafPjJdJy8-fJI9y9t-tiuOaDZFGedaHBDfFZCvTZbYKvHgDmRrqycXAp7vx1lesvPLv?encodeFailures=1&width=722&height=758)
```

### Comparing `BNumMet-1.0.0.dev6/setup.cfg` & `BNumMet-1.0.0.dev7/setup.cfg`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet/Interpolation.py` & `BNumMet-1.0.0.dev7/src/BNumMet/Interpolation.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet/LinearSystems.py` & `BNumMet-1.0.0.dev7/src/BNumMet/LinearSystems.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet/NonLinear.py` & `BNumMet-1.0.0.dev7/src/BNumMet/NonLinear.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet/Random.py` & `BNumMet-1.0.0.dev7/src/BNumMet/Random.py`

 * *Files 9% similar despite different names*

```diff
@@ -336,39 +336,39 @@
     if mt_vars["mti"] >= mt_vars["N"]:
         kk = 0
         y = None
 
         while kk < mt_vars["N"] - mt_vars["M"]:
             y = (mt_vars["mt"][kk] & mt_vars["UPPER_MASK"]) | (
                 mt_vars["mt"][kk + 1] & mt_vars["LOWER_MASK"]
-            )  # y = (mt[kk] & UPPER_MASK) | (mt[kk + 1] & LOWER_MASK)
+            )  # y = (mt[kk] AND UPPER_MASK) OR (mt[kk + 1] AND LOWER_MASK)
             mt_vars["mt"][kk] = (
                 mt_vars["mt"][kk + mt_vars["M"]] ^ (y >> 1) ^ mag01[y & 0x1]
-            )  # mt[kk] = mt[kk + M] ^ (y >> 1) ^ mag01[y & 0x1]
+            )  # mt[kk] = mt[kk + M] XOR (y >> 1) XOR mag01[y AND 0x1]
             kk += 1
 
         while kk < mt_vars["N"] - 1:
             y = (mt_vars["mt"][kk] & mt_vars["UPPER_MASK"]) | (
                 mt_vars["mt"][kk + 1] & mt_vars["LOWER_MASK"]
-            )  # y = (mt[kk] & UPPER_MASK) | (mt[kk + 1] & LOWER_MASK)
+            )  # y = (mt[kk] AND UPPER_MASK) OR (mt[kk + 1] AND LOWER_MASK)
             mt_vars["mt"][kk] = (
                 mt_vars["mt"][kk + (mt_vars["M"] - mt_vars["N"])]
                 ^ (y >> 1)
                 ^ mag01[y & 0x1]
-            )  # mt[kk] = mt[kk + (M - N)] ^ (y >> 1) ^ mag01[y & 0x1]
+            )  # mt[kk] = mt[kk + (M - N)] XOR (y >> 1) AND mag01[y & 0x1]
             kk += 1
 
         y = (mt_vars["mt"][mt_vars["N"] - 1] & mt_vars["UPPER_MASK"]) | (
             mt_vars["mt"][0] & mt_vars["LOWER_MASK"]
-        )  # y = (mt[N - 1] & UPPER_MASK) | (mt[0] & LOWER_MASK)
+        )  # y = (mt[N - 1] AND UPPER_MASK) OR (mt[0] AND LOWER_MASK)
         mt_vars["mt"][mt_vars["N"] - 1] = (
             mt_vars["mt"][mt_vars["M"] - 1] ^ (y >> 1) ^ mag01[y & 0x1]
-        )  # mt[N - 1] = mt[M - 1] ^ (y >> 1) ^ mag01[y & 0x1]
+        )  # mt[N - 1] = mt[M - 1] XOR (y >> 1) XOR mag01[y & 0x1]
 
-        mt_vars["mti"] = 0  # mti = 0
+        mt_vars["mti"] = 0
 
     y = mt_vars["mt"][mt_vars["mti"]]  # y = mt[mti++]
     mt_vars["mti"] += 1
 
     # Tempering
     y ^= mt_vars["TEMPERING_SHIFT_U"](y)
     y ^= mt_vars["TEMPERING_SHIFT_S"](y) & mt_vars["TEMPERING_MASK_B"]
```

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/InterpolationVisualizer.py` & `BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/InterpolationVisualizer.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/LUVisualizer.py` & `BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/LUVisualizer.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/LeastSquaresVisualizer.py` & `BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/LeastSquaresVisualizer.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet/Visualizers/NonLinearVisualizer.py` & `BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/NonLinearVisualizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class NonLinearVisualizer:
     def __init__(
         self, fun=lambda x: (x - 1) * (x - 4) * np.exp(-x), interval=(0, 3), tol=1e-3
     ):
         # Initialize basic Parameters
-        self.brentDekker = zBrentDekker(
+        self.brent_dekker = zBrentDekker(
             fun, interval, tol, iters=True, steps=True
         )  # Get the output of Brent Dekkers Alg --> (x, iters)
 
         # Set the input function, the interval for the function evaluation,
         # and the tolerance for the algorithm
         self.f = fun
         self.a, self.b = interval
@@ -31,102 +31,102 @@
         # First Step of the Algorithm
         # ==========================================================================
         ## Section: INT
         # Set the initial values for internal variables
         self.c, self.fc, self.e = self.a, self.fa, self.b - self.a
         ## Section: EXT
         # Call the sectionEXT() function to perform the first external section of the algorithm
-        self.sectionEXT()
+        self.section_ext()
 
         # Current Step Save Values
         # ==========================================================================
         # Save the current state of the algorithm in a tuple
-        self.currentStep = (self.a, self.b, self.c, self.e)
+        self.current_step = (self.a, self.b, self.c, self.e)
 
         # Revert Stack
         # ==========================================================================
         # Create an empty stack to keep track of previous states of the algorithm
-        self.revertStack = []
+        self.revert_stack = []
 
         # Draw mesh
         # ==========================================================================
         # Create a numpy array of 1000 evenly spaced values between the minimum and maximum
         # values of the function interval to use for plotting the function
         self.x = np.linspace(min(self.a, self.b), max(self.a, self.b), 1000)
         self.widen = False
 
-    def checkBoxChanged(self, change):
-        with self.Fig.hold_sync():  # Hold the figure syncronized
+    def checkbox_changed(self, change):
+        with self.fig.hold_sync():  # Hold the figure syncronized
             self.draw_figures()  # Draw the figures
 
-    def sectionINT(self):
+    def section_int(self):
         # Check if the function evaluates with the same sign on both sides of c
         if np.sign(self.fb) == np.sign(self.fc) != 0:
             # If the condition is met, update the values of c, fc and e
             self.c, self.fc, self.e = self.a, self.fa, self.b - self.a
 
-    def sectionEXT(self):
+    def section_ext(self):
         # Check which of the endpoints has the smaller absolute value of f
         if abs(self.fc) < abs(self.fb):
             # If the condition is met, swap the values of a, b and c with b, c and b respectively,
             # and update the values of fa, fb and fc accordingly
             self.a, self.b, self.c, self.fa, self.fb, self.fc = (
                 self.b,
                 self.c,
                 self.b,
                 self.fb,
                 self.fc,
                 self.fb,
             )
 
-    def initializeComponents(self):
+    def initialize_components(self):
         # Current Solution Text
         # ==========================================================================
         # Widget for displaying current solution output
         # Current Solution: (b, f(b))
         # Iterations: N
-        self.currentSolOut = widgets.Output()
+        self.current_solution_output = widgets.Output()
 
         # Helper Text
         # ==========================================================================
         # Widget for displaying helper output
         # Suggestion for next step: <Bisect/IQI/Secant>
-        self.helperOut = widgets.Output()  # Next Possible Step: <Bisect/IQI/None>
+        self.helper_output = widgets.Output()  # Next Possible Step: <Bisect/IQI/None>
 
         # Brent-Dekker Solution
         # ==========================================================================
         # Widget for displaying Brent-Dekker solution output
         # Brent-Dekker Solution: (x^, f(x^)) in N^ iterations
-        self.brentDekkerOut = widgets.HTML(
-            value=f"<blockquote> Brent-Dekker Solution: <b>({self.brentDekker[0]:.4e}, {self.f(self.brentDekker[0]):.4e})</b> in <b>{self.brentDekker[1]}</b> iterations"
+        self.brent_dekker_output = widgets.HTML(
+            value=f"<blockquote> Brent-Dekker Solution: <b>({self.brent_dekker[0]:.4e}, {self.f(self.brent_dekker[0]):.4e})</b> in <b>{self.brent_dekker[1]}</b> iterations"
         )
 
         # Reset Button
         # ==========================================================================
         # Widget for reset button
-        self.resetButton = widgets.Button(
+        self.reset_button = widgets.Button(
             description="Reset",
             disabled=False,
             button_style="danger",
             tooltip="Reset",
             icon="undo",
         )
-        self.resetButton.on_click(self.reset)
+        self.reset_button.on_click(self.reset)
 
         # Revert Button
         # ==========================================================================
         # Widget for revert button
-        self.revertButton = widgets.Button(
+        self.revert_button = widgets.Button(
             description="Revert",
             disable=False,
             button_style="warning",
             tooltip="Revert",
             icon="arrow-left",
         )
-        self.revertButton.on_click(self.revert)
+        self.revert_button.on_click(self.revert)
 
         # FIGURE
         # ==========================================================================
         # Widget for plotting the function and its zeros
         # Set up axes and scales for the plot
         self.x_sc = bq.LinearScale()
         self.y_sc = bq.LinearScale()
@@ -135,128 +135,128 @@
             scale=self.y_sc,
             orientation="vertical",
             tick_format="0.4e",
             grid_lines="solid",
             label="Y",
         )
         # Set up the plot figure
-        self.Fig = bq.Figure(
+        self.fig = bq.Figure(
             marks=[],
             axes=[ax_x, ax_y],
             title="Zeros of a Function",
         )
         # Set up the plot figure toolbar
-        self.Toolbar = bq.Toolbar(figure=self.Fig)
+        self.toolbar = bq.Toolbar(figure=self.fig)
         # Add default lines to the plot figure
-        self.defaultLines()
+        self.default_lines()
 
         # FUNCTION BUTTONS
         # ==========================================================================
         # Widgets for buttons for selecting the next function to perform
         # Each button has a pointIndex attribute that is used to identify the point in the points array
         # 0: Bisect  1: Secant  2: IQI
         # Bisect Button
-        self.bisectButton = widgets.Button(
+        self.bisect_button = widgets.Button(
             description="Bisect",
             disabled=False,
             tooltip="Bisect",
         )
-        self.bisectButton.pointIndex = 0
-        self.bisectButton.on_click(self.next_step)
+        self.bisect_button.pointIndex = 0
+        self.bisect_button.on_click(self.next_step)
 
         # Secant Button
-        self.secantButton = widgets.Button(
+        self.secant_button = widgets.Button(
             description="Secant",
             disabled=False,
             tooltip="Secant",
         )
-        self.secantButton.pointIndex = 1
-        self.secantButton.on_click(self.next_step)
+        self.secant_button.pointIndex = 1
+        self.secant_button.on_click(self.next_step)
 
         # IQI Button
-        self.IQIButton = widgets.Button(
+        self.iqi_button = widgets.Button(
             description="IQI",
             disabled=False,
             tooltip="IQI",
         )
-        self.IQIButton.pointIndex = 2
-        self.IQIButton.on_click(self.next_step)
+        self.iqi_button.pointIndex = 2
+        self.iqi_button.on_click(self.next_step)
 
         # CHECKBOXES FOR FUNCTION BUTTONS
         # ==========================================================================
-        self.bisectCheckbox = widgets.Checkbox(
+        self.bisect_checkbox = widgets.Checkbox(
             value=False,
             description="Bisect",
             disabled=False,
             indent=False,
         )
         # On change of checkbox, function checkBoxChanged
-        self.bisectCheckbox.observe(self.checkBoxChanged, names="value")
+        self.bisect_checkbox.observe(self.checkbox_changed, names="value")
 
-        self.secantCheckbox = widgets.Checkbox(
+        self.secant_checkbox = widgets.Checkbox(
             value=False,
             description="Secant",
             disabled=False,
             indent=False,
         )
-        self.secantCheckbox.observe(self.checkBoxChanged, names="value")
+        self.secant_checkbox.observe(self.checkbox_changed, names="value")
 
-        self.IQICheckbox = widgets.Checkbox(
+        self.iqi_checkbox = widgets.Checkbox(
             value=False,
             description="IQI",
             disabled=False,
             indent=False,
         )
-        self.IQICheckbox.observe(self.checkBoxChanged, names="value")
+        self.iqi_checkbox.observe(self.checkbox_changed, names="value")
 
         # GRID
         # ==========================================================================
         self.grid = widgets.GridspecLayout(2, 2)
-        self.grid[0, 0] = widgets.VBox([self.Toolbar, self.Fig])
+        self.grid[0, 0] = widgets.VBox([self.toolbar, self.fig])
 
         # Text Outputs Group
-        textGroup = widgets.VBox(
-            [self.currentSolOut, self.helperOut, self.brentDekkerOut]
+        texts_group = widgets.VBox(
+            [self.current_solution_output, self.helper_output, self.brent_dekker_output]
         )
-        self.grid[1, 0] = textGroup
+        self.grid[1, 0] = texts_group
 
         # Buttons Group
         text1 = widgets.HTML(value="<b>Next Step Selector</b>")  # Next Step Selector
         text2 = widgets.HTML(value="<b>Draw Step?</b>")  # Draw Step?
         selectors = widgets.VBox(  # Next Step Selectors
-            [text1, self.bisectButton, self.secantButton, self.IQIButton]
+            [text1, self.bisect_button, self.secant_button, self.iqi_button]
         )
         checkboxes = widgets.VBox(
-            [text2, self.bisectCheckbox, self.secantCheckbox, self.IQICheckbox]
+            [text2, self.bisect_checkbox, self.secant_checkbox, self.iqi_checkbox]
         )
-        buttonsGroup = widgets.HBox([selectors, checkboxes])
+        buttons_group = widgets.HBox([selectors, checkboxes])
 
-        self.grid[0, 1] = buttonsGroup
+        self.grid[0, 1] = buttons_group
 
         # Reset and Revert Buttons Group
-        buttonsGroup2 = widgets.HBox(
+        buttons_group_2 = widgets.HBox(
             [
-                self.revertButton,
-                self.resetButton,
+                self.revert_button,
+                self.reset_button,
             ]
         )
-        self.grid[1, 1] = buttonsGroup2
+        self.grid[1, 1] = buttons_group_2
 
-    def defaultLines(self):
+    def default_lines(self):
         # 0. Horizontal Line f(x)=0
-        self.hLine = bq.Lines(  # Horizontal Line f(x)=0
+        self.horizontal_line = bq.Lines(  # Horizontal Line f(x)=0
             x=self.x,
             y=[0] * len(self.x),
             scales={"x": self.x_sc, "y": self.y_sc},
             enable_move=False,
             enable_add=False,
             colors=["Black"],
         )
         # 1. Function Line f(x)
-        self.functionLine = bq.Lines(  # Function Line f(x)
+        self.function_line = bq.Lines(  # Function Line f(x)
             x=self.x,
             y=list(map(self.f, self.x)),
             scales={"x": self.x_sc, "y": self.y_sc},
             labels=["f(x)"],
             display_legend=False,
             enable_move=False,
             enable_add=False,
@@ -274,93 +274,93 @@
             The button that was clicked
 
         Returns
         -------
         None.
         """
 
-        if self.hintStep is None:
+        if self.hint_step is None:
             return
-        self.revertStack.append(
+        self.revert_stack.append(
             [self.a, self.b, self.c, self.e, self.iterations]
         )  # Add the current state to the revert stack
 
         self.a = self.b  # Set a = b
         self.fa = self.fb  # Set f(a) = f(b)
 
-        newB = self.nextPoints_addition[b.pointIndex]  # Get the next point
+        new_point_b = self.next_points_addition[b.pointIndex]  # Get the next point
         self.b = (
-            newB
-            if abs(self.b - newB) > self.tolerance
+            new_point_b
+            if abs(self.b - new_point_b) > self.tolerance
             else self.b + np.sign(0.5 * (self.c - self.b)) * self.tolerance
         )  # If the new point is too close to the current point, move it a little bit
         self.fb = self.f(self.b)  # Set f(b) = f(newB)
         self.e = self.errs[b.pointIndex]  # Set e = error
 
         self.iterations += 1  # Increment the number of iterations
 
         # Section: Ext
-        self.sectionEXT()  # Update the section
+        self.section_ext()  # Update the section
         # Section: Int
-        self.sectionINT()  # Update the section
+        self.section_int()  # Update the section
 
         self.one_step()  # Update the plot
 
     def reset(self, b):
         """
         Reset everything to the initial state, this can be understood as reverting all the steps
         """
-        if len(self.revertStack) == 0:
+        if len(self.revert_stack) == 0:
             return
 
-        self.a, self.b, self.c, self.e, self.iterations = self.revertStack[
+        self.a, self.b, self.c, self.e, self.iterations = self.revert_stack[
             0
         ]  # Get the initial state
         self.fb = self.f(self.b)  # Set f(b) = f(newB)
         self.fa = self.f(self.a)  # Set f(a) = f(b)
         self.fc = self.f(self.c)  # Set f(c) = f(newC)
 
-        self.revertStack = []  # Clear the revert stack
+        self.revert_stack = []  # Clear the revert stack
         self.one_step()  # Update the plot
 
     def revert(self, b):
         """
         This method reverts the last step
         """
-        if len(self.revertStack) == 0:  # If there is no step to revert
+        if len(self.revert_stack) == 0:  # If there is no step to revert
             return
 
         (
             self.a,
             self.b,
             self.c,
             self.e,
             self.iterations,
-        ) = self.revertStack.pop()  # Get the last state
+        ) = self.revert_stack.pop()  # Get the last state
         self.fb = self.f(self.b)  # Set f(b) = f(newB)
         self.fa = self.f(self.a)  # Set f(a) = f(b)
         self.fc = self.f(self.c)  # Set f(c) = f(newC)
 
         self.one_step()  # Update the plot
 
     def one_step(self):
         """
         This method is called when a step is made
         """
         with self.grid.hold_sync():  # Hold the grid syncronized
-            self.brent_dekker_Step()  # Update the Brent-Dekker step
-            self.IQIButton.disabled = (
-                self.nextPoints_addition[2] is None
+            self.brent_dekker_step()  # Update the Brent-Dekker step
+            self.iqi_button.disabled = (
+                self.next_points_addition[2] is None
             )  # Disable the IQI button if the IQI point is None
-            self.IQICheckbox.disabled = (
-                self.nextPoints_addition[2] is None
+            self.iqi_checkbox.disabled = (
+                self.next_points_addition[2] is None
             )  # Disable the IQI checkbox if the IQI point is None
 
             self.update_ouputs()  # Update the outputs
-            with self.Fig.hold_sync():  # Hold the figure syncronized
+            with self.fig.hold_sync():  # Hold the figure syncronized
                 self.draw_figures()  # Draw the figures
             # self.drawFigures()
 
     def draw_figures(self):
         """
         This method draws the figures
         1. The function
@@ -394,106 +394,115 @@
                 colors=["red"],
                 display_legend=True,
                 labels=["Secant Line"],
                 line_style="dashed",
             )  # Draw a line
             return secant
 
-        def bisect_draw(m, minY, maxY):
+        def bisect_draw(m, min_y, max_y):
             # m = (a + b) / 2
             # draw a vertical line at m
             bisect = bq.Lines(
                 x=[m, m],
-                y=[minY, maxY],
+                y=[min_y, max_y],
                 scales={"x": self.x_sc, "y": self.y_sc},
                 colors=["green"],
                 display_legend=True,
                 labels=["Bisect Line"],
                 line_style="dashed",
             )  # Draw a line
             return bisect
 
-        def iqi_draw(a, b, c, minY, maxY):
+        def iqi_draw(a, b, c, min_y, max_y):
             # draw a vertical line at m
-            interpolY = [self.f(a), self.f(b), self.f(c)]  # [f(a), f(b), f(c)]
-            interpolX = [a, b, c]  # [a, b, c]
-            yMesh = np.linspace(minY, maxY, 1000)
+            inperpolation_y = [self.f(a), self.f(b), self.f(c)]  # [f(a), f(b), f(c)]
+            interpolation_x = [a, b, c]  # [a, b, c]
+            y_mesh = np.linspace(min_y, max_y, 1000)
             # Lagrange interpolation with (Y,X)
             q_y = (  # Lagrange interpolation
-                lambda y: ((y - interpolY[1]) * (y - interpolY[2]))
-                / ((interpolY[0] - interpolY[1]) * (interpolY[0] - interpolY[2]))
-                * interpolX[0]
-                + ((y - interpolY[0]) * (y - interpolY[2]))
-                / ((interpolY[1] - interpolY[0]) * (interpolY[1] - interpolY[2]))
-                * interpolX[1]
-                + ((y - interpolY[0]) * (y - interpolY[1]))
-                / ((interpolY[2] - interpolY[0]) * (interpolY[2] - interpolY[1]))
-                * interpolX[2]
+                lambda y: ((y - inperpolation_y[1]) * (y - inperpolation_y[2]))
+                / (
+                    (inperpolation_y[0] - inperpolation_y[1])
+                    * (inperpolation_y[0] - inperpolation_y[2])
+                )
+                * interpolation_x[0]
+                + ((y - inperpolation_y[0]) * (y - inperpolation_y[2]))
+                / (
+                    (inperpolation_y[1] - inperpolation_y[0])
+                    * (inperpolation_y[1] - inperpolation_y[2])
+                )
+                * interpolation_x[1]
+                + ((y - inperpolation_y[0]) * (y - inperpolation_y[1]))
+                / (
+                    (inperpolation_y[2] - inperpolation_y[0])
+                    * (inperpolation_y[2] - inperpolation_y[1])
+                )
+                * interpolation_x[2]
             )
-            xMesh = q_y(yMesh)  # Get the x values for the y values
-            xMesh = np.where(
-                (xMesh < self.x[0]) | (xMesh > self.x[-1]), np.nan, xMesh
+            x_mesh = q_y(y_mesh)  # Get the x values for the y values
+            x_mesh = np.where(
+                (x_mesh < self.x[0]) | (x_mesh > self.x[-1]), np.nan, x_mesh
             )  # Set the x values outside the range to nan
-            IQILine = bq.Lines(  # Draw a line
-                x=xMesh,
-                y=yMesh,
+            iqi_line = bq.Lines(  # Draw a line
+                x=x_mesh,
+                y=y_mesh,
                 scales={"x": self.x_sc, "y": self.y_sc},
                 colors=["blue"],
                 display_legend=True,
                 labels=["IQI Line"],
                 line_style="dashed",
             )
-            return IQILine
+            return iqi_line
 
         points2check = [  # Points to check
             self.a,
             self.b,
             self.c,
-            self.nextPoints_addition[0],
-            self.nextPoints_addition[1],
+            self.next_points_addition[0],
+            self.next_points_addition[1],
         ] + (
             []
-            if self.nextPoints_addition[2] is None
+            if self.next_points_addition[2] is None
             else [
-                self.nextPoints_addition[2]
+                self.next_points_addition[2]
             ]  # If the IQI point is None, add it to the list
         )
 
-        if self.hintStep is None:  # If the hint step is None
-            self.Fig.marks = [
-                self.hLine,
-                self.functionLine,
+        if self.hint_step is None:  # If the hint step is None
+            self.fig.marks = [
+                self.horizontal_line,
+                self.function_line,
             ]  # Set the marks to the function and the horizontal line
             return
 
-        minMax = [
+        min_max = [
             min(points2check),
             max(points2check),
         ]  # Get the min and max of the points to check
 
-        if minMax[0] < min(self.original_data) or minMax[1] > max(
+        if min_max[0] < min(self.original_data) or min_max[1] > max(
             self.original_data
         ):  # If the min or max of the points to check is outside the range of the original data
             self.x = np.linspace(  # Set the x values to the min and max of the points to check
-                min(min(self.original_data), minMax[0]),
-                max(max(self.original_data), minMax[1]),
+                min(min(self.original_data), min_max[0]),
+                max(max(self.original_data), min_max[1]),
                 1000,
             )
-            self.defaultLines()  # Set the default lines
+            self.default_lines()  # Set the default lines
             self.widen = True  # Set widen to True
         elif self.widen:  # If widen is True
             self.x = np.linspace(
                 min(self.original_data), max(self.original_data), 1000
             )  # Set the x values to the min and max of the original data
-            self.defaultLines()  # Set the default lines
+            self.default_lines()  # Set the default lines
             self.widen = False  # Set widen to False
 
         marks2plot = [
-            self.hLine,
-            self.functionLine,
+            self.horizontal_line,
+            self.function_line,
         ]  # Set the marks to the function and the horizontal line
 
         # 1. The Current Points (a,b,c)
         marks2plot.append(
             draw_point(
                 self.a, self.fa, "red", "a", "circle", legend=False
             )  # Draw a point
@@ -513,113 +522,113 @@
                 self.c, self.fc, "green", "c", "circle", legend=False
             )  # Draw a point
         )
 
         # 2. The next step suggestions
         marks2plot.append(  # Bisect
             draw_point(
-                self.nextPoints_addition[0],
+                self.next_points_addition[0],
                 0,
                 "green",
                 "Bisection",
                 "rectangle",
             )
         )
         marks2plot.append(
             draw_point(  # Secant
-                self.nextPoints_addition[1],
+                self.next_points_addition[1],
                 0,
                 "red",
                 "Secant",
                 "triangle-up",
             )
         )
-        if self.nextPoints_addition[2] is not None:
+        if self.next_points_addition[2] is not None:
             marks2plot.append(
                 draw_point(  # IQI
-                    self.nextPoints_addition[2],
+                    self.next_points_addition[2],
                     0,
                     "blue",
                     "IQI",
                     "triangle-down",
                 )
             )
 
         # FIX THE VIEW
-        self.x_sc.min = minMax[
+        self.x_sc.min = min_max[
             0
         ]  # Set the x scale min to the min of the points to check
-        self.x_sc.max = minMax[
+        self.x_sc.max = min_max[
             1
         ]  # Set the x scale max to the max of the points to check
 
         self.y_sc.min = min(
-            self.f(minMax[0]), self.f(minMax[1])
+            self.f(min_max[0]), self.f(min_max[1])
         )  # Set the y scale min to the min of the function of the min and max of the points to check
         self.y_sc.max = max(
-            self.f(minMax[0]), self.f(minMax[1])
+            self.f(min_max[0]), self.f(min_max[1])
         )  # Set the y scale max to the max of the function of the min and max of the points to check
 
-        fX = list(map(self.f, self.x))  # Get the function values for the x values
-        yminMax = (min(fX), max(fX))  # Get the min and max of the function values
+        fx = list(map(self.f, self.x))  # Get the function values for the x values
+        y_min_max = (min(fx), max(fx))  # Get the min and max of the function values
 
         # 3. The steps
-        if self.secantCheckbox.value:  # If the secant checkbox is checked
+        if self.secant_checkbox.value:  # If the secant checkbox is checked
             marks2plot.append(secant_draw())  # Draw the secant line
 
-        if self.bisectCheckbox.value:  # If the bisect checkbox is checked
+        if self.bisect_checkbox.value:  # If the bisect checkbox is checked
             marks2plot.append(  # Draw the bisect line
                 bisect_draw(
-                    self.nextPoints_addition[0], yminMax[0], yminMax[1]
+                    self.next_points_addition[0], y_min_max[0], y_min_max[1]
                 )  # Draw the bisect line
             )
         if (
-            self.IQICheckbox.value and self.nextPoints_addition[2] is not None
+            self.iqi_checkbox.value and self.next_points_addition[2] is not None
         ):  # If the IQI checkbox is checked and the IQI point is not None
             marks2plot.append(
-                iqi_draw(self.a, self.b, self.c, yminMax[0], yminMax[1])
+                iqi_draw(self.a, self.b, self.c, y_min_max[0], y_min_max[1])
             )  # Draw the IQI line
 
-        self.Fig.marks = marks2plot  # Set the marks to the marks to plot
+        self.fig.marks = marks2plot  # Set the marks to the marks to plot
 
     def update_ouputs(self):
         """
         This method updates the outputs of the app
             > current solution
             > helper text
         The next step must be calculated before calling this method
         """
-        self.currentSolOut.clear_output()  # Clear the current solution output
-        self.helperOut.clear_output()  # Clear the helper output
+        self.current_solution_output.clear_output()  # Clear the current solution output
+        self.helper_output.clear_output()  # Clear the helper output
 
-        with self.currentSolOut:  # Print the current solution
+        with self.current_solution_output:  # Print the current solution
             print(
                 f"Current Solution: ({self.b:.4e}, {self.f(self.b):.4e})"
             )  # Print the current solution
             print(f"Iterations: {self.iterations}")  # Print the iterations
-        with self.helperOut:  # Print the helper text
+        with self.helper_output:  # Print the helper text
             print(  # Print the helper text
-                f"Next Step suggestion: {self.hintStep if self.hintStep is not None else 'FINISHED'}"
+                f"Next Step suggestion: {self.hint_step if self.hint_step is not None else 'FINISHED'}"
             )
 
     def run(self):
         """
         This method sets up everything and runs the app
 
         Returns
         -------
         Widgets.GridBox
             The GridBox containing all the widgets
         """
-        self.initializeComponents()  # Initialize the components
+        self.initialize_components()  # Initialize the components
         self.one_step()  # Run one step
 
         return self.grid
 
-    def brent_dekker_Step(self):
+    def brent_dekker_step(self):
         """
         This method imitates the Brent-Dekker in one step, instead of giving the result point, this method returns the 3 available points for the next step as well as the next possible step
 
         Returns
         -------
         - next_step: str
             The next possible step
@@ -629,33 +638,33 @@
             The errors of the 3 available points for the next step
         """
         self.tolerance = 2 * np.finfo(float).eps * abs(self.b) + self.t
         ## Midpoint error
         m = 0.5 * (self.c - self.b)
 
         if abs(m) <= self.tolerance or self.f(self.b) == 0 or self.f(self.a) == 0:
-            self.hintStep = None
-            self.nextPoints_addition = [None, None, None]
+            self.hint_step = None
+            self.next_points_addition = [None, None, None]
             self.errs = [None, None, None]
             self.update_ouputs()
             return
 
         next_step = None
-        nextPoints_addition = [None, None, None]
+        next_points_addition = [None, None, None]
         errs = [None, None, None]
 
-        nextPoints_addition[0] = self.b + m  # Always exists
+        next_points_addition[0] = self.b + m  # Always exists
         errs[0] = m  # Always exists
 
         # See if Bisection is possible
         # CHECK abs(self.e) < self.tolerance or abs(self.fa) <= abs(self.fb) in the original code
         # Here we do nothing because it is the midpoint - only thing next_step is Bisection (which will be default if secant/iqi fails)
 
         s = self.fb / self.fa
-        pqPair = None
+        pq_pair = None
         if self.a == self.c:
             # Linear Interpolation (Secant)
             p1 = 2 * m * s
             q1 = 1 - s
 
         else:
             # Linear Interpolation (Secant)
@@ -670,42 +679,42 @@
 
             # Correct signs of IQI
             if p2 > 0:
                 q2 = -q2
             else:
                 p2 = -p2
 
-            pqPair = (p2, q2)
+            pq_pair = (p2, q2)
 
         if p1 > 0:
             q1 = -q1
         else:
             p1 = -p1
 
         # Store e-Values for next step
         errs[1] = abs(p1 / q1)  # Secant always exists
         errs[2] = (
-            None if pqPair is None else abs(pqPair[0] / pqPair[1])
+            None if pq_pair is None else abs(pq_pair[0] / pq_pair[1])
         )  # IQI may not exist if a==c if it does, it is stored in pqPair
 
         # Store next points (Quantity to add) for next step
-        nextPoints_addition[1] = self.b + p1 / q1  # Secant always exists
-        nextPoints_addition[2] = (
-            None if pqPair is None else self.b + pqPair[0] / pqPair[1]
+        next_points_addition[1] = self.b + p1 / q1  # Secant always exists
+        next_points_addition[2] = (
+            None if pq_pair is None else self.b + pq_pair[0] / pq_pair[1]
         )  # IQI may not exist if a==c if it does, it is stored in pqPair
-        pqPair = (
-            (p1, q1) if pqPair is None else pqPair
+        pq_pair = (
+            (p1, q1) if pq_pair is None else pq_pair
         )  # If IQI does not exist, use Secant instead (pqPair is None if IQI does not exist), otherwise use IQI (pqPair is not None if IQI exists)
 
         # Choose the best interpolation
-        if 2 * pqPair[0] < 3 * m * pqPair[1] - abs(
-            self.tolerance * pqPair[1]
-        ) and pqPair[0] < abs(0.5 * self.e * pqPair[1]):
+        if 2 * pq_pair[0] < 3 * m * pq_pair[1] - abs(
+            self.tolerance * pq_pair[1]
+        ) and pq_pair[0] < abs(0.5 * self.e * pq_pair[1]):
             next_step = "IQI" if self.a != self.c else "Secant"
         else:
             next_step = "Bisection"
 
-        self.hintStep = next_step
-        self.nextPoints_addition = nextPoints_addition
+        self.hint_step = next_step
+        self.next_points_addition = next_points_addition
         self.errs = errs
 
-        return next_step, nextPoints_addition, errs
+        return next_step, next_points_addition, errs
```

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet/module.py` & `BNumMet-1.0.0.dev7/src/BNumMet/module.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet.egg-info/PKG-INFO` & `BNumMet-1.0.0.dev7/src/BNumMet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BNumMet
-Version: 1.0.0.dev6
+Version: 1.0.0.dev7
 Summary: Basic Numerical Methods for Python 3
 Home-page: https://github.com/fbpazos/Trabajo-Fin-Master/tree/main/Python_BNumMet
 Author: Fernando Bellido Pazos
 Author-email: fbellidopazos@gmail.com
 License: AGPL-3.0
 Platform: unix
 Platform: linux
@@ -227,15 +227,15 @@
 # Plotting using Matplotlib
 plt.plot(u, v, "b-", label="Interpolated")
 plt.plot(x, y, "ro", label="Original Points")
 plt.legend()
 plt.show()
 ```
 
-![Interpolation](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Interpolation/PCHIP%20Example%201.png?token=GHSAT0AAAAAAB4UDLTP2QAM3MIK5XNV3UQ2ZBKWKMQ)
+![Interpolation](https://dub07pap002files.storage.live.com/y4m52-hsxWxH8zjFakW7db0zDr1AGGI4j3VL3PTT_g5KO0AiotCnUBwwO5I9sSXIToLvJnfWtCBaOyZLukE_JBryO-JNNkodo2W0xjneL0cDoDy3CZaoFC-d8N0XbkOAWYjZgcu3M1K-j74BgEXUL5-oV6S_yLayyCtUl30xP6BPlC6bio1ZqPtqs2mARBgEP7e?encodeFailures=1&width=543&height=413)
 
 ### Non-Linear
 
 ```python
 from BNumMet.NonLinear import zBrentDekker
 fun = lambda x: x**2 - 2
 interval = [1, 2]
@@ -256,60 +256,60 @@
         marsaglia_rand(base=41, lag_r=2, lag_s=1, carry=0, seed_tuple=(0, 1)),
     )
     for i in range(100000)
 ]
 plt.scatter(*zip(*fail), s=1, c="black")
 plt.show()
 ```
-![Randomness](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Randomness/Marsaglia%20Rand%20Example%203.png?token=GHSAT0AAAAAAB4UDLTPNUUF6YTR75GHN7CCZBKWMCQ)
+![Randomness](https://dub07pap002files.storage.live.com/y4mzE0abSi6MSC6wlcNO6cc7HkixFGCybt2guF2nrsuJevEeYJ01VOcaZ244FjFpN27PlSrAUucq_62p8wlyPdlkW1hEGJTD2ngxsI5DX8KtFOGtFqfHSyijZiYvKO4D2QoeURctNgIbgg75bzDNkiYWIjcJhXbwdipgxoLEuQItQBXjEX3vGcH134768ZZXfF_?encodeFailures=1&width=547&height=413)
 
 ### Visualizers
 #### Linear Systems
 ```python
 from BNumMet.Visualizers.LUVisualizer import LUVisualizer
 luVisualizer = LUVisualizer()
 display(luVisualizer.run())
 ```
-![LUVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/LUVisualizer/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTPYKFM4QBOJKB4RDGQZBKWNDQ)
+![LUVisualizer](https://dub07pap002files.storage.live.com/y4m1q7uSd3dG2sMftf0YKDwNnz7aLGBnXeclboMbvU5un83LIpfX4Pw-8MJCHRzYcwLocDkZ1BeeAEx3qaowz7GUROV2rDzAYvmCcDEMw-X9P2HzXU9U3BzSMAQISEyUxxvVp3aNi46blEf1c1Liw_cADasxsqjOaZwwrrwTP7x7awPTudf0z4GwEmO2RH_akoB?encodeFailures=1&width=1080&height=404)
 
 #### Interpolation
 ```python
 from BNumMet.Visualizers.InterpolationVisualizer import InterpolVisualizer
 interpolVisualizer = InterpolVisualizer()
 display(interpolVisualizer.run())
 ```
-![interpolVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/Interpolation/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTOLYUOFN2JCWWDMMNWZBKWNPA)
+![interpolVisualizer](https://dub07pap002files.storage.live.com/y4mIg9iw5xzbHxOkHF5tfZGqdjS2yob1Zzd6LXkedOdQE8RBt54lqqfLUX8XB2113dOYLKqzjph5GDzoYvp-Qf7uaqL8NQ_GH0CBYfTQNT1FIqB6Yn-KO4dT78rau9Ka1FfR5zsbToR24NJnkJX5jy-xymWato5cUJ4aDJqAz_ENPJA2n1nNkCaFQ7WX58tmqzz?encodeFailures=1&width=952&height=551)
 
 
 #### Non-Linear
 ```python
 from BNumMet.Visualizers.NonLinearVisualizer import NonLinearVisualizer
 zerosVisualizer = NonLinearVisualizer()
 zerosVisualizer.run()
 ```
-![zerosVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/NonLinear/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTONMMPKCLJ6ESNJKC4ZBKWOXA)
+![zerosVisualizer](https://dub07pap002files.storage.live.com/y4m1UJWkc5j50NF4KZd1w9VENgIqMT-GMjhE-qhKLIdF3K-ymR4Rttav5ZwUjSaCDFzuz0mYyDPS-5MBo89JEyTOO-P5PdwXoJN4rCO1vlrn_MxwTHLsscwHGFITW_0KwLW1cWi0u5EAtXphyBQf_tCH-OT5aqPQT8TS6urP1bgeHDrmAm6twsn0E2AqWKhbMpX?encodeFailures=1&width=864&height=711)
 
 
 #### Least Squares
 ```python
 from BNumMet.Visualizers.LeastSquaresVisualizer import LSPVisualizer
 xData = np.array([0, 1, 2, 3, 4, 5])
 yData = np.array([4.5, 2.4, 1.5, 1, 1.5, 2.4])
 lspVisualizer = LSPVisualizer(xData, yData)
 lspVisualizer.run()
 ```
-![lspVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/LeastSquares/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTOGS7TTRSRNDBCS4KCZBKWPSA)
+![lspVisualizer](https://dub07pap002files.storage.live.com/y4mJQgX2hkcE5PU_vExDNiJb3-xPapyxDQqf7yZbw1uJ3kkxv5gxwsmYb13hUqf_IYyxdp9cZJHUP4UPYCuXzXs_hh27XFdwF5e6DsQSr0JGfKQhxivPBD6B_90wSpatlXWFG47NPzC5SxsDcM8Mj0u50hQUCGdXsbpGHHY5eDnB-CL_E2I1F0F0CkNPnAna5XW?encodeFailures=1&width=794&height=465)
 
 #### Randomness
 ```python
 from BNumMet.Visualizers.RandomVisualizer import RandomVisualizer
 randomVisualizer = RandomVisualizer()
 randomVisualizer.run()
 ```
-![randomVisualizer](https://raw.githubusercontent.com/fbpazos/Trabajo-Fin-Master/main/Latex/Include/Images/Thesis/Documentation/Visualizers/Randomness/Example%201/Example%201%20-%2000%20-%20Initial%20State.png?token=GHSAT0AAAAAAB4UDLTPTJFHTKTPLC43VJQAZBKWQHQ)
+![randomVisualizer](https://dub07pap002files.storage.live.com/y4mE3vUbK5Q6OnxGwiw3aQCfp8TrjYyo9mNdVMs1qjLWA3hNpGcLtisRHQZRXQEOEmdU3b3LLH4OLDgfgUFT2GrO4ktOIa6nyKB10ICQR_WIEyS-LPyM1NDXdEmKhe8uafPjJdJy8-fJI9y9t-tiuOaDZFGedaHBDfFZCvTZbYKvHgDmRrqycXAp7vx1lesvPLv?encodeFailures=1&width=722&height=758)
```

### Comparing `BNumMet-1.0.0.dev6/src/BNumMet.egg-info/SOURCES.txt` & `BNumMet-1.0.0.dev7/src/BNumMet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/tests/test_General.py` & `BNumMet-1.0.0.dev7/tests/test_General.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/tests/test_Interpolation.py` & `BNumMet-1.0.0.dev7/tests/test_Interpolation.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/tests/test_LeastSquares.py` & `BNumMet-1.0.0.dev7/tests/test_LeastSquares.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/tests/test_LinealSystems.py` & `BNumMet-1.0.0.dev7/tests/test_LinealSystems.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev6/tests/test_NonLinear.py` & `BNumMet-1.0.0.dev7/tests/test_NonLinear.py`

 * *Files 9% similar despite different names*

```diff
@@ -163,24 +163,24 @@
             f, interval, iters=True, steps=True, tol=tol
         )
         nonLinearVisualizer = NonLinearVisualizer(f, interval, tol=tol)
         nonLinearVisualizer.run()
 
         iters = 0
         guiStack = []
-        while nonLinearVisualizer.hintStep != None:
-            if nonLinearVisualizer.hintStep == "Bisection":
+        while nonLinearVisualizer.hint_step != None:
+            if nonLinearVisualizer.hint_step == "Bisection":
                 guiStack.append("Bisection")
-                nonLinearVisualizer.bisectButton.click()
-            elif nonLinearVisualizer.hintStep == "Secant":
+                nonLinearVisualizer.bisect_button.click()
+            elif nonLinearVisualizer.hint_step == "Secant":
                 guiStack.append("Secant")
-                nonLinearVisualizer.secantButton.click()
-            elif nonLinearVisualizer.hintStep == "IQI":
+                nonLinearVisualizer.secant_button.click()
+            elif nonLinearVisualizer.hint_step == "IQI":
                 guiStack.append("IQI")
-                nonLinearVisualizer.IQIButton.click()
+                nonLinearVisualizer.iqi_button.click()
             iters += 1
 
             if iters > itersbrentt:
                 self.fail(
                     "NonLinearVisualizer did not converge to the same value as zBrentDekker"
                 )
 
@@ -196,56 +196,56 @@
         tol = 1e-20
         x, iters, stack = zBrentDekker(f, interval, iters=True, steps=True, tol=tol)
         nonLinearVisualizer = NonLinearVisualizer(f, interval, tol=tol)
         nonLinearVisualizer.run()
 
         # Perform all steps and store them in a stack
         guiStack = []
-        while nonLinearVisualizer.hintStep != None:
-            guiStack.append(nonLinearVisualizer.hintStep)
-            if nonLinearVisualizer.hintStep == "Bisection":
-                nonLinearVisualizer.bisectButton.click()
-            elif nonLinearVisualizer.hintStep == "Secant":
-                nonLinearVisualizer.secantButton.click()
-            elif nonLinearVisualizer.hintStep == "IQI":
-                nonLinearVisualizer.IQIButton.click()
+        while nonLinearVisualizer.hint_step != None:
+            guiStack.append(nonLinearVisualizer.hint_step)
+            if nonLinearVisualizer.hint_step == "Bisection":
+                nonLinearVisualizer.bisect_button.click()
+            elif nonLinearVisualizer.hint_step == "Secant":
+                nonLinearVisualizer.secant_button.click()
+            elif nonLinearVisualizer.hint_step == "IQI":
+                nonLinearVisualizer.iqi_button.click()
 
         # Revert the last step and check if the hintStep is the same as the future step in the stack
         i = len(guiStack) - 1
-        while nonLinearVisualizer.revertStack != []:
-            nonLinearVisualizer.revertButton.click()
+        while nonLinearVisualizer.revert_stack != []:
+            nonLinearVisualizer.revert_button.click()
             i -= 1
-            self.assertTrue(nonLinearVisualizer.hintStep == stack[i + 1])
+            self.assertTrue(nonLinearVisualizer.hint_step == stack[i + 1])
 
     def test_reset(self):
         """
         Tests if the reset method works correctly
         """
         f = lambda x: x**2 - 1
         interval = (0, 2)
         tol = 1e-20
         x, iters, stack = zBrentDekker(f, interval, iters=True, steps=True, tol=tol)
         nonLinearVisualizer = NonLinearVisualizer(f, interval, tol=tol)
         nonLinearVisualizer.run()
 
         # Perform all steps and store them in a stack
         guiStack = []
-        while nonLinearVisualizer.hintStep != None:
-            guiStack.append(nonLinearVisualizer.hintStep)
-            if nonLinearVisualizer.hintStep == "Bisection":
-                nonLinearVisualizer.bisectButton.click()
-            elif nonLinearVisualizer.hintStep == "Secant":
-                nonLinearVisualizer.secantButton.click()
-            elif nonLinearVisualizer.hintStep == "IQI":
-                nonLinearVisualizer.IQIButton.click()
+        while nonLinearVisualizer.hint_step != None:
+            guiStack.append(nonLinearVisualizer.hint_step)
+            if nonLinearVisualizer.hint_step == "Bisection":
+                nonLinearVisualizer.bisect_button.click()
+            elif nonLinearVisualizer.hint_step == "Secant":
+                nonLinearVisualizer.secant_button.click()
+            elif nonLinearVisualizer.hint_step == "IQI":
+                nonLinearVisualizer.iqi_button.click()
 
         # A Reset should revert all steps and set the hintStep to the first step in the stack
-        nonLinearVisualizer.resetButton.click()
-        self.assertEqual(nonLinearVisualizer.revertStack, [])
-        self.assertTrue(nonLinearVisualizer.hintStep == stack[0])
+        nonLinearVisualizer.reset_button.click()
+        self.assertEqual(nonLinearVisualizer.revert_stack, [])
+        self.assertTrue(nonLinearVisualizer.hint_step == stack[0])
 
         a = nonLinearVisualizer.a
         c = nonLinearVisualizer.c
         b = nonLinearVisualizer.b
 
         self.assertEqual(nonLinearVisualizer.a, nonLinearVisualizer.c)
         self.assertListEqual(sorted([a, b]), list(nonLinearVisualizer.original_data))
@@ -257,40 +257,40 @@
         f = lambda x: x**2 - 1
         interval = (0, 2)
         tol = 1e-20
         x, iters, stack = zBrentDekker(f, interval, iters=True, steps=True, tol=tol)
         nonLinearVisualizer = NonLinearVisualizer(f, interval, tol=tol)
         nonLinearVisualizer.run()
 
-        og_length = len(nonLinearVisualizer.Fig.marks)
+        og_length = len(nonLinearVisualizer.fig.marks)
 
-        nonLinearVisualizer.bisectCheckbox.value = True
-        self.assertTrue(len(nonLinearVisualizer.Fig.marks) > og_length)
+        nonLinearVisualizer.bisect_checkbox.value = True
+        self.assertTrue(len(nonLinearVisualizer.fig.marks) > og_length)
 
-        nonLinearVisualizer.bisectCheckbox.value = False
-        self.assertEqual(len(nonLinearVisualizer.Fig.marks), og_length)
+        nonLinearVisualizer.bisect_checkbox.value = False
+        self.assertEqual(len(nonLinearVisualizer.fig.marks), og_length)
 
-        nonLinearVisualizer.secantCheckbox.value = True
-        self.assertTrue(len(nonLinearVisualizer.Fig.marks) > og_length)
+        nonLinearVisualizer.secant_checkbox.value = True
+        self.assertTrue(len(nonLinearVisualizer.fig.marks) > og_length)
 
         self.assertTrue(
-            nonLinearVisualizer.IQICheckbox.disabled
+            nonLinearVisualizer.iqi_checkbox.disabled
         )  # IQI is disabled by at first step of this function
         # Perform all steps and store them in a stack
         guiStack = []
-        while nonLinearVisualizer.hintStep != None:
-            guiStack.append(nonLinearVisualizer.hintStep)
-            if nonLinearVisualizer.hintStep == "Bisection":
-                nonLinearVisualizer.bisectButton.click()
-            elif nonLinearVisualizer.hintStep == "Secant":
-                nonLinearVisualizer.secantButton.click()
-            elif nonLinearVisualizer.hintStep == "IQI":
-                self.assertFalse(nonLinearVisualizer.IQICheckbox.disabled)
-                nonLinearVisualizer.IQICheckbox.value = True
-                self.assertTrue(len(nonLinearVisualizer.Fig.marks) > og_length)
+        while nonLinearVisualizer.hint_step != None:
+            guiStack.append(nonLinearVisualizer.hint_step)
+            if nonLinearVisualizer.hint_step == "Bisection":
+                nonLinearVisualizer.bisect_button.click()
+            elif nonLinearVisualizer.hint_step == "Secant":
+                nonLinearVisualizer.secant_button.click()
+            elif nonLinearVisualizer.hint_step == "IQI":
+                self.assertFalse(nonLinearVisualizer.iqi_checkbox.disabled)
+                nonLinearVisualizer.iqi_checkbox.value = True
+                self.assertTrue(len(nonLinearVisualizer.fig.marks) > og_length)
                 break
 
     def test_sign_not_guranteed(self):
         """
         Raise exception if signs are the same
         """
         f = lambda x: x**2 - 1
@@ -324,17 +324,17 @@
         interval = (0, 2)
         tol = 1e-20
         x, iters, stack = zBrentDekker(f, interval, iters=True, steps=True, tol=tol)
         nonLinearVisualizer = NonLinearVisualizer(f, interval, tol=tol)
         nonLinearVisualizer.run()
 
         # A Reset should revert all steps and set the hintStep to the first step in the stack
-        nonLinearVisualizer.resetButton.click()
-        self.assertEqual(nonLinearVisualizer.revertStack, [])
-        self.assertTrue(nonLinearVisualizer.hintStep == stack[0])
+        nonLinearVisualizer.reset_button.click()
+        self.assertEqual(nonLinearVisualizer.revert_stack, [])
+        self.assertTrue(nonLinearVisualizer.hint_step == stack[0])
 
     def test_exception_wrongSign(self):
         """
         Tests if the exception is raised when the signs are NOT different
         """
         f = lambda x: x**2 - 1
         interval = (2, 4)
```

### Comparing `BNumMet-1.0.0.dev6/tests/test_Random.py` & `BNumMet-1.0.0.dev7/tests/test_Random.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,56 +238,56 @@
 
 class test_RandomVisualizer(TestCase):
     def test_initiate(self):
         # Tests that the RandomVisualizer is initiated correctly without any arguments
         # No Exceptions should be raised
         rv = RandomVisualizer()
 
-        self.assertTrue(len(rv.generatedNumbers) == 0)
+        self.assertTrue(len(rv.generated_numbers) == 0)
         self.assertEqual(rv.iterations, 100)
 
-        random_float = rv.randGenerator()
+        random_float = rv.random_generator()
         self.assertGreaterEqual(random_float, 0)
         self.assertLessEqual(random_float, 1)
 
     def test_initiate_with_args(self):
         # Tests that the RandomVisualizer is initiated correctly with arguments
         # No Exceptions should be raised
-        rv = RandomVisualizer(randGenerator=Random.marsaglia_rand)
+        rv = RandomVisualizer(random_generator=Random.marsaglia_rand)
 
-        self.assertTrue(len(rv.generatedNumbers) == 0)
+        self.assertTrue(len(rv.generated_numbers) == 0)
         self.assertEqual(rv.iterations, 100)
 
-        random_float = rv.randGenerator()
+        random_float = rv.random_generator()
         self.assertGreaterEqual(random_float, 0)
         self.assertLessEqual(random_float, 1)
 
     def test_run_no_exception(self):
         # Tests that the RandomVisualizer is initiated correctly without any arguments
         # No Exceptions should be raised
         rv = RandomVisualizer()
         rv.run()
 
     def test_play(self):
         # Tests that the RandomVisualizer is initiated correctly without any arguments
         # No Exceptions should be raised
         rv = RandomVisualizer()
         rv.run()
-        rv.runButton.click()
+        rv.run_button.click()
 
-        self.assertTrue(rv.currentValue - np.pi < 0.7)
+        self.assertTrue(rv.current_value - np.pi < 0.7)
 
     def test_int_text(self):
         # Tests that the RandomVisualizer is initiated correctly without any arguments
         # No Exceptions should be raised
         rv = RandomVisualizer()
         rv.run()
 
-        rv.iterationsWidget.value = 10000
+        rv.iterations_widget.value = 10000
         self.assertEqual(
-            rv.iterationsWidget.value, 1000
+            rv.iterations_widget.value, 1000
         )  # Should be 1000 because of the max value
 
-        rv.iterationsWidget.value = 0
+        rv.iterations_widget.value = 0
         self.assertEqual(
-            rv.iterationsWidget.value, 1
+            rv.iterations_widget.value, 1
         )  # Should be 1 because of the min value
```

