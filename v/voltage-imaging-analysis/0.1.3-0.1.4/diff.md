# Comparing `tmp/voltage_imaging_analysis-0.1.3.tar.gz` & `tmp/voltage_imaging_analysis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltage_imaging_analysis-0.1.3.tar", last modified: Tue Feb 14 19:08:28 2023, max compression
+gzip compressed data, was "voltage_imaging_analysis-0.1.4.tar", last modified: Mon Apr 10 18:31:32 2023, max compression
```

## Comparing `voltage_imaging_analysis-0.1.3.tar` & `voltage_imaging_analysis-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-02-14 19:08:28.450990 voltage_imaging_analysis-0.1.3/
--rw-r--r--   0 rrsims     (501) staff       (20)     6148 2023-02-14 19:04:04.000000 voltage_imaging_analysis-0.1.3/.DS_Store
--rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-02-14 19:08:28.450667 voltage_imaging_analysis-0.1.3/PKG-INFO
--rw-r--r--   0 rrsims     (501) staff       (20)      101 2023-02-07 14:38:32.000000 voltage_imaging_analysis-0.1.3/README.md
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-02-14 19:08:28.448606 voltage_imaging_analysis-0.1.3/dist/
--rw-r--r--   0 rrsims     (501) staff       (20)     9193 2023-02-07 21:30:21.000000 voltage_imaging_analysis-0.1.3/dist/voltage_imaging_analysis-0.1.0.tar.gz
--rw-r--r--   0 rrsims     (501) staff       (20)       38 2023-02-14 19:08:28.451046 voltage_imaging_analysis-0.1.3/setup.cfg
--rw-r--r--   0 rrsims     (501) staff       (20)      697 2023-02-14 19:08:22.000000 voltage_imaging_analysis-0.1.3/setup.py
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-02-14 19:08:28.449143 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis/
--rw-r--r--   0 rrsims     (501) staff       (20)      125 2023-02-07 21:36:16.000000 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis/__init__.py
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-02-14 19:08:28.450300 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis/__pycache__/
--rw-r--r--   0 rrsims     (501) staff       (20)      321 2023-02-07 14:49:20.000000 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rrsims     (501) staff       (20)    26837 2023-02-07 21:36:05.000000 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-02-14 19:08:28.450154 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis.egg-info/
--rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-02-14 19:08:28.000000 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis.egg-info/PKG-INFO
--rw-r--r--   0 rrsims     (501) staff       (20)      466 2023-02-14 19:08:28.000000 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 rrsims     (501) staff       (20)        1 2023-02-14 19:08:28.000000 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 rrsims     (501) staff       (20)        6 2023-02-14 19:08:28.000000 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis.egg-info/requires.txt
--rw-r--r--   0 rrsims     (501) staff       (20)       25 2023-02-14 19:08:28.000000 voltage_imaging_analysis-0.1.3/voltage_imaging_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.788876 voltage_imaging_analysis-0.1.4/
+-rw-r--r--   0 rrsims     (501) staff       (20)     6148 2023-02-14 19:09:47.000000 voltage_imaging_analysis-0.1.4/.DS_Store
+-rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:31:32.788665 voltage_imaging_analysis-0.1.4/PKG-INFO
+-rw-r--r--   0 rrsims     (501) staff       (20)      101 2023-02-07 14:38:32.000000 voltage_imaging_analysis-0.1.4/README.md
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.786944 voltage_imaging_analysis-0.1.4/dist/
+-rw-r--r--   0 rrsims     (501) staff       (20)     9193 2023-02-07 21:30:21.000000 voltage_imaging_analysis-0.1.4/dist/voltage_imaging_analysis-0.1.0.tar.gz
+-rw-r--r--   0 rrsims     (501) staff       (20)       38 2023-04-10 18:31:32.788934 voltage_imaging_analysis-0.1.4/setup.cfg
+-rw-r--r--   0 rrsims     (501) staff       (20)      697 2023-04-10 18:31:14.000000 voltage_imaging_analysis-0.1.4/setup.py
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.787434 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/
+-rw-r--r--   0 rrsims     (501) staff       (20)      125 2023-02-14 19:08:52.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/__init__.py
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.788307 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/__pycache__/
+-rw-r--r--   0 rrsims     (501) staff       (20)      321 2023-02-07 14:49:20.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rrsims     (501) staff       (20)    26949 2023-04-10 13:23:54.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:31:32.788154 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/
+-rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 rrsims     (501) staff       (20)      466 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 rrsims     (501) staff       (20)        1 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 rrsims     (501) staff       (20)        6 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/requires.txt
+-rw-r--r--   0 rrsims     (501) staff       (20)       25 2023-04-10 18:31:32.000000 voltage_imaging_analysis-0.1.4/voltage_imaging_analysis.egg-info/top_level.txt
```

### Comparing `voltage_imaging_analysis-0.1.3/.DS_Store` & `voltage_imaging_analysis-0.1.4/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 000d  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 000e  ................
 00000050: 0000 0001 0000 1000 496c 6f63 626c 6f62  ........Ilocblob
 00000060: 0000 0010 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -58,15 +58,15 @@
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 000d 0000 0004  ................
+00000400: 0000 0000 0000 0000 0000 000e 0000 0004  ................
 00000410: 0064 0069 0073 0074 496c 6f63 626c 6f62  .d.i.s.tIlocblob
 00000420: 0000 0010 0000 0041 0000 002e ffff ffff  .......A........
 00000430: ffff 0000 0000 0004 0064 0069 0073 0074  .........d.i.s.t
 00000440: 6277 7370 626c 6f62 0000 00c9 6270 6c69  bwspblob....bpli
 00000450: 7374 3030 d701 0203 0405 0607 0808 0a0a  st00............
 00000460: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
 00000470: 725b 5368 6f77 5061 7468 6261 725b 5368  r[ShowPathbar[Sh
@@ -116,20 +116,20 @@
 00000730: 6c00 7900 7300 6900 7370 6831 5363 6f6d  l.y.s.i.sph1Scom
 00000740: 7000 0000 0000 0000 0000 0000 2100 7600  p...........!.v.
 00000750: 6f00 6c00 7400 6100 6700 6500 5f00 6900  o.l.t.a.g.e._.i.
 00000760: 6d00 6100 6700 6900 6e00 6700 5f00 6100  m.a.g.i.n.g._.a.
 00000770: 6e00 6100 6c00 7900 7300 6900 7300 2e00  n.a.l.y.s.i.s...
 00000780: 6500 6700 6700 2d00 6900 6e00 6600 6f49  e.g.g.-.i.n.f.oI
 00000790: 6c6f 6362 6c6f 6200 0000 1000 0001 f900  locblob.........
-000007a0: 0000 2eff ffff ffff ff00 0000 0000 0000  ................
-000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007a0: 0000 2eff ffff ffff ff00 0000 0000 2100  ..............!.
+000007b0: 7600 6f00 6c00 7400 6100 6700 6500 5f00  v.o.l.t.a.g.e._.
+000007c0: 6900 6d00 6100 6700 6900 6e00 6700 5f00  i.m.a.g.i.n.g._.
+000007d0: 6100 6e00 6100 6c00 7900 7300 6900 7300  a.n.a.l.y.s.i.s.
+000007e0: 2e00 6500 6700 6700 2d00 6900 6e00 6600  ..e.g.g.-.i.n.f.
+000007f0: 6f64 7363 6c62 6f6f 6c00 0000 0000 0000  odsclbool.......
 00000800: 0000 0000 0000 0001 0000 0000 0000 080b  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `voltage_imaging_analysis-0.1.3/dist/voltage_imaging_analysis-0.1.0.tar.gz` & `voltage_imaging_analysis-0.1.4/dist/voltage_imaging_analysis-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `voltage_imaging_analysis-0.1.3/setup.py` & `voltage_imaging_analysis-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='voltage_imaging_analysis',
-    version='0.1.3',    
+    version='0.1.4',    
     description='Python package used for analysing voltage imaging data.',
     url='https://github.com/rrsims21/voltage_imaging_analysis/',
     author='Ruth Sims',
     author_email='ruth.sims@inserm.fr',
     license='BSD 2-clause',
     packages=['voltage_imaging_analysis'],
     install_requires=[
```

### Comparing `voltage_imaging_analysis-0.1.3/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py` & `voltage_imaging_analysis-0.1.4/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from sklearn import linear_model
 from matplotlib import pyplot as plt
 import sys
 from scipy import stats
 import statistics
 from scipy.spatial import distance
 
+# timings analysis:
+    # generate timeseries from stack 
+    # segmentation
+    # ... 
+    # take a long time
+
 def generate_timeseries_from_stack(stack_to_analyse, whiten_data=True, no_border_pixels=1):
 
     # segment image to get initial estimate of trace
     # use local correlation image for initial segmentations: expect pixels within cell to be more correlated with oneanother than noisy pixels outside cell
     local_correlation_img = compute_local_correlation_image(stack_to_analyse, no_neighbours=8, to_whiten_data=whiten_data)
 
     # remove edge artefact
```

