# Comparing `tmp/PyQt6_3D-6.4.0.tar.gz` & `tmp/PyQt6_3D-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_3D-6.4.0.tar", last modified: Fri Sep 30 10:24:54 2022, max compression
+gzip compressed data, was "PyQt6_3D-6.5.0.tar", last modified: Tue Apr  4 15:19:42 2023, max compression
```

## Comparing `PyQt6_3D-6.4.0.tar` & `PyQt6_3D-6.5.0.tar`

### file list

```diff
@@ -1,355 +1,355 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.924523 PyQt6_3D-6.4.0/
--rw-r--r--   0 phil       (501) staff       (20)     9768 2022-09-30 10:24:53.368441 PyQt6_3D-6.4.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2022-09-30 10:24:53.191142 PyQt6_3D-6.4.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      578 2022-09-30 10:20:37.276480 PyQt6_3D-6.4.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1578 2022-09-30 10:24:54.924639 PyQt6_3D-6.4.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1265 2022-09-30 10:24:53.369466 PyQt6_3D-6.4.0/README
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.798790 PyQt6_3D-6.4.0/examples/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.828290 PyQt6_3D-6.4.0/examples/assets/
--rw-r--r--   0 phil       (501) staff       (20)      136 2022-09-30 10:20:37.289838 PyQt6_3D-6.4.0/examples/assets/LICENSE
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.827785 PyQt6_3D-6.4.0/examples/assets/chest/
--rw-r--r--   0 phil       (501) staff       (20)    46344 2022-09-30 10:20:37.291408 PyQt6_3D-6.4.0/examples/assets/chest/Chest.obj
--rw-r--r--   0 phil       (501) staff       (20)    70980 2022-09-30 10:20:37.292887 PyQt6_3D-6.4.0/examples/assets/chest/diffuse.webp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.810365 PyQt6_3D-6.4.0/examples/assets/cubemaps/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.809830 PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/
--rw-r--r--   0 phil       (501) staff       (20)      293 2022-09-30 10:20:37.294119 PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/README.TXT
--rw-r--r--   0 phil       (501) staff       (20)   121754 2022-09-30 10:20:37.296176 PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_negx.webp
--rw-r--r--   0 phil       (501) staff       (20)     1926 2022-09-30 10:20:37.297075 PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_negy.webp
--rw-r--r--   0 phil       (501) staff       (20)   147696 2022-09-30 10:20:37.299803 PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_negz.webp
--rw-r--r--   0 phil       (501) staff       (20)   136426 2022-09-30 10:20:37.302354 PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_posx.webp
--rw-r--r--   0 phil       (501) staff       (20)    57622 2022-09-30 10:20:37.303750 PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_posy.webp
--rw-r--r--   0 phil       (501) staff       (20)   164564 2022-09-30 10:20:37.306485 PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_posz.webp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.812382 PyQt6_3D-6.4.0/examples/assets/cubemaps/night/
--rw-r--r--   0 phil       (501) staff       (20)    38042 2022-09-30 10:20:37.307871 PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_negx.webp
--rw-r--r--   0 phil       (501) staff       (20)    42278 2022-09-30 10:20:37.308929 PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_negy.webp
--rw-r--r--   0 phil       (501) staff       (20)    36790 2022-09-30 10:20:37.310208 PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_negz.webp
--rw-r--r--   0 phil       (501) staff       (20)    37092 2022-09-30 10:20:37.311500 PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_posx.webp
--rw-r--r--   0 phil       (501) staff       (20)    26008 2022-09-30 10:20:37.312555 PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_posy.webp
--rw-r--r--   0 phil       (501) staff       (20)    37802 2022-09-30 10:20:37.313643 PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_posz.webp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.813306 PyQt6_3D-6.4.0/examples/assets/gltf/
--rw-r--r--   0 phil       (501) staff       (20)     1831 2022-09-30 10:20:37.314517 PyQt6_3D-6.4.0/examples/assets/gltf/LICENSE.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.818690 PyQt6_3D-6.4.0/examples/assets/gltf/wine/
--rw-r--r--   0 phil       (501) staff       (20)     8798 2022-09-30 10:20:37.315649 PyQt6_3D-6.4.0/examples/assets/gltf/wine/Wood_Cherry_Original_.jpg
--rw-r--r--   0 phil       (501) staff       (20)    46051 2022-09-30 10:20:37.317224 PyQt6_3D-6.4.0/examples/assets/gltf/wine/_2004_old_vine_zinfandel_btl_xlg.jpg
--rw-r--r--   0 phil       (501) staff       (20)    35585 2022-09-30 10:20:37.318634 PyQt6_3D-6.4.0/examples/assets/gltf/wine/artezin_bottle.jpg
--rw-r--r--   0 phil       (501) staff       (20)   329088 2022-09-30 10:20:37.323213 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine.bin
--rw-r--r--   0 phil       (501) staff       (20)   797366 2022-09-30 10:20:37.332238 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine.dae
--rw-r--r--   0 phil       (501) staff       (20)   275432 2022-09-30 10:20:37.335341 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine.gltf
--rw-r--r--   0 phil       (501) staff       (20)      497 2022-09-30 10:20:37.336331 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine0FS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      439 2022-09-30 10:20:37.337341 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine0VS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      489 2022-09-30 10:20:37.338193 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine1FS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      355 2022-09-30 10:20:37.338994 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine1VS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      219 2022-09-30 10:20:37.339773 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine2FS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      236 2022-09-30 10:20:37.340546 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine2VS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      441 2022-09-30 10:20:37.341400 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine3FS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      355 2022-09-30 10:20:37.342196 PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine3VS.glsl
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.846444 PyQt6_3D-6.4.0/examples/assets/houseplants/
--rw-r--r--   0 phil       (501) staff       (20)    13846 2022-09-30 10:20:37.343336 PyQt6_3D-6.4.0/examples/assets/houseplants/bamboo.webp
--rw-r--r--   0 phil       (501) staff       (20)    16614 2022-09-30 10:20:37.344299 PyQt6_3D-6.4.0/examples/assets/houseplants/bamboo_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    89192 2022-09-30 10:20:37.345936 PyQt6_3D-6.4.0/examples/assets/houseplants/cover.webp
--rw-r--r--   0 phil       (501) staff       (20)    21098 2022-09-30 10:20:37.346992 PyQt6_3D-6.4.0/examples/assets/houseplants/cover_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    44264 2022-09-30 10:20:37.348442 PyQt6_3D-6.4.0/examples/assets/houseplants/cross-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36076 2022-09-30 10:20:37.349720 PyQt6_3D-6.4.0/examples/assets/houseplants/cross-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9324 2022-09-30 10:20:37.350684 PyQt6_3D-6.4.0/examples/assets/houseplants/cross-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1822 2022-09-30 10:20:37.351561 PyQt6_3D-6.4.0/examples/assets/houseplants/cross-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)     8863 2022-09-30 10:20:37.352492 PyQt6_3D-6.4.0/examples/assets/houseplants/cross-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15838 2022-09-30 10:20:37.353586 PyQt6_3D-6.4.0/examples/assets/houseplants/cross-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2216 2022-09-30 10:20:37.354491 PyQt6_3D-6.4.0/examples/assets/houseplants/cross-spikes.obj
--rw-r--r--   0 phil       (501) staff       (20)    51505 2022-09-30 10:20:37.355959 PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36078 2022-09-30 10:20:37.358372 PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9328 2022-09-30 10:20:37.359362 PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1820 2022-09-30 10:20:37.360206 PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)     9026 2022-09-30 10:20:37.361134 PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15842 2022-09-30 10:20:37.362250 PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2216 2022-09-30 10:20:37.363160 PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-spikes.obj
--rw-r--r--   0 phil       (501) staff       (20)    33756 2022-09-30 10:20:37.364402 PyQt6_3D-6.4.0/examples/assets/houseplants/palm.webp
--rw-r--r--   0 phil       (501) staff       (20)    36186 2022-09-30 10:20:37.365571 PyQt6_3D-6.4.0/examples/assets/houseplants/palm_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)   120426 2022-09-30 10:20:37.367350 PyQt6_3D-6.4.0/examples/assets/houseplants/pine.webp
--rw-r--r--   0 phil       (501) staff       (20)    47352 2022-09-30 10:20:37.368591 PyQt6_3D-6.4.0/examples/assets/houseplants/pine_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)   366144 2022-09-30 10:20:37.381045 PyQt6_3D-6.4.0/examples/assets/houseplants/pot.webp
--rw-r--r--   0 phil       (501) staff       (20)    50950 2022-09-30 10:20:37.419678 PyQt6_3D-6.4.0/examples/assets/houseplants/pot_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    33100 2022-09-30 10:20:37.420708 PyQt6_3D-6.4.0/examples/assets/houseplants/shrub.webp
--rw-r--r--   0 phil       (501) staff       (20)    10180 2022-09-30 10:20:37.421476 PyQt6_3D-6.4.0/examples/assets/houseplants/shrub_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    51509 2022-09-30 10:20:37.422741 PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36082 2022-09-30 10:20:37.423818 PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9328 2022-09-30 10:20:37.424577 PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1820 2022-09-30 10:20:37.425281 PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)    46455 2022-09-30 10:20:37.426360 PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15842 2022-09-30 10:20:37.427253 PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2220 2022-09-30 10:20:37.428027 PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-spikes.obj
--rw-r--r--   0 phil       (501) staff       (20)    30338 2022-09-30 10:20:37.428916 PyQt6_3D-6.4.0/examples/assets/houseplants/spikes.webp
--rw-r--r--   0 phil       (501) staff       (20)    12028 2022-09-30 10:20:37.429744 PyQt6_3D-6.4.0/examples/assets/houseplants/spikes_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    51509 2022-09-30 10:20:37.430968 PyQt6_3D-6.4.0/examples/assets/houseplants/square-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36082 2022-09-30 10:20:37.431980 PyQt6_3D-6.4.0/examples/assets/houseplants/square-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9328 2022-09-30 10:20:37.432702 PyQt6_3D-6.4.0/examples/assets/houseplants/square-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1824 2022-09-30 10:20:37.433441 PyQt6_3D-6.4.0/examples/assets/houseplants/square-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)     3725 2022-09-30 10:20:37.434177 PyQt6_3D-6.4.0/examples/assets/houseplants/square-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15842 2022-09-30 10:20:37.434981 PyQt6_3D-6.4.0/examples/assets/houseplants/square-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2220 2022-09-30 10:20:37.435686 PyQt6_3D-6.4.0/examples/assets/houseplants/square-spikes.obj
--rw-r--r--   0 phil       (501) staff       (20)    28687 2022-09-30 10:20:37.436649 PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36082 2022-09-30 10:20:37.437740 PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9328 2022-09-30 10:20:37.438501 PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1808 2022-09-30 10:20:37.439160 PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)     2469 2022-09-30 10:20:37.439883 PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15842 2022-09-30 10:20:37.440734 PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2220 2022-09-30 10:20:37.441500 PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-spikes.obj
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.826832 PyQt6_3D-6.4.0/examples/assets/metalbarrel/
--rw-r--r--   0 phil       (501) staff       (20)   162040 2022-09-30 10:20:37.443558 PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_black.webp
--rw-r--r--   0 phil       (501) staff       (20)   101158 2022-09-30 10:20:37.444905 PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_blue.webp
--rw-r--r--   0 phil       (501) staff       (20)    74498 2022-09-30 10:20:37.446138 PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_green.webp
--rw-r--r--   0 phil       (501) staff       (20)    86874 2022-09-30 10:20:37.447380 PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_red.webp
--rw-r--r--   0 phil       (501) staff       (20)   254934 2022-09-30 10:20:37.449835 PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_rust.webp
--rw-r--r--   0 phil       (501) staff       (20)     6042 2022-09-30 10:20:37.450603 PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_stainless_steel.webp
--rw-r--r--   0 phil       (501) staff       (20)   101134 2022-09-30 10:20:37.452133 PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_yellow.webp
--rw-r--r--   0 phil       (501) staff       (20)    27126 2022-09-30 10:20:37.453179 PyQt6_3D-6.4.0/examples/assets/metalbarrel/metal_barrel.obj
--rw-r--r--   0 phil       (501) staff       (20)    29446 2022-09-30 10:20:37.454137 PyQt6_3D-6.4.0/examples/assets/metalbarrel/normal_hard_bumps.webp
--rw-r--r--   0 phil       (501) staff       (20)    25560 2022-09-30 10:20:37.455059 PyQt6_3D-6.4.0/examples/assets/metalbarrel/normal_middle_bumps.webp
--rw-r--r--   0 phil       (501) staff       (20)    21544 2022-09-30 10:20:37.456059 PyQt6_3D-6.4.0/examples/assets/metalbarrel/normal_no_bumps.webp
--rw-r--r--   0 phil       (501) staff       (20)    23620 2022-09-30 10:20:37.457040 PyQt6_3D-6.4.0/examples/assets/metalbarrel/normal_soft_bumps.webp
--rw-r--r--   0 phil       (501) staff       (20)   420416 2022-09-30 10:20:37.460638 PyQt6_3D-6.4.0/examples/assets/metalbarrel/specular.webp
--rw-r--r--   0 phil       (501) staff       (20)   330298 2022-09-30 10:20:37.463654 PyQt6_3D-6.4.0/examples/assets/metalbarrel/specular_rust.webp
--rw-r--r--   0 phil       (501) staff       (20)   220224 2022-09-30 10:20:37.466079 PyQt6_3D-6.4.0/examples/assets/metalbarrel/specular_stainless_steel.webp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.801658 PyQt6_3D-6.4.0/examples/assets/obj/
--rw-r--r--   0 phil       (501) staff       (20)   346814 2022-09-30 10:20:37.469516 PyQt6_3D-6.4.0/examples/assets/obj/ball.obj
--rw-r--r--   0 phil       (501) staff       (20)  1764501 2022-09-30 10:20:37.484484 PyQt6_3D-6.4.0/examples/assets/obj/toyplane.obj
--rw-r--r--   0 phil       (501) staff       (20)   263373 2022-09-30 10:20:37.487504 PyQt6_3D-6.4.0/examples/assets/obj/trefoil.obj
--rw-r--r--   0 phil       (501) staff       (20)   127711 2022-09-30 10:20:37.489229 PyQt6_3D-6.4.0/examples/assets/test_scene.dae
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.804385 PyQt6_3D-6.4.0/examples/assets/textures/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.806451 PyQt6_3D-6.4.0/examples/assets/textures/pattern_09/
--rw-r--r--   0 phil       (501) staff       (20)   677322 2022-09-30 10:20:37.496810 PyQt6_3D-6.4.0/examples/assets/textures/pattern_09/diffuse.webp
--rw-r--r--   0 phil       (501) staff       (20)   822594 2022-09-30 10:20:37.502625 PyQt6_3D-6.4.0/examples/assets/textures/pattern_09/normal.webp
--rw-r--r--   0 phil       (501) staff       (20)      152 2022-09-30 10:20:37.503345 PyQt6_3D-6.4.0/examples/assets/textures/pattern_09/readme.txt
--rw-r--r--   0 phil       (501) staff       (20)  1005334 2022-09-30 10:20:37.512594 PyQt6_3D-6.4.0/examples/assets/textures/pattern_09/specular.webp
--rw-r--r--   0 phil       (501) staff       (20)    10285 2022-09-30 10:20:37.513475 PyQt6_3D-6.4.0/examples/basicshapes-py.py
--rw-r--r--   0 phil       (501) staff       (20)    18568 2022-09-30 10:20:37.514483 PyQt6_3D-6.4.0/examples/materials-py.py
--rw-r--r--   0 phil       (501) staff       (20)     6082 2022-09-30 10:20:37.515183 PyQt6_3D-6.4.0/examples/simple-py.py
--rw-r--r--   0 phil       (501) staff       (20)     1072 2022-09-30 10:24:53.370020 PyQt6_3D-6.4.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.889849 PyQt6_3D-6.4.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.889460 PyQt6_3D-6.4.0/sip/Qt3DAnimation/
--rw-r--r--   0 phil       (501) staff       (20)     2857 2022-09-30 10:24:54.481191 PyQt6_3D-6.4.0/sip/Qt3DAnimation/Qt3DAnimationmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     4844 2022-09-30 10:24:54.483370 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     1344 2022-09-30 10:24:54.480691 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractanimationclip.sip
--rw-r--r--   0 phil       (501) staff       (20)     1257 2022-09-30 10:24:54.471200 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractchannelmapping.sip
--rw-r--r--   0 phil       (501) staff       (20)     2214 2022-09-30 10:24:54.472186 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractclipanimator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1336 2022-09-30 10:24:54.481703 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractclipblendnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1959 2022-09-30 10:24:54.474061 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qadditiveclipblend.sip
--rw-r--r--   0 phil       (501) staff       (20)     1286 2022-09-30 10:24:54.474944 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationaspect.sip
--rw-r--r--   0 phil       (501) staff       (20)     1538 2022-09-30 10:24:54.478253 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationclip.sip
--rw-r--r--   0 phil       (501) staff       (20)     1631 2022-09-30 10:24:54.476249 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationclipdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     1848 2022-09-30 10:24:54.472677 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationcliploader.sip
--rw-r--r--   0 phil       (501) staff       (20)     2530 2022-09-30 10:24:54.476749 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationcontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     1884 2022-09-30 10:24:54.470791 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationgroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     1605 2022-09-30 10:24:54.471659 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qblendedclipanimator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1724 2022-09-30 10:24:54.479154 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qchannel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1659 2022-09-30 10:24:54.473137 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qchannelcomponent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1497 2022-09-30 10:24:54.475369 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qchannelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1758 2022-09-30 10:24:54.474531 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qchannelmapping.sip
--rw-r--r--   0 phil       (501) staff       (20)     1519 2022-09-30 10:24:54.480279 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qclipanimator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1646 2022-09-30 10:24:54.473590 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qclipblendvalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     1381 2022-09-30 10:24:54.475801 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qclock.sip
--rw-r--r--   0 phil       (501) staff       (20)     2025 2022-09-30 10:24:54.482270 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qkeyframe.sip
--rw-r--r--   0 phil       (501) staff       (20)     2787 2022-09-30 10:24:54.479846 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qkeyframeanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     1900 2022-09-30 10:24:54.470305 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qlerpclipblend.sip
--rw-r--r--   0 phil       (501) staff       (20)     2779 2022-09-30 10:24:54.477267 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qmorphinganimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     1721 2022-09-30 10:24:54.477827 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qmorphtarget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1529 2022-09-30 10:24:54.482695 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qskeletonmapping.sip
--rw-r--r--   0 phil       (501) staff       (20)     2199 2022-09-30 10:24:54.478715 PyQt6_3D-6.4.0/sip/Qt3DAnimation/qvertexblendanimation.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.854595 PyQt6_3D-6.4.0/sip/Qt3DCore/
--rw-r--r--   0 phil       (501) staff       (20)     2729 2022-09-30 10:24:54.370525 PyQt6_3D-6.4.0/sip/Qt3DCore/Qt3DCoremod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1557 2022-09-30 10:24:54.371306 PyQt6_3D-6.4.0/sip/Qt3DCore/qabstractaspect.sip
--rw-r--r--   0 phil       (501) staff       (20)     1262 2022-09-30 10:24:54.358258 PyQt6_3D-6.4.0/sip/Qt3DCore/qabstractfunctor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1311 2022-09-30 10:24:54.371932 PyQt6_3D-6.4.0/sip/Qt3DCore/qabstractskeleton.sip
--rw-r--r--   0 phil       (501) staff       (20)     1459 2022-09-30 10:24:54.356485 PyQt6_3D-6.4.0/sip/Qt3DCore/qarmature.sip
--rw-r--r--   0 phil       (501) staff       (20)     2108 2022-09-30 10:24:54.358884 PyQt6_3D-6.4.0/sip/Qt3DCore/qaspectengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     4235 2022-09-30 10:24:54.372988 PyQt6_3D-6.4.0/sip/Qt3DCore/qattribute.sip
--rw-r--r--   0 phil       (501) staff       (20)     2024 2022-09-30 10:24:54.375550 PyQt6_3D-6.4.0/sip/Qt3DCore/qbackendnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     2124 2022-09-30 10:24:54.374758 PyQt6_3D-6.4.0/sip/Qt3DCore/qboundingvolume.sip
--rw-r--r--   0 phil       (501) staff       (20)     2252 2022-09-30 10:24:54.355300 PyQt6_3D-6.4.0/sip/Qt3DCore/qbuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1604 2022-09-30 10:24:54.359750 PyQt6_3D-6.4.0/sip/Qt3DCore/qcomponent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1481 2022-09-30 10:24:54.357057 PyQt6_3D-6.4.0/sip/Qt3DCore/qcoresettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     1740 2022-09-30 10:24:54.359326 PyQt6_3D-6.4.0/sip/Qt3DCore/qentity.sip
--rw-r--r--   0 phil       (501) staff       (20)     2182 2022-09-30 10:24:54.361069 PyQt6_3D-6.4.0/sip/Qt3DCore/qgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     3346 2022-09-30 10:24:54.355899 PyQt6_3D-6.4.0/sip/Qt3DCore/qgeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     2574 2022-09-30 10:24:54.354721 PyQt6_3D-6.4.0/sip/Qt3DCore/qjoint.sip
--rw-r--r--   0 phil       (501) staff       (20)     4044 2022-09-30 10:24:54.357831 PyQt6_3D-6.4.0/sip/Qt3DCore/qnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1631 2022-09-30 10:24:54.373786 PyQt6_3D-6.4.0/sip/Qt3DCore/qnodeid.sip
--rw-r--r--   0 phil       (501) staff       (20)     3247 2022-09-30 10:24:54.360498 PyQt6_3D-6.4.0/sip/Qt3DCore/qsharedpointer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1429 2022-09-30 10:24:54.361490 PyQt6_3D-6.4.0/sip/Qt3DCore/qskeleton.sip
--rw-r--r--   0 phil       (501) staff       (20)     2040 2022-09-30 10:24:54.376356 PyQt6_3D-6.4.0/sip/Qt3DCore/qskeletonloader.sip
--rw-r--r--   0 phil       (501) staff       (20)     3350 2022-09-30 10:24:54.362028 PyQt6_3D-6.4.0/sip/Qt3DCore/qtransform.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.879170 PyQt6_3D-6.4.0/sip/Qt3DExtras/
--rw-r--r--   0 phil       (501) staff       (20)     3472 2022-09-30 10:24:54.441213 PyQt6_3D-6.4.0/sip/Qt3DExtras/Qt3DExtrasmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2125 2022-09-30 10:24:54.427682 PyQt6_3D-6.4.0/sip/Qt3DExtras/qabstractcameracontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     1709 2022-09-30 10:24:54.430191 PyQt6_3D-6.4.0/sip/Qt3DExtras/qabstractspritesheet.sip
--rw-r--r--   0 phil       (501) staff       (20)     2448 2022-09-30 10:24:54.421737 PyQt6_3D-6.4.0/sip/Qt3DExtras/qconegeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     2192 2022-09-30 10:24:54.441726 PyQt6_3D-6.4.0/sip/Qt3DExtras/qconegeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     2150 2022-09-30 10:24:54.420259 PyQt6_3D-6.4.0/sip/Qt3DExtras/qconemesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     2498 2022-09-30 10:24:54.425483 PyQt6_3D-6.4.0/sip/Qt3DExtras/qcuboidgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     2186 2022-09-30 10:24:54.428699 PyQt6_3D-6.4.0/sip/Qt3DExtras/qcuboidgeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     2144 2022-09-30 10:24:54.442229 PyQt6_3D-6.4.0/sip/Qt3DExtras/qcuboidmesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     2028 2022-09-30 10:24:54.423656 PyQt6_3D-6.4.0/sip/Qt3DExtras/qcylindergeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1772 2022-09-30 10:24:54.426616 PyQt6_3D-6.4.0/sip/Qt3DExtras/qcylindergeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1730 2022-09-30 10:24:54.469737 PyQt6_3D-6.4.0/sip/Qt3DExtras/qcylindermesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     2070 2022-09-30 10:24:54.392524 PyQt6_3D-6.4.0/sip/Qt3DExtras/qdiffusemapmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2191 2022-09-30 10:24:54.437629 PyQt6_3D-6.4.0/sip/Qt3DExtras/qdiffusespecularmapmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2329 2022-09-30 10:24:54.393125 PyQt6_3D-6.4.0/sip/Qt3DExtras/qdiffusespecularmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1880 2022-09-30 10:24:54.440114 PyQt6_3D-6.4.0/sip/Qt3DExtras/qextrudedtextgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1670 2022-09-30 10:24:54.438577 PyQt6_3D-6.4.0/sip/Qt3DExtras/qextrudedtextmesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     1372 2022-09-30 10:24:54.436634 PyQt6_3D-6.4.0/sip/Qt3DExtras/qfirstpersoncameracontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     2847 2022-09-30 10:24:54.393720 PyQt6_3D-6.4.0/sip/Qt3DExtras/qforwardrenderer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2138 2022-09-30 10:24:54.427173 PyQt6_3D-6.4.0/sip/Qt3DExtras/qgoochmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2235 2022-09-30 10:24:54.434384 PyQt6_3D-6.4.0/sip/Qt3DExtras/qmetalroughmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2001 2022-09-30 10:24:54.432673 PyQt6_3D-6.4.0/sip/Qt3DExtras/qmorphphongmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1384 2022-09-30 10:24:54.422281 PyQt6_3D-6.4.0/sip/Qt3DExtras/qnormaldiffusemapalphamaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2306 2022-09-30 10:24:54.422979 PyQt6_3D-6.4.0/sip/Qt3DExtras/qnormaldiffusemapmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2425 2022-09-30 10:24:54.433270 PyQt6_3D-6.4.0/sip/Qt3DExtras/qnormaldiffusespecularmapmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1468 2022-09-30 10:24:54.438077 PyQt6_3D-6.4.0/sip/Qt3DExtras/qorbitcameracontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     1326 2022-09-30 10:24:54.424248 PyQt6_3D-6.4.0/sip/Qt3DExtras/qpervertexcolormaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     3390 2022-09-30 10:24:54.420926 PyQt6_3D-6.4.0/sip/Qt3DExtras/qphongalphamaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1831 2022-09-30 10:24:54.431641 PyQt6_3D-6.4.0/sip/Qt3DExtras/qphongmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2119 2022-09-30 10:24:54.436213 PyQt6_3D-6.4.0/sip/Qt3DExtras/qplanegeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1823 2022-09-30 10:24:54.437121 PyQt6_3D-6.4.0/sip/Qt3DExtras/qplanegeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1827 2022-09-30 10:24:54.424812 PyQt6_3D-6.4.0/sip/Qt3DExtras/qplanemesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     1813 2022-09-30 10:24:54.439112 PyQt6_3D-6.4.0/sip/Qt3DExtras/qskyboxentity.sip
--rw-r--r--   0 phil       (501) staff       (20)     2106 2022-09-30 10:24:54.440624 PyQt6_3D-6.4.0/sip/Qt3DExtras/qspheregeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1794 2022-09-30 10:24:54.426082 PyQt6_3D-6.4.0/sip/Qt3DExtras/qspheregeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1752 2022-09-30 10:24:54.429659 PyQt6_3D-6.4.0/sip/Qt3DExtras/qspheremesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     1501 2022-09-30 10:24:54.432105 PyQt6_3D-6.4.0/sip/Qt3DExtras/qspritegrid.sip
--rw-r--r--   0 phil       (501) staff       (20)     1739 2022-09-30 10:24:54.430698 PyQt6_3D-6.4.0/sip/Qt3DExtras/qspritesheet.sip
--rw-r--r--   0 phil       (501) staff       (20)     1635 2022-09-30 10:24:54.431164 PyQt6_3D-6.4.0/sip/Qt3DExtras/qspritesheetitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     7090 2022-09-30 10:24:54.435240 PyQt6_3D-6.4.0/sip/Qt3DExtras/qt3dwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     1847 2022-09-30 10:24:54.439622 PyQt6_3D-6.4.0/sip/Qt3DExtras/qtext2dentity.sip
--rw-r--r--   0 phil       (501) staff       (20)     2009 2022-09-30 10:24:54.429178 PyQt6_3D-6.4.0/sip/Qt3DExtras/qtexturematerial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2035 2022-09-30 10:24:54.428196 PyQt6_3D-6.4.0/sip/Qt3DExtras/qtorusgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1779 2022-09-30 10:24:54.433835 PyQt6_3D-6.4.0/sip/Qt3DExtras/qtorusgeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1737 2022-09-30 10:24:54.435715 PyQt6_3D-6.4.0/sip/Qt3DExtras/qtorusmesh.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.862100 PyQt6_3D-6.4.0/sip/Qt3DInput/
--rw-r--r--   0 phil       (501) staff       (20)     2590 2022-09-30 10:24:54.378608 PyQt6_3D-6.4.0/sip/Qt3DInput/Qt3DInputmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1234 2022-09-30 10:24:54.384980 PyQt6_3D-6.4.0/sip/Qt3DInput/qabstractactioninput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1506 2022-09-30 10:24:54.390406 PyQt6_3D-6.4.0/sip/Qt3DInput/qabstractaxisinput.sip
--rw-r--r--   0 phil       (501) staff       (20)     4384 2022-09-30 10:24:54.380910 PyQt6_3D-6.4.0/sip/Qt3DInput/qabstractphysicaldevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1742 2022-09-30 10:24:54.381765 PyQt6_3D-6.4.0/sip/Qt3DInput/qaction.sip
--rw-r--r--   0 phil       (501) staff       (20)     1694 2022-09-30 10:24:54.386404 PyQt6_3D-6.4.0/sip/Qt3DInput/qactioninput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1417 2022-09-30 10:24:54.383100 PyQt6_3D-6.4.0/sip/Qt3DInput/qanalogaxisinput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1719 2022-09-30 10:24:54.379262 PyQt6_3D-6.4.0/sip/Qt3DInput/qaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2101 2022-09-30 10:24:54.382543 PyQt6_3D-6.4.0/sip/Qt3DInput/qaxisaccumulator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1688 2022-09-30 10:24:54.376933 PyQt6_3D-6.4.0/sip/Qt3DInput/qaxissetting.sip
--rw-r--r--   0 phil       (501) staff       (20)     1852 2022-09-30 10:24:54.389249 PyQt6_3D-6.4.0/sip/Qt3DInput/qbuttonaxisinput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1405 2022-09-30 10:24:54.378000 PyQt6_3D-6.4.0/sip/Qt3DInput/qinputaspect.sip
--rw-r--r--   0 phil       (501) staff       (20)     1836 2022-09-30 10:24:54.387632 PyQt6_3D-6.4.0/sip/Qt3DInput/qinputchord.sip
--rw-r--r--   0 phil       (501) staff       (20)     2010 2022-09-30 10:24:54.387044 PyQt6_3D-6.4.0/sip/Qt3DInput/qinputsequence.sip
--rw-r--r--   0 phil       (501) staff       (20)     1435 2022-09-30 10:24:54.383614 PyQt6_3D-6.4.0/sip/Qt3DInput/qinputsettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     1795 2022-09-30 10:24:54.388726 PyQt6_3D-6.4.0/sip/Qt3DInput/qkeyboarddevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3906 2022-09-30 10:24:54.384417 PyQt6_3D-6.4.0/sip/Qt3DInput/qkeyboardhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1715 2022-09-30 10:24:54.377519 PyQt6_3D-6.4.0/sip/Qt3DInput/qkeyevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2048 2022-09-30 10:24:54.388288 PyQt6_3D-6.4.0/sip/Qt3DInput/qlogicaldevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2065 2022-09-30 10:24:54.379956 PyQt6_3D-6.4.0/sip/Qt3DInput/qmousedevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2756 2022-09-30 10:24:54.389921 PyQt6_3D-6.4.0/sip/Qt3DInput/qmouseevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2037 2022-09-30 10:24:54.385838 PyQt6_3D-6.4.0/sip/Qt3DInput/qmousehandler.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.863167 PyQt6_3D-6.4.0/sip/Qt3DLogic/
--rw-r--r--   0 phil       (501) staff       (20)     2006 2022-09-30 10:24:54.390911 PyQt6_3D-6.4.0/sip/Qt3DLogic/Qt3DLogicmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2049 2022-09-30 10:24:54.391559 PyQt6_3D-6.4.0/sip/Qt3DLogic/qframeaction.sip
--rw-r--r--   0 phil       (501) staff       (20)     1254 2022-09-30 10:24:54.391946 PyQt6_3D-6.4.0/sip/Qt3DLogic/qlogicaspect.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:24:54.924299 PyQt6_3D-6.4.0/sip/Qt3DRender/
--rw-r--r--   0 phil       (501) staff       (20)     4863 2022-09-30 10:24:54.591621 PyQt6_3D-6.4.0/sip/Qt3DRender/Qt3DRendermod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1664 2022-09-30 10:24:54.539580 PyQt6_3D-6.4.0/sip/Qt3DRender/qabstractlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     2656 2022-09-30 10:24:54.585057 PyQt6_3D-6.4.0/sip/Qt3DRender/qabstractraycaster.sip
--rw-r--r--   0 phil       (501) staff       (20)     8855 2022-09-30 10:24:54.538619 PyQt6_3D-6.4.0/sip/Qt3DRender/qabstracttexture.sip
--rw-r--r--   0 phil       (501) staff       (20)     1933 2022-09-30 10:24:54.570236 PyQt6_3D-6.4.0/sip/Qt3DRender/qabstracttextureimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     1275 2022-09-30 10:24:54.541553 PyQt6_3D-6.4.0/sip/Qt3DRender/qalphacoverage.sip
--rw-r--r--   0 phil       (501) staff       (20)     1915 2022-09-30 10:24:54.588310 PyQt6_3D-6.4.0/sip/Qt3DRender/qalphatest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1731 2022-09-30 10:24:54.529881 PyQt6_3D-6.4.0/sip/Qt3DRender/qblendequation.sip
--rw-r--r--   0 phil       (501) staff       (20)     3658 2022-09-30 10:24:54.533169 PyQt6_3D-6.4.0/sip/Qt3DRender/qblendequationarguments.sip
--rw-r--r--   0 phil       (501) staff       (20)     2712 2022-09-30 10:24:54.585627 PyQt6_3D-6.4.0/sip/Qt3DRender/qblitframebuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)    15325 2022-09-30 10:24:54.523499 PyQt6_3D-6.4.0/sip/Qt3DRender/qcamera.sip
--rw-r--r--   0 phil       (501) staff       (20)     3588 2022-09-30 10:24:54.590792 PyQt6_3D-6.4.0/sip/Qt3DRender/qcameralens.sip
--rw-r--r--   0 phil       (501) staff       (20)     1466 2022-09-30 10:24:54.526693 PyQt6_3D-6.4.0/sip/Qt3DRender/qcameraselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     2555 2022-09-30 10:24:54.525830 PyQt6_3D-6.4.0/sip/Qt3DRender/qclearbuffers.sip
--rw-r--r--   0 phil       (501) staff       (20)     1623 2022-09-30 10:24:54.534830 PyQt6_3D-6.4.0/sip/Qt3DRender/qclipplane.sip
--rw-r--r--   0 phil       (501) staff       (20)     1805 2022-09-30 10:24:54.584425 PyQt6_3D-6.4.0/sip/Qt3DRender/qcolormask.sip
--rw-r--r--   0 phil       (501) staff       (20)     2069 2022-09-30 10:24:54.487662 PyQt6_3D-6.4.0/sip/Qt3DRender/qcomputecommand.sip
--rw-r--r--   0 phil       (501) staff       (20)     1617 2022-09-30 10:24:54.542552 PyQt6_3D-6.4.0/sip/Qt3DRender/qcullface.sip
--rw-r--r--   0 phil       (501) staff       (20)     1534 2022-09-30 10:24:54.583880 PyQt6_3D-6.4.0/sip/Qt3DRender/qdepthrange.sip
--rw-r--r--   0 phil       (501) staff       (20)     1765 2022-09-30 10:24:54.580706 PyQt6_3D-6.4.0/sip/Qt3DRender/qdepthtest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1504 2022-09-30 10:24:54.542100 PyQt6_3D-6.4.0/sip/Qt3DRender/qdirectionallight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1653 2022-09-30 10:24:54.572123 PyQt6_3D-6.4.0/sip/Qt3DRender/qdispatchcompute.sip
--rw-r--r--   0 phil       (501) staff       (20)     1251 2022-09-30 10:24:54.541164 PyQt6_3D-6.4.0/sip/Qt3DRender/qdithering.sip
--rw-r--r--   0 phil       (501) staff       (20)     2066 2022-09-30 10:24:54.593168 PyQt6_3D-6.4.0/sip/Qt3DRender/qeffect.sip
--rw-r--r--   0 phil       (501) staff       (20)     1770 2022-09-30 10:24:54.542997 PyQt6_3D-6.4.0/sip/Qt3DRender/qenvironmentlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1529 2022-09-30 10:24:54.528768 PyQt6_3D-6.4.0/sip/Qt3DRender/qfilterkey.sip
--rw-r--r--   0 phil       (501) staff       (20)     1339 2022-09-30 10:24:54.592048 PyQt6_3D-6.4.0/sip/Qt3DRender/qframegraphnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1638 2022-09-30 10:24:54.589669 PyQt6_3D-6.4.0/sip/Qt3DRender/qfrontface.sip
--rw-r--r--   0 phil       (501) staff       (20)     1284 2022-09-30 10:24:54.579083 PyQt6_3D-6.4.0/sip/Qt3DRender/qfrustumculling.sip
--rw-r--r--   0 phil       (501) staff       (20)     3665 2022-09-30 10:24:54.540764 PyQt6_3D-6.4.0/sip/Qt3DRender/qgeometryrenderer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2598 2022-09-30 10:24:54.487149 PyQt6_3D-6.4.0/sip/Qt3DRender/qgraphicsapifilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     1345 2022-09-30 10:24:54.522137 PyQt6_3D-6.4.0/sip/Qt3DRender/qlayer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2112 2022-09-30 10:24:54.571379 PyQt6_3D-6.4.0/sip/Qt3DRender/qlayerfilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2582 2022-09-30 10:24:54.524072 PyQt6_3D-6.4.0/sip/Qt3DRender/qlevelofdetail.sip
--rw-r--r--   0 phil       (501) staff       (20)     1682 2022-09-30 10:24:54.578098 PyQt6_3D-6.4.0/sip/Qt3DRender/qlevelofdetailboundingsphere.sip
--rw-r--r--   0 phil       (501) staff       (20)     1313 2022-09-30 10:24:54.583423 PyQt6_3D-6.4.0/sip/Qt3DRender/qlevelofdetailswitch.sip
--rw-r--r--   0 phil       (501) staff       (20)     1498 2022-09-30 10:24:54.492811 PyQt6_3D-6.4.0/sip/Qt3DRender/qlinewidth.sip
--rw-r--r--   0 phil       (501) staff       (20)     7581 2022-09-30 10:24:54.587796 PyQt6_3D-6.4.0/sip/Qt3DRender/qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1635 2022-09-30 10:24:54.576184 PyQt6_3D-6.4.0/sip/Qt3DRender/qmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2100 2022-09-30 10:24:54.592579 PyQt6_3D-6.4.0/sip/Qt3DRender/qmemorybarrier.sip
--rw-r--r--   0 phil       (501) staff       (20)     1797 2022-09-30 10:24:54.530391 PyQt6_3D-6.4.0/sip/Qt3DRender/qmesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     1335 2022-09-30 10:24:54.535778 PyQt6_3D-6.4.0/sip/Qt3DRender/qmultisampleantialiasing.sip
--rw-r--r--   0 phil       (501) staff       (20)     1263 2022-09-30 10:24:54.573897 PyQt6_3D-6.4.0/sip/Qt3DRender/qnodepthmask.sip
--rw-r--r--   0 phil       (501) staff       (20)     1236 2022-09-30 10:24:54.588729 PyQt6_3D-6.4.0/sip/Qt3DRender/qnodraw.sip
--rw-r--r--   0 phil       (501) staff       (20)     1254 2022-09-30 10:24:54.578570 PyQt6_3D-6.4.0/sip/Qt3DRender/qnopicking.sip
--rw-r--r--   0 phil       (501) staff       (20)     2105 2022-09-30 10:24:54.521694 PyQt6_3D-6.4.0/sip/Qt3DRender/qobjectpicker.sip
--rw-r--r--   0 phil       (501) staff       (20)     1850 2022-09-30 10:24:54.520556 PyQt6_3D-6.4.0/sip/Qt3DRender/qpaintedtextureimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     1752 2022-09-30 10:24:54.489859 PyQt6_3D-6.4.0/sip/Qt3DRender/qparameter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2414 2022-09-30 10:24:54.581344 PyQt6_3D-6.4.0/sip/Qt3DRender/qpickevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1270 2022-09-30 10:24:54.488048 PyQt6_3D-6.4.0/sip/Qt3DRender/qpickingproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     2955 2022-09-30 10:24:54.486475 PyQt6_3D-6.4.0/sip/Qt3DRender/qpickingsettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     1583 2022-09-30 10:24:54.526267 PyQt6_3D-6.4.0/sip/Qt3DRender/qpicklineevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1484 2022-09-30 10:24:54.527800 PyQt6_3D-6.4.0/sip/Qt3DRender/qpickpointevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1944 2022-09-30 10:24:54.579570 PyQt6_3D-6.4.0/sip/Qt3DRender/qpicktriangleevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1771 2022-09-30 10:24:54.581837 PyQt6_3D-6.4.0/sip/Qt3DRender/qpointlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1698 2022-09-30 10:24:54.532551 PyQt6_3D-6.4.0/sip/Qt3DRender/qpointsize.sip
--rw-r--r--   0 phil       (501) staff       (20)     1573 2022-09-30 10:24:54.533623 PyQt6_3D-6.4.0/sip/Qt3DRender/qpolygonoffset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1637 2022-09-30 10:24:54.536243 PyQt6_3D-6.4.0/sip/Qt3DRender/qproximityfilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     1924 2022-09-30 10:24:54.580160 PyQt6_3D-6.4.0/sip/Qt3DRender/qrastermode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1800 2022-09-30 10:24:54.577590 PyQt6_3D-6.4.0/sip/Qt3DRender/qraycaster.sip
--rw-r--r--   0 phil       (501) staff       (20)     2004 2022-09-30 10:24:54.488516 PyQt6_3D-6.4.0/sip/Qt3DRender/qraycasterhit.sip
--rw-r--r--   0 phil       (501) staff       (20)     1151 2022-09-30 10:24:54.536726 PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderapi.sip
--rw-r--r--   0 phil       (501) staff       (20)     1555 2022-09-30 10:24:54.491279 PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderaspect.sip
--rw-r--r--   0 phil       (501) staff       (20)     2740 2022-09-30 10:24:54.534213 PyQt6_3D-6.4.0/sip/Qt3DRender/qrendercapabilities.sip
--rw-r--r--   0 phil       (501) staff       (20)     1846 2022-09-30 10:24:54.586151 PyQt6_3D-6.4.0/sip/Qt3DRender/qrendercapture.sip
--rw-r--r--   0 phil       (501) staff       (20)     2788 2022-09-30 10:24:54.570861 PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderpass.sip
--rw-r--r--   0 phil       (501) staff       (20)     2140 2022-09-30 10:24:54.525267 PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderpassfilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2036 2022-09-30 10:24:54.574454 PyQt6_3D-6.4.0/sip/Qt3DRender/qrendersettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     1196 2022-09-30 10:24:54.576676 PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderstate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1719 2022-09-30 10:24:54.590127 PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderstateset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1804 2022-09-30 10:24:54.528292 PyQt6_3D-6.4.0/sip/Qt3DRender/qrendersurfaceselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     1703 2022-09-30 10:24:54.589201 PyQt6_3D-6.4.0/sip/Qt3DRender/qrendertarget.sip
--rw-r--r--   0 phil       (501) staff       (20)     2734 2022-09-30 10:24:54.582495 PyQt6_3D-6.4.0/sip/Qt3DRender/qrendertargetoutput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1545 2022-09-30 10:24:54.519887 PyQt6_3D-6.4.0/sip/Qt3DRender/qrendertargetselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     2168 2022-09-30 10:24:54.537247 PyQt6_3D-6.4.0/sip/Qt3DRender/qsceneloader.sip
--rw-r--r--   0 phil       (501) staff       (20)     1697 2022-09-30 10:24:54.483979 PyQt6_3D-6.4.0/sip/Qt3DRender/qscissortest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1533 2022-09-30 10:24:54.529196 PyQt6_3D-6.4.0/sip/Qt3DRender/qscreenraycaster.sip
--rw-r--r--   0 phil       (501) staff       (20)     1287 2022-09-30 10:24:54.535317 PyQt6_3D-6.4.0/sip/Qt3DRender/qseamlesscubemap.sip
--rw-r--r--   0 phil       (501) staff       (20)     1575 2022-09-30 10:24:54.539070 PyQt6_3D-6.4.0/sip/Qt3DRender/qsetfence.sip
--rw-r--r--   0 phil       (501) staff       (20)     1690 2022-09-30 10:24:54.489005 PyQt6_3D-6.4.0/sip/Qt3DRender/qshaderdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     3207 2022-09-30 10:24:54.485359 PyQt6_3D-6.4.0/sip/Qt3DRender/qshaderimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     3718 2022-09-30 10:24:54.524755 PyQt6_3D-6.4.0/sip/Qt3DRender/qshaderprogram.sip
--rw-r--r--   0 phil       (501) staff       (20)     3778 2022-09-30 10:24:54.484672 PyQt6_3D-6.4.0/sip/Qt3DRender/qshaderprogrambuilder.sip
--rw-r--r--   0 phil       (501) staff       (20)     1904 2022-09-30 10:24:54.572716 PyQt6_3D-6.4.0/sip/Qt3DRender/qsortpolicy.sip
--rw-r--r--   0 phil       (501) staff       (20)     2076 2022-09-30 10:24:54.490820 PyQt6_3D-6.4.0/sip/Qt3DRender/qspotlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1595 2022-09-30 10:24:54.583001 PyQt6_3D-6.4.0/sip/Qt3DRender/qstencilmask.sip
--rw-r--r--   0 phil       (501) staff       (20)     1418 2022-09-30 10:24:54.491680 PyQt6_3D-6.4.0/sip/Qt3DRender/qstenciloperation.sip
--rw-r--r--   0 phil       (501) staff       (20)     2778 2022-09-30 10:24:54.521170 PyQt6_3D-6.4.0/sip/Qt3DRender/qstenciloperationarguments.sip
--rw-r--r--   0 phil       (501) staff       (20)     1378 2022-09-30 10:24:54.577107 PyQt6_3D-6.4.0/sip/Qt3DRender/qstenciltest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2409 2022-09-30 10:24:54.574998 PyQt6_3D-6.4.0/sip/Qt3DRender/qstenciltestarguments.sip
--rw-r--r--   0 phil       (501) staff       (20)     1655 2022-09-30 10:24:54.492354 PyQt6_3D-6.4.0/sip/Qt3DRender/qsubtreeenabler.sip
--rw-r--r--   0 phil       (501) staff       (20)     2572 2022-09-30 10:24:54.573380 PyQt6_3D-6.4.0/sip/Qt3DRender/qtechnique.sip
--rw-r--r--   0 phil       (501) staff       (20)     2118 2022-09-30 10:24:54.531433 PyQt6_3D-6.4.0/sip/Qt3DRender/qtechniquefilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     4644 2022-09-30 10:24:54.543969 PyQt6_3D-6.4.0/sip/Qt3DRender/qtexture.sip
--rw-r--r--   0 phil       (501) staff       (20)     3172 2022-09-30 10:24:54.530945 PyQt6_3D-6.4.0/sip/Qt3DRender/qtexturedata.sip
--rw-r--r--   0 phil       (501) staff       (20)     2108 2022-09-30 10:24:54.490317 PyQt6_3D-6.4.0/sip/Qt3DRender/qtexturedataupdate.sip
--rw-r--r--   0 phil       (501) staff       (20)     2041 2022-09-30 10:24:54.485880 PyQt6_3D-6.4.0/sip/Qt3DRender/qtextureimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     2474 2022-09-30 10:24:54.540092 PyQt6_3D-6.4.0/sip/Qt3DRender/qtextureimagedata.sip
--rw-r--r--   0 phil       (501) staff       (20)     1539 2022-09-30 10:24:54.489422 PyQt6_3D-6.4.0/sip/Qt3DRender/qtextureimagedatagenerator.sip
--rw-r--r--   0 phil       (501) staff       (20)     2330 2022-09-30 10:24:54.531926 PyQt6_3D-6.4.0/sip/Qt3DRender/qtexturewrapmode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1599 2022-09-30 10:24:54.575594 PyQt6_3D-6.4.0/sip/Qt3DRender/qviewport.sip
--rw-r--r--   0 phil       (501) staff       (20)     1943 2022-09-30 10:24:54.527236 PyQt6_3D-6.4.0/sip/Qt3DRender/qwaitfence.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.392443 PyQt6_3D-6.5.0/
+-rw-r--r--   0 phil       (501) staff       (20)     9973 2023-04-04 15:19:40.738745 PyQt6_3D-6.5.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2023-04-04 15:19:40.556064 PyQt6_3D-6.5.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      633 2023-04-04 15:15:05.481365 PyQt6_3D-6.5.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1578 2023-04-04 15:19:42.392567 PyQt6_3D-6.5.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1265 2023-04-04 15:19:40.739693 PyQt6_3D-6.5.0/README
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.265746 PyQt6_3D-6.5.0/examples/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.292551 PyQt6_3D-6.5.0/examples/assets/
+-rw-r--r--   0 phil       (501) staff       (20)      136 2023-04-04 15:15:05.493864 PyQt6_3D-6.5.0/examples/assets/LICENSE
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.292055 PyQt6_3D-6.5.0/examples/assets/chest/
+-rw-r--r--   0 phil       (501) staff       (20)    46344 2023-04-04 15:15:05.495251 PyQt6_3D-6.5.0/examples/assets/chest/Chest.obj
+-rw-r--r--   0 phil       (501) staff       (20)    70980 2023-04-04 15:15:05.496746 PyQt6_3D-6.5.0/examples/assets/chest/diffuse.webp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.276079 PyQt6_3D-6.5.0/examples/assets/cubemaps/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.275633 PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/
+-rw-r--r--   0 phil       (501) staff       (20)      293 2023-04-04 15:15:05.497546 PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/README.TXT
+-rw-r--r--   0 phil       (501) staff       (20)   121754 2023-04-04 15:15:05.499269 PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_negx.webp
+-rw-r--r--   0 phil       (501) staff       (20)     1926 2023-04-04 15:15:05.499854 PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_negy.webp
+-rw-r--r--   0 phil       (501) staff       (20)   147696 2023-04-04 15:15:05.502407 PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_negz.webp
+-rw-r--r--   0 phil       (501) staff       (20)   136426 2023-04-04 15:15:05.504474 PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_posx.webp
+-rw-r--r--   0 phil       (501) staff       (20)    57622 2023-04-04 15:15:05.505512 PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_posy.webp
+-rw-r--r--   0 phil       (501) staff       (20)   164564 2023-04-04 15:15:05.507721 PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_posz.webp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.278217 PyQt6_3D-6.5.0/examples/assets/cubemaps/night/
+-rw-r--r--   0 phil       (501) staff       (20)    38042 2023-04-04 15:15:05.508896 PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_negx.webp
+-rw-r--r--   0 phil       (501) staff       (20)    42278 2023-04-04 15:15:05.509796 PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_negy.webp
+-rw-r--r--   0 phil       (501) staff       (20)    36790 2023-04-04 15:15:05.510640 PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_negz.webp
+-rw-r--r--   0 phil       (501) staff       (20)    37092 2023-04-04 15:15:05.511641 PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_posx.webp
+-rw-r--r--   0 phil       (501) staff       (20)    26008 2023-04-04 15:15:05.512303 PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_posy.webp
+-rw-r--r--   0 phil       (501) staff       (20)    37802 2023-04-04 15:15:05.513363 PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_posz.webp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.279059 PyQt6_3D-6.5.0/examples/assets/gltf/
+-rw-r--r--   0 phil       (501) staff       (20)     1831 2023-04-04 15:15:05.514218 PyQt6_3D-6.5.0/examples/assets/gltf/LICENSE.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.284805 PyQt6_3D-6.5.0/examples/assets/gltf/wine/
+-rw-r--r--   0 phil       (501) staff       (20)     8798 2023-04-04 15:15:05.515466 PyQt6_3D-6.5.0/examples/assets/gltf/wine/Wood_Cherry_Original_.jpg
+-rw-r--r--   0 phil       (501) staff       (20)    46051 2023-04-04 15:15:05.517055 PyQt6_3D-6.5.0/examples/assets/gltf/wine/_2004_old_vine_zinfandel_btl_xlg.jpg
+-rw-r--r--   0 phil       (501) staff       (20)    35585 2023-04-04 15:15:05.518112 PyQt6_3D-6.5.0/examples/assets/gltf/wine/artezin_bottle.jpg
+-rw-r--r--   0 phil       (501) staff       (20)   329088 2023-04-04 15:15:05.521639 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine.bin
+-rw-r--r--   0 phil       (501) staff       (20)   797366 2023-04-04 15:15:05.528195 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine.dae
+-rw-r--r--   0 phil       (501) staff       (20)   275432 2023-04-04 15:15:05.530702 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine.gltf
+-rw-r--r--   0 phil       (501) staff       (20)      497 2023-04-04 15:15:05.531603 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine0FS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      439 2023-04-04 15:15:05.532376 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine0VS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      489 2023-04-04 15:15:05.532903 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine1FS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      355 2023-04-04 15:15:05.533430 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine1VS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      219 2023-04-04 15:15:05.533998 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine2FS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      236 2023-04-04 15:15:05.534930 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine2VS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      441 2023-04-04 15:15:05.535489 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine3FS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      355 2023-04-04 15:15:05.536595 PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine3VS.glsl
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.312691 PyQt6_3D-6.5.0/examples/assets/houseplants/
+-rw-r--r--   0 phil       (501) staff       (20)    13846 2023-04-04 15:15:05.537980 PyQt6_3D-6.5.0/examples/assets/houseplants/bamboo.webp
+-rw-r--r--   0 phil       (501) staff       (20)    16614 2023-04-04 15:15:05.538838 PyQt6_3D-6.5.0/examples/assets/houseplants/bamboo_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    89192 2023-04-04 15:15:05.540557 PyQt6_3D-6.5.0/examples/assets/houseplants/cover.webp
+-rw-r--r--   0 phil       (501) staff       (20)    21098 2023-04-04 15:15:05.541519 PyQt6_3D-6.5.0/examples/assets/houseplants/cover_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    44264 2023-04-04 15:15:05.542816 PyQt6_3D-6.5.0/examples/assets/houseplants/cross-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36076 2023-04-04 15:15:05.545454 PyQt6_3D-6.5.0/examples/assets/houseplants/cross-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9324 2023-04-04 15:15:05.546195 PyQt6_3D-6.5.0/examples/assets/houseplants/cross-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1822 2023-04-04 15:15:05.547184 PyQt6_3D-6.5.0/examples/assets/houseplants/cross-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)     8863 2023-04-04 15:15:05.547931 PyQt6_3D-6.5.0/examples/assets/houseplants/cross-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15838 2023-04-04 15:15:05.549218 PyQt6_3D-6.5.0/examples/assets/houseplants/cross-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2216 2023-04-04 15:15:05.550443 PyQt6_3D-6.5.0/examples/assets/houseplants/cross-spikes.obj
+-rw-r--r--   0 phil       (501) staff       (20)    51505 2023-04-04 15:15:05.552155 PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36078 2023-04-04 15:15:05.553521 PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9328 2023-04-04 15:15:05.554405 PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1820 2023-04-04 15:15:05.555366 PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9026 2023-04-04 15:15:05.556118 PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15842 2023-04-04 15:15:05.557254 PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2216 2023-04-04 15:15:05.558035 PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-spikes.obj
+-rw-r--r--   0 phil       (501) staff       (20)    33756 2023-04-04 15:15:05.558799 PyQt6_3D-6.5.0/examples/assets/houseplants/palm.webp
+-rw-r--r--   0 phil       (501) staff       (20)    36186 2023-04-04 15:15:05.559562 PyQt6_3D-6.5.0/examples/assets/houseplants/palm_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)   120426 2023-04-04 15:15:05.561608 PyQt6_3D-6.5.0/examples/assets/houseplants/pine.webp
+-rw-r--r--   0 phil       (501) staff       (20)    47352 2023-04-04 15:15:05.562612 PyQt6_3D-6.5.0/examples/assets/houseplants/pine_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)   366144 2023-04-04 15:15:05.566470 PyQt6_3D-6.5.0/examples/assets/houseplants/pot.webp
+-rw-r--r--   0 phil       (501) staff       (20)    50950 2023-04-04 15:15:05.567625 PyQt6_3D-6.5.0/examples/assets/houseplants/pot_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    33100 2023-04-04 15:15:05.568484 PyQt6_3D-6.5.0/examples/assets/houseplants/shrub.webp
+-rw-r--r--   0 phil       (501) staff       (20)    10180 2023-04-04 15:15:05.569429 PyQt6_3D-6.5.0/examples/assets/houseplants/shrub_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    51509 2023-04-04 15:15:05.571610 PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36082 2023-04-04 15:15:05.572714 PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9328 2023-04-04 15:15:05.573430 PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1820 2023-04-04 15:15:05.574118 PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)    46455 2023-04-04 15:15:05.575312 PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15842 2023-04-04 15:15:05.576074 PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2220 2023-04-04 15:15:05.576863 PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-spikes.obj
+-rw-r--r--   0 phil       (501) staff       (20)    30338 2023-04-04 15:15:05.577490 PyQt6_3D-6.5.0/examples/assets/houseplants/spikes.webp
+-rw-r--r--   0 phil       (501) staff       (20)    12028 2023-04-04 15:15:05.578181 PyQt6_3D-6.5.0/examples/assets/houseplants/spikes_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    51509 2023-04-04 15:15:05.579233 PyQt6_3D-6.5.0/examples/assets/houseplants/square-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36082 2023-04-04 15:15:05.580293 PyQt6_3D-6.5.0/examples/assets/houseplants/square-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9328 2023-04-04 15:15:05.580934 PyQt6_3D-6.5.0/examples/assets/houseplants/square-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1824 2023-04-04 15:15:05.581543 PyQt6_3D-6.5.0/examples/assets/houseplants/square-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)     3725 2023-04-04 15:15:05.582240 PyQt6_3D-6.5.0/examples/assets/houseplants/square-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15842 2023-04-04 15:15:05.582964 PyQt6_3D-6.5.0/examples/assets/houseplants/square-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2220 2023-04-04 15:15:05.583432 PyQt6_3D-6.5.0/examples/assets/houseplants/square-spikes.obj
+-rw-r--r--   0 phil       (501) staff       (20)    28687 2023-04-04 15:15:05.584304 PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36082 2023-04-04 15:15:05.585213 PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9328 2023-04-04 15:15:05.585743 PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1808 2023-04-04 15:15:05.586215 PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2469 2023-04-04 15:15:05.586654 PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15842 2023-04-04 15:15:05.587386 PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2220 2023-04-04 15:15:05.588016 PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-spikes.obj
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.291189 PyQt6_3D-6.5.0/examples/assets/metalbarrel/
+-rw-r--r--   0 phil       (501) staff       (20)   162040 2023-04-04 15:15:05.596057 PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_black.webp
+-rw-r--r--   0 phil       (501) staff       (20)   101158 2023-04-04 15:15:05.597358 PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_blue.webp
+-rw-r--r--   0 phil       (501) staff       (20)    74498 2023-04-04 15:15:05.598759 PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_green.webp
+-rw-r--r--   0 phil       (501) staff       (20)    86874 2023-04-04 15:15:05.600446 PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_red.webp
+-rw-r--r--   0 phil       (501) staff       (20)   254934 2023-04-04 15:15:05.604051 PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_rust.webp
+-rw-r--r--   0 phil       (501) staff       (20)     6042 2023-04-04 15:15:05.604945 PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_stainless_steel.webp
+-rw-r--r--   0 phil       (501) staff       (20)   101134 2023-04-04 15:15:05.606400 PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_yellow.webp
+-rw-r--r--   0 phil       (501) staff       (20)    27126 2023-04-04 15:15:05.607572 PyQt6_3D-6.5.0/examples/assets/metalbarrel/metal_barrel.obj
+-rw-r--r--   0 phil       (501) staff       (20)    29446 2023-04-04 15:15:05.608416 PyQt6_3D-6.5.0/examples/assets/metalbarrel/normal_hard_bumps.webp
+-rw-r--r--   0 phil       (501) staff       (20)    25560 2023-04-04 15:15:05.609274 PyQt6_3D-6.5.0/examples/assets/metalbarrel/normal_middle_bumps.webp
+-rw-r--r--   0 phil       (501) staff       (20)    21544 2023-04-04 15:15:05.610117 PyQt6_3D-6.5.0/examples/assets/metalbarrel/normal_no_bumps.webp
+-rw-r--r--   0 phil       (501) staff       (20)    23620 2023-04-04 15:15:05.610943 PyQt6_3D-6.5.0/examples/assets/metalbarrel/normal_soft_bumps.webp
+-rw-r--r--   0 phil       (501) staff       (20)   420416 2023-04-04 15:15:05.615135 PyQt6_3D-6.5.0/examples/assets/metalbarrel/specular.webp
+-rw-r--r--   0 phil       (501) staff       (20)   330298 2023-04-04 15:15:05.618200 PyQt6_3D-6.5.0/examples/assets/metalbarrel/specular_rust.webp
+-rw-r--r--   0 phil       (501) staff       (20)   220224 2023-04-04 15:15:05.620728 PyQt6_3D-6.5.0/examples/assets/metalbarrel/specular_stainless_steel.webp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.269120 PyQt6_3D-6.5.0/examples/assets/obj/
+-rw-r--r--   0 phil       (501) staff       (20)   346814 2023-04-04 15:15:05.624090 PyQt6_3D-6.5.0/examples/assets/obj/ball.obj
+-rw-r--r--   0 phil       (501) staff       (20)  1764501 2023-04-04 15:15:05.638475 PyQt6_3D-6.5.0/examples/assets/obj/toyplane.obj
+-rw-r--r--   0 phil       (501) staff       (20)   263373 2023-04-04 15:15:05.641770 PyQt6_3D-6.5.0/examples/assets/obj/trefoil.obj
+-rw-r--r--   0 phil       (501) staff       (20)   127711 2023-04-04 15:15:05.643511 PyQt6_3D-6.5.0/examples/assets/test_scene.dae
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.269687 PyQt6_3D-6.5.0/examples/assets/textures/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.272027 PyQt6_3D-6.5.0/examples/assets/textures/pattern_09/
+-rw-r--r--   0 phil       (501) staff       (20)   677322 2023-04-04 15:15:05.650981 PyQt6_3D-6.5.0/examples/assets/textures/pattern_09/diffuse.webp
+-rw-r--r--   0 phil       (501) staff       (20)   822594 2023-04-04 15:15:05.656782 PyQt6_3D-6.5.0/examples/assets/textures/pattern_09/normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-04 15:15:05.657509 PyQt6_3D-6.5.0/examples/assets/textures/pattern_09/readme.txt
+-rw-r--r--   0 phil       (501) staff       (20)  1005334 2023-04-04 15:15:05.666225 PyQt6_3D-6.5.0/examples/assets/textures/pattern_09/specular.webp
+-rw-r--r--   0 phil       (501) staff       (20)    10285 2023-04-04 15:15:05.667422 PyQt6_3D-6.5.0/examples/basicshapes-py.py
+-rw-r--r--   0 phil       (501) staff       (20)    18568 2023-04-04 15:15:05.668343 PyQt6_3D-6.5.0/examples/materials-py.py
+-rw-r--r--   0 phil       (501) staff       (20)     6082 2023-04-04 15:15:05.668993 PyQt6_3D-6.5.0/examples/simple-py.py
+-rw-r--r--   0 phil       (501) staff       (20)     1072 2023-04-04 15:19:40.740054 PyQt6_3D-6.5.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.358243 PyQt6_3D-6.5.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.357646 PyQt6_3D-6.5.0/sip/Qt3DAnimation/
+-rw-r--r--   0 phil       (501) staff       (20)     2857 2023-04-04 15:19:41.925782 PyQt6_3D-6.5.0/sip/Qt3DAnimation/Qt3DAnimationmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4844 2023-04-04 15:19:41.927792 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1344 2023-04-04 15:19:41.925282 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractanimationclip.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1257 2023-04-04 15:19:41.915648 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractchannelmapping.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2214 2023-04-04 15:19:41.916677 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractclipanimator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1336 2023-04-04 15:19:41.926179 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractclipblendnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1959 2023-04-04 15:19:41.918696 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qadditiveclipblend.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1286 2023-04-04 15:19:41.919628 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationaspect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1538 2023-04-04 15:19:41.922925 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationclip.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1631 2023-04-04 15:19:41.920945 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationclipdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1848 2023-04-04 15:19:41.917216 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationcliploader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2530 2023-04-04 15:19:41.921478 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationcontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1884 2023-04-04 15:19:41.915224 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationgroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1605 2023-04-04 15:19:41.916153 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qblendedclipanimator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1724 2023-04-04 15:19:41.923857 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qchannel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1659 2023-04-04 15:19:41.917668 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qchannelcomponent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1497 2023-04-04 15:19:41.920050 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qchannelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1758 2023-04-04 15:19:41.919209 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qchannelmapping.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1519 2023-04-04 15:19:41.924841 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qclipanimator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1646 2023-04-04 15:19:41.918156 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qclipblendvalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1381 2023-04-04 15:19:41.920478 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qclock.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2025 2023-04-04 15:19:41.926725 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qkeyframe.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2787 2023-04-04 15:19:41.924400 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qkeyframeanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1900 2023-04-04 15:19:41.914643 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qlerpclipblend.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2779 2023-04-04 15:19:41.922031 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qmorphinganimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1721 2023-04-04 15:19:41.922481 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qmorphtarget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1529 2023-04-04 15:19:41.927143 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qskeletonmapping.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2199 2023-04-04 15:19:41.923401 PyQt6_3D-6.5.0/sip/Qt3DAnimation/qvertexblendanimation.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.321103 PyQt6_3D-6.5.0/sip/Qt3DCore/
+-rw-r--r--   0 phil       (501) staff       (20)     2740 2023-04-04 15:19:41.816313 PyQt6_3D-6.5.0/sip/Qt3DCore/Qt3DCoremod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1557 2023-04-04 15:19:41.816848 PyQt6_3D-6.5.0/sip/Qt3DCore/qabstractaspect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1262 2023-04-04 15:19:41.811107 PyQt6_3D-6.5.0/sip/Qt3DCore/qabstractfunctor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1311 2023-04-04 15:19:41.817360 PyQt6_3D-6.5.0/sip/Qt3DCore/qabstractskeleton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1459 2023-04-04 15:19:41.809147 PyQt6_3D-6.5.0/sip/Qt3DCore/qarmature.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2108 2023-04-04 15:19:41.811731 PyQt6_3D-6.5.0/sip/Qt3DCore/qaspectengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4235 2023-04-04 15:19:41.818189 PyQt6_3D-6.5.0/sip/Qt3DCore/qattribute.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2024 2023-04-04 15:19:41.819956 PyQt6_3D-6.5.0/sip/Qt3DCore/qbackendnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2124 2023-04-04 15:19:41.819349 PyQt6_3D-6.5.0/sip/Qt3DCore/qboundingvolume.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2252 2023-04-04 15:19:41.807809 PyQt6_3D-6.5.0/sip/Qt3DCore/qbuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1604 2023-04-04 15:19:41.812855 PyQt6_3D-6.5.0/sip/Qt3DCore/qcomponent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1481 2023-04-04 15:19:41.809707 PyQt6_3D-6.5.0/sip/Qt3DCore/qcoresettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1740 2023-04-04 15:19:41.812304 PyQt6_3D-6.5.0/sip/Qt3DCore/qentity.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2182 2023-04-04 15:19:41.814420 PyQt6_3D-6.5.0/sip/Qt3DCore/qgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3346 2023-04-04 15:19:41.808595 PyQt6_3D-6.5.0/sip/Qt3DCore/qgeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2574 2023-04-04 15:19:41.807089 PyQt6_3D-6.5.0/sip/Qt3DCore/qjoint.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4044 2023-04-04 15:19:41.810595 PyQt6_3D-6.5.0/sip/Qt3DCore/qnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1631 2023-04-04 15:19:41.818758 PyQt6_3D-6.5.0/sip/Qt3DCore/qnodeid.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3247 2023-04-04 15:19:41.813816 PyQt6_3D-6.5.0/sip/Qt3DCore/qsharedpointer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1429 2023-04-04 15:19:41.814961 PyQt6_3D-6.5.0/sip/Qt3DCore/qskeleton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2040 2023-04-04 15:19:41.820550 PyQt6_3D-6.5.0/sip/Qt3DCore/qskeletonloader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3350 2023-04-04 15:19:41.815675 PyQt6_3D-6.5.0/sip/Qt3DCore/qtransform.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.347720 PyQt6_3D-6.5.0/sip/Qt3DExtras/
+-rw-r--r--   0 phil       (501) staff       (20)     3472 2023-04-04 15:19:41.912442 PyQt6_3D-6.5.0/sip/Qt3DExtras/Qt3DExtrasmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2125 2023-04-04 15:19:41.871072 PyQt6_3D-6.5.0/sip/Qt3DExtras/qabstractcameracontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1709 2023-04-04 15:19:41.873833 PyQt6_3D-6.5.0/sip/Qt3DExtras/qabstractspritesheet.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2448 2023-04-04 15:19:41.865352 PyQt6_3D-6.5.0/sip/Qt3DExtras/qconegeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2192 2023-04-04 15:19:41.912962 PyQt6_3D-6.5.0/sip/Qt3DExtras/qconegeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2150 2023-04-04 15:19:41.864004 PyQt6_3D-6.5.0/sip/Qt3DExtras/qconemesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2498 2023-04-04 15:19:41.868783 PyQt6_3D-6.5.0/sip/Qt3DExtras/qcuboidgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2186 2023-04-04 15:19:41.872226 PyQt6_3D-6.5.0/sip/Qt3DExtras/qcuboidgeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2144 2023-04-04 15:19:41.913473 PyQt6_3D-6.5.0/sip/Qt3DExtras/qcuboidmesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2028 2023-04-04 15:19:41.867132 PyQt6_3D-6.5.0/sip/Qt3DExtras/qcylindergeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1772 2023-04-04 15:19:41.869892 PyQt6_3D-6.5.0/sip/Qt3DExtras/qcylindergeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1730 2023-04-04 15:19:41.913956 PyQt6_3D-6.5.0/sip/Qt3DExtras/qcylindermesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2070 2023-04-04 15:19:41.861853 PyQt6_3D-6.5.0/sip/Qt3DExtras/qdiffusemapmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2191 2023-04-04 15:19:41.908374 PyQt6_3D-6.5.0/sip/Qt3DExtras/qdiffusespecularmapmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2329 2023-04-04 15:19:41.862505 PyQt6_3D-6.5.0/sip/Qt3DExtras/qdiffusespecularmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1880 2023-04-04 15:19:41.911281 PyQt6_3D-6.5.0/sip/Qt3DExtras/qextrudedtextgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1670 2023-04-04 15:19:41.909575 PyQt6_3D-6.5.0/sip/Qt3DExtras/qextrudedtextmesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1372 2023-04-04 15:19:41.880031 PyQt6_3D-6.5.0/sip/Qt3DExtras/qfirstpersoncameracontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2847 2023-04-04 15:19:41.863361 PyQt6_3D-6.5.0/sip/Qt3DExtras/qforwardrenderer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2138 2023-04-04 15:19:41.870496 PyQt6_3D-6.5.0/sip/Qt3DExtras/qgoochmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2235 2023-04-04 15:19:41.877826 PyQt6_3D-6.5.0/sip/Qt3DExtras/qmetalroughmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2001 2023-04-04 15:19:41.876306 PyQt6_3D-6.5.0/sip/Qt3DExtras/qmorphphongmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1384 2023-04-04 15:19:41.865876 PyQt6_3D-6.5.0/sip/Qt3DExtras/qnormaldiffusemapalphamaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2306 2023-04-04 15:19:41.866490 PyQt6_3D-6.5.0/sip/Qt3DExtras/qnormaldiffusemapmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2425 2023-04-04 15:19:41.876819 PyQt6_3D-6.5.0/sip/Qt3DExtras/qnormaldiffusespecularmapmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1468 2023-04-04 15:19:41.909092 PyQt6_3D-6.5.0/sip/Qt3DExtras/qorbitcameracontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1326 2023-04-04 15:19:41.867604 PyQt6_3D-6.5.0/sip/Qt3DExtras/qpervertexcolormaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3390 2023-04-04 15:19:41.864685 PyQt6_3D-6.5.0/sip/Qt3DExtras/qphongalphamaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1831 2023-04-04 15:19:41.875363 PyQt6_3D-6.5.0/sip/Qt3DExtras/qphongmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2119 2023-04-04 15:19:41.879614 PyQt6_3D-6.5.0/sip/Qt3DExtras/qplanegeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1823 2023-04-04 15:19:41.880523 PyQt6_3D-6.5.0/sip/Qt3DExtras/qplanegeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1827 2023-04-04 15:19:41.868177 PyQt6_3D-6.5.0/sip/Qt3DExtras/qplanemesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1813 2023-04-04 15:19:41.910098 PyQt6_3D-6.5.0/sip/Qt3DExtras/qskyboxentity.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2106 2023-04-04 15:19:41.911850 PyQt6_3D-6.5.0/sip/Qt3DExtras/qspheregeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1794 2023-04-04 15:19:41.869347 PyQt6_3D-6.5.0/sip/Qt3DExtras/qspheregeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1752 2023-04-04 15:19:41.873312 PyQt6_3D-6.5.0/sip/Qt3DExtras/qspheremesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1501 2023-04-04 15:19:41.875818 PyQt6_3D-6.5.0/sip/Qt3DExtras/qspritegrid.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1739 2023-04-04 15:19:41.874359 PyQt6_3D-6.5.0/sip/Qt3DExtras/qspritesheet.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1635 2023-04-04 15:19:41.874891 PyQt6_3D-6.5.0/sip/Qt3DExtras/qspritesheetitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7090 2023-04-04 15:19:41.878628 PyQt6_3D-6.5.0/sip/Qt3DExtras/qt3dwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1847 2023-04-04 15:19:41.910631 PyQt6_3D-6.5.0/sip/Qt3DExtras/qtext2dentity.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2009 2023-04-04 15:19:41.872773 PyQt6_3D-6.5.0/sip/Qt3DExtras/qtexturematerial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2035 2023-04-04 15:19:41.871656 PyQt6_3D-6.5.0/sip/Qt3DExtras/qtorusgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1779 2023-04-04 15:19:41.877319 PyQt6_3D-6.5.0/sip/Qt3DExtras/qtorusgeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1737 2023-04-04 15:19:41.879109 PyQt6_3D-6.5.0/sip/Qt3DExtras/qtorusmesh.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.329684 PyQt6_3D-6.5.0/sip/Qt3DInput/
+-rw-r--r--   0 phil       (501) staff       (20)     2590 2023-04-04 15:19:41.822742 PyQt6_3D-6.5.0/sip/Qt3DInput/Qt3DInputmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1234 2023-04-04 15:19:41.827927 PyQt6_3D-6.5.0/sip/Qt3DInput/qabstractactioninput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1506 2023-04-04 15:19:41.859280 PyQt6_3D-6.5.0/sip/Qt3DInput/qabstractaxisinput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4384 2023-04-04 15:19:41.824591 PyQt6_3D-6.5.0/sip/Qt3DInput/qabstractphysicaldevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1742 2023-04-04 15:19:41.825142 PyQt6_3D-6.5.0/sip/Qt3DInput/qaction.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1694 2023-04-04 15:19:41.828962 PyQt6_3D-6.5.0/sip/Qt3DInput/qactioninput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1417 2023-04-04 15:19:41.826239 PyQt6_3D-6.5.0/sip/Qt3DInput/qanalogaxisinput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1719 2023-04-04 15:19:41.823280 PyQt6_3D-6.5.0/sip/Qt3DInput/qaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2101 2023-04-04 15:19:41.825733 PyQt6_3D-6.5.0/sip/Qt3DInput/qaxisaccumulator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1688 2023-04-04 15:19:41.821180 PyQt6_3D-6.5.0/sip/Qt3DInput/qaxissetting.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1852 2023-04-04 15:19:41.831623 PyQt6_3D-6.5.0/sip/Qt3DInput/qbuttonaxisinput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1405 2023-04-04 15:19:41.822180 PyQt6_3D-6.5.0/sip/Qt3DInput/qinputaspect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1836 2023-04-04 15:19:41.830047 PyQt6_3D-6.5.0/sip/Qt3DInput/qinputchord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2010 2023-04-04 15:19:41.829512 PyQt6_3D-6.5.0/sip/Qt3DInput/qinputsequence.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1435 2023-04-04 15:19:41.826753 PyQt6_3D-6.5.0/sip/Qt3DInput/qinputsettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1795 2023-04-04 15:19:41.831099 PyQt6_3D-6.5.0/sip/Qt3DInput/qkeyboarddevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3906 2023-04-04 15:19:41.827450 PyQt6_3D-6.5.0/sip/Qt3DInput/qkeyboardhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1715 2023-04-04 15:19:41.821705 PyQt6_3D-6.5.0/sip/Qt3DInput/qkeyevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2048 2023-04-04 15:19:41.830616 PyQt6_3D-6.5.0/sip/Qt3DInput/qlogicaldevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2065 2023-04-04 15:19:41.823855 PyQt6_3D-6.5.0/sip/Qt3DInput/qmousedevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2756 2023-04-04 15:19:41.858537 PyQt6_3D-6.5.0/sip/Qt3DInput/qmouseevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2037 2023-04-04 15:19:41.828469 PyQt6_3D-6.5.0/sip/Qt3DInput/qmousehandler.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.330888 PyQt6_3D-6.5.0/sip/Qt3DLogic/
+-rw-r--r--   0 phil       (501) staff       (20)     2006 2023-04-04 15:19:41.859947 PyQt6_3D-6.5.0/sip/Qt3DLogic/Qt3DLogicmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2049 2023-04-04 15:19:41.860669 PyQt6_3D-6.5.0/sip/Qt3DLogic/qframeaction.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1254 2023-04-04 15:19:41.861157 PyQt6_3D-6.5.0/sip/Qt3DLogic/qlogicaspect.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:19:42.392158 PyQt6_3D-6.5.0/sip/Qt3DRender/
+-rw-r--r--   0 phil       (501) staff       (20)     4863 2023-04-04 15:19:42.066170 PyQt6_3D-6.5.0/sip/Qt3DRender/Qt3DRendermod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1664 2023-04-04 15:19:42.013078 PyQt6_3D-6.5.0/sip/Qt3DRender/qabstractlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2656 2023-04-04 15:19:42.059454 PyQt6_3D-6.5.0/sip/Qt3DRender/qabstractraycaster.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8855 2023-04-04 15:19:42.012107 PyQt6_3D-6.5.0/sip/Qt3DRender/qabstracttexture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1933 2023-04-04 15:19:42.018527 PyQt6_3D-6.5.0/sip/Qt3DRender/qabstracttextureimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1275 2023-04-04 15:19:42.015417 PyQt6_3D-6.5.0/sip/Qt3DRender/qalphacoverage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1915 2023-04-04 15:19:42.062752 PyQt6_3D-6.5.0/sip/Qt3DRender/qalphatest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1731 2023-04-04 15:19:41.976926 PyQt6_3D-6.5.0/sip/Qt3DRender/qblendequation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3658 2023-04-04 15:19:41.980063 PyQt6_3D-6.5.0/sip/Qt3DRender/qblendequationarguments.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2712 2023-04-04 15:19:42.060012 PyQt6_3D-6.5.0/sip/Qt3DRender/qblitframebuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)    15325 2023-04-04 15:19:41.970775 PyQt6_3D-6.5.0/sip/Qt3DRender/qcamera.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3588 2023-04-04 15:19:42.065348 PyQt6_3D-6.5.0/sip/Qt3DRender/qcameralens.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1466 2023-04-04 15:19:41.974192 PyQt6_3D-6.5.0/sip/Qt3DRender/qcameraselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2555 2023-04-04 15:19:41.973242 PyQt6_3D-6.5.0/sip/Qt3DRender/qclearbuffers.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1623 2023-04-04 15:19:42.008188 PyQt6_3D-6.5.0/sip/Qt3DRender/qclipplane.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1805 2023-04-04 15:19:42.058809 PyQt6_3D-6.5.0/sip/Qt3DRender/qcolormask.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2069 2023-04-04 15:19:41.960001 PyQt6_3D-6.5.0/sip/Qt3DRender/qcomputecommand.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1617 2023-04-04 15:19:42.016519 PyQt6_3D-6.5.0/sip/Qt3DRender/qcullface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1534 2023-04-04 15:19:42.058135 PyQt6_3D-6.5.0/sip/Qt3DRender/qdepthrange.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1765 2023-04-04 15:19:42.028274 PyQt6_3D-6.5.0/sip/Qt3DRender/qdepthtest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1504 2023-04-04 15:19:42.016027 PyQt6_3D-6.5.0/sip/Qt3DRender/qdirectionallight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1653 2023-04-04 15:19:42.020341 PyQt6_3D-6.5.0/sip/Qt3DRender/qdispatchcompute.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1251 2023-04-04 15:19:42.014959 PyQt6_3D-6.5.0/sip/Qt3DRender/qdithering.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2066 2023-04-04 15:19:42.067757 PyQt6_3D-6.5.0/sip/Qt3DRender/qeffect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1770 2023-04-04 15:19:42.016946 PyQt6_3D-6.5.0/sip/Qt3DRender/qenvironmentlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1529 2023-04-04 15:19:41.975998 PyQt6_3D-6.5.0/sip/Qt3DRender/qfilterkey.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1339 2023-04-04 15:19:42.066711 PyQt6_3D-6.5.0/sip/Qt3DRender/qframegraphnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1638 2023-04-04 15:19:42.064177 PyQt6_3D-6.5.0/sip/Qt3DRender/qfrontface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1284 2023-04-04 15:19:42.026789 PyQt6_3D-6.5.0/sip/Qt3DRender/qfrustumculling.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3665 2023-04-04 15:19:42.014575 PyQt6_3D-6.5.0/sip/Qt3DRender/qgeometryrenderer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2598 2023-04-04 15:19:41.958885 PyQt6_3D-6.5.0/sip/Qt3DRender/qgraphicsapifilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1345 2023-04-04 15:19:41.969401 PyQt6_3D-6.5.0/sip/Qt3DRender/qlayer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2112 2023-04-04 15:19:42.019895 PyQt6_3D-6.5.0/sip/Qt3DRender/qlayerfilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2582 2023-04-04 15:19:41.971432 PyQt6_3D-6.5.0/sip/Qt3DRender/qlevelofdetail.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1682 2023-04-04 15:19:42.025998 PyQt6_3D-6.5.0/sip/Qt3DRender/qlevelofdetailboundingsphere.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1313 2023-04-04 15:19:42.030848 PyQt6_3D-6.5.0/sip/Qt3DRender/qlevelofdetailswitch.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1498 2023-04-04 15:19:41.966615 PyQt6_3D-6.5.0/sip/Qt3DRender/qlinewidth.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7581 2023-04-04 15:19:42.062211 PyQt6_3D-6.5.0/sip/Qt3DRender/qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1635 2023-04-04 15:19:42.024249 PyQt6_3D-6.5.0/sip/Qt3DRender/qmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2100 2023-04-04 15:19:42.067264 PyQt6_3D-6.5.0/sip/Qt3DRender/qmemorybarrier.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1797 2023-04-04 15:19:41.977430 PyQt6_3D-6.5.0/sip/Qt3DRender/qmesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1335 2023-04-04 15:19:42.009095 PyQt6_3D-6.5.0/sip/Qt3DRender/qmultisampleantialiasing.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1263 2023-04-04 15:19:42.022121 PyQt6_3D-6.5.0/sip/Qt3DRender/qnodepthmask.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1236 2023-04-04 15:19:42.063187 PyQt6_3D-6.5.0/sip/Qt3DRender/qnodraw.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1254 2023-04-04 15:19:42.026390 PyQt6_3D-6.5.0/sip/Qt3DRender/qnopicking.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2105 2023-04-04 15:19:41.968974 PyQt6_3D-6.5.0/sip/Qt3DRender/qobjectpicker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1850 2023-04-04 15:19:41.967777 PyQt6_3D-6.5.0/sip/Qt3DRender/qpaintedtextureimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1752 2023-04-04 15:19:41.963090 PyQt6_3D-6.5.0/sip/Qt3DRender/qparameter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2414 2023-04-04 15:19:42.028807 PyQt6_3D-6.5.0/sip/Qt3DRender/qpickevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1270 2023-04-04 15:19:41.960843 PyQt6_3D-6.5.0/sip/Qt3DRender/qpickingproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2955 2023-04-04 15:19:41.931002 PyQt6_3D-6.5.0/sip/Qt3DRender/qpickingsettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1583 2023-04-04 15:19:41.973711 PyQt6_3D-6.5.0/sip/Qt3DRender/qpicklineevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1484 2023-04-04 15:19:41.975096 PyQt6_3D-6.5.0/sip/Qt3DRender/qpickpointevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1944 2023-04-04 15:19:42.027264 PyQt6_3D-6.5.0/sip/Qt3DRender/qpicktriangleevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1771 2023-04-04 15:19:42.029251 PyQt6_3D-6.5.0/sip/Qt3DRender/qpointlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1698 2023-04-04 15:19:41.979454 PyQt6_3D-6.5.0/sip/Qt3DRender/qpointsize.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1573 2023-04-04 15:19:41.980551 PyQt6_3D-6.5.0/sip/Qt3DRender/qpolygonoffset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1637 2023-04-04 15:19:42.009603 PyQt6_3D-6.5.0/sip/Qt3DRender/qproximityfilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1924 2023-04-04 15:19:42.027822 PyQt6_3D-6.5.0/sip/Qt3DRender/qrastermode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1800 2023-04-04 15:19:42.025467 PyQt6_3D-6.5.0/sip/Qt3DRender/qraycaster.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2004 2023-04-04 15:19:41.961612 PyQt6_3D-6.5.0/sip/Qt3DRender/qraycasterhit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1151 2023-04-04 15:19:42.010153 PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderapi.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1555 2023-04-04 15:19:41.965273 PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderaspect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2740 2023-04-04 15:19:41.981190 PyQt6_3D-6.5.0/sip/Qt3DRender/qrendercapabilities.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1846 2023-04-04 15:19:42.060523 PyQt6_3D-6.5.0/sip/Qt3DRender/qrendercapture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2788 2023-04-04 15:19:42.019276 PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderpass.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2140 2023-04-04 15:19:41.972647 PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderpassfilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2036 2023-04-04 15:19:42.022626 PyQt6_3D-6.5.0/sip/Qt3DRender/qrendersettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1196 2023-04-04 15:19:42.024639 PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderstate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1719 2023-04-04 15:19:42.064682 PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderstateset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1804 2023-04-04 15:19:41.975555 PyQt6_3D-6.5.0/sip/Qt3DRender/qrendersurfaceselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1703 2023-04-04 15:19:42.063685 PyQt6_3D-6.5.0/sip/Qt3DRender/qrendertarget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2734 2023-04-04 15:19:42.029795 PyQt6_3D-6.5.0/sip/Qt3DRender/qrendertargetoutput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1545 2023-04-04 15:19:41.967146 PyQt6_3D-6.5.0/sip/Qt3DRender/qrendertargetselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2168 2023-04-04 15:19:42.010754 PyQt6_3D-6.5.0/sip/Qt3DRender/qsceneloader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1697 2023-04-04 15:19:41.928396 PyQt6_3D-6.5.0/sip/Qt3DRender/qscissortest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1533 2023-04-04 15:19:41.976454 PyQt6_3D-6.5.0/sip/Qt3DRender/qscreenraycaster.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1287 2023-04-04 15:19:42.008631 PyQt6_3D-6.5.0/sip/Qt3DRender/qseamlesscubemap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1575 2023-04-04 15:19:42.012569 PyQt6_3D-6.5.0/sip/Qt3DRender/qsetfence.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1690 2023-04-04 15:19:41.962101 PyQt6_3D-6.5.0/sip/Qt3DRender/qshaderdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3207 2023-04-04 15:19:41.929841 PyQt6_3D-6.5.0/sip/Qt3DRender/qshaderimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3718 2023-04-04 15:19:41.972144 PyQt6_3D-6.5.0/sip/Qt3DRender/qshaderprogram.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3778 2023-04-04 15:19:41.928955 PyQt6_3D-6.5.0/sip/Qt3DRender/qshaderprogrambuilder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1904 2023-04-04 15:19:42.020873 PyQt6_3D-6.5.0/sip/Qt3DRender/qsortpolicy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2076 2023-04-04 15:19:41.964678 PyQt6_3D-6.5.0/sip/Qt3DRender/qspotlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1595 2023-04-04 15:19:42.030414 PyQt6_3D-6.5.0/sip/Qt3DRender/qstencilmask.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1418 2023-04-04 15:19:41.965717 PyQt6_3D-6.5.0/sip/Qt3DRender/qstenciloperation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2778 2023-04-04 15:19:41.968423 PyQt6_3D-6.5.0/sip/Qt3DRender/qstenciloperationarguments.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1378 2023-04-04 15:19:42.025030 PyQt6_3D-6.5.0/sip/Qt3DRender/qstenciltest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2409 2023-04-04 15:19:42.023138 PyQt6_3D-6.5.0/sip/Qt3DRender/qstenciltestarguments.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1655 2023-04-04 15:19:41.966174 PyQt6_3D-6.5.0/sip/Qt3DRender/qsubtreeenabler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2572 2023-04-04 15:19:42.021391 PyQt6_3D-6.5.0/sip/Qt3DRender/qtechnique.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2118 2023-04-04 15:19:41.978453 PyQt6_3D-6.5.0/sip/Qt3DRender/qtechniquefilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4644 2023-04-04 15:19:42.017928 PyQt6_3D-6.5.0/sip/Qt3DRender/qtexture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3172 2023-04-04 15:19:41.977961 PyQt6_3D-6.5.0/sip/Qt3DRender/qtexturedata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2108 2023-04-04 15:19:41.963879 PyQt6_3D-6.5.0/sip/Qt3DRender/qtexturedataupdate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2041 2023-04-04 15:19:41.930436 PyQt6_3D-6.5.0/sip/Qt3DRender/qtextureimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2474 2023-04-04 15:19:42.013831 PyQt6_3D-6.5.0/sip/Qt3DRender/qtextureimagedata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1539 2023-04-04 15:19:41.962531 PyQt6_3D-6.5.0/sip/Qt3DRender/qtextureimagedatagenerator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2330 2023-04-04 15:19:41.978958 PyQt6_3D-6.5.0/sip/Qt3DRender/qtexturewrapmode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1599 2023-04-04 15:19:42.023575 PyQt6_3D-6.5.0/sip/Qt3DRender/qviewport.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1943 2023-04-04 15:19:41.974685 PyQt6_3D-6.5.0/sip/Qt3DRender/qwaitfence.sip
```

### Comparing `PyQt6_3D-6.4.0/ChangeLog` & `PyQt6_3D-6.5.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+2023-03-31  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-3D.msp:
+	Updated for Qt v6.5.0rc.
+	[56538be6fbcd] [6.5.0]
+
 2022-09-30  Phil Thompson  <phil@riverbankcomputing.com>
 
