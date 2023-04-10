# Comparing `tmp/NICpolpy-0.1.4.tar.gz` & `tmp/NICpolpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NICpolpy-0.1.4.tar", last modified: Fri Apr  7 10:19:56 2023, max compression
+gzip compressed data, was "NICpolpy-0.1.5.tar", last modified: Mon Apr 10 07:35:31 2023, max compression
```

## Comparing `NICpolpy-0.1.4.tar` & `NICpolpy-0.1.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-07 10:19:56.932954 NICpolpy-0.1.4/
--rw-r--r--   0 ysbach     (501) staff       (20)     1238 2022-07-25 04:56:05.000000 NICpolpy-0.1.4/.gitignore
--rw-r--r--   0 ysbach     (501) staff       (20)     1464 2022-10-13 08:50:15.000000 NICpolpy-0.1.4/LICENSE
--rw-r--r--   0 ysbach     (501) staff       (20)      158 2022-10-14 06:39:22.000000 NICpolpy-0.1.4/MANIFEST.in
-drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-07 10:19:56.913369 NICpolpy-0.1.4/NICpolpy.egg-info/
--rw-r--r--   0 ysbach     (501) staff       (20)    11164 2023-04-07 10:19:56.000000 NICpolpy-0.1.4/NICpolpy.egg-info/PKG-INFO
--rw-r--r--   0 ysbach     (501) staff       (20)     2017 2023-04-07 10:19:56.000000 NICpolpy-0.1.4/NICpolpy.egg-info/SOURCES.txt
--rw-r--r--   0 ysbach     (501) staff       (20)        1 2023-04-07 10:19:56.000000 NICpolpy-0.1.4/NICpolpy.egg-info/dependency_links.txt
--rw-r--r--   0 ysbach     (501) staff       (20)        1 2023-04-07 10:19:56.000000 NICpolpy-0.1.4/NICpolpy.egg-info/not-zip-safe
--rw-r--r--   0 ysbach     (501) staff       (20)      122 2023-04-07 10:19:56.000000 NICpolpy-0.1.4/NICpolpy.egg-info/requires.txt
--rw-r--r--   0 ysbach     (501) staff       (20)        9 2023-04-07 10:19:56.000000 NICpolpy-0.1.4/NICpolpy.egg-info/top_level.txt
--rw-r--r--   0 ysbach     (501) staff       (20)    11164 2023-04-07 10:19:56.933079 NICpolpy-0.1.4/PKG-INFO
--rw-r--r--   0 ysbach     (501) staff       (20)     8372 2023-03-31 10:33:12.000000 NICpolpy-0.1.4/README.md
-drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-07 10:19:56.915877 NICpolpy-0.1.4/nicpolpy/
--rw-r--r--   0 ysbach     (501) staff       (20)    41451 2022-10-13 05:45:35.000000 NICpolpy-0.1.4/nicpolpy/NICPolReduc.py
--rw-r--r--   0 ysbach     (501) staff       (20)      244 2022-02-10 17:30:23.000000 NICpolpy-0.1.4/nicpolpy/__init__.py
--rw-r--r--   0 ysbach     (501) staff       (20)     4106 2022-10-13 06:29:07.000000 NICpolpy-0.1.4/nicpolpy/phot.py
--rw-r--r--   0 ysbach     (501) staff       (20)    42797 2022-10-13 05:46:57.000000 NICpolpy-0.1.4/nicpolpy/prepare.py
--rw-r--r--   0 ysbach     (501) staff       (20)    16617 2022-10-13 06:28:49.000000 NICpolpy-0.1.4/nicpolpy/preproc.py
--rw-r--r--   0 ysbach     (501) staff       (20)    46490 2022-10-13 05:46:12.000000 NICpolpy-0.1.4/nicpolpy/util.py
-drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-07 10:19:56.921555 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/
--rw-r--r--   0 ysbach     (501) staff       (20)      671 2022-01-12 04:41:50.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/__init__.py
--rw-r--r--   0 ysbach     (501) staff       (20)    10718 2021-11-08 08:12:28.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/airmass.py
--rw-r--r--   0 ysbach     (501) staff       (20)     2178 2022-03-20 08:34:23.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/astroim.py
--rw-r--r--   0 ysbach     (501) staff       (20)    22496 2020-11-06 05:49:48.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/astrometry.py
--rw-r--r--   0 ysbach     (501) staff       (20)    40193 2022-03-20 08:55:54.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/combutil.py
--rw-r--r--   0 ysbach     (501) staff       (20)    34775 2022-03-20 08:23:59.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/filemgmt.py
--rw-r--r--   0 ysbach     (501) staff       (20)    10102 2022-06-12 07:51:40.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/fitting.py
--rw-r--r--   0 ysbach     (501) staff       (20)   117008 2022-07-15 13:58:09.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/hduutil.py
-drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-07 10:19:56.925399 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/
--rw-r--r--   0 ysbach     (501) staff       (20)      347 2022-03-20 08:55:33.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/__init__.py
--rw-r--r--   0 ysbach     (501) staff       (20)    16404 2022-01-25 07:31:36.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/docstrings.py
--rw-r--r--   0 ysbach     (501) staff       (20)    12943 2022-02-27 14:29:44.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imarith.py
--rw-r--r--   0 ysbach     (501) staff       (20)    40787 2022-05-11 12:04:38.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imcombine.py
--rw-r--r--   0 ysbach     (501) staff       (20)     5638 2022-02-27 14:31:47.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imcopy.py
--rw-r--r--   0 ysbach     (501) staff       (20)      865 2022-02-27 14:54:23.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imsmooth.py
--rw-r--r--   0 ysbach     (501) staff       (20)    16154 2022-01-05 06:16:21.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_comb.py
--rw-r--r--   0 ysbach     (501) staff       (20)     9950 2020-11-13 02:08:13.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_lmedian.py
--rw-r--r--   0 ysbach     (501) staff       (20)    15064 2022-01-05 06:16:19.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_reject.py
--rw-r--r--   0 ysbach     (501) staff       (20)    48138 2022-05-18 13:43:21.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/misc.py
--rw-r--r--   0 ysbach     (501) staff       (20)    71737 2022-09-25 09:26:09.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/preproc.py
-drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-07 10:19:56.925884 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/tests/
--rw-r--r--   0 ysbach     (501) staff       (20)        0 2021-05-21 01:18:27.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/tests/__init__.py
--rw-r--r--   0 ysbach     (501) staff       (20)      663 2021-05-21 07:58:54.000000 NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/tests/test_misc.py
-drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-07 10:19:56.930721 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/
--rw-r--r--   0 ysbach     (501) staff       (20)      211 2022-10-14 06:26:37.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/__init__.py
--rw-r--r--   0 ysbach     (501) staff       (20)    11282 2023-03-12 14:35:47.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/aperture.py
--rw-r--r--   0 ysbach     (501) staff       (20)    13683 2022-07-07 04:43:13.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/apphot.py
--rw-r--r--   0 ysbach     (501) staff       (20)     5900 2022-06-09 12:31:35.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/background.py
--rw-r--r--   0 ysbach     (501) staff       (20)    34050 2022-07-15 05:38:34.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/center.py
--rw-r--r--   0 ysbach     (501) staff       (20)     3710 2022-07-07 04:43:11.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/daopsf.py
--rw-r--r--   0 ysbach     (501) staff       (20)     3147 2020-01-23 08:48:25.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/growth.py
--rw-r--r--   0 ysbach     (501) staff       (20)    31643 2022-07-18 05:29:40.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/polarimetry.py
--rw-r--r--   0 ysbach     (501) staff       (20)    48206 2022-10-14 07:48:11.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/queryutil.py
--rw-r--r--   0 ysbach     (501) staff       (20)    22802 2022-06-11 09:21:12.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/seputil.py
-drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-07 10:19:56.931425 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/tests/
--rw-r--r--   0 ysbach     (501) staff       (20)      335 2022-06-09 11:56:23.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/tests/__init__.py
--rw-r--r--   0 ysbach     (501) staff       (20)        0 2022-06-09 12:10:21.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/tests/test_apphot.py
--rw-r--r--   0 ysbach     (501) staff       (20)      796 2022-06-09 12:31:38.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/tests/test_background.py
--rw-r--r--   0 ysbach     (501) staff       (20)    15703 2022-07-07 04:43:08.000000 NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/util.py
--rw-r--r--   0 ysbach     (501) staff       (20)       86 2022-10-14 06:37:14.000000 NICpolpy-0.1.4/pyproject.toml
-drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-07 10:19:56.931800 NICpolpy-0.1.4/readme_images/
--rw-r--r--   0 ysbach     (501) staff       (20)   985898 2020-01-09 09:23:17.000000 NICpolpy-0.1.4/readme_images/ap_selection.png
--rw-r--r--   0 ysbach     (501) staff       (20)     1580 2023-04-07 10:19:56.933757 NICpolpy-0.1.4/setup.cfg
--rw-r--r--   0 ysbach     (501) staff       (20)       69 2022-10-14 06:36:27.000000 NICpolpy-0.1.4/setup.py
+drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-10 07:35:31.296766 NICpolpy-0.1.5/
+-rw-r--r--   0 ysbach     (501) staff       (20)     1238 2022-07-25 04:56:05.000000 NICpolpy-0.1.5/.gitignore
+-rw-r--r--   0 ysbach     (501) staff       (20)     1464 2022-10-13 08:50:15.000000 NICpolpy-0.1.5/LICENSE
+-rw-r--r--   0 ysbach     (501) staff       (20)      158 2022-10-14 06:39:22.000000 NICpolpy-0.1.5/MANIFEST.in
+drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-10 07:35:31.275212 NICpolpy-0.1.5/NICpolpy.egg-info/
+-rw-r--r--   0 ysbach     (501) staff       (20)    11164 2023-04-10 07:35:31.000000 NICpolpy-0.1.5/NICpolpy.egg-info/PKG-INFO
+-rw-r--r--   0 ysbach     (501) staff       (20)     2017 2023-04-10 07:35:31.000000 NICpolpy-0.1.5/NICpolpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ysbach     (501) staff       (20)        1 2023-04-10 07:35:31.000000 NICpolpy-0.1.5/NICpolpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ysbach     (501) staff       (20)        1 2023-04-07 10:19:56.000000 NICpolpy-0.1.5/NICpolpy.egg-info/not-zip-safe
+-rw-r--r--   0 ysbach     (501) staff       (20)      122 2023-04-10 07:35:31.000000 NICpolpy-0.1.5/NICpolpy.egg-info/requires.txt
+-rw-r--r--   0 ysbach     (501) staff       (20)        9 2023-04-10 07:35:31.000000 NICpolpy-0.1.5/NICpolpy.egg-info/top_level.txt
+-rw-r--r--   0 ysbach     (501) staff       (20)    11164 2023-04-10 07:35:31.296879 NICpolpy-0.1.5/PKG-INFO
+-rw-r--r--   0 ysbach     (501) staff       (20)     8372 2023-03-31 10:33:12.000000 NICpolpy-0.1.5/README.md
+drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-10 07:35:31.277192 NICpolpy-0.1.5/nicpolpy/
+-rw-r--r--   0 ysbach     (501) staff       (20)    41451 2022-10-13 05:45:35.000000 NICpolpy-0.1.5/nicpolpy/NICPolReduc.py
+-rw-r--r--   0 ysbach     (501) staff       (20)      244 2022-02-10 17:30:23.000000 NICpolpy-0.1.5/nicpolpy/__init__.py
+-rw-r--r--   0 ysbach     (501) staff       (20)     4106 2022-10-13 06:29:07.000000 NICpolpy-0.1.5/nicpolpy/phot.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    42797 2022-10-13 05:46:57.000000 NICpolpy-0.1.5/nicpolpy/prepare.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    16617 2022-10-13 06:28:49.000000 NICpolpy-0.1.5/nicpolpy/preproc.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    52258 2023-04-07 17:35:45.000000 NICpolpy-0.1.5/nicpolpy/util.py
+drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-10 07:35:31.283211 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/
+-rw-r--r--   0 ysbach     (501) staff       (20)      671 2022-01-12 04:41:50.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/__init__.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    10718 2021-11-08 08:12:28.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/airmass.py
+-rw-r--r--   0 ysbach     (501) staff       (20)     2178 2022-03-20 08:34:23.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/astroim.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    22496 2020-11-06 05:49:48.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/astrometry.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    40193 2022-03-20 08:55:54.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/combutil.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    34775 2022-03-20 08:23:59.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/filemgmt.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    10102 2022-06-12 07:51:40.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/fitting.py
+-rw-r--r--   0 ysbach     (501) staff       (20)   117008 2022-07-15 13:58:09.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/hduutil.py
+drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-10 07:35:31.287881 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/
+-rw-r--r--   0 ysbach     (501) staff       (20)      347 2022-03-20 08:55:33.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/__init__.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    16404 2022-01-25 07:31:36.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/docstrings.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    12943 2022-02-27 14:29:44.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imarith.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    40787 2022-05-11 12:04:38.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imcombine.py
+-rw-r--r--   0 ysbach     (501) staff       (20)     5638 2022-02-27 14:31:47.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imcopy.py
+-rw-r--r--   0 ysbach     (501) staff       (20)      865 2022-02-27 14:54:23.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imsmooth.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    16154 2022-01-05 06:16:21.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_comb.py
+-rw-r--r--   0 ysbach     (501) staff       (20)     9950 2020-11-13 02:08:13.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_lmedian.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    15064 2022-01-05 06:16:19.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_reject.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    48138 2022-05-18 13:43:21.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/misc.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    71737 2022-09-25 09:26:09.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/preproc.py
+drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-10 07:35:31.288626 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/tests/
+-rw-r--r--   0 ysbach     (501) staff       (20)        0 2021-05-21 01:18:27.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/tests/__init__.py
+-rw-r--r--   0 ysbach     (501) staff       (20)      663 2021-05-21 07:58:54.000000 NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/tests/test_misc.py
+drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-10 07:35:31.294154 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/
+-rw-r--r--   0 ysbach     (501) staff       (20)      211 2022-10-14 06:26:37.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/__init__.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    11282 2023-03-12 14:35:47.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/aperture.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    13683 2022-07-07 04:43:13.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/apphot.py
+-rw-r--r--   0 ysbach     (501) staff       (20)     5900 2022-06-09 12:31:35.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/background.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    34050 2022-07-15 05:38:34.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/center.py
+-rw-r--r--   0 ysbach     (501) staff       (20)     3710 2022-07-07 04:43:11.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/daopsf.py
+-rw-r--r--   0 ysbach     (501) staff       (20)     3147 2020-01-23 08:48:25.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/growth.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    31667 2023-04-10 07:16:07.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/polarimetry.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    48206 2022-10-14 07:48:11.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/queryutil.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    22802 2022-06-11 09:21:12.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/seputil.py
+drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-10 07:35:31.294976 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/tests/
+-rw-r--r--   0 ysbach     (501) staff       (20)      335 2022-06-09 11:56:23.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/tests/__init__.py
+-rw-r--r--   0 ysbach     (501) staff       (20)        0 2022-06-09 12:10:21.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/tests/test_apphot.py
+-rw-r--r--   0 ysbach     (501) staff       (20)      796 2022-06-09 12:31:38.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/tests/test_background.py
+-rw-r--r--   0 ysbach     (501) staff       (20)    11253 2023-04-07 17:31:30.000000 NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/util.py
+-rw-r--r--   0 ysbach     (501) staff       (20)       86 2022-10-14 06:37:14.000000 NICpolpy-0.1.5/pyproject.toml
+drwxr-xr-x   0 ysbach     (501) staff       (20)        0 2023-04-10 07:35:31.295343 NICpolpy-0.1.5/readme_images/
+-rw-r--r--   0 ysbach     (501) staff       (20)   985898 2020-01-09 09:23:17.000000 NICpolpy-0.1.5/readme_images/ap_selection.png
+-rw-r--r--   0 ysbach     (501) staff       (20)     1580 2023-04-10 07:35:31.297341 NICpolpy-0.1.5/setup.cfg
+-rw-r--r--   0 ysbach     (501) staff       (20)       69 2022-10-14 06:36:27.000000 NICpolpy-0.1.5/setup.py
```

### Comparing `NICpolpy-0.1.4/.gitignore` & `NICpolpy-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/LICENSE` & `NICpolpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/NICpolpy.egg-info/PKG-INFO` & `NICpolpy-0.1.5/NICpolpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NICpolpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nishi-Harima Astronomical Observatory (NHAO) Near-Infrared Camera (NIC) polarimetry pipeline.
 Home-page: https://github.com/ysBach/NICpolpy
 Author: Yoonsoo P. Bach
 Author-email: ysbach93@gmail.com,
 License: BSD 3-clause
 Project-URL: Source, https://github.com/ysBach/NICpolpy
 Project-URL: Tracker, https://github.com/ysBach/NICpolpy/issues
