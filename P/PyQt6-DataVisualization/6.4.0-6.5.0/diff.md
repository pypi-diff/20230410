# Comparing `tmp/PyQt6_DataVisualization-6.4.0.tar.gz` & `tmp/PyQt6_DataVisualization-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_DataVisualization-6.4.0.tar", last modified: Fri Sep 30 10:27:12 2022, max compression
+gzip compressed data, was "PyQt6_DataVisualization-6.5.0.tar", last modified: Tue Apr  4 15:22:07 2023, max compression
```

## Comparing `PyQt6_DataVisualization-6.4.0.tar` & `PyQt6_DataVisualization-6.5.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.288896 PyQt6_DataVisualization-6.4.0/
--rw-r--r--   0 phil       (501) staff       (20)     4130 2022-09-30 10:27:11.655159 PyQt6_DataVisualization-6.4.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2022-09-30 10:27:11.494203 PyQt6_DataVisualization-6.4.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      322 2022-09-30 10:26:22.344462 PyQt6_DataVisualization-6.4.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1711 2022-09-30 10:27:12.289014 PyQt6_DataVisualization-6.4.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1354 2022-09-30 10:27:11.656100 PyQt6_DataVisualization-6.4.0/README
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.273225 PyQt6_DataVisualization-6.4.0/examples/
--rwxr-xr-x   0 phil       (501) staff       (20)    17259 2022-09-30 10:26:22.348800 PyQt6_DataVisualization-6.4.0/examples/bars.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.269816 PyQt6_DataVisualization-6.4.0/examples/custominput/
--rwxr-xr-x   0 phil       (501) staff       (20)     7671 2022-09-30 10:26:22.349618 PyQt6_DataVisualization-6.4.0/examples/custominput/custominput.py
--rw-r--r--   0 phil       (501) staff       (20)    28985 2022-09-30 10:26:22.350743 PyQt6_DataVisualization-6.4.0/examples/custominput/data.txt
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.271956 PyQt6_DataVisualization-6.4.0/examples/customproxy/
--rwxr-xr-x   0 phil       (501) staff       (20)     9930 2022-09-30 10:26:22.351409 PyQt6_DataVisualization-6.4.0/examples/customproxy/customproxy.py
--rw-r--r--   0 phil       (501) staff       (20)     1995 2022-09-30 10:26:22.352049 PyQt6_DataVisualization-6.4.0/examples/customproxy/raindata.txt
--rwxr-xr-x   0 phil       (501) staff       (20)     5944 2022-09-30 10:26:22.352639 PyQt6_DataVisualization-6.4.0/examples/itemmodel.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.270575 PyQt6_DataVisualization-6.4.0/examples/rotations/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.271133 PyQt6_DataVisualization-6.4.0/examples/rotations/mesh/
--rw-r--r--   0 phil       (501) staff       (20)    59358 2022-09-30 10:26:22.354091 PyQt6_DataVisualization-6.4.0/examples/rotations/mesh/largesphere.obj
--rw-r--r--   0 phil       (501) staff       (20)    11371 2022-09-30 10:26:22.354830 PyQt6_DataVisualization-6.4.0/examples/rotations/mesh/narrowarrow.obj
--rwxr-xr-x   0 phil       (501) staff       (20)     8199 2022-09-30 10:26:22.355598 PyQt6_DataVisualization-6.4.0/examples/rotations/rotations.py
--rwxr-xr-x   0 phil       (501) staff       (20)     9599 2022-09-30 10:26:22.356216 PyQt6_DataVisualization-6.4.0/examples/scatter.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.272882 PyQt6_DataVisualization-6.4.0/examples/surface/
--rw-r--r--   0 phil       (501) staff       (20)    34540 2022-09-30 10:26:22.357111 PyQt6_DataVisualization-6.4.0/examples/surface/mountain.png
--rwxr-xr-x   0 phil       (501) staff       (20)    14938 2022-09-30 10:26:22.357825 PyQt6_DataVisualization-6.4.0/examples/surface/surface.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.273691 PyQt6_DataVisualization-6.4.0/examples/volumetric/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.274605 PyQt6_DataVisualization-6.4.0/examples/volumetric/heightmaps/
--rw-r--r--   0 phil       (501) staff       (20)    62477 2022-09-30 10:26:22.359575 PyQt6_DataVisualization-6.4.0/examples/volumetric/heightmaps/layer_ground.png
--rw-r--r--   0 phil       (501) staff       (20)    16550 2022-09-30 10:26:22.360538 PyQt6_DataVisualization-6.4.0/examples/volumetric/heightmaps/layer_magma.png
--rw-r--r--   0 phil       (501) staff       (20)    10181 2022-09-30 10:26:22.361354 PyQt6_DataVisualization-6.4.0/examples/volumetric/heightmaps/layer_water.png
--rwxr-xr-x   0 phil       (501) staff       (20)    36700 2022-09-30 10:26:22.362426 PyQt6_DataVisualization-6.4.0/examples/volumetric/volumetric.py
--rw-r--r--   0 phil       (501) staff       (20)      861 2022-09-30 10:27:11.656416 PyQt6_DataVisualization-6.4.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.275218 PyQt6_DataVisualization-6.4.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:27:12.288621 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/
--rw-r--r--   0 phil       (501) staff       (20)     3419 2022-09-30 10:27:12.055784 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/QtDataVisualizationmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3181 2022-09-30 10:27:12.090317 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dbars.sip
--rw-r--r--   0 phil       (501) staff       (20)     3278 2022-09-30 10:27:12.057835 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dcamera.sip
--rw-r--r--   0 phil       (501) staff       (20)     1988 2022-09-30 10:27:12.053504 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dinputhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1272 2022-09-30 10:27:12.093039 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1449 2022-09-30 10:27:12.095085 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     1997 2022-09-30 10:27:12.056322 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dscatter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2763 2022-09-30 10:27:12.060741 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dscene.sip
--rw-r--r--   0 phil       (501) staff       (20)     2143 2022-09-30 10:27:12.089607 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dsurface.sip
--rw-r--r--   0 phil       (501) staff       (20)     7480 2022-09-30 10:27:12.050237 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dtheme.sip
--rw-r--r--   0 phil       (501) staff       (20)     2550 2022-09-30 10:27:12.050900 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstract3daxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     6233 2022-09-30 10:27:12.091413 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstract3dgraph.sip
--rw-r--r--   0 phil       (501) staff       (20)     2344 2022-09-30 10:27:12.048705 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstract3dinputhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     3949 2022-09-30 10:27:12.061488 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstract3dseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1314 2022-09-30 10:27:12.054509 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstractdataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1987 2022-09-30 10:27:12.054047 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qbar3dseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1343 2022-09-30 10:27:12.096615 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qbardataitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     3390 2022-09-30 10:27:12.055142 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qbardataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1302 2022-09-30 10:27:12.094635 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qcategory3daxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2692 2022-09-30 10:27:12.048124 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qcustom3ditem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2209 2022-09-30 10:27:12.095575 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qcustom3dlabel.sip
--rw-r--r--   0 phil       (501) staff       (20)     7271 2022-09-30 10:27:12.059170 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qcustom3dvolume.sip
--rw-r--r--   0 phil       (501) staff       (20)     2871 2022-09-30 10:27:12.097233 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qheightmapsurfacedataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     5828 2022-09-30 10:27:12.047464 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qitemmodelbardataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     3934 2022-09-30 10:27:12.096185 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qitemmodelscatterdataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     6348 2022-09-30 10:27:12.057136 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qitemmodelsurfacedataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     4388 2022-09-30 10:27:12.094200 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1849 2022-09-30 10:27:12.091969 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qlogvalue3daxisformatter.sip
--rw-r--r--   0 phil       (501) staff       (20)     1706 2022-09-30 10:27:12.052432 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qscatter3dseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1616 2022-09-30 10:27:12.060168 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qscatterdataitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2190 2022-09-30 10:27:12.092548 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qscatterdataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     2766 2022-09-30 10:27:12.089006 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qsurface3dseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1453 2022-09-30 10:27:12.051931 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qsurfacedataitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2615 2022-09-30 10:27:12.052995 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qsurfacedataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1261 2022-09-30 10:27:12.097648 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qtouch3dinputhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1068 2022-09-30 10:27:12.049137 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qutils.sip
--rw-r--r--   0 phil       (501) staff       (20)     1835 2022-09-30 10:27:12.059692 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qvalue3daxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2019 2022-09-30 10:27:12.051452 PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qvalue3daxisformatter.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.208363 PyQt6_DataVisualization-6.5.0/
+-rw-r--r--   0 phil       (501) staff       (20)     4350 2023-04-04 15:22:06.571153 PyQt6_DataVisualization-6.5.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2023-04-04 15:22:06.405542 PyQt6_DataVisualization-6.5.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      377 2023-04-04 15:21:14.839851 PyQt6_DataVisualization-6.5.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1711 2023-04-04 15:22:07.208520 PyQt6_DataVisualization-6.5.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1354 2023-04-04 15:22:06.572104 PyQt6_DataVisualization-6.5.0/README
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.190410 PyQt6_DataVisualization-6.5.0/examples/
+-rwxr-xr-x   0 phil       (501) staff       (20)    17259 2023-04-04 15:21:14.845340 PyQt6_DataVisualization-6.5.0/examples/bars.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.186899 PyQt6_DataVisualization-6.5.0/examples/custominput/
+-rwxr-xr-x   0 phil       (501) staff       (20)     7671 2023-04-04 15:21:14.846289 PyQt6_DataVisualization-6.5.0/examples/custominput/custominput.py
+-rw-r--r--   0 phil       (501) staff       (20)    28985 2023-04-04 15:21:14.847447 PyQt6_DataVisualization-6.5.0/examples/custominput/data.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.189065 PyQt6_DataVisualization-6.5.0/examples/customproxy/
+-rwxr-xr-x   0 phil       (501) staff       (20)     9930 2023-04-04 15:21:14.848154 PyQt6_DataVisualization-6.5.0/examples/customproxy/customproxy.py
+-rw-r--r--   0 phil       (501) staff       (20)     1995 2023-04-04 15:21:14.848765 PyQt6_DataVisualization-6.5.0/examples/customproxy/raindata.txt
+-rwxr-xr-x   0 phil       (501) staff       (20)     5944 2023-04-04 15:21:14.849440 PyQt6_DataVisualization-6.5.0/examples/itemmodel.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.187706 PyQt6_DataVisualization-6.5.0/examples/rotations/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.188225 PyQt6_DataVisualization-6.5.0/examples/rotations/mesh/
+-rw-r--r--   0 phil       (501) staff       (20)    59358 2023-04-04 15:21:14.850817 PyQt6_DataVisualization-6.5.0/examples/rotations/mesh/largesphere.obj
+-rw-r--r--   0 phil       (501) staff       (20)    11371 2023-04-04 15:21:14.851484 PyQt6_DataVisualization-6.5.0/examples/rotations/mesh/narrowarrow.obj
+-rwxr-xr-x   0 phil       (501) staff       (20)     8199 2023-04-04 15:21:14.852122 PyQt6_DataVisualization-6.5.0/examples/rotations/rotations.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     9599 2023-04-04 15:21:14.852787 PyQt6_DataVisualization-6.5.0/examples/scatter.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.190028 PyQt6_DataVisualization-6.5.0/examples/surface/
+-rw-r--r--   0 phil       (501) staff       (20)    34540 2023-04-04 15:21:14.853708 PyQt6_DataVisualization-6.5.0/examples/surface/mountain.png
+-rwxr-xr-x   0 phil       (501) staff       (20)    14938 2023-04-04 15:21:14.854394 PyQt6_DataVisualization-6.5.0/examples/surface/surface.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.190980 PyQt6_DataVisualization-6.5.0/examples/volumetric/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.192097 PyQt6_DataVisualization-6.5.0/examples/volumetric/heightmaps/
+-rw-r--r--   0 phil       (501) staff       (20)    62477 2023-04-04 15:21:14.855894 PyQt6_DataVisualization-6.5.0/examples/volumetric/heightmaps/layer_ground.png
+-rw-r--r--   0 phil       (501) staff       (20)    16550 2023-04-04 15:21:14.856799 PyQt6_DataVisualization-6.5.0/examples/volumetric/heightmaps/layer_magma.png
+-rw-r--r--   0 phil       (501) staff       (20)    10181 2023-04-04 15:21:14.857666 PyQt6_DataVisualization-6.5.0/examples/volumetric/heightmaps/layer_water.png
+-rwxr-xr-x   0 phil       (501) staff       (20)    36700 2023-04-04 15:21:14.858519 PyQt6_DataVisualization-6.5.0/examples/volumetric/volumetric.py
+-rw-r--r--   0 phil       (501) staff       (20)      861 2023-04-04 15:22:06.572411 PyQt6_DataVisualization-6.5.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.192664 PyQt6_DataVisualization-6.5.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:22:07.208010 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/
+-rw-r--r--   0 phil       (501) staff       (20)     3445 2023-04-04 15:22:06.972336 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/QtDataVisualizationmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3181 2023-04-04 15:22:07.006299 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dbars.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3278 2023-04-04 15:22:06.974348 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dcamera.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1988 2023-04-04 15:22:06.969995 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dinputhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1272 2023-04-04 15:22:07.008688 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1449 2023-04-04 15:22:07.010633 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1997 2023-04-04 15:22:06.972832 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dscatter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2763 2023-04-04 15:22:06.977262 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dscene.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2143 2023-04-04 15:22:07.005670 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dsurface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7480 2023-04-04 15:22:06.966765 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dtheme.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2550 2023-04-04 15:22:06.967414 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstract3daxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6233 2023-04-04 15:22:07.007270 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstract3dgraph.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2344 2023-04-04 15:22:06.965273 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstract3dinputhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3949 2023-04-04 15:22:06.977988 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstract3dseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1314 2023-04-04 15:22:06.971043 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstractdataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1987 2023-04-04 15:22:06.970557 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qbar3dseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1343 2023-04-04 15:22:07.012147 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qbardataitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3390 2023-04-04 15:22:06.971694 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qbardataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1302 2023-04-04 15:22:07.010188 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qcategory3daxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2692 2023-04-04 15:22:06.964730 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qcustom3ditem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2209 2023-04-04 15:22:07.011137 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qcustom3dlabel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7271 2023-04-04 15:22:06.975707 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qcustom3dvolume.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2871 2023-04-04 15:22:07.012975 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qheightmapsurfacedataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5828 2023-04-04 15:22:06.964127 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qitemmodelbardataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3934 2023-04-04 15:22:07.011736 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qitemmodelscatterdataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6348 2023-04-04 15:22:06.973654 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qitemmodelsurfacedataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4388 2023-04-04 15:22:07.009761 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1849 2023-04-04 15:22:07.007768 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qlogvalue3daxisformatter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1706 2023-04-04 15:22:06.968915 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qscatter3dseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1616 2023-04-04 15:22:06.976703 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qscatterdataitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2190 2023-04-04 15:22:07.008262 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qscatterdataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2766 2023-04-04 15:22:07.005136 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qsurface3dseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1453 2023-04-04 15:22:06.968407 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qsurfacedataitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2615 2023-04-04 15:22:06.969482 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qsurfacedataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1261 2023-04-04 15:22:07.013352 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qtouch3dinputhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1068 2023-04-04 15:22:06.965680 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qutils.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1835 2023-04-04 15:22:06.976213 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qvalue3daxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2019 2023-04-04 15:22:06.967934 PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qvalue3daxisformatter.sip
```

### Comparing `PyQt6_DataVisualization-6.4.0/ChangeLog` & `PyQt6_DataVisualization-6.5.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+2023-03-31  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-DataVisualization.msp:
+	Updated for Qt v6.5.0rc.
+	[f93c93b4661a] [6.5.0]
+
 2022-09-30  Phil Thompson  <phil@riverbankcomputing.com>
 