+	* .hgtags:
+	Added tag 6.4.0 for changeset ed2fbf0055ac
+	[88ee04b892d8]
+
 	* NEWS, PyQt6-3D.msp:
 	Updated for Qt v6.4.0.
 	[ed2fbf0055ac] [6.4.0]
 
 2022-09-21  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-3D.msp:
```

### Comparing `PyQt6_3D-6.4.0/LICENSE` & `PyQt6_3D-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/NEWS` & `PyQt6_3D-6.5.0/NEWS`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+v6.5.0 31st March 2023
+  - Added support for Qt v6.5.
+
 v6.4.0 30th September 2022
   - Added support for Qt v6.4.
 
 v6.3.0 31st March 2022
   - Added support for Qt v6.3.
 
 v6.2.0 30th September 2021
```

### Comparing `PyQt6_3D-6.4.0/PKG-INFO` & `PyQt6_3D-6.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-3D
-Version: 6.4.0
+Version: 6.5.0
 Requires-Python: >=3.7
 Summary: Python bindings for the Qt 3D framework
 Home-Page: https://www.riverbankcomputing.com/software/pyqt3d/
 Author: Riverbank Computing Limited
 Author-Email: info@riverbankcomputing.com
 License: GPL v3
 Requires-Dist: PyQt6 (>=6.2.0)