```

### Comparing `NICpolpy-0.1.4/NICpolpy.egg-info/SOURCES.txt` & `NICpolpy-0.1.5/NICpolpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/PKG-INFO` & `NICpolpy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NICpolpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nishi-Harima Astronomical Observatory (NHAO) Near-Infrared Camera (NIC) polarimetry pipeline.
 Home-page: https://github.com/ysBach/NICpolpy
 Author: Yoonsoo P. Bach
 Author-email: ysbach93@gmail.com,
 License: BSD 3-clause
 Project-URL: Source, https://github.com/ysBach/NICpolpy
 Project-URL: Tracker, https://github.com/ysBach/NICpolpy/issues
```

### Comparing `NICpolpy-0.1.4/README.md` & `NICpolpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/NICPolReduc.py` & `NICpolpy-0.1.5/nicpolpy/NICPolReduc.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/phot.py` & `NICpolpy-0.1.5/nicpolpy/phot.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/prepare.py` & `NICpolpy-0.1.5/nicpolpy/prepare.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/preproc.py` & `NICpolpy-0.1.5/nicpolpy/preproc.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/util.py` & `NICpolpy-0.1.5/nicpolpy/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from astropy.nddata import CCDData
 from astropy.stats import sigma_clipped_stats
 from astropy.time import Time
 from astropy.visualization import (ImageNormalize, LinearStretch,
                                    ZScaleInterval, simple_norm)
 from matplotlib import pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