+	* .hgtags:
+	Added tag 6.4.0 for changeset af6451080821
+	[0ed23912fa45]
+
 	* NEWS:
 	Updated for Qt v6.4.0.
 	[af6451080821] [6.4.0]
 
 2022-09-21  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-DataVisualization.msp:
```

### Comparing `PyQt6_DataVisualization-6.4.0/LICENSE` & `PyQt6_DataVisualization-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/PKG-INFO` & `PyQt6_DataVisualization-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-DataVisualization
-Version: 6.4.0
+Version: 6.5.0
 Requires-Python: >=3.7
 Summary: Python bindings for the Qt Data Visualization library
 Home-Page: https://www.riverbankcomputing.com/software/pyqtdatavisualization/
 Author: Riverbank Computing Limited
 Author-Email: info@riverbankcomputing.com
 License: GPL v3
 Requires-Dist: PyQt6 (>=6.2.0)
```

### Comparing `PyQt6_DataVisualization-6.4.0/README` & `PyQt6_DataVisualization-6.5.0/README`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/bars.py` & `PyQt6_DataVisualization-6.5.0/examples/bars.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/custominput/custominput.py` & `PyQt6_DataVisualization-6.5.0/examples/custominput/custominput.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/custominput/data.txt` & `PyQt6_DataVisualization-6.5.0/examples/custominput/data.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/customproxy/customproxy.py` & `PyQt6_DataVisualization-6.5.0/examples/customproxy/customproxy.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/customproxy/raindata.txt` & `PyQt6_DataVisualization-6.5.0/examples/customproxy/raindata.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/itemmodel.py` & `PyQt6_DataVisualization-6.5.0/examples/itemmodel.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/rotations/mesh/largesphere.obj` & `PyQt6_DataVisualization-6.5.0/examples/rotations/mesh/largesphere.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/rotations/mesh/narrowarrow.obj` & `PyQt6_DataVisualization-6.5.0/examples/rotations/mesh/narrowarrow.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/rotations/rotations.py` & `PyQt6_DataVisualization-6.5.0/examples/rotations/rotations.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/scatter.py` & `PyQt6_DataVisualization-6.5.0/examples/scatter.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/surface/mountain.png` & `PyQt6_DataVisualization-6.5.0/examples/surface/mountain.png`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/surface/surface.py` & `PyQt6_DataVisualization-6.5.0/examples/surface/surface.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/volumetric/heightmaps/layer_ground.png` & `PyQt6_DataVisualization-6.5.0/examples/volumetric/heightmaps/layer_ground.png`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/volumetric/heightmaps/layer_magma.png` & `PyQt6_DataVisualization-6.5.0/examples/volumetric/heightmaps/layer_magma.png`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/volumetric/heightmaps/layer_water.png` & `PyQt6_DataVisualization-6.5.0/examples/volumetric/heightmaps/layer_water.png`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/examples/volumetric/volumetric.py` & `PyQt6_DataVisualization-6.5.0/examples/volumetric/volumetric.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.4.0/pyproject.toml` & `PyQt6_DataVisualization-6.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["sip >=6, <7", "PyQt-builder >=1.10, <2"]
 build-backend = "sipbuild.api"
 
 # Specify the PEP 566 metadata for the project.
 [tool.sip.metadata]
 name = "PyQt6-DataVisualization"
-version = "6.4.0"
+version = "6.5.0"
 summary = "Python bindings for the Qt Data Visualization library"
 home-page = "https://www.riverbankcomputing.com/software/pyqtdatavisualization/"
 author = "Riverbank Computing Limited"
 author-email = "info@riverbankcomputing.com"
 license = "GPL v3"
 description-file = "README"
 requires-dist = "PyQt6 (>=6.2.0)"
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/QtDataVisualizationmod.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/QtDataVisualizationmod.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtDataVisualizationmod.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -20,18 +20,18 @@
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 %Module(name=PyQt6.QtDataVisualization, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtGui/QtGuimod.sip
 
-%Timeline {QtDataVisualization_6_0_0 QtDataVisualization_6_1_0 QtDataVisualization_6_2_0 QtDataVisualization_6_3_0 QtDataVisualization_6_4_0}
+%Timeline {QtDataVisualization_6_0_0 QtDataVisualization_6_1_0 QtDataVisualization_6_2_0 QtDataVisualization_6_3_0 QtDataVisualization_6_4_0 QtDataVisualization_6_5_0}
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-DataVisualization.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -47,16 +47,16 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_DATAVISUALIZATION_VERSION;
 const char *PYQT_DATAVISUALIZATION_VERSION_STR;
 
 %ModuleCode
-static int PYQT_DATAVISUALIZATION_VERSION = 0x060400;
-static const char *PYQT_DATAVISUALIZATION_VERSION_STR = "6.4.0";
+static int PYQT_DATAVISUALIZATION_VERSION = 0x060500;
+static const char *PYQT_DATAVISUALIZATION_VERSION_STR = "6.5.0";
 %End
 
 %Include q3dbars.sip
 %Include q3dcamera.sip
 %Include q3dinputhandler.sip
 %Include q3dlight.sip
 %Include q3dobject.sip
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dbars.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dbars.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dbars.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dcamera.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dcamera.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dcamera.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dinputhandler.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dinputhandler.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dinputhandler.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dlight.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dlight.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dlight.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dobject.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dobject.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dobject.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dscatter.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dscatter.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dscatter.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dscene.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dscene.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dscene.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dsurface.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dsurface.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dsurface.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/q3dtheme.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/q3dtheme.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dtheme.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstract3daxis.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstract3daxis.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstract3daxis.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstract3dgraph.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstract3dgraph.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstract3dgraph.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstract3dinputhandler.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstract3dinputhandler.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstract3dinputhandler.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstract3dseries.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstract3dseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstract3dseries.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qabstractdataproxy.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qabstractdataproxy.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractdataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qbar3dseries.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qbar3dseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbar3dseries.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qbardataitem.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qbardataitem.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbardataitem.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qbardataproxy.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qbardataproxy.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbardataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qcategory3daxis.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qcategory3daxis.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcategory3daxis.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qcustom3ditem.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qcustom3ditem.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcustom3ditem.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qcustom3dlabel.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qcustom3dlabel.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcustom3dlabel.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qcustom3dvolume.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qcustom3dvolume.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcustom3dvolume.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qheightmapsurfacedataproxy.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qheightmapsurfacedataproxy.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qheightmapsurfacedataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qitemmodelbardataproxy.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qitemmodelbardataproxy.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qitemmodelbardataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qitemmodelscatterdataproxy.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qitemmodelscatterdataproxy.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qitemmodelscatterdataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qitemmodelsurfacedataproxy.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qitemmodelsurfacedataproxy.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qitemmodelsurfacedataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qlist.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qlist.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 // This is the SIP interface definition for the QList based mapped types.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qlogvalue3daxisformatter.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qlogvalue3daxisformatter.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlogvalue3daxisformatter.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qscatter3dseries.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qscatter3dseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscatter3dseries.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qscatterdataitem.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qscatterdataitem.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscatterdataitem.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qscatterdataproxy.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qscatterdataproxy.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscatterdataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qsurface3dseries.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qsurface3dseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsurface3dseries.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qsurfacedataitem.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qsurfacedataitem.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsurfacedataitem.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qsurfacedataproxy.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qsurfacedataproxy.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsurfacedataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qtouch3dinputhandler.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qtouch3dinputhandler.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtouch3dinputhandler.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qutils.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qutils.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qutils.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qvalue3daxis.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qvalue3daxis.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvalue3daxis.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.4.0/sip/QtDataVisualization/qvalue3daxisformatter.sip` & `PyQt6_DataVisualization-6.5.0/sip/QtDataVisualization/qvalue3daxisformatter.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvalue3daxisformatter.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