```

### Comparing `PyQt6_3D-6.4.0/README` & `PyQt6_3D-6.5.0/README`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/chest/Chest.obj` & `PyQt6_3D-6.5.0/examples/assets/chest/Chest.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/chest/diffuse.webp` & `PyQt6_3D-6.5.0/examples/assets/chest/diffuse.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_negx.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_negx.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_negy.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_negy.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_negz.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_negz.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_posx.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_posx.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_posy.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_posy.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/miramar/miramar_posz.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/miramar/miramar_posz.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_negx.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_negx.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_negy.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_negy.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_negz.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_negz.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_posx.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_posx.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_posy.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_posy.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/cubemaps/night/night_posz.webp` & `PyQt6_3D-6.5.0/examples/assets/cubemaps/night/night_posz.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/gltf/LICENSE.md` & `PyQt6_3D-6.5.0/examples/assets/gltf/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/gltf/wine/Wood_Cherry_Original_.jpg` & `PyQt6_3D-6.5.0/examples/assets/gltf/wine/Wood_Cherry_Original_.jpg`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/gltf/wine/_2004_old_vine_zinfandel_btl_xlg.jpg` & `PyQt6_3D-6.5.0/examples/assets/gltf/wine/_2004_old_vine_zinfandel_btl_xlg.jpg`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/gltf/wine/artezin_bottle.jpg` & `PyQt6_3D-6.5.0/examples/assets/gltf/wine/artezin_bottle.jpg`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine.bin` & `PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine.bin`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine.dae` & `PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine.dae`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/gltf/wine/wine.gltf` & `PyQt6_3D-6.5.0/examples/assets/gltf/wine/wine.gltf`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/bamboo.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/bamboo.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/bamboo_normal.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/bamboo_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cover.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cover.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cover_normal.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cover_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cross-bamboo.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cross-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cross-palm.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cross-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cross-pine.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cross-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cross-pot-cover.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cross-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cross-pot.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cross-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cross-shrub.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cross-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cross-spikes.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cross-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-bamboo.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-palm.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-pine.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-pot-cover.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-pot.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-shrub.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/cylinder-spikes.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/cylinder-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/palm.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/palm.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/palm_normal.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/palm_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/pine.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/pine.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/pine_normal.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/pine_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/pot.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/pot.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/pot_normal.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/pot_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/shrub.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/shrub.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/shrub_normal.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/shrub_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-bamboo.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-palm.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-pine.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-pot-cover.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-pot.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-shrub.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/sphere-spikes.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/sphere-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/spikes.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/spikes.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/spikes_normal.webp` & `PyQt6_3D-6.5.0/examples/assets/houseplants/spikes_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/square-bamboo.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/square-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/square-palm.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/square-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/square-pine.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/square-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/square-pot-cover.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/square-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/square-pot.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/square-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/square-shrub.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/square-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/square-spikes.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/square-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-bamboo.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-palm.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-pine.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-pot-cover.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-pot.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-shrub.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/houseplants/triangle-spikes.obj` & `PyQt6_3D-6.5.0/examples/assets/houseplants/triangle-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_black.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_black.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_blue.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_blue.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_green.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_green.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_red.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_red.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_rust.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_rust.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_stainless_steel.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_stainless_steel.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/diffus_yellow.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/diffus_yellow.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/metal_barrel.obj` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/metal_barrel.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/normal_hard_bumps.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/normal_hard_bumps.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/normal_middle_bumps.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/normal_middle_bumps.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/normal_no_bumps.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/normal_no_bumps.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/normal_soft_bumps.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/normal_soft_bumps.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/specular.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/specular.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/specular_rust.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/specular_rust.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/metalbarrel/specular_stainless_steel.webp` & `PyQt6_3D-6.5.0/examples/assets/metalbarrel/specular_stainless_steel.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/obj/ball.obj` & `PyQt6_3D-6.5.0/examples/assets/obj/ball.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/obj/toyplane.obj` & `PyQt6_3D-6.5.0/examples/assets/obj/toyplane.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/obj/trefoil.obj` & `PyQt6_3D-6.5.0/examples/assets/obj/trefoil.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/test_scene.dae` & `PyQt6_3D-6.5.0/examples/assets/test_scene.dae`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/textures/pattern_09/diffuse.webp` & `PyQt6_3D-6.5.0/examples/assets/textures/pattern_09/diffuse.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/textures/pattern_09/normal.webp` & `PyQt6_3D-6.5.0/examples/assets/textures/pattern_09/normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/assets/textures/pattern_09/specular.webp` & `PyQt6_3D-6.5.0/examples/assets/textures/pattern_09/specular.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/basicshapes-py.py` & `PyQt6_3D-6.5.0/examples/basicshapes-py.py`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/materials-py.py` & `PyQt6_3D-6.5.0/examples/materials-py.py`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/examples/simple-py.py` & `PyQt6_3D-6.5.0/examples/simple-py.py`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.4.0/pyproject.toml` & `PyQt6_3D-6.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["sip >=6, <7", "PyQt-builder >=1.9, <2"]
 build-backend = "sipbuild.api"
 
 # Specify the PEP 566 metadata for the project.
 [tool.sip.metadata]
 name = "PyQt6-3D"
