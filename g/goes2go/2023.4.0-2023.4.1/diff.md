# Comparing `tmp/goes2go-2023.4.0.tar.gz` & `tmp/goes2go-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goes2go-2023.4.0.tar", last modified: Mon Apr 10 16:52:01 2023, max compression
+gzip compressed data, was "goes2go-2023.4.1.tar", last modified: Mon Apr 10 19:04:41 2023, max compression
```

## Comparing `goes2go-2023.4.0.tar` & `goes2go-2023.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 16:52:01.000000 goes2go-2023.4.0/
--rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-03-07 22:50:31.000000 goes2go-2023.4.0/.gitattributes
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     2027 2023-02-02 16:15:19.000000 goes2go-2023.4.0/.gitignore
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1079 2023-02-02 16:12:51.000000 goes2go-2023.4.0/.readthedocs.yml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      977 2023-04-10 16:44:33.000000 goes2go-2023.4.0/CITATION.cff
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1076 2022-03-07 22:50:31.000000 goes2go-2023.4.0/LICENSE
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      102 2022-10-20 19:50:16.000000 goes2go-2023.4.0/MANIFEST.in
--rw-------   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-10 16:52:01.000000 goes2go-2023.4.0/PKG-INFO
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     8722 2023-02-02 16:12:51.000000 goes2go-2023.4.0/README.md
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     2393 2022-11-15 17:49:05.000000 goes2go-2023.4.0/environment-dev.yml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      747 2022-11-15 17:45:56.000000 goes2go-2023.4.0/environment-test-conda.yml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1038 2022-10-20 20:22:08.000000 goes2go-2023.4.0/environment-test.yml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1352 2023-02-02 16:28:56.000000 goes2go-2023.4.0/environment.yml
-drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 16:52:01.000000 goes2go-2023.4.0/goes2go/
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     7797 2022-10-20 15:16:21.000000 goes2go-2023.4.0/goes2go/NEW.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     3105 2023-03-20 15:41:44.000000 goes2go-2023.4.0/goes2go/__init__.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      166 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go/_version.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)    41053 2023-03-20 15:41:44.000000 goes2go-2023.4.0/goes2go/accessors.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)    21281 2023-03-20 15:46:12.000000 goes2go-2023.4.0/goes2go/data.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     6710 2022-05-12 15:43:43.000000 goes2go-2023.4.0/goes2go/product_table.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)    35108 2023-03-20 15:41:44.000000 goes2go-2023.4.0/goes2go/rgb.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     6593 2022-03-21 20:48:21.000000 goes2go-2023.4.0/goes2go/tools.py
-drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 16:52:01.000000 goes2go-2023.4.0/goes2go.egg-info/
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go.egg-info/PKG-INFO
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      656 2023-04-10 16:52:00.000000 goes2go-2023.4.0/goes2go.egg-info/SOURCES.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go.egg-info/dependency_links.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2021-02-22 16:48:38.000000 goes2go-2023.4.0/goes2go.egg-info/not-zip-safe
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      237 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go.egg-info/requires.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)       14 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go.egg-info/top_level.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      277 2022-10-20 19:33:08.000000 goes2go-2023.4.0/pyproject.toml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      107 2022-10-20 18:27:34.000000 goes2go-2023.4.0/requirements.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1541 2023-04-10 16:52:01.000000 goes2go-2023.4.0/setup.cfg
--rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-10-20 19:32:14.000000 goes2go-2023.4.0/setup.py
-drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 16:52:01.000000 goes2go-2023.4.0/tests/
--rw-r-----   0 blaylock (922916) 0381G056  (8708)        0 2022-10-20 15:16:21.000000 goes2go-2023.4.0/tests/__init__.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      532 2022-11-15 17:49:05.000000 goes2go-2023.4.0/tests/test_GOES.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      302 2022-03-21 20:48:21.000000 goes2go-2023.4.0/tests/test_abi.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     2756 2023-03-20 15:41:44.000000 goes2go-2023.4.0/tests/test_data.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      332 2022-03-21 20:48:21.000000 goes2go-2023.4.0/tests/test_glm.py
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 19:04:41.000000 goes2go-2023.4.1/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-03-07 22:50:31.000000 goes2go-2023.4.1/.gitattributes
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     2027 2023-02-02 16:15:19.000000 goes2go-2023.4.1/.gitignore
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1079 2023-02-02 16:12:51.000000 goes2go-2023.4.1/.readthedocs.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      977 2023-04-10 16:44:33.000000 goes2go-2023.4.1/CITATION.cff
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1076 2022-03-07 22:50:31.000000 goes2go-2023.4.1/LICENSE
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      102 2022-10-20 19:50:16.000000 goes2go-2023.4.1/MANIFEST.in
+-rw-------   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-10 19:04:41.000000 goes2go-2023.4.1/PKG-INFO
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     8722 2023-02-02 16:12:51.000000 goes2go-2023.4.1/README.md
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     2393 2022-11-15 17:49:05.000000 goes2go-2023.4.1/environment-dev.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      747 2022-11-15 17:45:56.000000 goes2go-2023.4.1/environment-test-conda.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1038 2022-10-20 20:22:08.000000 goes2go-2023.4.1/environment-test.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1352 2023-02-02 16:28:56.000000 goes2go-2023.4.1/environment.yml
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 19:04:41.000000 goes2go-2023.4.1/goes2go/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     7797 2022-10-20 15:16:21.000000 goes2go-2023.4.1/goes2go/NEW.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     3105 2023-03-20 15:41:44.000000 goes2go-2023.4.1/goes2go/__init__.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      166 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go/_version.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)    41018 2023-04-10 18:53:52.000000 goes2go-2023.4.1/goes2go/accessors.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)    21281 2023-03-20 15:46:12.000000 goes2go-2023.4.1/goes2go/data.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     6710 2022-05-12 15:43:43.000000 goes2go-2023.4.1/goes2go/product_table.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)    35082 2023-04-10 18:44:07.000000 goes2go-2023.4.1/goes2go/rgb.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     6947 2023-04-10 18:59:52.000000 goes2go-2023.4.1/goes2go/tools.py
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 19:04:41.000000 goes2go-2023.4.1/goes2go.egg-info/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go.egg-info/PKG-INFO
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      656 2023-04-10 19:04:41.000000 goes2go-2023.4.1/goes2go.egg-info/SOURCES.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go.egg-info/dependency_links.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2021-02-22 16:48:38.000000 goes2go-2023.4.1/goes2go.egg-info/not-zip-safe
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      237 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go.egg-info/requires.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)       14 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go.egg-info/top_level.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      277 2022-10-20 19:33:08.000000 goes2go-2023.4.1/pyproject.toml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      107 2022-10-20 18:27:34.000000 goes2go-2023.4.1/requirements.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1541 2023-04-10 19:04:41.000000 goes2go-2023.4.1/setup.cfg
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-10-20 19:32:14.000000 goes2go-2023.4.1/setup.py
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 19:04:41.000000 goes2go-2023.4.1/tests/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)        0 2022-10-20 15:16:21.000000 goes2go-2023.4.1/tests/__init__.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      532 2022-11-15 17:49:05.000000 goes2go-2023.4.1/tests/test_GOES.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      302 2022-03-21 20:48:21.000000 goes2go-2023.4.1/tests/test_abi.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     2756 2023-03-20 15:41:44.000000 goes2go-2023.4.1/tests/test_data.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      332 2022-03-21 20:48:21.000000 goes2go-2023.4.1/tests/test_glm.py
```

### Comparing `goes2go-2023.4.0/.gitignore` & `goes2go-2023.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/.readthedocs.yml` & `goes2go-2023.4.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/CITATION.cff` & `goes2go-2023.4.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/LICENSE` & `goes2go-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/PKG-INFO` & `goes2go-2023.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goes2go
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Retrieve GOES-16/17 data from AWS. Also proves some RGB recipes.
 Home-page: https://github.com/blaylockbk/goes2go
 Author: Brian K. Blaylock
 Author-email: blaylockbk@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/blaylockbk/goes2go
 Project-URL: Documentation, https://goes2go.readthedocs.io/