+from scipy.stats import t as tdist
 
 from .ysfitsutilpy4nicpolpy import (CCDData_astype, cmt2hdr, find_extpix,
                                     find_satpix, give_stats, imslice,
                                     is_list_like, load_ccd, make_summary,
                                     slicefy)
 
 __all__ = ["iterator",
@@ -32,15 +33,16 @@
            #    "parse_fpath",
            "_save", "_summary_path_parse",
            "_set_dir_iol", "_sanitize_objects", "_sanitize_fits",
            "_load_as_dict", "_find_calframe",
            "_save_or_load_summary", "_select_summary_rows",
            "summary_nic", "zscale_lims", "norm_imshow", "vrange_sigc", "colorbaring",
            "thumb_with_stat", "thumb_with_satpix",
-           "plot_nightly_check_fig"
+           "plot_nightly_check_fig",
+           "outliers_gesd"
            ]
 
 
 def iterator(it, show_progress=True):
     if show_progress:
         try:
             from tqdm import tqdm
@@ -1284,7 +1286,149 @@
     plt.suptitle(figtitle)
 
     plt.tight_layout()
     fig.align_ylabels(axs)
     fig.align_xlabels(axs)
     plt.savefig(output)
     return fig, axs
+
+
+def outliers_gesd(
+        x: list | np.ndarray,
+        outliers: int = 5,
+        hypo: bool = False,
+        report: bool = False,
+        alpha: float = 0.05) -> np.ndarray:
+    """ Directly from https://github.com/maximtrp/scikit-posthocs/pull/56
+    The generalized (Extreme Studentized Deviate) ESD test is used
+    to detect one or more outliers in a univariate data set that follows
+    an approximately normal distribution [1]_.
+
+    Parameters
+    ----------
+    x : Union[List, np.ndarray]
+        An array, any object exposing the array interface, containing
+        data to test for outliers.
+    outliers : int = 5
+        Number of potential outliers to test for. Test is two-tailed, i.e.
+        maximum and minimum values are checked for potential outliers.
+    hypo : bool = False
+        Specifies whether to return a bool value of a hypothesis test result.
+        Returns True when we can reject the null hypothesis. Otherwise, False.
+        Available options are:
+        1) True - return a hypothesis test result.
+        2) False - return a filtered array without an outlier (default).
+    report : bool = False
+        Specifies whether to print a summary table of the test.
+    alpha : float = 0.05
+        Significance level for a hypothesis test.
+
+    Returns
+    -------
+    np.ndarray
+        Returns the filtered array if alternative hypo is True, otherwise an
+        unfiltered (input) array.
+
+    Notes
+    -----
+    .. [1] Rosner, Bernard (May 1983), Percentage Points for a Generalized
+        ESD Many-Outlier Procedure,Technometrics, 25(2), pp. 165-172.
+
+    Examples
+    --------
+    >>> data = np.array([-0.25, 0.68, 0.94, 1.15, 1.2, 1.26, 1.26, 1.34,
+        1.38, 1.43, 1.49, 1.49, 1.55, 1.56, 1.58, 1.65, 1.69, 1.7, 1.76,
+        1.77, 1.81, 1.91, 1.94, 1.96, 1.99, 2.06, 2.09, 2.1, 2.14, 2.15,
+        2.23, 2.24, 2.26, 2.35, 2.37, 2.4, 2.47, 2.54, 2.62, 2.64, 2.9,
+        2.92, 2.92, 2.93, 3.21, 3.26, 3.3, 3.59, 3.68, 4.3, 4.64, 5.34,
+        5.42, 6.01])
+    >>> outliers_gesd(data, 5)
+    array([-0.25,  0.68,  0.94,  1.15,  1.2 ,  1.26,  1.26,  1.34,  1.38,
+            1.43,  1.49,  1.49,  1.55,  1.56,  1.58,  1.65,  1.69,  1.7 ,
+            1.76,  1.77,  1.81,  1.91,  1.94,  1.96,  1.99,  2.06,  2.09,
+            2.1 ,  2.14,  2.15,  2.23,  2.24,  2.26,  2.35,  2.37,  2.4 ,
+            2.47,  2.54,  2.62,  2.64,  2.9 ,  2.92,  2.92,  2.93,  3.21,
+            3.26,  3.3 ,  3.59,  3.68,  4.3 ,  4.64])
+    >>> outliers_gesd(data, outliers = 5, report = True)
+    H0: no outliers in the data
+    Ha: up to 5 outliers in the data
+    Significance level:  α = 0.05
+    Reject H0 if Ri > Critical Value (λi)
+    Summary Table for Two-Tailed Test
+    ---------------------------------------
+          Exact           Test     Critical
+      Number of      Statistic    Value, λi
+    Outliers, i      Value, Ri          5 %
+    ---------------------------------------
+              1          3.119        3.159
+              2          2.943        3.151
+              3          3.179        3.144 *
+              4           2.81        3.136
+              5          2.816        3.128
+    """
+    rs, ls = np.zeros(outliers, dtype=float), np.zeros(outliers, dtype=float)
+    ms = []
+
+    data_proc = np.copy(x)
+    argsort_index = np.argsort(data_proc)
+    data = data_proc[argsort_index]
+    n = data_proc.size
+
+    # Lambda values (critical values): do not depend on the outliers.
+    nol = np.arange(outliers)  # the number of outliers
+    df = n - nol - 2  # degrees of freedom
+    t_ppr = tdist.ppf(1 - alpha / (2 * (n - nol)), df)
+    ls = ((n - nol - 1) * t_ppr) / np.sqrt((df + t_ppr**2) * (n - nol))
+
+    for i in np.arange(outliers):
+
+        abs_d = np.abs(data_proc - np.mean(data_proc))
+
+        # R-value calculation
+        R = np.max(abs_d) / np.std(data_proc, ddof=1)
+        rs[i] = R
+
+        # Masked values
+        lms = ms[-1] if len(ms) > 0 else []
+        ms.append(
+            lms + np.where(data == data_proc[np.argmax(abs_d)])[0].tolist())
+
+        # Remove the observation that maximizes |xi - xmean|
+        data_proc = np.delete(data_proc, np.argmax(abs_d))
+
+    if report:
+
+        report = ["H0: no outliers in the data",
+                  "Ha: up to " + str(outliers) + " outliers in the data",
+                  "Significance level:  α = " + str(alpha),
+                  "Reject H0 if Ri > Critical Value (λi)", "",
+                  "Summary Table for Two-Tailed Test",
+                  "---------------------------------------",
+                  "      Exact           Test     Critical",
+                  "  Number of      Statistic    Value, λi",
+                  "Outliers, i      Value, Ri      {:5.3g} %".format(100*alpha),
+                  "---------------------------------------"]
+
+        for i, (r, l) in enumerate(zip(rs, ls)):
+            report.append('{: >11s}'.format(str(i+1)) +
+                          '{: >15s}'.format(str(np.round(r, 3))) +
+                          '{: >13s}'.format(str(np.round(l, 3))) +
+                          (" *" if r > l else ""))
+
+        print("\n".join(report))
+
+    # Remove masked values
+    # for which the test statistic is greater
+    # than the critical value and return the result
+
+    if any(rs > ls):
+        if hypo:
+            data[:] = False
+            data[ms[np.max(np.where(rs > ls))]] = True
+            # rearrange data so mask is in same order as incoming data
+            data = np.vstack((data, np.arange(0, data.shape[0])[argsort_index]))
+            data = data[0, data.argsort()[1, ]]
+            data = data.astype('bool')
+        else:
+            data = np.delete(data, ms[np.max(np.where(rs > ls))])
+
+    return data
```

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/__init__.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/__init__.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/airmass.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/airmass.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/astroim.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/astroim.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/astrometry.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/astrometry.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/combutil.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/combutil.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/filemgmt.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/filemgmt.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/fitting.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/fitting.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/hduutil.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/hduutil.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/docstrings.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/docstrings.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imarith.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imarith.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imcombine.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imcombine.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imcopy.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imcopy.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imsmooth.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/imsmooth.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_comb.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_comb.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_lmedian.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_lmedian.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_reject.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/imutil/util_reject.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/misc.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/misc.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/preproc.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/preproc.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysfitsutilpy4nicpolpy/tests/test_misc.py` & `NICpolpy-0.1.5/nicpolpy/ysfitsutilpy4nicpolpy/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/aperture.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/aperture.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/apphot.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/apphot.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/background.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/background.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/center.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/center.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/daopsf.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/daopsf.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/growth.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/growth.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/polarimetry.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/polarimetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
     #     thr -= np.pi/2 if thr > np.pi else 0
     # else:
     #     thr[thr < 0] += np.pi/2
     #     thr[thr > np.pi] -= np.pi/2
     cos2r = np.cos(2*thr)
     sin2r = np.sin(2*thr)
     polr = pol*cos2r
-    dpolr = err_prop(dpol*cos2r, pol*(-2*sin2r)*dthp)
+    dpolr = np.max([err_prop(dpol*cos2r, pol*(-2*sin2r)*dthp), dpol], axis=0)
     dthr = err_prop(dthp, dsuntargetpa)
     polr, dpolr = convert_pct(polr, dpolr, already=False, convert2unit=out_pct)
     thr, dthr = convert_deg(thr, dthr, already=False, convert2unit=out_deg)
 
     return polr, thr, dpolr, dthr
```

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/queryutil.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/queryutil.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/seputil.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/seputil.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/tests/test_background.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/nicpolpy/ysphotutilpy4nicpolpy/util.py` & `NICpolpy-0.1.5/nicpolpy/ysphotutilpy4nicpolpy/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -340,141 +340,8 @@
     Notes
     -----
     photutils.centroids.GaussianConst2D is also usable.
     """
     fitted, fitter = fit_astropy_model(data=data, model_init=model_init, sigma=sigma, fitter=fitter, **kwargs)
     if correct:
         fitted = Gaussian2D_correct(fitted)
-    return fitted, fitter
-
-
-'''
-from warnings import warn
-from astropy.modeling import Fittable2DModel, Parameter
-from astropy.modeling.fitting import LevMarLSQFitter
-from astropy.modeling.models import CONSTRAINTS_DOC, Const2D, Moffat2D
-from astropy.utils.exceptions import AstropyUserWarning
-
-# TODO: Elliptical moffat...
-# https://iraf.net/irafhelp.php?val=daopars&help=Help+Page
-class MoffatConst2D(Fittable2DModel):
-    """
-    A model for a 2D Moffat plus a constant.
-
-    Parameters
-    ----------
-    constant : float
-        Value of the constant.
-    amplitude : float
-        Amplitude of the model.
-    x_0 : float
-        x position of the maximum of the Moffat model.
-    y_0 : float
-        y position of the maximum of the Moffat model.
-    gamma : float
-        Core width of the Moffat model.
-    alpha : float
-        Power index of the Moffat model.
-    """
-
-    constant = Parameter(default=1)
-    amplitude = Parameter(default=1)
-    x_0 = Parameter(default=0)
-    y_0 = Parameter(default=0)
-    gamma = Parameter(default=1)
-    alpha = Parameter(default=1)
-
-    @staticmethod
-    def evaluate(x, y, constant, amplitude, x_0, y_0, gamma, alpha):
-        """Two dimensional Gaussian plus constant function."""
-
-        model = Const2D(constant)(x, y) + Moffat2D(amplitude, x_0, y_0,
-                                                   gamma, alpha)(x, y)
-        return model
-
-
-MoffatConst2D.__doc__ += CONSTRAINTS_DOC
-
-
-def fit_2dmoffat(data, error=None, mask=None):
-    """
-    Fit a 2D Moffat plus a constant to a 2D image.
-
-    Invalid values (e.g. NaNs or infs) in the ``data`` or ``error``
-    arrays are automatically masked.  The mask for invalid values
-    represents the combination of the invalid-value masks for the
-    ``data`` and ``error`` arrays.
-
-    Parameters
-    ----------
-    data : array_like
-        The 2D array of the image.
-
-    error : array_like, optional
-        The 2D array of the 1-sigma errors of the input ``data``.
-
-    mask : array_like (bool), optional
-        A boolean mask, with the same shape as ``data``, where a `True`
-        value indicates the corresponding element of ``data`` is masked.
-
-    Returns
-    -------
-    result : A `MoffatConst2D` model instance.
-        The best-fitting Moffat 2D model.
-    """
-
-    from ..morphology import data_properties  # prevent circular imports
-
-    data = np.ma.asanyarray(data)
-
-    if mask is not None and mask is not np.ma.nomask:
-        mask = np.asanyarray(mask)
-        if data.shape != mask.shape:
-            raise ValueError('data and mask must have the same shape.')
-        data.mask |= mask
-
-    if np.any(~np.isfinite(data)):
-        data = np.ma.masked_invalid(data)
-        warn('Input data contains input values (e.g. NaNs or infs), '
-             'which were automatically masked.', AstropyUserWarning)
-
-    if error is not None:
-        error = np.ma.masked_invalid(error)
-        if data.shape != error.shape:
-            raise ValueError('data and error must have the same shape.')
-        data.mask |= error.mask
-        weights = 1.0 / error.clip(min=1.e-30)
-    else:
-        weights = np.ones(data.shape)
-
-    if np.ma.count(data) < 7:
-        raise ValueError('Input data must have a least 7 unmasked values to '
-                         'fit a 2D Moffat plus a constant.')
-
-    # assign zero weight to masked pixels
-    if data.mask is not np.ma.nomask:
-        weights[data.mask] = 0.
-
-    mask = data.mask
-    data.fill_value = 0.0
-    data = data.filled()
-
-    # Subtract the minimum of the data as a crude background estimate.
-    # This will also make the data values positive, preventing issues with
-    # the moment estimation in data_properties (moments from negative data
-    # values can yield undefined Gaussian parameters, e.g. x/y_stddev).
-    props = data_properties(data - np.min(data), mask=mask)
-
-    init_const = 0.  # subtracted data minimum above
-    init_amplitude = np.ptp(data)
-    g_init = GaussianConst2D(constant=init_const, amplitude=init_amplitude,
-                             x_mean=props.xcentroid.value,
-                             y_mean=props.ycentroid.value,
-                             x_stddev=props.semimajor_axis_sigma.value,
-                             y_stddev=props.semiminor_axis_sigma.value,
-                             theta=props.orientation.value)
-    fitter = LevMarLSQFitter()
-    y, x = np.indices(data.shape)
-    gfit = fitter(g_init, x, y, data, weights=weights)
-
-    return gfit
-'''
+    return fitted, fitter
```

### Comparing `NICpolpy-0.1.4/readme_images/ap_selection.png` & `NICpolpy-0.1.5/readme_images/ap_selection.png`

 * *Files identical despite different names*

### Comparing `NICpolpy-0.1.4/setup.cfg` & `NICpolpy-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = NICpolpy
-version = 0.1.4
+version = 0.1.5
 description = Nishi-Harima Astronomical Observatory (NHAO) Near-Infrared Camera (NIC) polarimetry pipeline.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/ysBach/NICpolpy
 author = Yoonsoo P. Bach
 author_email = ysbach93@gmail.com,
 license = BSD 3-clause
```