-version = "6.4.0"
+version = "6.5.0"
 summary = "Python bindings for the Qt 3D framework"
 home-page = "https://www.riverbankcomputing.com/software/pyqt3d/"
 author = "Riverbank Computing Limited"
 author-email = "info@riverbankcomputing.com"
 license = "GPL v3"
 description-file = "README"
 requires-dist = "PyQt6 (>=6.2.0)"
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/Qt3DAnimationmod.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/Qt3DAnimationmod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DAnimationmod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -23,15 +23,15 @@
 %Module(name=PyQt6.Qt3DAnimation, keyword_arguments="Optional", use_limited_api=True)
 
 %Import Qt3DCore/Qt3DCoremod.sip
 %Import Qt3DRender/Qt3DRendermod.sip
 %Import QtCore/QtCoremod.sip
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractanimation.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractanimation.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractanimation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractanimationclip.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractanimationclip.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractanimationclip.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractchannelmapping.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractchannelmapping.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractchannelmapping.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractclipanimator.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractclipanimator.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractclipanimator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qabstractclipblendnode.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qabstractclipblendnode.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractclipblendnode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qadditiveclipblend.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qadditiveclipblend.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qadditiveclipblend.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationaspect.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationaspect.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationaspect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationclip.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationclip.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationclip.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationclipdata.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationclipdata.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationclipdata.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationcliploader.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationcliploader.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationcliploader.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationcontroller.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationcontroller.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationcontroller.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qanimationgroup.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qanimationgroup.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationgroup.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qblendedclipanimator.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qblendedclipanimator.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qblendedclipanimator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qchannel.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qchannel.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchannel.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qchannelcomponent.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qchannelcomponent.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchannelcomponent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qchannelmapper.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qchannelmapper.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchannelmapper.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qchannelmapping.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qchannelmapping.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchannelmapping.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qclipanimator.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qclipanimator.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclipanimator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qclipblendvalue.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qclipblendvalue.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclipblendvalue.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qclock.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qclock.sip`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclock.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qkeyframe.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qkeyframe.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyframe.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qkeyframeanimation.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qkeyframeanimation.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyframeanimation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qlerpclipblend.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qlerpclipblend.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlerpclipblend.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qmorphinganimation.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qmorphinganimation.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmorphinganimation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qmorphtarget.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qmorphtarget.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmorphtarget.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qskeletonmapping.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qskeletonmapping.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qskeletonmapping.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DAnimation/qvertexblendanimation.sip` & `PyQt6_3D-6.5.0/sip/Qt3DAnimation/qvertexblendanimation.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvertexblendanimation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/Qt3DCoremod.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/Qt3DCoremod.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DCoremod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -21,18 +21,18 @@
 
 
 %Module(name=PyQt6.Qt3DCore, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 
-%Timeline {Qt3D_6_0_0 Qt3D_6_1_0 Qt3D_6_2_0 Qt3D_6_3_0 Qt3D_6_4_0}
+%Timeline {Qt3D_6_0_0 Qt3D_6_1_0 Qt3D_6_2_0 Qt3D_6_3_0 Qt3D_6_4_0 Qt3D_6_5_0}
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -49,16 +49,16 @@
 %DefaultSupertype PyQt6.sip.simplewrapper
 %HideNamespace Qt3DCore
 
 int PYQT_3D_VERSION;
 const char *PYQT_3D_VERSION_STR;
 
 %ModuleCode
-static int PYQT_3D_VERSION = 0x060400;
-static const char *PYQT_3D_VERSION_STR = "6.4.0";
+static int PYQT_3D_VERSION = 0x060500;
+static const char *PYQT_3D_VERSION_STR = "6.5.0";
 %End
 
 %Include qabstractaspect.sip
 %Include qabstractfunctor.sip
 %Include qabstractskeleton.sip
 %Include qarmature.sip
 %Include qaspectengine.sip
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qabstractaspect.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qabstractaspect.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractaspect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qabstractfunctor.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qabstractfunctor.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractfunctor.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qabstractskeleton.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qabstractskeleton.sip`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractskeleton.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qarmature.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qarmature.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qarmature.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qaspectengine.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qaspectengine.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaspectengine.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qattribute.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qattribute.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qattribute.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qbackendnode.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qbackendnode.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbackendnode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qboundingvolume.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qboundingvolume.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qboundingvolume.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qbuffer.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qbuffer.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbuffer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qcomponent.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qcomponent.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcomponent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qcoresettings.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qcoresettings.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcoresettings.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qentity.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qentity.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qentity.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qgeometry.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qgeometry.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qgeometryview.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qgeometryview.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qjoint.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qjoint.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qjoint.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qnode.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qnode.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qnodeid.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qnodeid.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnodeid.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qsharedpointer.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qsharedpointer.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // This is the SIP interface definition for the QSharedPointer based mapped
 // types specific to PyQt3D.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qskeleton.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qskeleton.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qskeleton.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qskeletonloader.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qskeletonloader.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qskeletonloader.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DCore/qtransform.sip` & `PyQt6_3D-6.5.0/sip/Qt3DCore/qtransform.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtransform.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/Qt3DExtrasmod.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/Qt3DExtrasmod.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DExtrasmod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -25,15 +25,15 @@
 %Import Qt3DCore/Qt3DCoremod.sip
 %Import Qt3DInput/Qt3DInputmod.sip
 %Import Qt3DRender/Qt3DRendermod.sip
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qabstractcameracontroller.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qabstractcameracontroller.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractcameracontroller.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qabstractspritesheet.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qabstractspritesheet.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractspritesheet.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qconegeometry.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qconegeometry.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qconegeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qconegeometryview.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qconegeometryview.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qconegeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qconemesh.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qconemesh.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qconemesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qcuboidgeometry.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qcuboidgeometry.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcuboidgeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qcuboidgeometryview.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qcuboidgeometryview.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcuboidgeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qcuboidmesh.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qcuboidmesh.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcuboidmesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qcylindergeometry.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qcylindergeometry.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcylindergeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qcylindergeometryview.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qcylindergeometryview.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcylindergeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qcylindermesh.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qcylindermesh.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcylindermesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qdiffusemapmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qdiffusemapmaterial.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdiffusemapmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qdiffusespecularmapmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qdiffusespecularmapmaterial.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdiffusespecularmapmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qdiffusespecularmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qdiffusespecularmaterial.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdiffusespecularmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qextrudedtextgeometry.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qextrudedtextgeometry.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qextrudedtextgeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qextrudedtextmesh.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qextrudedtextmesh.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qextrudedtextmesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qfirstpersoncameracontroller.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qfirstpersoncameracontroller.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qfirstpersoncameracontroller.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qforwardrenderer.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qforwardrenderer.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qforwardrenderer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qgoochmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qgoochmaterial.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgoochmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qmetalroughmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qmetalroughmaterial.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmetalroughmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qmorphphongmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qmorphphongmaterial.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmorphphongmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qnormaldiffusemapalphamaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qnormaldiffusemapalphamaterial.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnormaldiffusemapalphamaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qnormaldiffusemapmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qnormaldiffusemapmaterial.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnormaldiffusemapmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qnormaldiffusespecularmapmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qnormaldiffusespecularmapmaterial.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnormaldiffusespecularmapmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qorbitcameracontroller.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qorbitcameracontroller.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qorbitcameracontroller.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qpervertexcolormaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qpervertexcolormaterial.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpervertexcolormaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qphongalphamaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qphongalphamaterial.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qphongalphamaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qphongmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qphongmaterial.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qphongmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qplanegeometry.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qplanegeometry.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qplanegeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qplanegeometryview.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qplanegeometryview.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qplanegeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qplanemesh.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qplanemesh.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qplanemesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qskyboxentity.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qskyboxentity.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qskyboxentity.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qspheregeometry.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qspheregeometry.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspheregeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qspheregeometryview.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qspheregeometryview.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspheregeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qspheremesh.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qspheremesh.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspheremesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qspritegrid.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qspritegrid.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspritegrid.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qspritesheet.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qspritesheet.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspritesheet.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qspritesheetitem.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qspritesheetitem.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspritesheetitem.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qt3dwindow.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qt3dwindow.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qt3dwindow.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qtext2dentity.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qtext2dentity.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtext2dentity.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qtexturematerial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qtexturematerial.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexturematerial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qtorusgeometry.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qtorusgeometry.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtorusgeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qtorusgeometryview.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qtorusgeometryview.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtorusgeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DExtras/qtorusmesh.sip` & `PyQt6_3D-6.5.0/sip/Qt3DExtras/qtorusmesh.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtorusmesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/Qt3DInputmod.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/Qt3DInputmod.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DInputmod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -23,15 +23,15 @@
 %Module(name=PyQt6.Qt3DInput, keyword_arguments="Optional", use_limited_api=True)
 
 %Import Qt3DCore/Qt3DCoremod.sip
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qabstractactioninput.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qabstractactioninput.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractactioninput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qabstractaxisinput.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qabstractaxisinput.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractaxisinput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qabstractphysicaldevice.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qabstractphysicaldevice.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractphysicaldevice.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qaction.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qaction.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaction.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qactioninput.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qactioninput.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qactioninput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qanalogaxisinput.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qanalogaxisinput.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanalogaxisinput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qaxis.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qaxis.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaxis.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qaxisaccumulator.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qaxisaccumulator.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaxisaccumulator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qaxissetting.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qaxissetting.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaxissetting.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qbuttonaxisinput.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qbuttonaxisinput.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbuttonaxisinput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qinputaspect.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qinputaspect.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qinputaspect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qinputchord.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qinputchord.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qinputchord.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qinputsequence.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qinputsequence.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qinputsequence.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qinputsettings.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qinputsettings.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qinputsettings.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qkeyboarddevice.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qkeyboarddevice.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyboarddevice.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qkeyboardhandler.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qkeyboardhandler.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyboardhandler.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qkeyevent.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qkeyevent.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qlogicaldevice.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qlogicaldevice.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlogicaldevice.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qmousedevice.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qmousedevice.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmousedevice.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qmouseevent.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qmouseevent.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmouseevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DInput/qmousehandler.sip` & `PyQt6_3D-6.5.0/sip/Qt3DInput/qmousehandler.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmousehandler.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DLogic/Qt3DLogicmod.sip` & `PyQt6_3D-6.5.0/sip/Qt3DLogic/Qt3DLogicmod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DLogicmod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DLogic Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -21,15 +21,15 @@
 
 
 %Module(name=PyQt6.Qt3DLogic, keyword_arguments="Optional", use_limited_api=True)
 
 %Import Qt3DCore/Qt3DCoremod.sip
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DLogic/qframeaction.sip` & `PyQt6_3D-6.5.0/sip/Qt3DLogic/qframeaction.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qframeaction.sip generated by MetaSIP
 //
 // This file is part of the Qt3DLogic Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DLogic/qlogicaspect.sip` & `PyQt6_3D-6.5.0/sip/Qt3DLogic/qlogicaspect.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlogicaspect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DLogic Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/Qt3DRendermod.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/Qt3DRendermod.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DRendermod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -24,15 +24,15 @@
 
 %Import Qt3DCore/Qt3DCoremod.sip
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 %Import QtOpenGL/QtOpenGLmod.sip
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qabstractlight.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qabstractlight.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractlight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qabstractraycaster.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qabstractraycaster.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractraycaster.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qabstracttexture.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qabstracttexture.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstracttexture.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qabstracttextureimage.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qabstracttextureimage.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstracttextureimage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qalphacoverage.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qalphacoverage.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qalphacoverage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qalphatest.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qalphatest.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qalphatest.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qblendequation.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qblendequation.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qblendequation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qblendequationarguments.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qblendequationarguments.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qblendequationarguments.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qblitframebuffer.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qblitframebuffer.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qblitframebuffer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qcamera.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qcamera.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcamera.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qcameralens.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qcameralens.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcameralens.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qcameraselector.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qcameraselector.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcameraselector.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qclearbuffers.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qclearbuffers.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclearbuffers.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qclipplane.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qclipplane.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclipplane.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qcolormask.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qcolormask.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcolormask.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qcomputecommand.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qcomputecommand.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcomputecommand.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qcullface.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qcullface.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcullface.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qdepthrange.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qdepthrange.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdepthrange.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qdepthtest.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qdepthtest.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdepthtest.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qdirectionallight.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qdirectionallight.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdirectionallight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qdispatchcompute.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qdispatchcompute.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdispatchcompute.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qdithering.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qdithering.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdithering.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qeffect.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qeffect.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qeffect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qenvironmentlight.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qenvironmentlight.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qenvironmentlight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qfilterkey.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qfilterkey.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qfilterkey.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qframegraphnode.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qframegraphnode.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qframegraphnode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qfrontface.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qfrontface.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qfrontface.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qfrustumculling.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qfrustumculling.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qfrustumculling.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qgeometryrenderer.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qgeometryrenderer.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgeometryrenderer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qgraphicsapifilter.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qgraphicsapifilter.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgraphicsapifilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qlayer.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qlayer.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlayer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qlayerfilter.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qlayerfilter.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlayerfilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qlevelofdetail.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qlevelofdetail.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlevelofdetail.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qlevelofdetailboundingsphere.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qlevelofdetailboundingsphere.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlevelofdetailboundingsphere.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qlevelofdetailswitch.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qlevelofdetailswitch.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlevelofdetailswitch.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qlinewidth.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qlinewidth.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlinewidth.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qlist.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qlist.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // This is the SIP interface definition for the QList based mapped types
 // specific to Qt3DRender.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qmaterial.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qmaterial.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qmemorybarrier.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qmemorybarrier.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmemorybarrier.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qmesh.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qmesh.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qmultisampleantialiasing.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qmultisampleantialiasing.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmultisampleantialiasing.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qnodepthmask.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qnodepthmask.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnodepthmask.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qnodraw.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qnodraw.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnodraw.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qnopicking.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qnopicking.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnopicking.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qobjectpicker.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qobjectpicker.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qobjectpicker.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpaintedtextureimage.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpaintedtextureimage.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpaintedtextureimage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qparameter.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qparameter.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qparameter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpickevent.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpickevent.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpickevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpickingproxy.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpickingproxy.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpickingproxy.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpickingsettings.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpickingsettings.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpickingsettings.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpicklineevent.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpicklineevent.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpicklineevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpickpointevent.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpickpointevent.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpickpointevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpicktriangleevent.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpicktriangleevent.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpicktriangleevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpointlight.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpointlight.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpointlight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpointsize.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpointsize.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpointsize.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qpolygonoffset.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qpolygonoffset.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpolygonoffset.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qproximityfilter.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qproximityfilter.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qproximityfilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrastermode.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrastermode.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrastermode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qraycaster.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qraycaster.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qraycaster.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qraycasterhit.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qraycasterhit.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qraycasterhit.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderapi.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderapi.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderapi.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderaspect.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderaspect.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderaspect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrendercapabilities.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrendercapabilities.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendercapabilities.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrendercapture.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrendercapture.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendercapture.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderpass.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderpass.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderpass.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderpassfilter.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderpassfilter.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderpassfilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrendersettings.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrendersettings.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendersettings.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderstate.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderstate.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderstate.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrenderstateset.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrenderstateset.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderstateset.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrendersurfaceselector.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrendersurfaceselector.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendersurfaceselector.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrendertarget.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrendertarget.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendertarget.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrendertargetoutput.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrendertargetoutput.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendertargetoutput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qrendertargetselector.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qrendertargetselector.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendertargetselector.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qsceneloader.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qsceneloader.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsceneloader.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qscissortest.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qscissortest.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscissortest.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qscreenraycaster.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qscreenraycaster.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscreenraycaster.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qseamlesscubemap.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qseamlesscubemap.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qseamlesscubemap.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qsetfence.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qsetfence.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsetfence.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qshaderdata.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qshaderdata.sip`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qshaderdata.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qshaderimage.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qshaderimage.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qshaderimage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qshaderprogram.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qshaderprogram.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qshaderprogram.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qshaderprogrambuilder.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qshaderprogrambuilder.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qshaderprogrambuilder.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qsortpolicy.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qsortpolicy.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsortpolicy.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qspotlight.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qspotlight.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspotlight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qstencilmask.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qstencilmask.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstencilmask.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qstenciloperation.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qstenciloperation.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstenciloperation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qstenciloperationarguments.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qstenciloperationarguments.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstenciloperationarguments.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qstenciltest.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qstenciltest.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstenciltest.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qstenciltestarguments.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qstenciltestarguments.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstenciltestarguments.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qsubtreeenabler.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qsubtreeenabler.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsubtreeenabler.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qtechnique.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qtechnique.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtechnique.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qtechniquefilter.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qtechniquefilter.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtechniquefilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qtexture.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qtexture.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexture.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qtexturedata.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qtexturedata.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexturedata.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qtexturedataupdate.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qtexturedataupdate.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexturedataupdate.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qtextureimage.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qtextureimage.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtextureimage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qtextureimagedata.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qtextureimagedata.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtextureimagedata.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qtextureimagedatagenerator.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qtextureimagedatagenerator.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtextureimagedatagenerator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qtexturewrapmode.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qtexturewrapmode.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexturewrapmode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qviewport.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qviewport.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qviewport.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.4.0/sip/Qt3DRender/qwaitfence.sip` & `PyQt6_3D-6.5.0/sip/Qt3DRender/qwaitfence.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwaitfence.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