```

### Comparing `goes2go-2023.4.0/README.md` & `goes2go-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/environment-dev.yml` & `goes2go-2023.4.1/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/environment-test-conda.yml` & `goes2go-2023.4.1/environment-test-conda.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/environment-test.yml` & `goes2go-2023.4.1/environment-test.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/environment.yml` & `goes2go-2023.4.1/environment.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/goes2go/NEW.py` & `goes2go-2023.4.1/goes2go/NEW.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/goes2go/__init__.py` & `goes2go-2023.4.1/goes2go/__init__.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/goes2go/accessors.py` & `goes2go-2023.4.1/goes2go/accessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,14 @@
             # can plot it correctly.
             # TODO: Is there a more "correct" way to handle this?
             sat_height = ds.goes_imager_projection.perspective_point_height
             FOV_degrees = 17.4
             FOV_degrees -= 0.06
             FOV_radius = np.radians(FOV_degrees / 2) * sat_height
             FOV_polygon = Point(0, 0).buffer(FOV_radius, resolution=160)
-            return FOV_polygon
         elif ds.title.startswith("GLM"):
             # Field of view (FOV) of GLM is different than ABI.
             # Do a little offset to better match boundary from
             # Rudlosky et al. 2018
             sat_height = ds.nominal_satellite_height.item() * 1000
             FOV_degrees = 8 * 2
             FOV_degrees += 0.15
