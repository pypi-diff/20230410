# Comparing `tmp/Piff-1.3.2.tar.gz` & `tmp/Piff-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Piff-1.3.2.tar", last modified: Fri Mar 10 18:20:16 2023, max compression
+gzip compressed data, was "Piff-1.3.3.tar", last modified: Mon Apr 10 19:21:25 2023, max compression
```

## Comparing `Piff-1.3.2.tar` & `Piff-1.3.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:20:16.108908 Piff-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-10 18:18:31.000000 Piff-1.3.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-10 18:18:31.000000 Piff-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-10 18:18:31.000000 Piff-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-03-10 18:20:16.108908 Piff-1.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:20:16.100908 Piff-1.3.2/Piff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-03-10 18:20:16.000000 Piff-1.3.2/Piff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-10 18:20:16.000000 Piff-1.3.2/Piff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 18:20:16.000000 Piff-1.3.2/Piff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-10 18:20:16.000000 Piff-1.3.2/Piff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-10 18:20:16.000000 Piff-1.3.2/Piff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-03-10 18:18:31.000000 Piff-1.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:20:16.104908 Piff-1.3.2/piff/
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20477 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/basis_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:20:16.104908 Piff-1.3.2/piff/des/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/des/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/des/decam_wavefront.py
--rw-r--r--   0 runner    (1001) docker     (123)    16351 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/des/decaminfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/gp_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/gsobject_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    51519 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/knn_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/mean_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/optical_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/pixelgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17535 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/polynomial_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27602 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/psf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23087 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/simplepsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/singlechip.py
--rw-r--r--   0 runner    (1001) docker     (123)    27214 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/size_mag.py
--rw-r--r--   0 runner    (1001) docker     (123)    40492 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/star.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/star_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    41594 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    24700 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/twod_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    33902 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-03-10 18:18:31.000000 Piff-1.3.2/piff/wavefront.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:20:16.104908 Piff-1.3.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-03-10 18:18:31.000000 Piff-1.3.2/scripts/meanify
--rwxr-xr-x   0 runner    (1001) docker     (123)     3174 2023-03-10 18:18:31.000000 Piff-1.3.2/scripts/piffify
--rwxr-xr-x   0 runner    (1001) docker     (123)     3109 2023-03-10 18:18:31.000000 Piff-1.3.2/scripts/plotify
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 18:20:16.108908 Piff-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-03-10 18:18:31.000000 Piff-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:20:16.108908 Piff-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/custom_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/piff_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_gp_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_gsobject_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    65796 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_knn_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_meanify.py
--rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_optics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    64329 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_poly.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_sizemag.py
--rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_star.py
--rw-r--r--   0 runner    (1001) docker     (123)    49289 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_wavefront.py
--rw-r--r--   0 runner    (1001) docker     (123)    32217 2023-03-10 18:18:31.000000 Piff-1.3.2/tests/test_wcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:21:25.466745 Piff-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-10 19:19:19.000000 Piff-1.3.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-10 19:19:19.000000 Piff-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 19:19:19.000000 Piff-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-10 19:21:25.466745 Piff-1.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:21:25.454745 Piff-1.3.3/Piff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-10 19:21:25.000000 Piff-1.3.3/Piff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-10 19:21:25.000000 Piff-1.3.3/Piff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:21:25.000000 Piff-1.3.3/Piff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-10 19:21:25.000000 Piff-1.3.3/Piff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 19:21:25.000000 Piff-1.3.3/Piff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-10 19:19:19.000000 Piff-1.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:21:25.458745 Piff-1.3.3/piff/
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20477 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/basis_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:21:25.462745 Piff-1.3.3/piff/des/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/des/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/des/decam_wavefront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16351 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/des/decaminfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/gp_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/gsobject_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51519 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/knn_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/mean_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/optical_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/pixelgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17535 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/polynomial_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27602 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/psf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23087 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/simplepsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/singlechip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27214 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/size_mag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40492 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/star_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42511 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24700 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/twod_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33902 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-10 19:19:19.000000 Piff-1.3.3/piff/wavefront.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:21:25.462745 Piff-1.3.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-04-10 19:19:19.000000 Piff-1.3.3/scripts/meanify
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3174 2023-04-10 19:19:19.000000 Piff-1.3.3/scripts/piffify
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3109 2023-04-10 19:19:19.000000 Piff-1.3.3/scripts/plotify
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:21:25.466745 Piff-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-04-10 19:19:19.000000 Piff-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:21:25.466745 Piff-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-10 19:19:19.000000 Piff-1.3.3/tests/custom_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/piff_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_gp_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_gsobject_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65796 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_knn_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_meanify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_optics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64329 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_sizemag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49519 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_wavefront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32217 2023-04-10 19:19:20.000000 Piff-1.3.3/tests/test_wcs.py
```

### Comparing `Piff-1.3.2/CHANGELOG.rst` & `Piff-1.3.3/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -58,7 +58,12 @@
 - Removed is_reserve column from the HSM output file, which was accidentally added, and is
   equivalent to the existing reserve column.
 
 Changes from version 1.3.1 to 1.3.2
 ===================================
 
 - Added piff_version to the FITS header in the HSM output file. (#148)
+
+Changes from version 1.3.2 to 1.3.3
+===================================
+
+- Added guards against HSM failures when doing fourth_order/raw_moments in HSM output file. (#149)
```

### Comparing `Piff-1.3.2/LICENSE` & `Piff-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/PKG-INFO` & `Piff-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Piff
-Version: 1.3.2
+Version: 1.3.3
 Summary: PSFs in the Full FOV
 Home-page: https://github.com/rmjarvis/Piff
-Download-URL: https://github.com/rmjarvis/Piff/releases/tag/v1.3.2.zip
+Download-URL: https://github.com/rmjarvis/Piff/releases/tag/v1.3.3.zip
 Author: Mike Jarvis
 Author-email: michael@jarvis.net
 License: BSD License
 License-File: LICENSE
 
 PIFF: PSFs In the Full FOV
 ==========================
```

### Comparing `Piff-1.3.2/Piff.egg-info/PKG-INFO` & `Piff-1.3.3/Piff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Piff
-Version: 1.3.2
+Version: 1.3.3
 Summary: PSFs in the Full FOV
 Home-page: https://github.com/rmjarvis/Piff
-Download-URL: https://github.com/rmjarvis/Piff/releases/tag/v1.3.2.zip
+Download-URL: https://github.com/rmjarvis/Piff/releases/tag/v1.3.3.zip
 Author: Mike Jarvis
 Author-email: michael@jarvis.net
 License: BSD License
 License-File: LICENSE
 
 PIFF: PSFs In the Full FOV
 ==========================
```

### Comparing `Piff-1.3.2/Piff.egg-info/SOURCES.txt` & `Piff-1.3.3/Piff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/README.rst` & `Piff-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/__init__.py` & `Piff-1.3.3/piff/__init__.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/_version.py` & `Piff-1.3.3/piff/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the disclaimer given in the accompanying LICENSE
 #    file.
 # 2. Redistributions in binary form must reproduce the above copyright notice,
 #    this list of conditions and the disclaimer given in the documentation
 #    and/or other materials provided with the distribution.
 
-__version__ = '1.3.2'
+__version__ = '1.3.3'
 __version_info__ = tuple(map(int, __version__.split('.')))
```

### Comparing `Piff-1.3.2/piff/basis_interp.py` & `Piff-1.3.3/piff/basis_interp.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/config.py` & `Piff-1.3.3/piff/config.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/des/__init__.py` & `Piff-1.3.3/piff/des/__init__.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/des/decam_wavefront.py` & `Piff-1.3.3/piff/des/decam_wavefront.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/des/decaminfo.py` & `Piff-1.3.3/piff/des/decaminfo.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/gp_interp.py` & `Piff-1.3.3/piff/gp_interp.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/gsobject_model.py` & `Piff-1.3.3/piff/gsobject_model.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/input.py` & `Piff-1.3.3/piff/input.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/interp.py` & `Piff-1.3.3/piff/interp.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/knn_interp.py` & `Piff-1.3.3/piff/knn_interp.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/mean_interp.py` & `Piff-1.3.3/piff/mean_interp.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/model.py` & `Piff-1.3.3/piff/model.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/optical_model.py` & `Piff-1.3.3/piff/optical_model.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/outliers.py` & `Piff-1.3.3/piff/outliers.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/output.py` & `Piff-1.3.3/piff/output.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/pixelgrid.py` & `Piff-1.3.3/piff/pixelgrid.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/polynomial_interp.py` & `Piff-1.3.3/piff/polynomial_interp.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/psf.py` & `Piff-1.3.3/piff/psf.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/select.py` & `Piff-1.3.3/piff/select.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/simplepsf.py` & `Piff-1.3.3/piff/simplepsf.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/singlechip.py` & `Piff-1.3.3/piff/singlechip.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/size_mag.py` & `Piff-1.3.3/piff/size_mag.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/star.py` & `Piff-1.3.3/piff/star.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/star_stats.py` & `Piff-1.3.3/piff/star_stats.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/stats.py` & `Piff-1.3.3/piff/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,32 +178,42 @@
                 kwargs = dict(fourth_order=True)
                 nshapes += 5
             if raw_moments:
                 nshapes += 18
                 kwargs = dict(third_order=True, fourth_order=True, radial=True)
             for i, star in enumerate(stars):
                 d = shapes_data[i]
-                m = calculate_moments(star, **kwargs)
 
-                if fourth_order:
-                    d.extend([m['M22']/m['M11'],
-                            m['M31']/m['M11']**2, m['M13']/m['M11']**2,
-                            m['M40']/m['M11']**2, m['M04']/m['M11']**2])
-
-                    # Subtract off 3e from the 4th order shapes to remove the leading order
-                    # term from the overall ellipticity, which is already captured in the
-                    # second order shape.  (For a Gaussian, this makes g4 very close to 0.)
-                    shape = galsim.Shear(g1=star.hsm[4], g2=star.hsm[5])
-                    d[8] -= 3*shape.e1
-                    d[9] -= 3*shape.e2
-                if raw_moments:
-                    d.extend([m['M00'], m['M10'], m['M01'], m['M11'], m['M20'], m['M02'],
-                              m['M21'], m['M12'], m['M30'], m['M03'],
-                              m['M22'], m['M31'], m['M13'], m['M40'], m['M04'],
-                              m['M22n'], m['M33n'], m['M44n']])
+                try:
+                    m = calculate_moments(star, **kwargs)
+                except RuntimeError as e:
+                    # Make sure the flag is set.
+                    if 'HSM failed' in e.args[0]:
+                        d[6] = int(e.args[0].split()[-1])
+                    else: # pragma: no cover
+                        # The HSM failed error is the only one we expect, but just in case...
+                        d[6] = 1
+                    d.extend([0] * (nshapes - 7))
+                else:
+                    if fourth_order:
+                        d.extend([m['M22']/m['M11'],
+                                m['M31']/m['M11']**2, m['M13']/m['M11']**2,
+                                m['M40']/m['M11']**2, m['M04']/m['M11']**2])
+
+                        # Subtract off 3e from the 4th order shapes to remove the leading order
+                        # term from the overall ellipticity, which is already captured in the
+                        # second order shape.  (For a Gaussian, this makes g4 very close to 0.)
+                        shape = galsim.Shear(g1=star.hsm[4], g2=star.hsm[5])
+                        d[8] -= 3*shape.e1
+                        d[9] -= 3*shape.e2
+                    if raw_moments:
+                        d.extend([m['M00'], m['M10'], m['M01'], m['M11'], m['M20'], m['M02'],
+                                m['M21'], m['M12'], m['M30'], m['M03'],
+                                m['M22'], m['M31'], m['M13'], m['M40'], m['M04'],
+                                m['M22n'], m['M33n'], m['M44n']])
 
         # Turn it into a proper numpy array.
         shapes_data = np.array(shapes_data)
         # If no stars, then shapes_data is the wrong shape.  This line is normally a no op
         # but makes things work right if len(stars)=0.
         shapes_data = shapes_data.reshape((len(stars),nshapes))
         for star, shape in zip(stars, shapes_data):
@@ -238,27 +248,35 @@
                 stars = psf.interpolateStarList(stars)
             model_stars = psf.drawStarList(stars)
             shapes_model = [list(star.hsm) for star in model_stars]
 
             if fourth_order or raw_moments:
                 for i, star in enumerate(model_stars):
                     d = shapes_model[i]
-                    m = calculate_moments(star, **kwargs)
-                    if fourth_order:
-                        d.extend([m['M22']/m['M11'],
-                                  m['M31']/m['M11']**2, m['M13']/m['M11']**2,
-                                  m['M40']/m['M11']**2, m['M04']/m['M11']**2])
-                        shape = galsim.Shear(g1=star.hsm[4], g2=star.hsm[5])
-                        d[8] -= 3*shape.e1
-                        d[9] -= 3*shape.e2
-                    if raw_moments:
-                        d.extend([m['M00'], m['M10'], m['M01'], m['M11'], m['M20'], m['M02'],
-                                  m['M21'], m['M12'], m['M30'], m['M03'],
-                                  m['M22'], m['M31'], m['M13'], m['M40'], m['M04'],
-                                  m['M22n'], m['M33n'], m['M44n']])
+                    try:
+                        m = calculate_moments(star, **kwargs)
+                    except RuntimeError as e:
+                        if 'HSM failed' in e.args[0]:
+                            d[6] = int(e.args[0].split()[-1])
+                        else: # pragma: no cover
+                            d[6] = 1
+                        d.extend([0] * (nshapes - 7))
+                    else:
+                        if fourth_order:
+                            d.extend([m['M22']/m['M11'],
+                                    m['M31']/m['M11']**2, m['M13']/m['M11']**2,
+                                    m['M40']/m['M11']**2, m['M04']/m['M11']**2])
+                            shape = galsim.Shear(g1=star.hsm[4], g2=star.hsm[5])
+                            d[8] -= 3*shape.e1
+                            d[9] -= 3*shape.e2
+                        if raw_moments:
+                            d.extend([m['M00'], m['M10'], m['M01'], m['M11'], m['M20'], m['M02'],
+                                    m['M21'], m['M12'], m['M30'], m['M03'],
+                                    m['M22'], m['M31'], m['M13'], m['M40'], m['M04'],
+                                    m['M22n'], m['M33n'], m['M44n']])
 
             shapes_model = np.array(shapes_model)
             shapes_model = shapes_model.reshape((len(model_stars),nshapes))
 
             gsq = shapes_model[:,4]**2 + shapes_model[:,5]**2
             shapes_model[:,3] = 2*shapes_model[:,3]**2 * (1+gsq)/(1-gsq)
             for star, shape in zip(model_stars, shapes_model):
```

### Comparing `Piff-1.3.2/piff/twod_stats.py` & `Piff-1.3.3/piff/twod_stats.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/util.py` & `Piff-1.3.3/piff/util.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/piff/wavefront.py` & `Piff-1.3.3/piff/wavefront.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/scripts/meanify` & `Piff-1.3.3/scripts/meanify`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/scripts/piffify` & `Piff-1.3.3/scripts/piffify`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/scripts/plotify` & `Piff-1.3.3/scripts/plotify`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/setup.py` & `Piff-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/custom_wcs.py` & `Piff-1.3.3/tests/custom_wcs.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/piff_test_helper.py` & `Piff-1.3.3/tests/piff_test_helper.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_gp_interp.py` & `Piff-1.3.3/tests/test_gp_interp.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_gsobject_model.py` & `Piff-1.3.3/tests/test_gsobject_model.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_input.py` & `Piff-1.3.3/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_knn_interp.py` & `Piff-1.3.3/tests/test_knn_interp.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_meanify.py` & `Piff-1.3.3/tests/test_meanify.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_moments.py` & `Piff-1.3.3/tests/test_moments.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_optics.py` & `Piff-1.3.3/tests/test_optics.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_outliers.py` & `Piff-1.3.3/tests/test_outliers.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_output.py` & `Piff-1.3.3/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_pixel.py` & `Piff-1.3.3/tests/test_pixel.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_poly.py` & `Piff-1.3.3/tests/test_poly.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_simple.py` & `Piff-1.3.3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_sizemag.py` & `Piff-1.3.3/tests/test_sizemag.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_star.py` & `Piff-1.3.3/tests/test_star.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_stats.py` & `Piff-1.3.3/tests/test_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,14 +712,15 @@
 
     twodhist_file = os.path.join('output','bad_hsm_twod.pdf')
     whisker_file = os.path.join('output','bad_hsm_whisk.pdf')
     rho_file = os.path.join('output','bad_hsm_rho.pdf')
     shape_file = os.path.join('output','bad_hsm_shape.pdf')
     star_file = os.path.join('output','bad_hsm_star.pdf')
     hsm_file = os.path.join('output','bad_hsm_hsm.fits')
+    hsm4_file = os.path.join('output','bad_hsm_hsm_fourth.fits')
     sizemag_file = os.path.join('output','bad_hsm_sizemag.png')
 
     stamp_size = 25
 
     # The configuration dict with the right input fields for the file we're using.
     config = {
         'input' : {
@@ -767,14 +768,19 @@
                     'type': 'SizeMag',
                     'file_name': sizemag_file,
                 },
                 {
                     'type': 'HSMCatalog',
                     'file_name': hsm_file,
                 },
+                {
+                    'type': 'HSMCatalog',
+                    'file_name': hsm4_file,
+                    'fourth_order': True,
+                },
             ],
         },
         'psf' : {
             'model' : {
                 'type' : 'PixelGrid',
                 'scale' : 0.3,
                 'size' : 10,
```

### Comparing `Piff-1.3.2/tests/test_wavefront.py` & `Piff-1.3.3/tests/test_wavefront.py`

 * *Files identical despite different names*

### Comparing `Piff-1.3.2/tests/test_wcs.py` & `Piff-1.3.3/tests/test_wcs.py`

 * *Files identical despite different names*

