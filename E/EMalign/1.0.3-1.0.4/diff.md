# Comparing `tmp/EMalign-1.0.3.tar.gz` & `tmp/EMalign-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EMalign-1.0.3.tar", last modified: Sun Dec 11 09:48:44 2022, max compression
+gzip compressed data, was "EMalign-1.0.4.tar", last modified: Mon Apr 10 11:49:05 2023, max compression
```

## Comparing `EMalign-1.0.3.tar` & `EMalign-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 yoelsh    (5722) math_shkolnisky (31855)        0 2022-12-11 09:48:44.033401 EMalign-1.0.3/
-drwxr-xr-x   0 yoelsh    (5722) math_shkolnisky (31855)        0 2022-12-11 09:48:44.033401 EMalign-1.0.3/EMalign.egg-info/
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     2672 2022-12-11 09:48:44.000000 EMalign-1.0.3/EMalign.egg-info/PKG-INFO
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)      684 2022-12-11 09:48:44.000000 EMalign-1.0.3/EMalign.egg-info/SOURCES.txt
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)        1 2022-12-11 09:48:44.000000 EMalign-1.0.3/EMalign.egg-info/dependency_links.txt
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)       42 2022-12-11 09:48:44.000000 EMalign-1.0.3/EMalign.egg-info/entry_points.txt
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)        1 2022-09-08 11:38:23.000000 EMalign-1.0.3/EMalign.egg-info/not-zip-safe
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)       46 2022-12-11 09:48:44.000000 EMalign-1.0.3/EMalign.egg-info/requires.txt
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)        4 2022-12-11 09:48:44.000000 EMalign-1.0.3/EMalign.egg-info/top_level.txt
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)    35149 2022-09-08 08:22:37.000000 EMalign-1.0.3/LICENSE
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     2672 2022-12-11 09:48:44.033401 EMalign-1.0.3/PKG-INFO
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     2363 2022-12-11 09:47:32.000000 EMalign-1.0.3/README.md
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)       38 2022-12-11 09:48:44.033401 EMalign-1.0.3/setup.cfg
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)      897 2022-12-11 09:47:45.000000 EMalign-1.0.3/setup.py
-drwxr-xr-x   0 yoelsh    (5722) math_shkolnisky (31855)        0 2022-12-11 09:48:44.033401 EMalign-1.0.3/src/
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)    12052 2022-09-08 08:22:37.000000 EMalign-1.0.3/src/SymmetryGroups.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)       17 2022-09-08 08:22:37.000000 EMalign-1.0.3/src/__init__.py
--rwxr-xr-x   0 yoelsh    (5722) math_shkolnisky (31855)       30 2022-09-08 08:22:37.000000 EMalign-1.0.3/src/__main__.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)    17431 2022-12-08 07:37:31.000000 EMalign-1.0.3/src/align_projection_2d.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)    26464 2022-12-11 09:19:10.000000 EMalign-1.0.3/src/align_volumes_3d.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     3172 2022-12-11 08:49:12.000000 EMalign-1.0.3/src/common_finufft.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     2307 2022-12-06 10:05:50.000000 EMalign-1.0.3/src/commonline_R2.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     2361 2022-12-11 09:37:09.000000 EMalign-1.0.3/src/cryo_fetch_emdID.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     5900 2022-09-08 08:22:37.000000 EMalign-1.0.3/src/cryo_project_itay_finufft.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)      666 2022-09-08 08:22:37.000000 EMalign-1.0.3/src/dev_utils.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     9533 2022-12-11 09:19:35.000000 EMalign-1.0.3/src/emalign_input.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)    13001 2022-12-06 10:05:50.000000 EMalign-1.0.3/src/fastrotate3d.py
--rwx------   0 yoelsh    (5722) math_shkolnisky (31855)    10077 2022-09-29 09:10:13.000000 EMalign-1.0.3/src/fastrotate3d_fftw.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)    14645 2022-10-01 17:47:27.000000 EMalign-1.0.3/src/fsc.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     3649 2022-09-08 08:22:37.000000 EMalign-1.0.3/src/genRotationsGrid.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     2692 2022-12-11 09:19:59.000000 EMalign-1.0.3/src/gentestdata.py
--rwxr-xr-x   0 yoelsh    (5722) math_shkolnisky (31855)     4459 2022-12-11 09:36:06.000000 EMalign-1.0.3/src/main.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     2200 2022-09-08 08:22:37.000000 EMalign-1.0.3/src/rand_rots.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     1703 2022-09-08 08:22:37.000000 EMalign-1.0.3/src/read_write.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     3954 2022-12-11 07:37:53.000000 EMalign-1.0.3/src/register_translations_3d.py
--rw-r--r--   0 yoelsh    (5722) math_shkolnisky (31855)     8647 2022-12-11 08:30:50.000000 EMalign-1.0.3/src/reshift_vol.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:49:05.000808 EMalign-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-04-10 11:49:04.580673 EMalign-1.0.4/EMalign.egg-info/
+-rw-rw-rw-   0        0        0     2931 2023-04-10 11:49:04.000000 EMalign-1.0.4/EMalign.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2023-04-10 11:49:04.000000 EMalign-1.0.4/EMalign.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 11:49:04.000000 EMalign-1.0.4/EMalign.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 11:49:04.000000 EMalign-1.0.4/EMalign.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-10 11:49:03.000000 EMalign-1.0.4/EMalign.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-04-10 11:49:04.000000 EMalign-1.0.4/EMalign.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-10 11:49:04.000000 EMalign-1.0.4/EMalign.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-04-10 11:45:41.000000 EMalign-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2931 2023-04-10 11:49:04.998814 EMalign-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2610 2023-04-10 11:45:41.000000 EMalign-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 11:49:05.001810 EMalign-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      926 2023-04-10 11:45:41.000000 EMalign-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:49:04.994825 EMalign-1.0.4/src/
+-rw-rw-rw-   0        0        0    12240 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/SymmetryGroups.py
+-rw-rw-rw-   0        0        0       18 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/__main__.py
+-rw-rw-rw-   0        0        0    17835 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/align_projection_2d.py
+-rw-rw-rw-   0        0        0    27079 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/align_volumes_3d.py
+-rw-rw-rw-   0        0        0     3347 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/common_finufft.py
+-rw-rw-rw-   0        0        0     2395 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/commonline_R2.py
+-rw-rw-rw-   0        0        0     2440 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/cryo_fetch_emdID.py
+-rw-rw-rw-   0        0        0     6053 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/cryo_project_itay_finufft.py
+-rw-rw-rw-   0        0        0      695 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/dev_utils.py
+-rw-rw-rw-   0        0        0    10429 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/emalign_input.py
+-rw-rw-rw-   0        0        0    13382 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/fastrotate3d.py
+-rw-rw-rw-   0        0        0    15115 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/fsc.py
+-rw-rw-rw-   0        0        0     3741 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/genRotationsGrid.py
+-rw-rw-rw-   0        0        0     2772 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/gentestdata.py
+-rw-rw-rw-   0        0        0     4880 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/main.py
+-rw-rw-rw-   0        0        0     2271 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/rand_rots.py
+-rw-rw-rw-   0        0        0     1757 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/read_write.py
+-rw-rw-rw-   0        0        0     4081 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/register_translations_3d.py
+-rw-rw-rw-   0        0        0     8886 2023-04-10 11:45:41.000000 EMalign-1.0.4/src/reshift_vol.py
```

### Comparing `EMalign-1.0.3/EMalign.egg-info/PKG-INFO` & `EMalign-1.0.4/EMalign.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Metadata-Version: 2.1
-Name: EMalign
-Version: 1.0.3
-Summary: EM align
-Home-page: https://github.com/ShkolniskyLab/EMalign
-Author: Yoel Shkolnisky
-Author-email: yoelsh@tauex.tau.ac.il
-License: GNU General Public License v3.0
-Requires-Python: ~=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1>emalign</h1>
-
-A algorithm for aligning rotation, reflection, and translation between volumes. 
-
-Current version: 1.0.3
-
-Project's homepage: https://github.com/ShkolniskyLab/emalign
-
-Date: 12/2022
-
-Please cite the following paper when using this package: 
-XXX
-
-<h2>Recommended Environments:</h2>
-The package has been tested on Ubuntu 18.04 and Windows 10. It should probably work on other versions of Windows and Linux, but has not been tested on them yet. Similarly for macOS.
-
-* Python 3.6.0+ is required.
-
-* The package makes use of the pyfftw package, which in turn uses the FFTW library. Before installing emalign make sure you have the FFTW library installed on your system: http://www.fftw.org/fftw3_doc/Installation-and-Customization.html#Installation-and-Customization
-
-
-<h2>Install emalign</h2>
-<h3>Install emalign via pip:</h3>
-We recommend installing emalign via pip:
-
-
-    $ pip install emalign
-
-<h3>Install emalign from source</h3>
-The tarball of the source tree is available via pip download emalign. You can install emalign from the tarball:
-
-
-    $ pip install emalign-x.x.x.tar.gz
-
-
-You can also install the development version of emalign from a cloned Git repository:
-
-
-    $ git clone https://github.com/ShkolniskyLab/emalign.git
-
-    $ cd emalign
-
-    $ pip install .
-
-<h2>Uninstall emalign</h2>
-Use pip to uninstall emalign:
-
-
-    $ pip uninstall emalign
-
-<h2>Upgrade emalign</h2>
-Just use pip with -U option:
-
-
-    $ pip install -U emalign
-
-<h2>Getting started:</h2>
-Please read the user manual for usage instructions, available at the homepage of the project on Github: https://github.com/ShkolniskyLab/emalign
-
-
-<h2>Basic usage:</h2>
-Generate test data via
-
-    $ emalign --make-test-data -v
-
-This will download EMD-2660 from EMDB (https://www.ebi.ac.uk/emdb/), downsample it to size 129 pixels (with pixel size 
-3.74A), and save the downsampled map into map_ref_2660.mrc. The function then rotates and shifts the map (see log messages 
-for the exact transformation parameters) and saves the transformed map to map_transformed_2660.mrc. These two maps can
-be used to test the alignment algorithm.
-
-Run the alignment algorithm via
-
-    $  emalign -v1 ./map_ref_2660.mrc -v2 ./map_transformed_2660.mrc -o ./map_aligned_2660.mrc -v
-
-The algorithm will align v2 to v1, saving the aligned map. 
-
-Type
-
-```   
-$  emalign -h 
-```
-
-for help.
-
+Metadata-Version: 2.1
+Name: EMalign
+Version: 1.0.4
+Summary: EM align
+Home-page: https://github.com/ShkolniskyLab/EMalign
+Author: Yoel Shkolnisky
+Author-email: yoelsh@tauex.tau.ac.il
+License: GNU General Public License v3.0
+Requires-Python: ~=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1>emalign</h1>
+
+A algorithm for aligning rotation, reflection, and translation between volumes. 
+
+Current version: 1.0.4
+
+Project's homepage: https://github.com/ShkolniskyLab/emalign
+
+Date: 12/2022
+
+Please cite the following paper when using this package: 
+Harpaz, Y., & Shkolnisky, Y. (2023). Three-dimensional alignment of density maps in cryo-electron microscopy. Biological Imaging, 3, E8. doi:10.1017/S2633903X23000089
+
+<h2>Recommended Environments:</h2>
+The package has been tested on Ubuntu 18.04 and Windows 10. It should probably work on other versions of Windows and Linux, but has not been tested on them yet. Similarly for macOS.
+
+* Python 3.6.0+ is required.
+
+* The package makes use of the pyfftw package, which in turn uses the FFTW library. Before installing emalign make sure you have the FFTW library installed on your system: http://www.fftw.org/fftw3_doc/Installation-and-Customization.html#Installation-and-Customization
+
+
+<h2>Install emalign</h2>
+<h3>Install emalign via pip:</h3>
+We recommend installing emalign via pip:
+
+
+    $ pip install emalign
+
+<h3>Install emalign from source</h3>
+The tarball of the source tree is available via pip download emalign. You can install emalign from the tarball:
+
+
+    $ pip install emalign-x.x.x.tar.gz
+
+
+You can also install the development version of emalign from a cloned Git repository:
+
+
+    $ git clone https://github.com/ShkolniskyLab/emalign.git
+
+    $ cd emalign
+
+    $ pip install .
+
+<h2>Uninstall emalign</h2>
+Use pip to uninstall emalign:
+
+
+    $ pip uninstall emalign
+
+<h2>Upgrade emalign</h2>
+Just use pip with -U option:
+
+
+    $ pip install -U emalign
+
+<h2>Getting started:</h2>
+Please read the user manual for usage instructions, available at the homepage of the project on Github: https://github.com/ShkolniskyLab/emalign
+
+
+<h2>Basic usage:</h2>
+Generate test data via
+
+    $ emalign --make-test-data -v
+
+This will download EMD-2660 from EMDB (https://www.ebi.ac.uk/emdb/), downsample it to size 129 pixels (with pixel size 
+3.74A), and save the downsampled map into map_ref_2660.mrc. The function then rotates and shifts the map (see log messages 
+for the exact transformation parameters) and saves the transformed map to map_transformed_2660.mrc. These two maps can
+be used to test the alignment algorithm.
+
+Run the alignment algorithm via
+
+    $  emalign -v1 ./map_ref_2660.mrc -v2 ./map_transformed_2660.mrc -o ./map_aligned_2660.mrc -v
+
+The algorithm will align v2 to v1, saving the aligned map. 
+
+Type
+
+```   
+$  emalign -h 
+```
+
+for help.
+
```

### Comparing `EMalign-1.0.3/EMalign.egg-info/SOURCES.txt` & `EMalign-1.0.4/EMalign.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 src/common_finufft.py
 src/commonline_R2.py
 src/cryo_fetch_emdID.py
 src/cryo_project_itay_finufft.py
 src/dev_utils.py
 src/emalign_input.py
 src/fastrotate3d.py
-src/fastrotate3d_fftw.py
 src/fsc.py
 src/genRotationsGrid.py
 src/gentestdata.py
 src/main.py
 src/rand_rots.py
 src/read_write.py
 src/register_translations_3d.py
```

### Comparing `EMalign-1.0.3/LICENSE` & `EMalign-1.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `EMalign-1.0.3/PKG-INFO` & `EMalign-1.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Metadata-Version: 2.1
-Name: EMalign
-Version: 1.0.3
-Summary: EM align
-Home-page: https://github.com/ShkolniskyLab/EMalign
-Author: Yoel Shkolnisky
-Author-email: yoelsh@tauex.tau.ac.il
-License: GNU General Public License v3.0
-Requires-Python: ~=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1>emalign</h1>
-
-A algorithm for aligning rotation, reflection, and translation between volumes. 
-
-Current version: 1.0.3
-
-Project's homepage: https://github.com/ShkolniskyLab/emalign
-
-Date: 12/2022
-
-Please cite the following paper when using this package: 
-XXX
-
-<h2>Recommended Environments:</h2>
-The package has been tested on Ubuntu 18.04 and Windows 10. It should probably work on other versions of Windows and Linux, but has not been tested on them yet. Similarly for macOS.
-
-* Python 3.6.0+ is required.
-
-* The package makes use of the pyfftw package, which in turn uses the FFTW library. Before installing emalign make sure you have the FFTW library installed on your system: http://www.fftw.org/fftw3_doc/Installation-and-Customization.html#Installation-and-Customization
-
-
-<h2>Install emalign</h2>
-<h3>Install emalign via pip:</h3>
-We recommend installing emalign via pip:
-
-
-    $ pip install emalign
-
-<h3>Install emalign from source</h3>
-The tarball of the source tree is available via pip download emalign. You can install emalign from the tarball:
-
-
-    $ pip install emalign-x.x.x.tar.gz
-
-
-You can also install the development version of emalign from a cloned Git repository:
-
-
-    $ git clone https://github.com/ShkolniskyLab/emalign.git
-
-    $ cd emalign
-
-    $ pip install .
-
-<h2>Uninstall emalign</h2>
-Use pip to uninstall emalign:
-
-
-    $ pip uninstall emalign
-
-<h2>Upgrade emalign</h2>
-Just use pip with -U option:
-
-
-    $ pip install -U emalign
-
-<h2>Getting started:</h2>
-Please read the user manual for usage instructions, available at the homepage of the project on Github: https://github.com/ShkolniskyLab/emalign
-
-
-<h2>Basic usage:</h2>
-Generate test data via
-
-    $ emalign --make-test-data -v
-
-This will download EMD-2660 from EMDB (https://www.ebi.ac.uk/emdb/), downsample it to size 129 pixels (with pixel size 
-3.74A), and save the downsampled map into map_ref_2660.mrc. The function then rotates and shifts the map (see log messages 
-for the exact transformation parameters) and saves the transformed map to map_transformed_2660.mrc. These two maps can
-be used to test the alignment algorithm.
-
-Run the alignment algorithm via
-
-    $  emalign -v1 ./map_ref_2660.mrc -v2 ./map_transformed_2660.mrc -o ./map_aligned_2660.mrc -v
-
-The algorithm will align v2 to v1, saving the aligned map. 
-
-Type
-
-```   
-$  emalign -h 
-```
-
-for help.
-
+Metadata-Version: 2.1
+Name: EMalign
+Version: 1.0.4
+Summary: EM align
+Home-page: https://github.com/ShkolniskyLab/EMalign
+Author: Yoel Shkolnisky
+Author-email: yoelsh@tauex.tau.ac.il
+License: GNU General Public License v3.0
+Requires-Python: ~=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1>emalign</h1>
+
+A algorithm for aligning rotation, reflection, and translation between volumes. 
+
+Current version: 1.0.4
+
+Project's homepage: https://github.com/ShkolniskyLab/emalign
+
+Date: 12/2022
+
+Please cite the following paper when using this package: 
+Harpaz, Y., & Shkolnisky, Y. (2023). Three-dimensional alignment of density maps in cryo-electron microscopy. Biological Imaging, 3, E8. doi:10.1017/S2633903X23000089
+
+<h2>Recommended Environments:</h2>
+The package has been tested on Ubuntu 18.04 and Windows 10. It should probably work on other versions of Windows and Linux, but has not been tested on them yet. Similarly for macOS.
+
+* Python 3.6.0+ is required.
+
+* The package makes use of the pyfftw package, which in turn uses the FFTW library. Before installing emalign make sure you have the FFTW library installed on your system: http://www.fftw.org/fftw3_doc/Installation-and-Customization.html#Installation-and-Customization
+
+
+<h2>Install emalign</h2>
+<h3>Install emalign via pip:</h3>
+We recommend installing emalign via pip:
+
+
+    $ pip install emalign
+
+<h3>Install emalign from source</h3>
+The tarball of the source tree is available via pip download emalign. You can install emalign from the tarball:
+
+
+    $ pip install emalign-x.x.x.tar.gz
+
+
+You can also install the development version of emalign from a cloned Git repository:
+
+
+    $ git clone https://github.com/ShkolniskyLab/emalign.git
+
+    $ cd emalign
+
+    $ pip install .
+
+<h2>Uninstall emalign</h2>
+Use pip to uninstall emalign:
+
+
+    $ pip uninstall emalign
+
+<h2>Upgrade emalign</h2>
+Just use pip with -U option:
+
+
+    $ pip install -U emalign
+
+<h2>Getting started:</h2>
+Please read the user manual for usage instructions, available at the homepage of the project on Github: https://github.com/ShkolniskyLab/emalign
+
+
+<h2>Basic usage:</h2>
+Generate test data via
+
+    $ emalign --make-test-data -v
+
+This will download EMD-2660 from EMDB (https://www.ebi.ac.uk/emdb/), downsample it to size 129 pixels (with pixel size 
+3.74A), and save the downsampled map into map_ref_2660.mrc. The function then rotates and shifts the map (see log messages 
+for the exact transformation parameters) and saves the transformed map to map_transformed_2660.mrc. These two maps can
+be used to test the alignment algorithm.
+
+Run the alignment algorithm via
+
+    $  emalign -v1 ./map_ref_2660.mrc -v2 ./map_transformed_2660.mrc -o ./map_aligned_2660.mrc -v
+
+The algorithm will align v2 to v1, saving the aligned map. 
+
+Type
+
+```   
+$  emalign -h 
+```
+
+for help.
+
```

### Comparing `EMalign-1.0.3/README.md` & `EMalign-1.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-<h1>emalign</h1>
-
-A algorithm for aligning rotation, reflection, and translation between volumes. 
-
-Current version: 1.0.3
-
-Project's homepage: https://github.com/ShkolniskyLab/emalign
-
-Date: 12/2022
-
-Please cite the following paper when using this package: 
-XXX
-
-<h2>Recommended Environments:</h2>
-The package has been tested on Ubuntu 18.04 and Windows 10. It should probably work on other versions of Windows and Linux, but has not been tested on them yet. Similarly for macOS.
-
-* Python 3.6.0+ is required.
-
-* The package makes use of the pyfftw package, which in turn uses the FFTW library. Before installing emalign make sure you have the FFTW library installed on your system: http://www.fftw.org/fftw3_doc/Installation-and-Customization.html#Installation-and-Customization
-
-
-<h2>Install emalign</h2>
-<h3>Install emalign via pip:</h3>
-We recommend installing emalign via pip:
-
-
-    $ pip install emalign
-
-<h3>Install emalign from source</h3>
-The tarball of the source tree is available via pip download emalign. You can install emalign from the tarball:
-
-
-    $ pip install emalign-x.x.x.tar.gz
-
-
-You can also install the development version of emalign from a cloned Git repository:
-
-
-    $ git clone https://github.com/ShkolniskyLab/emalign.git
-
-    $ cd emalign
-
-    $ pip install .
-
-<h2>Uninstall emalign</h2>
-Use pip to uninstall emalign:
-
-
-    $ pip uninstall emalign
-
-<h2>Upgrade emalign</h2>
-Just use pip with -U option:
-
-
-    $ pip install -U emalign
-
-<h2>Getting started:</h2>
-Please read the user manual for usage instructions, available at the homepage of the project on Github: https://github.com/ShkolniskyLab/emalign
-
-
-<h2>Basic usage:</h2>
-Generate test data via
-
-    $ emalign --make-test-data -v
-
-This will download EMD-2660 from EMDB (https://www.ebi.ac.uk/emdb/), downsample it to size 129 pixels (with pixel size 
-3.74A), and save the downsampled map into map_ref_2660.mrc. The function then rotates and shifts the map (see log messages 
-for the exact transformation parameters) and saves the transformed map to map_transformed_2660.mrc. These two maps can
-be used to test the alignment algorithm.
-
-Run the alignment algorithm via
-
-    $  emalign -v1 ./map_ref_2660.mrc -v2 ./map_transformed_2660.mrc -o ./map_aligned_2660.mrc -v
-
-The algorithm will align v2 to v1, saving the aligned map. 
-
-Type
-
-```   
-$  emalign -h 
-```
-
-for help.
-
+<h1>emalign</h1>
+
+A algorithm for aligning rotation, reflection, and translation between volumes. 
+
+Current version: 1.0.4
+
+Project's homepage: https://github.com/ShkolniskyLab/emalign
+
+Date: 12/2022
+
+Please cite the following paper when using this package: 
+Harpaz, Y., & Shkolnisky, Y. (2023). Three-dimensional alignment of density maps in cryo-electron microscopy. Biological Imaging, 3, E8. doi:10.1017/S2633903X23000089
+
+<h2>Recommended Environments:</h2>
+The package has been tested on Ubuntu 18.04 and Windows 10. It should probably work on other versions of Windows and Linux, but has not been tested on them yet. Similarly for macOS.
+
+* Python 3.6.0+ is required.
+
+* The package makes use of the pyfftw package, which in turn uses the FFTW library. Before installing emalign make sure you have the FFTW library installed on your system: http://www.fftw.org/fftw3_doc/Installation-and-Customization.html#Installation-and-Customization
+
+
+<h2>Install emalign</h2>
+<h3>Install emalign via pip:</h3>
+We recommend installing emalign via pip:
+
+
+    $ pip install emalign
+
+<h3>Install emalign from source</h3>
+The tarball of the source tree is available via pip download emalign. You can install emalign from the tarball:
+
+
+    $ pip install emalign-x.x.x.tar.gz
+
+
+You can also install the development version of emalign from a cloned Git repository:
+
+
+    $ git clone https://github.com/ShkolniskyLab/emalign.git
+
+    $ cd emalign
+
+    $ pip install .
+
+<h2>Uninstall emalign</h2>
+Use pip to uninstall emalign:
+
+
+    $ pip uninstall emalign
+
+<h2>Upgrade emalign</h2>
+Just use pip with -U option:
+
+
+    $ pip install -U emalign
+
+<h2>Getting started:</h2>
+Please read the user manual for usage instructions, available at the homepage of the project on Github: https://github.com/ShkolniskyLab/emalign
+
+
+<h2>Basic usage:</h2>
+Generate test data via
+
+    $ emalign --make-test-data -v
+
+This will download EMD-2660 from EMDB (https://www.ebi.ac.uk/emdb/), downsample it to size 129 pixels (with pixel size 
+3.74A), and save the downsampled map into map_ref_2660.mrc. The function then rotates and shifts the map (see log messages 
+for the exact transformation parameters) and saves the transformed map to map_transformed_2660.mrc. These two maps can
+be used to test the alignment algorithm.
+
+Run the alignment algorithm via
+
+    $  emalign -v1 ./map_ref_2660.mrc -v2 ./map_transformed_2660.mrc -o ./map_aligned_2660.mrc -v
+
+The algorithm will align v2 to v1, saving the aligned map. 
+
+Type
+
+```   
+$  emalign -h 
+```
+
+for help.
+
```

### Comparing `EMalign-1.0.3/setup.py` & `EMalign-1.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from setuptools import setup, find_packages
-from os import path
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(name='EMalign',
-      version='1.0.3',
-      description='EM align',
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      url='https://github.com/ShkolniskyLab/EMalign',
-      author='Yoel Shkolnisky',
-      author_email='yoelsh@tauex.tau.ac.il',
-      packages=find_packages(),
-      license='GNU General Public License v3.0',
-      entry_points={
-        "console_scripts": ['emalign = src.main:main']
-        },
-      install_requires=[
-          'numpy>=1.16',
-          'mrcfile',
-          'scipy>=1.3',
-          'pyfftw',
-          'finufft'
-      ],
-      python_requires='~=3.6',
-      zip_safe=False
-      )
+from setuptools import setup, find_packages
+from os import path
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(name='EMalign',
+      version='1.0.4',
+      description='EM align',
+      long_description=long_description,
+      long_description_content_type='text/markdown',
+      url='https://github.com/ShkolniskyLab/EMalign',
+      author='Yoel Shkolnisky',
+      author_email='yoelsh@tauex.tau.ac.il',
+      packages=find_packages(),
+      license='GNU General Public License v3.0',
+      entry_points={
+        "console_scripts": ['emalign = src.main:main']
+        },
+      install_requires=[
+          'numpy>=1.16',
+          'mrcfile',
+          'scipy>=1.3',
+          'pyfftw',
+          'finufft'
+      ],
+      python_requires='~=3.6',
+      zip_safe=False
+      )
```

### Comparing `EMalign-1.0.3/src/SymmetryGroups.py` & `EMalign-1.0.4/src/SymmetryGroups.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Feb 16 14:17:56 2021
-
-@author: yaelharpaz1
-"""
-
-import numpy as np
-from scipy.spatial.transform import Rotation as R
-from numpy import linalg as LA
-
-
-def genSymGroup(sym):  
-    # This function generates the symmetry group of the given symmetry type. 
-    # The symmetry elements are being generated according to the most common 
-    # coordinate systems of molecules from the EMDB. Note that it is necessary  
-    # to check that the generated symmetry group is indeed the appropriate one.  
-    ## Input:
-    # sym- the symmetry type- 'Cn'\'Dn'\'T'\'O'\'I', where n is the the symmetry
-    #      order.  
-    ## Output:
-    # G- size=(3,3,N) the symmetry group elemnts, where N is the amount of 
-    #    symmetry elements in G.    
-    #%%
-    s = sym[0] 
-    n_s = 0
-    if len(sym) > 1:
-        n_s = int(sym[1:len(sym)])
-    #%% Cyclic symmetry group:
-    if s == 'C':
-        if n_s == 0:
-            raise TypeError("The symmetry order must be an input in case of cyclic symmetry")
-        G = np.zeros((n_s,3,3))
-        theta = 2*180/n_s
-        for i in range(n_s):
-            G[i,:,:] = R.from_euler('z', i*theta, degrees=True).as_matrix()    
-    #%% Dihedral symmetry group:      
-    elif s == 'D':
-        if n_s == 0:
-            raise TypeError("The symmetry order must be an input in case of dihedral symmetry")         
-        G = np.zeros((2*n_s,3,3))
-        theta = 2*180/n_s    
-        for i in range(n_s):
-            G[i,:,:] = R.from_euler('z', i*theta, degrees=True).as_matrix()
-        G[n_s,:,:] = R.from_euler('y', 180, degrees=True).as_matrix()
-        for i in range(1,n_s):
-            G[n_s+i,:,:] = np.matmul(G[n_s,:,:],G[i,:,:])        
-    #%% T symmetry group:
-    elif s == 'T':    
-        n = 12                                  # The size of group T is 12
-        G = np.zeros((n,3,3))                       
-        G[0,:,:]  = np.eye(3)
-        G[1,:,:] = np.array([[0,0, 1],[ 1,0,0],[0, 1,0]])    # axis: [ 1, 1, 1] angle: 120
-        G[2,:,:] = np.array([[0, 1,0],[0,0, 1],[ 1,0,0]])    # axis: [ 1, 1, 1] angle: 240    G(2) = G(3)^T
-        G[3,:,:] = np.array([[0,0,-1],[ 1,0,0],[0,-1,0]])    # axis: [-1,-1, 1] angle: 120
-        G[4,:,:] = np.array([[0, 1,0],[0,0,-1],[-1,0,0]])    # axis: [-1,-1, 1] angle: 240    G(4) = G(3)^T
-        G[5,:,:] = np.array([[0,0,-1],[-1,0,0],[0, 1,0]])    # axis: [ 1,-1,-1] angle: 120
-        G[6,:,:] = np.array([[0,-1,0],[0,0, 1],[-1,0,0]])    # axis: [ 1,-1,-1] angle: 240    G(6) = G(5)^T
-        G[7,:,:] = np.array([[0,0, 1],[-1,0,0],[0,-1,0]])    # axis: [-1, 1,-1] angle: 120
-        G[8,:,:] = np.array([[0,-1,0],[0,0,-1],[ 1,0,0]])    # axis: [-1, 1,-1] angle: 240    G(8) = G(7)^T        
-        G[9,:,:] = np.array([[ 1,0,0],[0,-1,0],[0,0,-1]])    # axis: [ 1, 0, 0] angle: 180    G(9) = G(9)^T
-        G[10,:,:] = np.array([[-1,0,0],[0, 1,0],[0,0,-1]])    # axis: [ 0, 1, 0] angle: 180    G(10) = G(10)^T
-        G[11,:,:] = np.array([[-1,0,0],[0,-1,0],[0,0, 1]])    # axis: [ 0, 0, 1] angle: 180    G(11) = G(11)^T
-    #%% O symmetry group:
-    elif s == 'O':
-        n  = 24                                # The size of group O is 24
-        G = np.zeros((n,3,3))                        
-        G[0,:,:] = np.eye(3) 
-        G[1,:,:] = np.array([[0,-1,0],[ 1,0,0],[0,0, 1]])   
-        G[2,:,:] = np.array([[0, 1,0],[-1,0,0],[0,0, 1]])      # G_2 = G_1.'
-        G[3,:,:] = np.array([[ 1,0,0],[0,0,-1],[0, 1,0]])   
-        G[4,:,:] = np.array([[ 1,0,0],[0,0, 1],[0,-1,0]])      # G_4 = G_3.'
-        G[5,:,:] = np.array([[0,-1,0],[0,0,-1],[ 1,0,0]])   
-        G[6,:,:] = np.array([[0,0, 1],[-1,0,0],[0,-1,0]])      # G_6 = G_5.'
-        G[7,:,:] = np.array([[0,-1,0],[0,0, 1],[-1,0,0]])   
-        G[8,:,:] = np.array([[0,0,-1],[-1,0,0],[0, 1,0]])      # G_8 = G_7.'
-        G[9,:,:] = np.array([[0, 1,0],[0,0, 1],[ 1,0,0]])   
-        G[10,:,:] = np.array([[0,0, 1],[ 1,0,0],[0, 1,0]])      # G_10 = G_9.'
-        G[11,:,:] = np.array([[0,0, 1],[0, 1,0],[-1,0,0]])   
-        G[12,:,:] = np.array([[0,0,-1],[0, 1,0],[ 1,0,0]])      # G_12 = G_11.'
-        G[13,:,:] = np.array([[0, 1,0],[0,0,-1],[-1,0,0]])   
-        G[14,:,:] = np.array([[0,0,-1],[ 1,0,0],[0,-1,0]])      # G_14 = G_13.'   
-        G[15,:,:] = np.array([[-1,0,0],[0,-1,0],[0,0, 1]])      # 2-fold
-        G[16,:,:] = np.array([[-1,0,0],[0,0,-1],[0,-1,0]])   
-        G[17,:,:] = np.array([[ 1,0,0],[0,-1,0],[0,0,-1]])
-        G[18,:,:] = np.array([[0,-1,0],[-1,0,0],[0,0,-1]])   
-        G[19,:,:] = np.array([[-1,0,0],[0, 1,0],[0,0,-1]])
-        G[20,:,:] = np.array([[0, 1,0],[ 1,0,0],[0,0,-1]])   
-        G[21,:,:] = np.array([[-1,0,0],[0,0, 1],[0, 1,0]])
-        G[22,:,:] = np.array([[0,0, 1],[0,-1,0],[ 1,0,0]])   
-        G[23,:,:] = np.array([[0,0,-1],[0,-1,0],[-1,0,0]])
-    #%%
-    elif s =='I': 
-        n  = 60;                                 # The size of group I is 60
-        G = np.zeros((n,3,3))                        
-        phi = (1 + np.sqrt(5))/2
-        G[0,:,:] = np.eye(3) 
-        # 6 rotation axis joining the extreme opposite vertices, by angles 
-        # 2pi/5, 4pi/5, 6pi/5 and 8pi/5:
-        G[1,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([0, phi,  1]/LA.norm([0, phi,  1]))).as_matrix() 
-        G[2,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([0, phi,  1]/LA.norm([0, phi,  1]))).as_matrix()
-        G[3,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([0, phi,  1]/LA.norm([0, phi,  1]))).as_matrix()
-        G[4,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([0, phi,  1]/LA.norm([0, phi,  1]))).as_matrix()
-        
-        G[5,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([0, phi, -1]/LA.norm([0, phi, -1]))).as_matrix()
-        G[6,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([0, phi, -1]/LA.norm([0, phi, -1]))).as_matrix()
-        G[7,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([0, phi, -1]/LA.norm([0, phi, -1]))).as_matrix()
-        G[8,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([0, phi, -1]/LA.norm([0, phi, -1]))).as_matrix()
-        
-        G[9,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([1, 0,  phi]/LA.norm([1, 0,  phi]))).as_matrix()
-        G[10,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([1, 0,  phi]/LA.norm([1, 0,  phi]))).as_matrix()
-        G[11,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([1, 0,  phi]/LA.norm([1, 0,  phi]))).as_matrix()
-        G[12,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([1, 0,  phi]/LA.norm([1, 0,  phi]))).as_matrix()
-        
-        G[13,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([-1, 0, phi]/LA.norm([-1, 0, phi]))).as_matrix()
-        G[14,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([-1, 0, phi]/LA.norm([-1, 0, phi]))).as_matrix()
-        G[15,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([-1, 0, phi]/LA.norm([-1, 0, phi]))).as_matrix()
-        G[16,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([-1, 0, phi]/LA.norm([-1, 0, phi]))).as_matrix()
-        
-        G[17,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([phi, -1, 0]/LA.norm([phi, -1, 0]))).as_matrix()
-        G[18,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([phi, -1, 0]/LA.norm([phi, -1, 0]))).as_matrix()
-        G[19,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([phi, -1, 0]/LA.norm([phi, -1, 0]))).as_matrix()
-        G[20,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([phi, -1, 0]/LA.norm([phi, -1, 0]))).as_matrix()
-        
-        G[21,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([phi,  1, 0]/LA.norm([phi,  1, 0]))).as_matrix()
-        G[22,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([phi,  1, 0]/LA.norm([phi,  1, 0]))).as_matrix()
-        G[23,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([phi,  1, 0]/LA.norm([phi,  1, 0]))).as_matrix()
-        G[24,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([phi,  1, 0]/LA.norm([phi,  1, 0]))).as_matrix()
-    
-        # 10 rotation axis joining the centers of opposite faces, by angles 
-        # 2pi/3 and 4pi/3:  
-        G[25,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([0,-1,phi**2]/LA.norm([0,-1,phi**2]))).as_matrix()
-        G[26,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([0,-1,phi**2]/LA.norm([0,-1,phi**2]))).as_matrix()
-        
-        G[27,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([0, 1,phi**2]/LA.norm([0, 1,phi**2]))).as_matrix()
-        G[28,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([0, 1,phi**2]/LA.norm([0, 1,phi**2]))).as_matrix()
-        
-        G[29,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([-1,phi**2,0]/LA.norm([-1,phi**2,0]))).as_matrix()
-        G[30,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([-1,phi**2,0]/LA.norm([-1,phi**2,0]))).as_matrix()
-        
-        G[31:,:] = R.from_rotvec((2*np.pi)/3 * np.array([ 1,phi**2,0]/LA.norm([ 1,phi**2,0]))).as_matrix()
-        G[32,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([ 1,phi**2,0]/LA.norm([ 1,phi**2,0]))).as_matrix()
-        
-        G[33,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([phi**2,0,-1]/LA.norm([phi**2,0,-1]))).as_matrix()
-        G[34,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([phi**2,0,-1]/LA.norm([phi**2,0,-1]))).as_matrix()
-        
-        G[35,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([phi**2,0, 1]/LA.norm([phi**2,0, 1]))).as_matrix()
-        G[36,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([phi**2,0, 1]/LA.norm([phi**2,0, 1]))).as_matrix()
-        
-        G[37,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([  1, -1, 1]/LA.norm([  1, -1, 1]))).as_matrix()
-        G[38,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([  1, -1, 1]/LA.norm([  1, -1, 1]))).as_matrix()
-    
-        G[39,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([ -1,  1, 1]/LA.norm([ -1,  1, 1]))).as_matrix()
-        G[40,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([ -1,  1, 1]/LA.norm([ -1,  1, 1]))).as_matrix()
-
-        G[41,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([  1, 1, -1]/LA.norm([  1, 1, -1]))).as_matrix()
-        G[42,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([  1, 1, -1]/LA.norm([  1, 1, -1]))).as_matrix()
-
-        G[43,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([  1, 1,  1]/LA.norm([  1, 1,  1]))).as_matrix()
-        G[44,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([  1, 1,  1]/LA.norm([  1, 1,  1]))).as_matrix()
-    
-        # 15 rotation axis joining the midpoints of opposite edges, by angle pi:
-        G[45,:,:] = R.from_rotvec(np.pi * np.array([  0,   1,  0]/LA.norm([  0,   1,  0]))).as_matrix()
-        G[46,:,:] = R.from_rotvec(np.pi * np.array([  0,   0,  1]/LA.norm([  0,   0,  1]))).as_matrix()                                   
-        G[47,:,:] = R.from_rotvec(np.pi * np.array([  1,   0,  0]/LA.norm([  1,   0,  0]))).as_matrix()                                  
-        G[48,:,:] = R.from_rotvec(np.pi * np.array([-1/phi,1,phi]/LA.norm([-1/phi,1,phi]))).as_matrix()
-        G[49,:,:] = R.from_rotvec(np.pi * np.array([1/phi,-1,phi]/LA.norm([1/phi,-1,phi]))).as_matrix()
-        G[50,:,:] = R.from_rotvec(np.pi * np.array([1/phi,1,-phi]/LA.norm([1/phi,1,-phi]))).as_matrix()
-        G[51,:,:] = R.from_rotvec(np.pi * np.array([1/phi, 1,phi]/LA.norm([1/phi, 1,phi]))).as_matrix()
-        G[52,:,:] = R.from_rotvec(np.pi * np.array([-1,phi,1/phi]/LA.norm([-1,phi,1/phi]))).as_matrix()
-        G[53,:,:] = R.from_rotvec(np.pi * np.array([1,-phi,1/phi]/LA.norm([1,-phi,1/phi]))).as_matrix()
-        G[54,:,:] = R.from_rotvec(np.pi * np.array([1,phi,-1/phi]/LA.norm([1,phi,-1/phi]))).as_matrix()
-        G[55,:,:] = R.from_rotvec(np.pi * np.array([1,phi, 1/phi]/LA.norm([1,phi, 1/phi]))).as_matrix()
-        G[56,:,:] = R.from_rotvec(np.pi * np.array([-phi,1/phi,1]/LA.norm([-phi,1/phi,1]))).as_matrix()
-        G[57,:,:] = R.from_rotvec(np.pi * np.array([phi,-1/phi,1]/LA.norm([phi,-1/phi,1]))).as_matrix()
-        G[58,:,:] = R.from_rotvec(np.pi * np.array([phi,1/phi,-1]/LA.norm([phi,1/phi,-1]))).as_matrix()
-        G[59,:,:] = R.from_rotvec(np.pi * np.array([phi,1/phi, 1]/LA.norm([phi,1/phi, 1]))).as_matrix()
-        
-        O_g = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]]) #x-y axes transformation matrix.
-        for i in range(60): 
-            G[i,:,:] = O_g @ G[i,:,:] @ O_g.T
-    
-    else: 
-        raise TypeError("sym was not entered properly")               
-    return G
-
-
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Feb 16 14:17:56 2021
+
+@author: yaelharpaz1
+"""
+
+import numpy as np
+from scipy.spatial.transform import Rotation as R
+from numpy import linalg as LA
+
+
+def genSymGroup(sym):  
+    # This function generates the symmetry group of the given symmetry type. 
+    # The symmetry elements are being generated according to the most common 
+    # coordinate systems of molecules from the EMDB. Note that it is necessary  
+    # to check that the generated symmetry group is indeed the appropriate one.  
+    ## Input:
+    # sym- the symmetry type- 'Cn'\'Dn'\'T'\'O'\'I', where n is the the symmetry
+    #      order.  
+    ## Output:
+    # G- size=(3,3,N) the symmetry group elemnts, where N is the amount of 
+    #    symmetry elements in G.    
+    #%%
+    s = sym[0] 
+    n_s = 0
+    if len(sym) > 1:
+        n_s = int(sym[1:len(sym)])
+    #%% Cyclic symmetry group:
+    if s == 'C':
+        if n_s == 0:
+            raise TypeError("The symmetry order must be an input in case of cyclic symmetry")
+        G = np.zeros((n_s,3,3))
+        theta = 2*180/n_s
+        for i in range(n_s):
+            G[i,:,:] = R.from_euler('z', i*theta, degrees=True).as_matrix()    
+    #%% Dihedral symmetry group:      
+    elif s == 'D':
+        if n_s == 0:
+            raise TypeError("The symmetry order must be an input in case of dihedral symmetry")         
+        G = np.zeros((2*n_s,3,3))
+        theta = 2*180/n_s    
+        for i in range(n_s):
+            G[i,:,:] = R.from_euler('z', i*theta, degrees=True).as_matrix()
+        G[n_s,:,:] = R.from_euler('y', 180, degrees=True).as_matrix()
+        for i in range(1,n_s):
+            G[n_s+i,:,:] = np.matmul(G[n_s,:,:],G[i,:,:])        
+    #%% T symmetry group:
+    elif s == 'T':    
+        n = 12                                  # The size of group T is 12
+        G = np.zeros((n,3,3))                       
+        G[0,:,:]  = np.eye(3)
+        G[1,:,:] = np.array([[0,0, 1],[ 1,0,0],[0, 1,0]])    # axis: [ 1, 1, 1] angle: 120
+        G[2,:,:] = np.array([[0, 1,0],[0,0, 1],[ 1,0,0]])    # axis: [ 1, 1, 1] angle: 240    G(2) = G(3)^T
+        G[3,:,:] = np.array([[0,0,-1],[ 1,0,0],[0,-1,0]])    # axis: [-1,-1, 1] angle: 120
+        G[4,:,:] = np.array([[0, 1,0],[0,0,-1],[-1,0,0]])    # axis: [-1,-1, 1] angle: 240    G(4) = G(3)^T
+        G[5,:,:] = np.array([[0,0,-1],[-1,0,0],[0, 1,0]])    # axis: [ 1,-1,-1] angle: 120
+        G[6,:,:] = np.array([[0,-1,0],[0,0, 1],[-1,0,0]])    # axis: [ 1,-1,-1] angle: 240    G(6) = G(5)^T
+        G[7,:,:] = np.array([[0,0, 1],[-1,0,0],[0,-1,0]])    # axis: [-1, 1,-1] angle: 120
+        G[8,:,:] = np.array([[0,-1,0],[0,0,-1],[ 1,0,0]])    # axis: [-1, 1,-1] angle: 240    G(8) = G(7)^T        
+        G[9,:,:] = np.array([[ 1,0,0],[0,-1,0],[0,0,-1]])    # axis: [ 1, 0, 0] angle: 180    G(9) = G(9)^T
+        G[10,:,:] = np.array([[-1,0,0],[0, 1,0],[0,0,-1]])    # axis: [ 0, 1, 0] angle: 180    G(10) = G(10)^T
+        G[11,:,:] = np.array([[-1,0,0],[0,-1,0],[0,0, 1]])    # axis: [ 0, 0, 1] angle: 180    G(11) = G(11)^T
+    #%% O symmetry group:
+    elif s == 'O':
+        n  = 24                                # The size of group O is 24
+        G = np.zeros((n,3,3))                        
+        G[0,:,:] = np.eye(3) 
+        G[1,:,:] = np.array([[0,-1,0],[ 1,0,0],[0,0, 1]])   
+        G[2,:,:] = np.array([[0, 1,0],[-1,0,0],[0,0, 1]])      # G_2 = G_1.'
+        G[3,:,:] = np.array([[ 1,0,0],[0,0,-1],[0, 1,0]])   
+        G[4,:,:] = np.array([[ 1,0,0],[0,0, 1],[0,-1,0]])      # G_4 = G_3.'
+        G[5,:,:] = np.array([[0,-1,0],[0,0,-1],[ 1,0,0]])   
+        G[6,:,:] = np.array([[0,0, 1],[-1,0,0],[0,-1,0]])      # G_6 = G_5.'
+        G[7,:,:] = np.array([[0,-1,0],[0,0, 1],[-1,0,0]])   
+        G[8,:,:] = np.array([[0,0,-1],[-1,0,0],[0, 1,0]])      # G_8 = G_7.'
+        G[9,:,:] = np.array([[0, 1,0],[0,0, 1],[ 1,0,0]])   
+        G[10,:,:] = np.array([[0,0, 1],[ 1,0,0],[0, 1,0]])      # G_10 = G_9.'
+        G[11,:,:] = np.array([[0,0, 1],[0, 1,0],[-1,0,0]])   
+        G[12,:,:] = np.array([[0,0,-1],[0, 1,0],[ 1,0,0]])      # G_12 = G_11.'
+        G[13,:,:] = np.array([[0, 1,0],[0,0,-1],[-1,0,0]])   
+        G[14,:,:] = np.array([[0,0,-1],[ 1,0,0],[0,-1,0]])      # G_14 = G_13.'   
+        G[15,:,:] = np.array([[-1,0,0],[0,-1,0],[0,0, 1]])      # 2-fold
+        G[16,:,:] = np.array([[-1,0,0],[0,0,-1],[0,-1,0]])   
+        G[17,:,:] = np.array([[ 1,0,0],[0,-1,0],[0,0,-1]])
+        G[18,:,:] = np.array([[0,-1,0],[-1,0,0],[0,0,-1]])   
+        G[19,:,:] = np.array([[-1,0,0],[0, 1,0],[0,0,-1]])
+        G[20,:,:] = np.array([[0, 1,0],[ 1,0,0],[0,0,-1]])   
+        G[21,:,:] = np.array([[-1,0,0],[0,0, 1],[0, 1,0]])
+        G[22,:,:] = np.array([[0,0, 1],[0,-1,0],[ 1,0,0]])   
+        G[23,:,:] = np.array([[0,0,-1],[0,-1,0],[-1,0,0]])
+    #%%
+    elif s =='I': 
+        n  = 60;                                 # The size of group I is 60
+        G = np.zeros((n,3,3))                        
+        phi = (1 + np.sqrt(5))/2
+        G[0,:,:] = np.eye(3) 
+        # 6 rotation axis joining the extreme opposite vertices, by angles 
+        # 2pi/5, 4pi/5, 6pi/5 and 8pi/5:
+        G[1,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([0, phi,  1]/LA.norm([0, phi,  1]))).as_matrix() 
+        G[2,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([0, phi,  1]/LA.norm([0, phi,  1]))).as_matrix()
+        G[3,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([0, phi,  1]/LA.norm([0, phi,  1]))).as_matrix()
+        G[4,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([0, phi,  1]/LA.norm([0, phi,  1]))).as_matrix()
+        
+        G[5,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([0, phi, -1]/LA.norm([0, phi, -1]))).as_matrix()
+        G[6,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([0, phi, -1]/LA.norm([0, phi, -1]))).as_matrix()
+        G[7,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([0, phi, -1]/LA.norm([0, phi, -1]))).as_matrix()
+        G[8,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([0, phi, -1]/LA.norm([0, phi, -1]))).as_matrix()
+        
+        G[9,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([1, 0,  phi]/LA.norm([1, 0,  phi]))).as_matrix()
+        G[10,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([1, 0,  phi]/LA.norm([1, 0,  phi]))).as_matrix()
+        G[11,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([1, 0,  phi]/LA.norm([1, 0,  phi]))).as_matrix()
+        G[12,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([1, 0,  phi]/LA.norm([1, 0,  phi]))).as_matrix()
+        
+        G[13,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([-1, 0, phi]/LA.norm([-1, 0, phi]))).as_matrix()
+        G[14,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([-1, 0, phi]/LA.norm([-1, 0, phi]))).as_matrix()
+        G[15,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([-1, 0, phi]/LA.norm([-1, 0, phi]))).as_matrix()
+        G[16,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([-1, 0, phi]/LA.norm([-1, 0, phi]))).as_matrix()
+        
+        G[17,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([phi, -1, 0]/LA.norm([phi, -1, 0]))).as_matrix()
+        G[18,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([phi, -1, 0]/LA.norm([phi, -1, 0]))).as_matrix()
+        G[19,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([phi, -1, 0]/LA.norm([phi, -1, 0]))).as_matrix()
+        G[20,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([phi, -1, 0]/LA.norm([phi, -1, 0]))).as_matrix()
+        
+        G[21,:,:] = R.from_rotvec((2*np.pi)/5 * np.array([phi,  1, 0]/LA.norm([phi,  1, 0]))).as_matrix()
+        G[22,:,:] = R.from_rotvec((4*np.pi)/5 * np.array([phi,  1, 0]/LA.norm([phi,  1, 0]))).as_matrix()
+        G[23,:,:] = R.from_rotvec((6*np.pi)/5 * np.array([phi,  1, 0]/LA.norm([phi,  1, 0]))).as_matrix()
+        G[24,:,:] = R.from_rotvec((8*np.pi)/5 * np.array([phi,  1, 0]/LA.norm([phi,  1, 0]))).as_matrix()
+    
+        # 10 rotation axis joining the centers of opposite faces, by angles 
+        # 2pi/3 and 4pi/3:  
+        G[25,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([0,-1,phi**2]/LA.norm([0,-1,phi**2]))).as_matrix()
+        G[26,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([0,-1,phi**2]/LA.norm([0,-1,phi**2]))).as_matrix()
+        
+        G[27,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([0, 1,phi**2]/LA.norm([0, 1,phi**2]))).as_matrix()
+        G[28,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([0, 1,phi**2]/LA.norm([0, 1,phi**2]))).as_matrix()
+        
+        G[29,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([-1,phi**2,0]/LA.norm([-1,phi**2,0]))).as_matrix()
+        G[30,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([-1,phi**2,0]/LA.norm([-1,phi**2,0]))).as_matrix()
+        
+        G[31:,:] = R.from_rotvec((2*np.pi)/3 * np.array([ 1,phi**2,0]/LA.norm([ 1,phi**2,0]))).as_matrix()
+        G[32,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([ 1,phi**2,0]/LA.norm([ 1,phi**2,0]))).as_matrix()
+        
+        G[33,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([phi**2,0,-1]/LA.norm([phi**2,0,-1]))).as_matrix()
+        G[34,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([phi**2,0,-1]/LA.norm([phi**2,0,-1]))).as_matrix()
+        
+        G[35,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([phi**2,0, 1]/LA.norm([phi**2,0, 1]))).as_matrix()
+        G[36,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([phi**2,0, 1]/LA.norm([phi**2,0, 1]))).as_matrix()
+        
+        G[37,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([  1, -1, 1]/LA.norm([  1, -1, 1]))).as_matrix()
+        G[38,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([  1, -1, 1]/LA.norm([  1, -1, 1]))).as_matrix()
+    
+        G[39,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([ -1,  1, 1]/LA.norm([ -1,  1, 1]))).as_matrix()
+        G[40,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([ -1,  1, 1]/LA.norm([ -1,  1, 1]))).as_matrix()
+
+        G[41,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([  1, 1, -1]/LA.norm([  1, 1, -1]))).as_matrix()
+        G[42,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([  1, 1, -1]/LA.norm([  1, 1, -1]))).as_matrix()
+
+        G[43,:,:] = R.from_rotvec((2*np.pi)/3 * np.array([  1, 1,  1]/LA.norm([  1, 1,  1]))).as_matrix()
+        G[44,:,:] = R.from_rotvec((4*np.pi)/3 * np.array([  1, 1,  1]/LA.norm([  1, 1,  1]))).as_matrix()
+    
+        # 15 rotation axis joining the midpoints of opposite edges, by angle pi:
+        G[45,:,:] = R.from_rotvec(np.pi * np.array([  0,   1,  0]/LA.norm([  0,   1,  0]))).as_matrix()
+        G[46,:,:] = R.from_rotvec(np.pi * np.array([  0,   0,  1]/LA.norm([  0,   0,  1]))).as_matrix()                                   
+        G[47,:,:] = R.from_rotvec(np.pi * np.array([  1,   0,  0]/LA.norm([  1,   0,  0]))).as_matrix()                                  
+        G[48,:,:] = R.from_rotvec(np.pi * np.array([-1/phi,1,phi]/LA.norm([-1/phi,1,phi]))).as_matrix()
+        G[49,:,:] = R.from_rotvec(np.pi * np.array([1/phi,-1,phi]/LA.norm([1/phi,-1,phi]))).as_matrix()
+        G[50,:,:] = R.from_rotvec(np.pi * np.array([1/phi,1,-phi]/LA.norm([1/phi,1,-phi]))).as_matrix()
+        G[51,:,:] = R.from_rotvec(np.pi * np.array([1/phi, 1,phi]/LA.norm([1/phi, 1,phi]))).as_matrix()
+        G[52,:,:] = R.from_rotvec(np.pi * np.array([-1,phi,1/phi]/LA.norm([-1,phi,1/phi]))).as_matrix()
+        G[53,:,:] = R.from_rotvec(np.pi * np.array([1,-phi,1/phi]/LA.norm([1,-phi,1/phi]))).as_matrix()
+        G[54,:,:] = R.from_rotvec(np.pi * np.array([1,phi,-1/phi]/LA.norm([1,phi,-1/phi]))).as_matrix()
+        G[55,:,:] = R.from_rotvec(np.pi * np.array([1,phi, 1/phi]/LA.norm([1,phi, 1/phi]))).as_matrix()
+        G[56,:,:] = R.from_rotvec(np.pi * np.array([-phi,1/phi,1]/LA.norm([-phi,1/phi,1]))).as_matrix()
+        G[57,:,:] = R.from_rotvec(np.pi * np.array([phi,-1/phi,1]/LA.norm([phi,-1/phi,1]))).as_matrix()
+        G[58,:,:] = R.from_rotvec(np.pi * np.array([phi,1/phi,-1]/LA.norm([phi,1/phi,-1]))).as_matrix()
+        G[59,:,:] = R.from_rotvec(np.pi * np.array([phi,1/phi, 1]/LA.norm([phi,1/phi, 1]))).as_matrix()
+        
+        O_g = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]]) #x-y axes transformation matrix.
+        for i in range(60): 
+            G[i,:,:] = O_g @ G[i,:,:] @ O_g.T
+    
+    else: 
+        raise TypeError("sym was not entered properly")               
+    return G
+
+
```

### Comparing `EMalign-1.0.3/src/align_projection_2d.py` & `EMalign-1.0.4/src/align_projection_2d.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,404 +1,404 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Feb 23 10:56:14 2021
-
-@author: yaelharpaz1
-"""
-
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Feb  9 16:55:46 2021
-
-@author: yaelharpaz1
-"""
-import time
-import numpy as np
-import math
-import cmath
-import logging
-import threading
-from concurrent.futures import ThreadPoolExecutor
-from concurrent.futures import wait
-
-from src.cryo_project_itay_finufft import cryo_project
-from src.common_finufft import cryo_pft
-#from src.commonline_R2 import commonline_R2, cryo_normalize
-from src.commonline_R2 import cryo_normalize
-from src.genRotationsGrid import genRotationsGrid
-from numpy import linalg as LA
-
-def compute_commonlines_aux(Rj,candidate_rots,L):
-    Nrot = candidate_rots.shape[2]
-    Ckj = (-1)*np.ones((Nrot),dtype=int)
-    Cjk = (-1)*np.ones((Nrot),dtype=int)
-    Mkj = np.zeros((Nrot),dtype=int)
-        
-    for k in range(Nrot):
-        Rk = np.transpose(candidate_rots[:,:,k])
-        dot_RkRj = Rk[0,2]*Rj[0,2] + Rk[1,2]*Rj[1,2] + Rk[2,2]*Rj[2,2]
-        if dot_RkRj < 0.999:
-            Rk3 = Rk[2,:]
-            Rj3 = Rj[2,:]
-
-            clvec = np.array([[Rk3[1]*Rj3[2] - Rk3[2]*Rj3[1]],
-                                 [Rk3[2]*Rj3[0] - Rk3[0]*Rj3[2]],
-                                 [Rk3[0]*Rj3[1] - Rk3[1]*Rj3[0]]])
-
-            cij = Rk @ clvec
-            cji = Rj @ clvec
-                    
-            alphaij = math.atan2(cij[1], cij[0])
-            alphaji = math.atan2(cji[1], cji[0])
-                
-            alphaij = alphaij + np.pi 
-            alphaji = alphaji + np.pi 
-                
-            l_ij = alphaij/(2*np.pi )*L
-            l_ji = alphaji/(2*np.pi )*L
-                
-            ckj = int(round(l_ij) % L)
-            cjk = int(round(l_ji) % L)
-                
-            Ckj[k] = ckj
-            Cjk[k] = cjk
-            Mkj[k] = 1
-            
-    return Ckj, Cjk, Mkj
-
-def align_projection(projs,vol,verbose=0,opt=None):
-    '''
-    This function aligns given projection in a given volume.
-    This is a secondary algorithm for cryo_align_vols.
-    input: 
-    projs- projection images for the alignment.
-    vol- reference volume.
-    verbose- Set verbose to nonzero for verbose printouts (default is zero).
-    opt- Structure with optimizer options.
-    
-    output:
-        Rots_est- size=3x3x(size(projs,3)). The estimated rotation matrices of 
-                  the projections. If we project the volume in these
-                  orientations we will receive the same projections.
-        Shifts- size=(size(projs,3))x2. The 2D estimated shift of the 
-                projections, first column contained the shift in the x-axis, and  
-                the secound colunm in the y-axis.
-        corrs- size=size((projs,3))x2. Statistics of the alignment. The i'th  
-               entry of the first column contains the correlation of the common    
-               lines between the i'th image and all the reference images induced  
-               by the best matching rotation. The  i'th entry of the second   
-               column contains the mean matching correlation over all tested 
-               rotations.
-        err_Rots- error calculation between the true rotations and the estimated
-                  rotations.
-        err_shifts- error calculation between the true shifts and the estimated
-                    shifts, in x and y axis.
-    Options:
-        opt.sym- the symmetry type- 'Cn'\'Dn'\'T'\'O'\'I', where n is the the 
-             symmetry order (for example: 'C2'). This input is reqired only for 
-             the error calculation.
-        opt.Nprojs- number of reference projections for the alignment. (default 
-                   is 30).
-        opt.isshift- set isshift to nonzero in order to estimate the translations 
-                     of the projections (default is zero).
-        opt.G- Array of matrices of size 3x3xn containing the symmetry group
-               elemnts. This input is for error calculation. 
-        opt.trueRots- the true rotations of the projections.
-        opt.trueRots_J- the true rotations of the projections in case of 
-                      reflection between the projection and the volume.
-        opt.trueShifts- the true shifts-(dx,dy) of projs.
-        opt.Rots - size=3x3x(size(Rots,3)). a set of candidate rotations.
-    '''
-    #logging.basicConfig(level=logging.DEBUG,
-    #format='%(asctime)s %(levelname)s %(message)s')
-    logger = logging.getLogger()  
-    if verbose == 0 : logger.disabled = True
-    
-    # Check options:
-    if hasattr(opt,'sym'): sym = opt.sym
-    else: sym = None    
-    
-    if hasattr(opt,'Nprojs'): Nprojs = opt.Nprojs
-    else: Nprojs = 30
-        
-    if hasattr(opt,'G'): G = opt.G
-    else: G = None
-        
-    if hasattr(opt,'trueRots'): trueRots = opt.trueRots
-    else: trueRots = None
-        
-    if hasattr(opt,'trueRots_J'): trueRots_J = opt.trueRots_J
-    else: trueRots_J = None
-        
-    if hasattr(opt,'isshift'): isshift = opt.isshift
-    else: isshift = 0
-        
-    if hasattr(opt,'trueShifts'): trueShifts = opt.trueShifts
-    else: trueShifts = None  
-        
-    if hasattr(opt,'Rots'): Rots = opt.Rots
-    else: Rots = None  
-    
-    # Define parameters:
-    G_flag = 0
-    if sym is not None:   
-        s = sym[0] 
-        n_s = 0
-        if s == 'C' and n_s == 1: 
-            G = np.eye(3).reshape((1,3,3))     
-    if G is not None:
-        G_flag = 1   
-        # The symmetry group should be adjusted so it will be acurate for the 
-        # projection images. We use the permute function on the projections 
-        # such that it replaces the x-axis and the y-axis, so we have to do the
-        # same for the symmetry group.
-        n_g = np.size(G,0)
-        O_g = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]]) #x-y axes transformation matrix.
-        for i in range(n_g): 
-            G[i,:,:] = O_g @ G[i,:,:] @ O_g.T
-    refrot = 1
-    if trueRots is None: refrot = 0        
-    refrot_J = 1
-    if trueRots_J is None: refrot_J = 0
-    refshift = 1
-    if trueShifts is None: refshift = 0
-    canrots = 1
-    if Rots is None: canrots = 0                
-    n = np.size(vol,0); n_r = math.ceil(n/2); 
-    L = 360
-                        
-    # Compute polar Fourier transform of projs:
-    logger.info('Computing polar Fourier transform of unaligned projections using n_r= %i, L= %i',n_r,L)  
-    projs_hat = cryo_pft(projs,n_r,L)[0]
-    # Normalize polar Fourier transforms:
-    logger.info('Normalizing the polar Fourier transform of unaligned projections')
-    projs_hat = cryo_normalize(projs_hat)
-    n_projs = np.size(projs_hat,2)
-    
-    # Generate candidate rotations and reference projections:
-    logger.info('Generating %i reference projections', Nprojs)
-    if canrots == 0:
-        Rots = genRotationsGrid(75)
-    candidate_rots = Rots
-    Nrot = np.size(candidate_rots,2)
-    logger.info('Using %i candidate rotations for the alignment', Nrot)     
-    rots_ref = Rots[:,:,np.random.randint(Nrot, size=Nprojs)] 
-    #rots_ref = mat_to_npy('rots_ref_for_align_projection_2d')
-    
-    ref_projs = cryo_project(vol, rots_ref)    
-    ref_projs = np.transpose(ref_projs,(1,0,2))  
-    rots_ref = np.transpose(rots_ref,(1,0,2)) # the true rots
-    
-    # Compute polar Fourier transform of reference projections:
-    logger.info('Computing polar Fourier transform of reference projections using n_r=%i, L=%i', n_r, L)
-    refprojs_hat = cryo_pft(ref_projs,n_r,L)[0]
-    # Normalize polar Fourier transforms:
-    logger.info('Normalizing the polar Fourier transform of reference projections')
-    refprojs_hat = cryo_normalize(refprojs_hat)
-            
-    # Compute the common lines between the candidate rotations and the 
-    # references:
-    logger.info('Computing the common lines between reference and unaligned projections')     
-
-    t1 = time.perf_counter()
-    Ckj = (-1)*np.ones((Nrot,Nprojs),dtype=int)
-    Cjk = (-1)*np.ones((Nrot,Nprojs),dtype=int)
-    Mkj = np.zeros((Nrot,Nprojs),dtype=int)
-    for j in range(Nprojs):
-        Rj = np.transpose(rots_ref[:,:,j])
-        for k in range(Nrot):
-            Rk = np.transpose(candidate_rots[:,:,k])
-            #if np.sum(Rk[:,2] @ Rj[:,2]) < 0.999:
-                
-            # The following is an optimization of np.dot(Rk[:,2],Rj[:,2])
-            dot_RkRj = Rk[0,2]*Rj[0,2] + Rk[1,2]*Rj[1,2] + Rk[2,2]*Rj[2,2]
-            if dot_RkRj < 0.999:
-                                
-                #(ckj,cjk) = commonline_R2(Rk,Rj,L)
-                # Embed call to eliminate overhead
-                ##############################
-                Rk3 = Rk[2,:]
-                Rj3 = Rj[2,:]
-
-                clvec = np.array([[Rk3[1]*Rj3[2] - Rk3[2]*Rj3[1]],
-                                  [Rk3[2]*Rj3[0] - Rk3[0]*Rj3[2]],
-                                  [Rk3[0]*Rj3[1] - Rk3[1]*Rj3[0]]])
-
-
-                cij = Rk @ clvec
-                cji = Rj @ clvec
-                    
-                alphaij = math.atan2(cij[1], cij[0])
-                alphaji = math.atan2(cji[1], cji[0])
-                
-                alphaij = alphaij + np.pi 
-                alphaji = alphaji + np.pi 
-                
-                l_ij = alphaij/(2*np.pi )*L
-                l_ji = alphaji/(2*np.pi )*L
-                
-                ckj = int(round(l_ij) % L)
-                cjk = int(round(l_ji) % L)
-                
-                #(tmpckj,tmpcjk) = commonline_R2(Rk,Rj,L)
-                #assert(tmpckj==ckj and tmpcjk==cjk)
-                ##############################
-                # Convert the returned indices ckj and cjk into 1-based
-                Ckj[k,j] = ckj
-                Cjk[k,j] = cjk
-                Mkj[k,j] = 1
-                
-    t2 = time.perf_counter()
-    logger.info('Computing the common lines is done. Took %5.2f seconds', t2-t1)
-   
-# Multithreaded version of the above code, if we need it some day.
-# Currently it is slower than the above code.    
-# =============================================================================
-#     t1 = time.perf_counter()    
-#     Ckj2 = (-1)*np.ones((Nrot,Nprojs),dtype=int)
-#     Cjk2 = (-1)*np.ones((Nrot,Nprojs),dtype=int)
-#     Mkj2 = np.zeros((Nrot,Nprojs),dtype=int)
-# 
-#     futures = []
-#     with ThreadPoolExecutor(max_workers=threading.active_count()) as executor:
-#         for j in range(Nprojs):
-#             Rj = np.transpose(rots_ref[:,:,j])
-#             f = executor.submit(compute_commonlines_aux, Rj,candidate_rots,L)
-#             futures.append(f)
-# 
-#     wait(futures)
-# 
-#     for j in range(Nprojs):
-#         c1, c2, m = futures[j].result()   
-#         Ckj2[:,j] = c1
-#         Cjk2[:,j] = c2
-#         Mkj2[:,j] = m
-#     t2 = time.perf_counter()        
-#     logger.info('Computing the common lines is done. Took %5.2f seconds', t2-t1)
-#     assert(np.sum(np.abs(Ckj-Ckj2))==0)
-#     assert(np.sum(np.abs(Cjk-Cjk2))==0)
-#     assert(np.sum(np.abs(Mkj-Mkj2))==0)
-#     
-# =============================================================================
-    # Generate shift grid:
-    # generating a shift grid on the common lines, and choosing the shift
-    # that brings the best correlation in the comparisson between the common 
-    # lines. 
-    # after applying polar FFT on each projection, the shift in quartesian
-    # coordinates- (delta(x),delta(y)) becomes a shift only in the r variable
-    # in the common lines (the common line have a specific theta so we have to
-    # consider a shift only in the r variable.
-    # the equation for the shift phase in the common lines is:
-    # exp((-2*pi*i)*r*delta(r)).
-    max_s = int(np.round(0.2*np.size(projs_hat,0))) # set the maximum shift.
-    s_step = 0.5
-    n_shifts = int((2/s_step)*max_s + 1) # always odd number (to have zero value without shift).
-    max_r = np.size(projs_hat,0)
-    s_vec = np.linspace(-max_s,max_s,n_shifts).reshape((1,n_shifts)) # those are the shifts in the r variable in the common lines. 
-    r_vec = np.arange(max_r).reshape((1,max_r))
-    s_phases = np.exp((-2*math.pi*cmath.sqrt(-1))/(2*max_r+1)*(r_vec.conj().T @ s_vec)) # size of (n_rXn_shift)
-    
-    # Main loop- compute the cross correlation: 
-    # computing the correlation between the common line, first choose the best
-    # shift, and then chose the best rotation.
-    logger.info('Aligning unaligned projections using reference projections')
-    Rots_est = np.zeros((3,3,n_projs))
-    corrs = np.zeros((n_projs,2)) # Statistics on common-lines matching.
-    shifts = np.zeros((2,n_projs))
-    dtheta = 2*math.pi/L
-    if refrot == 1:
-        err_Rots = np.zeros((n_projs,1))
-    if refshift == 1:
-        err_shifts = np.zeros((2,n_projs))
-    for projidx in range(n_projs):
-        cross_corr_m = np.zeros((Nrot,Nprojs))
-        for j in range(Nprojs):
-            iidx = np.array(np.where(Mkj[:,j] != 0)).T
-            conv_hat = (projs_hat[:,Ckj[iidx,j],projidx].conj() * refprojs_hat[:,Cjk[iidx,j],j]).reshape((n_r,np.size(iidx,axis=0))) # size of (n_rxsize(iidx))
-            temp_corr = np.real(s_phases.conj().T @ conv_hat)
-            cross_corr_m[iidx,j] = temp_corr.max(axis=0).reshape(iidx.shape)
-        # calculating the mean of each row in cross_corr_m:
-        cross_corr = (np.sum(cross_corr_m,axis=1)/np.sum(cross_corr_m>0,axis=1)).reshape((Nrot,1))       
-        # Find estimated rotation:
-        bestRscore = np.amax(cross_corr)
-        bestRidx = np.array(np.where(cross_corr == bestRscore))[0,0]
-        meanRscore = np.mean(cross_corr)
-        corrs[projidx,0] = bestRscore
-        corrs[projidx,1] = meanRscore
-        Rots_est[:,:,projidx] = candidate_rots[:,:,bestRidx]       
-        # Error calculation for estimated rotation:
-        if refrot == 1 and G_flag == 1:
-            g_est_t = Rots_est[:,:,projidx] @ trueRots[:,:,projidx].T
-            n_g = np.size(G,0)
-            dist = np.zeros((n_g,1))
-            for g_idx in range(n_g):
-                dist[g_idx,0] = LA.norm(g_est_t-G[g_idx,:,:],'fro')
-            minidx = np.array(np.where(dist == np.amin(dist)))
-            g_est = G[minidx[0,0],:,:]           
-            R_est = g_est.T @ Rots_est[:,:,projidx]
-            R = trueRots[:,:,projidx] @ R_est.T
-            err_Rots[projidx,:] = np.rad2deg(math.acos((np.trace(R)-1)/2))
-        # Error calculation for reflection case:
-        # if there is a reflection between the projection and the volume
-        # then, the relation is R_est=gJRJ.
-        if refrot_J == 1 and G_flag == 1:
-            J3 = np.diag([1, 1, -1])
-            g_est_t = Rots_est[:,:,projidx] @ (J3 @ trueRots_J[:,:,projidx] @ J3).T
-            n_g = np.size(G,0)
-            dist = np.zeros((n_g,1))
-            for g_idx in range(n_g):
-                dist[g_idx,0] = LA.norm(g_est_t-G[g_idx,:,:],'fro')
-            min_idx = np.array(np.where(dist == np.amin(dist)))
-            g_est = G[min_idx[0,0],:,:]    
-            R_est = J3 @ g_est.T @ Rots_est[:,:,projidx] @ J3
-            R = trueRots_J[:,:,projidx] @ R_est.T
-            err_2 = np.rad2deg(math.acos((np.trace(R)-1)/2)) 
-            if err_Rots[projidx,:] != 0:
-                if err_Rots[projidx,:] <= err_2:
-                    err_Rots[projidx,:] = err_Rots[projidx,:]
-                else:
-                    err_Rots[projidx,:] = err_2
-            else:
-                err_Rots[projidx,:] = err_2 
-        
-        # Find estimated shift:
-        # by least-squares on the estimated rotation with the reference projections. 
-        if isshift == 1:
-            idx = np.array(np.where(Mkj[bestRidx,:] == 1)).transpose()
-            n = np.size(idx,0)
-            shift_eq = np.zeros((n,2))
-            shift = np.zeros((n,1))
-            i=0
-            for j in idx:
-                conv_hat = projs_hat[:,Ckj[bestRidx,j],projidx].conj() * refprojs_hat[:,Cjk[bestRidx,j],j] # size of (n_rxsize(iidx))
-                temp_corr = np.real(s_phases.conj().T @ conv_hat) # size of (n_shiftX1). 
-                s_idx = np.array(np.where(temp_corr == temp_corr.max(axis=0)))
-                shift[i,0] = s_vec[s_idx[1,0],s_idx[0,0]]
-                theta = (Ckj[bestRidx,j]-1)*dtheta # Angle of the common line.
-                shift_eq[i,0] = math.sin(theta)
-                shift_eq[i,1] = math.cos(theta)
-                i = i+1
-            shifts[:,projidx] = LA.lstsq(shift_eq,shift)[0].reshape(2)
-            # Error calc for estimated shifts:
-            if refshift != 0:
-                err_shifts[0,projidx] = LA.norm(trueShifts[projidx,0]-shifts[0,projidx],2)
-                err_shifts[1,projidx] = LA.norm(trueShifts[projidx,1]-shifts[1,projidx],2)
-    if refrot == 1 and G_flag == 1:
-        mean_err = np.mean(err_Rots)
-        logger.info('Mean error in estimating the rotations of the projections is: %.3f degrees', mean_err)
-    if isshift == 1 and refshift == 1:
-        mean_err_shift = np.mean(err_shifts)
-        logger.info('Mean error in estimating the translations of the projections is: %.3f', mean_err_shift)
-        
-    logging.shutdown()
-    
-    if refrot != 0 and G_flag != 0 and isshift != 0 and refshift != 0:
-        return Rots_est, shifts, corrs, err_Rots, err_shifts
-    elif refrot != 0 and G_flag != 0 and isshift == 0 and refshift == 0:
-        return Rots_est, shifts, corrs, err_Rots
-    elif refrot == 0 and G_flag == 0 and isshift != 0 and refshift != 0:
-        return Rots_est, shifts, corrs, err_shifts
-    else:
-        return Rots_est, shifts, corrs
-    
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Feb 23 10:56:14 2021
+
+@author: yaelharpaz1
+"""
+
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Feb  9 16:55:46 2021
+
+@author: yaelharpaz1
+"""
+import time
+import numpy as np
+import math
+import cmath
+import logging
+import threading
+from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import wait
+
+from src.cryo_project_itay_finufft import cryo_project
+from src.common_finufft import cryo_pft
+#from src.commonline_R2 import commonline_R2, cryo_normalize
+from src.commonline_R2 import cryo_normalize
+from src.genRotationsGrid import genRotationsGrid
+from numpy import linalg as LA
+
+def compute_commonlines_aux(Rj,candidate_rots,L):
+    Nrot = candidate_rots.shape[2]
+    Ckj = (-1)*np.ones((Nrot),dtype=int)
+    Cjk = (-1)*np.ones((Nrot),dtype=int)
+    Mkj = np.zeros((Nrot),dtype=int)
+        
+    for k in range(Nrot):
+        Rk = np.transpose(candidate_rots[:,:,k])
+        dot_RkRj = Rk[0,2]*Rj[0,2] + Rk[1,2]*Rj[1,2] + Rk[2,2]*Rj[2,2]
+        if dot_RkRj < 0.999:
+            Rk3 = Rk[2,:]
+            Rj3 = Rj[2,:]
+
+            clvec = np.array([[Rk3[1]*Rj3[2] - Rk3[2]*Rj3[1]],
+                                 [Rk3[2]*Rj3[0] - Rk3[0]*Rj3[2]],
+                                 [Rk3[0]*Rj3[1] - Rk3[1]*Rj3[0]]])
+
+            cij = Rk @ clvec
+            cji = Rj @ clvec
+                    
+            alphaij = math.atan2(cij[1], cij[0])
+            alphaji = math.atan2(cji[1], cji[0])
+                
+            alphaij = alphaij + np.pi 
+            alphaji = alphaji + np.pi 
+                
+            l_ij = alphaij/(2*np.pi )*L
+            l_ji = alphaji/(2*np.pi )*L
+                
+            ckj = int(round(l_ij) % L)
+            cjk = int(round(l_ji) % L)
+                
+            Ckj[k] = ckj
+            Cjk[k] = cjk
+            Mkj[k] = 1
+            
+    return Ckj, Cjk, Mkj
+
+def align_projection(projs,vol,verbose=0,opt=None):
+    '''
+    This function aligns given projection in a given volume.
+    This is a secondary algorithm for cryo_align_vols.
+    input: 
+    projs- projection images for the alignment.
+    vol- reference volume.
+    verbose- Set verbose to nonzero for verbose printouts (default is zero).
+    opt- Structure with optimizer options.
+    
+    output:
+        Rots_est- size=3x3x(size(projs,3)). The estimated rotation matrices of 
+                  the projections. If we project the volume in these
+                  orientations we will receive the same projections.
+        Shifts- size=(size(projs,3))x2. The 2D estimated shift of the 
+                projections, first column contained the shift in the x-axis, and  
+                the secound colunm in the y-axis.
+        corrs- size=size((projs,3))x2. Statistics of the alignment. The i'th  
+               entry of the first column contains the correlation of the common    
+               lines between the i'th image and all the reference images induced  
+               by the best matching rotation. The  i'th entry of the second   
+               column contains the mean matching correlation over all tested 
+               rotations.
+        err_Rots- error calculation between the true rotations and the estimated
+                  rotations.
+        err_shifts- error calculation between the true shifts and the estimated
+                    shifts, in x and y axis.
+    Options:
+        opt.sym- the symmetry type- 'Cn'\'Dn'\'T'\'O'\'I', where n is the the 
+             symmetry order (for example: 'C2'). This input is reqired only for 
+             the error calculation.
+        opt.Nprojs- number of reference projections for the alignment. (default 
+                   is 30).
+        opt.isshift- set isshift to nonzero in order to estimate the translations 
+                     of the projections (default is zero).
+        opt.G- Array of matrices of size 3x3xn containing the symmetry group
+               elemnts. This input is for error calculation. 
+        opt.trueRots- the true rotations of the projections.
+        opt.trueRots_J- the true rotations of the projections in case of 
+                      reflection between the projection and the volume.
+        opt.trueShifts- the true shifts-(dx,dy) of projs.
+        opt.Rots - size=3x3x(size(Rots,3)). a set of candidate rotations.
+    '''
+    #logging.basicConfig(level=logging.DEBUG,
+    #format='%(asctime)s %(levelname)s %(message)s')
+    logger = logging.getLogger()  
+    if verbose == 0 : logger.disabled = True
+    
+    # Check options:
+    if hasattr(opt,'sym'): sym = opt.sym
+    else: sym = None    
+    
+    if hasattr(opt,'Nprojs'): Nprojs = opt.Nprojs
+    else: Nprojs = 30
+        
+    if hasattr(opt,'G'): G = opt.G
+    else: G = None
+        
+    if hasattr(opt,'trueRots'): trueRots = opt.trueRots
+    else: trueRots = None
+        
+    if hasattr(opt,'trueRots_J'): trueRots_J = opt.trueRots_J
+    else: trueRots_J = None
+        
+    if hasattr(opt,'isshift'): isshift = opt.isshift
+    else: isshift = 0
+        
+    if hasattr(opt,'trueShifts'): trueShifts = opt.trueShifts
+    else: trueShifts = None  
+        
+    if hasattr(opt,'Rots'): Rots = opt.Rots
+    else: Rots = None  
+    
+    # Define parameters:
+    G_flag = 0
+    if sym is not None:   
+        s = sym[0] 
+        n_s = 0
+        if s == 'C' and n_s == 1: 
+            G = np.eye(3).reshape((1,3,3))     
+    if G is not None:
+        G_flag = 1   
+        # The symmetry group should be adjusted so it will be acurate for the 
+        # projection images. We use the permute function on the projections 
+        # such that it replaces the x-axis and the y-axis, so we have to do the
+        # same for the symmetry group.
+        n_g = np.size(G,0)
+        O_g = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]]) #x-y axes transformation matrix.
+        for i in range(n_g): 
+            G[i,:,:] = O_g @ G[i,:,:] @ O_g.T
+    refrot = 1
+    if trueRots is None: refrot = 0        
+    refrot_J = 1
+    if trueRots_J is None: refrot_J = 0
+    refshift = 1
+    if trueShifts is None: refshift = 0
+    canrots = 1
+    if Rots is None: canrots = 0                
+    n = np.size(vol,0); n_r = math.ceil(n/2); 
+    L = 360
+                        
+    # Compute polar Fourier transform of projs:
+    logger.info('Computing polar Fourier transform of unaligned projections using n_r= %i, L= %i',n_r,L)  
+    projs_hat = cryo_pft(projs,n_r,L)[0]
+    # Normalize polar Fourier transforms:
+    logger.info('Normalizing the polar Fourier transform of unaligned projections')
+    projs_hat = cryo_normalize(projs_hat)
+    n_projs = np.size(projs_hat,2)
+    
+    # Generate candidate rotations and reference projections:
+    logger.info('Generating %i reference projections', Nprojs)
+    if canrots == 0:
+        Rots = genRotationsGrid(75)
+    candidate_rots = Rots
+    Nrot = np.size(candidate_rots,2)
+    logger.info('Using %i candidate rotations for the alignment', Nrot)     
+    rots_ref = Rots[:,:,np.random.randint(Nrot, size=Nprojs)] 
+    #rots_ref = mat_to_npy('rots_ref_for_align_projection_2d')
+    
+    ref_projs = cryo_project(vol, rots_ref)    
+    ref_projs = np.transpose(ref_projs,(1,0,2))  
+    rots_ref = np.transpose(rots_ref,(1,0,2)) # the true rots
+    
+    # Compute polar Fourier transform of reference projections:
+    logger.info('Computing polar Fourier transform of reference projections using n_r=%i, L=%i', n_r, L)
+    refprojs_hat = cryo_pft(ref_projs,n_r,L)[0]
+    # Normalize polar Fourier transforms:
+    logger.info('Normalizing the polar Fourier transform of reference projections')
+    refprojs_hat = cryo_normalize(refprojs_hat)
+            
+    # Compute the common lines between the candidate rotations and the 
+    # references:
+    logger.info('Computing the common lines between reference and unaligned projections')     
+
+    t1 = time.perf_counter()
+    Ckj = (-1)*np.ones((Nrot,Nprojs),dtype=int)
+    Cjk = (-1)*np.ones((Nrot,Nprojs),dtype=int)
+    Mkj = np.zeros((Nrot,Nprojs),dtype=int)
+    for j in range(Nprojs):
+        Rj = np.transpose(rots_ref[:,:,j])
+        for k in range(Nrot):
+            Rk = np.transpose(candidate_rots[:,:,k])
+            #if np.sum(Rk[:,2] @ Rj[:,2]) < 0.999:
+                
+            # The following is an optimization of np.dot(Rk[:,2],Rj[:,2])
+            dot_RkRj = Rk[0,2]*Rj[0,2] + Rk[1,2]*Rj[1,2] + Rk[2,2]*Rj[2,2]
+            if dot_RkRj < 0.999:
+                                
+                #(ckj,cjk) = commonline_R2(Rk,Rj,L)
+                # Embed call to eliminate overhead
+                ##############################
+                Rk3 = Rk[2,:]
+                Rj3 = Rj[2,:]
+
+                clvec = np.array([[Rk3[1]*Rj3[2] - Rk3[2]*Rj3[1]],
+                                  [Rk3[2]*Rj3[0] - Rk3[0]*Rj3[2]],
+                                  [Rk3[0]*Rj3[1] - Rk3[1]*Rj3[0]]])
+
+
+                cij = Rk @ clvec
+                cji = Rj @ clvec
+                    
+                alphaij = math.atan2(cij[1], cij[0])
+                alphaji = math.atan2(cji[1], cji[0])
+                
+                alphaij = alphaij + np.pi 
+                alphaji = alphaji + np.pi 
+                
+                l_ij = alphaij/(2*np.pi )*L
+                l_ji = alphaji/(2*np.pi )*L
+                
+                ckj = int(round(l_ij) % L)
+                cjk = int(round(l_ji) % L)
+                
+                #(tmpckj,tmpcjk) = commonline_R2(Rk,Rj,L)
+                #assert(tmpckj==ckj and tmpcjk==cjk)
+                ##############################
+                # Convert the returned indices ckj and cjk into 1-based
+                Ckj[k,j] = ckj
+                Cjk[k,j] = cjk
+                Mkj[k,j] = 1
+                
+    t2 = time.perf_counter()
+    logger.info('Computing the common lines is done. Took %5.2f seconds', t2-t1)
+   
+# Multithreaded version of the above code, if we need it some day.
+# Currently it is slower than the above code.    
+# =============================================================================
+#     t1 = time.perf_counter()    
+#     Ckj2 = (-1)*np.ones((Nrot,Nprojs),dtype=int)
+#     Cjk2 = (-1)*np.ones((Nrot,Nprojs),dtype=int)
+#     Mkj2 = np.zeros((Nrot,Nprojs),dtype=int)
+# 
+#     futures = []
+#     with ThreadPoolExecutor(max_workers=threading.active_count()) as executor:
+#         for j in range(Nprojs):
+#             Rj = np.transpose(rots_ref[:,:,j])
+#             f = executor.submit(compute_commonlines_aux, Rj,candidate_rots,L)
+#             futures.append(f)
+# 
+#     wait(futures)
+# 
+#     for j in range(Nprojs):
+#         c1, c2, m = futures[j].result()   
+#         Ckj2[:,j] = c1
+#         Cjk2[:,j] = c2
+#         Mkj2[:,j] = m
+#     t2 = time.perf_counter()        
+#     logger.info('Computing the common lines is done. Took %5.2f seconds', t2-t1)
+#     assert(np.sum(np.abs(Ckj-Ckj2))==0)
+#     assert(np.sum(np.abs(Cjk-Cjk2))==0)
+#     assert(np.sum(np.abs(Mkj-Mkj2))==0)
+#     
+# =============================================================================
+    # Generate shift grid:
+    # generating a shift grid on the common lines, and choosing the shift
+    # that brings the best correlation in the comparisson between the common 
+    # lines. 
+    # after applying polar FFT on each projection, the shift in quartesian
+    # coordinates- (delta(x),delta(y)) becomes a shift only in the r variable
+    # in the common lines (the common line have a specific theta so we have to
+    # consider a shift only in the r variable.
+    # the equation for the shift phase in the common lines is:
+    # exp((-2*pi*i)*r*delta(r)).
+    max_s = int(np.round(0.2*np.size(projs_hat,0))) # set the maximum shift.
+    s_step = 0.5
+    n_shifts = int((2/s_step)*max_s + 1) # always odd number (to have zero value without shift).
+    max_r = np.size(projs_hat,0)
+    s_vec = np.linspace(-max_s,max_s,n_shifts).reshape((1,n_shifts)) # those are the shifts in the r variable in the common lines. 
+    r_vec = np.arange(max_r).reshape((1,max_r))
+    s_phases = np.exp((-2*math.pi*cmath.sqrt(-1))/(2*max_r+1)*(r_vec.conj().T @ s_vec)) # size of (n_rXn_shift)
+    
+    # Main loop- compute the cross correlation: 
+    # computing the correlation between the common line, first choose the best
+    # shift, and then chose the best rotation.
+    logger.info('Aligning unaligned projections using reference projections')
+    Rots_est = np.zeros((3,3,n_projs))
+    corrs = np.zeros((n_projs,2)) # Statistics on common-lines matching.
+    shifts = np.zeros((2,n_projs))
+    dtheta = 2*math.pi/L
+    if refrot == 1:
+        err_Rots = np.zeros((n_projs,1))
+    if refshift == 1:
+        err_shifts = np.zeros((2,n_projs))
+    for projidx in range(n_projs):
+        cross_corr_m = np.zeros((Nrot,Nprojs))
+        for j in range(Nprojs):
+            iidx = np.array(np.where(Mkj[:,j] != 0)).T
+            conv_hat = (projs_hat[:,Ckj[iidx,j],projidx].conj() * refprojs_hat[:,Cjk[iidx,j],j]).reshape((n_r,np.size(iidx,axis=0))) # size of (n_rxsize(iidx))
+            temp_corr = np.real(s_phases.conj().T @ conv_hat)
+            cross_corr_m[iidx,j] = temp_corr.max(axis=0).reshape(iidx.shape)
+        # calculating the mean of each row in cross_corr_m:
+        cross_corr = (np.sum(cross_corr_m,axis=1)/np.sum(cross_corr_m>0,axis=1)).reshape((Nrot,1))       
+        # Find estimated rotation:
+        bestRscore = np.amax(cross_corr)
+        bestRidx = np.array(np.where(cross_corr == bestRscore))[0,0]
+        meanRscore = np.mean(cross_corr)
+        corrs[projidx,0] = bestRscore
+        corrs[projidx,1] = meanRscore
+        Rots_est[:,:,projidx] = candidate_rots[:,:,bestRidx]       
+        # Error calculation for estimated rotation:
+        if refrot == 1 and G_flag == 1:
+            g_est_t = Rots_est[:,:,projidx] @ trueRots[:,:,projidx].T
+            n_g = np.size(G,0)
+            dist = np.zeros((n_g,1))
+            for g_idx in range(n_g):
+                dist[g_idx,0] = LA.norm(g_est_t-G[g_idx,:,:],'fro')
+            minidx = np.array(np.where(dist == np.amin(dist)))
+            g_est = G[minidx[0,0],:,:]           
+            R_est = g_est.T @ Rots_est[:,:,projidx]
+            R = trueRots[:,:,projidx] @ R_est.T
+            err_Rots[projidx,:] = np.rad2deg(math.acos((np.trace(R)-1)/2))
+        # Error calculation for reflection case:
+        # if there is a reflection between the projection and the volume
+        # then, the relation is R_est=gJRJ.
+        if refrot_J == 1 and G_flag == 1:
+            J3 = np.diag([1, 1, -1])
+            g_est_t = Rots_est[:,:,projidx] @ (J3 @ trueRots_J[:,:,projidx] @ J3).T
+            n_g = np.size(G,0)
+            dist = np.zeros((n_g,1))
+            for g_idx in range(n_g):
+                dist[g_idx,0] = LA.norm(g_est_t-G[g_idx,:,:],'fro')
+            min_idx = np.array(np.where(dist == np.amin(dist)))
+            g_est = G[min_idx[0,0],:,:]    
+            R_est = J3 @ g_est.T @ Rots_est[:,:,projidx] @ J3
+            R = trueRots_J[:,:,projidx] @ R_est.T
+            err_2 = np.rad2deg(math.acos((np.trace(R)-1)/2)) 
+            if err_Rots[projidx,:] != 0:
+                if err_Rots[projidx,:] <= err_2:
+                    err_Rots[projidx,:] = err_Rots[projidx,:]
+                else:
+                    err_Rots[projidx,:] = err_2
+            else:
+                err_Rots[projidx,:] = err_2 
+        
+        # Find estimated shift:
+        # by least-squares on the estimated rotation with the reference projections. 
+        if isshift == 1:
+            idx = np.array(np.where(Mkj[bestRidx,:] == 1)).transpose()
+            n = np.size(idx,0)
+            shift_eq = np.zeros((n,2))
+            shift = np.zeros((n,1))
+            i=0
+            for j in idx:
+                conv_hat = projs_hat[:,Ckj[bestRidx,j],projidx].conj() * refprojs_hat[:,Cjk[bestRidx,j],j] # size of (n_rxsize(iidx))
+                temp_corr = np.real(s_phases.conj().T @ conv_hat) # size of (n_shiftX1). 
+                s_idx = np.array(np.where(temp_corr == temp_corr.max(axis=0)))
+                shift[i,0] = s_vec[s_idx[1,0],s_idx[0,0]]
+                theta = (Ckj[bestRidx,j]-1)*dtheta # Angle of the common line.
+                shift_eq[i,0] = math.sin(theta)
+                shift_eq[i,1] = math.cos(theta)
+                i = i+1
+            shifts[:,projidx] = LA.lstsq(shift_eq,shift)[0].reshape(2)
+            # Error calc for estimated shifts:
+            if refshift != 0:
+                err_shifts[0,projidx] = LA.norm(trueShifts[projidx,0]-shifts[0,projidx],2)
+                err_shifts[1,projidx] = LA.norm(trueShifts[projidx,1]-shifts[1,projidx],2)
+    if refrot == 1 and G_flag == 1:
+        mean_err = np.mean(err_Rots)
+        logger.info('Mean error in estimating the rotations of the projections is: %.3f degrees', mean_err)
+    if isshift == 1 and refshift == 1:
+        mean_err_shift = np.mean(err_shifts)
+        logger.info('Mean error in estimating the translations of the projections is: %.3f', mean_err_shift)
+        
+    logging.shutdown()
+    
+    if refrot != 0 and G_flag != 0 and isshift != 0 and refshift != 0:
+        return Rots_est, shifts, corrs, err_Rots, err_shifts
+    elif refrot != 0 and G_flag != 0 and isshift == 0 and refshift == 0:
+        return Rots_est, shifts, corrs, err_Rots
+    elif refrot == 0 and G_flag == 0 and isshift != 0 and refshift != 0:
+        return Rots_est, shifts, corrs, err_shifts
+    else:
+        return Rots_est, shifts, corrs
+
```

### Comparing `EMalign-1.0.3/src/align_volumes_3d.py` & `EMalign-1.0.4/src/align_volumes_3d.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,615 +1,615 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Sun Feb 28 20:06:16 2021
-
-@author: yaelharpaz1
-"""
-import math
-import logging
-import numpy as np
-from numpy import linalg as LA
-from scipy.optimize import minimize
-from scipy.spatial.transform import Rotation
-from src.common_finufft import cryo_downsample
-from src.cryo_project_itay_finufft import cryo_project
-from src.genRotationsGrid import genRotationsGrid
-from src.align_projection_2d import align_projection
-from src.fastrotate3d import fastrotate3d
-from src.register_translations_3d import register_translations_3d
-from src.register_translations_3d import refine3DshiftBFGS
-from src.reshift_vol import reshift_vol
-import  src.reshift_vol
-from src.SymmetryGroups import genSymGroup
-
-
-def fast_alignment_3d(sym, vol1, vol2, Nprojs=30, trueR=None, G_group=None, refrot=0, verbose=0):
-    '''
-    This function does the work for align_volumes.
-    Input:
-    sym- the symmetry type- 'Cn'\'Dn'\'T'\'O'\'I', where n is the the
-         symmetry order (for example: 'C2').
-    vol1- 3D reference volume that vol2 should be aligned accordingly.
-    vol2- 3D volume to be aligned.
-    verbose- Set verbose to nonzero for verbose printouts (default is zero).
-    Nprojs- number of reference projections for the alignment.
-    trueR- the true rotation matrix between vol2 and vol1.
-    refrot- indicator for true_R. If true_R exist then refrot=1, else
-            refrot=0.
-    G_group- size=(n,3,3) all n symmetry group elemnts.
-
-    output:
-    Rest- the estimated rotation between vol_2 and vol_1 without reflection.
-    Rest_J- the estimated rotation between vol_2 and vol_1 with reflection.
-    '''
-    #logging.basicConfig(level=logging.DEBUG,
-    #                    format='%(asctime)s %(levelname)s %(message)s')
-    logger = logging.getLogger()
-    if verbose == 0:
-        logger.disabled = True
-        
-    # Generate reference projections from vol2:
-    logger.info('Generating %i reference projections.', Nprojs)
-    Rots = genRotationsGrid(75)
-    sz_Rots = np.size(Rots, 2)
-    R_ref = Rots[:, :, np.random.randint(sz_Rots, size=Nprojs)]  # size (3,3,N_projs)
-    # R_ref = mat_to_npy('R_ref_for_fastAlignment3D')
-
-    ref_projs = cryo_project(vol2, R_ref)
-    ref_projs = np.transpose(ref_projs, (1, 0, 2))
-    R_ref = np.transpose(R_ref, (1, 0, 2))  # the true rotations.
-
-    # Align reference projections to vol1:
-    class Struct:
-        '''
-        Used to pass optimal paramters to the alignment function
-        '''
-        pass
-
-    opt = Struct()
-    opt.Nprojs = Nprojs
-    opt.G = G_group
-    opt.Rots = Rots
-    opt.sym = sym
-    logger.info('Aligning reference projections of vol2 to vol1.')
-    if refrot == 1:
-        R = trueR
-        R = R.T
-        R = R[:, [1, 0, 2]][[1, 0, 2]]
-        trueR_tild = np.zeros((3, 3, Nprojs))
-        trueR_tild_J = np.zeros((3, 3, Nprojs))
-        for i in range(Nprojs):
-            trueR_tild[:, :, i] = R @ R_ref[:, :, i]
-            J3 = np.diag([1, 1, -1])
-            trueR_tild_J[:, :, i] = J3 @ R @ J3 @ R_ref[:, :, i]
-        opt.trueRots = trueR_tild
-        opt.trueRots_J = trueR_tild_J
-        R_tild = align_projection(ref_projs, vol1, verbose, opt)  # size=(3,3,N_projs).
-    else:
-        R_tild = align_projection(ref_projs, vol1, verbose, opt)  # size (3,3,N_projs).
-    # Synchronization:
-    # A synchronization algorithm is used In order to revel the symmetry
-    # elements of the reference projections. The relation between the volumes
-    # is V2(r)=V1(Or). Denote the rotation between the volumes as X.
-    # 1. In the case there is no reflection between the volumes, the rotation
-    #    Ri_tilde estimates giORi, therefore the approximation is O =
-    #    gi.'Ri_tildeRi.', where g_i is the symmetry group element of reference
-    #    image i. If we define Xi=Ri*Ri_tilde.' then we get Xi.'*Xj=g_i*g_j.'.
-    # 2. In the case there is a reflection between the volumes, the rotation
-    #    Ri_tilde estimates qiJXRiJ, where O=JX. We have that qiJ=Jqi_tilde,
-    #    therefore the approximation is X=qi_tilde.'JRi_tildeJRi.', where
-    #    qi_tilde is a symmetry element in the symmetry group of
-    #    V1_tilde(r)=V1(Jr). If we define  Xi=Ri*(J*Ri_tild*J).', then we also
-    #    get Xi.'*Xj=qi_tilde*qj_tilde.'.
-    # Therefore, we can construct the synchronization matrix Xij=Xi.'*Xj for
-    # both cases. Then, estimate the group elemnts for each image with and
-    # whitout reflection, and latter choose the option that best describes the
-    # relation between the two volumes.
-
-    # Estimate X with or without reflection:
-    R_tild = R_tild[0]
-    X_mat = np.zeros((3, 3, Nprojs))
-    X_mat_J = np.zeros((3, 3, Nprojs))
-    J3 = np.diag([1, 1, -1])
-    for i in range(Nprojs):
-        X_mat[:, :, i] = R_ref[:, :, i] @ R_tild[:, :, i].T
-        X_mat_J[:, :, i] = R_ref[:, :, i] @ (J3 @ R_tild[:, :, i] @ J3).T
-    # Construct the synchronization matrix with and without reflection:
-    X_ij = np.zeros((3 * Nprojs, 3 * Nprojs))
-    X_ij_J = np.zeros((3 * Nprojs, 3 * Nprojs))
-    for i in range(Nprojs):
-        for j in range(i + 1, Nprojs):
-            X_ij[3 * i:3 * (i + 1), 3 * j:3 * (j + 1)] = X_mat[:, :, i].T @ X_mat[:, :, j]
-            X_ij_J[3 * i:3 * (i + 1), 3 * j:3 * (j + 1)] = X_mat_J[:, :, i].T @ X_mat_J[:, :, j]
-    # Enforce symmetry:
-    X_ij = X_ij + X_ij.T
-    X_ij = X_ij + np.eye(np.size(X_ij, 0))
-    X_ij_J = X_ij_J + X_ij_J.T
-    X_ij_J = X_ij_J + np.eye(np.size(X_ij_J, 0))
-    # Define v=[g_1.',..., g_N_projs.'].' (v is of size 3*N_projx3), then
-    # X_ij=v*v.', and Xij*v=N_projs*v. Thus, v is an eigenvector of Xij. The
-    # matrix Xij should be of rank 3. find the top 3 eigenvectors:
-    # without reflection:
-    s, U = LA.eigh(X_ij)  # s = np.diag(s);
-    ii = np.argsort(s, axis=0)[::-1]  # s = np.sort(s,axis=0)[::-1]
-    U = U[:, ii]
-    V = U[:, 0:3]
-    # With reflection:
-    sJ, UJ = LA.eigh(X_ij_J)  # sJ = np.diag(sJ);
-    iiJ = np.argsort(sJ, axis=0)[::-1]  # sJ = np.sort(sJ,axis=0)[::-1];
-    UJ = UJ[:, iiJ]
-    VJ = UJ[:, 0:3]
-    # estimating G:
-    # Estimate the group elemnts for each reference image. G denotes the
-    # estimated group without reflection, and G_J with reflection. This
-    # estimation is being done from the eigenvector v by using a rounding
-    # algorithm over SO(3) for each 3x3 block of v.
-    G = np.zeros((Nprojs, 3, 3))
-    G_J = np.zeros((Nprojs, 3, 3))
-    for i in range(Nprojs):
-        B = V[3 * i:3 * (i + 1), :]
-        u_tmp, _, v_tmp = LA.svd(B)
-        B_round = LA.det(u_tmp @ v_tmp) * (u_tmp @ v_tmp)
-        G[i, :, :] = B_round.T
-        # reflected case:
-        BJ = VJ[3 * i:3 * (i + 1), :]
-        uJ_tmp, _, vJ_tmp = LA.svd(BJ)
-        BJ_round = LA.det(uJ_tmp @ vJ_tmp) * (uJ_tmp @ vJ_tmp)
-        G_J[i, :, :] = BJ_round.T
-    # Set the global rotation to be an element from the symmetry group:
-    # The global rotation from the synchronization can be any rotation matrix
-    # from SO(3). So, in order to get the estimated symmetry elements to be
-    # from the symmetry group we set the global rotation to be also an element
-    # from the symmetry group.
-    O1 = G[0, :, :].T
-    O1_J = G_J[0, :, :].T
-    G_est = np.zeros((Nprojs, 3, 3))
-    G_J_est = np.zeros((Nprojs, 3, 3))
-    for i in range(Nprojs):
-        G_est[i, :, :] = O1 @ G[i, :, :]
-        G_J_est[i, :, :] = O1_J @ G_J[i, :, :]
-        # Estimating the rotation:
-    # Estimate the two candidate orthogonal transformations.
-    for i in range(Nprojs):
-        X_mat[:, :, i] = X_mat[:, :, i] @ G_est[i, :, :].T
-        X_mat_J[:, :, i] = X_mat_J[:, :, i] @ G_J_est[i, :, :].T
-    X = np.mean(X_mat, axis=2)
-    X_J = np.mean(X_mat_J, axis=2)
-    # Without reflection:
-    R = X
-    U, _, V = LA.svd(R)  # Project R to the nearest rotation.
-    R_est = U @ V
-    assert LA.det(R_est) > 0
-    R_est = R_est[:, [1, 0, 2]][[1, 0, 2]]
-    R_est = R_est.T
-    # reflected case:
-    R_J = X_J
-    U, _, V = LA.svd(R_J)  # Project R to the nearest rotation.
-    R_est_J = U @ V
-    assert LA.det(R_est_J) > 0
-    R_est_J = R_est_J[:, [1, 0, 2]][[1, 0, 2]]
-    R_est_J = R_est_J.T
-
-    logging.shutdown()
-
-    return R_est, R_est_J
-
-
-# %%
-def eval3Dmatchaux(X, vol1, vol2, rotate_fftw_data=None,
-                   reshift_fftw_data=None):
-    psi = X[0]
-    theta = X[1]
-    phi = X[2]
-    dx = X[3]
-    dy = X[4]
-    dz = X[5]
-    r = Rotation.from_euler('xyz', [psi, theta, phi], degrees=False)
-    Rot = r.as_matrix()
-
-    vol2_r = fastrotate3d(vol2, Rot,rotate_fftw_data)
-
-    vol2_rs = reshift_vol(vol2_r, np.array([dx, dy, dz]),reshift_fftw_data)
-    c = np.mean(np.corrcoef(vol1.ravel(), vol2_rs.ravel(), rowvar=False)[0, 1:]).astype('float64')
-    e = (1 - c).astype('float64')
-    return e
-
-
-# %%
-def refine3DmatchBFGS(vol1, vol2, R1, estdx):
-    # Create initial guess vector
-    R1 = Rotation.from_matrix(R1)
-    [psi, theta, phi] = R1.as_euler('xyz')
-    X0 = np.array([psi, theta, phi, estdx[0], estdx[1], estdx[2]]).astype('float64')
-    rotate_fftw_data = src.fastrotate3d.fftw_data_class(vol1)
-    reshift_fftw_data = src.reshift_vol.fftw_data_class(vol1)
-    # BFGS optimization:
-    res = minimize(eval3Dmatchaux, X0, args=(vol1, vol2, rotate_fftw_data,
-                reshift_fftw_data), method='BFGS', tol=1e-3,
-                options={'gtol': 1e-1, 'disp': False})
-    X = res.x
-    psi = X[0]
-    theta = X[1]
-    phi = X[2]
-    Rest = Rotation.from_euler('xyz', [psi, theta, phi], degrees=False)
-    estdx = np.array([X[3], X[4], X[5]])
-    return Rest
-
-
-# %%
-def evalO(X, R_true, R_est, G):
-    psi = X[0]
-    theta = X[1]
-    phi = X[2]
-    O = Rotation.as_matrix(Rotation.from_euler('xyz', [psi, theta, phi], degrees=False))
-    n = np.size(G, 0)
-    dist = np.zeros((1, n))
-    for i in range(n):
-        g = G[i, :, :]
-        dist[0, i] = LA.norm(R_true - O @ g @ O.T @ R_est, 'fro')
-    err = np.min(dist)
-    return err
-
-
-# %%
-def align_volumes(vol1, vol2, verbose=0, opt=None):
-    '''
-    This function aligns vol2 according to vol1
-    Aligning vol2 to vol1 by finding the relative rotation, translation and
-    reflection between vol1 and vol2, such that vol2 is best aligned with
-    vol1.
-    How to align the two volumes:
-        The user should align vol2 according to vol1 using the parameters bestR,
-        bestdx and reflect. If reflect=0 then there is no reflection between the
-        volumes. In that case the user should first rotate vol2 by bestR and then
-        reshift by bestdx. If reflect=1, then there is a reflection between the
-        volumes. In that case the user should first reflcet vol2 about the z axis
-        using the flip function, then rotate the volume by bestR and finally
-        reshift by bestdx.
-    Input:
-        vol1- 3D reference volume that vol2 should be aligned accordingly.
-        vol2- 3D volume to be aligned.
-        verbose- Set verbose to nonzero for verbose printouts (default is zero).
-    Output:
-        bestR- the estimated rotation between vol2 and vol1, such that bestR*vol2
-               will align vol2 to vol1.
-        bestdx- size=3x1. the estimated translation between vol2 and vol1.
-        reflect- indicator for reflection. If reflect=1 then there is a
-                 reflection between vol1 and vol2, else reflect=0. In order to
-                 align the volumes in the case of reflect=1, the user should
-                 first reflect vol2 about the z axis, and then rotate by bestR.
-        vol2aligned- vol2 after applyng the estimated transformation, so it is
-                     best aligned with vol1 (after optimization).
-        bestcorr- the coorelation between vol1 and vol2aligned.
-    Options:
-        sym- the symmetry type- 'Cn'\'Dn'\'T'\'O'\'I', where n is the the
-             symmetry order (for example: 'C2'). This input is required only for
-             the error calculation.
-        opt.downsample-  Downsample the volume to this size (in pixels) for
-                         faster alignment. Default is 48. Use larger value if
-                         alignment fails.
-        opt.Nprojs- Number of projections to use for the alignment.
-                     Defult is 30.
-        opt.trueR-  True rotation matrix between vol2 and vol1, such that
-                vol2 = fastrotate3d(vol1,true_R). In the case of reflection,
-                true_R should be the rotation between the volumes such that
-                vol2 = flip(fastrotate3d(vol1,true_R),3). In this case
-                O = J*true_R, where J is the reflection matrix over the z axis
-                J=diag([1,1,-1]). This input is used for debugging to calculate
-                errors.
-        opt.G- Array of matrices of size 3x3xn containing the symmetry group
-               elemnts of vol1. This input is for accurate error calculation. If
-               G is not submitted then the error will be calculated by
-               optimization over the symmetry group.
-    '''
-
-    logger = logging.getLogger()
-
-    if verbose is False:
-        logger.disabled = True
-    else:
-        logger.disabled = False
-
-    class Struct:
-        pass
-
-
-    ### Check options:
-    if opt is None:
-        opt = Struct()
-        opt.no_refine = False
-
-    if not hasattr(opt, 'no_refine'):
-        opt.no_refine = False
-
-    ### Check options:
-    if hasattr(opt, 'sym'):
-        sym = opt.sym
-    else:
-        sym = None
-
-    if hasattr(opt, 'Nprojs'):
-        Nprojs = opt.Nprojs
-    else:
-        Nprojs = 30
-
-    if hasattr(opt, 'G'):
-        G = opt.G
-    else:
-        G = None
-
-    if hasattr(opt, 'trueR'):
-        trueR = opt.trueR
-    else:
-        trueR = None
-
-    if hasattr(opt, 'downsample'):
-        downsample = opt.downsample
-    else:
-        downsample = 64
-
-    ### Define parameters:
-    sym_flag = 0
-    G_flag = 0
-    if sym is not None:
-        s = sym[0]
-        n_s = 0
-        if len(sym) > 1:
-            n_s = int(sym[1:len(sym)])
-        sym_flag = 1
-        if s == 'C' and n_s == 1:
-            G = np.eye(3).reshape((1, 3, 3))
-    if G is not None:
-        G_flag = 1
-    refrot = 1
-    if trueR is None:
-        refrot = 0
-
-    # Validate input:
-    # Input volumes must be 3-dimensional, where all dimensions must be equal.
-    # This restriction can be remove, but then, the calculation of nr (radial
-    # resolution in the Fourier domain) should be adjusted accordingly. Both
-    # vol_1 and vol_2 must have the same dimensions.
-    n_1 = np.shape(vol1)
-    assert np.size(n_1) == 3, "Inputs must be 3D"
-    assert n_1[0] == n_1[1], "All dimensions of input volumes must be equal"
-    n_2 = np.shape(vol2)
-    assert np.size(n_2) == 3, "Inputs must be 3D"
-    assert n_2[0] == n_1[1] and n_2[0] == n_1[1], "All dimensions of input volumes must be equal"
-    assert n_1[0] == n_2[0], "Input volumes have different dimensions"
-    n = n_1[0]
-    n_ds = min(n, downsample)  # Perform aligment on down sampled volumes.
-    # This speeds up calculation, and does not seem
-    # to degrade accuracy
-
-    if n_ds < n:
-        logger.info('Downsampling volumes from %i to %i pixels', n, n_ds)
-        vol1_ds = cryo_downsample(vol1, (n_ds, n_ds, n_ds))
-        vol2_ds = cryo_downsample(vol2, (n_ds, n_ds, n_ds))
-    else:
-        logger.info('No need for downsampling. n=%i n_ds=%i', n, n_ds)
-        vol1_ds = vol1
-        vol2_ds = vol2
-
-    # Aligning the volumes:
-    if G_flag == 1:
-        G_c = np.copy(G)
-    else:
-        G_c = None
-    R_est, R_est_J = fast_alignment_3d(sym, vol1_ds.copy(), vol2_ds.copy(),
-                                     Nprojs, trueR, G_c, refrot, verbose)
-
-    logger.debug("R_est=\n%s",str(R_est))
-    logger.debug("R_est_J=\n%s",str(R_est_J))
-
-    vol2_aligned_ds = fastrotate3d(vol2_ds, R_est)  # Rotate the original vol_2 back.
-    vol2_aligned_J_ds = fastrotate3d(vol2_ds, R_est_J)
-
-    vol2_aligned_J_ds = np.flip(vol2_aligned_J_ds, axis=2)
-    estdx_ds = register_translations_3d(vol1_ds, vol2_aligned_ds)
-    estdx_J_ds = register_translations_3d(vol1_ds, vol2_aligned_J_ds)
-    logger.debug("estdx_ds=%s",str(estdx_ds))
-    logger.debug("estdx_J_ds=%s",str(estdx_J_ds))
-
-    if np.size(estdx_ds) != 3 or np.size(estdx_J_ds) != 3:
-        raise Warning("***** Translation estimation failed *****")
-
-    # Prepare FFTW data to avoid unnecessary calaculations        
-    vol2_aligned_ds = src.reshift_vol.reshift_vol_int(vol2_aligned_ds, estdx_ds)
-    vol2_aligned_J_ds = src.reshift_vol.reshift_vol_int(vol2_aligned_J_ds, estdx_J_ds)
-    
-    no1 = np.mean(np.corrcoef(vol1_ds.ravel(), vol2_aligned_ds.ravel(), rowvar=False)[0, 1:])
-    no2 = np.mean(np.corrcoef(vol1_ds.ravel(), vol2_aligned_J_ds.ravel(), rowvar=False)[0, 1:])
-    logger.debug("no1=%f",no1)
-    logger.debug("no2=%f",no2)
-
-    # if max(no1, no2) < 0.1:  # The coorelations of the estimated rotations are
-    #     # smaller than 0.1, that is, no transformation was recovered.
-    #     raise Warning("***** Alignment failed *****")
-    # Do we have reflection?
-    reflect = 0
-    corr_v = no1
-    if no2 > no1:
-        J3 = np.diag([1, 1, -1])
-        corr_v = no2
-        R_est = R_est_J
-        R_est = J3 @ R_est @ J3
-        estdx_ds = estdx_J_ds
-        vol2_ds = np.flip(vol2_ds, axis=2)
-        vol2 = np.flip(vol2, axis=2)
-        reflect = 1
-        logger.info('Input volumes are reflected w.r.t each other')
-    logger.info('Correlation between downsampled aligned volumes '\
-                'before optimization is %.4f', corr_v)
-
-    logger.debug("R_est=\n%s",str(R_est))
-    logger.debug("estdx_ds=%s",str(estdx_ds))
-    logger.debug("reflect=%d", reflect)
-
-    if opt.no_refine:
-        logger.info('Skipping refinement of alignment parameters')
-        bestR = R_est
-    else:
-        logger.info('Using BFGS algorithm to refine alignment parameters')
-        # Optimization:
-        # We use the BFGS optimization algorithm in order to refine the resulted
-        # transformation between the two volumes.
-        bestR = refine3DmatchBFGS(vol1_ds.copy(), vol2_ds.copy(), R_est, estdx_ds)
-        bestR = Rotation.as_matrix(bestR)
-
-    logger.debug("bestR=\n%s",str(bestR))
-    logger.info('Done aligning downsampled volumes')
-    logger.info('Applying estimated rotation to original volumes')
-    vol2aligned = fastrotate3d(vol2, bestR)
-    logger.info('Estimating shift for original volumes')
-    bestdx = register_translations_3d(vol1, vol2aligned)
-    logger.debug("bestdx=%s",str(bestdx))
-    # if np.size(bestdx) != 3 :
-    #    raise Warning("***** Translation estimation failed *****")
-
-    if not opt.no_refine:
-        logger.info('Refining shift for original volumes')
-        bestdx = refine3DshiftBFGS(vol1, vol2, bestdx)
-        logger.debug("bestdx=%s",str(bestdx))
-    else:
-        logger.info('Skipping shift refinement')
-
-    logger.info('Translating original volumes')
-    if (np.round(bestdx) == bestdx).all():
-        # Use fast method
-        vol2aligned = src.reshift_vol.reshift_vol_int(vol2aligned, bestdx)
-    else:
-        vol2aligned = reshift_vol(vol2aligned, bestdx)
-
-    logger.info('Computing correlations of original volumes')
-    bestcorr = np.mean(np.corrcoef(vol1.ravel(), vol2aligned.ravel(), rowvar=False)[0, 1:])
-
-    logger.info('Estimated rotation:\n%s',str(bestR))
-    logger.info('Estimated translations: [%.3f, %.3f, %.3f]', bestdx[0], bestdx[1], bestdx[2])
-    logger.info('Correlation between original aligned volumes is %.4f', bestcorr)
-    # Accurate error calculation:
-    # The difference between the estimated and reference rotation should be an
-    # element from the symmetry group:
-    if refrot == 1 and G_flag == 1:
-        n_g = np.size(G, 0)
-        g_est_t = trueR.T @ bestR.T
-        dist = np.zeros((n_g))
-        for g_idx in range(n_g):
-            dist[g_idx] = LA.norm(g_est_t - G[g_idx, :, :], ord='fro')
-        min_idx = np.argmin(dist)
-        g_est = G[min_idx, :, :]
-        err_norm = LA.norm(trueR.T - (g_est @ bestR), ord='fro')
-        ref_true_R = trueR.T
-        logger.info('Reference rotation:')
-        logger.info('%.4f %.4f %.4f', ref_true_R[0, 0], ref_true_R[0, 1], ref_true_R[0, 2])
-        logger.info('%.4f %.4f %.4f', ref_true_R[1, 0], ref_true_R[1, 1], ref_true_R[1, 2])
-        logger.info('%.4f %.4f %.4f', ref_true_R[2, 0], ref_true_R[2, 1], ref_true_R[2, 2])
-        aligned_bestR = g_est @ bestR
-        logger.info('Estimated rotation (aligned by a symmetry element '\
-                    'according to the reference rotation):')
-        logger.info('%.4f %.4f %.4f', aligned_bestR[0, 0], aligned_bestR[0, 1], aligned_bestR[0, 2])
-        logger.info('%.4f %.4f %.4f', aligned_bestR[1, 0], aligned_bestR[1, 1], aligned_bestR[1, 2])
-        logger.info('%.4f %.4f %.4f', aligned_bestR[2, 0], aligned_bestR[2, 1], aligned_bestR[2, 2])
-        logger.info('Estimated symmetry element:')
-        logger.info('%.4f %.4f %.4f', g_est[0, 0], g_est[0, 1], g_est[0, 2])
-        logger.info('%.4f %.4f %.4f', g_est[1, 0], g_est[1, 1], g_est[1, 2])
-        logger.info('%.4f %.4f %.4f', g_est[2, 0], g_est[2, 1], g_est[2, 2])
-        logger.info('Estimation error (Frobenius norm) up to symmetry '\
-                    'group element is %.4f', err_norm)
-        vec_ref = Rotation.as_rotvec(Rotation.from_matrix(trueR.T))
-        angle_ref = LA.norm(vec_ref)
-        axis_ref = vec_ref / angle_ref
-        vec_est = Rotation.as_rotvec(Rotation.from_matrix(g_est @ bestR))
-        angle_est = LA.norm(vec_est)
-        axis_est = vec_est / angle_est
-        logger.info('Rotation axis:')
-        logger.info('Reference [ %.4f, %.4f, %.4f]', axis_ref[0], axis_ref[1], axis_ref[2])
-        logger.info('Estimated [ %.4f, %.4f, %.4f]', axis_est[0], axis_est[1], axis_est[2])
-        logger.info('Angle between axes is %.4f  degrees',
-                    math.degrees(np.arccos(np.dot(axis_est, axis_ref))))
-        logger.info('In-plane rotation:')
-        logger.info('Reference %.4f degrees', math.degrees(angle_ref))
-        logger.info('Estimated %.4f degrees', math.degrees(angle_est))
-        logger.info('Angle difference is %.4f degrees',
-                    abs(math.degrees(angle_ref) - math.degrees(angle_est)))
-    # Error calculation by optimization:
-    # The difference between the estimated and reference rotation should be an
-    # element from the symmetry group. In the case the symmetry group of vol1
-    # is not given, it can be estimated using optimization process.
-    # Let G be the symmetry group of the symmetry type of the molecule in the
-    # canonical coordinate system (G is obtained using genSymgroup). Then, the
-    # symmetry group of vol1 is given by O*G*O.', where O is the orthogonal
-    # transformation between the coordinate system of vol1 and the canonical
-    # one. Therefore, the symmetry group can be estimated by evaluating O using
-    # optimization algorithm.
-    if refrot == 1 and G_flag == 0 and sym_flag == 1:
-        # Creating initial guess by brute-force algorithm:
-        G = genSymGroup(sym)
-        n_g = np.size(G, 0)
-        Rots = genRotationsGrid(75)
-        n = np.size(Rots, 2)
-        dist = np.zeros((n, n_g))
-        for i in range(n):
-            for j in range(n_g):
-                O = Rots[:, :, i]
-                g = G[j, :, :]
-                dist[i, j] = LA.norm(trueR.T - (O @ g @ O.T @ bestR), ord='fro')
-        err = np.min(dist.ravel())
-        row = np.array(np.where(dist == err))[0]
-        O = Rots[:, :, row[0]]
-        # BFGS optimization:
-        [psi, theta, phi] = (Rotation.from_matrix(O)).as_euler('xyz')
-        X0 = np.array([psi, theta, phi]).astype('float64')
-        res = minimize(evalO, X0, args=(trueR.T, bestR, G), method='BFGS', tol=1e-4,
-                       options={'gtol': 1e-4, 'disp': False})
-        X = res.x
-        psi = X[0]
-        theta = X[1]
-        phi = X[2]
-        O = Rotation.as_matrix(Rotation.from_euler('xyz', [psi, theta, phi], degrees=False))
-        n_g = np.size(G, 0)
-        dist = np.zeros((1, n_g))
-        for i in range(n_g):
-            g = G[i, :, :]
-            dist[0, i] = LA.norm(trueR.T - (O @ g @ O.T @ bestR), 'fro')
-        err_norm = np.min(dist)
-        idx = np.array(np.where(dist == err_norm))
-        g = G[idx[1, 0], :, :]
-        g_est = O @ g @ O.T
-        ref_true_R = trueR.T
-        logger.info('Reference rotation:')
-        logger.info('%.4f %.4f %.4f', ref_true_R[0, 0], ref_true_R[0, 1], ref_true_R[0, 2])
-        logger.info('%.4f %.4f %.4f', ref_true_R[1, 0], ref_true_R[1, 1], ref_true_R[1, 2])
-        logger.info('%.4f %.4f %.4f', ref_true_R[2, 0], ref_true_R[2, 1], ref_true_R[2, 2])
-        aligned_bestR = g_est @ bestR
-        logger.info('Estimated rotation (aligned by a symmetry element '\
-                    'according to the reference rotation):')
-        logger.info('%.4f %.4f %.4f', aligned_bestR[0, 0], aligned_bestR[0, 1], aligned_bestR[0, 2])
-        logger.info('%.4f %.4f %.4f', aligned_bestR[1, 0], aligned_bestR[1, 1], aligned_bestR[1, 2])
-        logger.info('%.4f %.4f %.4f', aligned_bestR[2, 0], aligned_bestR[2, 1], aligned_bestR[2, 2])
-        logger.info('Estimated symmetry element:')
-        logger.info('%.4f %.4f %.4f', g_est[0, 0], g_est[0, 1], g_est[0, 2])
-        logger.info('%.4f %.4f %.4f', g_est[1, 0], g_est[1, 1], g_est[1, 2])
-        logger.info('%.4f %.4f %.4f', g_est[2, 0], g_est[2, 1], g_est[2, 2])
-        logger.info('Estimation error (Frobenius norm) up to symmetry '\
-                    'group element is %.4f', err_norm)
-        vec_ref = Rotation.as_rotvec(Rotation.from_matrix(trueR.T))
-        angle_ref = LA.norm(vec_ref)
-        axis_ref = vec_ref / angle_ref
-        vec_est = Rotation.as_rotvec(Rotation.from_matrix(g_est @ bestR))
-        angle_est = LA.norm(vec_est)
-        axis_est = vec_est / angle_est
-        logger.info('Rotation axis:')
-        logger.info('Reference [ %.4f, %.4f, %.4f]', axis_ref[0], axis_ref[1], axis_ref[2])
-        logger.info('Estimated [ %.4f, %.4f, %.4f]', axis_est[0], axis_est[1], axis_est[2])
-        logger.info('Angle between axes is %.4f  degrees',
-                    math.degrees(np.arccos(np.dot(axis_est, axis_ref))))
-        logger.info('In-plane rotation:')
-        logger.info('Reference %.4f degrees', math.degrees(angle_ref))
-        logger.info('Estimated %.4f degrees', math.degrees(angle_est))
-        logger.info('Angle difference is %.4f degrees',
-                    abs(math.degrees(angle_ref) - math.degrees(angle_est)))
-
-    logging.shutdown()
-
-    return bestR, bestdx, reflect, vol2aligned, bestcorr
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Sun Feb 28 20:06:16 2021
+
+@author: yaelharpaz1
+"""
+import math
+import logging
+import numpy as np
+from numpy import linalg as LA
+from scipy.optimize import minimize
+from scipy.spatial.transform import Rotation
+from src.common_finufft import cryo_downsample
+from src.cryo_project_itay_finufft import cryo_project
+from src.genRotationsGrid import genRotationsGrid
+from src.align_projection_2d import align_projection
+from src.fastrotate3d import fastrotate3d
+from src.register_translations_3d import register_translations_3d
+from src.register_translations_3d import refine3DshiftBFGS
+from src.reshift_vol import reshift_vol
+import  src.reshift_vol
+from src.SymmetryGroups import genSymGroup
+
+
+def fast_alignment_3d(sym, vol1, vol2, Nprojs=30, trueR=None, G_group=None, refrot=0, verbose=0):
+    '''
+    This function does the work for align_volumes.
+    Input:
+    sym- the symmetry type- 'Cn'\'Dn'\'T'\'O'\'I', where n is the the
+         symmetry order (for example: 'C2').
+    vol1- 3D reference volume that vol2 should be aligned accordingly.
+    vol2- 3D volume to be aligned.
+    verbose- Set verbose to nonzero for verbose printouts (default is zero).
+    Nprojs- number of reference projections for the alignment.
+    trueR- the true rotation matrix between vol2 and vol1.
+    refrot- indicator for true_R. If true_R exist then refrot=1, else
+            refrot=0.
+    G_group- size=(n,3,3) all n symmetry group elemnts.
+
+    output:
+    Rest- the estimated rotation between vol_2 and vol_1 without reflection.
+    Rest_J- the estimated rotation between vol_2 and vol_1 with reflection.
+    '''
+    #logging.basicConfig(level=logging.DEBUG,
+    #                    format='%(asctime)s %(levelname)s %(message)s')
+    logger = logging.getLogger()
+    if verbose == 0:
+        logger.disabled = True
+        
+    # Generate reference projections from vol2:
+    logger.info('Generating %i reference projections.', Nprojs)
+    Rots = genRotationsGrid(75)
+    sz_Rots = np.size(Rots, 2)
+    R_ref = Rots[:, :, np.random.randint(sz_Rots, size=Nprojs)]  # size (3,3,N_projs)
+    # R_ref = mat_to_npy('R_ref_for_fastAlignment3D')
+
+    ref_projs = cryo_project(vol2, R_ref)
+    ref_projs = np.transpose(ref_projs, (1, 0, 2))
+    R_ref = np.transpose(R_ref, (1, 0, 2))  # the true rotations.
+
+    # Align reference projections to vol1:
+    class Struct:
+        '''
+        Used to pass optimal paramters to the alignment function
+        '''
+        pass
+
+    opt = Struct()
+    opt.Nprojs = Nprojs
+    opt.G = G_group
+    opt.Rots = Rots
+    opt.sym = sym
+    logger.info('Aligning reference projections of vol2 to vol1.')
+    if refrot == 1:
+        R = trueR
+        R = R.T
+        R = R[:, [1, 0, 2]][[1, 0, 2]]
+        trueR_tild = np.zeros((3, 3, Nprojs))
+        trueR_tild_J = np.zeros((3, 3, Nprojs))
+        for i in range(Nprojs):
+            trueR_tild[:, :, i] = R @ R_ref[:, :, i]
+            J3 = np.diag([1, 1, -1])
+            trueR_tild_J[:, :, i] = J3 @ R @ J3 @ R_ref[:, :, i]
+        opt.trueRots = trueR_tild
+        opt.trueRots_J = trueR_tild_J
+        R_tild = align_projection(ref_projs, vol1, verbose, opt)  # size=(3,3,N_projs).
+    else:
+        R_tild = align_projection(ref_projs, vol1, verbose, opt)  # size (3,3,N_projs).
+    # Synchronization:
+    # A synchronization algorithm is used In order to revel the symmetry
+    # elements of the reference projections. The relation between the volumes
+    # is V2(r)=V1(Or). Denote the rotation between the volumes as X.
+    # 1. In the case there is no reflection between the volumes, the rotation
+    #    Ri_tilde estimates giORi, therefore the approximation is O =
+    #    gi.'Ri_tildeRi.', where g_i is the symmetry group element of reference
+    #    image i. If we define Xi=Ri*Ri_tilde.' then we get Xi.'*Xj=g_i*g_j.'.
+    # 2. In the case there is a reflection between the volumes, the rotation
+    #    Ri_tilde estimates qiJXRiJ, where O=JX. We have that qiJ=Jqi_tilde,
+    #    therefore the approximation is X=qi_tilde.'JRi_tildeJRi.', where
+    #    qi_tilde is a symmetry element in the symmetry group of
+    #    V1_tilde(r)=V1(Jr). If we define  Xi=Ri*(J*Ri_tild*J).', then we also
+    #    get Xi.'*Xj=qi_tilde*qj_tilde.'.
+    # Therefore, we can construct the synchronization matrix Xij=Xi.'*Xj for
+    # both cases. Then, estimate the group elemnts for each image with and
+    # whitout reflection, and latter choose the option that best describes the
+    # relation between the two volumes.
+
+    # Estimate X with or without reflection:
+    R_tild = R_tild[0]
+    X_mat = np.zeros((3, 3, Nprojs))
+    X_mat_J = np.zeros((3, 3, Nprojs))
+    J3 = np.diag([1, 1, -1])
+    for i in range(Nprojs):
+        X_mat[:, :, i] = R_ref[:, :, i] @ R_tild[:, :, i].T
+        X_mat_J[:, :, i] = R_ref[:, :, i] @ (J3 @ R_tild[:, :, i] @ J3).T
+    # Construct the synchronization matrix with and without reflection:
+    X_ij = np.zeros((3 * Nprojs, 3 * Nprojs))
+    X_ij_J = np.zeros((3 * Nprojs, 3 * Nprojs))
+    for i in range(Nprojs):
+        for j in range(i + 1, Nprojs):
+            X_ij[3 * i:3 * (i + 1), 3 * j:3 * (j + 1)] = X_mat[:, :, i].T @ X_mat[:, :, j]
+            X_ij_J[3 * i:3 * (i + 1), 3 * j:3 * (j + 1)] = X_mat_J[:, :, i].T @ X_mat_J[:, :, j]
+    # Enforce symmetry:
+    X_ij = X_ij + X_ij.T
+    X_ij = X_ij + np.eye(np.size(X_ij, 0))
+    X_ij_J = X_ij_J + X_ij_J.T
+    X_ij_J = X_ij_J + np.eye(np.size(X_ij_J, 0))
+    # Define v=[g_1.',..., g_N_projs.'].' (v is of size 3*N_projx3), then
+    # X_ij=v*v.', and Xij*v=N_projs*v. Thus, v is an eigenvector of Xij. The
+    # matrix Xij should be of rank 3. find the top 3 eigenvectors:
+    # without reflection:
+    s, U = LA.eigh(X_ij)  # s = np.diag(s);
+    ii = np.argsort(s, axis=0)[::-1]  # s = np.sort(s,axis=0)[::-1]
+    U = U[:, ii]
+    V = U[:, 0:3]
+    # With reflection:
+    sJ, UJ = LA.eigh(X_ij_J)  # sJ = np.diag(sJ);
+    iiJ = np.argsort(sJ, axis=0)[::-1]  # sJ = np.sort(sJ,axis=0)[::-1];
+    UJ = UJ[:, iiJ]
+    VJ = UJ[:, 0:3]
+    # estimating G:
+    # Estimate the group elemnts for each reference image. G denotes the
+    # estimated group without reflection, and G_J with reflection. This
+    # estimation is being done from the eigenvector v by using a rounding
+    # algorithm over SO(3) for each 3x3 block of v.
+    G = np.zeros((Nprojs, 3, 3))
+    G_J = np.zeros((Nprojs, 3, 3))
+    for i in range(Nprojs):
+        B = V[3 * i:3 * (i + 1), :]
+        u_tmp, _, v_tmp = LA.svd(B)
+        B_round = LA.det(u_tmp @ v_tmp) * (u_tmp @ v_tmp)
+        G[i, :, :] = B_round.T
+        # reflected case:
+        BJ = VJ[3 * i:3 * (i + 1), :]
+        uJ_tmp, _, vJ_tmp = LA.svd(BJ)
+        BJ_round = LA.det(uJ_tmp @ vJ_tmp) * (uJ_tmp @ vJ_tmp)
+        G_J[i, :, :] = BJ_round.T
+    # Set the global rotation to be an element from the symmetry group:
+    # The global rotation from the synchronization can be any rotation matrix
+    # from SO(3). So, in order to get the estimated symmetry elements to be
+    # from the symmetry group we set the global rotation to be also an element
+    # from the symmetry group.
+    O1 = G[0, :, :].T
+    O1_J = G_J[0, :, :].T
+    G_est = np.zeros((Nprojs, 3, 3))
+    G_J_est = np.zeros((Nprojs, 3, 3))
+    for i in range(Nprojs):
+        G_est[i, :, :] = O1 @ G[i, :, :]
+        G_J_est[i, :, :] = O1_J @ G_J[i, :, :]
+        # Estimating the rotation:
+    # Estimate the two candidate orthogonal transformations.
+    for i in range(Nprojs):
+        X_mat[:, :, i] = X_mat[:, :, i] @ G_est[i, :, :].T
+        X_mat_J[:, :, i] = X_mat_J[:, :, i] @ G_J_est[i, :, :].T
+    X = np.mean(X_mat, axis=2)
+    X_J = np.mean(X_mat_J, axis=2)
+    # Without reflection:
+    R = X
+    U, _, V = LA.svd(R)  # Project R to the nearest rotation.
+    R_est = U @ V
+    assert LA.det(R_est) > 0
+    R_est = R_est[:, [1, 0, 2]][[1, 0, 2]]
+    R_est = R_est.T
+    # reflected case:
+    R_J = X_J
+    U, _, V = LA.svd(R_J)  # Project R to the nearest rotation.
+    R_est_J = U @ V
+    assert LA.det(R_est_J) > 0
+    R_est_J = R_est_J[:, [1, 0, 2]][[1, 0, 2]]
+    R_est_J = R_est_J.T
+
+    logging.shutdown()
+
+    return R_est, R_est_J
+
+
+# %%
+def eval3Dmatchaux(X, vol1, vol2, rotate_fftw_data=None,
+                   reshift_fftw_data=None):
+    psi = X[0]
+    theta = X[1]
+    phi = X[2]
+    dx = X[3]
+    dy = X[4]
+    dz = X[5]
+    r = Rotation.from_euler('xyz', [psi, theta, phi], degrees=False)
+    Rot = r.as_matrix()
+
+    vol2_r = fastrotate3d(vol2, Rot,rotate_fftw_data)
+
+    vol2_rs = reshift_vol(vol2_r, np.array([dx, dy, dz]),reshift_fftw_data)
+    c = np.mean(np.corrcoef(vol1.ravel(), vol2_rs.ravel(), rowvar=False)[0, 1:]).astype('float64')
+    e = (1 - c).astype('float64')
+    return e
+
+
+# %%
+def refine3DmatchBFGS(vol1, vol2, R1, estdx):
+    # Create initial guess vector
+    R1 = Rotation.from_matrix(R1)
+    [psi, theta, phi] = R1.as_euler('xyz')
+    X0 = np.array([psi, theta, phi, estdx[0], estdx[1], estdx[2]]).astype('float64')
+    rotate_fftw_data = src.fastrotate3d.fftw_data_class(vol1)
+    reshift_fftw_data = src.reshift_vol.fftw_data_class(vol1)
+    # BFGS optimization:
+    res = minimize(eval3Dmatchaux, X0, args=(vol1, vol2, rotate_fftw_data,
+                reshift_fftw_data), method='BFGS', tol=1e-3,
+                options={'gtol': 1e-1, 'disp': False})
+    X = res.x
+    psi = X[0]
+    theta = X[1]
+    phi = X[2]
+    Rest = Rotation.from_euler('xyz', [psi, theta, phi], degrees=False)
+    estdx = np.array([X[3], X[4], X[5]])
+    return Rest
+
+
+# %%
+def evalO(X, R_true, R_est, G):
+    psi = X[0]
+    theta = X[1]
+    phi = X[2]
+    O = Rotation.as_matrix(Rotation.from_euler('xyz', [psi, theta, phi], degrees=False))
+    n = np.size(G, 0)
+    dist = np.zeros((1, n))
+    for i in range(n):
+        g = G[i, :, :]
+        dist[0, i] = LA.norm(R_true - O @ g @ O.T @ R_est, 'fro')
+    err = np.min(dist)
+    return err
+
+
+# %%
+def align_volumes(vol1, vol2, verbose=0, opt=None):
+    '''
+    This function aligns vol2 according to vol1
+    Aligning vol2 to vol1 by finding the relative rotation, translation and
+    reflection between vol1 and vol2, such that vol2 is best aligned with
+    vol1.
+    How to align the two volumes:
+        The user should align vol2 according to vol1 using the parameters bestR,
+        bestdx and reflect. If reflect=0 then there is no reflection between the
+        volumes. In that case the user should first rotate vol2 by bestR and then
+        reshift by bestdx. If reflect=1, then there is a reflection between the
+        volumes. In that case the user should first reflcet vol2 about the z axis
+        using the flip function, then rotate the volume by bestR and finally
+        reshift by bestdx.
+    Input:
+        vol1- 3D reference volume that vol2 should be aligned accordingly.
+        vol2- 3D volume to be aligned.
+        verbose- Set verbose to nonzero for verbose printouts (default is zero).
+    Output:
+        bestR- the estimated rotation between vol2 and vol1, such that bestR*vol2
+               will align vol2 to vol1.
+        bestdx- size=3x1. the estimated translation between vol2 and vol1.
+        reflect- indicator for reflection. If reflect=1 then there is a
+                 reflection between vol1 and vol2, else reflect=0. In order to
+                 align the volumes in the case of reflect=1, the user should
+                 first reflect vol2 about the z axis, and then rotate by bestR.
+        vol2aligned- vol2 after applyng the estimated transformation, so it is
+                     best aligned with vol1 (after optimization).
+        bestcorr- the coorelation between vol1 and vol2aligned.
+    Options:
+        sym- the symmetry type- 'Cn'\'Dn'\'T'\'O'\'I', where n is the the
+             symmetry order (for example: 'C2'). This input is required only for
+             the error calculation.
+        opt.downsample-  Downsample the volume to this size (in pixels) for
+                         faster alignment. Default is 48. Use larger value if
+                         alignment fails.
+        opt.Nprojs- Number of projections to use for the alignment.
+                     Defult is 30.
+        opt.trueR-  True rotation matrix between vol2 and vol1, such that
+                vol2 = fastrotate3d(vol1,true_R). In the case of reflection,
+                true_R should be the rotation between the volumes such that
+                vol2 = flip(fastrotate3d(vol1,true_R),3). In this case
+                O = J*true_R, where J is the reflection matrix over the z axis
+                J=diag([1,1,-1]). This input is used for debugging to calculate
+                errors.
+        opt.G- Array of matrices of size 3x3xn containing the symmetry group
+               elemnts of vol1. This input is for accurate error calculation. If
+               G is not submitted then the error will be calculated by
+               optimization over the symmetry group.
+    '''
+
+    logger = logging.getLogger()
+
+    if verbose is False:
+        logger.disabled = True
+    else:
+        logger.disabled = False
+
+    class Struct:
+        pass
+
+
+    ### Check options:
+    if opt is None:
+        opt = Struct()
+        opt.no_refine = False
+
+    if not hasattr(opt, 'no_refine'):
+        opt.no_refine = False
+
+    ### Check options:
+    if hasattr(opt, 'sym'):
+        sym = opt.sym
+    else:
+        sym = None
+
+    if hasattr(opt, 'Nprojs'):
+        Nprojs = opt.Nprojs
+    else:
+        Nprojs = 30
+
+    if hasattr(opt, 'G'):
+        G = opt.G
+    else:
+        G = None
+
+    if hasattr(opt, 'trueR'):
+        trueR = opt.trueR
+    else:
+        trueR = None
+
+    if hasattr(opt, 'downsample'):
+        downsample = opt.downsample
+    else:
+        downsample = 64
+
+    ### Define parameters:
+    sym_flag = 0
+    G_flag = 0
+    if sym is not None:
+        s = sym[0]
+        n_s = 0
+        if len(sym) > 1:
+            n_s = int(sym[1:len(sym)])
+        sym_flag = 1
+        if s == 'C' and n_s == 1:
+            G = np.eye(3).reshape((1, 3, 3))
+    if G is not None:
+        G_flag = 1
+    refrot = 1
+    if trueR is None:
+        refrot = 0
+
+    # Validate input:
+    # Input volumes must be 3-dimensional, where all dimensions must be equal.
+    # This restriction can be remove, but then, the calculation of nr (radial
+    # resolution in the Fourier domain) should be adjusted accordingly. Both
+    # vol_1 and vol_2 must have the same dimensions.
+    n_1 = np.shape(vol1)
+    assert np.size(n_1) == 3, "Inputs must be 3D"
+    assert n_1[0] == n_1[1], "All dimensions of input volumes must be equal"
+    n_2 = np.shape(vol2)
+    assert np.size(n_2) == 3, "Inputs must be 3D"
+    assert n_2[0] == n_1[1] and n_2[0] == n_1[1], "All dimensions of input volumes must be equal"
+    assert n_1[0] == n_2[0], "Input volumes have different dimensions"
+    n = n_1[0]
+    n_ds = min(n, downsample)  # Perform aligment on down sampled volumes.
+    # This speeds up calculation, and does not seem
+    # to degrade accuracy
+
+    if n_ds < n:
+        logger.info('Downsampling volumes from %i to %i pixels', n, n_ds)
+        vol1_ds = cryo_downsample(vol1, (n_ds, n_ds, n_ds))
+        vol2_ds = cryo_downsample(vol2, (n_ds, n_ds, n_ds))
+    else:
+        logger.info('No need for downsampling. n=%i n_ds=%i', n, n_ds)
+        vol1_ds = vol1
+        vol2_ds = vol2
+
+    # Aligning the volumes:
+    if G_flag == 1:
+        G_c = np.copy(G)
+    else:
+        G_c = None
+    R_est, R_est_J = fast_alignment_3d(sym, vol1_ds.copy(), vol2_ds.copy(),
+                                     Nprojs, trueR, G_c, refrot, verbose)
+
+    logger.debug("R_est=\n%s",str(R_est))
+    logger.debug("R_est_J=\n%s",str(R_est_J))
+
+    vol2_aligned_ds = fastrotate3d(vol2_ds, R_est)  # Rotate the original vol_2 back.
+    vol2_aligned_J_ds = fastrotate3d(vol2_ds, R_est_J)
+
+    vol2_aligned_J_ds = np.flip(vol2_aligned_J_ds, axis=2)
+    estdx_ds = register_translations_3d(vol1_ds, vol2_aligned_ds)
+    estdx_J_ds = register_translations_3d(vol1_ds, vol2_aligned_J_ds)
+    logger.debug("estdx_ds=%s",str(estdx_ds))
+    logger.debug("estdx_J_ds=%s",str(estdx_J_ds))
+
+    if np.size(estdx_ds) != 3 or np.size(estdx_J_ds) != 3:
+        raise Warning("***** Translation estimation failed *****")
+
+    # Prepare FFTW data to avoid unnecessary calaculations        
+    vol2_aligned_ds = src.reshift_vol.reshift_vol_int(vol2_aligned_ds, estdx_ds)
+    vol2_aligned_J_ds = src.reshift_vol.reshift_vol_int(vol2_aligned_J_ds, estdx_J_ds)
+    
+    no1 = np.mean(np.corrcoef(vol1_ds.ravel(), vol2_aligned_ds.ravel(), rowvar=False)[0, 1:])
+    no2 = np.mean(np.corrcoef(vol1_ds.ravel(), vol2_aligned_J_ds.ravel(), rowvar=False)[0, 1:])
+    logger.debug("no1=%f",no1)
+    logger.debug("no2=%f",no2)
+
+    # if max(no1, no2) < 0.1:  # The coorelations of the estimated rotations are
+    #     # smaller than 0.1, that is, no transformation was recovered.
+    #     raise Warning("***** Alignment failed *****")
+    # Do we have reflection?
+    reflect = 0
+    corr_v = no1
+    if no2 > no1:
+        J3 = np.diag([1, 1, -1])
+        corr_v = no2
+        R_est = R_est_J
+        R_est = J3 @ R_est @ J3
+        estdx_ds = estdx_J_ds
+        vol2_ds = np.flip(vol2_ds, axis=2)
+        vol2 = np.flip(vol2, axis=2)
+        reflect = 1
+        logger.info('Input volumes are reflected w.r.t each other')
+    logger.info('Correlation between downsampled aligned volumes '\
+                'before optimization is %.4f', corr_v)
+
+    logger.debug("R_est=\n%s",str(R_est))
+    logger.debug("estdx_ds=%s",str(estdx_ds))
+    logger.debug("reflect=%d", reflect)
+
+    if opt.no_refine:
+        logger.info('Skipping refinement of alignment parameters')
+        bestR = R_est
+    else:
+        logger.info('Using BFGS algorithm to refine alignment parameters')
+        # Optimization:
+        # We use the BFGS optimization algorithm in order to refine the resulted
+        # transformation between the two volumes.
+        bestR = refine3DmatchBFGS(vol1_ds.copy(), vol2_ds.copy(), R_est, estdx_ds)
+        bestR = Rotation.as_matrix(bestR)
+
+    logger.debug("bestR=\n%s",str(bestR))
+    logger.info('Done aligning downsampled volumes')
+    logger.info('Applying estimated rotation to original volumes')
+    vol2aligned = fastrotate3d(vol2, bestR)
+    logger.info('Estimating shift for original volumes')
+    bestdx = register_translations_3d(vol1, vol2aligned)
+    logger.debug("bestdx=%s",str(bestdx))
+    # if np.size(bestdx) != 3 :
+    #    raise Warning("***** Translation estimation failed *****")
+
+    if not opt.no_refine:
+        logger.info('Refining shift for original volumes')
+        bestdx = refine3DshiftBFGS(vol1, vol2, bestdx)
+        logger.debug("bestdx=%s",str(bestdx))
+    else:
+        logger.info('Skipping shift refinement')
+
+    logger.info('Translating original volumes')
+    if (np.round(bestdx) == bestdx).all():
+        # Use fast method
+        vol2aligned = src.reshift_vol.reshift_vol_int(vol2aligned, bestdx)
+    else:
+        vol2aligned = reshift_vol(vol2aligned, bestdx)
+
+    logger.info('Computing correlations of original volumes')
+    bestcorr = np.mean(np.corrcoef(vol1.ravel(), vol2aligned.ravel(), rowvar=False)[0, 1:])
+
+    logger.info('Estimated rotation:\n%s',str(bestR))
+    logger.info('Estimated translations: [%.3f, %.3f, %.3f]', bestdx[0], bestdx[1], bestdx[2])
+    logger.info('Correlation between original aligned volumes is %.4f', bestcorr)
+    # Accurate error calculation:
+    # The difference between the estimated and reference rotation should be an
+    # element from the symmetry group:
+    if refrot == 1 and G_flag == 1:
+        n_g = np.size(G, 0)
+        g_est_t = trueR.T @ bestR.T
+        dist = np.zeros((n_g))
+        for g_idx in range(n_g):
+            dist[g_idx] = LA.norm(g_est_t - G[g_idx, :, :], ord='fro')
+        min_idx = np.argmin(dist)
+        g_est = G[min_idx, :, :]
+        err_norm = LA.norm(trueR.T - (g_est @ bestR), ord='fro')
+        ref_true_R = trueR.T
+        logger.info('Reference rotation:')
+        logger.info('%.4f %.4f %.4f', ref_true_R[0, 0], ref_true_R[0, 1], ref_true_R[0, 2])
+        logger.info('%.4f %.4f %.4f', ref_true_R[1, 0], ref_true_R[1, 1], ref_true_R[1, 2])
+        logger.info('%.4f %.4f %.4f', ref_true_R[2, 0], ref_true_R[2, 1], ref_true_R[2, 2])
+        aligned_bestR = g_est @ bestR
+        logger.info('Estimated rotation (aligned by a symmetry element '\
+                    'according to the reference rotation):')
+        logger.info('%.4f %.4f %.4f', aligned_bestR[0, 0], aligned_bestR[0, 1], aligned_bestR[0, 2])
+        logger.info('%.4f %.4f %.4f', aligned_bestR[1, 0], aligned_bestR[1, 1], aligned_bestR[1, 2])
+        logger.info('%.4f %.4f %.4f', aligned_bestR[2, 0], aligned_bestR[2, 1], aligned_bestR[2, 2])
+        logger.info('Estimated symmetry element:')
+        logger.info('%.4f %.4f %.4f', g_est[0, 0], g_est[0, 1], g_est[0, 2])
+        logger.info('%.4f %.4f %.4f', g_est[1, 0], g_est[1, 1], g_est[1, 2])
+        logger.info('%.4f %.4f %.4f', g_est[2, 0], g_est[2, 1], g_est[2, 2])
+        logger.info('Estimation error (Frobenius norm) up to symmetry '\
+                    'group element is %.4f', err_norm)
+        vec_ref = Rotation.as_rotvec(Rotation.from_matrix(trueR.T))
+        angle_ref = LA.norm(vec_ref)
+        axis_ref = vec_ref / angle_ref
+        vec_est = Rotation.as_rotvec(Rotation.from_matrix(g_est @ bestR))
+        angle_est = LA.norm(vec_est)
+        axis_est = vec_est / angle_est
+        logger.info('Rotation axis:')
+        logger.info('Reference [ %.4f, %.4f, %.4f]', axis_ref[0], axis_ref[1], axis_ref[2])
+        logger.info('Estimated [ %.4f, %.4f, %.4f]', axis_est[0], axis_est[1], axis_est[2])
+        logger.info('Angle between axes is %.4f  degrees',
+                    math.degrees(np.arccos(np.dot(axis_est, axis_ref))))
+        logger.info('In-plane rotation:')
+        logger.info('Reference %.4f degrees', math.degrees(angle_ref))
+        logger.info('Estimated %.4f degrees', math.degrees(angle_est))
+        logger.info('Angle difference is %.4f degrees',
+                    abs(math.degrees(angle_ref) - math.degrees(angle_est)))
+    # Error calculation by optimization:
+    # The difference between the estimated and reference rotation should be an
+    # element from the symmetry group. In the case the symmetry group of vol1
+    # is not given, it can be estimated using optimization process.
+    # Let G be the symmetry group of the symmetry type of the molecule in the
+    # canonical coordinate system (G is obtained using genSymgroup). Then, the
+    # symmetry group of vol1 is given by O*G*O.', where O is the orthogonal
+    # transformation between the coordinate system of vol1 and the canonical
+    # one. Therefore, the symmetry group can be estimated by evaluating O using
+    # optimization algorithm.
+    if refrot == 1 and G_flag == 0 and sym_flag == 1:
+        # Creating initial guess by brute-force algorithm:
+        G = genSymGroup(sym)
+        n_g = np.size(G, 0)
+        Rots = genRotationsGrid(75)
+        n = np.size(Rots, 2)
+        dist = np.zeros((n, n_g))
+        for i in range(n):
+            for j in range(n_g):
+                O = Rots[:, :, i]
+                g = G[j, :, :]
+                dist[i, j] = LA.norm(trueR.T - (O @ g @ O.T @ bestR), ord='fro')
+        err = np.min(dist.ravel())
+        row = np.array(np.where(dist == err))[0]
+        O = Rots[:, :, row[0]]
+        # BFGS optimization:
+        [psi, theta, phi] = (Rotation.from_matrix(O)).as_euler('xyz')
+        X0 = np.array([psi, theta, phi]).astype('float64')
+        res = minimize(evalO, X0, args=(trueR.T, bestR, G), method='BFGS', tol=1e-4,
+                       options={'gtol': 1e-4, 'disp': False})
+        X = res.x
+        psi = X[0]
+        theta = X[1]
+        phi = X[2]
+        O = Rotation.as_matrix(Rotation.from_euler('xyz', [psi, theta, phi], degrees=False))
+        n_g = np.size(G, 0)
+        dist = np.zeros((1, n_g))
+        for i in range(n_g):
+            g = G[i, :, :]
+            dist[0, i] = LA.norm(trueR.T - (O @ g @ O.T @ bestR), 'fro')
+        err_norm = np.min(dist)
+        idx = np.array(np.where(dist == err_norm))
+        g = G[idx[1, 0], :, :]
+        g_est = O @ g @ O.T
+        ref_true_R = trueR.T
+        logger.info('Reference rotation:')
+        logger.info('%.4f %.4f %.4f', ref_true_R[0, 0], ref_true_R[0, 1], ref_true_R[0, 2])
+        logger.info('%.4f %.4f %.4f', ref_true_R[1, 0], ref_true_R[1, 1], ref_true_R[1, 2])
+        logger.info('%.4f %.4f %.4f', ref_true_R[2, 0], ref_true_R[2, 1], ref_true_R[2, 2])
+        aligned_bestR = g_est @ bestR
+        logger.info('Estimated rotation (aligned by a symmetry element '\
+                    'according to the reference rotation):')
+        logger.info('%.4f %.4f %.4f', aligned_bestR[0, 0], aligned_bestR[0, 1], aligned_bestR[0, 2])
+        logger.info('%.4f %.4f %.4f', aligned_bestR[1, 0], aligned_bestR[1, 1], aligned_bestR[1, 2])
+        logger.info('%.4f %.4f %.4f', aligned_bestR[2, 0], aligned_bestR[2, 1], aligned_bestR[2, 2])
+        logger.info('Estimated symmetry element:')
+        logger.info('%.4f %.4f %.4f', g_est[0, 0], g_est[0, 1], g_est[0, 2])
+        logger.info('%.4f %.4f %.4f', g_est[1, 0], g_est[1, 1], g_est[1, 2])
+        logger.info('%.4f %.4f %.4f', g_est[2, 0], g_est[2, 1], g_est[2, 2])
+        logger.info('Estimation error (Frobenius norm) up to symmetry '\
+                    'group element is %.4f', err_norm)
+        vec_ref = Rotation.as_rotvec(Rotation.from_matrix(trueR.T))
+        angle_ref = LA.norm(vec_ref)
+        axis_ref = vec_ref / angle_ref
+        vec_est = Rotation.as_rotvec(Rotation.from_matrix(g_est @ bestR))
+        angle_est = LA.norm(vec_est)
+        axis_est = vec_est / angle_est
+        logger.info('Rotation axis:')
+        logger.info('Reference [ %.4f, %.4f, %.4f]', axis_ref[0], axis_ref[1], axis_ref[2])
+        logger.info('Estimated [ %.4f, %.4f, %.4f]', axis_est[0], axis_est[1], axis_est[2])
+        logger.info('Angle between axes is %.4f  degrees',
+                    math.degrees(np.arccos(np.dot(axis_est, axis_ref))))
+        logger.info('In-plane rotation:')
+        logger.info('Reference %.4f degrees', math.degrees(angle_ref))
+        logger.info('Estimated %.4f degrees', math.degrees(angle_est))
+        logger.info('Angle difference is %.4f degrees',
+                    abs(math.degrees(angle_ref) - math.degrees(angle_est)))
+
+    logging.shutdown()
+
+    return bestR, bestdx, reflect, vol2aligned, bestcorr
```

### Comparing `EMalign-1.0.3/src/common_finufft.py` & `EMalign-1.0.4/src/common_finufft.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,83 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Feb  3 13:20:15 2021
-
-@author: yaelharpaz1
-"""
-
-import numpy as np
-import finufft
-
-from pyfftw.interfaces.numpy_fft import ifft2
-
-    
-    
-def cryo_pft(p, n_r, n_theta):
-    """
-    Compute the polar Fourier transform of projections with resolution n_r in the radial direction
-    and resolution n_theta in the angular direction.
-    :param p:
-    :param n_r: Number of samples along each ray (in the radial direction).
-    :param n_theta: Angular resolution. Number of Fourier rays computed for each projection.
-    :return:
-    """
-    if n_theta % 2 == 1:
-        raise ValueError('n_theta must be even')
-
-    n_projs = p.shape[2]
-    omega0 = 2 * np.pi / (2 * n_r - 1)
-    dtheta = 2 * np.pi / n_theta
-
-    freqs = np.zeros((2, n_r * n_theta // 2))
-    for i in range(n_theta // 2):
-        freqs[0, i * n_r: (i + 1) * n_r] = np.arange(n_r) * np.sin(i * dtheta)
-        freqs[1, i * n_r: (i + 1) * n_r] = np.arange(n_r) * np.cos(i * dtheta)
-
-    freqs *= omega0
-    # finufftpy require it to be aligned in fortran order
-    pf = np.empty((n_r * n_theta // 2, n_projs), dtype='complex128', order='F')
-    #finufftpy.nufft2d2many(freqs[0], freqs[1], pf, 1, 1e-15, p)
-    p_complex = p.astype('complex128')
-    for i in range(n_projs):
-        pf[:,i] = finufft.nufft2d2(freqs[0], freqs[1], p_complex[:,:,i])
-    pf = pf.reshape((n_r, n_theta // 2, n_projs), order='F')
-    pf = np.concatenate((pf.conj(), pf), axis=1).copy()
-    return pf, freqs
-
-def cryo_crop(x, out_shape):
-    """
-    :param x: ndarray of size (N_1,...N_k)
-    :param out_shape: iterable of integers of length k. The value in position i (n_i) is the size we want to cut from
-        the center of x in dimension i. If the value of n_i <= 0 or >= N_i then the dimension is left as is.
-    :return: out: The center of x with size outshape.
-    """
-    in_shape = np.array(x.shape)
-    out_shape = np.array([s if 0 < s < in_shape[i] else in_shape[i] for i, s in enumerate(out_shape)])
-    start_indices = in_shape // 2 - out_shape // 2
-    end_indices = start_indices + out_shape
-    indexer = tuple([slice(i, j) for (i, j) in zip(start_indices, end_indices)])
-    out = x[indexer]
-    return out
-
-def cryo_downsample(x, out_shape):
-    """
-    :param x: ndarray of size (N_1,...N_k)
-    :param out_shape: iterable of integers of length k. The value in position i (n_i) is the size we want to cut from
-        the center of x in dimension i. If the value of n_i <= 0 or >= N_i then the dimension is left as is.
-    :return: out: downsampled x
-    """
-    dtype_in = x.dtype
-    in_shape = np.array(x.shape)
-    out_shape = np.array([s if 0 < s < in_shape[i] else in_shape[i] for i, s in enumerate(out_shape)])
-    fourier_dims = np.array([i for i, s in enumerate(out_shape) if 0 < s < in_shape[i]])
-    size_in = np.prod(in_shape[fourier_dims])
-    size_out = np.prod(out_shape[fourier_dims])
-
-    fx = cryo_crop(np.fft.fftshift(np.fft.fft2(x, axes=fourier_dims), axes=fourier_dims), out_shape)
-    out = ifft2(np.fft.ifftshift(fx, axes=fourier_dims), axes=fourier_dims) * (size_out / size_in)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Feb  3 13:20:15 2021
+
+@author: yaelharpaz1
+"""
+
+import numpy as np
+import finufft
+
+from pyfftw.interfaces.numpy_fft import ifft2
+
+    
+    
+def cryo_pft(p, n_r, n_theta):
+    """
+    Compute the polar Fourier transform of projections with resolution n_r in the radial direction
+    and resolution n_theta in the angular direction.
+    :param p:
+    :param n_r: Number of samples along each ray (in the radial direction).
+    :param n_theta: Angular resolution. Number of Fourier rays computed for each projection.
+    :return:
+    """
+    if n_theta % 2 == 1:
+        raise ValueError('n_theta must be even')
+
+    n_projs = p.shape[2]
+    omega0 = 2 * np.pi / (2 * n_r - 1)
+    dtheta = 2 * np.pi / n_theta
+
+    freqs = np.zeros((2, n_r * n_theta // 2))
+    for i in range(n_theta // 2):
+        freqs[0, i * n_r: (i + 1) * n_r] = np.arange(n_r) * np.sin(i * dtheta)
+        freqs[1, i * n_r: (i + 1) * n_r] = np.arange(n_r) * np.cos(i * dtheta)
+
+    freqs *= omega0
+    # finufftpy require it to be aligned in fortran order
+    pf = np.empty((n_r * n_theta // 2, n_projs), dtype='complex128', order='F')
+    #finufftpy.nufft2d2many(freqs[0], freqs[1], pf, 1, 1e-15, p)
+    p_complex = p.astype('complex128')
+    for i in range(n_projs):
+        pf[:,i] = finufft.nufft2d2(freqs[0], freqs[1], p_complex[:,:,i])
+    pf = pf.reshape((n_r, n_theta // 2, n_projs), order='F')
+    pf = np.concatenate((pf.conj(), pf), axis=1).copy()
+    return pf, freqs
+
+def cryo_crop(x, out_shape):
+    """
+    :param x: ndarray of size (N_1,...N_k)
+    :param out_shape: iterable of integers of length k. The value in position i (n_i) is the size we want to cut from
+        the center of x in dimension i. If the value of n_i <= 0 or >= N_i then the dimension is left as is.
+    :return: out: The center of x with size outshape.
+    """
+    in_shape = np.array(x.shape)
+    out_shape = np.array([s if 0 < s < in_shape[i] else in_shape[i] for i, s in enumerate(out_shape)])
+    start_indices = in_shape // 2 - out_shape // 2
+    end_indices = start_indices + out_shape
+    indexer = tuple([slice(i, j) for (i, j) in zip(start_indices, end_indices)])
+    out = x[indexer]
+    return out
+
+def cryo_downsample(x, out_shape):
+    """
+    :param x: ndarray of size (N_1,...N_k)
+    :param out_shape: iterable of integers of length k. The value in position i (n_i) is the size we want to cut from
+        the center of x in dimension i. If the value of n_i <= 0 or >= N_i then the dimension is left as is.
+    :return: out: downsampled x
+    """
+    dtype_in = x.dtype
+    in_shape = np.array(x.shape)
+    out_shape = np.array([s if 0 < s < in_shape[i] else in_shape[i] for i, s in enumerate(out_shape)])
+    
+    if all(in_shape==out_shape):
+        return x.copy()  # No need to do anything
+    
+    fourier_dims = np.array([i for i, s in enumerate(out_shape) if 0 < s < in_shape[i]])
+    size_in = np.prod(in_shape[fourier_dims])
+    size_out = np.prod(out_shape[fourier_dims])
+
+    fx = cryo_crop(np.fft.fftshift(np.fft.fft2(x, axes=fourier_dims), axes=fourier_dims), out_shape)
+    out = ifft2(np.fft.ifftshift(fx, axes=fourier_dims), axes=fourier_dims) * (size_out / size_in)
     return (np.real(out)).astype(dtype_in)
```

### Comparing `EMalign-1.0.3/src/cryo_fetch_emdID.py` & `EMalign-1.0.4/src/cryo_fetch_emdID.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Mar  2 14:41:16 2022
-
-@author: Yoel Shkolnisky
-"""
-
-import ftplib 
-import logging
-import os
-import gzip
-import shutil
-
-def cryo_fetch_emdID(emdID,mrc_filename,verbose=1):
-    """
-    cryo_fetch_emdID  Fetch a density map from EMDB.
-    
-    This function fetchs the map file (MRC format) with the given emdID 
-    (integer) from EMDB. The MRC file is saved into the file mrc_filename, 
-    which should contain the full path to the saved file. 
-        
-    """
-       
-    #logging.basicConfig(level=logging.INFO,\
-    #                    format='%(asctime)s %(levelname)s %(message)s')
-    logger = logging.getLogger()
-    logger.disabled = False
-    if verbose == 0: 
-        logger.disabled = True  
-        
-    emdIDstr = str(emdID)
-    
-    # Connect FTP Server
-    hostname =  "ftp.ebi.ac.uk"
-    username = "anonymous"
-    password = ""
-    
-    logger.info('Establishing an FTP connection with the EMD server ...')
-    ftp_server = ftplib.FTP(hostname,username,password)
-    logger.info('FTP connection was established.')
-    
-    # force UTF-8 encoding
-    ftp_server.encoding = "utf-8"
-    
-    logger.info('Downloading the zipped density map ...')
-    remote_dir = '/pub/databases/emdb/structures/EMD-%s/map/' %(emdIDstr)
-    filename = 'emd_%s.map.gz' %(emdIDstr)
-    remote_filename = remote_dir+filename
-    output_dir = os.path.dirname(mrc_filename)    
-    local_filename = os.path.join(output_dir,filename)
-        
-    # Write file in binary mode    
-    with open(local_filename, "wb") as file:
-        # Command for Downloading the file "RETR filename"
-        ftp_server.retrbinary(f"RETR {remote_filename}", file.write)
-    logger.info('The zipped density map was downloaded as %s.',local_filename)
-    
-        
-    logger.info('Closing the FTP connection ...')
-    ftp_server.quit()
-    logger.info('The FTP connection was closed.')
-          
-       
-    logger.info('Unzipping the downloaded file ...')
-    # mrc_filename = (local_filename.removesuffix('.map.gz'))+".mrc"
-    with gzip.open(local_filename, 'rb') as f_in:
-        with open(mrc_filename, 'wb') as f_out:
-            shutil.copyfileobj(f_in, f_out)  
-            
-    # Delete gzip file and keep only MRC file.
-    os.remove(local_filename)
-    logger.info('Done. Save map to %s', mrc_filename)
-
-
-
-
-
-
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Mar  2 14:41:16 2022
+
+@author: Yoel Shkolnisky
+"""
+
+import ftplib 
+import logging
+import os
+import gzip
+import shutil
+
+def cryo_fetch_emdID(emdID,mrc_filename,verbose=1):
+    """
+    cryo_fetch_emdID  Fetch a density map from EMDB.
+    
+    This function fetchs the map file (MRC format) with the given emdID 
+    (integer) from EMDB. The MRC file is saved into the file mrc_filename, 
+    which should contain the full path to the saved file. 
+        
+    """
+       
+    #logging.basicConfig(level=logging.INFO,\
+    #                    format='%(asctime)s %(levelname)s %(message)s')
+    logger = logging.getLogger()
+    logger.disabled = False
+    if verbose == 0: 
+        logger.disabled = True  
+        
+    emdIDstr = str(emdID)
+    
+    # Connect FTP Server
+    hostname =  "ftp.ebi.ac.uk"
+    username = "anonymous"
+    password = ""
+    
+    logger.info('Establishing an FTP connection with the EMD server ...')
+    ftp_server = ftplib.FTP(hostname,username,password)
+    logger.info('FTP connection was established.')
+    
+    # force UTF-8 encoding
+    ftp_server.encoding = "utf-8"
+    
+    logger.info('Downloading the zipped density map ...')
+    remote_dir = '/pub/databases/emdb/structures/EMD-%s/map/' %(emdIDstr)
+    filename = 'emd_%s.map.gz' %(emdIDstr)
+    remote_filename = remote_dir+filename
+    output_dir = os.path.dirname(mrc_filename)    
+    local_filename = os.path.join(output_dir,filename)
+        
+    # Write file in binary mode    
+    with open(local_filename, "wb") as file:
+        # Command for Downloading the file "RETR filename"
+        ftp_server.retrbinary(f"RETR {remote_filename}", file.write)
+    logger.info('The zipped density map was downloaded as %s.',local_filename)
+    
+        
+    logger.info('Closing the FTP connection ...')
+    ftp_server.quit()
+    logger.info('The FTP connection was closed.')
+          
+       
+    logger.info('Unzipping the downloaded file ...')
+    # mrc_filename = (local_filename.removesuffix('.map.gz'))+".mrc"
+    with gzip.open(local_filename, 'rb') as f_in:
+        with open(mrc_filename, 'wb') as f_out:
+            shutil.copyfileobj(f_in, f_out)  
+            
+    # Delete gzip file and keep only MRC file.
+    os.remove(local_filename)
+    logger.info('Done. Save map to %s', mrc_filename)
+
+
+
+
+
+
```

### Comparing `EMalign-1.0.3/src/cryo_project_itay_finufft.py` & `EMalign-1.0.4/src/cryo_project_itay_finufft.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import numpy as np
-import finufft
-
-
-class FINufftPlan:
-    def __init__(self, sz, fourier_pts, epsilon=1e-15):
-        """
-        A plan for non-uniform FFT (3D)
-        :param sz: A tuple indicating the geometry of the signal
-        :param fourier_pts: The points in Fourier space where the Fourier transform is to be calculated,
-            arranged as a 3-by-K array. These need to be in the range [-pi, pi] in each dimension.
-        :param epsilon: The desired precision of the NUFFT
-        """
-        self.sz = sz
-        self.dim = len(sz)
-        # TODO: Things get messed up unless we ensure a 'C' ordering here - investigate why
-        self.fourier_pts = np.asarray(np.mod(fourier_pts + np.pi, 2 * np.pi) - np.pi, order='C')
-        self.num_pts = fourier_pts.shape[1]
-        self.epsilon = epsilon
-
-        # Get a handle on the appropriate 1d/2d/3d forward transform function in finufftpy
-        self.transform_function = getattr(finufft, {1: 'nufft1d2', 2: 'nufft2d2', 3: 'nufft3d2'}[self.dim])
-        # Get a handle on the appropriate 1d/2d/3d adjoint function in finufftpy
-        self.adjoint_function = getattr(finufft, {1: 'nufft1d1', 2: 'nufft2d1', 3: 'nufft3d1'}[self.dim])
-
-    def transform(self, signal):
-        epsilon = max(self.epsilon, np.finfo(signal.dtype).eps)
-
-        # Forward transform functions in finufftpy have signatures of the form:
-        # (x, y, z, c, isign, eps, f, ...)
-        # (x, y     c, isign, eps, f, ...)
-        # (x,       c, isign, eps, f, ...)
-        # Where f is a Fortran-order ndarray of the appropriate dimensions
-        # We form these function signatures here by tuple-unpacking
-
-        result = np.zeros(self.num_pts).astype('complex128')
-
-        result = self.transform_function(
-            self.fourier_pts[0].astype('float64'),
-            self.fourier_pts[1].astype('float64'),
-            self.fourier_pts[2].astype('float64'),
-            signal.astype('complex128'))
-            #*self.fourier_pts[0],
-            #*self.fourier_pts[1],
-            #*self.fourier_pts[2],
-            #signal
-            #*self.fourier_pts,
-            #result,
-            #-1,
-            #epsilon,
-            #signal
-        #)
-
-        #if result_code != 0:
-        #    raise RuntimeError(f'FINufft transform failed. Result code {result_code}')
-
-        return result
-
-    def adjoint(self, signal):
-
-        epsilon = max(self.epsilon, np.finfo(signal.dtype).eps)
-
-        # Adjoint functions in finufftpy have signatures of the form:
-        # (x, y, z, c, isign, eps, ms, mt, mu, f, ...)
-        # (x, y     c, isign, eps, ms, mt      f, ...)
-        # (x,       c, isign, eps, ms,         f, ...)
-        # Where f is a Fortran-order ndarray of the appropriate dimensions
-        # We form these function signatures here by tuple-unpacking
-
-        # Note: Important to have order='F' here!
-        result = np.zeros(self.sz, order='F').astype('complex128')
-
-        result = self.adjoint_function(       
-            self.fourier_pts[0].astype('float64'),
-            self.fourier_pts[1].astype('float64'),
-            self.fourier_pts[2].astype('float64'),
-            signal.astype('complex128'))
-            #*self.fourier_pts,
-            #signal,
-            #1,
-            #epsilon,
-            #*self.sz,
-            #result
-        #)
-        #if result_code != 0:
-        #    raise RuntimeError(f'FINufft adjoint failed. Result code {result_code}')
-
-        return result
-
-
-def cryo_project(vol, rot, n=None, eps=np.finfo(np.float32).eps, batch_size=100):
-    nv = vol.shape[0]
-    if n is None:
-        n = nv
-
-    r = np.arange(-(n - 1) / 2, (n - 1) / 2 + 1)
-    I, J = np.meshgrid(r, r)  # i, j are reverse, but I flatten them using python indexing so they are switched back
-    I = I.flatten()
-    J = J.flatten()
-
-    if n > nv + 1:
-        if (n - nv) % 2 == 1:
-            raise ValueError('Upsampling from odd to even sizes or vice versa is not supported')
-        dN = (n - nv) // 2
-        fv = cfftn(vol)
-        padded_vol = np.zeros((n, n, n), dtype='complex')
-        padded_vol[dN:dN+nv, dN:dN+nv, dN:dN+nv] = fv
-        vol = icfftn(padded_vol).astype('float32')
-        nv = n
-
-    num_rots = rot.shape[2]
-    batch_size = min(batch_size, num_rots)
-    num_batches = int(np.ceil(num_rots / batch_size))
-    out_projections = np.zeros((n, n, num_rots))
-    for batch in range(num_batches):
-        curr_batch_size = int(min(batch_size, num_rots - batch * batch_size))
-        p = np.zeros((len(I) * curr_batch_size, 3))
-        start = batch * batch_size
-
-        for k in range(curr_batch_size):
-            n_x = rot[0, :, start + k]
-            n_y = rot[1, :, start + k]
-            p[k * len(I): (k + 1) * len(I)] = np.outer(I, n_x) + np.outer(J, n_y)
-        p *= -2 * np.pi / nv
-        plan = FINufftPlan((nv, nv, nv), -p.T.copy(), eps)
-        projection_fourier = plan.transform(vol)
-        projection_fourier = np.reshape(projection_fourier, (len(I), curr_batch_size), 'F')
-        p = np.reshape(p, (len(I), curr_batch_size, 3), 'F')
-
-        if n % 2 == 0:
-            projection_fourier *= np.exp(np.sum(p, 2) * (1j / 2))
-            Irep = np.array([I] * curr_batch_size).T
-            Jrep = np.array([J] * curr_batch_size).T
-            projection_fourier *= np.exp((Irep + Jrep - 1) * (np.pi * 1j / n))
-
-        for k in range(curr_batch_size):
-            projection = np.reshape(projection_fourier[:, k], (n, n), 'F')
-            projection = np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(projection)))
-
-            if n % 2 == 0:
-                projection *= np.reshape(np.exp((I + J) * (np.pi * 1j / n)), (n, n), 'F')
-
-            out_projections[:, :, start + k] = np.real(projection)
-
-    return out_projections
-
-
-def cfftn(x):
-    return np.fft.fftshift(np.fft.fftn(np.fft.ifftshift(x)))
-
-
-def icfftn(x):
-    return np.fft.fftshift(np.fft.ifftn(np.fft.ifftshift(x)))
+import numpy as np
+import finufft
+
+
+class FINufftPlan:
+    def __init__(self, sz, fourier_pts, epsilon=1e-15):
+        """
+        A plan for non-uniform FFT (3D)
+        :param sz: A tuple indicating the geometry of the signal
+        :param fourier_pts: The points in Fourier space where the Fourier transform is to be calculated,
+            arranged as a 3-by-K array. These need to be in the range [-pi, pi] in each dimension.
+        :param epsilon: The desired precision of the NUFFT
+        """
+        self.sz = sz
+        self.dim = len(sz)
+        # TODO: Things get messed up unless we ensure a 'C' ordering here - investigate why
+        self.fourier_pts = np.asarray(np.mod(fourier_pts + np.pi, 2 * np.pi) - np.pi, order='C')
+        self.num_pts = fourier_pts.shape[1]
+        self.epsilon = epsilon
+
+        # Get a handle on the appropriate 1d/2d/3d forward transform function in finufftpy
+        self.transform_function = getattr(finufft, {1: 'nufft1d2', 2: 'nufft2d2', 3: 'nufft3d2'}[self.dim])
+        # Get a handle on the appropriate 1d/2d/3d adjoint function in finufftpy
+        self.adjoint_function = getattr(finufft, {1: 'nufft1d1', 2: 'nufft2d1', 3: 'nufft3d1'}[self.dim])
+
+    def transform(self, signal):
+        epsilon = max(self.epsilon, np.finfo(signal.dtype).eps)
+
+        # Forward transform functions in finufftpy have signatures of the form:
+        # (x, y, z, c, isign, eps, f, ...)
+        # (x, y     c, isign, eps, f, ...)
+        # (x,       c, isign, eps, f, ...)
+        # Where f is a Fortran-order ndarray of the appropriate dimensions
+        # We form these function signatures here by tuple-unpacking
+
+        result = np.zeros(self.num_pts).astype('complex128')
+
+        result = self.transform_function(
+            self.fourier_pts[0].astype('float64'),
+            self.fourier_pts[1].astype('float64'),
+            self.fourier_pts[2].astype('float64'),
+            signal.astype('complex128'))
+            #*self.fourier_pts[0],
+            #*self.fourier_pts[1],
+            #*self.fourier_pts[2],
+            #signal
+            #*self.fourier_pts,
+            #result,
+            #-1,
+            #epsilon,
+            #signal
+        #)
+
+        #if result_code != 0:
+        #    raise RuntimeError(f'FINufft transform failed. Result code {result_code}')
+
+        return result
+
+    def adjoint(self, signal):
+
+        epsilon = max(self.epsilon, np.finfo(signal.dtype).eps)
+
+        # Adjoint functions in finufftpy have signatures of the form:
+        # (x, y, z, c, isign, eps, ms, mt, mu, f, ...)
+        # (x, y     c, isign, eps, ms, mt      f, ...)
+        # (x,       c, isign, eps, ms,         f, ...)
+        # Where f is a Fortran-order ndarray of the appropriate dimensions
+        # We form these function signatures here by tuple-unpacking
+
+        # Note: Important to have order='F' here!
+        result = np.zeros(self.sz, order='F').astype('complex128')
+
+        result = self.adjoint_function(       
+            self.fourier_pts[0].astype('float64'),
+            self.fourier_pts[1].astype('float64'),
+            self.fourier_pts[2].astype('float64'),
+            signal.astype('complex128'))
+            #*self.fourier_pts,
+            #signal,
+            #1,
+            #epsilon,
+            #*self.sz,
+            #result
+        #)
+        #if result_code != 0:
+        #    raise RuntimeError(f'FINufft adjoint failed. Result code {result_code}')
+
+        return result
+
+
+def cryo_project(vol, rot, n=None, eps=np.finfo(np.float32).eps, batch_size=100):
+    nv = vol.shape[0]
+    if n is None:
+        n = nv
+
+    r = np.arange(-(n - 1) / 2, (n - 1) / 2 + 1)
+    I, J = np.meshgrid(r, r)  # i, j are reverse, but I flatten them using python indexing so they are switched back
+    I = I.flatten()
+    J = J.flatten()
+
+    if n > nv + 1:
+        if (n - nv) % 2 == 1:
+            raise ValueError('Upsampling from odd to even sizes or vice versa is not supported')
+        dN = (n - nv) // 2
+        fv = cfftn(vol)
+        padded_vol = np.zeros((n, n, n), dtype='complex')
+        padded_vol[dN:dN+nv, dN:dN+nv, dN:dN+nv] = fv
+        vol = icfftn(padded_vol).astype('float32')
+        nv = n
+
+    num_rots = rot.shape[2]
+    batch_size = min(batch_size, num_rots)
+    num_batches = int(np.ceil(num_rots / batch_size))
+    out_projections = np.zeros((n, n, num_rots))
+    for batch in range(num_batches):
+        curr_batch_size = int(min(batch_size, num_rots - batch * batch_size))
+        p = np.zeros((len(I) * curr_batch_size, 3))
+        start = batch * batch_size
+
+        for k in range(curr_batch_size):
+            n_x = rot[0, :, start + k]
+            n_y = rot[1, :, start + k]
+            p[k * len(I): (k + 1) * len(I)] = np.outer(I, n_x) + np.outer(J, n_y)
+        p *= -2 * np.pi / nv
+        plan = FINufftPlan((nv, nv, nv), -p.T.copy(), eps)
+        projection_fourier = plan.transform(vol)
+        projection_fourier = np.reshape(projection_fourier, (len(I), curr_batch_size), 'F')
+        p = np.reshape(p, (len(I), curr_batch_size, 3), 'F')
+
+        if n % 2 == 0:
+            projection_fourier *= np.exp(np.sum(p, 2) * (1j / 2))
+            Irep = np.array([I] * curr_batch_size).T
+            Jrep = np.array([J] * curr_batch_size).T
+            projection_fourier *= np.exp((Irep + Jrep - 1) * (np.pi * 1j / n))
+
+        for k in range(curr_batch_size):
+            projection = np.reshape(projection_fourier[:, k], (n, n), 'F')
+            projection = np.fft.fftshift(np.fft.ifft2(np.fft.ifftshift(projection)))
+
+            if n % 2 == 0:
+                projection *= np.reshape(np.exp((I + J) * (np.pi * 1j / n)), (n, n), 'F')
+
+            out_projections[:, :, start + k] = np.real(projection)
+
+    return out_projections
+
+
+def cfftn(x):
+    return np.fft.fftshift(np.fft.fftn(np.fft.ifftshift(x)))
+
+
+def icfftn(x):
+    return np.fft.fftshift(np.fft.ifftn(np.fft.ifftshift(x)))
```

### Comparing `EMalign-1.0.3/src/emalign_input.py` & `EMalign-1.0.4/src/emalign_input.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,233 +1,248 @@
-from pathlib import Path
-import sys
-import subprocess
-import argparse
-import os
-
-DEFAULT_DOWNSAMPLE = 64
-DEFAULT_N_PROJS = 30
-
-
-def parse_args():
-    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    
-    parser.add_argument('-v1', '--vol1', help='Full path of first mrc input file', type=check_mrc_file_exist)
-    parser.add_argument('-v2', '--vol2', help='Full path of second mrc input file', type=check_mrc_file_exist)
-    parser.add_argument('-o', '--output-vol', help='Full path of output mrc file', type=check_mrc_file_not_exist)
-    parser.add_argument('--downsample', help='Dimension to downsample input volumes', default=DEFAULT_DOWNSAMPLE,
-                        type=check_positive_int)
-    parser.add_argument('--n-projs', help='Number of projections', default=DEFAULT_N_PROJS,
-                        type=check_positive_int)
-    parser.add_argument('--no-refine', help='Skip optimization to refine aligment parameters', action='store_true', default=False)
-    parser.add_argument('--output-parameters', help='Full path of output txt file for alignment parameters', default=None,
-                        type=check_txt_file_not_exist)
-    parser.add_argument('-v', '--verbose', action='store_true',
-                        help='Print progress messages', default=False)
-
-    # Make emalign to generate two volumes, which can be used to test the 
-    # alignment algorithm.
-    parser.add_argument('--make-test-data', help='Generate test volumes to test emalign', action='store_true',
-                        default=False)
-
-    # Version
-    parser.add_argument('--version', help='print program version and exit', action='store_true', default=False)
-
-    args = parser.parse_args()
-    return args
-
-
-def check_positive_int(value):
-    ivalue = int(value)
-    if ivalue <= 0:
-        raise argparse.ArgumentTypeError("%s is an invalid positive int value" % value)
-    return ivalue
-
-
-def check_mrc_file_exist(output_file):
-    if not os.path.isfile(output_file):
-        raise argparse.ArgumentTypeError("There is no file with the name %s." % output_file)
-    if output_file[-4:] != '.mrc':
-        raise argparse.ArgumentTypeError('%s is not an mrc file.' % output_file)
-    return output_file
-
-
-def check_mrc_file_not_exist(output_file):
-    if os.path.isfile(output_file):
-        raise argparse.ArgumentTypeError("There is already a file with the name %s." % output_file)
-    output_dir, _ = os.path.split(output_file)
-    if output_dir == "":    # No directory not specified. Use current directory.
-        output_dir = "."
-        output_file = os.path.join(output_dir, output_file)
-    if not os.path.isdir(output_dir):
-        raise argparse.ArgumentTypeError(
-            'Directory %s does not exist. Please specify a file in existing directory.' % output_dir)
-    if output_file[-4:] != '.mrc':
-        raise argparse.ArgumentTypeError('%s is not an mrc file.' % output_file)
-    return output_file
-
-
-def check_txt_file_not_exist(output_file):
-    if os.path.isfile(output_file):
-        raise argparse.ArgumentTypeError("There is already a file with the name %s." % output_file)
-    output_dir, _ = os.path.split(output_file)
-    if output_dir == "":    # No directory not specified. Use current directory.
-        output_dir = "."
-        output_file = os.path.join(output_dir, output_file)
-    if not os.path.isdir(output_dir):
-        raise argparse.ArgumentTypeError(
-            'Directory %s does not exist. Please specify a file in existing directory.' % output_dir)
-    if output_file[-4:] != '.txt':
-        raise argparse.ArgumentTypeError('%s is not an txt file.' % output_file)
-    return output_file
-
-
-def get_args():
-    # print("\n")
-    while True:
-        vol1 = input('Enter full path of reference volume MRC file: ')
-        if vol1[-4:] != '.mrc':
-            print('Please enter an MRC file')
-            continue
-        if not os.path.isfile(vol1):
-            # replace = input('There is already a file with the name {}.'. format())
-            print('File does not exist')
-            continue
-        break
-    while True:
-        vol2 = input('Enter full path of query volume MRC file: ')
-        if vol2[-4:] != '.mrc':
-            print('Please enter an MRC file')
-            continue
-        if not os.path.isfile(vol2):
-            # replace = input('There is already a file with the name {}.'. format())
-            print('File does not exist')
-            continue
-        break
-
-    while True:
-        output_vol = input('Enter full path of output aligned volume MRC file: ')
-        if output_vol[-4:] != '.mrc':
-            print('Please enter an MRC file')
-            continue
-        if os.path.isfile(output_vol):
-            break_flag = False
-            while True:
-                replace = input(
-                    'There is already a file with the name {}. Do you want to replace it [y/n]?: '.format(output_vol))
-                if replace.lower().startswith('y'):
-                    break_flag = True
-                    break
-                if replace.lower().startswith('n'):
-                    break
-            if break_flag:
-                break
-        break
-
-    while True:
-        downsample = input('Enter the downsampled size in pixels (default {}): '.format(DEFAULT_DOWNSAMPLE))
-        if downsample == '':
-            downsample = DEFAULT_DOWNSAMPLE
-            break
-        try:
-            downsample = int(downsample)
-            if downsample < 1:
-                print("Downsample size must be a positive integer.")
-            else:
-                break
-        except ValueError:
-            print("Downsample size must be a positive integer.")
-
-    while True:
-        n_projs = input('Enter the number of projections (default {}): '.format(DEFAULT_N_PROJS))
-        if n_projs == '':
-            n_projs = DEFAULT_N_PROJS
-            break
-        try:
-            n_projs = int(n_projs)
-            if n_projs < 1:
-                print("Number of projections must be a positive integer.")
-            else:
-                break
-        except ValueError:
-            print("Number of projections must be a positive integer.")
-            
-    # Ask to skip refinement of alignment parameters
-    while True:
-        no_refine = input('Do you want to refine alignment parameters [y/n]')
-
-        if any(no_refine.lower() == f for f in ["yes", 'y', '1', 'ye']):
-            no_refine = False
-            break
-        elif any(no_refine.lower() == f for f in ['no', 'n', '0']):
-            no_refine = True
-            break
-        else:
-            print("Please choose y/n.")
-            
-    # Check if user want to save parameters
-    while True:
-        save_params = input('Do you want to save output parameters [y/n]: ')
-        if save_params.lower().startswith('y'):
-            # If he does, ask for file
-            while True:
-                output_parameters = input('Enter full path of output parameters txt file: ')
-                if output_parameters[-4:] != '.txt':
-                    print('Please enter an txt file')
-                    continue
-                if os.path.isfile(output_parameters):
-                    break_flag = False
-                    while True:
-                        replace = str(input(
-                            'There is already a file with the name {}. Do you want to replace it [y/n]?: '.format(
-                                output_parameters)))
-                        if replace.lower().startswith('y'):
-                            break_flag = True
-                            break
-                        if replace.lower().startswith('n'):
-                            break
-                    if break_flag:
-                        break
-                break
-            break
-        if save_params.lower().startswith('n'):
-            output_parameters = None
-            break
-
-    verbose = 0
-    while verbose == 0:
-        verbose_in = input('Display detailed progress? [y/n]: ')
-        if verbose_in.strip().lower().startswith('y'):
-            verbose = 1
-        elif verbose_in.strip().lower().startswith('n'):
-            verbose = 0
-            break
-        else:
-            print("Please choose y/n.")
-
-    return vol1, vol2, output_vol, downsample, n_projs, no_refine, output_parameters, verbose
-
-
-def check_for_newer_version():
-    """
-    This function checks whether there is a newer version of kltpicker
-    available on PyPI. If there is, it issues a warning.
-
-    """
-    name = 'EMalign'
-    # Use pip to try and install a version of kltpicker which does not exist.
-    # In answer, you get all available versions. Find the newest one.
-    latest_version = str(
-        subprocess.run([sys.executable, '-m', 'pip', 'install', '%s==random' % name], capture_output=True, text=True))
-    latest_version = latest_version[latest_version.find('(from versions:') + 15:]
-    latest_version = latest_version[:latest_version.find(')')]
-    latest_version = latest_version.replace(' ', '').split(',')[-1]
-
-    if latest_version == 'none':  # Got an unexpected response.
-        pass
-    else:  # Use pip to determine the installed version.
-        import pkg_resources  # part of setuptools
-        current_version = pkg_resources.require(name)[0].version
-        if latest_version > current_version:
-            print(
-                "NOTE: you are running an old version of %s (%s). A newer version (%s) is available, please upgrade." % (
-                    name, current_version, latest_version))
+from pathlib import Path
+import sys
+import subprocess
+import argparse
+import os
+
+DEFAULT_DOWNSAMPLE = 64
+DEFAULT_N_PROJS = 30
+
+
+def parse_args():
+    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    
+    parser.add_argument('-v1', '--vol1', help='Full path of first mrc input file', type=check_mrc_file_exist)
+    parser.add_argument('-v2', '--vol2', help='Full path of second mrc input file', type=check_mrc_file_exist)
+    parser.add_argument('-o', '--output-vol', help='Full path of output mrc file', type=check_mrc_file_not_exist)
+    parser.add_argument('--downsample', help='Dimension to downsample input volumes', default=DEFAULT_DOWNSAMPLE,
+                        type=check_positive_int)
+    parser.add_argument('--n-projs', help='Number of projections', default=DEFAULT_N_PROJS,
+                        type=check_positive_int)     
+    parser.add_argument('--apply-filtering', help='Lowpass filter input volumes (helps when input is noisy)', action='store_true', default=False)    
+    parser.add_argument('--no-refine', help='Skip optimization to refine aligment parameters', action='store_true', default=False)
+    parser.add_argument('--output-parameters', help='Full path of output txt file for alignment parameters', default=None,
+                        type=check_txt_file_not_exist)
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='Print progress messages', default=False)
+
+    # Make emalign to generate two volumes, which can be used to test the 
+    # alignment algorithm.
+    parser.add_argument('--make-test-data', help='Generate test volumes to test emalign', action='store_true',
+                        default=False)
+
+    # Version
+    parser.add_argument('--version', help='print program version and exit', action='store_true', default=False)
+
+    args = parser.parse_args()
+    return args
+
+
+def check_positive_int(value):
+    ivalue = int(value)
+    if ivalue <= 0:
+        raise argparse.ArgumentTypeError("%s is an invalid positive int value" % value)
+    return ivalue
+
+
+def check_mrc_file_exist(output_file):
+    if not os.path.isfile(output_file):
+        raise argparse.ArgumentTypeError("There is no file with the name %s." % output_file)
+    if output_file[-4:] != '.mrc':
+        raise argparse.ArgumentTypeError('%s is not an mrc file.' % output_file)
+    return output_file
+
+
+def check_mrc_file_not_exist(output_file):
+    if os.path.isfile(output_file):
+        raise argparse.ArgumentTypeError("There is already a file with the name %s." % output_file)
+    output_dir, _ = os.path.split(output_file)
+    if output_dir == "":    # No directory not specified. Use current directory.
+        output_dir = "."
+        output_file = os.path.join(output_dir, output_file)
+    if not os.path.isdir(output_dir):
+        raise argparse.ArgumentTypeError(
+            'Directory %s does not exist. Please specify a file in existing directory.' % output_dir)
+    if output_file[-4:] != '.mrc':
+        raise argparse.ArgumentTypeError('%s is not an mrc file.' % output_file)
+    return output_file
+
+
+def check_txt_file_not_exist(output_file):
+    if os.path.isfile(output_file):
+        raise argparse.ArgumentTypeError("There is already a file with the name %s." % output_file)
+    output_dir, _ = os.path.split(output_file)
+    if output_dir == "":    # No directory not specified. Use current directory.
+        output_dir = "."
+        output_file = os.path.join(output_dir, output_file)
+    if not os.path.isdir(output_dir):
+        raise argparse.ArgumentTypeError(
+            'Directory %s does not exist. Please specify a file in existing directory.' % output_dir)
+    if output_file[-4:] != '.txt':
+        raise argparse.ArgumentTypeError('%s is not an txt file.' % output_file)
+    return output_file
+
+
+def get_args():
+    # print("\n")
+    while True:
+        vol1 = input('Enter full path of reference volume MRC file: ')
+        if vol1[-4:] != '.mrc':
+            print('Please enter an MRC file')
+            continue
+        if not os.path.isfile(vol1):
+            # replace = input('There is already a file with the name {}.'. format())
+            print('File does not exist')
+            continue
+        break
+    while True:
+        vol2 = input('Enter full path of query volume MRC file: ')
+        if vol2[-4:] != '.mrc':
+            print('Please enter an MRC file')
+            continue
+        if not os.path.isfile(vol2):
+            # replace = input('There is already a file with the name {}.'. format())
+            print('File does not exist')
+            continue
+        break
+
+    while True:
+        output_vol = input('Enter full path of output aligned volume MRC file: ')
+        if output_vol[-4:] != '.mrc':
+            print('Please enter an MRC file')
+            continue
+        if os.path.isfile(output_vol):
+            break_flag = False
+            while True:
+                replace = input(
+                    'There is already a file with the name {}. Do you want to replace it [y/n]?: '.format(output_vol))
+                if replace.lower().startswith('y'):
+                    break_flag = True
+                    break
+                if replace.lower().startswith('n'):
+                    break
+            if break_flag:
+                break
+        break
+
+    while True:
+        downsample = input('Enter the downsampled size in pixels (default {}): '.format(DEFAULT_DOWNSAMPLE))
+        if downsample == '':
+            downsample = DEFAULT_DOWNSAMPLE
+            break
+        try:
+            downsample = int(downsample)
+            if downsample < 1:
+                print("Downsample size must be a positive integer.")
+            else:
+                break
+        except ValueError:
+            print("Downsample size must be a positive integer.")
+
+    while True:
+        n_projs = input('Enter the number of projections (default {}): '.format(DEFAULT_N_PROJS))
+        if n_projs == '':
+            n_projs = DEFAULT_N_PROJS
+            break
+        try:
+            n_projs = int(n_projs)
+            if n_projs < 1:
+                print("Number of projections must be a positive integer.")
+            else:
+                break
+        except ValueError:
+            print("Number of projections must be a positive integer.")
+            
+    # Ask whether to lowpass filter input volumes
+    while True:
+        apply_filtering = input('Do you want to lowpass filter input volumes [y/n]')
+
+        if any(apply_filtering.lower() == f for f in ["yes", 'y', '1', 'ye']):
+            apply_filtering = True
+            break
+        elif any(apply_filtering.lower() == f for f in ['no', 'n', '0']):
+            apply_filtering = False
+            break
+        else:
+            print("Please choose y/n.")
+
+    # Ask to skip refinement of alignment parameters
+    while True:
+        no_refine = input('Do you want to refine alignment parameters [y/n]')
+
+        if any(no_refine.lower() == f for f in ["yes", 'y', '1', 'ye']):
+            no_refine = False
+            break
+        elif any(no_refine.lower() == f for f in ['no', 'n', '0']):
+            no_refine = True
+            break
+        else:
+            print("Please choose y/n.")
+            
+    # Check if user want to save parameters
+    while True:
+        save_params = input('Do you want to save output parameters [y/n]: ')
+        if save_params.lower().startswith('y'):
+            # If he does, ask for file
+            while True:
+                output_parameters = input('Enter full path of output parameters txt file: ')
+                if output_parameters[-4:] != '.txt':
+                    print('Please enter an txt file')
+                    continue
+                if os.path.isfile(output_parameters):
+                    break_flag = False
+                    while True:
+                        replace = str(input(
+                            'There is already a file with the name {}. Do you want to replace it [y/n]?: '.format(
+                                output_parameters)))
+                        if replace.lower().startswith('y'):
+                            break_flag = True
+                            break
+                        if replace.lower().startswith('n'):
+                            break
+                    if break_flag:
+                        break
+                break
+            break
+        if save_params.lower().startswith('n'):
+            output_parameters = None
+            break
+
+    verbose = 0
+    while verbose == 0:
+        verbose_in = input('Display detailed progress? [y/n]: ')
+        if verbose_in.strip().lower().startswith('y'):
+            verbose = 1
+        elif verbose_in.strip().lower().startswith('n'):
+            verbose = 0
+            break
+        else:
+            print("Please choose y/n.")
+
+    return vol1, vol2, output_vol, downsample, n_projs, apply_filtering,\
+        no_refine, output_parameters, verbose
+
+
+def check_for_newer_version():
+    """
+    This function checks whether there is a newer version of kltpicker
+    available on PyPI. If there is, it issues a warning.
+
+    """
+    name = 'EMalign'
+    # Use pip to try and install a version of kltpicker which does not exist.
+    # In answer, you get all available versions. Find the newest one.
+    latest_version = str(
+        subprocess.run([sys.executable, '-m', 'pip', 'install', '%s==random' % name], capture_output=True, text=True))
+    latest_version = latest_version[latest_version.find('(from versions:') + 15:]
+    latest_version = latest_version[:latest_version.find(')')]
+    latest_version = latest_version.replace(' ', '').split(',')[-1]
+
+    if latest_version == 'none':  # Got an unexpected response.
+        pass
+    else:  # Use pip to determine the installed version.
+        import pkg_resources  # part of setuptools
+        current_version = pkg_resources.require(name)[0].version
+        if latest_version > current_version:
+            print(
+                "NOTE: you are running an old version of %s (%s). A newer version (%s) is available, please upgrade." % (
+                    name, current_version, latest_version))
```

### Comparing `EMalign-1.0.3/src/fastrotate3d.py` & `EMalign-1.0.4/src/fastrotate3d.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,381 +1,381 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Wed May 26 11:11:19 2021
-
-@author: yaelharpaz1
-"""
-
-import numpy as np
-import math
-import cmath
-import scipy.spatial.transform
-import pyfftw
-
-class fftw_data_class:
-    def __init__(self, in_data, num_threads=1):
-        n = in_data.shape[0]
-        n2 = n//2 + 1
-        
-        if in_data.dtype == np.float32:
-            real_type = np.float32
-            complex_type = np.complex64
-        else:
-            real_type = np.float64
-            complex_type = np.complex128
-        
-        self.in_array_f_0 = pyfftw.empty_aligned((n,n), dtype=real_type)
-        self.out_array_f_0 = pyfftw.empty_aligned((n2,n), dtype=complex_type)
-        self.in_array_f_1 = pyfftw.empty_aligned((n,n), dtype=real_type)
-        self.out_array_f_1 = pyfftw.empty_aligned((n,n2), dtype=complex_type)
-        self.in_array_b_0 = pyfftw.empty_aligned((n2,n), dtype=complex_type)
-        self.out_array_b_0 = pyfftw.empty_aligned((n,n), dtype=real_type)
-        self.in_array_b_1 = pyfftw.empty_aligned((n,n2), dtype=complex_type)
-        self.out_array_b_1 = pyfftw.empty_aligned((n,n), dtype=real_type)
-        
-        self.fftw_object_0 = pyfftw.FFTW(self.in_array_f_0,
-                          self.out_array_f_0,
-                          direction="FFTW_FORWARD",
-                          flags=("FFTW_ESTIMATE", ),
-                          axes=(0,),
-                          threads=num_threads)
-
-        self.fftw_object_1 = pyfftw.FFTW(self.in_array_f_1,
-                          self.out_array_f_1,
-                          direction="FFTW_FORWARD",
-                          flags=("FFTW_ESTIMATE", ),
-                          axes=(1,),
-                          threads=num_threads)
-
-        
-        self.ifftw_object_0 = pyfftw.FFTW(self.in_array_b_0,
-                          self.out_array_b_0,
-                          direction="FFTW_BACKWARD",
-                          flags=("FFTW_ESTIMATE", ),
-                          axes=(0,),
-                          normalise_idft=True,
-                          threads=num_threads)
-        
-        self.ifftw_object_1 = pyfftw.FFTW(self.in_array_b_1,
-                          self.out_array_b_1,
-                          direction="FFTW_BACKWARD",
-                          flags=("FFTW_ESTIMATE", ),
-                          axes=(1,),
-                          normalise_idft=True,
-                          threads=num_threads)
-
-
-#%%
-def fastrotate3d(vol,Rot,fftw_data=None):
-    #FASTROTATE3D Rotate a 3D volume by a given rotation matrix.
-    # Input parameters:
-    #  INPUT    Volume to rotate, can be odd or even. 
-    #  Rot        3x3 rotation matrix.
-    # Output parameters:
-    #  OUTPUT   The rotated volume.
-    # Examples:
-    #   Rot=rand_rots(1);
-    #   rvol=fastrotate3d(vol,Rot);
-    #Yoel Shkolnisky, November 2013.
-    
-    if fftw_data is None:
-        fftw_data = fftw_data_class(vol)
-
-    Rot_obj = scipy.spatial.transform.Rotation.from_matrix(Rot)
-    [psi,theta,phi]  = Rot_obj.as_euler('xyz')
-
-    psid = psi*180/np.pi
-    thetad = theta*180/np.pi 
-    phid = phi*180/np.pi
-    
-    tmp = fastrotate3x(vol,psid,fftw_data)
-    tmp = fastrotate3y(tmp,thetad,fftw_data)
-    vol_out = fastrotate3z(tmp,phid,fftw_data)
-    return vol_out
-
-#%%
-def adjustrotate(phi):
-    # Decompose a rotation CCW by phi into a rotation of mult90 times 90
-    # degrees followed by a rotation by phi2, where phi2 is between -45 and 45.
-    # mult90 is an integer between 0 and 3 describing by how many multiples of
-    # 90 degrees the image should be rotated so that an additional rotation by
-    # phi2 is equivalent to rotation by phi.
-    
-    phi = np.mod(phi,360)
-    mult90 = 0
-    phi2 = phi   
-    # Note that any two consecutive cases can be combine, but I decided to
-    # leave them separated for clarity.
-    if phi >= 45 and phi < 90: mult90 = 1; phi2 = -(90-phi)
-    elif phi >= 90 and phi < 135: mult90 = 1; phi2 = phi-90     
-    elif phi >= 135 and phi < 180: mult90 = 2; phi2 = -(180-phi)
-    elif phi >= 180 and phi < 225: mult90 = 2; phi2 = phi-180
-    elif phi >= 215 and phi < 270: mult90 = 3; phi2 = -(270-phi)
-    elif phi >= 270 and phi < 315: mult90 = 3; phi2 = phi-270
-    elif phi >= 315 and phi < 360: mult90 = 0; phi2 = phi-360
-    return phi2, mult90    
-    
-#%%  
-def fastrotateprecomp(SzX,SzY,phi):
-    # Compute the interpolation tables required to rotate an image with SzX
-    # rows and SzY columns by an angle phi CCW.
-    #
-    # This function is used to accelerate fastrotate, in case many images are
-    # needed to be rotated by the same angle. In such a case it allows to
-    # precompute the interpolation tables only once instead of computing them
-    # for each image.
-    #
-    # M is a structure containing phi, Mx, My, where Mx and My are the
-    # interpolation tables used by fastrotate.
-    
-    # Adjust the rotation angle to be between -45 and 45 degrees.
-    [phi,mult90] = adjustrotate(phi)   
-    phi = np.pi*phi/180
-    phi = -phi # To match Yaroslavsky's code which rotates CW.    
-    if np.mod(SzY,2) == 0:
-        cy = SzY/2+1
-        sy = 1/2 # By how much should we shift the cy to get the center of the image
-    else:
-        cy = (SzY+1)/2
-        sy = 0    
-    if np.mod(SzX,2) == 0:
-        cx = SzX/2+1 # By how much should we shift the cy to get the center of the image
-        sx = 1/2
-    else: cx = (SzX+1)/2; sx = 0
-    # Precompte My and Mx:
-    My = np.zeros((SzY,SzX)).astype(complex)
-    r = np.arange(0,cy).astype(int)
-    u = (1-math.cos(phi))/math.sin(phi+2.2204e-16)
-    alpha1 = 2*np.pi*cmath.sqrt(-1)*(r)/SzY
-    for x in range(SzX):
-        Ux = u*(x+1-cx+sx)
-        My[r,x] = np.exp(alpha1*Ux)
-        My[np.arange(SzY-1,cy-1,-1).astype(int),x] = np.conj(My[np.arange(1,cy-2*sy).astype(int),x])
-    My = My.T # Remove when implementing using the loops below.  
-    Mx = np.zeros((SzX,SzY)).astype(complex)
-    r = np.arange(0,cx).astype(int)
-    u = -math.sin(phi)
-    alpha2 = 2*np.pi*cmath.sqrt(-1)*(r)/SzX
-    for y in range(SzY):
-        Uy = u*(y+1-cy+sy)
-        Mx[r,y] = np.exp(alpha2*Uy)
-        Mx[np.arange(SzX-1,cx-1,-1).astype(int),y] = np.conj(Mx[np.arange(1,cx-2*sx).astype(int),y])
-    class Struct:
-        pass
-    M = Struct() 
-    M.phi = phi
-    M.Mx = Mx
-    M.My = My
-    M.mult90 = mult90
-    return M
-
-#%%
-def fastrotate(im,phi,M=None, fftw_data=None):
-    # 3-step image rotation by shearing.
-    # 
-    # input parameters:
-    #  im      Image to rotate, can be odd or even. 2D array of size nxn.
-    #  phi      Rotation angle in degrees CCW. Can be any angle (not limited
-    #           like fastrotate_ref). Note that Yaroslavsky's code take phi CW.
-    #  M        (Optional) Precomputed interpolation tables, as generated by
-    #           fastrotateprecomp. If M is given than phi is ignored. This is
-    #           useful if many images need to be rotated by the same angle,
-    #           since then the computation of the same interpolation tables
-    #           over and over again is avoided.
-    # Output parameters:
-    #  im_out   The rotated image.
-    
-    if fftw_data is None:
-        fftw_data = fftw_data_class(im)
-    
-    im_out = im.copy()  # Create a copy of the input the prevent changing the 
-                      # calling object
-    SzX, SzY = im.shape
-
-    if M is None:
-        M = fastrotateprecomp(SzX,SzY,phi)
-    Mx = M.Mx
-    My = M.My 
-    mult90 = M.mult90
-
-    n = im.shape[0]
-    n2 = n//2 + 1
-    spinput_0 = np.zeros((n2,n),dtype=np.complex128)
-    spinput_1 = np.zeros((n,n2),dtype=np.complex128)
-    
-    
-    # Rotate by multiples of 90 degrees.
-    if mult90 == 1: im_out = rot90(im_out)  
-    elif mult90 == 2: im_out = rot180(im_out)
-    elif mult90 == 3: im_out = rot270(im_out)
-    elif mult90 != 0: TypeError('Invalid value for mult90')
-        
-    # Old code:
-    #spinput = fft(vol[:,:,k],n=None,axis=1)
-    #spinput = spinput*My
-    #vol_out[:,:,k] = np.real(ifft(spinput,n=None,axis=1))
-
-    fftw_data.in_array_f_1[:,:] = im_out
-    spinput_1[:,:] = fftw_data.fftw_object_1(fftw_data.in_array_f_1)
-    spinput_1 = spinput_1*My[:,0:n2]
-    fftw_data.in_array_b_1[:,:] = spinput_1[:,:]
-    im_out[:,:] = fftw_data.ifftw_object_1(fftw_data.in_array_b_1)
-        
-
-    # Old code:
-    #spinput = fft(vol_out[:,:,k],n=None,axis=0)
-    #spinput = spinput*Mx
-    #vol_out[:,:,k] = np.real(ifft(spinput,n=None,axis=0))
-
-    fftw_data.in_array_f_0[:,:] = im_out
-    spinput_0[:,:] = fftw_data.fftw_object_0(fftw_data.in_array_f_0)
-    spinput_0 = spinput_0*Mx[0:n2,:]
-    fftw_data.in_array_b_0[:,:] = spinput_0[:,:]
-    im_out[:,:] = fftw_data.ifftw_object_0(fftw_data.in_array_b_0)
-        
-                
-    # Old code:
-    #spinput = fft(vol_out[:,:,k],n=None,axis=1)
-    #spinput = spinput*My
-    #vol_out[:,:,k] = np.real(ifft(spinput,n=None,axis=1))
-    
-    fftw_data.in_array_f_1[:,:] = im_out
-    spinput_1[:,:] = fftw_data.fftw_object_1(fftw_data.in_array_f_1)
-    spinput_1 = spinput_1*My[:,0:n2]
-    fftw_data.in_array_b_1[:,:] = spinput_1[:,:]
-    im_out[:,:] = fftw_data.ifftw_object_1(fftw_data.in_array_b_1)
-        
-    return im_out 
-   
-#%%
-def rot90(A):
-    # Rotate the image A by 90 degrees CCW.
-    #   B = rot90(A)
-    B = A.T
-    B = np.flip(B,0)
-    return B
-
-#%%
-def rot180(A):
-    # Rotate the image A by 180 degrees CCW.
-    #   B = rot180(A) 
-    B = np.flip(A,0)
-    B = np.flip(B,1)
-    return B
-
-#%% 
-def rot270(A):
-    # Rotate the image A by 270 degrees CCW.
-    #   B = rot270(A)
-    
-    B = A.T
-    B = np.flip(B,1)
-    return B
-
-#%%
-def fastrotate3x(vol,phi,fftw_data=None):
-    #FASTROTATE3X Rotate a 3D volume around the x-axis.
-    # Input parameters:
-    #  INPUT    Volume to rotate, can be odd or even. 
-    #  phi      Rotation angle in degrees CCW. 
-    #  M        (Optional) Precomputed interpolation tables, as generated by
-    #           fastrotateprecomp. If M is given than phi is ignored. 
-    #
-    # Output parameters:
-    #  OUTPUT   The rotated volume.
-    #
-    # Examples:
-    #
-    #   rvol=fastrotate3x(vol,20);
-    #
-    #   M=fastrotateprecomp(size(vol,2),size(vol,3),20);
-    #   rvol=fastrotate(vol,[],M);
-
-    if fftw_data is None:
-        fftw_data = fftw_data_class(vol)
-
-    SzX = np.size(vol,0); SzY = np.size(vol,1); SzZ = np.size(vol,2)  
-    # Precompte M
-    M = fastrotateprecomp(SzY,SzZ,phi)    
-    vol_out = np.zeros((SzX,SzY,SzZ),dtype=float)
-    for k in range(SzX):
-        im = vol[:,k,:]
-        rim = fastrotate(im,[],M,fftw_data)
-        vol_out[:,k,:] = rim
-    return vol_out
-
-#%%
-def fastrotate3y(vol,phi,fftw_data=None):
-    #FASTROTATE3X Rotate a 3D volume around the x-axis.
-    # Input parameters:
-    #  INPUT    Volume to rotate, can be odd or even. 
-    #  phi      Rotation angle in degrees CCW. 
-    #  M        (Optional) Precomputed interpolation tables, as generated by
-    #           fastrotateprecomp. If M is given than phi is ignored. 
-    #
-    # Output parameters:
-    #  OUTPUT   The rotated volume.
-    #
-    # Examples:
-    #
-    #   rvol=fastrotate3x(vol,20);
-    #
-    #   M=fastrotateprecomp(size(vol,2),size(vol,3),20);
-    #   rvol=fastrotate(vol,[],M);
-
-    if fftw_data is None:
-        fftw_data = fftw_data_class(vol)
-
-    SzX = np.size(vol,0); SzY = np.size(vol,1); SzZ = np.size(vol,2)
-    # Precompte M
-    M = fastrotateprecomp(SzX,SzY,-phi)
-    vol_out = np.zeros((SzX,SzY,SzZ),dtype=float)
-    for k in range(SzY):
-        im = vol[k,:,:]
-        rim = fastrotate(im,[],M,fftw_data)
-        vol_out[k,:,:] = rim
-    return vol_out
-
-#%%
-def fastrotate3z(vol,phi,fftw_data=None):
-    #FASTROTATE3X Rotate a 3D volume around the x-axis.
-    # Input parameters:
-    #  INPUT    Volume to rotate, can be odd or even. 
-    #  phi      Rotation angle in degrees CCW. 
-    #  M        (Optional) Precomputed interpolation tables, as generated by
-    #           fastrotateprecomp. If M is given than phi is ignored. 
-    #
-    # Output parameters:
-    #  OUTPUT   The rotated volume.
-    #
-    # Examples:
-    #
-    #   rvol=fastrotate3x(vol,20);
-    #
-    #   M=fastrotateprecomp(size(vol,2),size(vol,3),20);
-    #   rvol=fastrotate(vol,[],M);
-    
-    if fftw_data is None:
-        fftw_data = fftw_data_class(vol)
-    
-    SzX = np.size(vol,0); SzY = np.size(vol,1); SzZ = np.size(vol,2)    
-    # Precompte M
-    M = fastrotateprecomp(SzX,SzY,-phi)    
-    vol_out = np.zeros((SzX,SzY,SzZ),dtype=float)
-    for k in range(SzZ):
-        im = vol[:,:,k]
-        rim = fastrotate(im,[],M,fftw_data)
-        vol_out[:,:,k] = rim
-    return vol_out
-
-#import scipy.io as matio
-#mat_vars = matio.loadmat("../mattemp.mat")
-#vol = mat_vars["vol"]
-#R = mat_vars["R"]
-#vol_rot = fastrotate3d(vol, R)
-#print(np.linalg.norm(vol_rot - mat_vars["vol_rot"])/np.linalg.norm(vol_rot))
-#vol_rot = fastrotate3d(vol, R)
-#print(np.linalg.norm(vol_rot - mat_vars["vol_rot"])/np.linalg.norm(vol_rot))
-#vol2 = fastrotate3d(vol_rot,R.transpose())
-#np.corrcoef(vol2.ravel(),vol.ravel())
-#aaa = 1
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Wed May 26 11:11:19 2021
+
+@author: yaelharpaz1
+"""
+
+import numpy as np
+import math
+import cmath
+import scipy.spatial.transform
+import pyfftw
+
+class fftw_data_class:
+    def __init__(self, in_data, num_threads=1):
+        n = in_data.shape[0]
+        n2 = n//2 + 1
+        
+        if in_data.dtype == np.float32:
+            real_type = np.float32
+            complex_type = np.complex64
+        else:
+            real_type = np.float64
+            complex_type = np.complex128
+        
+        self.in_array_f_0 = pyfftw.empty_aligned((n,n), dtype=real_type)
+        self.out_array_f_0 = pyfftw.empty_aligned((n2,n), dtype=complex_type)
+        self.in_array_f_1 = pyfftw.empty_aligned((n,n), dtype=real_type)
+        self.out_array_f_1 = pyfftw.empty_aligned((n,n2), dtype=complex_type)
+        self.in_array_b_0 = pyfftw.empty_aligned((n2,n), dtype=complex_type)
+        self.out_array_b_0 = pyfftw.empty_aligned((n,n), dtype=real_type)
+        self.in_array_b_1 = pyfftw.empty_aligned((n,n2), dtype=complex_type)
+        self.out_array_b_1 = pyfftw.empty_aligned((n,n), dtype=real_type)
+        
+        self.fftw_object_0 = pyfftw.FFTW(self.in_array_f_0,
+                          self.out_array_f_0,
+                          direction="FFTW_FORWARD",
+                          flags=("FFTW_ESTIMATE", ),
+                          axes=(0,),
+                          threads=num_threads)
+
+        self.fftw_object_1 = pyfftw.FFTW(self.in_array_f_1,
+                          self.out_array_f_1,
+                          direction="FFTW_FORWARD",
+                          flags=("FFTW_ESTIMATE", ),
+                          axes=(1,),
+                          threads=num_threads)
+
+        
+        self.ifftw_object_0 = pyfftw.FFTW(self.in_array_b_0,
+                          self.out_array_b_0,
+                          direction="FFTW_BACKWARD",
+                          flags=("FFTW_ESTIMATE", ),
+                          axes=(0,),
+                          normalise_idft=True,
+                          threads=num_threads)
+        
+        self.ifftw_object_1 = pyfftw.FFTW(self.in_array_b_1,
+                          self.out_array_b_1,
+                          direction="FFTW_BACKWARD",
+                          flags=("FFTW_ESTIMATE", ),
+                          axes=(1,),
+                          normalise_idft=True,
+                          threads=num_threads)
+
+
+#%%
+def fastrotate3d(vol,Rot,fftw_data=None):
+    #FASTROTATE3D Rotate a 3D volume by a given rotation matrix.
+    # Input parameters:
+    #  INPUT    Volume to rotate, can be odd or even. 
+    #  Rot        3x3 rotation matrix.
+    # Output parameters:
+    #  OUTPUT   The rotated volume.
+    # Examples:
+    #   Rot=rand_rots(1);
+    #   rvol=fastrotate3d(vol,Rot);
+    #Yoel Shkolnisky, November 2013.
+    
+    if fftw_data is None:
+        fftw_data = fftw_data_class(vol)
+
+    Rot_obj = scipy.spatial.transform.Rotation.from_matrix(Rot)
+    [psi,theta,phi]  = Rot_obj.as_euler('xyz')
+
+    psid = psi*180/np.pi
+    thetad = theta*180/np.pi 
+    phid = phi*180/np.pi
+    
+    tmp = fastrotate3x(vol,psid,fftw_data)
+    tmp = fastrotate3y(tmp,thetad,fftw_data)
+    vol_out = fastrotate3z(tmp,phid,fftw_data)
+    return vol_out
+
+#%%
+def adjustrotate(phi):
+    # Decompose a rotation CCW by phi into a rotation of mult90 times 90
+    # degrees followed by a rotation by phi2, where phi2 is between -45 and 45.
+    # mult90 is an integer between 0 and 3 describing by how many multiples of
+    # 90 degrees the image should be rotated so that an additional rotation by
+    # phi2 is equivalent to rotation by phi.
+    
+    phi = np.mod(phi,360)
+    mult90 = 0
+    phi2 = phi   
+    # Note that any two consecutive cases can be combine, but I decided to
+    # leave them separated for clarity.
+    if phi >= 45 and phi < 90: mult90 = 1; phi2 = -(90-phi)
+    elif phi >= 90 and phi < 135: mult90 = 1; phi2 = phi-90     
+    elif phi >= 135 and phi < 180: mult90 = 2; phi2 = -(180-phi)
+    elif phi >= 180 and phi < 225: mult90 = 2; phi2 = phi-180
+    elif phi >= 215 and phi < 270: mult90 = 3; phi2 = -(270-phi)
+    elif phi >= 270 and phi < 315: mult90 = 3; phi2 = phi-270
+    elif phi >= 315 and phi < 360: mult90 = 0; phi2 = phi-360
+    return phi2, mult90    
+    
+#%%  
+def fastrotateprecomp(SzX,SzY,phi):
+    # Compute the interpolation tables required to rotate an image with SzX
+    # rows and SzY columns by an angle phi CCW.
+    #
+    # This function is used to accelerate fastrotate, in case many images are
+    # needed to be rotated by the same angle. In such a case it allows to
+    # precompute the interpolation tables only once instead of computing them
+    # for each image.
+    #
+    # M is a structure containing phi, Mx, My, where Mx and My are the
+    # interpolation tables used by fastrotate.
+    
+    # Adjust the rotation angle to be between -45 and 45 degrees.
+    [phi,mult90] = adjustrotate(phi)   
+    phi = np.pi*phi/180
+    phi = -phi # To match Yaroslavsky's code which rotates CW.    
+    if np.mod(SzY,2) == 0:
+        cy = SzY/2+1
+        sy = 1/2 # By how much should we shift the cy to get the center of the image
+    else:
+        cy = (SzY+1)/2
+        sy = 0    
+    if np.mod(SzX,2) == 0:
+        cx = SzX/2+1 # By how much should we shift the cy to get the center of the image
+        sx = 1/2
+    else: cx = (SzX+1)/2; sx = 0
+    # Precompte My and Mx:
+    My = np.zeros((SzY,SzX)).astype(complex)
+    r = np.arange(0,cy).astype(int)
+    u = (1-math.cos(phi))/math.sin(phi+2.2204e-16)
+    alpha1 = 2*np.pi*cmath.sqrt(-1)*(r)/SzY
+    for x in range(SzX):
+        Ux = u*(x+1-cx+sx)
+        My[r,x] = np.exp(alpha1*Ux)
+        My[np.arange(SzY-1,cy-1,-1).astype(int),x] = np.conj(My[np.arange(1,cy-2*sy).astype(int),x])
+    My = My.T # Remove when implementing using the loops below.  
+    Mx = np.zeros((SzX,SzY)).astype(complex)
+    r = np.arange(0,cx).astype(int)
+    u = -math.sin(phi)
+    alpha2 = 2*np.pi*cmath.sqrt(-1)*(r)/SzX
+    for y in range(SzY):
+        Uy = u*(y+1-cy+sy)
+        Mx[r,y] = np.exp(alpha2*Uy)
+        Mx[np.arange(SzX-1,cx-1,-1).astype(int),y] = np.conj(Mx[np.arange(1,cx-2*sx).astype(int),y])
+    class Struct:
+        pass
+    M = Struct() 
+    M.phi = phi
+    M.Mx = Mx
+    M.My = My
+    M.mult90 = mult90
+    return M
+
+#%%
+def fastrotate(im,phi,M=None, fftw_data=None):
+    # 3-step image rotation by shearing.
+    # 
+    # input parameters:
+    #  im      Image to rotate, can be odd or even. 2D array of size nxn.
+    #  phi      Rotation angle in degrees CCW. Can be any angle (not limited
+    #           like fastrotate_ref). Note that Yaroslavsky's code take phi CW.
+    #  M        (Optional) Precomputed interpolation tables, as generated by
+    #           fastrotateprecomp. If M is given than phi is ignored. This is
+    #           useful if many images need to be rotated by the same angle,
+    #           since then the computation of the same interpolation tables
+    #           over and over again is avoided.
+    # Output parameters:
+    #  im_out   The rotated image.
+    
+    if fftw_data is None:
+        fftw_data = fftw_data_class(im)
+    
+    im_out = im.copy()  # Create a copy of the input the prevent changing the 
+                      # calling object
+    SzX, SzY = im.shape
+
+    if M is None:
+        M = fastrotateprecomp(SzX,SzY,phi)
+    Mx = M.Mx
+    My = M.My 
+    mult90 = M.mult90
+
+    n = im.shape[0]
+    n2 = n//2 + 1
+    spinput_0 = np.zeros((n2,n),dtype=np.complex128)
+    spinput_1 = np.zeros((n,n2),dtype=np.complex128)
+    
+    
+    # Rotate by multiples of 90 degrees.
+    if mult90 == 1: im_out = rot90(im_out)  
+    elif mult90 == 2: im_out = rot180(im_out)
+    elif mult90 == 3: im_out = rot270(im_out)
+    elif mult90 != 0: TypeError('Invalid value for mult90')
+        
+    # Old code:
+    #spinput = fft(vol[:,:,k],n=None,axis=1)
+    #spinput = spinput*My
+    #vol_out[:,:,k] = np.real(ifft(spinput,n=None,axis=1))
+
+    fftw_data.in_array_f_1[:,:] = im_out
+    spinput_1[:,:] = fftw_data.fftw_object_1(fftw_data.in_array_f_1)
+    spinput_1 = spinput_1*My[:,0:n2]
+    fftw_data.in_array_b_1[:,:] = spinput_1[:,:]
+    im_out[:,:] = fftw_data.ifftw_object_1(fftw_data.in_array_b_1)
+        
+
+    # Old code:
+    #spinput = fft(vol_out[:,:,k],n=None,axis=0)
+    #spinput = spinput*Mx
+    #vol_out[:,:,k] = np.real(ifft(spinput,n=None,axis=0))
+
+    fftw_data.in_array_f_0[:,:] = im_out
+    spinput_0[:,:] = fftw_data.fftw_object_0(fftw_data.in_array_f_0)
+    spinput_0 = spinput_0*Mx[0:n2,:]
+    fftw_data.in_array_b_0[:,:] = spinput_0[:,:]
+    im_out[:,:] = fftw_data.ifftw_object_0(fftw_data.in_array_b_0)
+        
+                
+    # Old code:
+    #spinput = fft(vol_out[:,:,k],n=None,axis=1)
+    #spinput = spinput*My
+    #vol_out[:,:,k] = np.real(ifft(spinput,n=None,axis=1))
+    
+    fftw_data.in_array_f_1[:,:] = im_out
+    spinput_1[:,:] = fftw_data.fftw_object_1(fftw_data.in_array_f_1)
+    spinput_1 = spinput_1*My[:,0:n2]
+    fftw_data.in_array_b_1[:,:] = spinput_1[:,:]
+    im_out[:,:] = fftw_data.ifftw_object_1(fftw_data.in_array_b_1)
+        
+    return im_out 
+   
+#%%
+def rot90(A):
+    # Rotate the image A by 90 degrees CCW.
+    #   B = rot90(A)
+    B = A.T
+    B = np.flip(B,0)
+    return B
+
+#%%
+def rot180(A):
+    # Rotate the image A by 180 degrees CCW.
+    #   B = rot180(A) 
+    B = np.flip(A,0)
+    B = np.flip(B,1)
+    return B
+
+#%% 
+def rot270(A):
+    # Rotate the image A by 270 degrees CCW.
+    #   B = rot270(A)
+    
+    B = A.T
+    B = np.flip(B,1)
+    return B
+
+#%%
+def fastrotate3x(vol,phi,fftw_data=None):
+    #FASTROTATE3X Rotate a 3D volume around the x-axis.
+    # Input parameters:
+    #  INPUT    Volume to rotate, can be odd or even. 
+    #  phi      Rotation angle in degrees CCW. 
+    #  M        (Optional) Precomputed interpolation tables, as generated by
+    #           fastrotateprecomp. If M is given than phi is ignored. 
+    #
+    # Output parameters:
+    #  OUTPUT   The rotated volume.
+    #
+    # Examples:
+    #
+    #   rvol=fastrotate3x(vol,20);
+    #
+    #   M=fastrotateprecomp(size(vol,2),size(vol,3),20);
+    #   rvol=fastrotate(vol,[],M);
+
+    if fftw_data is None:
+        fftw_data = fftw_data_class(vol)
+
+    SzX = np.size(vol,0); SzY = np.size(vol,1); SzZ = np.size(vol,2)  
+    # Precompte M
+    M = fastrotateprecomp(SzY,SzZ,phi)    
+    vol_out = np.zeros((SzX,SzY,SzZ),dtype=float)
+    for k in range(SzX):
+        im = vol[:,k,:]
+        rim = fastrotate(im,[],M,fftw_data)
+        vol_out[:,k,:] = rim
+    return vol_out
+
+#%%
+def fastrotate3y(vol,phi,fftw_data=None):
+    #FASTROTATE3X Rotate a 3D volume around the x-axis.
+    # Input parameters:
+    #  INPUT    Volume to rotate, can be odd or even. 
+    #  phi      Rotation angle in degrees CCW. 
+    #  M        (Optional) Precomputed interpolation tables, as generated by
+    #           fastrotateprecomp. If M is given than phi is ignored. 
+    #
+    # Output parameters:
+    #  OUTPUT   The rotated volume.
+    #
+    # Examples:
+    #
+    #   rvol=fastrotate3x(vol,20);
+    #
+    #   M=fastrotateprecomp(size(vol,2),size(vol,3),20);
+    #   rvol=fastrotate(vol,[],M);
+
+    if fftw_data is None:
+        fftw_data = fftw_data_class(vol)
+
+    SzX = np.size(vol,0); SzY = np.size(vol,1); SzZ = np.size(vol,2)
+    # Precompte M
+    M = fastrotateprecomp(SzX,SzY,-phi)
+    vol_out = np.zeros((SzX,SzY,SzZ),dtype=float)
+    for k in range(SzY):
+        im = vol[k,:,:]
+        rim = fastrotate(im,[],M,fftw_data)
+        vol_out[k,:,:] = rim
+    return vol_out
+
+#%%
+def fastrotate3z(vol,phi,fftw_data=None):
+    #FASTROTATE3X Rotate a 3D volume around the x-axis.
+    # Input parameters:
+    #  INPUT    Volume to rotate, can be odd or even. 
+    #  phi      Rotation angle in degrees CCW. 
+    #  M        (Optional) Precomputed interpolation tables, as generated by
+    #           fastrotateprecomp. If M is given than phi is ignored. 
+    #
+    # Output parameters:
+    #  OUTPUT   The rotated volume.
+    #
+    # Examples:
+    #
+    #   rvol=fastrotate3x(vol,20);
+    #
+    #   M=fastrotateprecomp(size(vol,2),size(vol,3),20);
+    #   rvol=fastrotate(vol,[],M);
+    
+    if fftw_data is None:
+        fftw_data = fftw_data_class(vol)
+    
+    SzX = np.size(vol,0); SzY = np.size(vol,1); SzZ = np.size(vol,2)    
+    # Precompte M
+    M = fastrotateprecomp(SzX,SzY,-phi)    
+    vol_out = np.zeros((SzX,SzY,SzZ),dtype=float)
+    for k in range(SzZ):
+        im = vol[:,:,k]
+        rim = fastrotate(im,[],M,fftw_data)
+        vol_out[:,:,k] = rim
+    return vol_out
+
+#import scipy.io as matio
+#mat_vars = matio.loadmat("../mattemp.mat")
+#vol = mat_vars["vol"]
+#R = mat_vars["R"]
+#vol_rot = fastrotate3d(vol, R)
+#print(np.linalg.norm(vol_rot - mat_vars["vol_rot"])/np.linalg.norm(vol_rot))
+#vol_rot = fastrotate3d(vol, R)
+#print(np.linalg.norm(vol_rot - mat_vars["vol_rot"])/np.linalg.norm(vol_rot))
+#vol2 = fastrotate3d(vol_rot,R.transpose())
+#np.corrcoef(vol2.ravel(),vol.ravel())
+#aaa = 1
```

### Comparing `EMalign-1.0.3/src/fsc.py` & `EMalign-1.0.4/src/fsc.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,470 +1,470 @@
-"""
-Created on Sun Sep 25 21:49:00 2022
-
-@author: yoel shkolnisky
-"""
-import numpy as np
-import matplotlib.pyplot as plt
-import scipy.interpolate as interp
-    
-def ndgrid (*xi):
-    '''
-    Implementation of MATLAB's ndgrid function.
-    Similar to meshgrid by with a different output ordering
-    
-    Parameters
-    ----------
-    *xi : x1, x2,...,xn: array_like
-        1-D arrays representing the coordinates of a grid.
-
-    Returns
-    -------
-    
-    X1, X2,...,xn ndarray
-    ndgrid(x1,x2,...,xn) replicates the grid vectors x1,x2,...,xn to produce 
-    an n-dimensional full grid.
-    '''
-
-    return np.meshgrid(*xi, indexing='ij')
-
-
-def FSCorr(m1,m2): 
-    '''
-    Compute the fourier shell correlation between the 3D maps m1 and m2,
-    which must be n x n x n in size with the same n, assumed to be even.
-    
-    The FSC is defined as
-                sum{F1 .* conj(F2)}
-    c(i) = -----------------------------
-           sqrt(sum|F1|^2 * sum|F2|^2)
-    where F1 and F2 are the Fourier components at the given spatial 
-    frequency i. i ranges from 1 to n/2-1, times the unit frequency 1/(n*res) 
-    where res is the pixel size.
-    
-    Examples:
-    --------
-    c=FSCorr(m1,m2)
-    
-    Parameters
-    ----------
-    m1,m2 : ndarray
-        n x n x n array. n assumed to be even
-
-    Returns
-    -------
-    c : 1-D vector with Fourier shell correlation coefficients computed as 
-    described above. 
-    
-    '''
-    
-    # First, construct the radius values for defining the shells.
-    n,n1,n2 = m1.shape
-    ctr = (n + 1) / 2
-    origin = np.transpose(np.array([ctr,ctr,ctr]))
-
-    x,y,z = ndgrid(np.arange(1 - origin[0],n - origin[0]+1),np.arange(1 - origin[1],n - origin[1]+1),np.arange(1 - origin[2],n - origin[2]+1))
-    R = np.sqrt(x ** 2 + y ** 2 + z ** 2)
-    eps = 0.0001
-
-    # Fourier-transform the maps
-    f1 = np.fft.fftshift(np.fft.fftn(m1))
-    f2 = np.fft.fftshift(np.fft.fftn(m2))
-
-    # Perform the sums
-    d0 = R < 0.5 + eps
-    c = np.zeros((int(np.floor(n / 2)),1))
-    
-    for i in np.arange(1,int(np.floor(n / 2)+1)).reshape(-1):
-        d1 = R < 0.5 + i + eps
-        ring = np.logical_xor(d1,d0)
-        #r1 = np.multiply(ring,f1)
-        #r2 = np.multiply(ring,f2)
-        #num = np.real(sum(sum(sum(np.multiply(r1,np.conjugate(r2))))))
-        #den = np.sqrt(sum(sum(sum(np.abs(r1) ** 2))) * sum(sum(sum(np.abs(r2) ** 2))))
-        
-        r1 = f1[ring]
-        r2 = f2[ring]
-        num = np.real(sum(np.multiply(r1,np.conjugate(r2))))
-        den = np.sqrt(sum(np.abs(r1) ** 2) * sum(np.abs(r2) ** 2))
-            
-        c[i-1] = num / den
-        d0 = d1
-    
-    return c
-    
-    
-def fscres(fsc,cutoff):
-    '''
-    Find the resolution from an FSC curve.
-    r=fscres(fsc,cutoff)    determines the index of the last bin of the
-    given fsc curve that is above the the given cutoff. Intermediate values
-    of the FSC curve are estimated using interpolation.
-
-    Parameters
-    ----------
-    fsc : 1-D array
-        Fourier shell correlation coefficients, computed using FSCorr
-    cutoff : float
-        Cutoff value to determine resolution. 
-
-    Returns
-    -------
-    r : double
-        Estimated resolution
-        
-    '''
-    
-    n = np.asarray(fsc).size
-    r = n
-    x = np.arange(1,n+1)
-    xx = np.arange(1,n+0.01,0.01)
-    fsc_interp = interp.PchipInterpolator(x,fsc)
-    y = fsc_interp(xx)
-    ii = next((i for i, val in enumerate(y) if val < cutoff),-1)
-
-    if ii != -1 :
-        r = xx[ii]
-
-    return r
-    
-def plotFSC(vol1, vol2 ,cutoff = 0.143, pixelsize = 1.0): 
-    '''
-    Draw Fourier shell correlation curve and estimated resolution.
-
-    plotFSC(vol1,vol2,cutoff,pixelsize)
-    Draw the Fourier shell correlation curve for the volumes vol1 and vol2,
-    and determine the resolution according the the given cutoff and
-    pixelsize. The volumes vol1 and vol2 must be aligned.
-    
-    Example
-    -------
-    vol1 = mrcfile.open('map_ref.mrc')
-    vol2 = mrcfile.open('map_aligned.mrc')
-    cutoff=0.143
-    resA, fig = plotFSC(vol1.data,vol2.data,cutoff,1.5)
-
-
-    Algorithm
-    ---------
-    The resolution resA is determined as follows.
-    # The derivation is given in 1-D, but it is the same for 3D, if the three
-    dimesions of the volume are equal.
-    Denote
-    B   bandwidth of the signal
-    fs  Maximal frequnecy
-    T   Sampling rate (pixel size)
-    N   Length of the signal
-    j   The index of the last frequnecy bin where the correlation is above
-    the cutoff value.
-    
-    1. The bandwidth B is given by B=2*fs, as the signal has frequencies
-    in the range [-fs,fs].
-    2. According to the Nyquist criterion, the samping frequency 1/T must
-    satisfy 1/T>=B. The critical sampling rate is 1/T=B=2*fs.
-    3. The width of each frequnecy bin is B/N=2*fs/N.
-    4. The frequnecy of the bin at index j is fc=2*fs*j/N.
-    5. The resolution is defined as resA=1/fc=N/(2*fs*j).
-    Due to 2 above, resA=N*T/j.
-    6. FSCorr returns correlation values only for positive freqnecuies,
-    that is is returns the correlation at n frequnecies such that N=2*n
-    (it assumes that N is even). Thus, in terms n, resA is given by
-    resA = 2*n*T/j = (2*T)*(n/j).
-    
-    Parameters
-    ----------
-    vol1, vol2 : ndarray
-        3-D arrays of the same dimensions. Volumes must be aligned.
-    cutoff : float, optional
-        Correlation cutoff threshold to determine resolution. The resolution 
-        is determined by the first frequnecy where the correlation goes below 
-        this value. Common values are 0.143 and 0.5. The default is 0.143.
-    pixelsize : float, optional
-        Pixel size of the volumes. The default is 1.0A.
-
-    Returns
-    -------
-    resA : float
-    Resolution of the structure in Angstrom according to the given cutoff 
-    value.
-    
-    fig :  matplotlib.figure.Figure
-    Handle to the FSC curve plot.
-
-    '''
-    
-    fsc = FSCorr(vol1,vol2)
-    n = np.asarray(fsc).size
-    
-    fig, ax = plt.subplots(constrained_layout=True)
-    ax.grid(visible = True, axis = 'both')
-    ax.plot(np.arange(1,n+1),fsc,'-g', linewidth = 2.0)
-    
-    plt.xlim(np.array([1,n]))
-    plt.ylim(np.array([- 0.1,1.05]))
-    
-    # Plot cutoff line
-    y = np.ones((n)) * cutoff
-    ax.plot(np.arange(1,n+1),y, color='b', linestyle='--', linewidth=1.5)
-    
-    # Compute resolution - fscres return the bin number where the cutoff
-    # resolution is obtained.    
-    j = fscres(fsc,cutoff)
-    resA = 2 * pixelsize * n / j
-        
-    yy = ax.get_ylim()
-    ax.vlines(j,0,yy[1], colors='b', linestyles='dashed') 
-
-    # Replace the default ticks with frequnecy values   
-    xticks_locs = ax.get_xticks()    
-    df = 1.0 / (2.0 * pixelsize * n)
-    xticks = xticks_locs * df
-    
-    xticks_labels = []
-    for e in xticks:
-        xticks_labels.append('{0:7.3f}'.format(e))
-    ax.set_xticks(xticks_locs,xticks_labels)        
-    ax.set_xlabel('1/A')
-    
-    # Add top axis
-    ax2 = ax.twiny()
-    xticks_locs = ax.get_xticks()   
-    xticks_labels = []
-    for e in xticks:
-        if e > 0:
-            xticks_labels.append('{0:7.3f}'.format(1/e))
-        else:
-            xticks_labels.append(' ')
-                        
-    ax2.set_xticks(xticks_locs,xticks_labels)        
-    ax2.set_xlabel('A')
-       
-    plt.title('Resolution={0:5.2f}A'.format(resA))
-    plt.show()
-
-    return resA, fig    
-
-
-def plotFSC2(vol1a, vol2a , vol1b, vol2b, labels=None, 
-             cutoff = 0.143, pixelsize = 1.0, figname=None): 
-    '''
-    Draw Fourier shell correlation curve and estimate resolution.
-    
-    Use this function to plot the Fourier shell correlations of two pairs on 
-    volumes on the same axis. This can be used to compare the quality of two
-    reconstructions. 
-    
-    Specifically, draw the Fourier shell correlation curve for the pairs of 
-    volumes (vol1a,vol2a) and (vol1b, vol2b), and determine the resolution of 
-    each pair according the the given cutoff and pixelsize. Each pair of 
-    volumes must be aligned.
-    
-    Use the given cutoff value for determining resolution. Common values
-    for cutoff are 0.143 and 0.5.  The resolution is determined by the 
-    first frequnecy where the correlation goes below this value.
-
-    Example
-    -------
-    vol1a=ReadMRC('./vol1a.mrc');
-    vol2a=ReadMRC('./vol2a.mrc');
-    vol1b=ReadMRC('./vol1b.mrc');
-    vol2b=ReadMRC('./vol2b.mrc');
-    cutoff=0.143;
-    resA=plotFSC(vol1a.data,vol2a.data,vol1b.data,vol2b.data,cutoff,1.5); 
-
-
-    Parameters
-    ----------
-    vol1a, vol2a, vol1b, vol2b : ndarray
-        3-D arrays of the same dimensions. Volumes must be aligned.
-    cutoff : float, optional
-        Correlation cutoff threshold to determine resolution. The resolution 
-        is determined by the first frequnecy where the correlation goes below 
-        this value. Common values are 0.143 and 0.5. The default is 0.143.
-    pixelsize : float, optional
-        Pixel size of the volumes. The default is 1.0A.
-    figname: string, optional
-        If not None, the FSC plot would be saved to a file with this name.
-
-    Returns
-    -------
-    resAa : float
-        Estimated resolution of vol1a and vol2a
-    resAb : float
-        Estimated resolution of vol1b and vol2b
-    fig :  matplotlib.figure.Figure
-        Handle to the FSC curve plot.
-        
-        
-    See plotFSC for more details.
-
-    '''
-
-    sz1a = vol1a.shape
-    sz2a = vol2a.shape
-    sz1b = vol1b.shape
-    sz2b = vol2b.shape
-    
-    if (sz1a != sz2a) or (sz1a != sz1b) or (sz1a != sz2b):
-        raise ValueError('Dimensions of all input volumes must be the same')
-
-    if (labels is not None) and (len(labels)!=2) :
-        raise ValueError('labels must contain two labels')
-
-    fsc_a = FSCorr(vol1a,vol2a)
-    n = np.asarray(fsc_a).size
-    fsc_b = FSCorr(vol1b,vol2b)
-    
-    fig, ax = plt.subplots(constrained_layout=True)
-    ax.grid(visible = True, axis = 'both')
-    ax.plot(np.arange(1,n+1),fsc_a,'-g', linewidth = 2.0)
-    ax.plot(np.arange(1,n+1),fsc_b,'-r', linewidth = 2.0)
-    
-    plt.xlim(np.array([1,n]))
-    plt.ylim(np.array([- 0.1,1.05]))
-    
-    # Plot cutoff line
-    y = np.ones((n)) * cutoff
-    ax.plot(np.arange(1,n+1),y, color='b', linestyle='--', linewidth=1.5)
-    
-    # Compute resolution - fscres return the bin number where the cutoff
-    # resolution is obtained.    
-    j_a = fscres(fsc_a,cutoff)
-    resAa = 2 * pixelsize * n / j_a
-    j_b = fscres(fsc_b,cutoff)
-    resAb = 2 * pixelsize * n / j_b
-        
-    yy = ax.get_ylim()
-    ax.vlines(j_a,0,yy[1], colors='b', linestyles='dashed') 
-    ax.vlines(j_b,0,yy[1], colors='b', linestyles='dashed') 
-
-    # Replace the default ticks with frequnecy values   
-    xticks_locs = ax.get_xticks()    
-    df = 1.0 / (2.0 * pixelsize * n)
-    xticks = xticks_locs * df
-    
-    xticks_labels = []
-    for e in xticks:
-        xticks_labels.append('{0:7.3f}'.format(e))
-    ax.set_xticks(xticks_locs,xticks_labels)        
-    ax.set_xlabel('1/A')
-    
-    # Add top axis
-    ax2 = ax.twiny()
-    xticks_locs = ax.get_xticks()   
-    xticks_labels = []
-    for e in xticks:
-        if e > 0:
-            xticks_labels.append('{0:7.3f}'.format(1/e))
-        else:
-            xticks_labels.append(' ')
-                        
-    ax2.set_xticks(xticks_locs,xticks_labels)        
-    ax2.set_xlabel('A')
-           
-    if labels is None:      
-        ax.legend(['{0:5.2f}A'.format(resAa), '{0:5.2f}A'.format(resAb)])
-    else:
-        ax.legend([labels[0]+' {0:5.2f}A'.format(resAa), 
-                   labels[1]+' {0:5.2f}A'.format(resAb)])
-
-    fig1 = plt.gcf()
-    plt.show()
-    plt.draw()
-
-    if figname is not None:
-        fig1.savefig(figname, dpi = 300)
-
-    return resAa, resAb, fig    
-
-
-def plotFSC3(vol1a, vol2a , vol1b, vol2b, vol1c, vol2c, labels=None,
-             cutoff = 0.143, pixelsize = 1.0, figname=None): 
-    '''
-    Same as plotFSC2 but for three pairs of volumes
-    '''
-
-    sz1a = vol1a.shape
-    sz2a = vol2a.shape
-    sz1b = vol1b.shape
-    sz2b = vol2b.shape
-    sz1c = vol1c.shape
-    sz2c = vol2c.shape
-    
-    if not all(x == sz1a for x in [sz2a,sz1b,sz2b,sz1c,sz2c]):
-        raise ValueError('Dimensions of all input volumes must be the same')
-        
-    if (labels is not None) and (len(labels)!=3) :
-        raise ValueError('labels must contain three labels')
-
-    fsc_a = FSCorr(vol1a,vol2a)
-    n = np.asarray(fsc_a).size
-    fsc_b = FSCorr(vol1b,vol2b)
-    fsc_c = FSCorr(vol1c,vol2c)
-    
-    fig, ax = plt.subplots(constrained_layout=True)
-    ax.grid(visible = True, axis = 'both')
-    ax.plot(np.arange(1,n+1),fsc_a,'-g', linewidth = 2.0)
-    ax.plot(np.arange(1,n+1),fsc_b,'-r', linewidth = 2.0)
-    ax.plot(np.arange(1,n+1),fsc_c,'-b', linewidth = 2.0)
-    
-    plt.xlim(np.array([1,n]))
-    plt.ylim(np.array([- 0.1,1.05]))
-    
-    # Plot cutoff line
-    y = np.ones((n)) * cutoff
-    ax.plot(np.arange(1,n+1),y, color='b', linestyle='--', linewidth=1.5)
-    
-    # Compute resolution - fscres return the bin number where the cutoff
-    # resolution is obtained.    
-    j_a = fscres(fsc_a,cutoff)
-    resAa = 2 * pixelsize * n / j_a
-    j_b = fscres(fsc_b,cutoff)
-    resAb = 2 * pixelsize * n / j_b
-    j_c = fscres(fsc_c,cutoff)
-    resAc = 2 * pixelsize * n / j_c
-            
-    yy = ax.get_ylim()
-    ax.vlines(j_a,0,yy[1], colors='b', linestyles='dashed') 
-    ax.vlines(j_b,0,yy[1], colors='b', linestyles='dashed') 
-    ax.vlines(j_c,0,yy[1], colors='b', linestyles='dashed') 
-
-    # Replace the default ticks with frequnecy values   
-    xticks_locs = ax.get_xticks()    
-    df = 1.0 / (2.0 * pixelsize * n)
-    xticks = xticks_locs * df
-    
-    xticks_labels = []
-    for e in xticks:
-        xticks_labels.append('{0:7.3f}'.format(e))
-    ax.set_xticks(xticks_locs,xticks_labels)        
-    ax.set_xlabel('1/A')
-    
-    # Add top axis
-    ax2 = ax.twiny()
-    xticks_locs = ax.get_xticks()   
-    xticks_labels = []
-    for e in xticks:
-        if e > 0:
-            xticks_labels.append('{0:7.3f}'.format(1/e))
-        else:
-            xticks_labels.append(' ')
-                        
-    ax2.set_xticks(xticks_locs,xticks_labels)        
-    ax2.set_xlabel('A')
-     
-    if labels is None:      
-        ax.legend(['{0:5.2f}A'.format(resAa), '{0:5.2f}A'.format(resAb), 
-                   '{0:5.2f}A'.format(resAc)])
-    else:
-        ax.legend([labels[0]+' {0:5.2f}A'.format(resAa), 
-                   labels[1]+' {0:5.2f}A'.format(resAb), 
-                   labels[2]+' {0:5.2f}A'.format(resAc)])
-        
-    fig1 = plt.gcf()
-    plt.show()
-    plt.draw()
-
-    if figname is not None:
-        fig1.savefig(figname, dpi = 300)
-
-    return resAa, resAb, resAc, fig    
+"""
+Created on Sun Sep 25 21:49:00 2022
+
+@author: yoel shkolnisky
+"""
+import numpy as np
+import matplotlib.pyplot as plt
+import scipy.interpolate as interp
+    
+def ndgrid (*xi):
+    '''
+    Implementation of MATLAB's ndgrid function.
+    Similar to meshgrid by with a different output ordering
+    
+    Parameters
+    ----------
+    *xi : x1, x2,...,xn: array_like
+        1-D arrays representing the coordinates of a grid.
+
+    Returns
+    -------
+    
+    X1, X2,...,xn ndarray
+    ndgrid(x1,x2,...,xn) replicates the grid vectors x1,x2,...,xn to produce 
+    an n-dimensional full grid.
+    '''
+
+    return np.meshgrid(*xi, indexing='ij')
+
+
+def FSCorr(m1,m2): 
+    '''
+    Compute the fourier shell correlation between the 3D maps m1 and m2,
+    which must be n x n x n in size with the same n, assumed to be even.
+    
+    The FSC is defined as
+                sum{F1 .* conj(F2)}
+    c(i) = -----------------------------
+           sqrt(sum|F1|^2 * sum|F2|^2)
+    where F1 and F2 are the Fourier components at the given spatial 
+    frequency i. i ranges from 1 to n/2-1, times the unit frequency 1/(n*res) 
+    where res is the pixel size.
+    
+    Examples:
+    --------
+    c=FSCorr(m1,m2)
+    
+    Parameters
+    ----------
+    m1,m2 : ndarray
+        n x n x n array. n assumed to be even
+
+    Returns
+    -------
+    c : 1-D vector with Fourier shell correlation coefficients computed as 
+    described above. 
+    
+    '''
+    
+    # First, construct the radius values for defining the shells.
+    n,n1,n2 = m1.shape
+    ctr = (n + 1) / 2
+    origin = np.transpose(np.array([ctr,ctr,ctr]))
+
+    x,y,z = ndgrid(np.arange(1 - origin[0],n - origin[0]+1),np.arange(1 - origin[1],n - origin[1]+1),np.arange(1 - origin[2],n - origin[2]+1))
+    R = np.sqrt(x ** 2 + y ** 2 + z ** 2)
+    eps = 0.0001
+
+    # Fourier-transform the maps
+    f1 = np.fft.fftshift(np.fft.fftn(m1))
+    f2 = np.fft.fftshift(np.fft.fftn(m2))
+
+    # Perform the sums
+    d0 = R < 0.5 + eps
+    c = np.zeros((int(np.floor(n / 2)),1))
+    
+    for i in np.arange(1,int(np.floor(n / 2)+1)).reshape(-1):
+        d1 = R < 0.5 + i + eps
+        ring = np.logical_xor(d1,d0)
+        #r1 = np.multiply(ring,f1)
+        #r2 = np.multiply(ring,f2)
+        #num = np.real(sum(sum(sum(np.multiply(r1,np.conjugate(r2))))))
+        #den = np.sqrt(sum(sum(sum(np.abs(r1) ** 2))) * sum(sum(sum(np.abs(r2) ** 2))))
+        
+        r1 = f1[ring]
+        r2 = f2[ring]
+        num = np.real(sum(np.multiply(r1,np.conjugate(r2))))
+        den = np.sqrt(sum(np.abs(r1) ** 2) * sum(np.abs(r2) ** 2))
+            
+        c[i-1] = num / den
+        d0 = d1
+    
+    return c
+    
+    
+def fscres(fsc,cutoff):
+    '''
+    Find the resolution from an FSC curve.
+    r=fscres(fsc,cutoff)    determines the index of the last bin of the
+    given fsc curve that is above the the given cutoff. Intermediate values
+    of the FSC curve are estimated using interpolation.
+
+    Parameters
+    ----------
+    fsc : 1-D array
+        Fourier shell correlation coefficients, computed using FSCorr
+    cutoff : float
+        Cutoff value to determine resolution. 
+
+    Returns
+    -------
+    r : double
+        Estimated resolution
+        
+    '''
+    
+    n = np.asarray(fsc).size
+    r = n
+    x = np.arange(1,n+1)
+    xx = np.arange(1,n+0.01,0.01)
+    fsc_interp = interp.PchipInterpolator(x,fsc)
+    y = fsc_interp(xx)
+    ii = next((i for i, val in enumerate(y) if val < cutoff),-1)
+
+    if ii != -1 :
+        r = xx[ii]
+
+    return r
+    
+def plotFSC(vol1, vol2 ,cutoff = 0.143, pixelsize = 1.0): 
+    '''
+    Draw Fourier shell correlation curve and estimated resolution.
+
+    plotFSC(vol1,vol2,cutoff,pixelsize)
+    Draw the Fourier shell correlation curve for the volumes vol1 and vol2,
+    and determine the resolution according the the given cutoff and
+    pixelsize. The volumes vol1 and vol2 must be aligned.
+    
+    Example
+    -------
+    vol1 = mrcfile.open('map_ref.mrc')
+    vol2 = mrcfile.open('map_aligned.mrc')
+    cutoff=0.143
+    resA, fig = plotFSC(vol1.data,vol2.data,cutoff,1.5)
+
+
+    Algorithm
+    ---------
+    The resolution resA is determined as follows.
+    # The derivation is given in 1-D, but it is the same for 3D, if the three
+    dimesions of the volume are equal.
+    Denote
+    B   bandwidth of the signal
+    fs  Maximal frequnecy
+    T   Sampling rate (pixel size)
+    N   Length of the signal
+    j   The index of the last frequnecy bin where the correlation is above
+    the cutoff value.
+    
+    1. The bandwidth B is given by B=2*fs, as the signal has frequencies
+    in the range [-fs,fs].
+    2. According to the Nyquist criterion, the samping frequency 1/T must
+    satisfy 1/T>=B. The critical sampling rate is 1/T=B=2*fs.
+    3. The width of each frequnecy bin is B/N=2*fs/N.
+    4. The frequnecy of the bin at index j is fc=2*fs*j/N.
+    5. The resolution is defined as resA=1/fc=N/(2*fs*j).
+    Due to 2 above, resA=N*T/j.
+    6. FSCorr returns correlation values only for positive freqnecuies,
+    that is is returns the correlation at n frequnecies such that N=2*n
+    (it assumes that N is even). Thus, in terms n, resA is given by
+    resA = 2*n*T/j = (2*T)*(n/j).
+    
+    Parameters
+    ----------
+    vol1, vol2 : ndarray
+        3-D arrays of the same dimensions. Volumes must be aligned.
+    cutoff : float, optional
+        Correlation cutoff threshold to determine resolution. The resolution 
+        is determined by the first frequnecy where the correlation goes below 
+        this value. Common values are 0.143 and 0.5. The default is 0.143.
+    pixelsize : float, optional
+        Pixel size of the volumes. The default is 1.0A.
+
+    Returns
+    -------
+    resA : float
+    Resolution of the structure in Angstrom according to the given cutoff 
+    value.
+    
+    fig :  matplotlib.figure.Figure
+    Handle to the FSC curve plot.
+
+    '''
+    
+    fsc = FSCorr(vol1,vol2)
+    n = np.asarray(fsc).size
+    
+    fig, ax = plt.subplots(constrained_layout=True)
+    ax.grid(visible = True, axis = 'both')
+    ax.plot(np.arange(1,n+1),fsc,'-g', linewidth = 2.0)
+    
+    plt.xlim(np.array([1,n]))
+    plt.ylim(np.array([- 0.1,1.05]))
+    
+    # Plot cutoff line
+    y = np.ones((n)) * cutoff
+    ax.plot(np.arange(1,n+1),y, color='b', linestyle='--', linewidth=1.5)
+    
+    # Compute resolution - fscres return the bin number where the cutoff
+    # resolution is obtained.    
+    j = fscres(fsc,cutoff)
+    resA = 2 * pixelsize * n / j
+        
+    yy = ax.get_ylim()
+    ax.vlines(j,0,yy[1], colors='b', linestyles='dashed') 
+
+    # Replace the default ticks with frequnecy values   
+    xticks_locs = ax.get_xticks()    
+    df = 1.0 / (2.0 * pixelsize * n)
+    xticks = xticks_locs * df
+    
+    xticks_labels = []
+    for e in xticks:
+        xticks_labels.append('{0:7.3f}'.format(e))
+    ax.set_xticks(xticks_locs,xticks_labels)        
+    ax.set_xlabel('1/A')
+    
+    # Add top axis
+    ax2 = ax.twiny()
+    xticks_locs = ax.get_xticks()   
+    xticks_labels = []
+    for e in xticks:
+        if e > 0:
+            xticks_labels.append('{0:7.3f}'.format(1/e))
+        else:
+            xticks_labels.append(' ')
+                        
+    ax2.set_xticks(xticks_locs,xticks_labels)        
+    ax2.set_xlabel('A')
+       
+    plt.title('Resolution={0:5.2f}A'.format(resA))
+    plt.show()
+
+    return resA, fig    
+
+
+def plotFSC2(vol1a, vol2a , vol1b, vol2b, labels=None, 
+             cutoff = 0.143, pixelsize = 1.0, figname=None): 
+    '''
+    Draw Fourier shell correlation curve and estimate resolution.
+    
+    Use this function to plot the Fourier shell correlations of two pairs on 
+    volumes on the same axis. This can be used to compare the quality of two
+    reconstructions. 
+    
+    Specifically, draw the Fourier shell correlation curve for the pairs of 
+    volumes (vol1a,vol2a) and (vol1b, vol2b), and determine the resolution of 
+    each pair according the the given cutoff and pixelsize. Each pair of 
+    volumes must be aligned.
+    
+    Use the given cutoff value for determining resolution. Common values
+    for cutoff are 0.143 and 0.5.  The resolution is determined by the 
+    first frequnecy where the correlation goes below this value.
+
+    Example
+    -------
+    vol1a=ReadMRC('./vol1a.mrc');
+    vol2a=ReadMRC('./vol2a.mrc');
+    vol1b=ReadMRC('./vol1b.mrc');
+    vol2b=ReadMRC('./vol2b.mrc');
+    cutoff=0.143;
+    resA=plotFSC(vol1a.data,vol2a.data,vol1b.data,vol2b.data,cutoff,1.5); 
+
+
+    Parameters
+    ----------
+    vol1a, vol2a, vol1b, vol2b : ndarray
+        3-D arrays of the same dimensions. Volumes must be aligned.
+    cutoff : float, optional
+        Correlation cutoff threshold to determine resolution. The resolution 
+        is determined by the first frequnecy where the correlation goes below 
+        this value. Common values are 0.143 and 0.5. The default is 0.143.
+    pixelsize : float, optional
+        Pixel size of the volumes. The default is 1.0A.
+    figname: string, optional
+        If not None, the FSC plot would be saved to a file with this name.
+
+    Returns
+    -------
+    resAa : float
+        Estimated resolution of vol1a and vol2a
+    resAb : float
+        Estimated resolution of vol1b and vol2b
+    fig :  matplotlib.figure.Figure
+        Handle to the FSC curve plot.
+        
+        
+    See plotFSC for more details.
+
+    '''
+
+    sz1a = vol1a.shape
+    sz2a = vol2a.shape
+    sz1b = vol1b.shape
+    sz2b = vol2b.shape
+    
+    if (sz1a != sz2a) or (sz1a != sz1b) or (sz1a != sz2b):
+        raise ValueError('Dimensions of all input volumes must be the same')
+
+    if (labels is not None) and (len(labels)!=2) :
+        raise ValueError('labels must contain two labels')
+
+    fsc_a = FSCorr(vol1a,vol2a)
+    n = np.asarray(fsc_a).size
+    fsc_b = FSCorr(vol1b,vol2b)
+    
+    fig, ax = plt.subplots(constrained_layout=True)
+    ax.grid(visible = True, axis = 'both')
+    ax.plot(np.arange(1,n+1),fsc_a,'-g', linewidth = 2.0)
+    ax.plot(np.arange(1,n+1),fsc_b,'-r', linewidth = 2.0)
+    
+    plt.xlim(np.array([1,n]))
+    plt.ylim(np.array([- 0.1,1.05]))
+    
+    # Plot cutoff line
+    y = np.ones((n)) * cutoff
+    ax.plot(np.arange(1,n+1),y, color='b', linestyle='--', linewidth=1.5)
+    
+    # Compute resolution - fscres return the bin number where the cutoff
+    # resolution is obtained.    
+    j_a = fscres(fsc_a,cutoff)
+    resAa = 2 * pixelsize * n / j_a
+    j_b = fscres(fsc_b,cutoff)
+    resAb = 2 * pixelsize * n / j_b
+        
+    yy = ax.get_ylim()
+    ax.vlines(j_a,0,yy[1], colors='b', linestyles='dashed') 
+    ax.vlines(j_b,0,yy[1], colors='b', linestyles='dashed') 
+
+    # Replace the default ticks with frequnecy values   
+    xticks_locs = ax.get_xticks()    
+    df = 1.0 / (2.0 * pixelsize * n)
+    xticks = xticks_locs * df
+    
+    xticks_labels = []
+    for e in xticks:
+        xticks_labels.append('{0:7.3f}'.format(e))
+    ax.set_xticks(xticks_locs,xticks_labels)        
+    ax.set_xlabel('1/A')
+    
+    # Add top axis
+    ax2 = ax.twiny()
+    xticks_locs = ax.get_xticks()   
+    xticks_labels = []
+    for e in xticks:
+        if e > 0:
+            xticks_labels.append('{0:7.3f}'.format(1/e))
+        else:
+            xticks_labels.append(' ')
+                        
+    ax2.set_xticks(xticks_locs,xticks_labels)        
+    ax2.set_xlabel('A')
+           
+    if labels is None:      
+        ax.legend(['{0:5.2f}A'.format(resAa), '{0:5.2f}A'.format(resAb)])
+    else:
+        ax.legend([labels[0]+' {0:5.2f}A'.format(resAa), 
+                   labels[1]+' {0:5.2f}A'.format(resAb)])
+
+    fig1 = plt.gcf()
+    plt.show()
+    plt.draw()
+
+    if figname is not None:
+        fig1.savefig(figname, dpi = 300)
+
+    return resAa, resAb, fig    
+
+
+def plotFSC3(vol1a, vol2a , vol1b, vol2b, vol1c, vol2c, labels=None,
+             cutoff = 0.143, pixelsize = 1.0, figname=None): 
+    '''
+    Same as plotFSC2 but for three pairs of volumes
+    '''
+
+    sz1a = vol1a.shape
+    sz2a = vol2a.shape
+    sz1b = vol1b.shape
+    sz2b = vol2b.shape
+    sz1c = vol1c.shape
+    sz2c = vol2c.shape
+    
+    if not all(x == sz1a for x in [sz2a,sz1b,sz2b,sz1c,sz2c]):
+        raise ValueError('Dimensions of all input volumes must be the same')
+        
+    if (labels is not None) and (len(labels)!=3) :
+        raise ValueError('labels must contain three labels')
+
+    fsc_a = FSCorr(vol1a,vol2a)
+    n = np.asarray(fsc_a).size
+    fsc_b = FSCorr(vol1b,vol2b)
+    fsc_c = FSCorr(vol1c,vol2c)
+    
+    fig, ax = plt.subplots(constrained_layout=True)
+    ax.grid(visible = True, axis = 'both')
+    ax.plot(np.arange(1,n+1),fsc_a,'-g', linewidth = 2.0)
+    ax.plot(np.arange(1,n+1),fsc_b,'-r', linewidth = 2.0)
+    ax.plot(np.arange(1,n+1),fsc_c,'-b', linewidth = 2.0)
+    
+    plt.xlim(np.array([1,n]))
+    plt.ylim(np.array([- 0.1,1.05]))
+    
+    # Plot cutoff line
+    y = np.ones((n)) * cutoff
+    ax.plot(np.arange(1,n+1),y, color='b', linestyle='--', linewidth=1.5)
+    
+    # Compute resolution - fscres return the bin number where the cutoff
+    # resolution is obtained.    
+    j_a = fscres(fsc_a,cutoff)
+    resAa = 2 * pixelsize * n / j_a
+    j_b = fscres(fsc_b,cutoff)
+    resAb = 2 * pixelsize * n / j_b
+    j_c = fscres(fsc_c,cutoff)
+    resAc = 2 * pixelsize * n / j_c
+            
+    yy = ax.get_ylim()
+    ax.vlines(j_a,0,yy[1], colors='b', linestyles='dashed') 
+    ax.vlines(j_b,0,yy[1], colors='b', linestyles='dashed') 
+    ax.vlines(j_c,0,yy[1], colors='b', linestyles='dashed') 
+
+    # Replace the default ticks with frequnecy values   
+    xticks_locs = ax.get_xticks()    
+    df = 1.0 / (2.0 * pixelsize * n)
+    xticks = xticks_locs * df
+    
+    xticks_labels = []
+    for e in xticks:
+        xticks_labels.append('{0:7.3f}'.format(e))
+    ax.set_xticks(xticks_locs,xticks_labels)        
+    ax.set_xlabel('1/A')
+    
+    # Add top axis
+    ax2 = ax.twiny()
+    xticks_locs = ax.get_xticks()   
+    xticks_labels = []
+    for e in xticks:
+        if e > 0:
+            xticks_labels.append('{0:7.3f}'.format(1/e))
+        else:
+            xticks_labels.append(' ')
+                        
+    ax2.set_xticks(xticks_locs,xticks_labels)        
+    ax2.set_xlabel('A')
+     
+    if labels is None:      
+        ax.legend(['{0:5.2f}A'.format(resAa), '{0:5.2f}A'.format(resAb), 
+                   '{0:5.2f}A'.format(resAc)])
+    else:
+        ax.legend([labels[0]+' {0:5.2f}A'.format(resAa), 
+                   labels[1]+' {0:5.2f}A'.format(resAb), 
+                   labels[2]+' {0:5.2f}A'.format(resAc)])
+        
+    fig1 = plt.gcf()
+    plt.show()
+    plt.draw()
+
+    if figname is not None:
+        fig1.savefig(figname, dpi = 300)
+
+    return resAa, resAb, resAc, fig
```

### Comparing `EMalign-1.0.3/src/genRotationsGrid.py` & `EMalign-1.0.4/src/genRotationsGrid.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Feb 10 23:42:18 2021
-
-@author: yaelharpaz1
-"""
-
-import numpy as np
-import math
-
-
-def q_to_rot(q):
-    # Convert a quaternion into a rotation matrix.
-    
-    #   Input: 
-    #           q: quaternion. May be a vector of dimensions 4 x n
-    #   Output: 
-    #           rot_matrix: 3x3xn rotation matrix
-    
-    #   Yariv Aizenbud 31.01.2016
-    
-    n = np.size(q, axis=1)
-    rot_matrix = np.zeros((3,3,n))
-    
-    rot_matrix[0,0,:] = q[0,:]**2 + q[1,:]**2 - q[2,:]**2 - q[3,:]**2
-    rot_matrix[0,1,:] = 2*q[1,:]*q[2,:] - 2*q[0,:]*q[3,:] 
-    rot_matrix[0,2,:] = 2*q[0,:]*q[2,:] + 2*q[1,:]*q[3,:] 
-    
-    rot_matrix[1,0,:] = 2*q[1,:]*q[2,:] + 2*q[0,:]*q[3,:]
-    rot_matrix[1,1,:] = q[0,:]**2 - q[1,:]**2 + q[2,:]**2 - q[3,:]**2 
-    rot_matrix[1,2,:] = -2*q[0,:]*q[1,:] + 2*q[2,:]*q[3,:]
-    
-    rot_matrix[2,0,:] = -2*q[0,:]*q[2,:] + 2*q[1,:]*q[3,:] 
-    rot_matrix[2,1,:] = 2*q[0,:]*q[1,:] + 2*q[2,:]*q[3,:] 
-    rot_matrix[2,2,:] = q[0,:]**2 - q[1,:]**2 - q[2,:]**2 + q[3,:]**2
-    
-    return rot_matrix
-
-def genRotationsGrid(res):
-    # genRotationsGrid generate approximatly equally spaced rotations.
-    #   Input:
-    #       resolution - the number of samples per 2*pi.
-    #                    for example:
-    #                        resolution = 50  you get   4484 rotations
-    #                        resolution = 75  you get  15236 rotations
-    #                        resolution = 100 you get  39365 rotations
-    #                        resolution = 150 you get 129835 rotations
-    #   Output:
-    #       rotations - 3X3Xnumber_of_rotations matrix. of all the rotations.
-    # angles - 3Xnumber_of_rotations matrix. each column contains three
-    #          angles of the rotation in the following parametrization for
-    #          quaternions:
-    #          parametrization for SO3
-    #               x = sin(tau)* sin(theta)* sin(phi);
-    #               y = sin(tau)* sin(theta)* cos(phi);
-    #               z = sin(tau)* cos(theta);
-    #               w = cos(tau);
-    
-    counter = 0
-    tau_step = (math.pi/2)/(res/4)
-    for tau1 in np.arange(tau_step/2, (math.pi/2-tau_step/2), tau_step):
-        theta_step = math.pi/(res/2*math.sin(tau1))
-        for theta1 in np.arange(theta_step/2, math.pi-theta_step/2, theta_step):
-            phi_step = (2*math.pi)/(res*math.sin(tau1)*math.sin(theta1))
-            for phi1 in np.arange(0,2*math.pi-phi_step,phi_step):
-                counter = counter + 1
-    n_of_rotations = counter
-    
-    angles = np.zeros((3,n_of_rotations))   
-    rotations = np.zeros((3,3,n_of_rotations))
-    counter = -1
-    
-    for tau1 in np.arange(tau_step/2, (math.pi/2-tau_step/2), tau_step):
-        sintau1 = math.sin(tau1)
-        costau1 = math.cos(tau1)
-        theta_step = math.pi/(res/2*math.sin(tau1))
-        for theta1 in np.arange(theta_step/2, math.pi-theta_step/2, theta_step):
-            sintheta1 = math.sin(theta1)
-            costheta1 = math.cos(theta1)
-            phi_step = (2*math.pi)/(res*math.sin(tau1)*math.sin(theta1))
-            for phi1 in np.arange(0,2*math.pi-phi_step,phi_step):
-                counter = counter + 1
-                angles[:,counter] = np.array([tau1,theta1,phi1])
-                rotations[:,:,counter] = q_to_rot(np.array([sintau1*sintheta1*math.sin(phi1), 
-                                           sintau1*sintheta1*math.cos(phi1),
-                                           sintau1*costheta1,
-                                           costau1]).reshape((4,1))).reshape((3,3))
-    return rotations    
-                                
-    
-    
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Feb 10 23:42:18 2021
+
+@author: yaelharpaz1
+"""
+
+import numpy as np
+import math
+
+
+def q_to_rot(q):
+    # Convert a quaternion into a rotation matrix.
+    
+    #   Input: 
+    #           q: quaternion. May be a vector of dimensions 4 x n
+    #   Output: 
+    #           rot_matrix: 3x3xn rotation matrix
+    
+    #   Yariv Aizenbud 31.01.2016
+    
+    n = np.size(q, axis=1)
+    rot_matrix = np.zeros((3,3,n))
+    
+    rot_matrix[0,0,:] = q[0,:]**2 + q[1,:]**2 - q[2,:]**2 - q[3,:]**2
+    rot_matrix[0,1,:] = 2*q[1,:]*q[2,:] - 2*q[0,:]*q[3,:] 
+    rot_matrix[0,2,:] = 2*q[0,:]*q[2,:] + 2*q[1,:]*q[3,:] 
+    
+    rot_matrix[1,0,:] = 2*q[1,:]*q[2,:] + 2*q[0,:]*q[3,:]
+    rot_matrix[1,1,:] = q[0,:]**2 - q[1,:]**2 + q[2,:]**2 - q[3,:]**2 
+    rot_matrix[1,2,:] = -2*q[0,:]*q[1,:] + 2*q[2,:]*q[3,:]
+    
+    rot_matrix[2,0,:] = -2*q[0,:]*q[2,:] + 2*q[1,:]*q[3,:] 
+    rot_matrix[2,1,:] = 2*q[0,:]*q[1,:] + 2*q[2,:]*q[3,:] 
+    rot_matrix[2,2,:] = q[0,:]**2 - q[1,:]**2 - q[2,:]**2 + q[3,:]**2
+    
+    return rot_matrix
+
+def genRotationsGrid(res):
+    # genRotationsGrid generate approximatly equally spaced rotations.
+    #   Input:
+    #       resolution - the number of samples per 2*pi.
+    #                    for example:
+    #                        resolution = 50  you get   4484 rotations
+    #                        resolution = 75  you get  15236 rotations
+    #                        resolution = 100 you get  39365 rotations
+    #                        resolution = 150 you get 129835 rotations
+    #   Output:
+    #       rotations - 3X3Xnumber_of_rotations matrix. of all the rotations.
+    # angles - 3Xnumber_of_rotations matrix. each column contains three
+    #          angles of the rotation in the following parametrization for
+    #          quaternions:
+    #          parametrization for SO3
+    #               x = sin(tau)* sin(theta)* sin(phi);
+    #               y = sin(tau)* sin(theta)* cos(phi);
+    #               z = sin(tau)* cos(theta);
+    #               w = cos(tau);
+    
+    counter = 0
+    tau_step = (math.pi/2)/(res/4)
+    for tau1 in np.arange(tau_step/2, (math.pi/2-tau_step/2), tau_step):
+        theta_step = math.pi/(res/2*math.sin(tau1))
+        for theta1 in np.arange(theta_step/2, math.pi-theta_step/2, theta_step):
+            phi_step = (2*math.pi)/(res*math.sin(tau1)*math.sin(theta1))
+            for phi1 in np.arange(0,2*math.pi-phi_step,phi_step):
+                counter = counter + 1
+    n_of_rotations = counter
+    
+    angles = np.zeros((3,n_of_rotations))   
+    rotations = np.zeros((3,3,n_of_rotations))
+    counter = -1
+    
+    for tau1 in np.arange(tau_step/2, (math.pi/2-tau_step/2), tau_step):
+        sintau1 = math.sin(tau1)
+        costau1 = math.cos(tau1)
+        theta_step = math.pi/(res/2*math.sin(tau1))
+        for theta1 in np.arange(theta_step/2, math.pi-theta_step/2, theta_step):
+            sintheta1 = math.sin(theta1)
+            costheta1 = math.cos(theta1)
+            phi_step = (2*math.pi)/(res*math.sin(tau1)*math.sin(theta1))
+            for phi1 in np.arange(0,2*math.pi-phi_step,phi_step):
+                counter = counter + 1
+                angles[:,counter] = np.array([tau1,theta1,phi1])
+                rotations[:,:,counter] = q_to_rot(np.array([sintau1*sintheta1*math.sin(phi1), 
+                                           sintau1*sintheta1*math.cos(phi1),
+                                           sintau1*costheta1,
+                                           costau1]).reshape((4,1))).reshape((3,3))
+    return rotations    
+                                
+    
+
```

### Comparing `EMalign-1.0.3/src/gentestdata.py` & `EMalign-1.0.4/src/gentestdata.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Sat Apr  2 01:25:14 2022
-
-@author: yaelharpaz1
-"""
-
-
-import numpy as np
-from src.cryo_fetch_emdID import cryo_fetch_emdID
-from src.common_finufft import cryo_downsample
-from src.rand_rots import rand_rots
-from src.fastrotate3d import fastrotate3d
-from src.reshift_vol import reshift_vol
-import logging
-import mrcfile
-import shutil
-
-
-def gentestdata(ref_mrc_filename,transformed_mrc_filename,emdID=2660,verbose=1):
-    """
-    gentestdata  generates test volumes for the function align_volumes in 
-    align_volumes_3d.
-    
-    This function fetchs the map file (MRC format) with the given emdID 
-    (integer) from EMDB.
-    Generates a volume demonstrating the 3D structure from the retrived map 
-    file. Generates an additional rotated and shifted volume, and saves the 
-    two volumes.
-    """
-    np.random.seed(2021)
-    
-    logger = logging.getLogger()
-    logger.disabled = False
-    if verbose == 0: 
-        logger.disabled = True  
-    
-    # Read molecule:    
-    logger.info('Downloading the volume from EMDB')
-    cryo_fetch_emdID(emdID,ref_mrc_filename,verbose) 
-    logger.info('The volume was downloaded')
-    
-    vol = np.ascontiguousarray(mrcfile.open(ref_mrc_filename).data.T)
-    
-    n_ds = 128
-    logger.info('Downsampling volume to %i pixels', n_ds)
-    vol = cryo_downsample(vol,(n_ds, n_ds, n_ds)).astype('float64')
-
-    # Rotate and shift the volume:
-    logger.info('Generating a rotated and shifted volume')
-    R_true = rand_rots(1).reshape((3,3))
-    vol_rotated = fastrotate3d(vol.copy(), R_true)
-    shift = np.array([-10, 1 ,10])
-    vol_rotated = reshift_vol(vol_rotated.copy(), shift)
-    
-    logger.info('Ground truth rotation:')
-    logger.info('%.4f %.4f %.4f', R_true[0,0], R_true[0,1], R_true[0,2])
-    logger.info('%.4f %.4f %.4f', R_true[1,0], R_true[1,1], R_true[1,2])
-    logger.info('%.4f %.4f %.4f', R_true[2,0], R_true[2,1], R_true[2,2])
-    
-    logger.info('Ground truth translation: [%.3f, %.3f, %.3f]',shift[0], shift[1], shift[2])
-
-    # Save downsampled reference volume
-    mrc_fh = mrcfile.open(ref_mrc_filename, mode='r+')
-    mrc_fh.set_data(vol.astype('float32').T)
-    mrc_fh.set_volume()
-    mrc_fh.update_header_stats()
-    mrc_fh.close()
-
-    # Save transformed volume
-    # Copy reference volume to transformed volume to duplicate the correct header
-    shutil.copyfile(ref_mrc_filename, transformed_mrc_filename)
-
-    # Update data with transformed volume and save
-    mrc_fh = mrcfile.open(transformed_mrc_filename, mode='r+')
-    mrc_fh.set_data(vol_rotated.astype('float32').T)
-    mrc_fh.set_volume()
-    mrc_fh.update_header_stats()
-    mrc_fh.close()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Sat Apr  2 01:25:14 2022
+
+@author: yaelharpaz1
+"""
+
+
+import numpy as np
+from src.cryo_fetch_emdID import cryo_fetch_emdID
+from src.common_finufft import cryo_downsample
+from src.rand_rots import rand_rots
+from src.fastrotate3d import fastrotate3d
+from src.reshift_vol import reshift_vol
+import logging
+import mrcfile
+import shutil
+
+
+def gentestdata(ref_mrc_filename,transformed_mrc_filename,emdID=2660,verbose=1):
+    """
+    gentestdata  generates test volumes for the function align_volumes in 
+    align_volumes_3d.
+    
+    This function fetchs the map file (MRC format) with the given emdID 
+    (integer) from EMDB.
+    Generates a volume demonstrating the 3D structure from the retrived map 
+    file. Generates an additional rotated and shifted volume, and saves the 
+    two volumes.
+    """
+    np.random.seed(2021)
+    
+    logger = logging.getLogger()
+    logger.disabled = False
+    if verbose == 0: 
+        logger.disabled = True  
+    
+    # Read molecule:    
+    logger.info('Downloading the volume from EMDB')
+    cryo_fetch_emdID(emdID,ref_mrc_filename,verbose) 
+    logger.info('The volume was downloaded')
+    
+    vol = np.ascontiguousarray(mrcfile.open(ref_mrc_filename).data.T)
+    
+    n_ds = 128
+    logger.info('Downsampling volume to %i pixels', n_ds)
+    vol = cryo_downsample(vol,(n_ds, n_ds, n_ds)).astype('float64')
+
+    # Rotate and shift the volume:
+    logger.info('Generating a rotated and shifted volume')
+    R_true = rand_rots(1).reshape((3,3))
+    vol_rotated = fastrotate3d(vol.copy(), R_true)
+    shift = np.array([-10, 1 ,10])
+    vol_rotated = reshift_vol(vol_rotated.copy(), shift)
+    
+    logger.info('Ground truth rotation:')
+    logger.info('%.4f %.4f %.4f', R_true[0,0], R_true[0,1], R_true[0,2])
+    logger.info('%.4f %.4f %.4f', R_true[1,0], R_true[1,1], R_true[1,2])
+    logger.info('%.4f %.4f %.4f', R_true[2,0], R_true[2,1], R_true[2,2])
+    
+    logger.info('Ground truth translation: [%.3f, %.3f, %.3f]',shift[0], shift[1], shift[2])
+
+    # Save downsampled reference volume
+    mrc_fh = mrcfile.open(ref_mrc_filename, mode='r+')
+    mrc_fh.set_data(vol.astype('float32').T)
+    mrc_fh.set_volume()
+    mrc_fh.update_header_stats()
+    mrc_fh.close()
+
+    # Save transformed volume
+    # Copy reference volume to transformed volume to duplicate the correct header
+    shutil.copyfile(ref_mrc_filename, transformed_mrc_filename)
+
+    # Update data with transformed volume and save
+    mrc_fh = mrcfile.open(transformed_mrc_filename, mode='r+')
+    mrc_fh.set_data(vol_rotated.astype('float32').T)
+    mrc_fh.set_volume()
+    mrc_fh.update_header_stats()
+    mrc_fh.close()
```

### Comparing `EMalign-1.0.3/src/main.py` & `EMalign-1.0.4/src/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,128 +1,140 @@
-import shutil
-import warnings
-from sys import exit, argv
-import logging
-from src.emalign_input import check_for_newer_version, get_args, parse_args
-from src.align_volumes_3d import align_volumes
-from src.read_write import read_mrc, copy_and_rename
-from src.gentestdata import gentestdata
-import mrcfile
-#from src.common_finufft import cryo_downsample
-#import os
-#import shutil
-
-warnings.filterwarnings("ignore")
-
-# Check if CuPy is installed and we have GPU devices
-
-
-def main():
-    # Get user arguments:
-    user_input = argv
-    if len(user_input) > 1:  # User entered arguments. Use command line mode.
-        args = parse_args()
-        # Check if user entered the mandatory arguments: input and output
-        # directory and particle size. If not, exit.
-        if args.version:
-            import pkg_resources  # part of setuptools
-            version = pkg_resources.require('EMalign')[0].version
-            print('EMalign {}'.format(version))
-            exit()
-            
-        if args.make_test_data:
-            emdID = 2660
-            ref_mrc_filename = "map_ref_{0}.mrc".format(emdID)
-            transformed_mrc_filename = "map_transformed_{0}.mrc".format(emdID)
-            
-            
-            # Setup logger
-            logging.basicConfig(level=logging.INFO, format='%(message)s')
-            logger = logging.getLogger()
-
-            if args.verbose == 0:
-                logger.disabled = True
-            else:
-                logger.disabled = False
-
-            print("Generating test data...")
-            gentestdata(ref_mrc_filename, transformed_mrc_filename, emdID, args.verbose)
-            print("Test volume saved to " + ref_mrc_filename)
-            print("Transformed volume saved to "+ transformed_mrc_filename)
-            exit()
-            
-        if args.vol1 is None or args.vol2 is None or args.output_vol is None:
-            print(
-                "Error: one or more of the following arguments are missing: vol1, vol2, output-vol. For help run kltpicker -h")
-            exit()
-
-    else:  # User didn't enter arguments, use interactive mode to get arguments.
-        args = parse_args()  # Initiate args with default values.
-        args.vol1, args.vol2, args.output_vol, args.downsample, args.n_projs, args.no_refine, args.output_parameters, args.verbose = get_args()
-
-    # Check newer version
-    try:
-        check_for_newer_version()
-    except:
-        pass
-
-    # Setup logger    
-    logging.basicConfig(level=logging.INFO, format='%(message)s')
-    logger = logging.getLogger()
-
-    if args.verbose == 0:
-        logger.disabled = True
-    else:
-        logger.disabled = False
-    
-    # Load volumes
-    vol1 = read_mrc(args.vol1)
-    vol2 = read_mrc(args.vol2)
-    
-    if not ((vol1.shape[1]==vol1.shape[0]) and (vol1.shape[2]==vol1.shape[0]) 
-            and (vol1.shape[0] % 2 == 0)):
-        raise ValueError("All three dimensions of input volumes must be equal and even")   
-
-    if not ((vol1.shape[1]==vol1.shape[0]) and (vol1.shape[2]==vol1.shape[0]) 
-            and (vol1.shape[0] % 2 == 0)):
-        raise ValueError("All three dimensions of input volumes must be equal and even")
-        
-    if (vol1.shape[0] != vol2.shape[0]):
-        raise ValueError("Input volumes must be of same dimensions")
-    
-    # If we decide to downsample them to the same size
-    # n1 = vol1.shape[0]
-    # n2 = vol2.shape[0]
-    # if n1 < n2:
-    #     vol2 = cryo_downsample(vol2, (n1, n1, n1))
-    # elif n2 < n1:
-    #     vol1 = cryo_downsample(vol1, (n2, n2, n2))
-
-    # create params
-    class Struct:
-        pass
-
-    opt = Struct()
-    opt.Nprojs = args.n_projs
-    opt.downsample = args.downsample
-    opt.no_refine = args.no_refine
-    
-    # Run
-    bestR, bestdx, reflect, vol2aligned, bestcorr = align_volumes(vol1, vol2, args.verbose, opt)
-
-    # Save
-    # Copy vol2 to save header
-    shutil.copyfile(args.vol2, args.output_vol)
-
-    # Change and save
-    mrc_fh = mrcfile.open(args.output_vol, mode='r+')
-    mrc_fh.set_data(vol2aligned.astype('float32').T)
-    mrc_fh.set_volume()
-    mrc_fh.update_header_stats()
-    mrc_fh.close()
-
-    # Save parameters
-    if args.output_parameters is not None:
-        lines = ['reflect:\t{}'.format(reflect), 'correlation:\t{}'.format(bestcorr),
-                 'estimated translation:\t{}'.format(bestdx), 'rotation:\n{}'.format(bestR)]
-        with open(args.output_parameters, 'w') as f:
-            f.writelines('\n'.join(lines))
+import shutil
+import warnings
+from sys import exit, argv
+import logging
+from src.emalign_input import check_for_newer_version, get_args, parse_args
+from src.align_volumes_3d import align_volumes
+from src.read_write import read_mrc, copy_and_rename
+from src.gentestdata import gentestdata
+import mrcfile
+import scipy.ndimage
+
+
+#from src.common_finufft import cryo_downsample
+#import os
+#import shutil
+
+warnings.filterwarnings("ignore")
+
+# Check if CuPy is installed and we have GPU devices
+
+
+def main():
+    # Get user arguments:
+    user_input = argv
+    if len(user_input) > 1:  # User entered arguments. Use command line mode.
+        args = parse_args()
+        # Check if user entered the mandatory arguments: input and output
+        # directory and particle size. If not, exit.
+        if args.version:
+            import pkg_resources  # part of setuptools
+            version = pkg_resources.require('EMalign')[0].version
+            print('EMalign {}'.format(version))
+            exit()
+            
+        if args.make_test_data:
+            emdID = 2660
+            ref_mrc_filename = "map_ref_{0}.mrc".format(emdID)
+            transformed_mrc_filename = "map_transformed_{0}.mrc".format(emdID)
+            
+            
+            # Setup logger
+            logging.basicConfig(level=logging.INFO, format='%(message)s')
+            logger = logging.getLogger()
+
+            if args.verbose == 0:
+                logger.disabled = True
+            else:
+                logger.disabled = False
+
+            print("Generating test data...")
+            gentestdata(ref_mrc_filename, transformed_mrc_filename, emdID, args.verbose)
+            print("Test volume saved to " + ref_mrc_filename)
+            print("Transformed volume saved to "+ transformed_mrc_filename)
+            exit()
+            
+        if args.vol1 is None or args.vol2 is None or args.output_vol is None:
+            print(
+                "Error: one or more of the following arguments are missing: vol1, vol2, output-vol. For help run kltpicker -h")
+            exit()
+
+    else:  # User didn't enter arguments, use interactive mode to get arguments.
+        args = parse_args()  # Initiate args with default values.
+        args.vol1, args.vol2, args.output_vol, args.downsample, args.n_projs,\
+            args.apply_filtering, args.no_refine, args.output_parameters,\
+            args.verbose = get_args()
+
+    # Check newer version
+    try:
+        check_for_newer_version()
+    except:
+        pass
+
+    # Setup logger    
+    logging.basicConfig(level=logging.INFO, format='%(message)s')
+    logger = logging.getLogger()
+
+    if args.verbose == 0:
+        logger.disabled = True
+    else:
+        logger.disabled = False
+    
+    # Load volumes
+    vol1 = read_mrc(args.vol1)
+    vol2 = read_mrc(args.vol2)
+    
+    if not ((vol1.shape[1]==vol1.shape[0]) and (vol1.shape[2]==vol1.shape[0]) 
+            and (vol1.shape[0] % 2 == 0)):
+        raise ValueError("All three dimensions of input volumes must be equal and even")   
+
+    if not ((vol1.shape[1]==vol1.shape[0]) and (vol1.shape[2]==vol1.shape[0]) 
+            and (vol1.shape[0] % 2 == 0)):
+        raise ValueError("All three dimensions of input volumes must be equal and even")
+        
+    if (vol1.shape[0] != vol2.shape[0]):
+        raise ValueError("Input volumes must be of same dimensions")
+
+
+    # Filter volumes
+    if args.apply_filtering:
+       logger.info("Lowpass filtering input volumes")
+       vol1 = scipy.ndimage.gaussian_filter(vol1,1.5)
+       vol2 = scipy.ndimage.gaussian_filter(vol2,1.5)
+
+    # If we decide to downsample them to the same size
+    # n1 = vol1.shape[0]
+    # n2 = vol2.shape[0]
+    # if n1 < n2:
+    #     vol2 = cryo_downsample(vol2, (n1, n1, n1))
+    # elif n2 < n1:
+    #     vol1 = cryo_downsample(vol1, (n2, n2, n2))
+
+    # create params
+    class Struct:
+        pass
+
+    opt = Struct()
+    opt.Nprojs = args.n_projs
+    opt.downsample = args.downsample
+    opt.no_refine = args.no_refine
+    
+    # Run
+    bestR, bestdx, reflect, vol2aligned, bestcorr = align_volumes(vol1, vol2, args.verbose, opt)
+
+    # Save
+    # Copy vol2 to save header
+    shutil.copyfile(args.vol2, args.output_vol)
+
+    # Change and save
+    mrc_fh = mrcfile.open(args.output_vol, mode='r+')
+    mrc_fh.set_data(vol2aligned.astype('float32').T)
+    mrc_fh.set_volume()
+    mrc_fh.update_header_stats()
+    mrc_fh.close()
+
+    # Save parameters
+    if args.output_parameters is not None:
+        lines = ['reflect:\t{}'.format(reflect), 'correlation:\t{}'.format(bestcorr),
+                 'estimated translation:\t{}'.format(bestdx), 'rotation:\n{}'.format(bestR)]
+        with open(args.output_parameters, 'w') as f:
+            f.writelines('\n'.join(lines))
```

### Comparing `EMalign-1.0.3/src/rand_rots.py` & `EMalign-1.0.4/src/rand_rots.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Feb 10 18:46:35 2021
-
-@author: yaelharpaz1
-"""
-
-import numpy as np
-
-def qrand(k):
-    # Generate K random uniformly distributed quaternions.
-    # Each quaternions is a four-elements column vector. Returns a matrix of
-    # size 4xK.
-    
-    # The 3-sphere S^3 in R^4 is a double cover of the rotation group SO(3),
-    # SO(3) = RP^3. 
-    # We identify unit norm quaternions a^2+b^2+c^2+d^2=1 with group elements. 
-    # The antipodal points (-a,-b,-c,-d) and (a,b,c,d) are identified as the
-    # same group elements, so we take a>=0.
-    from scipy.stats import norm
-    q = norm.ppf(np.random.rand(k, 4).T)
-    
-    l2_norm = np.sqrt(q[0,:]**2 + q[1,:]**2 + q[2,:]**2 +q[3,:]**2)
-    for i in range(4):
-        q[i,:] = q[i,:]/l2_norm
-    for k in range(k):
-        if q[0,k] < 0:
-            q[:,k] = -q[:,k]
-            
-    return q
-
-def q_to_rot(q):
-    # Convert a quaternion into a rotation matrix.
-    
-    #   Input: 
-    #           q: quaternion. May be a vector of dimensions 4 x n
-    #   Output: 
-    #           rot_matrix: 3x3xn rotation matrix
-    
-    #   Yariv Aizenbud 31.01.2016
-    
-    n = np.size(q, axis=1)
-    rot_matrix = np.zeros((3,3,n))
-    
-    rot_matrix[0,0,:] = q[0,:]**2 + q[1,:]**2 - q[2,:]**2 - q[3,:]**2
-    rot_matrix[0,1,:] = 2*q[1,:]*q[2,:] - 2*q[0,:]*q[3,:] 
-    rot_matrix[0,2,:] = 2*q[0,:]*q[2,:] + 2*q[1,:]*q[3,:] 
-    
-    rot_matrix[1,0,:] = 2*q[1,:]*q[2,:] + 2*q[0,:]*q[3,:]
-    rot_matrix[1,1,:] = q[0,:]**2 - q[1,:]**2 + q[2,:]**2 - q[3,:]**2 
-    rot_matrix[1,2,:] = -2*q[0,:]*q[1,:] + 2*q[2,:]*q[3,:]
-    
-    rot_matrix[2,0,:] = -2*q[0,:]*q[2,:] + 2*q[1,:]*q[3,:] 
-    rot_matrix[2,1,:] = 2*q[0,:]*q[1,:] + 2*q[2,:]*q[3,:] 
-    rot_matrix[2,2,:] = q[0,:]**2 - q[1,:]**2 - q[2,:]**2 + q[3,:]**2
-    
-    return rot_matrix
-
-def rand_rots(n):
-    # rand_rots generate random rotations
-    # Input
-    #    n: The number of rotations to generate.
-    # Output
-    #    rot_matrices: An array of size 3-by-3-by-n containing n rotation matrices
-    #    sampled from the unifoorm distribution on SO(3).
-
-    qs = qrand(n)
-    rot_matrices = q_to_rot(qs)
-    
-    return rot_matrices
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Feb 10 18:46:35 2021
+
+@author: yaelharpaz1
+"""
+
+import numpy as np
+
+def qrand(k):
+    # Generate K random uniformly distributed quaternions.
+    # Each quaternions is a four-elements column vector. Returns a matrix of
+    # size 4xK.
+    
+    # The 3-sphere S^3 in R^4 is a double cover of the rotation group SO(3),
+    # SO(3) = RP^3. 
+    # We identify unit norm quaternions a^2+b^2+c^2+d^2=1 with group elements. 
+    # The antipodal points (-a,-b,-c,-d) and (a,b,c,d) are identified as the
+    # same group elements, so we take a>=0.
+    from scipy.stats import norm
+    q = norm.ppf(np.random.rand(k, 4).T)
+    
+    l2_norm = np.sqrt(q[0,:]**2 + q[1,:]**2 + q[2,:]**2 +q[3,:]**2)
+    for i in range(4):
+        q[i,:] = q[i,:]/l2_norm
+    for k in range(k):
+        if q[0,k] < 0:
+            q[:,k] = -q[:,k]
+            
+    return q
+
+def q_to_rot(q):
+    # Convert a quaternion into a rotation matrix.
+    
+    #   Input: 
+    #           q: quaternion. May be a vector of dimensions 4 x n
+    #   Output: 
+    #           rot_matrix: 3x3xn rotation matrix
+    
+    #   Yariv Aizenbud 31.01.2016
+    
+    n = np.size(q, axis=1)
+    rot_matrix = np.zeros((3,3,n))
+    
+    rot_matrix[0,0,:] = q[0,:]**2 + q[1,:]**2 - q[2,:]**2 - q[3,:]**2
+    rot_matrix[0,1,:] = 2*q[1,:]*q[2,:] - 2*q[0,:]*q[3,:] 
+    rot_matrix[0,2,:] = 2*q[0,:]*q[2,:] + 2*q[1,:]*q[3,:] 
+    
+    rot_matrix[1,0,:] = 2*q[1,:]*q[2,:] + 2*q[0,:]*q[3,:]
+    rot_matrix[1,1,:] = q[0,:]**2 - q[1,:]**2 + q[2,:]**2 - q[3,:]**2 
+    rot_matrix[1,2,:] = -2*q[0,:]*q[1,:] + 2*q[2,:]*q[3,:]
+    
+    rot_matrix[2,0,:] = -2*q[0,:]*q[2,:] + 2*q[1,:]*q[3,:] 
+    rot_matrix[2,1,:] = 2*q[0,:]*q[1,:] + 2*q[2,:]*q[3,:] 
+    rot_matrix[2,2,:] = q[0,:]**2 - q[1,:]**2 - q[2,:]**2 + q[3,:]**2
+    
+    return rot_matrix
+
+def rand_rots(n):
+    # rand_rots generate random rotations
+    # Input
+    #    n: The number of rotations to generate.
+    # Output
+    #    rot_matrices: An array of size 3-by-3-by-n containing n rotation matrices
+    #    sampled from the unifoorm distribution on SO(3).
+
+    qs = qrand(n)
+    rot_matrices = q_to_rot(qs)
+    
+    return rot_matrices
```

### Comparing `EMalign-1.0.3/src/read_write.py` & `EMalign-1.0.4/src/read_write.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# -*- coding: utf-8 -*-
-"""
-Spyder Editor
-
-This is a temporary script file.
-"""
-
-import mrcfile
-import numpy as np
-import shutil
-import os
-
-
-def write_mrc(file_path, x):
-    # For now it is transposed, when moving to C aligned this should be removed
-    with mrcfile.new(file_path, overwrite=True) as mrc_fh:
-        mrc_fh.set_data(x.astype('float32').T)
-    return
-
-
-def read_mrc(file_path):
-    return np.ascontiguousarray(mrcfile.open(file_path).data.T)
-
-
-def copy_and_rename(source_file, target_file):
-    # Copy vol2 first
-    target_destination, target_name = os.path.split(target_file)
-    source_destination, source_name = os.path.split(source_file)
-    intermidiate_file = os.path.join(target_destination, source_name)
-    if os.path.isfile(intermidiate_file):
-        # If the target directory has a file with this name create a temporary directory
-        i = 0
-        while True:
-            tmp_dir = os.path.join(target_destination, 'tmp{}'.format(i))
-            if os.path.isdir(tmp_dir):
-                i += 1
-            else:
-                os.mkdir(tmp_dir)
-                break
-
-        # Copy file to new dir and rename it
-        intermidiate_file = os.path.join(tmp_dir, source_name)
-        shutil.copy(source_file, tmp_dir)
-        os.rename(intermidiate_file, os.path.join(tmp_dir, target_name))
-
-        # Copy from tmp dir to the real dir
-        shutil.copy(os.path.join(tmp_dir, target_name), target_destination)
-
-        # Delete intermidiate file and directory
-        shutil.rmtree(tmp_dir)
-    else:
-        # Copy and rename
-        shutil.copy(source_file, target_destination)
-        os.rename(intermidiate_file, os.path.join(target_destination, target_name))
+# -*- coding: utf-8 -*-
+"""
+Spyder Editor
+
+This is a temporary script file.
+"""
+
+import mrcfile
+import numpy as np
+import shutil
+import os
+
+
+def write_mrc(file_path, x):
+    # For now it is transposed, when moving to C aligned this should be removed
+    with mrcfile.new(file_path, overwrite=True) as mrc_fh:
+        mrc_fh.set_data(x.astype('float32').T)
+    return
+
+
+def read_mrc(file_path):
+    return np.ascontiguousarray(mrcfile.open(file_path).data.T)
+
+
+def copy_and_rename(source_file, target_file):
+    # Copy vol2 first
+    target_destination, target_name = os.path.split(target_file)
+    source_destination, source_name = os.path.split(source_file)
+    intermidiate_file = os.path.join(target_destination, source_name)
+    if os.path.isfile(intermidiate_file):
+        # If the target directory has a file with this name create a temporary directory
+        i = 0
+        while True:
+            tmp_dir = os.path.join(target_destination, 'tmp{}'.format(i))
+            if os.path.isdir(tmp_dir):
+                i += 1
+            else:
+                os.mkdir(tmp_dir)
+                break
+
+        # Copy file to new dir and rename it
+        intermidiate_file = os.path.join(tmp_dir, source_name)
+        shutil.copy(source_file, tmp_dir)
+        os.rename(intermidiate_file, os.path.join(tmp_dir, target_name))
+
+        # Copy from tmp dir to the real dir
+        shutil.copy(os.path.join(tmp_dir, target_name), target_destination)
+
+        # Delete intermidiate file and directory
+        shutil.rmtree(tmp_dir)
+    else:
+        # Copy and rename
+        shutil.copy(source_file, target_destination)
+        os.rename(intermidiate_file, os.path.join(target_destination, target_name))
```

### Comparing `EMalign-1.0.3/src/register_translations_3d.py` & `EMalign-1.0.4/src/register_translations_3d.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Oct 18 21:00:50 2022
-
-@author: yoelsh
-"""
-
-import numpy as np
-from numpy import fft
-from src.reshift_vol import reshift_vol
-import src.reshift_vol
-from scipy.optimize import minimize
-import pyfftw
-
-
-class fftw_data_class:
-    def __init__(self, in_data, num_threads=1):
-        n = in_data.shape[0]
-        n2 = n//2 + 1
-
-        if in_data.dtype == np.float32:
-            real_type = np.float32
-            complex_type = np.complex64
-        else:
-            real_type = np.float64
-            complex_type = np.complex128
-
-        self.in_array_f = pyfftw.empty_aligned((n,n,n),dtype=real_type)
-        self.in_array_b = pyfftw.empty_aligned((n,n,n2),dtype=complex_type)
-        self.fftw_object_f = pyfftw.builders.rfftn(self.in_array_f)
-        self.fftw_object_b = pyfftw.builders.irfftn(self.in_array_b)
-
-
-# %%
-def eval3Dshift(X, vol1, vol2, reshift_cache):
-    dx = X[0]
-    dy = X[1]
-    dz = X[2]
-    vol2_s = reshift_vol(vol2, np.array([dx, dy, dz]), reshift_cache)
-    c = np.mean(np.corrcoef(vol1.ravel(), vol2_s.ravel(), rowvar=False)[0, 1:]).astype('float64')
-    e = 1.0 - c
-    return e
-
-
-# %%
-def refine3DshiftBFGS(vol1, vol2, estdx):
-    # Create initial guess vector
-    X0 = np.array([estdx[0].real, estdx[1].real, estdx[2].real]).astype('float64')
-    # BFGS optimization:
-        
-    reshift_cache = src.reshift_vol.fftw_data_class(vol1)
-    res = minimize(eval3Dshift, X0, args=(vol1, vol2, reshift_cache), 
-                   method='BFGS', tol=1e-3, 
-                   options={'gtol': 1e-1, 'disp': False})
-    X = res.x
-    estdx = np.array([X[0], X[1], X[2]])
-    return estdx
-
-
-# %%
-def register_translations_3d(vol1, vol2, fftw_object=None):
-    # REGISTER_TRANSLATIONS_3D  Estimate relative shift between two volumes.
-    # register_translations_3d(vol1,vol2,refdx)
-    #   Estimate the relative shift between two volumes vol1 and vol2 to 
-    #   integral pixel accuracy. The function uses phase correlation to 
-    #   estimate the relative shift to within one pixel accuray.
-    #
-    #   Input parameters:
-    #   vol1,vol2 Two volumes to register. Volumes must be odd-sized.
-    #   refidx    Two-dimensional vector with the true shift between the images,
-    #             used for debugging purposes. (Optional)
-    #   Output parameters
-    #   estidx  A two-dimensional vector of how much to shift vol2 to aligh it
-    #           with vol1. Returns -1 on error.
-    #   err     Difference between estidx and refidx.
-
-    # Take Fourer transform of both volumes and compute the phase correlation
-    # factors.
-    
-    if fftw_object is None:
-        fftw_object=fftw_data_class(vol1)
-    
-    #hats1 = fft.fftn(vol1)  # Compute centered Fourier transform
-    #hats2 = fft.fftn(vol2)
-
-    fftw_object.in_array_f[:] = vol1[:]
-    hats1 = (fftw_object.fftw_object_f(fftw_object.in_array_f)).copy()
-    fftw_object.in_array_f[:] = vol2[:]
-    hats2 = (fftw_object.fftw_object_f(fftw_object.in_array_f)).copy()
-
-    tmp1 = hats1 * np.conj(hats2)
-    tmp2 = abs(tmp1)
-    bool_idx = tmp2 < 2*np.finfo(vol1.dtype).eps
-    tmp2[bool_idx] = 1 # Avoid division by zero. 
-                       # The numerator for these indices is small anyway.
-    rhat =  tmp1 / tmp2
-    
-
-    # Compute the relative shift between the images to to within 1 pixel
-    # accuracy.
-    #r = fft.ifftn(rhat).real
-    fftw_object.in_array_b[:] = rhat[:]
-    r = fftw_object.fftw_object_b(fftw_object.in_array_b)
-    ii = np.argmax(r)
-
-    # Find the center
-    n = np.size(vol1, 0)
-    cX = np.fix(n / 2)
-    cY = np.fix(n / 2)
-    cZ = np.fix(n / 2)
-    [sX, sY, sZ] = np.unravel_index(ii, np.shape(r))
-    if sX>cX:
-        sX = sX - n
-    if sY>cY:
-        sY = sY - n
-    if sZ>cZ:
-        sZ = sZ - n
-
-    estdx = [-sX,-sY,-sZ]
-
-    # No need to refine tranlations
-    return np.array(estdx)
-
-    # bestdx = refine3DshiftBFGS(vol1, vol2, estdx)
-
-    # return bestdx
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Oct 18 21:00:50 2022
+
+@author: yoelsh
+"""
+
+import numpy as np
+from numpy import fft
+from src.reshift_vol import reshift_vol
+import src.reshift_vol
+from scipy.optimize import minimize
+import pyfftw
+
+
+class fftw_data_class:
+    def __init__(self, in_data, num_threads=1):
+        n = in_data.shape[0]
+        n2 = n//2 + 1
+
+        if in_data.dtype == np.float32:
+            real_type = np.float32
+            complex_type = np.complex64
+        else:
+            real_type = np.float64
+            complex_type = np.complex128
+
+        self.in_array_f = pyfftw.empty_aligned((n,n,n),dtype=real_type)
+        self.in_array_b = pyfftw.empty_aligned((n,n,n2),dtype=complex_type)
+        self.fftw_object_f = pyfftw.builders.rfftn(self.in_array_f)
+        self.fftw_object_b = pyfftw.builders.irfftn(self.in_array_b)
+
+
+# %%
+def eval3Dshift(X, vol1, vol2, reshift_cache):
+    dx = X[0]
+    dy = X[1]
+    dz = X[2]
+    vol2_s = reshift_vol(vol2, np.array([dx, dy, dz]), reshift_cache)
+    c = np.mean(np.corrcoef(vol1.ravel(), vol2_s.ravel(), rowvar=False)[0, 1:]).astype('float64')
+    e = 1.0 - c
+    return e
+
+
+# %%
+def refine3DshiftBFGS(vol1, vol2, estdx):
+    # Create initial guess vector
+    X0 = np.array([estdx[0].real, estdx[1].real, estdx[2].real]).astype('float64')
+    # BFGS optimization:
+        
+    reshift_cache = src.reshift_vol.fftw_data_class(vol1)
+    res = minimize(eval3Dshift, X0, args=(vol1, vol2, reshift_cache), 
+                   method='BFGS', tol=1e-3, 
+                   options={'gtol': 1e-1, 'disp': False})
+    X = res.x
+    estdx = np.array([X[0], X[1], X[2]])
+    return estdx
+
+
+# %%
+def register_translations_3d(vol1, vol2, fftw_object=None):
+    # REGISTER_TRANSLATIONS_3D  Estimate relative shift between two volumes.
+    # register_translations_3d(vol1,vol2,refdx)
+    #   Estimate the relative shift between two volumes vol1 and vol2 to 
+    #   integral pixel accuracy. The function uses phase correlation to 
+    #   estimate the relative shift to within one pixel accuray.
+    #
+    #   Input parameters:
+    #   vol1,vol2 Two volumes to register. Volumes must be odd-sized.
+    #   refidx    Two-dimensional vector with the true shift between the images,
+    #             used for debugging purposes. (Optional)
+    #   Output parameters
+    #   estidx  A two-dimensional vector of how much to shift vol2 to aligh it
+    #           with vol1. Returns -1 on error.
+    #   err     Difference between estidx and refidx.
+
+    # Take Fourer transform of both volumes and compute the phase correlation
+    # factors.
+    
+    if fftw_object is None:
+        fftw_object=fftw_data_class(vol1)
+    
+    #hats1 = fft.fftn(vol1)  # Compute centered Fourier transform
+    #hats2 = fft.fftn(vol2)
+
+    fftw_object.in_array_f[:] = vol1[:]
+    hats1 = (fftw_object.fftw_object_f(fftw_object.in_array_f)).copy()
+    fftw_object.in_array_f[:] = vol2[:]
+    hats2 = (fftw_object.fftw_object_f(fftw_object.in_array_f)).copy()
+
+    tmp1 = hats1 * np.conj(hats2)
+    tmp2 = abs(tmp1)
+    bool_idx = tmp2 < 2*np.finfo(vol1.dtype).eps
+    tmp2[bool_idx] = 1 # Avoid division by zero. 
+                       # The numerator for these indices is small anyway.
+    rhat =  tmp1 / tmp2
+    
+
+    # Compute the relative shift between the images to to within 1 pixel
+    # accuracy.
+    #r = fft.ifftn(rhat).real
+    fftw_object.in_array_b[:] = rhat[:]
+    r = fftw_object.fftw_object_b(fftw_object.in_array_b)
+    ii = np.argmax(r)
+
+    # Find the center
+    n = np.size(vol1, 0)
+    cX = np.fix(n / 2)
+    cY = np.fix(n / 2)
+    cZ = np.fix(n / 2)
+    [sX, sY, sZ] = np.unravel_index(ii, np.shape(r))
+    if sX>cX:
+        sX = sX - n
+    if sY>cY:
+        sY = sY - n
+    if sZ>cZ:
+        sZ = sZ - n
+
+    estdx = [-sX,-sY,-sZ]
+
+    # No need to refine tranlations
+    return np.array(estdx)
+
+    # bestdx = refine3DshiftBFGS(vol1, vol2, estdx)
+
+    # return bestdx
```

### Comparing `EMalign-1.0.3/src/reshift_vol.py` & `EMalign-1.0.4/src/reshift_vol.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,240 +1,240 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Dec  2 11:54:51 2021
-
-@author: yaelharpaz1
-"""
-
-import numpy as np
-from numpy import fft
-from numpy import linalg as LA
-import pyfftw
-#from scipy.interpolate import RegularGridInterpolator
-
-class fftw_data_class:
-    def __init__(self, in_data, num_threads=8):
-        n = in_data.shape[0]
-        n2 = n//2+1
-
-        if in_data.dtype == np.float32:
-            real_type = np.float32
-            complex_type = np.complex64
-        else:
-            real_type = np.float64
-            complex_type = np.complex128
-
-        self.in_array_f = pyfftw.empty_aligned((n,n,n),dtype=real_type)
-        self.in_array_b = pyfftw.empty_aligned((n,n,n2),dtype=complex_type)
-        self.fftw_object_f = pyfftw.builders.rfftn(self.in_array_f,threads=num_threads)
-        self.fftw_object_b = pyfftw.builders.irfftn(self.in_array_b,threads=num_threads)
-
-        self.n = n
-        ll = np.fix(n/2)
-        freqrng = np.arange(-ll,n-ll)
-        [omega_x,omega_y,omega_z] = np.meshgrid(freqrng,freqrng,freqrng,indexing='ij')  
-        self.omega_x = 2*np.pi*omega_x/n 
-        self.omega_y = 2*np.pi*omega_y/n
-        self.omega_z = 2*np.pi*omega_z/n   
-   
-
-#%% 
-def reshift_vol_ref(vol,s,fftw_data=None):
-    # Shift the volume given by im by the vector s using trigonometric
-    # interpolation. The volume im is of nxnxn, where n can be odi or even. The vector
-    # s\in \mathbb{R}^{3} contains the hshifts.
-    #
-    # Example: Shift the volume vol by 1 pixel in the x direction, 2 in the y
-    # direction, and 3 in the z direction
-    #
-    #       s = [1 2 3];
-    #       vols=shift_vol(vol,s);
-    #
-    # NOTE: I don't know if s=[0 0 1 ] shifts up or down, but this can be easily checked. Same issue for the other directions.  
-    if vol.ndim != 3:
-        raise ValueError("Input must be a 3D volume")
-    if (np.size(vol,0) != np.size(vol,1)) or (np.size(vol,1) != np.size(vol,2)):
-        raise ValueError("All three dimensions of the input must be equal")   
-    n = np.size(vol,0)
-    ll = np.fix(n/2)
-    freqrng = np.arange(-ll,n-ll)
-    [omega_x,omega_y,omega_z] = np.meshgrid(freqrng,freqrng,freqrng,indexing='ij')  
-    omega_x = 2*np.pi*omega_x/n 
-    omega_y = 2*np.pi*omega_y/n
-    omega_z = 2*np.pi*omega_z/n   
-    phase_x = np.exp(1j*omega_x*s[0])
-    phase_y = np.exp(1j*omega_y*s[1])
-    phase_z = np.exp(1j*omega_z*s[2])   
-    # Force conjugate symmetry. Otherwise this frequency component has no
-    # corresponding negative frequency to cancel out its imaginary part.
-    if np.mod(n,2) == 0:
-         phase_x[0,:,:] = np.real(phase_x[0,:,:])
-         phase_y[:,0,:] = np.real(phase_y[:,0,:])
-         phase_z[:,:,0] = np.real(phase_z[:,:,0])        
-    phases = phase_x*phase_y*phase_z
-    pim = fft.fftshift(fft.fftn(fft.ifftshift(vol)))
-    pim = pim*phases
-
-    svol = fft.fftshift(fft.ifftn(fft.ifftshift(pim))) 
-    if LA.norm(np.imag(svol[:]))/LA.norm(svol[:]) > 1.0e-8:
-        raise ValueError("Large imaginary components")
-    svol = np.real(svol)
-    return svol
-
-#%% 
-# def reshift_vol(vol,s,fftw_data=None):
-#     # Shift the volume given by im by the vector s using trigonometric
-#     # interpolation. The volume im is of nxnxn, where n can be odi or even. The vector
-#     # s\in \mathbb{R}^{3} contains the hshifts.
-#     #
-#     # Example: Shift the volume vol by 1 pixel in the x direction, 2 in the y
-#     # direction, and 3 in the z direction
-#     #
-#     #       s = [1 2 3];
-#     #       vols=shift_vol(vol,s);
-#     #
-#     # NOTE: I don't know if s=[0 0 1 ] shifts up or down, but this can be easily checked. Same issue for the other directions.  
-            
-#     if vol.ndim != 3:
-#         raise ValueError("Input must be a 3D volume")
-#     if (np.size(vol,0) != np.size(vol,1)) or (np.size(vol,1) != np.size(vol,2)):
-#         raise ValueError("All three dimension of the input must be equal")   
-
-#     if fftw_data is None:
-#         fftw_data = fftw_data_class(vol)
-        
-#     n = np.size(vol,0)
-#     if fftw_data.n != n: # Cache is invalid. Recreate.
-#         fftw_data = fftw_data_class(vol)
-        
-#     phase_x = np.exp(1j*fftw_data.omega_x*s[0])
-#     phase_y = np.exp(1j*fftw_data.omega_y*s[1])
-#     phase_z = np.exp(1j*fftw_data.omega_z*s[2])   
-#     # Force conjugate symmetry. Otherwise this frequency component has no
-#     # corresponding negative frequency to cancel out its imaginary part.
-#     if np.mod(n,2) == 0:
-#          phase_x[0,:,:] = np.real(phase_x[0,:,:])
-#          phase_y[:,0,:] = np.real(phase_y[:,0,:])
-#          phase_z[:,:,0] = np.real(phase_z[:,:,0])        
-#     phases = phase_x*phase_y*phase_z
-       
-#     vol1 = fft.ifftshift(vol)    
-#     pim1 = pyfftw.interfaces.numpy_fft.fftn(vol1)
-
-#     phases1 = fft.ifftshift(phases)    
-
-#     pim = pim1 * phases1
-#     svol = pyfftw.interfaces.numpy_fft.ifftn(pim)
-#     svol = fft.fftshift(svol)
-       
-#     if LA.norm(np.imag(svol[:]))/LA.norm(svol[:]) > 5.0e-7:
-#         raise ValueError("Large imaginary components")
-#     svol = np.real(svol)
-   
-#     # tmpvol = reshift_vol_ref(vol, s)
-#     # err = np.linalg.norm(tmpvol.ravel()-svol.ravel())/np.linalg.norm(tmpvol.ravel())
-#     # if err >5.0e-7:
-#     #     aaa=1
-       
-#     # assert(err<5.0e-7)
-#     return svol
-
-
-#%% 
-def reshift_vol(vol,s,fftw_data=None):
-    # Shift the volume given by im by the vector s using trigonometric
-    # interpolation. The volume im is of nxnxn, where n can be odi or even. The vector
-    # s\in \mathbb{R}^{3} contains the hshifts.
-    #
-    # Example: Shift the volume vol by 1 pixel in the x direction, 2 in the y
-    # direction, and 3 in the z direction
-    #
-    #       s = [1 2 3];
-    #       vols=shift_vol(vol,s);
-    #
-    # NOTE: I don't know if s=[0 0 1 ] shifts up or down, but this can be easily checked. Same issue for the other directions.  
-            
-    if vol.ndim != 3:
-        raise ValueError("Input must be a 3D volume")
-    if (np.size(vol,0) != np.size(vol,1)) or (np.size(vol,1) != np.size(vol,2)):
-        raise ValueError("All three dimension of the input must be equal")   
-
-    if fftw_data is None:
-        fftw_data = fftw_data_class(vol)
-        
-    n = np.size(vol,0)
-    if fftw_data.n != n: # Cache is invalid. Recreate.
-        fftw_data = fftw_data_class(vol)
-        
-    phase_x = np.exp(1j*fftw_data.omega_x*s[0])
-    phase_y = np.exp(1j*fftw_data.omega_y*s[1])
-    phase_z = np.exp(1j*fftw_data.omega_z*s[2])   
-    # Force conjugate symmetry. Otherwise this frequency component has no
-    # corresponding negative frequency to cancel out its imaginary part.
-    if np.mod(n,2) == 0:
-         phase_x[0,:,:] = np.real(phase_x[0,:,:])
-         phase_y[:,0,:] = np.real(phase_y[:,0,:])
-         phase_z[:,:,0] = np.real(phase_z[:,:,0])        
-    phases = phase_x*phase_y*phase_z
-        
-    vol1 = fft.ifftshift(vol)    
-    #pim1 = pyfftw.interfaces.numpy_fft.rfftn(vol1)
-    pim1 = fftw_data.fftw_object_f(vol1)
-
-    phases1 = fft.ifftshift(phases)    
-    n2 = n//2 + 1
-    phases1 = phases1[:,:,:n2]
-
-    pim = pim1 * phases1
-    #svol = pyfftw.interfaces.numpy_fft.irfftn(pim)
-    svol = fftw_data.fftw_object_b(pim)
-
-    svol = fft.fftshift(svol)
-           
-    if LA.norm(np.imag(svol[:]))/LA.norm(svol[:]) > 5.0e-7:
-        raise ValueError("Large imaginary components")
-    svol = np.real(svol)
-   
-    # tmpvol = reshift_vol_ref(vol, s)
-    # err = np.linalg.norm(tmpvol.ravel()-svol.ravel())/np.linalg.norm(tmpvol.ravel())
-    # if err >5.0e-7:
-    #     aaa=1
-       
-    # assert(err<5.0e-7)
-    return svol
-
-
-#%% 
-def reshift_vol_int(vol,s):
-    # Shift a volume by the vector s.
-    # s must be be a vector of integers. 
-    # For non integer shifts use reshift_vol
-
-    s = np.array(s)
-    if not (np.round(s) == s).all():
-        raise ValueError("s must be a vector of integers.")
-        
-    return np.roll(vol,(-s).astype(int),axis=[0,1,2])
-        
-
-#%% A failed attempt to speed up shifting using linear interpolation.
-#   It is slower than reshift_vol
-# 
-# def reshift_vol_linear_interp(vol,s):
-    
-#     # Shift accurately to the nearest integer pixel
-#     vol = reshift_vol(vol, np.round(s))
-    
-#     # Use linear interpolation to shift the volume the required fractional 
-#     # pixel
-#     s = s - np.round(s)
-#     n = vol.shape[0]
-#     r = np.array(range(n))
-#     x, y, z = np.meshgrid(r,r,r,indexing='ij')
-#     interp = RegularGridInterpolator((r,r,r),vol,bounds_error=False,fill_value=0,method='linear')
-#     pts = np.vstack((x,y,z)).reshape(3,-1).T
-#     svol=interp(pts+s)
-#     svol=svol.reshape(n,n,n)
-    
-#     return svol
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Dec  2 11:54:51 2021
+
+@author: yaelharpaz1
+"""
+
+import numpy as np
+from numpy import fft
+from numpy import linalg as LA
+import pyfftw
+#from scipy.interpolate import RegularGridInterpolator
+
+class fftw_data_class:
+    def __init__(self, in_data, num_threads=8):
+        n = in_data.shape[0]
+        n2 = n//2+1
+
+        if in_data.dtype == np.float32:
+            real_type = np.float32
+            complex_type = np.complex64
+        else:
+            real_type = np.float64
+            complex_type = np.complex128
+
+        self.in_array_f = pyfftw.empty_aligned((n,n,n),dtype=real_type)
+        self.in_array_b = pyfftw.empty_aligned((n,n,n2),dtype=complex_type)
+        self.fftw_object_f = pyfftw.builders.rfftn(self.in_array_f,threads=num_threads)
+        self.fftw_object_b = pyfftw.builders.irfftn(self.in_array_b,threads=num_threads)
+
+        self.n = n
+        ll = np.fix(n/2)
+        freqrng = np.arange(-ll,n-ll)
+        [omega_x,omega_y,omega_z] = np.meshgrid(freqrng,freqrng,freqrng,indexing='ij')  
+        self.omega_x = 2*np.pi*omega_x/n 
+        self.omega_y = 2*np.pi*omega_y/n
+        self.omega_z = 2*np.pi*omega_z/n   
+   
+
+#%% 
+def reshift_vol_ref(vol,s,fftw_data=None):
+    # Shift the volume given by im by the vector s using trigonometric
+    # interpolation. The volume im is of nxnxn, where n can be odi or even. The vector
+    # s\in \mathbb{R}^{3} contains the hshifts.
+    #
+    # Example: Shift the volume vol by 1 pixel in the x direction, 2 in the y
+    # direction, and 3 in the z direction
+    #
+    #       s = [1 2 3];
+    #       vols=shift_vol(vol,s);
+    #
+    # NOTE: I don't know if s=[0 0 1 ] shifts up or down, but this can be easily checked. Same issue for the other directions.  
+    if vol.ndim != 3:
+        raise ValueError("Input must be a 3D volume")
+    if (np.size(vol,0) != np.size(vol,1)) or (np.size(vol,1) != np.size(vol,2)):
+        raise ValueError("All three dimensions of the input must be equal")   
+    n = np.size(vol,0)
+    ll = np.fix(n/2)
+    freqrng = np.arange(-ll,n-ll)
+    [omega_x,omega_y,omega_z] = np.meshgrid(freqrng,freqrng,freqrng,indexing='ij')  
+    omega_x = 2*np.pi*omega_x/n 
+    omega_y = 2*np.pi*omega_y/n
+    omega_z = 2*np.pi*omega_z/n   
+    phase_x = np.exp(1j*omega_x*s[0])
+    phase_y = np.exp(1j*omega_y*s[1])
+    phase_z = np.exp(1j*omega_z*s[2])   
+    # Force conjugate symmetry. Otherwise this frequency component has no
+    # corresponding negative frequency to cancel out its imaginary part.
+    if np.mod(n,2) == 0:
+         phase_x[0,:,:] = np.real(phase_x[0,:,:])
+         phase_y[:,0,:] = np.real(phase_y[:,0,:])
+         phase_z[:,:,0] = np.real(phase_z[:,:,0])        
+    phases = phase_x*phase_y*phase_z
+    pim = fft.fftshift(fft.fftn(fft.ifftshift(vol)))
+    pim = pim*phases
+
+    svol = fft.fftshift(fft.ifftn(fft.ifftshift(pim))) 
+    if LA.norm(np.imag(svol[:]))/LA.norm(svol[:]) > 1.0e-8:
+        raise ValueError("Large imaginary components")
+    svol = np.real(svol)
+    return svol
+
+#%% 
+# def reshift_vol(vol,s,fftw_data=None):
+#     # Shift the volume given by im by the vector s using trigonometric
+#     # interpolation. The volume im is of nxnxn, where n can be odi or even. The vector
+#     # s\in \mathbb{R}^{3} contains the hshifts.
+#     #
+#     # Example: Shift the volume vol by 1 pixel in the x direction, 2 in the y
+#     # direction, and 3 in the z direction
+#     #
+#     #       s = [1 2 3];
+#     #       vols=shift_vol(vol,s);
+#     #
+#     # NOTE: I don't know if s=[0 0 1 ] shifts up or down, but this can be easily checked. Same issue for the other directions.  
+            
+#     if vol.ndim != 3:
+#         raise ValueError("Input must be a 3D volume")
+#     if (np.size(vol,0) != np.size(vol,1)) or (np.size(vol,1) != np.size(vol,2)):
+#         raise ValueError("All three dimension of the input must be equal")   
+
+#     if fftw_data is None:
+#         fftw_data = fftw_data_class(vol)
+        
+#     n = np.size(vol,0)
+#     if fftw_data.n != n: # Cache is invalid. Recreate.
+#         fftw_data = fftw_data_class(vol)
+        
+#     phase_x = np.exp(1j*fftw_data.omega_x*s[0])
+#     phase_y = np.exp(1j*fftw_data.omega_y*s[1])
+#     phase_z = np.exp(1j*fftw_data.omega_z*s[2])   
+#     # Force conjugate symmetry. Otherwise this frequency component has no
+#     # corresponding negative frequency to cancel out its imaginary part.
+#     if np.mod(n,2) == 0:
+#          phase_x[0,:,:] = np.real(phase_x[0,:,:])
+#          phase_y[:,0,:] = np.real(phase_y[:,0,:])
+#          phase_z[:,:,0] = np.real(phase_z[:,:,0])        
+#     phases = phase_x*phase_y*phase_z
+       
+#     vol1 = fft.ifftshift(vol)    
+#     pim1 = pyfftw.interfaces.numpy_fft.fftn(vol1)
+
+#     phases1 = fft.ifftshift(phases)    
+
+#     pim = pim1 * phases1
+#     svol = pyfftw.interfaces.numpy_fft.ifftn(pim)
+#     svol = fft.fftshift(svol)
+       
+#     if LA.norm(np.imag(svol[:]))/LA.norm(svol[:]) > 5.0e-7:
+#         raise ValueError("Large imaginary components")
+#     svol = np.real(svol)
+   
+#     # tmpvol = reshift_vol_ref(vol, s)
+#     # err = np.linalg.norm(tmpvol.ravel()-svol.ravel())/np.linalg.norm(tmpvol.ravel())
+#     # if err >5.0e-7:
+#     #     aaa=1
+       
+#     # assert(err<5.0e-7)
+#     return svol
+
+
+#%% 
+def reshift_vol(vol,s,fftw_data=None):
+    # Shift the volume given by im by the vector s using trigonometric
+    # interpolation. The volume im is of nxnxn, where n can be odi or even. The vector
+    # s\in \mathbb{R}^{3} contains the hshifts.
+    #
+    # Example: Shift the volume vol by 1 pixel in the x direction, 2 in the y
+    # direction, and 3 in the z direction
+    #
+    #       s = [1 2 3];
+    #       vols=shift_vol(vol,s);
+    #
+    # NOTE: I don't know if s=[0 0 1 ] shifts up or down, but this can be easily checked. Same issue for the other directions.  
+            
+    if vol.ndim != 3:
+        raise ValueError("Input must be a 3D volume")
+    if (np.size(vol,0) != np.size(vol,1)) or (np.size(vol,1) != np.size(vol,2)):
+        raise ValueError("All three dimension of the input must be equal")   
+
+    if fftw_data is None:
+        fftw_data = fftw_data_class(vol)
+        
+    n = np.size(vol,0)
+    if fftw_data.n != n: # Cache is invalid. Recreate.
+        fftw_data = fftw_data_class(vol)
+        
+    phase_x = np.exp(1j*fftw_data.omega_x*s[0])
+    phase_y = np.exp(1j*fftw_data.omega_y*s[1])
+    phase_z = np.exp(1j*fftw_data.omega_z*s[2])   
+    # Force conjugate symmetry. Otherwise this frequency component has no
+    # corresponding negative frequency to cancel out its imaginary part.
+    if np.mod(n,2) == 0:
+         phase_x[0,:,:] = np.real(phase_x[0,:,:])
+         phase_y[:,0,:] = np.real(phase_y[:,0,:])
+         phase_z[:,:,0] = np.real(phase_z[:,:,0])        
+    phases = phase_x*phase_y*phase_z
+        
+    vol1 = fft.ifftshift(vol)    
+    #pim1 = pyfftw.interfaces.numpy_fft.rfftn(vol1)
+    pim1 = fftw_data.fftw_object_f(vol1)
+
+    phases1 = fft.ifftshift(phases)    
+    n2 = n//2 + 1
+    phases1 = phases1[:,:,:n2]
+
+    pim = pim1 * phases1
+    #svol = pyfftw.interfaces.numpy_fft.irfftn(pim)
+    svol = fftw_data.fftw_object_b(pim)
+
+    svol = fft.fftshift(svol)
+           
+    if LA.norm(np.imag(svol[:]))/LA.norm(svol[:]) > 5.0e-7:
+        raise ValueError("Large imaginary components")
+    svol = np.real(svol)
+   
+    # tmpvol = reshift_vol_ref(vol, s)
+    # err = np.linalg.norm(tmpvol.ravel()-svol.ravel())/np.linalg.norm(tmpvol.ravel())
+    # if err >5.0e-7:
+    #     aaa=1
+       
+    # assert(err<5.0e-7)
+    return svol
+
+
+#%% 
+def reshift_vol_int(vol,s):
+    # Shift a volume by the vector s.
+    # s must be be a vector of integers. 
+    # For non integer shifts use reshift_vol
+
+    s = np.array(s)
+    if not (np.round(s) == s).all():
+        raise ValueError("s must be a vector of integers.")
+        
+    return np.roll(vol,(-s).astype(int),axis=[0,1,2])
+        
+
+#%% A failed attempt to speed up shifting using linear interpolation.
+#   It is slower than reshift_vol
+# 
+# def reshift_vol_linear_interp(vol,s):
+    
+#     # Shift accurately to the nearest integer pixel
+#     vol = reshift_vol(vol, np.round(s))
+    
+#     # Use linear interpolation to shift the volume the required fractional 
+#     # pixel
+#     s = s - np.round(s)
+#     n = vol.shape[0]
+#     r = np.array(range(n))
+#     x, y, z = np.meshgrid(r,r,r,indexing='ij')
+#     interp = RegularGridInterpolator((r,r,r),vol,bounds_error=False,fill_value=0,method='linear')
+#     pts = np.vstack((x,y,z)).reshape(3,-1).T
+#     svol=interp(pts+s)
+#     svol=svol.reshape(n,n,n)
+    
+#     return svol
```