@@ -236,15 +235,15 @@
                 [(-cutout_FOV_length, i) for i in side_points]
                 + [(i, cutout_FOV_length) for i in side_points]
                 + [(cutout_FOV_length, i) for i in side_points][::-1]
                 + [(i, -cutout_FOV_length) for i in side_points][::-1]
             )
             cutout = Polygon(cutout_points)
             FOV_polygon = FOV_polygon.intersection(cutout)
-            return FOV_polygon
+        return FOV_polygon
 
     @property
     def domain(self):
         """
         Field of view for the ABI domain (CONUS or MesoScale).
 
         .. image:: /_static/ABI_field-of-view_16dom.png
```

### Comparing `goes2go-2023.4.0/goes2go/data.py` & `goes2go-2023.4.1/goes2go/data.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/goes2go/product_table.txt` & `goes2go-2023.4.1/goes2go/product_table.txt`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/goes2go/rgb.py` & `goes2go-2023.4.1/goes2go/rgb.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 """
 ===========
 RGB Recipes
 ===========
 
 .. image:: /_static/RGB_sample.png
 
-These functions take GOES-East or GOES-West multichannel data on a 
-fixed grid (files named ``ABI-L2-MCMIPC``) and generates a 3D 
+These functions take GOES-East or GOES-West multichannel data on a
+fixed grid (files named ``ABI-L2-MCMIPC``) and generates a 3D
 Red-Green-Blue (RGB) array for various GOES RGB products.
 
 RGB recipes are based on the `GOES Quick Guides
-<http://rammb.cira.colostate.edu/training/visit/quick_guides/>`_ 
+<http://rammb.cira.colostate.edu/training/visit/quick_guides/>`_
 and include the following:
 
     - NaturalColor
     - TrueColor
     - FireTemperature
     - AirMass
     - DayCloudPhase
@@ -32,46 +32,46 @@
     - Dust
     - SulfurDioxide
     - Ash
     - SplitWindowDifference
     - NightFogDifference
     - RocketPlume              ✨New - July 9, 2021
 
-The returned RGB can easily be viewed with ``plt.imshow(RGB)``. 
+The returned RGB can easily be viewed with ``plt.imshow(RGB)``.
 
-For imshow to show an RGB image, the values must range between 0 and 1. 
-Values are normalized between the range specified in the Quick Guides. 
-This normalization is synonymous to `contrast or histogram stretching 
+For imshow to show an RGB image, the values must range between 0 and 1.
+Values are normalized between the range specified in the Quick Guides.
+This normalization is synonymous to `contrast or histogram stretching
 <https://micro.magnet.fsu.edu/primer/java/digitalimaging/processing/histogramstretching/index.html>`_
 (`more info here
 <https://staff.fnwi.uva.nl/r.vandenboomgaard/IPCV20162017/LectureNotes/IP/PointOperators/ImageStretching.html>`_)
 and follows the formula:
 
