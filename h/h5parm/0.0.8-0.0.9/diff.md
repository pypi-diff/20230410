# Comparing `tmp/h5parm-0.0.8.tar.gz` & `tmp/h5parm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/h5parm-0.0.8.tar", last modified: Sun May 22 20:18:59 2022, max compression
+gzip compressed data, was "dist/h5parm-0.0.9.tar", last modified: Mon May 30 22:59:32 2022, max compression
```

## Comparing `h5parm-0.0.8.tar` & `h5parm-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-22 20:18:59.712034 h5parm-0.0.8/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1566 2022-05-22 20:18:59.712034 h5parm-0.0.8/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-0.0.8/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-22 20:18:59.712034 h5parm-0.0.8/h5parm/
--rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-0.0.8/h5parm/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-22 20:18:59.712034 h5parm-0.0.8/h5parm/arrays/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-0.0.8/h5parm/arrays/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-0.0.8/h5parm/arrays/dsa2000.W.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-0.0.8/h5parm/arrays/gmrtPos.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-0.0.8/h5parm/arrays/lofar.antenna.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-0.0.8/h5parm/arrays/lofar.hba.antenna.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)    33202 2021-06-02 01:08:45.000000 h5parm-0.0.8/h5parm/datapack.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-0.0.8/h5parm/maintenance.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12878 2022-05-22 20:13:46.000000 h5parm-0.0.8/h5parm/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-22 20:18:59.712034 h5parm-0.0.8/h5parm.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1566 2022-05-22 20:18:59.000000 h5parm-0.0.8/h5parm.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      388 2022-05-22 20:18:59.000000 h5parm-0.0.8/h5parm.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2022-05-22 20:18:59.000000 h5parm-0.0.8/h5parm.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        7 2022-05-22 20:18:59.000000 h5parm-0.0.8/h5parm.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2022-05-22 20:18:59.712034 h5parm-0.0.8/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     1201 2022-05-22 20:13:46.000000 h5parm-0.0.8/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-30 22:59:32.620300 h5parm-0.0.9/
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-0.0.9/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1385 2022-05-30 22:59:32.620300 h5parm-0.0.9/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-0.0.9/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-30 22:59:32.616300 h5parm-0.0.9/h5parm/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-30 22:59:32.620300 h5parm-0.0.9/h5parm/arrays/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/arrays/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-0.0.9/h5parm/arrays/dsa2000.W.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/arrays/gmrtPos.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/arrays/lofar.antenna.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/arrays/lofar.hba.antenna.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)    33202 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/datapack.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/maintenance.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12882 2022-05-30 22:59:05.000000 h5parm-0.0.9/h5parm/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-30 22:59:32.616300 h5parm-0.0.9/h5parm.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1385 2022-05-30 22:59:32.000000 h5parm-0.0.9/h5parm.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      396 2022-05-30 22:59:32.000000 h5parm-0.0.9/h5parm.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2022-05-30 22:59:32.000000 h5parm-0.0.9/h5parm.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        7 2022-05-30 22:59:32.000000 h5parm-0.0.9/h5parm.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2022-05-30 22:59:32.620300 h5parm-0.0.9/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     1201 2022-05-30 22:59:15.000000 h5parm-0.0.9/setup.py
```

### Comparing `h5parm-0.0.8/PKG-INFO` & `h5parm-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 0.0.8
+Version: 0.0.9
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 License: UNKNOWN
-Description: # h5parm
-        Provides H5Parm data interface
-        
-        # Example
-        
-        ```python
-        from h5parm.utils import make_example_datapack
-        from h5parm import DataPack
-        datapack = make_example_datapack(4,5,6)
-        #select your slices
-        datapack.select(ant="RS*", time=slice(0,None,2), freq=2)
-        ```
-        This will select all antennas with names starting with 'RS', every other time, and the 3rd frequency.
-        ```python
-        #get your soltab
-        phase, axes = datapack.phase
-        #get the coordinates of axes
-        patch_names, directions = datapack.get_directions(axes['dir'])
-        antenna_labels, antennas = datapack.get_antennas(axes['ant'])
-        timestamp, times = datapack.get_antennas(axes['time'])
-        freq_labels, freqs = datapack.get_freqs(axes['freq'])
-        pol_labels, pols = datapack.get_pols(axes['pol'])
-        ```
-        In general the first element returned by all `get_*` methods are string labels, and the second is a dimensionful `astropy` object, e.g. `ICRS` object, `Time` object etc.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# h5parm
+Provides H5Parm data interface
+
+# Example
+
+```python
+from h5parm.utils import make_example_datapack
+from h5parm import DataPack
+datapack = make_example_datapack(4,5,6)
+#select your slices
+datapack.select(ant="RS*", time=slice(0,None,2), freq=2)
+```
+This will select all antennas with names starting with 'RS', every other time, and the 3rd frequency.
+```python
+#get your soltab
+phase, axes = datapack.phase
+#get the coordinates of axes
+patch_names, directions = datapack.get_directions(axes['dir'])
+antenna_labels, antennas = datapack.get_antennas(axes['ant'])
+timestamp, times = datapack.get_antennas(axes['time'])
+freq_labels, freqs = datapack.get_freqs(axes['freq'])
+pol_labels, pols = datapack.get_pols(axes['pol'])
+```
+In general the first element returned by all `get_*` methods are string labels, and the second is a dimensionful `astropy` object, e.g. `ICRS` object, `Time` object etc.
+
+
```

### Comparing `h5parm-0.0.8/README.md` & `h5parm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.8/h5parm/arrays/dsa2000.W.cfg` & `h5parm-0.0.9/h5parm/arrays/dsa2000.W.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.8/h5parm/arrays/gmrtPos.cfg` & `h5parm-0.0.9/h5parm/arrays/gmrtPos.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.8/h5parm/arrays/lofar.antenna.cfg` & `h5parm-0.0.9/h5parm/arrays/lofar.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.8/h5parm/arrays/lofar.hba.antenna.cfg` & `h5parm-0.0.9/h5parm/arrays/lofar.hba.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.8/h5parm/datapack.py` & `h5parm-0.0.9/h5parm/datapack.py`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.8/h5parm/maintenance.py` & `h5parm-0.0.9/h5parm/maintenance.py`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.8/h5parm/utils.py` & `h5parm-0.0.9/h5parm/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,16 +281,16 @@
         if to_solset not in datapack.solsets:
             datapack.add_solset(to_solset,
                                 array_file=DataPack.lofar_array_hba,
                                 directions=np.stack([directions.ra.to(au.rad).value,
                                                      directions.dec.to(au.rad).value], axis=1),
                                 patch_names=patch_names)
         for soltab in to_soltab:
-            if not soltab.endswith("000"):
-                raise ValueError("By Losoto convention soltabs should end in XXX or similar. We only support XXX=000.")
+#             if not soltab.endswith("000"):
+#                 raise ValueError("By Losoto convention soltabs should end in XXX or similar. We only support XXX=000.")
             if 'tec' in soltab:
                 datapack.add_soltab(soltab, weightDtype='f16', time=times.mjd * 86400., pol=pol_labels,
                                     ant=antenna_labels,
                                     dir=patch_names)
             if 'clock' in soltab:
                 datapack.add_soltab(soltab, weightDtype='f16', time=times.mjd * 86400., pol=pol_labels,
                                     ant=antenna_labels, dir=patch_names)
```

### Comparing `h5parm-0.0.8/h5parm.egg-info/PKG-INFO` & `h5parm-0.0.9/h5parm.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 0.0.8
+Version: 0.0.9
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 License: UNKNOWN
-Description: # h5parm
-        Provides H5Parm data interface
-        
-        # Example
-        
-        ```python
-        from h5parm.utils import make_example_datapack
-        from h5parm import DataPack
-        datapack = make_example_datapack(4,5,6)
-        #select your slices
-        datapack.select(ant="RS*", time=slice(0,None,2), freq=2)
-        ```
-        This will select all antennas with names starting with 'RS', every other time, and the 3rd frequency.
-        ```python
-        #get your soltab
-        phase, axes = datapack.phase
-        #get the coordinates of axes
-        patch_names, directions = datapack.get_directions(axes['dir'])
-        antenna_labels, antennas = datapack.get_antennas(axes['ant'])
-        timestamp, times = datapack.get_antennas(axes['time'])
-        freq_labels, freqs = datapack.get_freqs(axes['freq'])
-        pol_labels, pols = datapack.get_pols(axes['pol'])
-        ```
-        In general the first element returned by all `get_*` methods are string labels, and the second is a dimensionful `astropy` object, e.g. `ICRS` object, `Time` object etc.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# h5parm
+Provides H5Parm data interface
+
+# Example
+
+```python
+from h5parm.utils import make_example_datapack
+from h5parm import DataPack
+datapack = make_example_datapack(4,5,6)
+#select your slices
+datapack.select(ant="RS*", time=slice(0,None,2), freq=2)
+```
+This will select all antennas with names starting with 'RS', every other time, and the 3rd frequency.
+```python
+#get your soltab
+phase, axes = datapack.phase
+#get the coordinates of axes
+patch_names, directions = datapack.get_directions(axes['dir'])
+antenna_labels, antennas = datapack.get_antennas(axes['ant'])
+timestamp, times = datapack.get_antennas(axes['time'])
+freq_labels, freqs = datapack.get_freqs(axes['freq'])
+pol_labels, pols = datapack.get_pols(axes['pol'])
+```
+In general the first element returned by all `get_*` methods are string labels, and the second is a dimensionful `astropy` object, e.g. `ICRS` object, `Time` object etc.
+
+
```

### Comparing `h5parm-0.0.8/setup.py` & `h5parm-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                   'tables>=' + __minimum_tables_version__,
                   'astropy>=' + __minimum_astropy_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='h5parm',
-      version='0.0.8',
+      version='0.0.9',
       description='H5Parm data pack interface',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/h5parm",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