-    .. code-block:: python 
+    .. code-block:: python
 
         NormalizedValue = (OriginalValue-LowerLimit)/(UpperLimit-LowerLimit)
 
 `Gamma correction <https://en.wikipedia.org/wiki/Gamma_correction>`_
-darkens or lightens an image (`more info 
-<https://www.cambridgeincolour.com/tutorials/gamma-correction.htm>`_) 
+darkens or lightens an image (`more info
+<https://www.cambridgeincolour.com/tutorials/gamma-correction.htm>`_)
 and follows the decoding formula:
 
-    .. code-block:: python 
-        
+    .. code-block:: python
+
         R_corrected = R**(1/gamma)
 
 The input for all these functions are denoted by ``C`` for "channels" which
 represents the GOES ABI multichannel file opened with xarray. For example:
 
-    .. code-block:: python 
-        
+    .. code-block:: python
+
         FILE = 'OR_ABI-L2-MCMIPC-M6_G17_s20192201631196_e20192201633575_c20192201634109.nc'
         C = xarray.open_dataset(FILE)
 
-All RGB products are demonstarted in the `make_RGB_Demo 
+All RGB products are demonstarted in the `make_RGB_Demo
 <https://github.com/blaylockbk/goes2go/tree/master/notebooks>`_ notebook.
 
 Note: I don't have a `GeoColor <https://journals.ametsoc.org/view/journals/atot/37/3/JTECH-D-19-0134.1.xml>`_
 RGB, because it is much more involved than simply stacking RGB channels. If anyone does do
 something similar to a GeoColor image, let me know!
 
 ABI Band Reference
@@ -160,15 +160,15 @@
 
     """
     # Assemble a new xarray.Dataset for the RGB data
     ds = xr.Dataset({description.replace(" ", ""): (["y", "x", "rgb"], RGB)})
     ds.attrs["description"] = description
 
     # Convert x, y points to latitude/longitude
-    _, crs = field_of_view(G)
+    _, _, crs = field_of_view(G)
     sat_h = G.goes_imager_projection.perspective_point_height
     x2 = G.x * sat_h
     y2 = G.y * sat_h
     ds.coords["x2"] = x2
     ds.coords["y2"] = y2
 
     ds["x2"].attrs["long_name"] = "x sweep in crs units (m); x * sat_height"
```

### Comparing `goes2go-2023.4.0/goes2go/tools.py` & `goes2go-2023.4.1/goes2go/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,49 +16,59 @@
     import metpy  # Need accessors to get projection info.
 except:
     # Not sure why sphinx can't import metpy??
     warnings.warn("Metpy not imported.")
 from shapely.geometry import Point, Polygon
 
 
+# TODO: Remove this someday
 def field_of_view(G, resolution=60, reduce_abi_fov=0.06):
     """
     Create a field-of-view polygon for the GOES data.
 
     Based on information from the `GOES-R Series Data Book
     <https://www.goes-r.gov/downloads/resources/documents/GOES-RSeriesDataBook.pdf>`_.
 
     GLM lense field of view is 16 degree, or +/- 8 degrees (see page 225)
     ABI full-disk field of view if 17.4 degrees (see page 48)
 
     To plot the field of view on the cartopy axes, do the following:
 
     .. code:: python
 
-        FOV, geo = field_of_view(G)
-        ax = plt.subplot(projection=geo)
-        ax.add_geometries([FOV], crs=geo)
+        pFOV_inst, pFOV_dom, crs = field_of_view(G)
+        ax = plt.subplot(projection=crs)
+        ax.add_geometries([FOV], crs=crs)
 
     Parameters
     ----------
     G : xarray.Dataset
         The GOES NetCDF file opened with xarray. A file is required
         because we get info from the file to define the projection.
     resolution : int
         Resolution of polygon shapes
     reduce_abi_fov : float or int
         Since the globe isn't a perfect ellipse, reduce the field of
         view just slightly to get all the points to be on the projection
         plane. If this number is less than the default, the polygon
         will not be calculated correctly because edge points will lie
         off the projection globe.
+
+    Returns
+    -------
+    pFOV_inst is a polygon of the instrument field of view.
+    pFOV_dom is a polygon of the domain field of view
+    crs is the cartopy coordinate reference system for the instrument
     """
     warnings.warn(
-        "DEPRECIATION. Use the FOV accessor instead `G.FOV.full_disk` or `G.FOV.domain`"
-    )
+            "Use the FOV accessor instead `G.FOV.full_disk` or `G.FOV.domain`",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
     if G.title.startswith("ABI"):
         globe_kwargs = dict(
             semimajor_axis=G.goes_imager_projection.semi_major_axis,
             semiminor_axis=G.goes_imager_projection.semi_minor_axis,
             inverse_flattening=G.goes_imager_projection.inverse_flattening,
         )
         sat_height = G.goes_imager_projection.perspective_point_height
@@ -93,15 +103,15 @@
 
     # Create polygon of the field of view. This polygon is in
     # the geostationary crs projection units, and is in meters.
     # The central point is at 0,0 (not the nadir position), because
     # we are working in the geostationary projection coordinates
     # and the center point is 0,0 meters.
     FOV_radius = np.radians(FOV / 2) * sat_height
-    FOV_poly = Point(0, 0).buffer(FOV_radius, resolution=resolution)
+    pFOV_inst = Point(0, 0).buffer(FOV_radius, resolution=resolution)
 
     ## GLM is a bit funny. I haven't found this in the documentation
     ## anywhere, yet, but the GLM field-of-view is not exactly
     ## the full circle, there is a square area cut out of it.
     ## The square FOV is ~ 15 degrees
     if G.title.startswith("GLM"):
         FOV_square = 15 / 2
@@ -123,30 +133,30 @@
         side4x, side4y = (
             np.linspace(FOV_radius, -FOV_radius, resolution),
             np.ones(resolution) * -FOV_radius,
         )
         x = np.hstack([side1x, side2x, side3x, side4x])
         y = np.hstack([side1y, side2y, side3y, side4y])
         square_FOV = Polygon(zip(x, y))
-        FOV_poly = FOV_poly.intersection(square_FOV)
-
-        return FOV_poly, crs
+        pFOV_inst = pFOV_inst.intersection(square_FOV)
+        pFOV_dom = None # there is no "domain" for the GLM instrument
 
     if G.title.startswith("ABI"):
-        # We have the global field of view
+        # We have the global field of view,
         # now we need the domain field of view
         dom_border = np.array(
             [(i, G.y.data[0]) for i in G.x.data]
             + [(G.x.data[-1], i) for i in G.y.data]
             + [(i, G.y.data[-1]) for i in G.x.data[::-1]]
             + [(G.x.data[0], i) for i in G.y.data[::-1]]
         )
-        FOV_dom = Polygon(dom_border * sat_height)
-        FOV_dom = FOV_dom.intersection(FOV_poly)
-        return FOV_poly, FOV_dom, crs
+        pFOV_dom = Polygon(dom_border * sat_height)
+        pFOV_dom = pFOV_dom.intersection(pFOV_inst)
+
+    return pFOV_inst, pFOV_dom, crs
 
 
 def abi_crs(G, reference_variable="CMI_C01"):
     """
     Get coordinate reference system for the Advanced Baseline Imager (ABI).
 
     Parameters
```

### Comparing `goes2go-2023.4.0/goes2go.egg-info/PKG-INFO` & `goes2go-2023.4.1/goes2go.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goes2go
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Retrieve GOES-16/17 data from AWS. Also proves some RGB recipes.
 Home-page: https://github.com/blaylockbk/goes2go
 Author: Brian K. Blaylock
 Author-email: blaylockbk@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/blaylockbk/goes2go
 Project-URL: Documentation, https://goes2go.readthedocs.io/
```

### Comparing `goes2go-2023.4.0/goes2go.egg-info/SOURCES.txt` & `goes2go-2023.4.1/goes2go.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/setup.cfg` & `goes2go-2023.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/tests/test_GOES.py` & `goes2go-2023.4.1/tests/test_GOES.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.0/tests/test_data.py` & `goes2go-2023.4.1/tests/test_data.py`

 * *Files identical despite different names*

