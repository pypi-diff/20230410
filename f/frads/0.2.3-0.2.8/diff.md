# Comparing `tmp/frads-0.2.3.tar.gz` & `tmp/frads-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frads-0.2.3.tar", last modified: Mon Apr 11 22:16:42 2022, max compression
+gzip compressed data, was "frads-0.2.8.tar", last modified: Thu Oct 27 19:48:50 2022, max compression
```

## Comparing `frads-0.2.3.tar` & `frads-0.2.8.tar`

### file list

```diff
@@ -1,130 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 22:16:42.494768 frads-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     4946 2022-04-11 22:16:42.494768 frads-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4541 2022-04-11 22:16:32.000000 frads-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 22:16:42.478768 frads-0.2.3/frads/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1305 2022-04-11 22:16:32.000000 frads-0.2.3/frads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 22:16:42.478768 frads-0.2.3/frads/data/
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/WC.DAT
--rw-r--r--   0 runner    (1001) docker     (121)   929489 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/epw_url.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 22:16:42.494768 frads-0.2.3/frads/data/standards/
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1931 X.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1931 X.loc
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1931 Y.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1931 Y.loc
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1931 Z.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1964 X.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1964 X.loc
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1964 Y.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1964 Y.loc
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 1964 Z.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Illuminant A.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Illuminant C.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Illuminant D50.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Illuminant D55.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Illuminant D65.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Table 5-1 X.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Table 5-1 Y.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Table 5-1 Z.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Table 5-19 X.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Table 5-19 Y.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E308 Table 5-19 Z.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E891 Table 1 Direct AM1_5.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM E891 Table3 50 Sel Ord AM1_5.ssp
--rw-r--r--   0 runner    (1001) docker     (121)    26829 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM G173 AM1_5 37 Tilt Direct Full Spectrum.ssp
--rw-r--r--   0 runner    (1001) docker     (121)    26346 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM G173 AM1_5 37 Tilt Global Full Spectrum.ssp
--rw-r--r--   0 runner    (1001) docker     (121)    26380 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM G197 AM1_5 20 Tilt Direct Full Spectrum.ssp
--rw-r--r--   0 runner    (1001) docker     (121)    26353 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM G197 AM1_5 20 Tilt Global Full Spectrum.ssp
--rw-r--r--   0 runner    (1001) docker     (121)    26413 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM G197 AM1_5 90 Tilt Direct Full Spectrum.ssp
--rw-r--r--   0 runner    (1001) docker     (121)    26309 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ASTM G197 AM1_5 90 Tilt Global Full Spectrum.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     9259 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 1nm X.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     7721 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 1nm X.loc
--rw-r--r--   0 runner    (1001) docker     (121)     9317 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 1nm Y.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     8191 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 1nm Y.loc
--rw-r--r--   0 runner    (1001) docker     (121)     8885 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 1nm Z.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 5nm X.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 5nm X.loc
--rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 5nm Y.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 5nm Y.loc
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1931 5nm Z.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     8955 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 1nm X.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     7724 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 1nm X.loc
--rw-r--r--   0 runner    (1001) docker     (121)     9075 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 1nm Y.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     7722 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 1nm Y.loc
--rw-r--r--   0 runner    (1001) docker     (121)     8736 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 1nm Z.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 5nm X.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 5nm X.loc
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 5nm Y.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 5nm Y.loc
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE 1964 5nm Z.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     8829 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE Illuminant A 1nm.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     8751 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE Illuminant D65 1nm.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     9120 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE S 026 1nm.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE SPF McKinlay UV.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CIE85 Table4 Global AM1_0.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/CRI.std
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/Color 5nm.wvl
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/EqualEnergy.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ISO 9050 Table 1.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ISO 9050 Table 2.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ISO 9050 Table 3.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ISO 9050 Table 4.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ISO 9845 Table 1 Direct AM1_5.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ISO 9845 Table 1 Norm Global AM1_5.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ISO 9845 Table 1 Raw Global AM1_5.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ISO 9845 Table 3 50 Sel Ord AM1_5.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/ISO_9050.std
--rw-r--r--   0 runner    (1001) docker     (121)     2344 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/Moon Solar Source AM2_0.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/NFRC_300_2003.std
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/Optics5.wvl
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/Radiance.std
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/SAE J1796 Table 1.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/SAE J1796 Table 2.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/Sayre UV Source.ssp
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/W5_NFRC_2003.std
--rw-r--r--   0 runner    (1001) docker     (121)     3087 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/W7_G173_37Tilt_Direct.std
--rw-r--r--   0 runner    (1001) docker     (121)     3087 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/W7_G173_37Tilt_Global.std
--rw-r--r--   0 runner    (1001) docker     (121)     3087 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/W7_G197_20Tilt_Direct.std
--rw-r--r--   0 runner    (1001) docker     (121)     3087 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/W7_G197_20Tilt_Global.std
--rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/W7_G197_90Tilt_Direct.std
--rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/W7_G197_90Tilt_Global.std
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/WINDOW4.std
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/mssccprj.scc
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/prEN 410 Table 2 AM1_0.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/prEN 410 Table 5 D65.ssp
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/prEN 410 Table 6 1931 X.dsp
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/prEN 410 Table 6 1931 Y.dsp
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/prEN 410 Table 6 1931 Z.dsp
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/prEN_410.std
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/standards/vssver.scc
--rwxr-xr-x   0 runner    (1001) docker     (121)  6662005 2022-04-11 22:16:32.000000 frads-0.2.3/frads/data/zip_latlon.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    21406 2022-04-11 22:16:32.000000 frads-0.2.3/frads/epjson2rad.py
--rw-r--r--   0 runner    (1001) docker     (121)    12489 2022-04-11 22:16:32.000000 frads-0.2.3/frads/gencolorsky.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6924 2022-04-11 22:16:32.000000 frads-0.2.3/frads/genfmtx.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8605 2022-04-11 22:16:32.000000 frads-0.2.3/frads/genglazing.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6729 2022-04-11 22:16:32.000000 frads-0.2.3/frads/genmtx.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8112 2022-04-11 22:16:32.000000 frads-0.2.3/frads/geombsdf.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18747 2022-04-11 22:16:32.000000 frads-0.2.3/frads/makesky.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12958 2022-04-11 22:16:32.000000 frads-0.2.3/frads/mfacade.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12054 2022-04-11 22:16:32.000000 frads-0.2.3/frads/mrad.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    40583 2022-04-11 22:16:32.000000 frads-0.2.3/frads/mtxmethod.py
--rw-r--r--   0 runner    (1001) docker     (121)    13585 2022-04-11 22:16:32.000000 frads-0.2.3/frads/mtxmult.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14288 2022-04-11 22:16:32.000000 frads-0.2.3/frads/radgeom.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13218 2022-04-11 22:16:32.000000 frads-0.2.3/frads/radmtx.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    24679 2022-04-11 22:16:32.000000 frads-0.2.3/frads/radutil.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7679 2022-04-11 22:16:32.000000 frads-0.2.3/frads/room.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    33781 2022-04-11 22:16:32.000000 frads-0.2.3/frads/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 22:16:42.478768 frads-0.2.3/frads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4946 2022-04-11 22:16:41.000000 frads-0.2.3/frads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4676 2022-04-11 22:16:42.000000 frads-0.2.3/frads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-11 22:16:42.000000 frads-0.2.3/frads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-04-11 22:16:42.000000 frads-0.2.3/frads.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-11 22:16:42.000000 frads-0.2.3/frads.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-11 22:16:42.494768 frads-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-04-11 22:16:32.000000 frads-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 22:16:42.494768 frads-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2573 2022-04-11 22:16:32.000000 frads-0.2.3/test/test_epjson2rad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-04-11 22:16:32.000000 frads-0.2.3/test/test_genfmtx.py
--rw-r--r--   0 runner    (1001) docker     (121)     2455 2022-04-11 22:16:32.000000 frads-0.2.3/test/test_genmtx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-04-11 22:16:32.000000 frads-0.2.3/test/test_getwea.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-04-11 22:16:32.000000 frads-0.2.3/test/test_makesky.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-04-11 22:16:32.000000 frads-0.2.3/test/test_mrad.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.121840 frads-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-27 19:48:40.000000 frads-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8941 2022-10-27 19:48:50.121840 frads-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6196 2022-10-27 19:48:40.000000 frads-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.117840 frads-0.2.8/frads/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4156 2022-10-27 19:48:40.000000 frads-0.2.8/frads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33347 2022-10-27 19:48:40.000000 frads-0.2.8/frads/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6722 2022-10-27 19:48:40.000000 frads-0.2.8/frads/color.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60540 2022-10-27 19:48:40.000000 frads-0.2.8/frads/color_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.117840 frads-0.2.8/frads/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2022-10-27 19:48:40.000000 frads-0.2.8/frads/data/WC.DAT
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-10-27 19:48:40.000000 frads-0.2.8/frads/data/mrad_default.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)    21391 2022-10-27 19:48:40.000000 frads-0.2.8/frads/epjson2rad.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19402 2022-10-27 19:48:40.000000 frads-0.2.8/frads/gencolorsky.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15936 2022-10-27 19:48:40.000000 frads-0.2.8/frads/geom.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12083 2022-10-27 19:48:40.000000 frads-0.2.8/frads/matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    36345 2022-10-27 19:48:40.000000 frads-0.2.8/frads/methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8799 2022-10-27 19:48:40.000000 frads-0.2.8/frads/mtxmult.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    17474 2022-10-27 19:48:40.000000 frads-0.2.8/frads/ncp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18997 2022-10-27 19:48:40.000000 frads-0.2.8/frads/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7098 2022-10-27 19:48:40.000000 frads-0.2.8/frads/raycall.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7473 2022-10-27 19:48:40.000000 frads-0.2.8/frads/room.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15429 2022-10-27 19:48:40.000000 frads-0.2.8/frads/sky.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16402 2022-10-27 19:48:40.000000 frads-0.2.8/frads/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    22593 2022-10-27 19:48:40.000000 frads-0.2.8/frads/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.117840 frads-0.2.8/frads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8941 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 19:48:49.000000 frads-0.2.8/frads.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-27 19:48:40.000000 frads-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-27 19:48:50.125841 frads-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.121840 frads-0.2.8/test/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.121840 frads-0.2.8/test/Resources/
+-rw-r--r--   0 runner    (1001) docker     (121)  1640229 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (121)   449366 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/blinds30.xml
+-rw-r--r--   0 runner    (1001) docker     (121)   846532 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/klems_aniso_high.xml
+-rw-r--r--   0 runner    (1001) docker     (121)   150134 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/oak.wea
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/test.wea
+-rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1820 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_epjson2rad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)      872 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_mtxmult.py
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_ncp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_raycall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_sky.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4841 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_utils.py
```

### Comparing `frads-0.2.3/PKG-INFO` & `frads-0.2.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,15 @@
-Metadata-Version: 2.1
-Name: frads
-Version: 0.2.3
-Summary: UNKNOWN
-Home-page: https://github.com/LBNL-ETA/frads
-Author: LBNL
-Author-email: taoningwang@lbl.gov
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 ![Install + Test](https://github.com/LBNL-ETA/frads/actions/workflows/main.yml/badge.svg)
 ![CodeQL](https://github.com/LBNL-ETA/frads/actions/workflows/codeql-analysis.yml/badge.svg)
 [![Upload Python Package](https://github.com/LBNL-ETA/frads/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LBNL-ETA/frads/actions/workflows/python-publish.yml)
 # _frads_: Framework for Radiance simulation control
 
 This is the repository for _frads_ development. Radiance is a free and open-source, raytracing-based lighting engine that is used extensively by engineering firms for innovative solar control, lighting, and daylighting design to improve the energy efficiency of buildings. With matrix algebraic methods, climate-based annual simulations can now be conducted in less than two minutes. _frads_ automates setup of these simulations by providing end users with an open-source, high-level abstraction of the Radiance command-line workflow (Unix toolbox model), helping to reduce the steep learning curve and associated user errors. _frads_ also provides the necessary infrastructure needed for seamless integration of Radiance and other modeling tools, such as EnergyPlus.
 
-[Documentation](https://frads.readthedocs.io/en/latest/)
+[Documentation](https://lbnl-eta.github.io/frads/)
 
 ## Contact/ Support
 We welcome beta users of _frads_. Feel free to post questions and suggestions in the Discussion section of this GitHub site or contact the principal author at taoningwang@lbl.gov.
 Information about Radiance can be found at: https://www.radiance-online.org .
 The Radiance community is active and welcomes new users via the Radiance Discourse site or Unmet Hours.
 
 ## Testing
@@ -32,37 +17,80 @@
 Integration tests are the main type of test performed for _frads_ commit and releases.  These tests also use the GitHub Action system.
 
 ## Releases
 _frads_ is a work in progress (see to-do list below). _frads_ has been tested on the latest official release of Radiance (September 2020, v5.3) but may not have been tested on the latest HEAD release, which contains source code changes made as recently as yesterday. _frads_ has also been tested on the latest official EnergyPlus release (> v9.3).
 
 ## Installation
 
+Before you can use frads, you need to install it.
+
+### Install Python
+
+Being a Python based library, you'll need to install Python first.
+Python version **3.8** or newer is required for frads.
+
+Get the latest version of Python at https://www.python.org/downloads/ or with your operating system’s package manager.
+
+You can verify that Python is installed by typing python from your cmd/powershell/terminal; you should see something like:
+
+	$ python
+	Python 3.X.X
+	[GCC 4.x] on linux
+	Type "help", "copyright", "credits" or "license" for more information.
+	>>>
+
+### Install Radiance
+
+If you haven't already, you will need to install Radiance. `frads` will check your Radiance
+installation, so make sure you install it first.
+
+To install Radiance, visit Radiance Github [repo](https://github.com/LBNL-ETA/Radiance/releases)
+ to download the latest release for your operating system.
+
+You can verify that Radiance is installed properly by typing in the command-line:
+
+```
+$ rtrace -version
+RADIANCE 5.4a ...
+```
+
+### Install frads
+
+After you have Python installed, you should have `pip` command available in your shell environment as well. You can then use `pip` to install `frads`:
+
+	$ python -m pip install frads
+
+Alternatively, more recent version of `frads` can be installed directly from github as well. Watch for the passing/failed tag on github to check if the current version passed the tests.:
+
+	$ python -m pip install git+https://github.com/LBNL-ETA/frads
+
+### Verifying
+
+To verify that `frads` can be seen by Python, type `python` from your shell. Then at the Python prompt, try to import `frads`
+
+	>>> import frads
+	>>> print(frads.__version__)
+	0.2.7
+
+### Optional external library
+
+`Frads` uses Python standard library for all of its functionalities. However, it will take advantage of [Numpy](https://numpy.org) if you have it installed. It will greatly accelerate the matrix multiplication process, especially for progressive simulation workflow.
+
+The [gencolorsky](other_cli.md#gencolorsky) command line tool in `frads` also relies on [libRadTran](http://www.libradtran.org/) a radiative transfer library for computing the spectrally-resolved radiation data. You'd need to install it first to use [gencolorsky](other_cli.md#gencolorsky).
+
 _frads_ runs from the terminal prompt (command line) on Windows, Mac, and Linux OS. Radiance must be [installed](https://www.radiance-online.org/download-install/radiance-source-code/latest-release) prior to use of _frads_.  You can then install _frads_ by entering the following command in your terminal/cmd/powershell:
 
 ```
 pip install frads
 ```
 
 You can also install _frads_ from this Github repository using this command:
 
 ```
 pip install git+https://github.com/LBNL-ETA/frads.git
 ```
 
-## To do
-- [x] 2-, 3-, 4-, and 5-phase methods implemented (image-based 5-phase works on Windows by aggressive sun-culling, 4-phase to be tested)
-- [x] epJSON to Radiance workflow implemented (not fully tested), window puncher + wall thickener
-- [x] EnergyPlus Radiance runtime interaction preliminarily implemented
-- [ ] Automated window subdivision analysis
-- [ ] Implement daylight metrics calculation with EnergyPlus integration
-- [ ] Implement thermal and visual comfort calculation with EnergyPlus integration
-- [ ] Link to global fenestration systems database and implement BSDF combination routines
-- [ ] Spawn of EnergyPlus integration, variable timestep detailed HVAC and control modeling
-
 ## Reference
 
 Wang, T., "Frads: A Python Library for Radiance Simulation Control", 2021 Radiance workshop, Bilbao, Spain, August 19, 2021, [ppt](https://www.radiance-online.org/community/workshops/2021-bilbao-spain-2/presentations/19_thursday/frads.pdf) , [voice recording](https://www.radiance-online.org/community/workshops/2021-bilbao-spain-2)
 
-Wang, T., Ward, G., and Lee, E.S. (2021), A Python Library for Radiance Matrix-based Simulation Control and EnergyPlus Integration, Proceedings of Building Simulation 2021, International Building Performance Simulation Association, Bruges, September 1-3, 2021. Publication to be posted: [pdf](https://eta.lbl.gov/publications)
-
-
-
+Wang, T., Ward, G., and Lee, E.S. (2021), A Python Library for Radiance Matrix-based Simulation Control and EnergyPlus Integration, Proceedings of Building Simulation 2021, International Building Performance Simulation Association, Bruges, September 1-3, 2021. Publication to be posted: [pdf](https://www.researchgate.net/publication/358969936_A_Python_Library_for_Radiance_Matrix-based_Simulation_Control_and_EnergyPlus_Integration)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `frads-0.2.3/frads/data/WC.DAT` & `frads-0.2.8/frads/data/WC.DAT`

 * *Files identical despite different names*

### Comparing `frads-0.2.3/frads/epjson2rad.py` & `frads-0.2.8/frads/epjson2rad.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,573 +1,561 @@
-"""
-import osn EnergyPlus model as a parsed dictionary
-to Radiance primitives.
-TODO:
-    * Parse window data file for Constradutilction:WindowDataFile
+"""Convert an EnergyPlus epJSON file into Radiance model[s]."""
 
-"""
-import argparse
 from configparser import ConfigParser
-from dataclasses import dataclass
 import json
 import logging
 import os
+from pathlib import Path
 import subprocess as sp
-from typing import Dict, List
+from typing import Any, Mapping, Dict
+from typing import List
 
-from frads import radgeom, radutil, util
-
-logger = logging.getLogger("frads.epjson2rad")
-
-
-@dataclass
-class EPlusWindowGas:
-    name: str
-    thickness: float
-    type: list
-    percentage: list
-    primitive: str = ""
-
-
-@dataclass
-class EPlusOpaqueMaterial:
-    name: str
-    roughness: str
-    solar_absorptance: float
-    visible_absorptance: float
-    visible_reflectance: float
-    primitive: radutil.Primitive
-    thickness: float = 0.0
-
-
-@dataclass
-class EPlusWindowMaterial:
-    name: str
-    visible_transmittance: float
-    primitive: radutil.Primitive
-
-
-@dataclass
-class EPlusConstruction:
-    name: str
-    type: str
-    layers: list
-
-
-@dataclass
-class EPlusOpaqueSurface:
-    name: str
-    type: str
-    polygon: radgeom.Polygon
-    construction: str
-    boundary: str
-    sun_exposed: bool
-    zone: str
-    fenestrations: list
-
-
-@dataclass
-class EPlusFenestration:
-    name: str
-    type: str
-    polygon: radgeom.Polygon
-    construction: EPlusConstruction
-    host: EPlusOpaqueSurface
-
-
-@dataclass
-class EPlusZone:
-    name: str
-    wall: Dict[str, EPlusOpaqueSurface]
-    ceiling: Dict[str, EPlusOpaqueSurface]
-    roof: Dict[str, EPlusOpaqueSurface]
-    floor: Dict[str, EPlusOpaqueSurface]
-    window: Dict[str, EPlusFenestration]
-
-
-def thicken(surface: radgeom.Polygon,
-            windows: List[radgeom.Polygon],
-            thickness: float) -> list:
+from frads import geom
+from frads import utils
+from frads.types import Primitive
+from frads.types import BSDFData
+from frads.types import RadMatrix
+from frads.types import EPlusWindowGas
+from frads.types import EPlusOpaqueMaterial
+from frads.types import EPlusWindowMaterial
+from frads.types import EPlusConstruction
+from frads.types import EPlusOpaqueSurface
+from frads.types import EPlusFenestration
+from frads.types import EPlusZone
+
+logger: logging.Logger = logging.getLogger("frads.epjson2rad")
+
+
+def thicken(
+    surface: geom.Polygon, windows: List[geom.Polygon], thickness: float
+) -> list:
     """Thicken window-wall."""
-    direction = surface.normal().scale(thickness)
+    direction = surface.normal.scale(thickness)
     facade = surface.extrude(direction)[:2]
     for window in windows:
         facade.extend(window.extrude(direction)[2:])
     uniq = facade.copy()
     for idx, val in enumerate(facade):
-        for rep in facade[:idx] + facade[idx + 1:]:
+        for rep in facade[:idx] + facade[idx + 1 :]:
             if set(val.to_list()) == set(rep.to_list()):
                 uniq.remove(rep)
     return uniq
 
 
 def get_construction_thickness(
-        construction: EPlusConstruction, materials: dict) -> float:
+    construction: EPlusConstruction, materials: dict
+) -> float:
     """Get construction total thickness."""
     layer_thickness = []
     for layer in construction.layers:
         layer_thickness.append(materials[layer.lower()].thickness)
     return sum(layer_thickness)
 
 
-def check_outward(polygon: radgeom.Polygon, zone_center: radgeom.Vector) -> bool:
+def check_outward(polygon: geom.Polygon, zone_center: geom.Vector) -> bool:
     """Check whether a surface is facing outside."""
     pi = 3.14159265358579
     outward = True
-    angle2center = polygon.normal().angle_from(
-        zone_center - polygon.centroid())
+    angle2center = polygon.normal.angle_from(zone_center - polygon.centroid)
     if angle2center < pi / 4:
         outward = False
     return outward
 
 
 def eplus_surface2primitive(
-        surfaces: dict, constructions, zone_center, materials) -> dict:
+    surfaces: dict, constructions, zone_center, materials
+) -> dict:
     """Conert EPlusOpaqueSurface (and its windows) to Radiance primitives."""
     surface_primitives: dict = {}
     for _, surface in surfaces.items():
         name = surface.name
         surface_primitives[name] = {}
         surface_primitives[name]["window"] = []
         surface_primitives[name]["xml"] = []
         surface_polygon = surface.polygon
         if not check_outward(surface_polygon, zone_center):
             surface_polygon = surface_polygon.flip()
         window_polygons = []
         for fen in surface.fenestrations:
-            if constructions[fen.construction].type == 'cfs':
+            if constructions[fen.construction].type == "cfs":
                 window_material = "void"
                 surface_primitives[name]["xml"].append(fen.construction + ".xml")
             else:
                 # Get the last construction layer
-                window_material = constructions[
-                    fen.construction].layers[0].replace(" ", "_")
+                window_material = (
+                    constructions[fen.construction].layers[0].replace(" ", "_")
+                )
             window_polygon = fen.polygon
             if check_outward(fen.polygon, zone_center):
                 window_polygon = window_polygon.flip()
             window_polygons.append(window_polygon)
             surface_primitives[name]["window"].append(
-                radutil.polygon2prim(
-                    window_polygon, window_material, fen.name))
+                utils.polygon2prim(window_polygon, window_material, fen.name)
+            )
         surface_primitives[name]["surface"] = []
         surface_construction_layers = constructions[surface.construction].layers
         # Second to the last of construction layers
         inner_material = surface_construction_layers[
-            -min(2, len(surface_construction_layers))].replace(" ", "_")
+            -min(2, len(surface_construction_layers))
+        ].replace(" ", "_")
         surface_primitives[name]["surface"].append(
-            radutil.polygon2prim(surface_polygon, inner_material, surface.name))
+            utils.polygon2prim(surface_polygon, inner_material, surface.name)
+        )
         if surface.sun_exposed:
             outer_material = surface_construction_layers[-1].replace(" ", "_")
             thickness = get_construction_thickness(
-                constructions[surface.construction], materials)
+                constructions[surface.construction], materials
+            )
             facade = thicken(surface_polygon, window_polygons, thickness)
             surface_primitives[name]["surface"].append(
-                radutil.polygon2prim(
-                    facade[1], outer_material, f"ext_{surface.name}"))
+                utils.polygon2prim(facade[1], outer_material, f"ext_{surface.name}")
+            )
             for idx in range(2, len(facade)):
                 surface_primitives[name]["surface"].append(
-                    radutil.polygon2prim(
-                        facade[idx], inner_material, f"sill_{surface.name}.{idx}"))
+                    utils.polygon2prim(
+                        facade[idx], inner_material, f"sill_{surface.name}.{idx}"
+                    )
+                )
     return surface_primitives
 
 
-def write_primitives(surfaces: dict, odir: str):
+def write_primitives(surfaces: dict, odir: str) -> None:
     """Write surface and subsurface primitives."""
     for name, item in surfaces.items():
         opath = os.path.join(odir, name + ".rad")
-        with open(opath, "w") as wtr:
+        with open(opath, "w", encoding="ascii") as wtr:
             for primitive in item["surface"]:
                 wtr.write(str(primitive))
         if item["window"] != []:
             opath = os.path.join(odir, name + "_window.rad")
-            with open(opath, "w") as wtr:
+            with open(opath, "w", encoding="ascii") as wtr:
                 for primitive in item["window"]:
                     wtr.write(str(primitive))
 
 
 def epluszone2rad(zone, constructions, materials):
     """Convert a EPlusZone object to a Radiance model."""
-    zone_center = radgeom.polygon_center(
-        *[wall.polygon for wall in zone.wall.values()])
-    wall = eplus_surface2primitive(
-        zone.wall, constructions, zone_center, materials)
+    zone_center = geom.polygon_center(*[wall.polygon for wall in zone.wall.values()])
+    wall = eplus_surface2primitive(zone.wall, constructions, zone_center, materials)
     ceiling = eplus_surface2primitive(
-        zone.ceiling, constructions, zone_center, materials)
-    roof = eplus_surface2primitive(
-        zone.roof, constructions, zone_center, materials)
-    floor = eplus_surface2primitive(
-        zone.floor, constructions, zone_center, materials)
+        zone.ceiling, constructions, zone_center, materials
+    )
+    roof = eplus_surface2primitive(zone.roof, constructions, zone_center, materials)
+    floor = eplus_surface2primitive(zone.floor, constructions, zone_center, materials)
     return wall, ceiling, roof, floor
 
 
 def parse_material(name: str, material: dict) -> EPlusOpaqueMaterial:
     """Parser EP Material."""
     name = name.replace(" ", "_")
     roughness = material.get("roughness", "Smooth")
     thickness = material.get("thickness", 0.0)
     solar_absorptance = material.get("solar_absorptance", 0.7)
     visible_absorptance = material.get("visible_absorptance", 0.7)
     visible_reflectance = round(1 - visible_absorptance, 2)
-    primitive = radutil.Primitive(
-        "void", "plastic", name, "0",
-        "5 {0} {0} {0} 0 0".format(visible_reflectance))
+    primitive = Primitive(
+        "void",
+        "plastic",
+        name,
+        ["0"],
+        [5, visible_reflectance, visible_reflectance, visible_reflectance, 0, 0],
+    )
     return EPlusOpaqueMaterial(
-        name, roughness, solar_absorptance, visible_absorptance,
-        visible_reflectance, primitive, thickness)
+        name,
+        roughness,
+        solar_absorptance,
+        visible_absorptance,
+        visible_reflectance,
+        primitive,
+        thickness,
+    )
 
 
 def parse_material_nomass(name: str, material: dict) -> EPlusOpaqueMaterial:
     """Parse EP Material:NoMass"""
     name = name.replace(" ", "_")
     roughness = material.get("roughness", "Smooth")
     solar_absorptance = material.get("solar_absorptance", 0.7)
     visible_absorptance = material.get("visible_absorptance", 0.7)
     visible_reflectance = round(1 - visible_absorptance, 2)
-    primitive = radutil.Primitive(
-        "void", "plastic", name, "0",
-        "5 {0} {0} {0} 0 0".format(visible_reflectance))
+    primitive = Primitive(
+        "void",
+        "plastic",
+        name,
+        ["0"],
+        [5, visible_reflectance, visible_reflectance, visible_reflectance, 0, 0],
+    )
     return EPlusOpaqueMaterial(
-        name, roughness, solar_absorptance,
-        visible_absorptance, visible_reflectance, primitive)
+        name,
+        roughness,
+        solar_absorptance,
+        visible_absorptance,
+        visible_reflectance,
+        primitive,
+    )
 
 
 def parse_windowmaterial_gap(name: str, material: dict) -> EPlusWindowGas:
     """Parse EP WindowMaterial:Gap"""
     name = name.replace(" ", "_")
     thickness = material["thickness"]
     gas = material["gas_or_gas_mixture_"]
     return EPlusWindowGas(name, thickness, gas, [1])
 
 
 def parse_windowmaterial_gas(name: str, material: dict) -> EPlusWindowGas:
     """Parse EP WindowMaterial:Gas"""
     name = name.replace(" ", "_")
-    type = [material["gas_type"]]
+    ptype = [material["gas_type"]]
     thickness = material["thickness"]
     percentage = [1]
-    return EPlusWindowGas(name, thickness, type, percentage)
+    return EPlusWindowGas(name, thickness, ptype, percentage)
 
 
-def parse_windowmaterial_gasmixture(
-        name: str, material: dict) -> EPlusWindowGas:
+def parse_windowmaterial_gasmixture(name: str, material: dict) -> EPlusWindowGas:
     """Parse EP WindowMaterial:GasMixture"""
     name = name.replace(" ", "_")
     thickness = material["thickness"]
     gas = [material["Gas"]]
     percentage = [1]
     return EPlusWindowGas(name, thickness, gas, percentage)
 
 
 def parse_windowmaterial_simpleglazingsystem(
-        name: str, material: dict) -> EPlusWindowMaterial:
+    name: str, material: dict
+) -> EPlusWindowMaterial:
     """Parse EP WindowMaterial:SimpleGlazingSystem"""
     identifier = name.replace(" ", "_")
     shgc = material["solar_heat_gain_coefficient"]
     tmit = material.get("visible_transmittance", shgc)
-    tmis = util.tmit2tmis(tmit)
-    primitive = radutil.Primitive(
-        "void", "glass", identifier, "0",
-        "3 {0:.2f} {0:.2f} {0:.2f}".format(tmis))
+    tmis = utils.tmit2tmis(tmit)
+    primitive = Primitive("void", "glass", identifier, ["0"], [3, tmis, tmis, tmis])
     return EPlusWindowMaterial(identifier, tmit, primitive)
 
 
 def parse_windowmaterial_simpleglazing(
-        name: str, material: dict) -> EPlusWindowMaterial:
+    name: str, material: dict
+) -> EPlusWindowMaterial:
     """Parse EP WindowMaterial:Simpleglazing"""
     identifier = name.replace(" ", "_")
-    tmit = material['visible_transmittance']
-    tmis = util.tmit2tmis(tmit)
-    primitive = radutil.Primitive(
-        "void", "glass", identifier, "0",
-        "3 {0:.2f} {0:.2f} {0:.2f}".format(tmis))
+    tmit = material["visible_transmittance"]
+    tmis = utils.tmit2tmis(tmit)
+    primitive = Primitive("void", "glass", identifier, ["0"], [3, tmis, tmis, tmis])
     return EPlusWindowMaterial(identifier, tmit, primitive)
 
 
-def parse_windowmaterial_glazing(
-        name: str, material: dict) -> EPlusWindowMaterial:
+def parse_windowmaterial_glazing(name: str, material: dict) -> EPlusWindowMaterial:
     """Parse EP WindowMaterial:Glazing"""
     identifier = name.replace(" ", "_")
-    if material['optical_data_type'].lower() == 'bsdf':
+    if material["optical_data_type"].lower() == "bsdf":
         tmit = 1
     else:
-        tmit = material['visible_transmittance_at_normal_incidence']
-    tmis = util.tmit2tmis(tmit)
-    primitive = radutil.Primitive('void', 'glass', identifier, '0',
-                                  "3 {0:.2f} {0:.2f} {0:.2f}".format(tmis))
+        tmit = material["visible_transmittance_at_normal_incidence"]
+    tmis = utils.tmit2tmis(tmit)
+    primitive = Primitive("void", "glass", identifier, ["0"], [3, tmis, tmis, tmis])
     return EPlusWindowMaterial(identifier, tmit, primitive)
 
 
 def parse_windowmaterial_blind(inp: dict) -> dict:
     """Parse EP WindowMaterial:Blind"""
     blind_prims = {}
     for key, val in inp.items():
-        _id = key.replace(' ', '_')
+        _id = key.replace(" ", "_")
         # back_beam_vis_refl = val['back_side_slat_beam_visible_reflectance']
         # back_diff_vis_refl = val['back_side_slat_diffuse_visible_reflectance']
         # front_beam_vis_refl = val['front_side_slat_beam_visible_reflectance']
-        front_diff_vis_refl = val['front_side_slat_diffuse_visible_reflectance']
+        front_diff_vis_refl = val["front_side_slat_diffuse_visible_reflectance"]
         # slat_width = val['slat_width']
         # slat_thickness = val['slat_thickness']
         # slat_separation = val['slat_separation']
         # slat_angle = val['slat_angle']
-        blind_prims[key] = radutil.Primitive(
-            'void', 'plastic', _id, '0',
-            '5 {0:.2f} {0:.2f} {0:.2f} 0 0'.format(front_diff_vis_refl))
-        # genblinds_cmd = f"genblinds {_id} {_id} {slat_width} 3 {20*slat_separation} {slat_angle}"
+        blind_prims[key] = Primitive(
+            "void",
+            "plastic",
+            _id,
+            ["0"],
+            [5, front_diff_vis_refl, front_diff_vis_refl, front_diff_vis_refl, 0, 0],
+        )
+        # genblinds_cmd = f"genblinds {_id} {_id} {slat_width} 3
+        # {20*slat_separation} {slat_angle}"
     return blind_prims
 
 
 def parse_epjson_material(epjs: dict) -> dict:
     """Parse each material type."""
     materials = {}
     for key, value in epjs.items():
-        if 'material' in key.split(':')[0].lower():
+        if "material" in key.split(":")[0].lower():
             for name, material in value.items():
                 tocall = globals()[f"parse_{key.replace(':', '_')}".lower()]
                 materials[name.lower()] = tocall(name, material)
     return materials
 
 
 def parse_construction_complexfenestrationstate(epjs):
     """Parser EP Construction:ComplexFenestrationState."""
     construction = epjs.get("Construction:ComplexFenestrationState", {})
     cfs = {}
     matrices = {}
     for key, val in construction.items():
-        val['ctype'] = "cfs"
-        tf_name = val['visible_optical_complex_front_transmittance_matrix_name']
-        tb_name = val['visible_optical_complex_back_transmittance_matrix_name']
-        tf_list = epjs["Matrix:TwoDimension"][tf_name]['values']
-        tb_list = epjs["Matrix:TwoDimension"][tb_name]['values']
-        ncolumn = epjs["Matrix:TwoDimension"][tf_name]['number_of_columns']
+        val["ctype"] = "cfs"
+        tf_name = val["visible_optical_complex_front_transmittance_matrix_name"]
+        tb_name = val["visible_optical_complex_back_transmittance_matrix_name"]
+        tf_list = epjs["Matrix:TwoDimension"][tf_name]["values"]
+        tb_list = epjs["Matrix:TwoDimension"][tb_name]["values"]
+        ncolumn = epjs["Matrix:TwoDimension"][tf_name]["number_of_columns"]
         # if ncolumn < 145:
-            # raise ValueError("BSDF resolution too low to take advantage of Radiance")
-        tf_bsdf = util.nest_list([v['value'] for v in tf_list], ncolumn)
-        tb_bsdf = util.nest_list([v['value'] for v in tb_list], ncolumn)
-        tf = radutil.BSDFData(tf_bsdf).to_sdata()
-        tb = radutil.BSDFData(tb_bsdf).to_sdata()
-        matrices[key] = radutil.RadMatrix(tf, tb)
+        # raise ValueError("BSDF resolution too low to take advantage of Radiance")
+        tf_bsdf = [v["value"] for v in tf_list]
+        tb_bsdf = [v["value"] for v in tb_list]
+        tf = utils.bsdf2sdata(BSDFData(tf_bsdf, ncolumn, ncolumn))
+        tb = utils.bsdf2sdata(BSDFData(tb_bsdf, ncolumn, ncolumn))
+        matrices[key] = RadMatrix(tf, tb)
         cfs[key] = EPlusConstruction(key, "cfs", [])
     return cfs, matrices
 
 
 def parse_construction(construction: dict) -> dict:
     """Parse EP Construction"""
     constructions = {}
     for cname, clayer in construction.items():
-        layers = [layer for layer in clayer.values()]
+        layers = list(clayer.values())
         constructions[cname] = EPlusConstruction(cname, "default", layers)
     return constructions
 
 
 def parse_opaque_surface(surfaces: dict, fenestrations: dict) -> dict:
     """Parse opaque surface to a EPlusOpaqueSurface object."""
     opaque_surfaces = {}
     for name, surface in surfaces.items():
         identifier = name.replace(" ", "_")
         fenes = [fen for fen in fenestrations.values() if fen.host == name]
-        type = surface['surface_type']
-        polygon = radgeom.Polygon(
-            [radgeom.Vector(*vertice.values()) for vertice in surface['vertices']])
+        ptype = surface["surface_type"]
+        polygon = geom.Polygon(
+            [geom.Vector(*vertice.values()) for vertice in surface["vertices"]]
+        )
         for fen in fenes:
             polygon -= fen.polygon
-        construction = surface['construction_name']
-        boundary = surface['outside_boundary_condition']
-        sun_exposed = surface['sun_exposure'] == 'SunExposed'
-        zone = surface['zone_name']
+        construction = surface["construction_name"]
+        boundary = surface["outside_boundary_condition"]
+        sun_exposed = surface["sun_exposure"] == "SunExposed"
+        zone = surface["zone_name"]
         opaque_surfaces[name] = EPlusOpaqueSurface(
-            identifier, type, polygon, construction,
-            boundary, sun_exposed, zone, fenes)
+            identifier, ptype, polygon, construction, boundary, sun_exposed, zone, fenes
+        )
     return opaque_surfaces
 
 
 def parse_epjson_fenestration(fenes: dict) -> Dict[str, EPlusFenestration]:
     """Parse fenestration dictionary to a EPlusFenestration object."""
     fenestrations = {}
     for name, fen in fenes.items():
-        surface_type = fen['surface_type']
+        surface_type = fen["surface_type"]
         if surface_type != "Door":
             name = name.replace(" ", "_")
-            host = fen['building_surface_name']
+            host = fen["building_surface_name"]
             vertices = []
-            for i in range(1, fen['number_of_vertices'] + 1):
+            for i in range(1, fen["number_of_vertices"] + 1):
                 vertices.append(
-                    radgeom.Vector(
+                    geom.Vector(
                         fen[f"vertex_{i}_x_coordinate"],
                         fen[f"vertex_{i}_y_coordinate"],
                         fen[f"vertex_{i}_z_coordinate"],
                     )
                 )
-            polygon = radgeom.Polygon(vertices)
-            construction = fen['construction_name']
+            polygon = geom.Polygon(vertices)
+            construction = fen["construction_name"]
             fenestrations[name] = EPlusFenestration(
-                name, surface_type, polygon, construction, host)
+                name, surface_type, polygon, construction, host
+            )
     return fenestrations
 
 
 def parse_epjson(epjs: dict) -> tuple:
     """
     Convert EnergyPlus JSON objects into Radiance primitives.
     """
     # get site information
-    site = list(epjs['Site:Location'].values())[0]
+    site = list(epjs["Site:Location"].values())[0]
 
     # parse each fenestration
     fenestrations = parse_epjson_fenestration(epjs["FenestrationSurface:Detailed"])
 
     # Get all the fenestration hosting surfaces
-    fene_hosts = set([val.host for val in fenestrations.values()])
+    fene_hosts = {val.host for val in fenestrations.values()}
 
     # parse each opaque surface
     opaque_surfaces = parse_opaque_surface(
-        epjs["BuildingSurface:Detailed"], fenestrations)
+        epjs["BuildingSurface:Detailed"], fenestrations
+    )
 
     # parse each construction
-    constructions = parse_construction(epjs['Construction'])
+    constructions = parse_construction(epjs["Construction"])
 
     cfs, matrices = parse_construction_complexfenestrationstate(epjs)
     constructions.update(cfs)
 
     # parse materials
     materials = parse_epjson_material(epjs)
 
     # get exterior zones
-    exterior_zones = [value.zone for key, value in opaque_surfaces.items()
-                      if (key in fene_hosts) and value.sun_exposed]
+    exterior_zones = [
+        value.zone
+        for key, value in opaque_surfaces.items()
+        if (key in fene_hosts) and value.sun_exposed
+    ]
 
     # get secondary zones, but we don't do anything with it yet.
     secondary_zones: dict = {}
     for key, value in opaque_surfaces.items():
         if (key in fene_hosts) and (value.zone not in exterior_zones):
             adjacent_zone = opaque_surfaces[value.boundary].zone
             if adjacent_zone in exterior_zones:
                 secondary_zones[value.zone] = {}
 
     zones = {}
     # go through each exterior zone, update zone dictionary.
     for zname in exterior_zones:
         zone_name = zname.replace(" ", "_")
         surface_map: dict = {"Wall": {}, "Ceiling": {}, "Roof": {}, "Floor": {}}
-        windows = {n: val for n, val in fenestrations.items()
-                   if opaque_surfaces[val.host].zone == zname}
+        windows = {
+            n: val
+            for n, val in fenestrations.items()
+            if opaque_surfaces[val.host].zone == zname
+        }
         for name, surface in opaque_surfaces.items():
             if surface.zone == zname:
                 surface_map[surface.type][name] = surface
         zones[zname] = EPlusZone(zone_name, *surface_map.values(), windows)
     return site, zones, constructions, materials, matrices
 
 
-def write_config(config):
+def write_config(config: Mapping[str, Mapping[str, Any]]) -> None:
+    """Write config."""
     cfg = ConfigParser(allow_no_value=True)
-    templ_config = config.to_dict()
-    cfg.read_dict(templ_config)
-    with open(f"{config.name}.cfg", "w") as rdr:
+    # templ_config = config.to_dict()
+    cfg.read_dict(config)
+    with open(f"{config.name}.cfg", "w", encoding="utf-8") as rdr:
         cfg.write(rdr)
 
 
-def epjson2rad(epjs: dict) -> dict:
+def epjson2rad(epjs: dict) -> None:
     """Command-line program to convert a energyplus model into a Radiance model."""
     # Setup file structure
-    util.mkdir_p("Objects")
-    util.mkdir_p("Resources")
-    util.mkdir_p("Matrices")
+    Path("Objects").mkdir(exist_ok=True)
+    Path("Resources").mkdir(exist_ok=True)
+    Path("Matrices").mkdir(exist_ok=True)
 
     site, zones, constructions, materials, matrices = parse_epjson(epjs)
     building_name = epjs["Building"].popitem()[0].replace(" ", "_")
 
     # Write material file
-    material_name = f"materials{building_name}.mat"
-    with open(os.path.join("Objects", material_name), 'w') as wtr:
+    material_path = os.path.join("Objects", f"materials{building_name}.mat")
+    with open(material_path, "w", encoding="ascii") as wtr:
         for material in materials.values():
             wtr.write(str(material.primitive))
 
     # Write matrix files to xml, if any
     xml_paths = {}
     for key, val in matrices.items():
-        opath = os.path.join('Resources', key + '.xml')
-        tf_path = os.path.join('Resources', key + '_tf.mtx')
-        tb_path = os.path.join('Resources', key + '_tb.mtx')
-        with open(tf_path, 'w') as wtr:
+        opath = os.path.join("Resources", key + ".xml")
+        tf_path = os.path.join("Resources", key + "_tf.mtx")
+        tb_path = os.path.join("Resources", key + "_tb.mtx")
+        with open(tf_path, "w", encoding="ascii") as wtr:
             wtr.write(repr(val.tf))
-        with open(tb_path, 'w') as wtr:
+        with open(tb_path, "w", encoding="ascii") as wtr:
             wtr.write(repr(val.tb))
-        basis = ''.join([word[0] for word in val.tf.basis.split()])
-        cmd = ['wrapBSDF', '-f', 'n=' + key, '-a', basis]
-        cmd += ['-tf', tf_path, '-tb', tb_path, '-U']
+        # basis = ''.join([word[0] for word in val.tf.basis.split()])
+        basis = "".join(
+            [word[0].lower() for word in utils.BASIS_DICT[str(val.tf.ncolumn)].split()]
+        )
+        cmd = ["wrapBSDF", "-f", "n=" + key, "-a", basis]
+        cmd += ["-tf", tf_path, "-tb", tb_path, "-U"]
         wb_process = sp.run(cmd, check=True, stdout=sp.PIPE, stderr=sp.PIPE)
-        with open(opath, 'wb') as wtr:
+        with open(opath, "wb") as wtr:
             wtr.write(wb_process.stdout)
         xml_paths[key] = opath
 
-    zone_config = {}
     # For each zone write primitves to files and create a config file
     for name, zone in zones.items():
-        mrad_config = util.MradConfig(
-            latitude=site["latitude"],
-            longitude=site["longitude"],
-            material=material_name,
-        )
+        mrad_config = ConfigParser(allow_no_value=False)
+        mrad_config["SimControl"] = {
+            "vmx_basis": "kf",
+            "vmx_opt": "-ab 5 -ad 65536 -lw 1e-5",
+            "fmx_basis": "kf",
+            "smx_basis": "r4",
+            "dmx_opt": "-ab 2 -ad 128 -c 5000",
+            "dsmx_opt": "-ab 7 -ad 16384 -lw 5e-5",
+            "cdsmx_opt": "-ab 1",
+            "cdsmx_basis": "r6",
+            "ray_count": "1",
+            "nprocess": "1",
+            "separate_direct": "False",
+            "overwrite": "False",
+            "method": "",
+        }
+        mrad_config["Site"] = {
+            "wea_path": "",
+            "zipcode": "",
+            "latitude": site["latitude"],
+            "longitude": site["longitude"],
+            "start_hour": "",
+            "end_hour": "",
+            "daylight_hours_only": "True",
+        }
         primitives = epluszone2rad(zone, constructions, materials)
         scene = []
         windows = []
         window_xmls = []
-        window_controls = []
         floors = []
         for primitive in primitives:
             write_primitives(primitive, "Objects")
             for _name, item in primitive.items():
                 if item["surface"] != []:
-                    scene.append(_name + ".rad")
+                    scene.append(os.path.join("Objects", _name + ".rad"))
                 if item["window"] != []:
-                    windows.append(_name + "_window.rad")
+                    windows.append(os.path.join("Objects", _name + "_window.rad"))
                 if item["xml"] != []:
-                    window_xmls.extend(item['xml'])
-                    window_controls.append("0")
+                    window_xmls.extend(
+                        [os.path.join("Resources", xml) for xml in item["xml"]]
+                    )
         # Get floors
         for primitive in primitives[-1]:
-            floors.append(primitive + ".rad")
+            floors.append(os.path.join("Objects", primitive + ".rad"))
 
-        mrad_config.scene = " ".join(scene)
-        mrad_config.window_paths = " ".join(windows)
-        mrad_config.window_xml = " ".join(window_xmls)
-        mrad_config.window_control = " ".join(window_controls)
-        mrad_config.grid_surface = " ".join(floors)
-        mrad_config.name = name
-        mrad_config.__post_init__()
-        zone_config[name] = mrad_config
-    return zone_config
+        mrad_config["Model"] = {
+            "material": material_path,
+            "scene": "\n".join(scene),
+            "window_paths": " ".join(windows),
+            "window_xml": " ".join(window_xmls),
+            "ncp_shade": "",
+        }
+        mrad_config["RaySender"] = {
+            "grid_surface": " ".join(floors),
+            "grid_spacing": "1",
+            "grid_height": "0.75",
+        }
+        with open(f"{name.replace(' ', '_')}.cfg", "w", encoding="utf-8") as wtr:
+            mrad_config.write(wtr)
 
 
-def read_ep_input(fpath: str) -> dict:
+def read_ep_input(fpath: Path) -> dict:
     """Load and parse input file into a JSON object.
     If the input file is in .idf fomart, use command-line
     energyplus program to convert it to epJSON format
     Args:
         fpath: input file path
     Returns:
         epjs: JSON object as a Python dictionary
     """
-    epjson_path: str = ''
-    if fpath.endswith('.idf'):
-        cmd = ['energyplus', '--convert-only', fpath]
-        sp.run(cmd, check=True, stderr=sp.PIPE, stdout=sp.PIPE)
-        epjson_path = os.path.splitext(os.path.basename(fpath))[0] + '.epJSON'
-        if not os.path.isfile(epjson_path):
-            raise OSError("idf to epjson conversion failed")
-    elif fpath.endswith('.epJSON'):
+    epjson_path: Path
+    if fpath.suffix == ".idf":
+        cmd = ["energyplus", "--convert-only", str(fpath)]
+        sp.run(cmd, check=True)
+        epjson_path = Path(fpath.with_suffix(".epJSON").name)
+        if not epjson_path.is_file():
+            raise FileNotFoundError(f"Converted {str(epjson_path)} not found.")
+    elif fpath.suffix == ".epJSON":
         epjson_path = fpath
     with open(epjson_path) as rdr:
         epjs = json.load(rdr)
     return epjs
-
-
-def epjson2rad_cmd():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('fpath')
-    parser.add_argument('-run', action='store_true', default=False)
-    args = parser.parse_args()
-    epjs = read_ep_input(args.fpath)
-    if "FenestrationSurface:Detailed" not in epjs:
-        raise ValueError("No windows found in this model")
-    configs = epjson2rad(epjs)
-    for config in configs.values():
-        write_config(config)
```

### Comparing `frads-0.2.3/frads/gencolorsky.py` & `frads-0.2.8/frads/matrix.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,329 +1,367 @@
-"""Call uvspec to generate spectrally resolved sky description."""
-import argparse
-from datetime import datetime, timedelta
+"""
+This module contains routines to generate sender and receiver objects, generate
+matrices by calling either rfluxmtx or rcontrib.
+"""
+
+from __future__ import annotations
 import logging
-import math
 import os
+from pathlib import Path
 import subprocess as sp
-import tempfile
-from frads import makesky, util, radutil
+import tempfile as tf
+from typing import Iterable
+from typing import List
+from typing import Optional
+from typing import Sequence
+from typing import Union
+
+from frads import sky
+from frads import geom
+from frads import parsers
+from frads import raycall
+from frads import utils
+from frads.types import Primitive
+from frads.types import Receiver
+from frads.types import Sender
+from frads.geom import Vector
+
 
+logger: logging.Logger = logging.getLogger("frads.matrix")
 
-def get_local_input(dt: str, latitude: float, longitude: float,
-                    altitude: float, zenith: float,
-                    azimuth: float) -> str:
-    """Get geographical and solar geometry input to uvspec.
-    args:
-        dt: datetime string
-        latitude: in deg
-        longitude: in deg
-        altitude: in km
-        zenith: solar zenith angle (deg)
-        azimuth: solar azimuth (deg) (0deg -> south)
-        doy: day of year
-    return
-        uvspec input string
+
+def surface_as_sender(prim_list: list, basis: str, offset=None, left=None) -> Sender:
     """
-    if longitude > 0:
-        longitude_str = f"W {longitude:.2f}"
-    else:
-        longitude_str = f"E {abs(longitude):.2f}"
-    if latitude > 0:
-        latitude_str = f"N {latitude:.2f}"
+    Construct a sender from a surface.
+
+    Args:
+        prim_list(list): a list of primitives
+        basis(str): sender sampling basis
+        offset(float): move the sender surface in its normal direction
+        left(bool): Use left-hand rule instead for matrix generation
+
+    Returns:
+        A sender object (Sender)
+
+    """
+    prim_str = prepare_surface(
+        prims=prim_list, basis=basis, offset=offset, left=left, source=None, out=None
+    )
+    logger.debug("Surface sender:\n%s", prim_str)
+    return Sender("s", prim_str.encode(), None, None)
+
+
+def view_as_sender(view: View, ray_cnt: int, xres: int, yres: int) -> Sender:
+    """
+    Construct a sender from a view.
+
+    Args:
+        view: a view object;
+        ray_cnt: ray count;
+        xres, yres: image resolution
+        c2c: Set to True to trim the fisheye corner rays.
+
+    Returns:
+        A sender object
+
+    """
+    if (xres is None) or (yres is None):
+        raise ValueError("Need to specify resolution")
+    res_cmd = [
+        "vwrays",
+        *view.args(),
+        "-x",
+        str(xres),
+        "-y",
+        str(yres),
+        "-d",
+    ]
+    logger.info("Check real image resolution: \n%s", " ".join(res_cmd))
+    res_proc = sp.run(res_cmd, check=True, stdout=sp.PIPE, encoding="ascii")
+    res_eval = res_proc.stdout.split()
+    new_xres, new_yres = int(res_eval[1]), int(res_eval[3])
+    if (new_xres != xres) and (new_yres != yres):
+        logger.info("Changed resolution to %s %s", new_xres, new_yres)
+    vwrays_cmd = ["vwrays", "-ff", "-x", str(new_xres), "-y", str(new_yres)]
+    if ray_cnt > 1:
+        vwrays_cmd.extend(["-c", str(ray_cnt), "-pj", "0.7"])
+    logger.debug("Ray count is %s", ray_cnt)
+    vwrays_cmd += view.args()
+    logger.info("Generate view rays with: \n%s", " ".join(vwrays_cmd))
+    vwrays_proc = sp.run(vwrays_cmd, check=True, stdout=sp.PIPE)
+    if view.vtype == "a":
+        flush_cmd = utils.get_flush_corner_rays_command(ray_cnt, xres)
+        logger.info("Flushing -vta corner rays: \n%s", " ".join(flush_cmd))
+        flush_proc = sp.run(
+            flush_cmd, check=True, input=vwrays_proc.stdout, stdout=sp.PIPE
+        )
+        vrays = flush_proc.stdout
     else:
-        latitude_str = f"S {abs(latitude):.2f}"
-    inp = f"latitude {latitude_str}\n"
-    inp += f"longitude {longitude_str}\n"
-    inp += f"time {dt}\n"
-    inp += f"altitude {altitude}\n"
-    inp += "albedo 0.2\n"
-    inp += f"sza {zenith}\n"
-    inp += f"phi0 {azimuth}\n"
-    return inp
-
-
-def get_output_input(umu: list, phis: list,
-                     output=None, silent=True, verbose=False) -> str:
-    """Get sampling angles and output format input for uvspec.
-    args:
-        umu:
-        phis:
-        output:
-        silent:
-    return:
-        uvspec input string
-    """
-    if output is None:
-        output = "lambda edir edn uu"
-    inp = ""
-    if umu is not None:
-        inp += f"umu {' '.join(map(str, umu))}\n"
-    if phis is not None:
-        inp += f"phi {' '.join(map(str, phis))}\n"
-    inp += f"output_user {output}\n"
-    if silent:
-        inp += "quiet\n"
-    if verbose:
-        inp += "verbose\n"
-    return inp
-
-
-def get_uniform_samples(step: int) -> tuple:
-    """Get uniform sky sampling angles.
-    args:
-        step: uniform sampling spacing (deg), need to be divisive by 90.
-    return:
-        cos(theta)
-        phi angles
-    """
-    if 90 % step != 0:
-        raise Exception("Angluar resolution not divisive by 90")
-    thetas = range(0, 90, step)
-    cos_thetas = [-math.cos(math.radians(i)) for i in thetas]
-    phis = list(range(0, 361, step))
-    return cos_thetas, phis
-
-
-def get_solar(year: str, month: str, day: str, hours: str,
-              lat: str, lon: str, tzone: str):
-    """Call gendaylit to get solar angles."""
-    cmd = makesky.gendaylit_cmd(month, day, hours, lat, lon, tzone, year=year)
-    gdl_proc = sp.run(list(map(str, cmd)), check=True,
-                      stdout=sp.PIPE, stderr=sp.PIPE)
-    gdl_prims = radutil.parse_primitive(gdl_proc.stdout.decode().splitlines())
-    source_prim = [prim for prim in gdl_prims if prim.ptype == "source"][0]
-    source_dir = list(map(float, source_prim.real_arg.split()[1:4]))
-    zenith_angle = math.degrees(math.acos(source_dir[2]))
-    azimuth_angle = math.degrees(math.atan2(-source_dir[0], -source_dir[1])) % 360
-    return source_prim, source_dir, zenith_angle, azimuth_angle
-
-
-def gen_rad_template() -> str:
-    """Generate sky.rad file template.
-    This function generates a static string for now.
-    """
-    sky_template = "void colordata skyfunc\n"
-    sky_template += "9 noop noop noop red.dat green.dat blue.dat . "
-    sky_template += '"Acos(Dz)/DEGREE" "mod(atan2(-Dx, -Dy)/DEGREE,360)"\n'
-    sky_template += "0\n0\n\n"
-    sky_template += "skyfunc glow skyglow 0 0 4 1 1 1 0\n"
-    sky_template += "skyglow source skydome 0 0 4 0 0 1 180\n"
-    return sky_template
-
-
-def gen_header(anglestep: int) -> str:
-    """Generate header for colordata data files."""
-    theta_interval = 90 / anglestep
-    phi_interval = 360 / anglestep + 1
-    header = "# Theta and phi dimensions\n2\n0 90 "
-    header += f"{theta_interval:.0f}\n0 360 {phi_interval:.0f}\n"
-    return header
-
-
-def get_logger(verbosity: int):
-    """Setup logger.
-    args:
-        verbosity: verbosity levels 0-5
-    returns:
-        logger object
-    """
-    logger = logging.getLogger("frads.gencolorsky")
-    formatter = logging.Formatter(
-        "%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-    console_handler = logging.StreamHandler()
-    _level = verbosity * 10
-    logger.setLevel(_level)
-    console_handler.setLevel(_level)
-    console_handler.setFormatter(formatter)
-    logger.addHandler(console_handler)
-    return logger
-
-
-def parse_cli_args():
-    """Parse commandline interface arguments."""
-    parser = argparse.ArgumentParser()
-    parser.add_argument("year", type=int)
-    parser.add_argument("month", type=int)
-    parser.add_argument("day", type=int)
-    parser.add_argument("hour", type=int)
-    parser.add_argument("minute", type=int)
-    parser.add_argument("-a", "--latitude", type=float, required=True)
-    parser.add_argument("-o", "--longitude", type=float, required=True)
-    parser.add_argument("-m", "--tzone", type=int, required=True)
-    parser.add_argument("-e", "--atm")
-    parser.add_argument("-s", "--observer", choices=["2", "10"], default="2")
-    parser.add_argument("-c", "--colorspace", default="radiance")
-    parser.add_argument("-b", "--cloudcover", type=float)
-    parser.add_argument("-t", "--total", action="store_true")
-    parser.add_argument("-g", "--cloudprofile", type=int)
-    parser.add_argument("-r", "--anglestep", type=int, default=3)
-    parser.add_argument("-u", "--altitude", default=0)
-    parser.add_argument("-d", "--aod", type=float)
-    parser.add_argument("-l", "--aerosol",
-                        choices=["continental_clean",
-                                 "continental_average",
-                                 "continental_polluted",
-                                 "urban",
-                                 "maritime_clean",
-                                 "maritime_polluted",
-                                 "maritime_tropical",
-                                 "desert",
-                                 "antarctic"])
-    parser.add_argument("-i", "--pmt", action="store_true")
-    parser.add_argument(
-        "-v", "--verbose", action="count", default=0,
-        help="Verbose mode: \n"
-        "\t-v=Debug\n"
-        "\t-vv=Info\n"
-        "\t-vvv=Warning\n"
-        "\t-vvvv=Error\n"
-        "\t-vvvvv=Critical\n"
-        "default=Warning")
-    args = parser.parse_args()
-    return args
-
-
-def main():
-    """gencolorsky entry point."""
-    # Solar disk solid angle
-    solar_sa = 6.7967e-5
-    start_wvl = 360
-    end_wvl = 800
-    wvl_step = 10
-    direct_sun = True
-    try:
-        lib_path = os.environ["LIBRADTRAN_DATA_FILES"]
-    except KeyError as ke:
-        raise KeyError("Can't find LIBRADTRAN_DATA_FILES in environment")
-    args = parse_cli_args()
-    logger = get_logger(args.verbose)
-    verbose = True if args.verbose < 3 else False
-    hours = args.hour + args.minute / 60.0
-    wavelengths = range(start_wvl, end_wvl + 1, wvl_step)
-    dt = datetime(args.year, args.month, args.day, args.hour, args.minute)
-    dt_str = (dt + timedelta(hours=int(args.tzone / (-15)))).strftime(
-        "%Y %m %d %H %M %S")
-    ct, phis = get_uniform_samples(args.anglestep)
-    source_prim, source_dir, zenith_angle, azimuth_angle = get_solar(
-        args.year, args.month, args.day, hours,
-        args.latitude, args.longitude, args.tzone)
-    # Generate input to uvspec
-    model = f"data_files_path {lib_path}\n"
-    model += f"source solar {lib_path}solar_flux/apm_1nm\n"
-    model += "pseudospherical\n"
-    model += "aerosol_default\n"
-    model += get_local_input(dt_str, args.latitude, args.longitude,
-                             args.altitude, zenith_angle, azimuth_angle)
-    if args.atm:
-        model += f"atmosphere_file {atm_file}\n"
-    if args.cloudcover:
-        if args.cloudprofile:
-            wc_path = args.cloudprofile
+        vrays = vwrays_proc.stdout
+    logger.debug("View sender:\n%s", vrays)
+    return Sender("v", vrays, xres, yres)
+
+
+def points_as_sender(pts_list: list, ray_cnt: Optional[int] = None) -> Sender:
+    """
+    Construct a sender from a list of points.
+
+    Args:
+        pts_list(list): a list of list of float
+        ray_cnt(int): sender ray count
+
+    Returns:
+        A sender object
+    """
+    ray_cnt = 1 if ray_cnt is None else ray_cnt
+    if pts_list is None:
+        raise ValueError("pts_list is None")
+    if not all(isinstance(item, list) for item in pts_list):
+        raise ValueError("All grid points has to be lists.")
+    pts_list = [i for i in pts_list for _ in range(ray_cnt)]
+    grid_str = os.linesep.join([" ".join(map(str, li)) for li in pts_list]) + os.linesep
+    logger.debug("Point sender:\n%s", grid_str)
+    return Sender("p", grid_str.encode(), None, len(pts_list))
+
+
+def sun_as_receiver(
+    basis,
+    smx_path: Path,
+    window_normals: Optional[List[Vector]],
+    full_mod: bool = False,
+) -> Receiver:
+    """
+    Instantiate a sun receiver object.
+
+    Args:
+        basis: receiver sampling basis {kf | r1 | sc25...}
+        smx_path: sky/sun matrix file path
+        window_paths: window file paths
+    Returns:
+        A sun receiver object
+    """
+
+    # gensun = sky.Gensun(int(basis[-1]))
+    if (smx_path is None) and (window_normals is None):
+        str_repr, mod_str = sky.gen_sun_source_full(int(basis[-1]))
+        return Receiver(str_repr, basis, modifier=mod_str)
+    str_repr, mod_str, mod_str_full = sky.gen_sun_source_culled(
+        int(basis[-1]), smx_path=smx_path, window_normals=window_normals
+    )
+    if full_mod:
+        return Receiver(receiver=str_repr, basis=basis, modifier=mod_str_full)
+    logger.debug("Sun receiver:\n%s", str_repr)
+    logger.debug("Sun modifier:\n%s", mod_str)
+    return Receiver(receiver=str_repr, basis=basis, modifier=mod_str)
+
+
+def sky_as_receiver(basis: str, out) -> Receiver:
+    """
+    Instantiate a sky receiver object.
+
+    Args:
+        basis: receiver sampling basis {kf | r1 | sc25...}
+    Returns:
+        A sky receiver object
+    """
+
+    if not basis.startswith("r"):
+        raise ValueError(f"Sky basis need to be Treganza/Reinhart, found {basis}")
+    out.parent.mkdir(exist_ok=True)
+    sky_str = f'#@rfluxmtx o="{str(out)}"\n'
+    sky_str += sky.basis_glow(basis)
+    logger.debug("Sky receiver:\n%s", sky_str)
+    return Receiver(sky_str, basis)
+
+
+def surface_as_receiver(
+    prim_list: Sequence[Primitive],
+    basis: str,
+    out: Union[None, str, Path],
+    offset=None,
+    left: bool = False,
+    source: str = "glow",
+) -> Receiver:
+    """
+    Instantiate a surface receiver object.
+
+    Args:
+        prim_list: list of primitives(dict)
+        basis: receiver sampling basis {kf | r1 | sc25...}
+        out: output path
+        offset: offset the surface in its normal direction
+        left: use instead left-hand rule for matrix generation
+        source: light source for receiver object {glow|light}
+    Returns:
+        A surface receiver object
+    """
+    rcvr_str = prepare_surface(
+        prims=prim_list, basis=basis, offset=offset, left=left, source=source, out=out
+    )
+    logger.debug("Surface receiver:\n%s", rcvr_str)
+    return Receiver(rcvr_str, basis)
+
+
+def prepare_surface(*, prims, basis, left, offset, source, out) -> str:
+    """
+    Prepare the sender or receiver surface, adding appropriate tags.
+
+    Args:
+        prims(list): list of primitives
+        basis(str): sampling basis
+        left(bool): use instead the left-hand rule
+        offset(float): offset surface in its normal direction
+        source(str): surface light source for receiver
+        out: output path
+    Returns:
+        The surface sender/receiver primitive as string
+    """
+
+    if basis is None:
+        raise ValueError("Sampling basis cannot be None")
+    if (source is not None) and (source not in ("glow", "light")):
+        raise ValueError(f"Unknown source type {source}")
+    upvector = utils.up_vector(prims)
+    upvector = upvector.scale(-1) if left else upvector
+    upvector_str = str(upvector).replace(" ", ",")
+    modifier_set = {p.modifier for p in prims}
+    if len(modifier_set) != 1:
+        logger.warning("Primitives don't share modifier")
+    src_mod = f"rflx{prims[0].modifier}{utils.id_generator()}"
+    header = f"#@rfluxmtx h={basis} u={upvector_str}\n"
+    if out is not None:
+        header += f'#@rfluxmtx o="{out}"\n\n'
+    if source == "glow":
+        source_prim = Primitive("void", source, src_mod, ("0"), (4, 1, 1, 1, 0))
+        header += str(source_prim)
+    elif source == "light":
+        source_prim = Primitive("void", source, src_mod, ("0"), (3, 1, 1, 1))
+        header += str(source_prim)
+    modifiers = [p.modifier for p in prims]
+    content = ""
+    for prim in prims:
+        if prim.identifier in modifiers:
+            _identifier = "discarded"
         else:
-            _file_path_ = os.path.dirname(__file__)
-            wc_path = os.path.join(_file_path_, 'data', "WC.DAT")
-        model += f"wc_file 1D {wc_path}\n"
-        model += f"cloudcover wc {args.cloudcover}\n"
-        model += "interpret_as_level wc\n"  # use independent pixel approximation
-        if args.cloudcover == 1:
-            direct_sun = False
-    if args.aerosol:
-        model += f"aerosol_species_file {args.aerosol}\n"
-    if args.aod:
-        model += f"aerosol_modify tau set {args.aod}\n"
-    if args.total:
-        inp = model
-        inp += "mol_abs_param kato2\n"
-        inp += get_output_input(None, None, output="edir edn", verbose=verbose)
-        inp += "output_process sum\n"
-        logger.info(inp)
-        proc = sp.run("uvspec", input=inp.encode(), stderr=sp.PIPE, stdout=sp.PIPE)
-        direct_hor, diff_hor = list(map(float, proc.stdout.decode().strip().split()))
-        direct_normal = direct_hor / source_dir[2]
-        print(f"DNI: {direct_normal:.2f} W/m2")
-        print(f"DHI: {diff_hor:.2f} W/m2")
-        print(f"GHI: {direct_hor + diff_hor:.2f} W/m2")
-        exit()
-    elif not direct_sun:
-        model += get_output_input(ct, phis, output="lambda uu")
-    else:
-        model += get_output_input(ct, phis)
-    result = []
-    for wvl in wavelengths:
-        inp = model
-        inp += f"wavelength {wvl}\n"
-        logger.info(inp)
-        proc = sp.run("uvspec", input=inp.encode(), stdout=sp.PIPE)
-        result.append(proc.stdout.decode().strip().split())
-    wvl_range = end_wvl - start_wvl + wvl_step
-    wavelengths = list(wavelengths)
-    wvl_length = len(wavelengths)
-    trix, triy, triz, mlnp = util.load_cie_tristi(wavelengths, args.observer)
-    columns = [col for col in zip(*result)]
-    # Carry out additional full solar spectra run if pmt requested
-    if args.pmt:
-        inp = model
-        inp += "mol_abs_param kato2\n"
-        inp += get_output_input(ct, phis, output="lambda edir edn uu", verbose=verbose)
-        inp += "output_process sum\n"
-        logger.info(inp)
-        proc = sp.run("uvspec", input=inp.encode(), stderr=sp.PIPE, stdout=sp.PIPE)
-        blue = [i / 1e3 for i in map(float, proc.stdout.decode().strip().split())]
-        pfact = util.LEMAX * wvl_range / wvl_length / 1e3
-        mfact = util.MLEMAX * wvl_range / wvl_length / 1e3
-        red = []
-        green = []
-        for col in columns[1:]:
-            col = list(map(float, col))
-            cieys = [i * j for i, j in zip(col, triy)]
-            edis = [i * j for i,j in zip(col, mlnp)]
-            cie_y = pfact * sum(cieys)
-            edi = mfact * sum(edis)
-            red.append(cie_y)
-            green.append(edi)
-    else:
-        coeffs = util.get_conversion_matrix(args.colorspace)
-        pfact = util.LEMAX * wvl_range / wvl_length / 1e3 / 179
-        # Get RGB for each sampled point from sky
-        red = []
-        green = []
-        blue = []
-        for col in columns[1:]:
-            col = list(map(float, col))
-            ciexs = [i * j for i, j in zip(col, trix)]
-            cieys = [i * j for i, j in zip(col, triy)]
-            ciezs = [i * j for i, j in zip(col, triz)]
-            cie_x = pfact * sum(ciexs)
-            cie_y = pfact * sum(cieys)
-            cie_z = pfact * sum(ciezs)
-            _r, _g, _b = util.xyz2rgb(cie_x, cie_y, cie_z, coeffs)
-            red.append(_r)
-            green.append(_g)
-            blue.append(_b)
-
-    out_dir = f"cs_{args.month:02d}{args.day:02d}{args.hour:02d}"
-    out_dir += f"{args.minute:02d}_{args.latitude}_{args.longitude}"
-    util.mkdir_p(out_dir)
-    if direct_sun:
-        sidx = 2
-    else:
-        sidx = 0
-    header = gen_header(args.anglestep)
-    with open(os.path.join(out_dir, "red.dat"), "w") as wtr:
-        wtr.write(header)
-        wtr.write("\n".join([str(value) for value in red[sidx:]]))
-    with open(os.path.join(out_dir, "green.dat"), "w") as wtr:
-        wtr.write(header)
-        wtr.write("\n".join([str(value) for value in green[sidx:]]))
-    with open(os.path.join(out_dir, "blue.dat"), "w") as wtr:
-        wtr.write(header)
-        wtr.write("\n".join([str(value) for value in blue[sidx:]]))
-    sky_template = gen_rad_template()
-    with open(os.path.join(out_dir, "sky.rad"), "w") as wtr:
-        if direct_sun:
-            wtr.write("void light solar\n0\n0\n3 ")
-            wtr.write(f"{red[0]/solar_sa/source_dir[2]} ")
-            wtr.write(f"{green[0]/solar_sa/source_dir[2]} ")
-            wtr.write(f"{blue[0]/solar_sa/source_dir[2]}\n")
-            wtr.write(str(source_prim) + "\n")
-        wtr.write(sky_template)
+            _identifier = prim.identifier
+        _modifier = src_mod
+        if offset is not None:
+            poly = parsers.parse_polygon(prim.real_arg)
+            offset_vec = poly.normal.scale(offset)
+            moved_pts = [pt + offset_vec for pt in poly.vertices]
+            _real_args = geom.Polygon(moved_pts).to_real()
+        else:
+            _real_args = prim.real_arg
+        new_prim = Primitive(
+            _modifier, prim.ptype, _identifier, prim.str_arg, _real_args
+        )
+        content += str(new_prim) + "\n"
+    return header + content
+
+
+def rfluxmtx(
+    sender: Sender,
+    receiver: Receiver,
+    env: Iterable[Path],
+    opt: Optional[List[str]] = None,
+) -> None:
+    """
+    Calling rfluxmtx to generate the matrices.
+
+    Args:
+        sender: Sender object
+        receiver: Receiver object
+        env: model environment, basically anything that's not the
+            sender or receiver
+        opt: option string
+
+    Returns:
+        return the stdout of the rfluxmtx run.
+    """
+    if None in (sender, receiver):
+        raise ValueError("Sender/Receiver object is None")
+    opt = [] if opt is None else opt
+    _sender = None
+    stdin: Optional[bytes] = sender.sender
+    with tf.TemporaryDirectory() as tempd:
+        receiver_path = Path(tempd, "receiver")
+        with open(receiver_path, "w", encoding="ascii") as wtr:
+            wtr.write(receiver.receiver)
+        if sender.form == "s":
+            sender_path = Path(tempd, "sender")
+            with open(sender_path, "wb") as wtr:
+                wtr.write(sender.sender)
+            _sender = sender_path
+            stdin = None
+        elif sender.form == "p":
+            opt.extend(["-I+", "-faa", "-y", str(sender.yres)])
+        elif sender.form == "v":
+            opt.extend(["-ffc", "-x", str(sender.xres), "-y", str(sender.yres), "-ld-"])
+        cmd = raycall.get_rfluxmtx_command(
+            receiver_path, option=opt, sender=_sender, sys_paths=env
+        )
+        logger.info("Running rfluxmtx with:\n%s", " ".join(cmd))
+        proc = sp.run(cmd, check=True, input=stdin, stderr=sp.PIPE)
+        if proc.stderr != b"":
+            logger.warning(proc.stderr.decode())
+
+
+def rcvr_oct(receiver, env, oct_path: Union[str, Path]) -> None:
+    """
+    Generate an octree of the environment and the receiver.
+
+    Args:
+        receiver: receiver object
+        env: environment file paths
+        oct_path: Path to write the octree to
+    Returns:
+        None
+    """
+
+    with tf.TemporaryDirectory() as tempd:
+        receiver_path = os.path.join(tempd, "rcvr_path")
+        with open(receiver_path, "w", encoding="utf-8") as wtr:
+            wtr.write(receiver.receiver)
+        ocmd = ["oconv", "-f", *map(str, env), receiver_path]
+        logger.info("Generate octree with:\n%s", " ".join(ocmd))
+        with open(oct_path, "wb") as wtr:
+            sp.run(ocmd, check=True, stdout=wtr)
+
+
+def rcontrib(
+    sender,
+    modifier: str,
+    octree: Union[str, Path],
+    out: Union[str, Path],
+    opt: List[str],
+) -> None:
+    """
+    Calling rcontrib to generate the matrices.
+
+    Args:
+        sender: Sender object
+        modifier: modifier str listing the receivers in octree
+        octree: the octree that includes the environment and the receiver
+        opt: option string
+        out: output path
+
+    Returns:
+        None
+
+    """
+    opt.append("-fo+")
+    with tf.TemporaryDirectory() as tempd:
+        modifier_path = os.path.join(tempd, "modifier")
+        with open(modifier_path, "w", encoding="utf-8") as wtr:
+            wtr.write(modifier)
+        cmd = ["rcontrib", *opt]
+        stdin = sender.sender
+        if sender.form == "p":
+            cmd += ["-I+", "-faf", "-y", str(sender.yres)]
+        elif sender.form == "v":
+            out = Path(out)
+            out.mkdir(exist_ok=True)
+            out = out / "%04d.hdr"
+            cmd += ["-ffc", "-x", str(sender.xres), "-y", str(sender.yres)]
+        cmd += ["-o", str(out), "-M", modifier_path, str(octree)]
+        logger.info("Running rcontrib with:\n%s", " ".join(cmd))
+        sp.run(cmd, check=True, input=stdin)
```

### Comparing `frads-0.2.3/frads/makesky.py` & `frads-0.2.8/frads/ncp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,509 +1,472 @@
+#!/usr/bin/env python
 """
-Routines for generating sky models
+This module contains functionalities relating to generating matrices for
+non-coplanar shading systems
 """
 
-import argparse
-import csv
-import datetime
 import logging
 import math
 import os
+from pathlib import Path
 import subprocess as sp
 import tempfile as tf
-from frads import radutil, util, radgeom
-from typing import List, Union, Set, NamedTuple
-
-LSEP = os.linesep
-
-logger = logging.getLogger("frads.makesky")
-
-
-class WeaMetaData(NamedTuple):
-    city: str
-    country: str
-    latitude: float
-    longitude: float
-    timezone: int
-    elevation: float
-
-    def wea_header(self) -> str:
-        header = f"place {self.city}_{self.country}\n"
-        header += f"latitude {self.latitude}\n"
-        header += f"longitude {self.longitude}\n"
-        header += f"time_zone {self.timezone}\n"
-        header += f"site_elevation {self.elevation}\n"
-        header += "weather_data_file_units 1\n"
-        return header
-
-
-class WeaDataRow(NamedTuple):
-    month: int
-    day: int
-    hour: int
-    minute: int
-    second: int
-    hours: float
-    dni: float
-    dhi: float
-
-    def __str__(self):
-        return f"{self.month} {self.day} {self.hours} {self.dni} {self.dhi}"
-
-    def dt_string(self):
-        return f"{self.month:02d}{self.day:02d}_{self.hour:02d}30"
-
-
-def basis_glow(sky_basis):
-    """Sky and ground glow primitives.
-    Args:
-        sky_basis: sky sampling basis, e.g. r1, r4
-    Returns:
-        ground and sky glow string
+from typing import List
+from typing import Optional
+from typing import Sequence
+
+from frads import matrix
+from frads import geom
+from frads import parsers
+from frads.types import Primitive
+from frads.types import NcpModel
+from frads import utils
+
+logger: logging.Logger = logging.getLogger("frads.mfacade")
+
+
+def ncp_compute_back(
+    model: NcpModel, src: dict, opt: Optional[List[str]] = None, refl: bool = False
+) -> None:
+    """compute front side calculation(backwards)."""
+    logger.info("Computing for front side")
+    for idx, wp in enumerate(model.windows):
+        logger.info("Front transmission for window %s", idx)
+        front_rcvr = matrix.surface_as_receiver(
+            prim_list=model.ports,
+            basis=model.rbasis,
+            left=True,
+            offset=None,
+            source="glow",
+            out=src[f"tb{idx}"],
+        )
+        # sndr_prim = utils.polygon2prim(wplg, 'fsender', f'window{idx}')
+        sndr = matrix.surface_as_sender(
+            prim_list=[wp], basis=model.sbasis, left=True, offset=None
+        )
+        if refl:
+            logger.info("Front reflection for window %s", idx)
+            wflip = parsers.parse_polygon(wp.real_arg).flip()
+            wflip_prim = utils.polygon2prim(wflip, "breceiver", f"window{idx}")
+            back_rcvr = matrix.surface_as_receiver(
+                prim_list=[wflip_prim],
+                basis="-" + model.rbasis,
+                left=False,
+                offset=None,
+                source="glow",
+                out=src[f"rb{idx}"],
+            )
+            front_rcvr += back_rcvr
+        matrix.rfluxmtx(sender=sndr, receiver=front_rcvr, env=model.env, opt=opt)
+
+
+def ncp_compute_front(model: NcpModel, src_dict, opt, refl: bool = False) -> None:
+    """compute back side calculation."""
+    sndr_prim = []
+    for p in model.ports:
+        np = Primitive(
+            p.modifier,
+            p.ptype,
+            p.identifier,
+            p.str_arg,
+            parsers.parse_polygon(p.real_arg).flip().to_real(),
+        )
+        sndr_prim.append(np)
+    sndr = matrix.surface_as_sender(
+        prim_list=sndr_prim, basis="-" + model.rbasis, offset=None, left=False
+    )
+    logger.info("Computing for back side")
+    for idx, wp in enumerate(model.windows):
+        logger.info("Back transmission for window %s", idx)
+        wplg = parsers.parse_polygon(wp.real_arg).flip()
+        rcvr_prim = utils.polygon2prim(wplg, "breceiver", f"window{idx}")
+        rcvr = matrix.surface_as_receiver(
+            prim_list=[rcvr_prim],
+            basis="-" + model.sbasis,
+            left=False,
+            offset=None,
+            source="glow",
+            out=src_dict[f"tf{idx}"],
+        )
+        if refl:
+            logger.info("Back reflection for window %s", idx)
+            # brcvr_prim = [utils.polygon2prim(plg, "freceiver", "window" + str(i))
+            #               for i, pp in enumerate(model.ports)]
+            brcvr = matrix.surface_as_receiver(
+                prim_list=model.ports,
+                basis=model.rbasis,
+                left=False,
+                offset=None,
+                source="glow",
+                out=src_dict[f"rf{idx}"],
+            )
+            rcvr += brcvr
+        matrix.rfluxmtx(sender=sndr, receiver=rcvr, env=model.env, opt=opt)
+
+
+def klems_wrap(model, src_dict, fwrap_dict, out) -> None:
+    """prepare wrapping for Klems basis."""
+    for key in src_dict:
+        for _, _ in enumerate(model.windows):
+            inp = src_dict[key]
+            rcmd = ["rmtxop", "-fa", "-t", "-c", ".265", ".67", ".065", inp]
+            ps1 = sp.run(rcmd, check=True, stdout=sp.PIPE)
+            with open(fwrap_dict[key], "wb") as wtr:
+                sp.run(["getinfo", "-"], check=True, input=ps1.stdout, stdout=wtr)
+    for i, _ in enumerate(model.windows):
+        out_name = out.parent / (out.stem + f"{i}.xml")
+        sub_dict = {k: fwrap_dict[k] for k in fwrap_dict if k.endswith(str(i))}
+        cmd = ["wrapBSDF", "-a", model.rbasis, "-c"]
+        for i, j in sub_dict.items():
+            cmd.append("-" + i[:2])
+            cmd.append(str(j))
+        logger.info("Calling wrapBSDF with:\n%s", " ".join(cmd))
+        with open(out_name, "wb") as wtr:
+            sp.run(cmd, check=True, stdout=wtr)
+
+
+# def klems_wrap2(out, out2, inp, basis):
+#     """prepare wrapping for Klems basis."""
+#     cmd = f"rmtxop -fa -t -c .265 .67 .065 {inp} | getinfo - > {out}"
+#     sp.run(cmd, shell=True)
+#     basis_dict = {"kq": "Klems Quarter", "kh": "Klems Half", "kf": "Klems Full"}
+#     coeff = utils.angle_basis_coeff(basis_dict[basis])
+#     with open(out, "r") as rdr:
+#         rows = [map(float, l.split()) for l in rdr.readlines()]
+#     res = [[str(val / c) for val in row] for row, c in zip(rows, coeff)]
+#     with open(out2, "w") as wtr:
+#         [wtr.write("\t".join(row) + "\n") for row in res]
+
+
+def rttree_reduce(
+    ttrank, ttlog2, pctcull, refl, src: str, dest, spec: str = "Visible"
+) -> None:
+    """call rttree_reduce to reduce shirley-chiu to tensor tree.
+    translated from genBSDF.pl.
     """
-
-    grnd_str = grndglow()
-    sky_str = skyglow(sky_basis)
-    return grnd_str + sky_str
-
-
-def skyglow(basis: str, upvect='+Y') -> str:
-    sky_string = f"#@rfluxmtx u={upvect} h={basis}{LSEP*2}"
-    sky_string += f"void glow skyglow{LSEP}"
-    sky_string += f"0{LSEP}0{LSEP}4 1 1 1 0{LSEP*2}"
-    sky_string += f"skyglow source sky{LSEP}"
-    sky_string += f"0{LSEP}0{LSEP}4 0 0 1 180{LSEP}"
-    return sky_string
-
-
-def grndglow(basis='u') -> str:
-    ground_string = f"#@rfluxmtx h={basis}{LSEP*2}"
-    ground_string += f"void glow groundglow{LSEP}"
-    ground_string += f"0{LSEP}0{LSEP}4 1 1 1 0{LSEP*2}"
-    ground_string += f"groundglow source ground{LSEP}"
-    ground_string += f"0{LSEP}0{LSEP}4 0 0 -1 180{LSEP*2}"
-    return ground_string
-
-
-class Gensun(object):
-    """Generate sun sources for matrix generation."""
-
-    def __init__(self, mf: int):
-        """."""
-        self.runlen = 144 * mf**2 + 3
-        self.rsrc = radutil.Reinsrc(mf)
-        self.mod_str = LSEP.join([f'sol{i}' for i in range(1, self.runlen)])
-
-    def gen_full(self):
-        """Generate full treganza based sun sources."""
-        out_lines = []
-        for i in range(1, self.runlen):
-            dirs = self.rsrc.dir_calc(i)
-            line = f"void light sol{i} 0 0 3 1 1 1 sol{i} "
-            line += "source sun 0 0 4 {:.6g} {:.6g} {:.6g} 0.533".format(*dirs[:-1])
-            out_lines.append(line)
-        return LSEP.join(out_lines)+LSEP
-
-    def gen_cull(self, smx_path=None, window_normals=None):
-        """Generate culled sun sources based on window orientation and
-        climate based sky matrix. The reduced sun sources will significantly
-        speed up the matrix generation.
-        Args:
-            smx_path: sky matrix path, usually the output of gendaymtx
-            window_normals: window normals
-        Returns:
-            Sun receiver primitives strings
-            Corresponding modifier strings
-        """
-
-        win_norm = []
-        if smx_path is not None:
-            cmd = f"rmtxop -ff -c .3 .6 .1 -t {smx_path} "
-            cmd += "| getinfo - | total -if5186 -t,"
-            dtot = [float(i)
-                    for i in sp.check_output(cmd, shell=True).split(b',')]
+    CIEuv = (
+        "Xi=.5141*Ri+.3239*Gi+.1620*Bi;Yi=.2651*Ri+.6701*Gi+.0648*Bi;"
+        "Zi=.0241*Ri+.1229*Gi+.8530*Bi;den=Xi+15*Yi+3*Zi;"
+        "uprime=if(Yi,4*Xi/den,4/19);vprime=if(Yi,9*Yi/den,9/19);"
+    )
+
+    ns2 = int((2**ttlog2) ** 2)
+    if spec == "Visible":
+        cmd = [
+            "rcalc",
+            "-e",
+            f"Omega:PI/{ns2}",
+            "-e",
+            "Ri=$1;Gi=$2;Bi=$3",
+            "-e",
+            CIEuv,
+            "-e",
+            "$1=Yi/Omega",
+        ]
+    elif spec == "CIE-u":
+        cmd = ["rcalc", "-e", "Ri=$1;Gi=$2;Bi=$3", "-e", CIEuv, "-e", "$1=uprime"]
+    elif spec == "CIE-v":
+        cmd = ["rcalc", "-e", "Ri=$1;Gi=$2;Bi=$3", "-e", CIEuv, "-e", "$1=vprime"]
+
+    if os.name == "posix":
+        cmd.insert(1, "-if3")
+    if pctcull >= 0:
+        avg = "-a" if refl else ""
+        pcull = pctcull if spec == "Visible" else (100 - (100 - pctcull) * 0.25)
+        rtcmd = [
+            "rttree_reduce",
+            avg,
+            "-h",
+            "-ff",
+            "-t",
+            pcull,
+            "-r",
+            ttrank,
+            "-g",
+            ttlog2,
+        ]
+        if os.name == "posix":
+            cmd.extend(["-of", src])
+            ps1 = sp.run(cmd + ["-of", src], check=True, stdout=sp.PIPE)
+            with open(dest, "wb") as wtr:
+                ps2 = sp.run(rtcmd, check=True, input=ps1.stdout, stdout=wtr)
+        else:
+            ps1 = sp.run(
+                ["rcollate", "-ho", "-oc", "1", src], check=True, stdout=sp.PIPE
+            )
+            ps2 = sp.run(cmd, check=True, input=ps1.stdout, stdout=sp.PIPE)
+            with open(dest, "wb") as wtr:
+                sp.run(rtcmd, check=True, input=ps2.stdout, stdout=wtr)
+    else:
+        if os.name == "posix":
+            with open(dest, "wb") as wtr:
+                sp.run(cmd.append(src), check=True, stdout=wtr)
         else:
-            dtot = [1] * self.runlen
-        out_lines = []
-        mod_str = []
-        if window_normals is not None:
-            win_norm = window_normals
-            for i in range(1, self.runlen):
-                dirs = radgeom.Vector(*self.rsrc.dir_calc(i)[:-1])
-                _mod = 'sol'+str(i)
-                v = 0
-                if dtot[i - 1] > 0:
-                    for norm in win_norm:
-                        if norm * dirs < 0:
-                            v = 1
-                            mod_str.append(_mod)
-                            break
-                line = f"void light sol{i} 0 0 3 {v} {v} {v} sol{i} "
-                line += f"source sun 0 0 4 {dirs.z:.6g} {dirs.x:.6g} {dirs.z:.6g} 0.533"
-                out_lines.append(line)
+            ps1 = sp.run(
+                ["rcollate", "-ho", "-oc", "1", src], check=True, stdout=sp.PIPE
+            )
+            with open(dest, "wb") as wtr:
+                sp.run(cmd, check=True, input=ps1.stdout, stdout=wtr)
+
+
+def tt_wrap(model, src_dict, fwrap_dict, out, refl) -> None:
+    """call wrapBSDF to wrap a XML file."""
+    sc = int(model.rbasis[2:])
+    ttlog2 = math.log(sc, 2)
+    assert ttlog2 % int(ttlog2) == 0
+    ttrank = 4  # only anisotropic
+    pctcull = 90
+    ttlog2 = int(ttlog2)
+    for i, _ in enumerate(model.windows):
+        sub_key = [k for k in src_dict if k.endswith(str(i))]
+        sub_dict = {k: fwrap_dict[k] for k in sub_key}
+        for key in sub_key:
+            rttree_reduce(ttrank, ttlog2, pctcull, refl, src_dict[key], fwrap_dict[key])
+        cmd = ["wrapBSDF", "-a", "t4", "-s", "Visible"]
+        cmd += [" ".join(("-" + i[:2], str(j))) for i, j in sub_dict.items()]
+        cmd += f"> {out}.xml"
+        with open(out, "wb") as wtr:
+            sp.run(cmd, check=True, stdout=wtr)
+
+
+def gen_ncp_mtx(
+    model: NcpModel,
+    out: Path,
+    opt: Optional[List[str]] = None,
+    refl: bool = False,
+    forw: bool = False,
+    wrap: bool = True,
+    # solar=False,
+) -> None:
+    """Generate a set of non-coplanar shading matrices."""
+
+    # Collect all the primitives
+    # all_prims = []
+    # for path in model.env:
+    #     all_prims.extend(utils.unpack_primitives(path))
+
+    # # Find out the modifier of the ncp polygon
+    # ncp_mod = [prim.modifier for prim in ncp_prims if prim.ptype == "polygon"][0]
+
+    # # Find out the ncp material primitive
+    # ncp_mat: Primitive
+    # ncp_type: str = ""
+    # for prim in all_prims:
+    #     if prim.identifier == ncp_mod:
+    #         ncp_mat = prim
+    #         ncp_type = prim.ptype
+    #         break
+    # if ncp_type == "":
+    #     raise ValueError("Unknown NCP material")
+
+    # dirname = out.parent
+    # if solar and ncp_type == "BSDF":
+    #     logger.info("Computing for solar and visible spectrum...")
+    #     xmlpath = ncp_mat.str_arg.split()[2]
+    #     td = tf.mkdtemp()
+    #     with open(xmlpath) as rdr:
+    #         raw = rdr.read()
+    #     raw = raw.replace(
+    #         '<Wavelength unit="Integral">Visible</Wavelength>',
+    #         '<Wavelength unit="Integral">Visible2</Wavelength>',
+    #     )
+    #     raw = raw.replace(
+    #         '<Wavelength unit="Integral">Solar</Wavelength>',
+    #         '<Wavelength unit="Integral">Visible</Wavelength>',
+    #     )
+    #     raw = raw.replace(
+    #         '<Wavelength unit="Integral">Visible2</Wavelength>',
+    #         '<Wavelength unit="Integral">Solar</Wavelength>',
+    #     )
+    #     solar_xml_path = os.path.join(td, "solar.xml")
+    #     with open(solar_xml_path, "w") as wtr:
+    #         wtr.write(raw)
+    #     _strarg = ncp_mat.str_arg.split()
+    #     _strarg[2] = solar_xml_path
+    #     solar_ncp_mat = Primitive(
+    #         ncp_mat.modifier,
+    #         ncp_mat.ptype,
+    #         ncp_mat.identifier + ".solar",
+    #         " ".join(_strarg),
+    #         "0",
+    #     )
+
+    #     _env_path = os.path.join(td, "env_solar.rad")
+    #     with open(_env_path, "w") as wtr:
+    #         for prim in all_prims:
+    #             wtr.write(str(prim))
+    #     outsolar = dirname / ("_solar_{out.stem}.dat")
+
+    klems = True
+    if wrap and (model.rbasis.startswith("sc")) and (model.sbasis.startswith("sc")):
+        klems = False
+        sc = int(model.rbasis[2:])
+        ttlog2 = math.log(sc, 2)
+        if ttlog2 % int(ttlog2) != 0:
+            raise ValueError("Invalid tensor tree resolution.")
+        if opt is not None:
+            opt.append("-hd")
+            opt.append("-ff")
+    with tf.TemporaryDirectory() as td:
+        src_dict = {}
+        fwrap_dict = {}
+        for idx, _ in enumerate(model.windows):
+            _tf = f"tf{idx}"
+            _rf = f"rf{idx}"
+            _tb = f"tb{idx}"
+            _rb = f"rb{idx}"
+            src_dict[_tb] = Path(td, _tb + ".dat")
+            fwrap_dict[_tb] = Path(td, _tb + "p.dat")
+            if forw:
+                src_dict[_tf] = Path(td, _tf + ".dat")
+                fwrap_dict[_tf] = Path(td, _tf + "p.dat")
+            if refl:
+                src_dict[_rb] = Path(td, _rb + ".dat")
+                fwrap_dict[_rb] = Path(td, _rb + "p.dat")
+                if forw:
+                    src_dict[_rf] = Path(td, _rf + ".dat")
+                    fwrap_dict[_rf] = Path(td, _rf + "p.dat")
+        ncp_compute_back(model, src_dict, opt, refl=refl)
+        if forw:
+            ncp_compute_front(model, src_dict, opt, refl=refl)
+        if wrap:
+            if klems:
+                klems_wrap(model, src_dict, fwrap_dict, out)
+            else:
+                tt_wrap(model, src_dict, fwrap_dict, out, refl)
         else:
-            for i in range(1, self.runlen):
-                dirs = radgeom.Vector(*self.rsrc.dir_calc(i)[:-1])
-                _mod = 'sol'+str(i)
-                v = 0
-                if dtot[i - 1] > 0:
-                    v = 1
-                    mod_str.append(_mod)
-                line = f"void light sol{i} 0 0 3 {v} {v} {v} sol{i} "
-                line += f"source sun 0 0 4 {dirs.z:.6g} {dirs.x:.6g} {dirs.z:.6g} 0.533"
-                out_lines.append(line)
-        logger.debug(out_lines)
-        logger.debug(mod_str)
-        return LSEP.join(out_lines), LSEP.join(mod_str)
-
-
-def epw2sunmtx(epw_path: str) -> str:
-    """Generate reinhart 6 sun matrix file from a epw file."""
-    smx_path = util.basename(epw_path) + ".smx"
-    with tf.NamedTemporaryFile() as wea:
-        cmd = f"epw2wea {epw_path} {wea.name}"
-        sp.call(cmd, shell=True)
-        cmd = f"gendaymtx -od -u -m 6 -d -5 .533 {wea.name} > {smx_path}"
-        sp.call(cmd, shell=True)
-    return smx_path
-
-
-def loc2sunmtx(basis, lat, lon, ele):
-    """Generate a psuedo reinhart 6 sun matrix file given lat, lon, etc..."""
-    tz = int(5 * round(lon / 5))
-    metadata = WeaMetaData('city', 'country', lat, lon, tz, ele)
-    header = metadata.wea_header()
-    header = str.encode(header)
-    string = ""
-    mday = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
-    for mo in range(12):
-        for da in range(mday[mo]):
-            for ho in range(24):
-                string += f"{mo+1} {da+1} {ho+.5} 100 100"
-    string = str.encode(string)
-    smx_path = f"sun_{lat}_{lon}_{basis}.smx"
-    with tf.NamedTemporaryFile() as wea:
-        wea.write(header)
-        wea.write(string)
-        cmd = f"gendaymtx -od -m 6 -u -d -5 .533 {wea.name} > {smx_path}"
-        sp.call(cmd, shell=True)
-    return smx_path
-
-
-def gendaymtx(data_entry: List[WeaDataRow], metadata: WeaMetaData,
-              mf=4, direct=False, solar=False, onesun=False,
-              rotate=0, binary=False):
-    """."""
-    cmd = ['gendaymtx', '-r', str(rotate), '-m', str(mf)]
-    if direct:
-        cmd.append('-d')
-    if solar:
-        cmd.append('-O1')
-    if onesun:
-        cmd.append('-5')
-        cmd.append('.533')
-    if binary:
-        cmd.append('-of')
-    wea_input = metadata.wea_header() + "\n".join(map(str, data_entry))
-    sky_matrix = util.spcheckout(cmd, inp=wea_input.encode())
-    return sky_matrix
-
-
-def gendaymtx_cmd(data_entry: List[str], metadata: WeaMetaData,
-                  mf=4, direct=False, solar=False, onesun=False,
-                  rotate=0, binary=False):
-    """."""
-    sun_only = ' -d' if direct else ''
-    spect = ' -O1' if solar else ' -O0'
-    _five = ' -5 .533' if onesun else ''
-    bi = '' if binary is False or os.name == 'nt' else ' -o' + binary
-    linesep = r'& echo' if os.name == 'nt' else LSEP
-    wea_head = f"place test{linesep}latitude {metadata.latitude}{linesep}"
-    wea_head += f"longitude {metadata.longitude}{linesep}"
-    wea_head += f"time_zone {metadata.timezone}{linesep}site_elevation "
-    wea_head += f"{metadata.elevation}{linesep}"
-    wea_head += f"weather_data_file_units 1{linesep}"
-    skv_cmd = f"gendaymtx -u -r {rotate} -m {mf}{sun_only}{_five}{spect}{bi}"
-    wea_data = linesep.join(data_entry)
-    if os.name == 'nt':
-        wea_cmd = f'(echo {wea_head}{wea_data}) | '
+            for key, file in src_dict.items():
+                out_name = f"{out.stem}_{key}.mtx"
+                file.rename(out.parent / out_name)
+
+    # if solar and ncp_type == "BSDF":
+    #     # process_thread.join()
+    #     vis_dict = {}
+    #     sol_dict = {}
+    #     oname = out.stem
+    #     mtxs = [
+    #         os.path.join(dirname, mtx)
+    #         for mtx in os.listdir(dirname)
+    #         if mtx.endswith(".mtx")
+    #     ]
+    #     for mtx in mtxs:
+    #         _direc = Path(mtx).stem.split("_")[-1][:2]
+    #         mtxname = Path(mtx).stem
+    #         if mtxname.startswith(oname):
+    #             # vis_dict[_direc] = os.path.join(dirname, f"_vis_{_direc}")
+    #             vis_dict[_direc] = os.path.join(td, f"vis_{_direc}")
+    #             out2 = os.path.join(dirname, f"vis_{_direc}")
+    #             klems_wrap(vis_dict[_direc], out2, mtx, args.ss)
+    #         if mtxname.startswith("_solar_"):
+    #             sol_dict[_direc] = os.path.join(td, f"sol_{_direc}")
+    #             out2 = os.path.join(dirname, f"sol_{_direc}")
+    #             klems_wrap(sol_dict[_direc], out2, mtx, args.ss)
+    #     cmd = f"wrapBSDF -a {args.ss} -c -s Visible "
+    #     cmd += " ".join([f"-{key} {vis_dict[key]}" for key in vis_dict])
+    #     cmd += " -s Solar "
+    #     cmd += " ".join([f"-{key} {sol_dict[key]}" for key in sol_dict])
+    #     cmd += f" > {os.path.join(dirname, oname)}.xml"
+    #     os.system(cmd)
+    #     shutil.rmtree(td)
+    #     [os.remove(mtx) for mtx in mtxs]
+
+
+def gen_port_prims_from_window_ncp(
+    wprim: Sequence[Primitive], nprim: Sequence[Primitive]
+) -> List[Primitive]:
+    """Generate port primitives from window and non-coplanar shading primitives."""
+    if len(wprim) > 1:
+        awprim = merge_windows(wprim)
     else:
-        wea_cmd = f'echo "{wea_head}{wea_data}" | '
-    cmd = wea_cmd + skv_cmd
-    return cmd
-
-
-def parse_csv(csv_path, ftype='csv', dt_col="date_time",
-              dt_format="%Y%m%d %H:%M:%S", dni_col='DNI',
-              dhi_col='DHI', stime=None, etime=None):
-    """Parse a csv file containing direct normal
-    and diffuse horizontal data, ignoring NULL
-    and zero values.
-
-    Parameters:
-        csv_path: str
-            Path to the csv/tsv file.
-        ftype: str, default csv
-            File type to choose between csv and tsv.
-        dt_col: str, default date_time
-            name of the datetime column.
-        dt_format: str, default %Y%m%d %H:%M:%S
-            Python datetime format.
-        dni_col: str, default DNI
-            Column name containing direct normal
-            irradiation data.
-        dhi_col: str, default DHI
-            Column name containing diffuse horizontal
-            irradiation data.
-        stime: str, default None
-            Exclude the data before this time. e.g.'09:00'
-        etime: str, default None
-            Exclude the data after this time. e.g.'17:00'
-    Returns: list object
-        a list of strings containing datetime
-        and solar radiation values
-    """
-
-    data_entry = []
-    if None not in (stime, etime):
-        stime = datetime.datetime.strptime(stime, "%H:%M")
-        etime = datetime.datetime.strptime(etime, "%H:%M")
-        shours = stime.hour + stime.minute / 60.0
-        ehours = etime.hour + etime.minute / 60.0
+        awprim = wprim[0]
+    wplg = parsers.parse_polygon(awprim.real_arg)
+    nplgs = [parsers.parse_polygon(p.real_arg) for p in nprim if p.ptype == "polygon"]
+    all_ports = gen_ports_from_window_ncp(wplg, nplgs)
+    port_prims = []
+    for idx, plg in enumerate(all_ports):
+        new_prim = utils.polygon2prim(plg, "port", f"portf{idx+1}")
+        logger.debug(str(new_prim))
+        port_prims.append(new_prim)
+    return port_prims
+
+
+def gen_port_prims_from_window(
+    wprim: Sequence[Primitive], depth: float, scale_factor: float
+) -> List[Primitive]:
+    """Generate port primitives from window primitives, depth, and scale factor."""
+    if len(wprim) > 1:
+        awprim = merge_windows(wprim)
     else:
-        shours = 0
-        ehours = 24
-    ftypes = {'csv': 'excel', 'tsv': 'excel-tab'}
-    with open(csv_path, encoding='utf-8-sig') as csvfile:
-        reader = csv.DictReader(csvfile, dialect=ftypes[ftype])
-        for row in reader:
-            _dt = datetime.datetime.strptime(row[dt_col], dt_format)
-            _year = str(_dt.year)
-            _month = str(_dt.month)
-            _day = str(_dt.day)
-            _hour = _dt.hour
-            _minute = _dt.minute
-            _hours = round(_hour + _minute / 60.0, 2)
-            if _hours < shours or _hours > ehours:
-                continue
-            try:
-                _dni = float(row[dni_col])
-                _dhi = float(row[dhi_col])
-            except ValueError:
-                continue
-            if int(_dni) == 0 and int(_dhi) == 0:
-                continue
-            data_entry.append(
-                [_year, _month, _day, _hour, _minute, _hours, _dni, _dhi])
-    return data_entry
-
-
-def sky_cont(mon, day, hrs, lat, lon, mer, dni, dhi,
-             year=None, grefl=.2, spect='0', rotate=None):
-    out_str = f'!gendaylit {mon} {day} {hrs} '
-    out_str += f'-a {lat} -o {lon} -m {mer} '
-    if year is not None:
-        out_str += f'-y {year} '
-    out_str += f'-W {dni} {dhi} -g {grefl} -O {spect}{LSEP*2}'
-    if rotate is not None:
-        out_str += f"| xform -rz {rotate}"
-    out_str += f'skyfunc glow skyglow 0 0 4 1 1 1 0{LSEP*2}'
-    out_str += f'skyglow source sky 0 0 4 0 0 1 180{LSEP*2}'
-    out_str += f'skyfunc glow groundglow 0 0 4 1 1 1 0{LSEP*2}'
-    out_str += f'groundglow source ground 0 0 4 0 0 -1 180{LSEP}'
-    return out_str
-
-
-def gendaylit_cmd(month: str, day: str, hours: str,
-                  lat: str, lon: str, tzone: str,
-                  year: str = None, dir_norm_ir: str = None,
-                  dif_hor_ir: str = None, dir_hor_ir: str = None,
-                  dir_norm_il: str = None, dif_hor_il: str = None,
-                  solar: bool = False) -> list:
-    """Get a gendaylit command as a list."""
-    cmd = ["gendaylit", month, day, hours]
-    cmd += ["-a", lat, "-o", lon, "-m", tzone]
-    if year is not None:
-        cmd += ["-y", year]
-    if None not in (dir_norm_ir, dif_hor_ir):
-        cmd += ["-W", dir_norm_ir, dif_hor_ir]
-    if None not in (dir_hor_ir, dif_hor_ir):
-        cmd += ["-G", dir_hor_ir, dif_hor_ir]
-    if None not in (dir_norm_il, dif_hor_il):
-        cmd += ["-L", dir_norm_il, dif_hor_il]
-    if solar:
-        cmd += ["-O", "1"]
-    return cmd
-
-
-def solar_angle(lat, lon, mer, month, day, hour):
-    """Simplified translation from the Radiance sun.c and gensky.c code.
-
-    This function test if the solar altitude is greater than zero
+        awprim = wprim[0]
+    wpoly = parsers.parse_polygon(awprim.real_arg)
+    extrude_vector = wpoly.normal.reverse().scale(depth)
+    scale_vector = geom.Vector(scale_factor, scale_factor, scale_factor)
+    scaled_window = wpoly.scale(scale_vector, wpoly.centroid())
+    all_ports = scaled_window.extrude(extrude_vector)[1:]
+    port_prims = []
+    for idx, plg in enumerate(all_ports):
+        new_prim = utils.polygon2prim(plg, "port", f"portf{idx+1}")
+        logger.debug(str(new_prim))
+        port_prims.append(new_prim)
+    return port_prims
+
+
+def gen_ports_from_window_ncp(
+    wp: geom.Polygon, np: List[geom.Polygon]
+) -> List[geom.Polygon]:
     """
-    latitude_r = math.radians(lat)
-    longitude_r = math.radians(lon)
-    s_meridian = math.radians(mer)
-    mo_da = [0, 31, 59, 90, 120, 151, 181, 212, 243, 273, 304, 334]
+    Generate ports polygons that encapsulate the window and NCP geometries.
 
-    julian_date = mo_da[month - 1] + day
-
-    solar_decline = 0.4093 * math.sin((2 * math.pi / 365) * (julian_date - 81))
-
-    solar_time = hour + (0.170 * math.sin((4 * math.pi / 373) * (julian_date - 80)) - 0.129 * math.sin((2 * math.pi / 355) * (julian_date - 8)) + (12/math.pi) * (s_meridian - longitude_r))
-    altitude = math.asin(math.sin(latitude_r) * math.sin(solar_decline) - math.cos(latitude_r) * math.cos(solar_decline) * math.cos(solar_time * (math.pi / 12)))
-    azimuth = -math.atan2(math.cos(solar_decline)*math.sin(solar_time*(math.pi/12.)), -math.cos(latitude_r)*math.sin(solar_time) - math.sin(latitude_r)*math.cos(solar_decline) * math.cos(solar_time*(math.pi/12)))
-
-    return altitude, azimuth
-
-
-def start_end_hour(data: list, sh: float, eh: float):
-    """Remove wea data entries outside of the
-    start and end hour."""
-    if sh == 0 and eh == 0:
-        return data
-
-    def filter_hour(dataline):
-        return sh <= float(dataline[2]) <= eh
-    return filter(filter_hour, data)
-
-
-def check_sun_above_horizon(data, metadata):
-    """Remove non-daylight hour entries."""
-    def solar_altitude_check(row: WeaDataRow):
-        alt, _ = solar_angle(metadata.latitude, metadata.longitude,
-                             metadata.timezone, row.month,
-                             row.day, row.hours)
-        return alt > 0
-    return filter(solar_altitude_check, data)
-
-
-def remove_wea_zero_entry(data, metadata: WeaMetaData, window_normal=None):
-    """Remove wea data entries with zero solar luminance.
-    If window normal supplied, eliminate entries not seen by window.
-    Solar luminance determined using Perez sky model.
-    Window field of view is 176 deg with 2 deg tolerance on each side.
+    window and NCP geometries are rotated around +Z axis until
+    the axis-aligned bounding box projected onto XY plane is
+    the smallest, thus the systems are facing
+    orthogonal direction. A boundary box is then generated with a slight
+    outward offset. This boundary box is then rotated back the same amount
+    to encapsulate the original window and NCP geomteries.
     """
-    check_window_normal = True if window_normal is not None else False
-    new_dataline = []
-    data = filter(lambda row: row.dni != 0, data)
-    for row in data:
-        cmd = ['gendaylit', str(row.month), str(row.day), str(row.hours),
-               '-a', str(metadata.latitude), '-o', str(metadata.longitude),
-               '-m', str(metadata.timezone), '-W', str(row.dni), str(row.dhi)]
-        process = sp.run(cmd, stderr=sp.PIPE, stdout=sp.PIPE)
-        primitives = radutil.parse_primitive(
-            process.stdout.decode().splitlines())
-        if process.stderr == b'':
-            light = float(primitives[0].real_arg.split()[2])
-            dirs = radgeom.Vector(*list(map(float, primitives[1].real_arg.split()[1:4])))
-            if light > 0:
-                if check_window_normal:
-                    for normal in window_normal:
-                        if normal * dirs < -0.035: # 2deg tolerance
-                            new_dataline.append(row)
-                            break
-                else:
-                    new_dataline.append(row)
-    return new_dataline
-
-
-def parse_epw(epw_str: str) -> tuple:
-    """Parse epw file and return wea header and data."""
-    raw = epw_str.splitlines()
-    epw_header = raw[0].split(',')
-    content = raw[8:]
-    data = []
-    for li in content:
-        line = li.split(',')
-        month = int(line[1])
-        day = int(line[2])
-        hour = int(line[3]) - 1
-        hours = hour + 0.5
-        dir_norm = float(line[14])
-        dif_hor = float(line[15])
-        data.append(WeaDataRow(
-            month, day, hour, 30, 0, hours, dir_norm, dif_hor))
-    city = epw_header[1]
-    country = epw_header[3]
-    latitude = float(epw_header[6])
-    longitude = -1 * float(epw_header[7])
-    tz = int(float(epw_header[8])) * (-15)
-    elevation = float(epw_header[9].rstrip())
-    meta_data = WeaMetaData(city, country, latitude, longitude, tz, elevation)
-    return meta_data, data
-
-
-def epw2wea(epw_str,
-            dhour=False, shour=None, ehour=None,
-            remove_zero=False, window_normal=None):
-    """epw2wea with added filter."""
-    metadata, data = parse_epw(epw_str)
-    if None not in (shour, ehour):
-        data = start_end_hour(data, shour, ehour)
-    if dhour:
-        data = check_sun_above_horizon(data, metadata)
-    if remove_zero:
-        data = remove_wea_zero_entry(data, metadata,
-                                     window_normal=window_normal)
-    return metadata, list(data)
-
-
-def getwea():
-    """Commandline program for generating a .wea file
-    from downloaded EPW data."""
-    parser = argparse.ArgumentParser(
-        prog='getwea',
-        description="Download the EPW files and convert it to a wea file")
-    parser.add_argument('-a', type=float, help='latitude')
-    parser.add_argument('-o', type=float, help='longitude')
-    parser.add_argument('-z', help='zipcode (U.S. only)')
-    parser.add_argument('-dh', action="store_true",
-                        help='output only for daylight hours')
-    parser.add_argument('-sh', type=float, help='start hour (float)')
-    parser.add_argument('-eh', type=float, help='end hour (float)')
-    parser.add_argument('-rz', action='store_true', help='remove zero solar luminance entries')
-    parser.add_argument('-wpths', nargs='+', help='window paths (.rad)')
-    parser.add_argument(
-        "-v", "--verbose", action="count", default=0,
-        help="Verbose mode: \n"
-        "\t-v=Debug\n"
-        "\t-vv=Info\n"
-        "\t-vvv=Warning\n"
-        "\t-vvvv=Error\n"
-        "\t-vvvvv=Critical\n"
-        "default=Warning")
-    args = parser.parse_args()
-    # Setup logger
-    formatter = logging.Formatter(
-        "%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-    console_handler = logging.StreamHandler()
-    _level = args.verbose * 10
-    logger.setLevel(_level)
-    console_handler.setLevel(_level)
-    console_handler.setFormatter(formatter)
-    logger.addHandler(console_handler)
-    window_normals: Union[None, Set[radgeom.Vector]] = None
-    if args.z is not None:
-        lat, lon = util.get_latlon_from_zipcode(args.z)
-    elif None not in (args.a, args.o):
-        lat, lon = args.a, args.o
-    else:
-        print("Exit: need either latitude and longitude or U.S. postcode")
-        exit()
-    _, url = util.get_epw_url(lat, lon)
-    logger.debug("EPW URL:" + url)
-    epw = util.request(url, {})
-    remove_zero = False
-    if args.wpths is not None:
-        window_normals = radutil.primitive_normal(args.wpths)
-        remove_zero = True
-    wea_metadata, wea_data = parse_epw(epw)
-    if None not in (args.sh, args.eh):
-        wea_data = start_end_hour(wea_data, args.sh, args.eh)
-    if args.dh:
-        wea_data = check_sun_above_horizon(wea_data, wea_metadata)
-    if remove_zero:
-        wea_data = remove_wea_zero_entry(
-            wea_data, wea_metadata, window_normals)
-    print(wea_metadata.wea_header())
-    print('\n'.join(map(str, wea_data)))
+    wn = wp.normal
+    if (abs(wn.y) == 1) or (abs(wn.x) == 1):
+        np.append(wp)
+        bbox = geom.getbbox(np, offset=0.00)
+        bbox.remove([b for b in bbox if b.normal.reverse() == wn][0])
+        return [b.move(wn.scale(-0.1)) for b in bbox]
+    xax = [1, 0, 0]
+    _xax = [-1, 0, 0]
+    yax = [0, 1, 0]
+    _yax = [0, -1, 0]
+    zaxis = geom.Vector(0, 0, 1)
+    rm_pg = [xax, _yax, _xax, yax]
+    area_list = []
+    win_normals = []
+    # Find axiel aligned rotation angle
+    bboxes = []
+    for deg in range(90):
+        rad = math.radians(deg)
+        win_polygon_r = wp.rotate(zaxis, rad)
+        win_normals.append(win_polygon_r.normal())
+        ncs_polygon_r = [p.rotate(zaxis, rad) for p in np]
+        ncs_polygon_r.append(win_polygon_r)
+        _bbox = geom.getbbox(ncs_polygon_r, offset=0.0)
+        bboxes.append(_bbox)
+        area_list.append(_bbox[0].area())
+    # Rotate to position
+    deg = area_list.index(min(area_list))
+    rrad = math.radians(deg)
+    bbox = bboxes[deg]
+    _win_normal = [round(i, 1) for i in win_normals[deg].to_list()]
+    del bbox[rm_pg.index(_win_normal) + 2]
+    rotate_back = [pg.rotate(zaxis, rrad * -1) for pg in bbox]
+    return rotate_back
+
+
+def merge_windows(prims: Sequence[Primitive]) -> Primitive:
+    """Merge rectangles if coplanar."""
+    polygons = [parsers.parse_polygon(p.real_arg) for p in prims]
+    normals = [p.normal() for p in polygons]
+    if len(set(normals)) > 1:
+        raise ValueError("Windows not co-planar")
+    points = [i for p in polygons for i in p.vertices]
+    hull_polygon = geom.convexhull(points, normals[0])
+    modifier = prims[0].modifier
+    identifier = prims[0].identifier
+    new_prim = utils.polygon2prim(hull_polygon, modifier, identifier)
+    return new_prim
```

### Comparing `frads-0.2.3/frads/mtxmult.py` & `frads-0.2.8/frads/sky.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,387 +1,460 @@
-"""Multiply Radiance matrix files.
+"""
+Routines for generating sky models
 """
 
-import argparse
-import multiprocessing as mp
-import glob
+import datetime
 import logging
+import math
 import os
-import re
+from pathlib import Path
 import subprocess as sp
-try:
-    import numpy as np
-    NUMPY_FOUND = True
-except ModuleNotFoundError:
-    NUMPY_FOUND = False
-
-from frads import util
-
-
-logger = logging.getLogger("frads.radutil")
-
-
-def parse_rad_header(header_str: str) -> tuple:
-    """Parse a Radiance matrix file header."""
-    compiled = re.compile(
-        r' NROWS=(.*) | NCOLS=(.*) | NCOMP=(.*) | FORMAT=(.*) ', flags=re.X)
-    matches = compiled.findall(header_str)
-    if len(matches) != 4:
-        raise ValueError("Can't find one of the header entries.")
-    nrow = int([mat[0] for mat in matches if mat[0] != ''][0])
-    ncol = int([mat[1] for mat in matches if mat[1] != ''][0])
-    ncomp = int([mat[2] for mat in matches if mat[2] != ''][0])
-    dtype = [mat[3] for mat in matches if mat[3] != ''][0].strip()
-    return nrow, ncol, ncomp, dtype
-
-
-def pcomb(inputs):
-    """Image operations with pcomb.
-    Parameter: inputs,
-        e.g: ['img1.hdr', '+', img2.hdr', '-', 'img3.hdr', 'output.hdr']
-    """
-    input_list = inputs[:-1]
-    out_dir = inputs[-1]
-    component_idx = range(0, len(input_list), 2)
-    components = [input_list[i] for i in component_idx]
-    color_op_list = []
-    for c in 'rgb':
-        color_op = input_list[:]
-        for i in component_idx:
-            color_op[i] = '%si(%d)' % (c, i/2+1)
-        cstr = '%so=%s' % (c, ''.join(color_op))
-        color_op_list.append(cstr)
-    rgb_str = ';'.join(color_op_list)
-    cmd = ['pcomb', '-e', '%s' % rgb_str]
-    img_name = util.basename(input_list[0], keep_ext=True)
-    for c in components:
-        cmd.append('-o')
-        cmd.append(c)
-    res = util.spcheckout(cmd)
-    with open(os.path.join(out_dir, img_name), 'wb') as wtr:
-        wtr.write(res)
-
-
-def dctimestep(input_list):
-    """Image operations in forms of Vs, VDs, VTDs, VDFs, VTDFs."""
-    inputs = input_list[:-1]
-    out_dir = input_list[-1]
-    inp_dir_count = len(inputs)
-    sky = input_list[-2]
-    img_name = util.basename(sky)
-    out_path = os.path.join(out_dir, img_name)
-
-    if inputs[1].endswith('.xml') is False\
-            and inp_dir_count > 2 and os.path.isdir(inputs[0]):
-        combined = "'!rmtxop %s" % (' '.join(inputs[1:-1]))
-        img = [i for i in os.listdir(inputs[0]) if i.endswith('.hdr')][0]
-        str_count = len(img.split('.hdr')[0])  # figure out unix %0d string
-        appendi = r"%0"+"%sd.hdr" % (str_count)
-        new_inp_dir = [os.path.join(inputs[0], appendi), combined]
-        cmd = "dctimestep -oc %s %s' > %s.hdr" \
-            % (' '.join(new_inp_dir), sky, out_path)
+from typing import SupportsFloat, Any
+from typing import List
+from typing import Optional
+from typing import Sequence
+from typing import Tuple
+from typing import Union
+
+from frads import geom
+from frads import parsers
+from frads.types import WeaMetaData
+from frads.types import WeaData
+from frads import utils
 
-    else:
-        if not os.path.isdir(inputs[0]) and not inputs[1].endswith('.xml'):
-            combined = os.path.join(os.path.dirname(inputs[0]), "tmp.vfdmtx")
-            stderr = combine_mtx(inputs[:-1], combined)
-            if stderr != "":
-                print(stderr)
-                return
-            inputs_ = [combined]
-
-        elif inp_dir_count == 5:
-            combined = os.path.join(os.path.dirname(inputs[2]), "tmp.fdmtx")
-            stderr = combine_mtx(inputs[2:4], combined)
-            if stderr != "":
-                print(stderr)
-                return
-            inputs_ = [inputs[0], inputs[1], combined]
-
-        else:
-            inputs_ = inputs[:-1]
-
-        if os.path.isdir(inputs[0]):
-            img = [i for i in os.listdir(inputs[0])
-                   if i.endswith('.hdr')][0]
-            str_count = len(img.split('.hdr')[0])
-            appendi = r"%0"+"%sd.hdr" % (str_count)
-            inputs_[0] = os.path.join(inputs[0], appendi)
-            out_ext = ".hdr"
-        else:
-            out_ext = ".dat"
-
-        input_string = ' '.join(inputs_)
-        out_path = out_path + out_ext
-        cmd = "dctimestep %s %s > %s" % (input_string, sky, out_path)
-    sp.call(cmd, shell=True)
-
-
-def dctsop(inputs, out_dir, nproc=1):
-    if not os.path.isdir(out_dir):
-        os.makedirs(out_dir)
-    nproc = mp.cpu_count() if nproc is None else nproc
-    process = mp.Pool(nproc)
-    assert len(inputs) > 1
-    mtx_inp = inputs[:-1]
-    sky_dir = inputs[-1]
-    sky_files = (os.path.join(sky_dir, i) for i in os.listdir(sky_dir))
-    grouped = [mtx_inp+[skv] for skv in sky_files]
-    [sub.append(out_dir) for sub in grouped]
-    process.map(dctimestep, grouped)
-
-
-def pcombop(inputs, out_dir, nproc=1):
-    """
-    inputs(list): e.g.[inpdir1,'+',inpdir2,'-',inpdir3]
-    out_dir: output directory
-    """
-    if not os.path.isdir(out_dir):
-        os.makedirs(out_dir)
-    nproc = mp.cpu_count() if nproc is None else nproc
-    process = mp.Pool(nproc)
-    assert len(inputs) > 2
-    assert len(inputs) % 2 == 1
-    inp_dir = [inputs[i] for i in range(0, len(inputs), 2)]
-    inp_cnt = len(inp_dir)
-    ops = [inputs[i] for i in range(1, len(inputs), 2)]
-    inp_lists = []
-    for i in inp_dir:
-        if os.path.isdir(i):
-            inp_lists.append(glob.glob(os.path.join(i, '*.hdr')))
-        else:
-            inp_lists.append(i)
-    inp_lists_full = []
-    for i in range(inp_cnt):
-        if os.path.isdir(inp_dir[i]):
-            inp_lists_full.append(inp_lists[i])
-        else:
-            inp_lists_full.append(inp_dir[i])
-    max_len = sorted([len(i) for i in inp_lists_full if type(i) == list])[0]
-    for i in range(len(inp_lists_full)):
-        if type(inp_lists_full[i]) is not list:
-            inp_lists_full[i] = [inp_lists_full[i]] * max_len
-    equal_len = all(len(i) == len(inp_lists_full[0]) for i in inp_lists_full)
-    if not equal_len:
-        logger.warning("Input directories don't the same number of files")
-    grouped = [list(i) for i in zip(*inp_lists_full)]
-    [sub.insert(i, ops[int((i-1)/2)])
-     for sub in grouped for i in range(1, len(sub)+1, 2)]
-    [sub.append(out_dir) for sub in grouped]
-    process.map(pcomb, grouped)
-
-
-def rpxop():
-    """Operate on input directories given a operation type."""
-    PROGRAM_SCRIPTION = "Image operations with parallel processing"
-    parser = argparse.ArgumentParser(
-        prog='imgop', description=PROGRAM_SCRIPTION)
-    parser.add_argument('-t', type=str, required=True,
-                        choices=['dcts', 'pcomb'],
-                        help='operation types: {pcomb|dcts}')
-    parser.add_argument('-i', type=str, required=True,
-                        nargs="+", help='list of inputs')
-    parser.add_argument('-o', type=str, required=True, help="output directory")
-    parser.add_argument('-n', type=int, help='number of processors to use')
-    args = parser.parse_args()
-    if args.t == "pcomb":
-        pcombop(args.i, args.o, nproc=args.n)
-    elif args.t == 'dcts':
-        dctsop(args.i, args.o, nproc=args.n)
-
-
-def combine_mtx(mtxs, out_dir):
-    """."""
-    cmd = "rmtxop"
-    args = " -ff %s > %s" % (" ".join(mtxs), out_dir)
-    process = sp.Popen(cmd + args, stdout=sp.PIPE, stderr=sp.PIPE, shell=True)
-    _, stderr = process.communicate()
-    return stderr
+logger: logging.Logger = logging.getLogger("frads.sky")
+
+# Solar disk solid angle (sr)
+SOLAR_SA = 6.7967e-5
 
 
-def mtxstr2nparray(data_str: bytes):
-    """Convert Radiance 3-channel matrix file to numpy array.
+def basis_glow(sky_basis: str) -> str:
+    """
+    Generate a set of regular sky and ground glow primitives string.
 
     Args:
-        data_str: file data string
+        sky_basis(str): sky sampling basis, e.g. r1, r4
+    Returns:
+        ground and sky glow string, usually used for rfluxmtx calls.
+    """
+    grnd_str = grndglow()
+    sky_str = skyglow(sky_basis)
+    return grnd_str + sky_str
 
+
+def skyglow(basis: str, upvect: str = "+Y") -> str:
+    """
+    Generate a set of skyglow string
+
+    Args:
+        basis(str): e.g., r1, r2, r4
+        upvect(str): Optional, default=+Y
     Returns:
-        RGB numpy arrays
+        A set of sky glow primitive string
     """
-    if not data_str.startswith(b"#?RADIANCE"):
-        raise ValueError("No header found")
-    if b"\r\n\r\n" in data_str:
-        linesep2 = b"\r\n\r\n"
-    else:
-        linesep2 = b"\n\n"
-    chunks = data_str.split(linesep2)
-    nrow, ncol, ncomp, dtype = parse_rad_header(chunks[0].decode())
-    if dtype == 'ascii':
-        data = np.array(
-            [line.split() for line in chunks[1].splitlines()], dtype=float)
-    else:
-        if dtype == 'float':
-            data = np.frombuffer(chunks[1], np.single).reshape(nrow, ncol * ncomp)
-        elif dtype == 'double':
-            data = np.frombuffer(chunks[1], np.double).reshape(nrow, ncol * ncomp)
-        else:
-            raise ValueError("Unsupported data type %s" % dtype)
-    rdata = data[:, ::ncomp]
-    gdata = data[:, 1::ncomp]
-    bdata = data[:, 2::ncomp]
-    if (len(bdata) != nrow) or (len(bdata[0]) != ncol):
-        raise ValueError("Parsing matrix file failed")
-    return rdata, gdata, bdata
-
-
-def smx2nparray(data_str):
-    """Convert Radiance sky matrix file to numpy array.
-    """
-    if not data_str.startswith(b"#?RADIANCE"):
-        raise ValueError("No header found")
-    if b"\r\n\r\n" in data_str:
-        linesep2 = b"\r\n\r\n"
-    else:
-        linesep2 = b"\n\n"
-    chunks = data_str.split(linesep2)
-    header_str = chunks[0].decode()
-    content = chunks[1:]
-    nrow, ncol, ncomp, dtype = parse_rad_header(header_str)
-    if dtype == 'ascii':
-        data = [i.splitlines() for i in content if i != b'']
-        rdata = np.array([[i.split()[::ncomp][0] for i in row] for row in data],
-                         dtype=float)
-        gdata = np.array([[i.split()[1::ncomp][0] for i in row] for row in data],
-                         dtype=float)
-        bdata = np.array([[i.split()[2::ncomp][0] for i in row] for row in data],
-                         dtype=float)
-    else:
-        if dtype == 'float':
-            data = np.frombuffer(b"\n\n".join(content), np.single).reshape(
-                nrow, ncol * ncomp)
-        elif dtype == 'double':
-            data = np.frombuffer(b"\n\n".join(content), np.double).reshape(
-                nrow, ncol * ncomp)
-        else:
-            raise ValueError("Unsupported data type %s" % dtype)
-        rdata = data[:, 0::ncomp]
-        gdata = data[:, 1::ncomp]
-        bdata = data[:, 2::ncomp]
-    if ncol == 1:
-        assert np.size(bdata, 1) == nrow
-        assert np.size(bdata, 0) == ncol
-        rdata = rdata.T
-        gdata = gdata.T
-        bdata = bdata.T
-    else:
-        assert np.size(bdata, 0) == nrow
-        assert np.size(bdata, 1) == ncol
-    return rdata, gdata, bdata
-
-
-def numpy_mtxmult(mtxs, weight=None):
-    """Matrix multiplication with Numpy."""
-    weight = (47.4, 119.9, 11.6) if weight is None else weight
-    resr = np.linalg.multi_dot([mat[0] for mat in mtxs]) * weight[0]
-    resg = np.linalg.multi_dot([mat[1] for mat in mtxs]) * weight[1]
-    resb = np.linalg.multi_dot([mat[2] for mat in mtxs]) * weight[2]
-    return resr + resg + resb
-
-
-def rad_mtxmult3(*mtxs, weights: tuple = (), no_header=True):
-    """Multiply matrices using dctimstep,
-    Applying weights using rmtxop and remove header if needed.
+    sky_string = f"#@rfluxmtx u={upvect} h={basis}\n\n"
+    sky_string += "void glow skyglow\n"
+    sky_string += "0\n0\n4 1 1 1 0\n\n"
+    sky_string += "skyglow source sky\n"
+    sky_string += "0\n0\n4 0 0 1 180\n"
+    return sky_string
 
+
+def grndglow(basis: str = "u") -> str:
+    """
+    Generate a set of ground string
     Args:
-        mtx: Radiance matrices file paths
-        weights: weight for the three channels
-        no_header: whether to remove header from output
+        basis(str): Optional default=u
+    Returns:
+        A set of ground glow primitive string
+    """
+    ground_string = f"#@rfluxmtx h={basis}\n\n"
+    ground_string += "void glow groundglow\n"
+    ground_string += "0\n0\n4 1 1 1 0\n\n"
+    ground_string += "groundglow source ground\n"
+    ground_string += "0\n0\n4 0 0 -1 180\n\n"
+    return ground_string
+
+
+def gen_sun_source_full(mf: int) -> Tuple[str, str]:
+    """
+    Generate a full set of sun light sources according to Reinhart basis.
 
+    Args:
+        mf(int): multiplication factor, usually 1, 2, or 4.
     Returns:
-        output as byte strings
+        A tuple of full set of sun light and source primitive string
+        and associated modifier string.
+    """
+    runlen = 144 * mf**2 + 3
+    mod_str = os.linesep.join([f"sol{i}" for i in range(1, runlen)])
+    dirs, omgs = utils.calc_reinsrc_dir(mf)
+    lines = []
+    for i, d in enumerate(dirs):
+        lines.append(
+            f"void light sol{i} 0 0 3 1 1 1 sol{i} source sun "
+            f"0 0 4 {d.x:.6g} {d.y:.6g} {d.z:.6g} 0.533"
+        )
+    return os.linesep.join(lines) + os.linesep, mod_str
+
+
+def gen_sun_source_culled(
+    mf,
+    smx_path: Optional[Path] = None,
+    window_normals: Optional[List[geom.Vector]] = None,
+) -> Tuple[str, str, str]:
+    """
+    Generate a culled set of sun sources based on either window orientation
+    and/or climate-based sky matrix. The reduced set of sun sources will
+    significantly speed up the direct-sun matrix generation.
 
-    Raises:
-        Only works with four or two matrices.
+    Args:
+        mf(int): multiplication factor, usually 1, 2, or 4.
+        smx_path(str): Optional, sky matrix path, usually the output of gendaymtx
+        window_normals(str): Optional, window normals
+    Returns:
+        A tuple of culled set of sun light and source primitive string,
+        corresponding modifier strings, and the full set of modifier string.
     """
-    if len(mtxs) not in (2, 4):
-        raise ValueError("Only works with two or four matrices")
-    if os.path.isfile(mtxs[-1]):
-        cmd1 = ['dctimestep', '-od'] + list(mtxs)
-        inp1 = None
+    runlen = 144 * mf**2 + 3
+    dirs, omgs = utils.calc_reinsrc_dir(mf)
+    full_mod_str = os.linesep.join([f"sol{i}" for i in range(1, runlen)])
+    win_norm = []
+    if smx_path is not None:
+        cmd1 = ["rmtxop", "-ff", "-c", ".3", ".6", ".1", "-t", str(smx_path)]
+        cmd2 = ["getinfo", "-"]
+        cmd3 = ["total", f"-if{runlen-1}", "-t,"]
+        proc1 = sp.run(cmd1, check=True, stdout=sp.PIPE)
+        proc2 = sp.run(cmd2, check=True, input=proc1.stdout, stdout=sp.PIPE)
+        proc3 = sp.run(cmd3, check=True, input=proc2.stdout, stdout=sp.PIPE)
+        dtot = [float(i) for i in proc3.stdout.split(b",")]
     else:
-        cmd1 = ['dctimestep', '-od'] + list(mtxs)[:-1]
-        inp1 = mtxs[-1].encode()
-    if weights == ():
-        weights = (47.4, 119.9, 11.6)
-        logger.warning("Using default photopic RGB weights")
-    cmd2 = ['rmtxop', '-fa', '-c', str(weights[0]),
-            str(weights[1]), str(weights[2]), '-', '-t']
-    out1 = sp.Popen(cmd1, stdin=inp1, stdout=sp.PIPE)
-    out2 = sp.Popen(cmd2, stdin=out1.stdout, stdout=sp.PIPE)
-    out1.stdout.close()
-    if no_header:
-        cmd3 = ['getinfo', '-']
-        out3 = sp.Popen(cmd3, stdin=out2.stdout, stdout=sp.PIPE)
-        out2.stdout.close()
-        out = out3.communicate()[0]
+        dtot = [1] * runlen
+    out_lines = []
+    mod_str = []
+    if window_normals is not None:
+        win_norm = window_normals
+        for i, d in enumerate(dirs):
+            _mod = "sol" + str(i)
+            v = 0
+            if dtot[i] > 0:
+                for norm in win_norm:
+                    if norm * d < 0:
+                        v = 1
+                        mod_str.append(_mod)
+                        break
+            out_lines.append(
+                f"void light sol{i} 0 0 3 {v} {v} {v} sol{i} source sun "
+                f"0 0 4 {d.x:.6g} {d.y:.6g} {d.z:.6g} 0.533"
+            )
     else:
-        out = out2.communicate()[0]
-    return out
-
+        for i, d in enumerate(dirs):
+            _mod = f"sol{i}"
+            v = 0
+            if dtot[i] > 0:
+                v = 1
+                mod_str.append(_mod)
+            out_lines.append(
+                f"void light sol{i} 0 0 3 {v} {v} {v} sol{i} source sun "
+                f"0 0 4 {d.x:.6g} {d.y:.6g} {d.z:.6g} 0.533"
+            )
+    logger.debug(out_lines)
+    logger.debug(mod_str)
+    return os.linesep.join(out_lines), os.linesep.join(mod_str), full_mod_str
+
+
+def gendaymtx(
+    out: Union[str, Path],
+    mf: int,
+    data: Optional[Sequence[WeaData]] = None,
+    meta: Optional[WeaMetaData] = None,
+    wpath: Optional[Path] = None,
+    direct: bool = False,
+    solar: bool = False,
+    onesun: bool = False,
+    rotate: Optional[float] = None,
+    binary: bool = False,
+) -> List[str]:
+    """
+    Call gendaymtx to generate a sky/sun matrix
+    and write results to out.  It takes either a .wea file path
+    or wea data and metadata (defined in frads.types).
+    If both are provided, .wea file path will be used.
 
-def mtxmult(*mtxs):
-    if NUMPY_FOUND:
-        def mtx_parser(fpath):
-            if fpath.endswith('.xml'):
-                raw = util.spcheckout(['rmtxop', fpath])
-            else:
-                with open(fpath, 'rb') as rdr:
-                    raw = rdr.read()
-            return mtxstr2nparray(raw)
-        npmtx = [mtx_parser(mtx) for mtx in mtxs[:-1]]
-        if os.path.isfile(mtxs[-1]):
-            with open(mtxs[-1], 'rb') as rdr:
-                smx_str = rdr.read()
-        else:
-            smx_str = mtxs[-1]
-        npmtx.append(smx2nparray(smx_str))
-        return numpy_mtxmult(npmtx)
+    Args:
+        out(str or pathlib.Path): outpath file path
+        mf(int): multiplication factor
+        data(Sequence[WeaData], optional): A sequence of WeaData.
+        meta(WeaMetaData, optional): A instance of WeaMetaData object.
+        wpath(Path, optional): .wea file path.
+        direct(bool, optional): Whether to generate sun-only sky matrix.
+        solar(bool, optional): Whether to generate sky matrix if solar spectrum.
+        onesun(bool, optional): Whether to generate single sun matrix (five-phase).
+        rotate(float, optional): rotate the sky counter-clock wise, looking down.
+        binary(bool, optional): Whether to have outputs in single precision floats.
+    Returns:
+        cmd(List[str]): the gendaymtx command called.
+    Raises:
+        ValueError: An error occurs if neither a .wea path nor wea data is provided.
+    """
+    stdin = None
+    cmd = ["gendaymtx", "-m", str(mf)]
+    if binary:
+        cmd.append("-of")
+    if direct:
+        cmd.append("-d")
+    if onesun:
+        cmd.extend(["-5", ".533"])
+    if rotate is not None:
+        cmd.extend(["-r", str(rotate)])
+    if solar:
+        cmd.append("-O1")
+    if wpath is not None:
+        cmd.append(str(wpath))
+    elif (data is not None) and (meta is not None):
+        wea_input = meta.wea_header() + "\n".join(map(str, data))
+        stdin = wea_input.encode("utf-8")
     else:
-        return rad_mtxmult3(*mtxs)
+        raise ValueError("Need to specify either .wea path or wea data.")
+    with open(out, "wb") as wtr:
+        logger.info("Calling gendaymtx with:\n%s", " ".join(cmd))
+        sp.run(cmd, check=True, input=stdin, stdout=wtr)
+    return cmd
 
 
-def imgmult(*mtx, odir):
-    """Image-based matrix multiplication using dctimestep."""
-    util.mkdir_p(odir)
-    cmd = ['dctimestep', '-oc', '-o', os.path.join(odir, '%04d.hdr')]
-    cmd += list(mtx)
+def gen_perez_sky(row, meta, grefl: float = 0.2, spect: str = "0", rotate=None) -> str:
+    gendaylit = gendaylit_cmd(
+        str(row.month),
+        str(row.day),
+        str(row.hours),
+        str(meta.latitude),
+        str(meta.longitude),
+        str(meta.timezone),
+        dir_norm_ir=str(row.dni),
+        dif_hor_ir=str(row.dhi),
+    )
+    out = []
+    rot = f"| xform -rz {rotate}" if rotate is not None else ""
+    out.append(f"!{' '.join(gendaylit)}{rot} \n")
+    out.append("skyfunc glow sglow 0 0 4 1 1 1 0\n")
+    out.append("sglow source sky 0 0 4 0 0 1 180\n")
+    out.append("sglow source ground 0 0 4 0 0 -1 180\n")
+    return " ".join(out)
+
+
+def gendaylit_cmd(
+    month: str,
+    day: str,
+    hours: str,
+    lat: str,
+    lon: str,
+    tzone: str,
+    year: str = None,
+    dir_norm_ir: str = None,
+    dif_hor_ir: Optional[str] = None,
+    dir_hor_ir: Optional[str] = None,
+    dir_norm_il: Optional[str] = None,
+    dif_hor_il: str = None,
+    solar: bool = False,
+) -> list:
+    """Get a gendaylit command as a list."""
+    cmd = ["gendaylit", month, day, hours]
+    cmd += ["-a", lat, "-o", lon, "-m", tzone]
+    if year is not None:
+        cmd += ["-y", year]
+    if None not in (dir_norm_ir, dif_hor_ir):
+        cmd += ["-W", str(dir_norm_ir), str(dif_hor_ir)]
+    if None not in (dir_hor_ir, dif_hor_ir):
+        cmd += ["-G", str(dir_hor_ir), str(dif_hor_ir)]
+    if None not in (dir_norm_il, dif_hor_il):
+        cmd += ["-L", str(dir_norm_il), str(dif_hor_il)]
+    if solar:
+        cmd += ["-O", "1"]
     return cmd
 
 
-def dctsnp():
-    """Commandline program that performs matrix multiplication using numpy."""
-    if not NUMPY_FOUND:
-        print("Numpy not found")
-        return
-    aparser = argparse.ArgumentParser(
-        prog='dctsnp',
-        description='dctimestep but using numpy (non-image)')
-    aparser.add_argument('-m', '--mtx', required=True,
-                         nargs='+', help='scene matrix')
-    aparser.add_argument('-s', '--smx', required=True, help='sky matrix')
-    aparser.add_argument('-w', '--weight', type=float, default=None,
-                         nargs=3, help='RGB weights')
-    aparser.add_argument('-o', '--output', required=True, help='output path')
-    args = aparser.parse_args()
-
-    def mtx_parser(fpath):
-        if fpath.endswith('.xml'):
-            raw = util.spcheckout(['rmtxop', fpath])
-        else:
-            with open(fpath, 'rb') as rdr:
-                raw = rdr.read()
-        return mtxstr2nparray(raw)
-    npmtx = [mtx_parser(mtx) for mtx in args.mtx]
-    with open(args.smx, 'rb') as rdr:
-        npmtx.append(smx2nparray(rdr.read()))
-    result = numpy_mtxmult(npmtx, weight=args.weight)
-    np.savetxt(args.output, result)
+def solar_angle(
+    lat: float,
+    lon: float,
+    mer: float,
+    month,
+    day: int,
+    hour,
+) -> Tuple[float, float]:
+    """
+    Simplified translation from the Radiance sun.c and gensky.c code.
+    """
+    latitude_r = math.radians(lat)
+    longitude_r = math.radians(lon)
+    s_meridian = math.radians(mer)
+    mo_da = [0, 31, 59, 90, 120, 151, 181, 212, 243, 273, 304, 334]
+
+    julian_date = mo_da[month - 1] + day
+
+    solar_decline = 0.4093 * math.sin((2 * math.pi / 365) * (julian_date - 81))
+
+    solar_time = hour + (
+        0.170 * math.sin((4 * math.pi / 373) * (julian_date - 80))
+        - 0.129 * math.sin((2 * math.pi / 355) * (julian_date - 8))
+        + (12 / math.pi) * (s_meridian - longitude_r)
+    )
+    altitude = math.asin(
+        math.sin(latitude_r) * math.sin(solar_decline)
+        - math.cos(latitude_r)
+        * math.cos(solar_decline)
+        * math.cos(solar_time * (math.pi / 12))
+    )
+    azimuth = -math.atan2(
+        math.cos(solar_decline) * math.sin(solar_time * (math.pi / 12.0)),
+        -math.cos(latitude_r) * math.sin(solar_time)
+        - math.sin(latitude_r)
+        * math.cos(solar_decline)
+        * math.cos(solar_time * (math.pi / 12)),
+    )
+
+    return altitude, azimuth
+
+
+def start_end_hour(data: Sequence[WeaData], sh: float, eh: float) -> Sequence[WeaData]:
+    """Remove wea data entries outside of the
+    start and end hour."""
+    if sh == 0 and eh == 0:
+        return data
+    return [row for row in data if sh <= (row.time.hour + row.time.minute / 60) <= eh]
+
+
+def check_sun_above_horizon(data, metadata):
+    """Remove non-daylight hour entries."""
+
+    def solar_altitude_check(row: WeaData):
+        alt, _ = solar_angle(
+            metadata.latitude,
+            metadata.longitude,
+            metadata.timezone,
+            row.time.month,
+            row.time.day,
+            row.time.hour + row.time.minute / 60,
+        )
+        return alt > 0
+
+    return [row for row in data if solar_altitude_check(row)]
+
+
+def filter_data_with_zero_dni(data):
+    """Filter out data entries with zero direct normal irradiance."""
+    return [row for row in data if row.dni != 0]
+
+
+def solar_minute(data: WeaData) -> int:
+    # assuming never leap year
+    mo_da = [0,31,59,90,120,151,181,212,243,273,304,334]
+    jd = mo_da[data.time.month - 1] + data.time.day
+    return 24 * 60 * (jd - 1) + int(data.time.hour * 60.0 + data.time.minute + 0.5)
+
+
+def filter_data_by_direct_sun(
+    data: Sequence[WeaData],
+    meta: WeaMetaData,
+    window_normal: Optional[Sequence[geom.Vector]] = None,
+) -> List[WeaData]:
+    """
+    Remove wea data entries with zero solar luminance according to
+    Perez All-Weather sky model. If window normal supplied,
+    eliminate entries not seen by window. Window field of view
+    is 176 deg with 2 deg tolerance on each side.
+
+    Args:
+        data: Sequence[WeaData],
+        meta: WeaMetaData,
+        window_normal: Optional[Sequence[geom.Vector]] = None,
+    Returns:
+        data(List[WeaData]):
+    """
+    wea_input = meta.wea_header() + "\n".join(map(str, data))
+    proc = sp.run(
+        ["gendaymtx", "-u", "-D", "-"],
+        check=True,
+        input=wea_input,
+        encoding="ascii",
+        stderr=sp.PIPE,
+        stdout=sp.PIPE,
+    )
+    prims = parsers.parse_primitive(proc.stdout.splitlines())
+    light_prims = [prim for prim in prims if prim.ptype == "light"]
+    keep_minutes = []
+    if window_normal is not None:
+        source_prims = [prim for prim in prims if prim.ptype == "source"]
+        for lpr, spr in zip(light_prims, source_prims):
+            if lpr.real_arg[1] > 0:
+                sdir = geom.Vector(*spr.real_arg[1:4])
+                for normal in window_normal:
+                    if normal * sdir < -0.035:  # 2deg tolerance
+                        keep_minutes.append(int(spr.modifier.lstrip("solar")))
+                        break
+    else:
+        for lpr in light_prims:
+            if lpr.real_arg[1] > 0:
+                keep_minutes.append(int(lpr.identifier.lstrip("solar")))
+    # inminutes = [solar_minute(d) for d in data]
+    inminutes = []
+    extra_day = 0
+    for d in data:
+        inm = solar_minute(d)
+        if d.time.month == 2 and d.time.day == 29:
+            extra_day = 1440
+        inm += extra_day
+        inminutes.append(inm)
+    new_dataline = [data for data, minu in zip(data, inminutes) if minu in keep_minutes]
+    return new_dataline
+
+
+def filter_wea(
+    wea_data: List[WeaData],
+    meta_data: WeaMetaData,
+    start_hour: Optional[float] = None,
+    end_hour: Optional[float] = None,
+    daylight_hours_only: bool = False,
+    remove_zero: bool = False,
+    window_normals: Optional[List[geom.Vector]] = None,
+) -> Tuple[List[WeaData], List[Any]]:
+    """
+    Obtain and prepare weather file data.
+
+    Args:
+        wea_data(List[WeaData]): A list of WeaData.
+        meta_data(WeaMetaData): A instance of WeaMetaData object.
+        start_hour(float, optional): Filter out wea data before this hour.
+        end_hour(float, optional): Filter out wea data after this hour.
+        daylight_hours_only(bool, optional): Filter out wea data below horizon.
+        remove_zero(bool, optional): Filter out wea data with zero DNI.
+        window_normals(List[geom.Vector], optional): Filter out wea data with direct
+            sun not seen by these window normals.
+    Returns:
+        wea_data(List[WeaData]): Filterd list of wea data
+        datetime_stamps(list): Remaining datetime stamps
+    """
+    logger.info("Filtering wea data, starting with %d rows", len(wea_data))
+    if (start_hour is not None) and (end_hour is not None):
+        wea_data = start_end_hour(wea_data, start_hour, end_hour)
+        logger.info(
+            "Filtering out hours outside of %f and %f: %d rows remaining",
+            start_hour,
+            end_hour,
+            len(wea_data),
+        )
+    if daylight_hours_only:
+        wea_data = check_sun_above_horizon(wea_data, meta_data)
+        logger.info("Filtering by daylight hours: %d rows remaining", len(wea_data))
+    if remove_zero:
+        wea_data = filter_data_with_zero_dni(wea_data)
+    if window_normals is not None:
+        wea_data = filter_data_by_direct_sun(
+            wea_data, meta_data, window_normal=window_normals
+        )
+        logger.info(
+            "Filtering zero DNI hours and suns not seen by window: %d rows remaining",
+            len(wea_data),
+        )
+    datetime_stamps = [str(row) for row in wea_data]
+    if len(wea_data) == 0:
+        logger.warning("Empty wea file")
+    return wea_data, datetime_stamps
```

### Comparing `frads-0.2.3/frads/radgeom.py` & `frads-0.2.8/frads/geom.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """
-Utilities for handling geometries.
+This module contains definitions of Vector and Polygon objects
+and other geometry related routines.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 import math
+from typing import Union
 from typing import List
+from typing import Tuple
+from typing import Sequence
 
 
 @dataclass(frozen=True)
 class Vector:
     """3D vector class.
 
     Attributes:
         x: x coordinate
         y: y coordinate
         z: z coordinate
-        length: length of the vector
     """
+
     x: float = 0
     y: float = 0
     z: float = 0
 
-    def __post_init__(self):
-        """Initialize vector."""
-
     def __str__(self) -> str:
         """Class string representation.
 
         Returns:
             The string representation of the vector(str)
 
         """
-        return "{:02f} {:02f} {:02f}".format(self.x, self.y, self.z)
+        return f"{self.x:02f} {self.y:02f} {self.z:02f}"
 
     def __add__(self, other) -> Vector:
         """Add the two vectors.
         Args:
             other(Vector): vector to add
 
         Returns:
@@ -49,66 +50,59 @@
     def __sub__(self, other: Vector) -> Vector:
         return Vector(self.x - other.x, self.y - other.y, self.z - other.z)
 
     def __mul__(self, other: Vector) -> float:
         """Return the dot produce between two vectors."""
         return self.x * other.x + self.y * other.y + self.z * other.z
 
-    def __eq__(self, other: object) -> bool:
-        """Check if two vectors are the same."""
-        if not isinstance(other, Vector):
-            return NotImplemented
-        return (self.x, self.y, self.z) == (other.x, other.y, other.z)
-
-    def __hash__(self):
-        return hash((self.x, self.y, self.z))
-
-    def length(self):
+    @property
+    def length(self) -> float:
+        """Get vector distance from origin."""
         return math.sqrt(self.x**2 + self.y**2 + self.z**2)
 
     def cross(self, other: Vector) -> Vector:
         """Return the cross product of the two vectors.
 
         Args:
             other: the vector to take a cross product
 
         Returns:
             The resulting vector
 
         """
-        x_ = self.y * other.z - self.z * other.y
-        y_ = self.z * other.x - self.x * other.z
-        z_ = self.x * other.y - self.y * other.x
-        return Vector(x_, y_, z_)
+        return Vector(
+            self.y * other.z - self.z * other.y,
+            self.z * other.x - self.x * other.z,
+            self.x * other.y - self.y * other.x,
+        )
 
-    def distance_from(self, other: Vector):
+    def distance_from(self, other: Vector) -> float:
         """Calculate the distance between two points."""
         dx = math.fabs(self.x - other.x)
         dy = math.fabs(self.y - other.y)
         dz = math.fabs(self.z - other.z)
         return math.sqrt(dx**2 + dy**2 + dz**2)
 
     def normalize(self) -> Vector:
         """Return the unit vector."""
         magnitude = math.sqrt(self.x**2 + self.y**2 + self.z**2)
-        return Vector(self.x / magnitude, self.y / magnitude,
-                      self.z / magnitude)
+        return Vector(self.x / magnitude, self.y / magnitude, self.z / magnitude)
 
     def reverse(self) -> Vector:
         """Return the reversed vector."""
         return Vector(self.x * -1, self.y * -1, self.z * -1)
 
-    def scale(self, factor) -> Vector:
+    def scale(self, factor: float) -> Vector:
         """Scale the vector by a scalar."""
         return Vector(self.x * factor, self.y * factor, self.z * factor)
 
-    def angle_from(self, other) -> float:
+    def angle_from(self, other: "Vector") -> float:
         """."""
         dot_prod = self * other
-        angle = math.acos(dot_prod / (self.length() * other.length()))
+        angle = math.acos(dot_prod / (self.length * other.length))
         return angle
 
     def rotate_3d(self, vector: Vector, theta: float) -> Vector:
         """Rotate the point around the vector theta radians.
 
         Args:
             vector: rotation axis
@@ -116,138 +110,178 @@
         Returns:
             the rotated point
 
         """
         cosa = math.cos(theta)
         sina = math.sin(theta)
 
-        row1 = [(vector.x * vector.x) + ((1 - (vector.x * vector.x)) * cosa),
-                (vector.x * vector.y * (1 - cosa)) - (vector.z * sina),
-                (vector.x * vector.z * (1 - cosa)) + (vector.y * sina), 0.0]
-        row2 = [(vector.x * vector.y * (1 - cosa)) + (vector.z * sina),
-                (vector.y * vector.y) + ((1 - (vector.y * vector.y)) * cosa),
-                (vector.y * vector.z * (1 - cosa)) - (vector.x * sina), 0.0]
-        row3 = [(vector.x * vector.z * (1.0 - cosa)) - (vector.y * sina),
-                (vector.y * vector.z * (1.0 - cosa)) + (vector.x * sina),
-                (vector.z * vector.z) + ((1.0 - (vector.z * vector.z)) * cosa),
-                0.0]
+        row1 = [
+            (vector.x * vector.x) + ((1 - (vector.x * vector.x)) * cosa),
+            (vector.x * vector.y * (1 - cosa)) - (vector.z * sina),
+            (vector.x * vector.z * (1 - cosa)) + (vector.y * sina),
+            0.0,
+        ]
+        row2 = [
+            (vector.x * vector.y * (1 - cosa)) + (vector.z * sina),
+            (vector.y * vector.y) + ((1 - (vector.y * vector.y)) * cosa),
+            (vector.y * vector.z * (1 - cosa)) - (vector.x * sina),
+            0.0,
+        ]
+        row3 = [
+            (vector.x * vector.z * (1.0 - cosa)) - (vector.y * sina),
+            (vector.y * vector.z * (1.0 - cosa)) + (vector.x * sina),
+            (vector.z * vector.z) + ((1.0 - (vector.z * vector.z)) * cosa),
+            0.0,
+        ]
 
         row4 = [0.0] * 4
 
-        rx = (self.x * row1[0]) + (self.y * row2[0]) + (self.z *
-                                                        row3[0]) + row4[0]
-        ry = (self.x * row1[1]) + (self.y * row2[1]) + (self.z *
-                                                        row3[1]) + row4[1]
-        rz = (self.x * row1[2]) + (self.y * row2[2]) + (self.z *
-                                                        row3[2]) + row4[2]
+        rx = (self.x * row1[0]) + (self.y * row2[0]) + (self.z * row3[0]) + row4[0]
+        ry = (self.x * row1[1]) + (self.y * row2[1]) + (self.z * row3[1]) + row4[1]
+        rz = (self.x * row1[2]) + (self.y * row2[2]) + (self.z * row3[2]) + row4[2]
 
         return Vector(rx, ry, rz)
 
     def to_sphr(self):
         """Convert cartesian to spherical coordinates."""
         r = self.distance_from(Vector())
         theta = math.atan(self.y / self.x)
         phi = math.acos(self.z / r)
         return theta, phi, r
 
-    def coplanar(self, other1, other2):
+    def coplanar(self, other1, other2) -> bool:
         """Test if the vector is coplanar with the other two vectors."""
         triple_prod = self * other1.cross(other2)
-        return triple_prod==0
+        return triple_prod == 0
 
-    def to_list(self):
+    def to_list(self) -> List[float]:
         """Return a list containing the coordinates."""
         return [self.x, self.y, self.z]
 
-    def to_tuple(self):
-        """Return a tuple containing the coordinates, and round to third decimal place."""
-        return (round(self.x,3), round(self.y, 3), round(self.z, 3))
+    def to_tuple(self) -> Tuple[float, ...]:
+        """Return a tuple containing the coordinates."""
+        return self.x, self.y, self.z
 
     @classmethod
-    def spherical(cls, theta, phi, r) -> Vector:
+    def spherical(
+        cls,
+        theta: float,
+        phi: float,
+        r: float,
+    ) -> Vector:
         """Construct a vector using spherical coordinates."""
         xcoord = math.sin(theta) * math.cos(phi) * r
         ycoord = math.sin(theta) * math.sin(phi) * r
         zcoord = math.cos(theta) * r
         return cls(xcoord, ycoord, zcoord)
 
 
+@dataclass(frozen=True)
 class Polygon:
-    """3D polygon class."""
+    """3D polygon class
 
-    def __init__(self, vertices):
+    Attributes:
+        vertices(List[Vector]): list of vertices of the polygon.
+    """
+
+    vertices: Tuple[Vector]
+
+    def __post_init__(self) -> None:
         """."""
-        self.vert_cnt = len(vertices)
-        assert self.vert_cnt > 2, "Need more than 2 vertices to make a polygon."
-        self.vertices = vertices
+        if len(self.vertices) < 3:
+            raise ValueError("Need more than 2 vertices to make a polygon.")
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Polygon):
+            return NotImplemented
+        if len(other.vertices) != len(self.vertices):
+            return False
+        for vert in self.vertices:
+            if vert not in other.vertices:
+                return False
+        return True
+
+    def __add__(self, other: Polygon) -> Polygon:
+        """Merge two polygons."""
+        sp, index = self.shared_pts(other)
+        if sp != 2:
+            raise ValueError("Trying to merge two polygons without shared sides")
+        t1 = self.vertices[index[0] :] + self.vertices[: index[0]]
+        oid = other.vertices.index(self.vertices[index[0]])
+        t2 = other.vertices[oid:] + other.vertices[:oid]
+        if t1[-1] == t2[1]:
+            return Polygon(t1 + t2[2:])
+        return Polygon(t2 + t1[2:])
 
     def __sub__(self, other: Polygon) -> Polygon:
         """Polygon subtraction.
 
         Args:
             other: subtract this polygon
 
         Returns:
             Clipped polygon (Polygon)
 
         """
         pt1 = self.vertices[0]
-        #opposite = False if self.normal() == other.normal() else True
+        # opposite = False if self.normal() == other.normal() else True
         opposite = False
         distances1 = [pt1.distance_from(i) for i in other.vertices]
         idx_min = distances1.index(min(distances1))
         new_other_vert = other.vertices[idx_min:] + other.vertices[:idx_min]
         results = [pt1]
         if opposite:
             results.extend(new_other_vert)
             results.append(other.vertices[idx_min])
         else:
             results.append(new_other_vert[0])
             results.extend(reversed(new_other_vert[1:]))
             results.append(new_other_vert[0])
         results.extend(self.vertices)
-        return Polygon(results)
-
-    def flip(self):
-        """Reverse the vertices order, thus reversing the normal."""
-        return Polygon([self.vertices[0]] + self.vertices[:0:-1])
+        return Polygon(tuple(results))
 
-    def normal(self):
+    @property
+    def normal(self) -> Vector:
         """Calculate the polygon normal."""
-        vect21 = self.vertices[1] - self.vertices[0]
-        vect32 = self.vertices[2] - self.vertices[1]
-        normal = vect21.cross(vect32)
-        normal_u = normal.normalize()
-        return normal_u
+        normal = Vector(0, 0, 0)
+        for idx in range(len(self.vertices) - 2):
+            normal += (self.vertices[idx + 1] - self.vertices[idx]).cross(
+                self.vertices[idx + 2] - self.vertices[idx + 1]
+            )
+        return normal.normalize()
 
-    def centroid(self):
+    @property
+    def centroid(self) -> Vector:
         """Return the geometric center point."""
-        return sum(self.vertices, Vector()).scale(1 / self.vert_cnt)
+        return sum(self.vertices, Vector()).scale(1 / len(self.vertices))
 
-    def area(self):
-        """Calculate the area of the polygon.
+    @property
+    def area(self) -> float:
+        """Calculate the area of the polygon."""
+        total = Vector(0, 0, 0)
+        for idx in range(1, len(self.vertices) - 1):
+            total += (self.vertices[idx] - self.vertices[0]).cross(
+                self.vertices[idx + 1] - self.vertices[0]
+            )
+        return abs(total * Vector(0.5, 0.5, 0.5))
 
-        Returns:
-            polygon area(float)
-
-        """
+    @property
+    def extreme(self) -> Tuple[float, ...]:
+        """."""
+        xs = [v.x for v in self.vertices]
+        ys = [v.y for v in self.vertices]
+        zs = [v.z for v in self.vertices]
+        return min(xs), max(xs), min(ys), max(ys), min(zs), max(zs)
 
-        total = Vector()
-        for i in range(self.vert_cnt):
-            vect1 = self.vertices[i]
-            if i == self.vert_cnt - 1:
-                vect2 = self.vertices[0]
-            else:
-                vect2 = self.vertices[i + 1]
-            prod = vect1.cross(vect2)
-            total += prod
-        area = abs(total * self.normal() / 2)
-        return area
+    def flip(self) -> "Polygon":
+        """Reverse the vertices order, thus reversing the normal."""
+        return Polygon(self.vertices[::-1])
+        # return Polygon([self.vertices[0]] + self.vertices[:0:-1])
 
-    def scale(self, scale_vect, center):
+    def scale(self, scale_vect, center) -> "Polygon":
         """Scale the polygon.
 
         Parameters:
             scale_vect (Vector): scale along x, y, z;
             center (Vector): center of scaling
         Return:
             Scaled polygon (Polygon)
@@ -255,107 +289,105 @@
         """
         new_vertices = []
         for vert in self.vertices:
             sx = center.x + (vert.x - center.x) * scale_vect.x
             sy = center.y + (vert.y - center.y) * scale_vect.y
             sz = center.z + (vert.z - center.z) * scale_vect.z
             new_vertices.append(Vector(sx, sy, sz))
-        return Polygon(new_vertices)
+        return Polygon(tuple(new_vertices))
 
     def extrude(self, vector: Vector) -> list:
         """Extrude the polygon.
 
         Args:
             vector (Vector): extrude along the vector;
 
         Returns:
             Polygon (list): a list of polygons;
 
         """
         polygons = [self]
-        polygon2 = Polygon([i + vector for i in self.vertices])
+        polygon2 = Polygon(([i + vector for i in self.vertices]))
         polygons.append(polygon2)
         for i in range(len(self.vertices) - 1):
             polygons.append(
-                Polygon([self.vertices[i], polygon2.vertices[i],
-                         polygon2.vertices[i + 1], self.vertices[i + 1]]))
+                Polygon(
+                    (
+                        self.vertices[i],
+                        polygon2.vertices[i],
+                        polygon2.vertices[i + 1],
+                        self.vertices[i + 1],
+                    )
+                )
+            )
         polygons.append(
-            Polygon([self.vertices[-1], polygon2.vertices[-1],
-                     polygon2.vertices[0], self.vertices[0]]))
+            Polygon(
+                (
+                    self.vertices[-1],
+                    polygon2.vertices[-1],
+                    polygon2.vertices[0],
+                    self.vertices[0],
+                )
+            )
+        )
         return polygons
 
-    def __add__(self, other: Polygon) -> Polygon:
-        """Merge two polygons."""
-        sp, index = self.shared_pts(other)
-        if sp != 2:
-            raise ValueError(
-                "Trying to merge two polygons without shared sides")
-        t1 = self.vertices[index[0]:] + self.vertices[:index[0]]
-        oid = other.vertices.index(self.vertices[index[0]])
-        t2 = other.vertices[oid:] + other.vertices[:oid]
-        if t1[-1] == t2[1]:
-            return Polygon(t1 + t2[2:])
-        return Polygon(t2 + t1[2:])
-
-    def shared_pts(self, other):
+    def shared_pts(self, other) -> Tuple[int, List[int]]:
         """Return the total number of share points between two polygons."""
         cnt = 0
         index = []
-        for pid in range(len(self.vertices)):
-            if self.vertices[pid].to_list() in other.to_list():
+        for pid, val in enumerate(self.vertices):
+            if val.to_list() in other.to_list():
                 cnt += 1
                 index.append(pid)
         return cnt, index
 
-    def rotate(self, vector, angle):
+    def rotate(self, vector, angle) -> "Polygon":
         """."""
         ro_pts = [v.rotate_3d(vector, angle) for v in self.vertices]
         return Polygon(ro_pts)
 
-    def move(self, vector):
+    def move(self, vector) -> "Polygon":
         """Return the moved polygon along a vector."""
         mo_pts = [v + vector for v in self.vertices]
         return Polygon(mo_pts)
 
-    def extreme(self):
-        """."""
-        xs = [v.x for v in self.vertices]
-        ys = [v.y for v in self.vertices]
-        zs = [v.z for v in self.vertices]
-        return min(xs), max(xs), min(ys), max(ys), min(zs), max(zs)
-
     def to_list(self):
         """Return a list of tuples."""
         return [p.to_tuple() for p in self.vertices]
 
-    def to_real(self):
+    def to_real(self) -> Union[List[float], List[int]]:
         """Convert the vertices to real arg string format."""
-        real_str = "{} ".format(3 * len(self.vertices))
-        vert_str = ' '.join([str(i) for i in self.vertices])
-        return real_str + vert_str
+        real_arg = [3 * len(self.vertices)]
+        for vert in self.vertices:
+            real_arg.append(vert.x)
+            real_arg.append(vert.y)
+            real_arg.append(vert.z)
+        return real_arg
 
     @classmethod
-    def rectangle3pts(cls, pt1, pt2, pt3):
+    def rectangle3pts(cls, pt1, pt2, pt3) -> "Polygon":
         """."""
         vect21 = pt2 - pt1
         vect32 = pt3 - pt2
         err_msg = "Three points are not at a right angle"
         assert vect21.angle_from(vect32) == math.pi / 2, err_msg
         vect12 = pt1 - pt2
         pt4 = pt3 + vect12
-        return cls([pt1, pt2, pt3, pt4])
+        return cls((pt1, pt2, pt3, pt4))
 
 
-def convexhull(points: List[Vector], normal: Vector):
+def convexhull(points: List[Vector], normal: Vector) -> Polygon:
     """Convex hull on coplanar points.
 
     Parameters:
         points (list): list of Point;
         normal (Vector): plane's normal
     """
+
     def toleft(u, v, points):
         """."""
         vect2 = v - u
         pts = []
         for p in points:
             vect1 = p - u
             cross_prod = vect1.cross(vect2)
@@ -372,65 +404,95 @@
         vect2 = v - u
         w = min(points, key=lambda p: (p - u).cross(vect2) * normal)
         p1, p2 = toleft(w, v, points), toleft(u, w, points)
         return extend_pts(w, v, p1) + [w] + extend_pts(u, w, p2)
 
     u = min(points, key=lambda p: p.x)
     v = max(points, key=lambda p: p.x)
-    if u.__str__() == v.__str__():
+    if u == v:
         u = min(points, key=lambda p: p.y)
         v = max(points, key=lambda p: p.y)
     left, right = toleft(u, v, points), toleft(v, u, points)
     points = [v] + extend_pts(u, v, left) + [u] + extend_pts(v, u, right)
+    points.append(points[0])
+    points.append(points[1])
+    to_remove = []
+    for i, p in enumerate(points):
+        if i < len(points) - 2:
+            p12 = p.distance_from(points[i + 1])
+            p23 = points[i + 1].distance_from(points[i + 2])
+            p13 = p.distance_from(points[i + 2])
+            if (p12 + p23) == p13:
+                to_remove.append(points[i + 1])
+    points.pop()
+    points.pop()
+    for r in to_remove:
+        points.remove(r)
     return Polygon(points)
 
 
 def polygon_center(*polygons):
     """Calculate the center from polygons."""
     vertices = [v for p in polygons for v in p.vertices]
     return sum(vertices, Vector()).scale(1 / len(vertices))
 
 
-def get_polygon_limits(polygon_list: list, offset=0.0):
+def get_polygon_limits(polygon_list: Sequence[Polygon], offset: float = 0.0):
     """Get the x,y,z limits from a list of polygons."""
-    extreme_list = [p.extreme() for p in polygon_list]
+    extreme_list = [p.extreme for p in polygon_list]
     lim = list(zip(*extreme_list))
     xmin = min(lim[0]) - offset
     xmax = max(lim[1]) + offset
     ymin = min(lim[2]) - offset
     ymax = max(lim[3]) + offset
     zmin = min(lim[4]) - offset
     zmax = max(lim[5]) + offset
     return xmin, xmax, ymin, ymax, zmin, zmax
 
 
-def getbbox(polygons: list, offset: float = 0.0):
+def getbbox(polygons: Sequence[Polygon], offset: float = 0.0):
     """Get a bounding box for a list of polygons.
 
     Return a list of polygon that is the
     orthogonal bounding box of a list of polygon.
 
     Args:
         polygons: list of polygons
         offset: make the box smaller or bigger
 
     Returns:
         A list of polygon that is the bounding box.
     """
-    xmin, xmax, ymin, ymax, zmin, zmax = get_polygon_limits(
-        polygons, offset=offset)
+    xmin, xmax, ymin, ymax, zmin, zmax = get_polygon_limits(polygons, offset=offset)
     fp1 = Vector(xmin, ymin, zmin)
     fp2 = Vector(xmax, ymin, zmin)
     fp3 = Vector(xmax, ymax, zmin)
-    fpg = Polygon.rectangle3pts(fp1, fp2, fp3) #-Z
+    fpg = Polygon.rectangle3pts(fp1, fp2, fp3)  # -Z
     cp1 = Vector(xmin, ymin, zmax)
     cp2 = Vector(xmax, ymin, zmax)
     cp3 = Vector(xmax, ymax, zmax)
-    cpg = Polygon.rectangle3pts(cp3, cp2, cp1) #+Z
-    swpg = Polygon.rectangle3pts(cp2, fp2, fp1) #-Y
-    ewpg = Polygon.rectangle3pts(fp3, fp2, cp2) #+X
+    cpg = Polygon.rectangle3pts(cp3, cp2, cp1)  # +Z
+    swpg = Polygon.rectangle3pts(cp2, fp2, fp1)  # -Y
+    ewpg = Polygon.rectangle3pts(fp3, fp2, cp2)  # +X
     s2n_vec = Vector(0, ymax - ymin, 0)
-    nwpg = Polygon([v + s2n_vec for v in swpg.vertices]).flip() #+Y
+    nwpg = Polygon([v + s2n_vec for v in swpg.vertices]).flip()  # +Y
     e2w_vec = Vector(xmax - xmin, 0, 0)
-    wwpg = Polygon([v - e2w_vec for v in ewpg.vertices]).flip() #-X
+    wwpg = Polygon([v - e2w_vec for v in ewpg.vertices]).flip()  # -X
 
     return [fpg, cpg, ewpg, swpg, wwpg, nwpg]
+
+
+def merge_polygon(polygons: Sequence[Polygon]) -> Polygon:
+    """Merge polygons into a polygon using Convex Hull.
+
+    Args:
+        polygons: Polygons to be merged
+    Returns:
+        Merged polygon
+    Raises:
+        ValueError if window normals are not the same
+    """
+    normals = [p.normal for p in polygons]
+    if len(set(normals)) > 1:
+        raise ValueError("Windows not co-planar")
+    points = [i for p in polygons for i in p.vertices]
+    return convexhull(points, normals[0])
```

### Comparing `frads-0.2.3/frads/radutil.py` & `frads-0.2.8/frads/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,703 +1,710 @@
-"""Utility functions."""
-
-import argparse
-from dataclasses import dataclass, field
-import json
+"""
+This module contains all utility functions used throughout frads.
+"""
+from io import TextIOWrapper
 import logging
 import math
-import os
+from pathlib import Path
+import random
+import string
 import subprocess as sp
-from typing import List, NamedTuple, Set
+from typing import Any, Dict, Optional, List
+from typing import Set
+from typing import Tuple
+from typing import Union
+
+from frads import geom
+from frads import parsers
+from frads.types import Primitive
+from frads.types import PaneRGB
+from frads.types import ScatteringData
+from frads.types import BSDFData
+
 
-from frads import radgeom, radmtx, util
-logger = logging.getLogger("frads.radutil")
+logger: logging.Logger = logging.getLogger("frads.utils")
 
 
-GEOM_TYPE = ['polygon', 'ring', 'tube', 'cone']
+GEOM_TYPE = ["polygon", "ring", "tube", "cone"]
 
-MATERIAL_TYPE = ['plastic', 'glass', 'trans', 'dielectric', 'BSDF']
+MATERIAL_TYPE = ["plastic", "glass", "trans", "dielectric", "BSDF"]
 
 BASIS_DICT = {
-    '145': 'Klems Full',
-    '73': 'Klems Half',
-    '41': 'Klems Quarter',
+    "145": "Klems Full",
+    "73": "Klems Half",
+    "41": "Klems Quarter",
 }
 
 TREG_BASE = [
-    (90., 0),
-    (78., 30),
-    (66., 30),
-    (54., 24),
-    (42., 24),
-    (30., 18),
-    (18., 12),
-    (6., 6),
-    (0., 1),
+    (90.0, 0),
+    (78.0, 30),
+    (66.0, 30),
+    (54.0, 24),
+    (42.0, 24),
+    (30.0, 18),
+    (18.0, 12),
+    (6.0, 6),
+    (0.0, 1),
 ]
 
 ABASE_LIST = {
-    "Klems Full": [(0., 1), (5., 8), (15., 16), (25., 20), (35., 24),
-                   (45., 24), (55., 24), (65., 16), (75., 12), (90., 0)],
-    "Klems Half": [(0., 1), (6.5, 8), (19.5, 12), (32.5, 16), (46.5, 20),
-                   (61.5, 12), (76.5, 4), (90., 0)],
-    "Klems Quarter": [(0., 1), (9., 8), (27., 12), (46., 12), (66., 8),
-                      (90., 0)]
+    "Klems Full": [
+        (0.0, 1),
+        (5.0, 8),
+        (15.0, 16),
+        (25.0, 20),
+        (35.0, 24),
+        (45.0, 24),
+        (55.0, 24),
+        (65.0, 16),
+        (75.0, 12),
+        (90.0, 0),
+    ],
+    "Klems Half": [
+        (0.0, 1),
+        (6.5, 8),
+        (19.5, 12),
+        (32.5, 16),
+        (46.5, 20),
+        (61.5, 12),
+        (76.5, 4),
+        (90.0, 0),
+    ],
+    "Klems Quarter": [(0.0, 1), (9.0, 8), (27.0, 12), (46.0, 12), (66.0, 8), (90.0, 0)],
 }
 
 
-class Primitive(NamedTuple):
-    modifier: str
-    ptype: str
-    identifier: str
-    str_arg: str
-    real_arg: str
-    int_arg: str = '0'
-
-    def __repr__(self) -> str:
-        output = f"{self.modifier} {self.ptype} {self.identifier} "
-        output += f"{self.str_arg} {self.int_arg} {self.real_arg} "
-        return output
-
-    def __str__(self) -> str:
-        if '' in (self.modifier, self.ptype, self.identifier):
-            return ''
-        output = f"\n{self.modifier} {self.ptype} {self.identifier}\n"
-        output += f"{self.str_arg}\n{self.int_arg}\n{self.real_arg}\n"
-        return output
-
-
-@dataclass
-class ScatteringData:
-    sdata: List[List[float]]
-    ncolumn: int = field(init=False)
-    nrow: int = field(init=False)
-    basis: str = field(init=False)
-
-    def __post_init__(self):
-        self.ncolumn = len(self.sdata[0])
-        self.nrow = len(self.sdata)
-        self.basis = BASIS_DICT[str(self.ncolumn)]
-
-    def to_bsdf(self):
-        lambdas = angle_basis_coeff(self.basis)
-        bsdf = [list(map(lambda x, y: x/y, i, lambdas)) for i in self.sdata]
-        return BSDFData(bsdf)
-
-    def __repr__(self) -> str:
-        out = ''
-        for row in self.sdata:
-            for val in row:
-                string = '%07.5f' % val
-                out += string + '\t'
-            out += '\n'
-        return out
-
-    def __str__(self) -> str:
-        out = '#?RADIANCE\nNCOMP=3\n'
-        out += 'NROWS=%d\nNCOLS=%d\n' % (self.nrow, self.ncolumn)
-        out += 'FORMAT=ascii\n\n'
-        for row in self.sdata:
-            for val in row:
-                string = '\t'.join(['%07.5f' % val] * 3)
-                out += string + '\t'
-            out += '\n'
-        return out
-
-
-@dataclass
-class BSDFData:
-    bsdf: List[List[float]]
-    ncolumn: int = field(init=False)
-    nrow: int = field(init=False)
-    basis: str = field(init=False)
-
-    def __post_init__(self):
-        self.ncolumn = len(self.bsdf[0])
-        self.nrow = len(self.bsdf)
-        self.basis = BASIS_DICT[str(self.ncolumn)]
-
-    def to_sdata(self) -> ScatteringData:
-        lambdas = angle_basis_coeff(self.basis)
-        sdata = [list(map(lambda x, y: x/y, i, lambdas))
-                 for i in self.bsdf]
-        return ScatteringData(sdata)
-
-
-@dataclass(frozen=True)
-class RadMatrix:
-    tf: ScatteringData
-    tb: ScatteringData
+def tmit2tmis(tmit: float) -> float:
+    """Convert from transmittance to transmissivity."""
+    tmis = round(
+        (math.sqrt(0.8402528435 + 0.0072522239 * tmit**2) - 0.9166530661)
+        / 0.0036261119
+        / tmit,
+        3,
+    )
+    return max(0, min(tmis, 1))
 
 
-def parse_primitive(lines: list) -> list:
-    """Parse Radiance primitives inside a file path into a list of dictionary.
-    Args:
-        lines: list of lines as strings
-
-    Returns:
-        list of primitives as dictionaries
-    """
-    # Expand in-line commands
-    cmd_lines = [(idx, line) for idx, line in enumerate(lines)
-                 if line.startswith('!')]
-    cmd_results = []
-    for cmd in cmd_lines:
-        cmd_results.append(
-            sp.run(cmd[1][1:], shell=True, stdout=sp.PIPE)
-            .stdout.decode().splitlines())
-    counter = 0
-    for idx, item in enumerate(cmd_lines):
-        counter += item[0]
-        lines[counter:counter+1] = cmd_results[idx]
-        counter += len(cmd_results[idx]) - 1 - item[0]
-
-    content = ' '.join([i.strip() for i in lines
-                        if i.strip() != '' and i[0] != '#']).split()
-    primitives: List[Primitive] = []
-    idx = 0
-    while idx < len(content):
-        _modifier = content[idx]
-        _type = content[idx + 1]
-        if _type == 'alias':
-            _name_to = content[idx + 2]
-            _name_from = content[idx + 3]
-            primitives.append(Primitive(_modifier, _type, _name_to, _name_from, '', int_arg=''))
-            idx += 4
-            continue
-        _identifier = content[idx + 2]
-        str_arg_cnt = int(content[idx + 3])
-        _str_args = ' '.join(content[idx + 3:idx + 4 + str_arg_cnt])
-        idx += 5 + str_arg_cnt
-        real_arg_cnt = int(content[idx])
-        _real_args = ' '.join(content[idx:idx + 1 + real_arg_cnt])
-        idx += real_arg_cnt + 1
-        primitives.append(Primitive(
-            _modifier, _type, _identifier, _str_args, _real_args))
-    return primitives
+def polygon2prim(polygon: geom.Polygon, modifier: str, identifier: str) -> Primitive:
+    """Generate a primitive from a polygon."""
+    return Primitive(modifier, "polygon", identifier, ["0"], polygon.to_real())
 
 
-def unpack_primitives(fpath: str) -> List[Primitive]:
-    """Open a file a to parse primitive."""
-    with open(fpath, 'r') as rdr:
-        return parse_primitive(rdr.readlines())
+def unpack_idf(path: str) -> dict:
+    """Read and parse and idf files."""
+    with open(path, "r") as rdr:
+        return parsers.parse_idf(rdr.read())
+
+
+def sdata2bsdf(sdata: ScatteringData) -> BSDFData:
+    """Convert sdata object to bsdf object."""
+    basis = BASIS_DICT[str(sdata.ncolumn)]
+    lambdas = angle_basis_coeff(basis)
+    bsdf = []
+    for irow in range(sdata.nrow):
+        for icol, lam in zip(range(sdata.ncolumn), lambdas):
+            bsdf.append(sdata.sdata[icol + irow * sdata.ncolumn] / lam)
+    return BSDFData(bsdf, sdata.ncolumn, sdata.nrow)
+
+
+def bsdf2sdata(bsdf: BSDFData) -> ScatteringData:
+    """Covert a bsdf object into a sdata object."""
+    basis = BASIS_DICT[str(bsdf.ncolumn)]
+    lambdas = angle_basis_coeff(basis)
+    sdata = []
+    for irow in range(bsdf.nrow):
+        for icol, lam in zip(range(bsdf.ncolumn), lambdas):
+            sdata.append(bsdf.bsdf[icol + irow * bsdf.ncolumn] * lam)
+    return ScatteringData(sdata, bsdf.ncolumn, bsdf.nrow)
+
+
+def frange_inc(start, stop, step):
+    """Generate increasing non-integer range."""
+    r = start
+    while r < stop:
+        yield r
+        r += step
 
 
-def parse_polygon(real_arg: str) -> radgeom.Polygon:
-    """Parse real arguments to polygon.
+def square2disk(in_square_a: float, in_square_b: float) -> tuple:
+    """Shirley-Chiu square to disk mapping.
     Args:
-        primitive: a dictionary object containing a primitive
-
-    Returns:
-        modified primitive
+        in_square_a: [-1, 1]
+        in_square_b: [-1, 1]
     """
-    real_args = real_arg.split()
-    coords = [float(i) for i in real_args[1:]]
-    arg_cnt = int(real_args[0])
-    vertices = [radgeom.Vector(*coords[i:i + 3]) for i in range(0, arg_cnt, 3)]
-    return radgeom.Polygon(vertices)
+    if in_square_a + in_square_b > 0:
+        if in_square_a > in_square_b:
+            in_square_rgn = 0
+        else:
+            in_square_rgn = 1
+    else:
+        if in_square_b > in_square_a:
+            in_square_rgn = 2
+        else:
+            in_square_rgn = 3
+    out_disk_r = [in_square_a, in_square_b, -in_square_a, -in_square_b][in_square_rgn]
+    if in_square_b * in_square_b > 0:
+        phi_select_4 = 6 - in_square_a / in_square_b
+    else:
+        phi_select_4 = 0
+    phi_select = [
+        in_square_b / in_square_a,
+        2 - in_square_a / in_square_b,
+        4 + in_square_b / in_square_a,
+        phi_select_4,
+    ]
+    out_disk_phi = math.pi / 4 * phi_select[in_square_rgn]
+    out_disk_x = out_disk_r * math.cos(out_disk_phi)
+    out_disk_y = out_disk_r * math.sin(out_disk_phi)
+    return out_disk_x, out_disk_y, out_disk_r, out_disk_phi
+
+
+def id_generator(size: int = 3, chars: Optional[str] = None) -> str:
+    """Generate random characters."""
+    if chars is None:
+        chars = string.ascii_uppercase + string.digits
+    return "".join(random.choice(chars) for _ in range(size))
 
 
-def polygon2prim(polygon: radgeom.Polygon,
-                 modifier: str, identifier: str) -> Primitive:
-    """Generate a primitive from a polygon."""
-    return Primitive(modifier, 'polygon', identifier, '0', polygon.to_real())
+def unpack_primitives(file: Union[str, Path, TextIOWrapper]) -> List[Primitive]:
+    """Open a file a to parse primitive."""
+    if isinstance(file, TextIOWrapper):
+        lines = file.readlines()
+    else:
+        with open(file, "r", encoding="ascii") as rdr:
+            lines = rdr.readlines()
+    return parsers.parse_primitive(lines)
 
 
-def primitive_normal(primitive_paths: List[str]) -> Set[radgeom.Vector]:
+def primitive_normal(primitive_paths: List[str]) -> Set[geom.Vector]:
     """Return a set of normal vectors given a list of primitive paths."""
     _primitives: List[Primitive] = []
-    _normals: List[radgeom.Vector]
+    _normals: List[geom.Vector]
     for path in primitive_paths:
         _primitives.extend(unpack_primitives(path))
-    _normals = [parse_polygon(prim.real_arg).normal() for prim in _primitives]
+    _normals = [parsers.parse_polygon(prim.real_arg).normal for prim in _primitives]
     return set(_normals)
 
 
-def samp_dir(primlist: list) -> radgeom.Vector:
+def samp_dir(primlist: list) -> geom.Vector:
     """Calculate the primitives' average sampling
     direction weighted by area."""
-    primlist = [p for p in primlist
-                if p.ptype == 'polygon' or p.ptype == 'ring']
-    normal_area = radgeom.Vector()
+    primlist = [p for p in primlist if p.ptype in ("polygon", "ring")]
+    normal_area = geom.Vector()
     for prim in primlist:
-        polygon = parse_polygon(prim.real_arg)
-        normal_area += polygon.normal().scale(polygon.area())
+        polygon = parsers.parse_polygon(prim.real_arg)
+        normal_area += polygon.normal.scale(polygon.area)
     sdir = normal_area.scale(1.0 / len(primlist))
     sdir = sdir.normalize()
     return sdir
 
 
-def up_vector(primitives: list) -> radgeom.Vector:
+def up_vector(primitives: list) -> geom.Vector:
     """Define the up vector given primitives.
 
     Args:
         primitives: list of dictionary (primitives)
 
     Returns:
         returns a str as x,y,z
 
     """
-    xaxis = radgeom.Vector(1, 0, 0)
-    yaxis = radgeom.Vector(0, 1, 0)
+    xaxis = geom.Vector(1, 0, 0)
+    yaxis = geom.Vector(0, 1, 0)
     norm_dir = samp_dir(primitives)
     if norm_dir not in (xaxis, xaxis.scale(-1)):
-        upvect = norm_dir.cross(xaxis)
+        upvect = xaxis.cross(norm_dir)
     else:
-        upvect = norm_dir.cross(yaxis)
+        upvect = yaxis.cross(norm_dir)
     return upvect
 
 
-def neutral_plastic_prim(mod: str, ident: str, refl: float,
-                         spec: float, rough: float) -> Primitive:
+def neutral_plastic_prim(
+    mod: str, ident: str, refl: float, spec: float, rough: float
+) -> Primitive:
     """Generate a neutral color plastic material.
     Args:
         mod(str): modifier to the primitive
         ident(str): identifier to the primitive
         refl (float): measured reflectance (0.0 - 1.0)
         specu (float): material specularity (0.0 - 1.0)
         rough (float): material roughness (0.0 - 1.0)
 
     Returns:
         A material primtive
     """
-    err_msg = 'reflectance, speculariy, and roughness have to be 0-1'
+    err_msg = "reflectance, speculariy, and roughness have to be 0-1"
     assert all(0 <= i <= 1 for i in [spec, refl, rough]), err_msg
-    real_args = '5 {0} {0} {0} {1} {2} \n'.format(refl, spec, rough)
-    return Primitive(mod, 'plastic', ident, '0', real_args)
+    real_args = [5, refl, refl, refl, spec, rough]
+    return Primitive(mod, "plastic", ident, ["0"], real_args)
 
 
-def neutral_trans_prim(mod: str, ident: str, trans: float, refl: float,
-                         spec: float, rough: float) -> Primitive:
+def neutral_trans_prim(
+    mod: str, ident: str, trans: float, refl: float, spec: float, rough: float
+) -> Primitive:
     """Generate a neutral color plastic material.
     Args:
         mod(str): modifier to the primitive
         ident(str): identifier to the primitive
         refl (float): measured reflectance (0.0 - 1.0)
         specu (float): material specularity (0.0 - 1.0)
         rough (float): material roughness (0.0 - 1.0)
 
     Returns:
         A material primtive
     """
     color = trans + refl
     t_diff = trans / color
     tspec = 0
-    err_msg = 'reflectance, speculariy, and roughness have to be 0-1'
+    err_msg = "reflectance, speculariy, and roughness have to be 0-1"
     assert all(0 <= i <= 1 for i in [spec, refl, rough]), err_msg
-    real_args = "7 {0} {0} {0} {1} {2} {3} {4}".format(color, spec, rough, t_diff, tspec)
-    return Primitive(mod, 'trans', ident, '0', real_args)
+    real_args = [7, color, color, color, spec, rough, t_diff, tspec]
+    return Primitive(mod, "trans", ident, ["0"], real_args)
 
 
-def color_plastic_prim(mod, ident, refl, red, green, blue, specu, rough):
+def color_plastic_prim(mod, ident, refl, red, green, blue, specu, rough) -> Primitive:
     """Generate a colored plastic material.
     Args:
         mod(str): modifier to the primitive
         ident(str): identifier to the primitive
         refl (float): measured reflectance (0.0 - 1.0)
         red; green; blue (int): rgb values (0 - 255)
         specu (float): material specularity (0.0 - 1.0)
         rough (float): material roughness (0.0 - 1.0)
 
     Returns:
         A material primtive
     """
-    err_msg = 'reflectance, speculariy, and roughness have to be 0-1'
+    err_msg = "reflectance, speculariy, and roughness have to be 0-1"
     assert all(0 <= i <= 1 for i in [specu, refl, rough]), err_msg
     red_eff = 0.3
     green_eff = 0.59
     blue_eff = 0.11
     weighted = red * red_eff + green * green_eff + blue * blue_eff
     matr = round(red / weighted * refl, 3)
     matg = round(green / weighted * refl, 3)
     matb = round(blue / weighted * refl, 3)
-    real_args = '5 %s %s %s %s %s\n' % (matr, matg, matb, specu, rough)
-    return Primitive(mod, 'plastic', ident, '0', real_args)
+    real_args = [5, matr, matg, matb, specu, rough]
+    return Primitive(mod, "plastic", ident, "0", real_args)
 
 
-def glass_prim(mod, ident, tr, tg, tb, refrac=1.52):
+def glass_prim(
+    mod, ident, tr: float, tg: float, tb: float, refrac: float = 1.52
+) -> Primitive:
     """Generate a glass material.
 
     Args:
         mod (str): modifier to the primitive
         ident (str): identifier to the primtive
         tr, tg, tb (float): transmmisivity in each channel (0.0 - 1.0)
         refrac (float): refraction index (default=1.52)
     Returns:
         material primtive (dict)
 
     """
-    tmsv_red = util.tmit2tmis(tr)
-    tmsv_green = util.tmit2tmis(tg)
-    tmsv_blue = util.tmit2tmis(tb)
-    real_args = '4 %s %s %s %s' % (tmsv_red, tmsv_green, tmsv_blue, refrac)
-    return Primitive(mod, 'glass', ident, '0', real_args)
-
-
-def bsdf_prim(mod, ident, xmlpath, upvec,
-              pe=False, thickness=0.0, xform=None, real_args='0'):
+    tmsv_red = tmit2tmis(tr)
+    tmsv_green = tmit2tmis(tg)
+    tmsv_blue = tmit2tmis(tb)
+    real_args = [4, tmsv_red, tmsv_green, tmsv_blue, refrac]
+    return Primitive(mod, "glass", ident, ["0"], real_args)
+
+
+def bsdf_prim(
+    mod,
+    ident,
+    xmlpath,
+    upvec,
+    pe: bool = False,
+    thickness: float = 0.0,
+    xform=None,
+    real_args: str = "0",
+) -> Primitive:
     """Create a BSDF primtive."""
-    str_args = '"{}" {} '.format(xmlpath, str(upvec))
+    str_args = [xmlpath, str(upvec)]
     str_args_count = 5
     if pe:
-        _type = 'aBSDF'
+        _type = "aBSDF"
     else:
         str_args_count += 1
-        str_args = '%s ' % thickness + str_args
-        _type = 'BSDF'
+        str_args = [str(thickness), *str_args]
+        _type = "BSDF"
     if xform is not None:
         str_args_count += len(xform.split())
-        str_args += xform
+        str_args.extend(*xform.split())
     else:
-        str_args += '.'
-    str_args = '%s ' % str_args_count + str_args
+        str_args.append(".")
+    str_args = [str(str_args_count), *str_args]
     return Primitive(mod, _type, ident, str_args, real_args)
 
 
-def lambda_calc(theta_lr, theta_up, nphi):
+def lambda_calc(theta_lr: float, theta_up: float, nphi: float) -> float:
     """."""
-    return ((math.cos(math.pi / 180 * theta_lr)**2 -
-             math.cos(math.pi / 180 * theta_up)**2) * math.pi / nphi)
+    return (
+        (
+            math.cos(math.pi / 180 * theta_lr) ** 2
+            - math.cos(math.pi / 180 * theta_up) ** 2
+        )
+        * math.pi
+        / nphi
+    )
 
 
 def angle_basis_coeff(basis: str) -> List[float]:
-    '''Calculate klems basis coefficient'''
+    """Calculate klems basis coefficient"""
     ablist = ABASE_LIST[basis]
     lambdas = []
     for i in range(len(ablist) - 1):
         tu = ablist[i + 1][0]
         tl = ablist[i][0]
         np = ablist[i][1]
         lambdas.extend([lambda_calc(tl, tu, np) for _ in range(np)])
     return lambdas
 
 
-def opt2str(opt: dict) -> str:
-    out_str = ""
-    for k, v in opt.items():
-        if isinstance(v, list):
-            val = ' '.join(map(str, v))
-        else:
-            val = v
-        if k == 'vt' or k == 'f':
-            out_str += "-{}{} ".format(k, val)
-        elif k == 'hd':
-            out_str += "-h "
-        else:
-            out_str += '-{} {} '.format(k, val)
-    return out_str
-
+def opt2list(opt: dict) -> List[str]:
+    """Convert option dictionary to list.
 
-class Reinsrc:
-    """Calculate Reinhart/Treganza sampling directions.
+    Key: str
+    Value: str | float | int | bool | list
 
-    Direct translation of Radiance reinsrc.cal file.
+    Args:
+        opt: option dictionary
+    Returns:
+        A list of strings
     """
+    out = []
+    for key, value in opt.items():
+        if isinstance(value, str):
+            if key == "vf":
+                out.extend(["-" + key, value])
+            else:
+                out.append(f"-{key}{value}")
+        elif isinstance(value, bool):
+            if value:
+                out.append(f"-{key}+")
+            else:
+                out.append(f"-{key}-")
+        elif isinstance(value, (int, float)):
+            out.extend(["-" + key, str(value)])
+        elif isinstance(value, list):
+            out.extend(["-" + key, *map(str, value)])
+    return out
 
-    TNAZ = [30, 30, 24, 24, 18, 12, 6]
 
-    def __init__(self, mf: int):
-        """Initialize with multiplication factor."""
-        self.mf = mf
-        self.rowMax = 7 * mf + 1
-        self.rmax = self.raccum(self.rowMax)
-        self.alpha = 90 / (mf * 7 + 0.5)
-
-    def dir_calc(self, rbin: int, x1=0.5, x2=0.5) -> tuple:
-        """Calculate the ray direction.
-
-        Parameter:
-            rbin: bin count
-            x1, x2: sampling position (0.5, 0.5) is at the center
-        Return:
-            Sampling direction (tuple)
-        """
-        rrow = self.rowMax - \
-            1 if rbin > (self.rmax - 0.5) else self.rfindrow(0, rbin)
-        rcol = rbin - self.raccum(rrow) - 1
-        razi_width = 2 * math.pi / self.rnaz(rrow)
-        rah = self.alpha * math.pi / 180
-        razi = (rcol + x2 - 0.5) * \
-            razi_width if rbin > 0.5 else 2 * math.pi * x2
-        ralt = (rrow + x1) * rah if rbin > 0.5 else math.asin(-x1)
-        cos_alt = math.cos(ralt)
-        if rbin < .5:
-            romega = 2 * math.pi
-        else:
-            if self.rmax - .5 > rbin:
-                romega = razi_width * (math.sin(rah * (rrow + 1)) - math.sin(rah * rrow))
-            else:
-                romega = 2 * math.pi * (1 - math.cos(rah / 2))
-        dx = math.sin(razi) * cos_alt
-        dy = math.cos(razi) * cos_alt
-        dz = math.sin(ralt)
-        return (dx, dy, dz, romega)
+def calc_reinsrc_dir(
+    mf: int, x1: float = 0.5, x2: float = 0.5
+) -> Tuple[List[geom.Vector], List[float]]:
+    """
+    Calculate Reinhart/Treganza sampling directions.
+    Direct translation of Radiance reinsrc.cal file.
 
-    def rnaz(self, r):
+    Args:
+        mf(int): multiplication factor.
+        x1(float, optional): bin position 1
+        x2(float, optional): bin position 2
+    Returns:
+        A list of geom.Vector
+        A list of solid angle associated with each vector
+    """
+
+    def rnaz(r):
         """."""
-        if r > (self.mf * 7 - .5):
+        if r > (mf * 7 - 0.5):
             return 1
-        else:
-            return self.mf * self.TNAZ[int(math.floor((r + 0.5) / self.mf))]
+        return mf * TNAZ[int(math.floor((r + 0.5) / mf))]
 
-    def raccum(self, r):
+    def raccum(r):
         """."""
         if r > 0.5:
-            return self.rnaz(r - 1) + self.raccum(r - 1)
-        else:
-            return 0
+            return rnaz(r - 1) + raccum(r - 1)
+        return 0
 
-    def rfindrow(self, r, rem):
+    def rfindrow(r, rem):
         """."""
-        if (rem - self.rnaz(r)) > 0.5:
-            return self.rfindrow(r + 1, rem - self.rnaz(r))
+        if (rem - rnaz(r)) > 0.5:
+            return rfindrow(r + 1, rem - rnaz(r))
+        return r
+
+    TNAZ = [30, 30, 24, 24, 18, 12, 6]
+    rowMax = 7 * mf + 1
+    runlen = 144 * mf**2 + 3
+    rmax = raccum(rowMax)
+    alpha = 90 / (mf * 7 + 0.5)
+    dvecs = []
+    omegas = []
+    for rbin in range(1, runlen):
+        rrow = rowMax - 1 if rbin > (rmax - 0.5) else rfindrow(0, rbin)
+        rcol = rbin - raccum(rrow) - 1
+        razi_width = 2 * math.pi / rnaz(rrow)
+        rah = alpha * math.pi / 180
+        razi = (rcol + x2 - 0.5) * razi_width if rbin > 0.5 else 2 * math.pi * x2
+        ralt = (rrow + x1) * rah if rbin > 0.5 else math.asin(-x1)
+        cos_alt = math.cos(ralt)
+        if rmax - 0.5 > rbin:
+            romega = razi_width * (math.sin(rah * (rrow + 1)) - math.sin(rah * rrow))
         else:
-            return r
+            romega = 2 * math.pi * (1 - math.cos(rah / 2))
+        dx = math.sin(razi) * cos_alt
+        dy = math.cos(razi) * cos_alt
+        dz = math.sin(ralt)
+        dvecs.append(geom.Vector(dx, dy, dz))
+        omegas.append(romega)
+    return dvecs, omegas
 
 
-class pt_inclusion(object):
+def pt_inclusion(pt: geom.Vector, polygon_pts: List[geom.Vector]) -> int:
     """Test whether a point is inside a polygon
     using winding number algorithm."""
 
-    def __init__(self, polygon_pts):
-        """Initialize the polygon."""
-        self.pt_cnt = len(polygon_pts)
-        polygon_pts.append(polygon_pts[0])
-        self.polygon_pts = polygon_pts
-
-    def isLeft(self, pt0, pt1, pt2):
+    def isLeft(pt0, pt1, pt2):
         """Test whether a point is left to a line."""
-        return (pt1.x - pt0.x) * (pt2.y - pt0.y) \
-            - (pt2.x - pt0.x) * (pt1.y - pt0.y)
+        return (pt1.x - pt0.x) * (pt2.y - pt0.y) - (pt2.x - pt0.x) * (pt1.y - pt0.y)
 
-    def test_inside(self, pt):
-        """Test if a point is inside the polygon."""
-        wn = 0
-        for i in range(self.pt_cnt):
-            if self.polygon_pts[i].y <= pt.y:
-                if self.polygon_pts[i + 1].y > pt.y:
-                    if self.isLeft(self.polygon_pts[i],
-                                   self.polygon_pts[i + 1], pt) > 0:
-                        wn += 1
-            else:
-                if self.polygon_pts[i + 1].y <= pt.y:
-                    if self.isLeft(self.polygon_pts[i],
-                                   self.polygon_pts[i + 1], pt) < 0:
-                        wn -= 1
-        return wn
+    # Close the polygon for looping
+    # polygon_pts.append(polygon_pts[0])
+    polygon_pts = [*polygon_pts, polygon_pts[0]]
+    wn = 0
+    for i in range(len(polygon_pts) - 1):
+        if polygon_pts[i].y <= pt.y:
+            if polygon_pts[i + 1].y > pt.y:
+                if isLeft(polygon_pts[i], polygon_pts[i + 1], pt) > 0:
+                    wn += 1
+        else:
+            if polygon_pts[i + 1].y <= pt.y:
+                if isLeft(polygon_pts[i], polygon_pts[i + 1], pt) < 0:
+                    wn -= 1
+    return wn
 
 
-def gen_grid(polygon: radgeom.Polygon, height: float, spacing: float) -> list:
+def gen_grid(polygon: geom.Polygon, height: float, spacing: float) -> list:
     """Generate a grid of points for orthogonal planar surfaces.
 
     Args:
         polygon: a polygon object
         height: points' distance from the surface in its normal direction
         spacing: distance between the grid points
     Returns:
         List of the points as list
     """
     vertices = polygon.vertices
-    plane_height = sum([i.z for i in vertices]) / len(vertices)
-    imin, imax, jmin, jmax, _, _ = polygon.extreme()
-    xlen_spc = ((imax - imin) / spacing)
-    ylen_spc = ((jmax - jmin) / spacing)
+    plane_height = sum(i.z for i in vertices) / len(vertices)
+    imin, imax, jmin, jmax, _, _ = polygon.extreme
+    xlen_spc = (imax - imin) / spacing
+    ylen_spc = (jmax - jmin) / spacing
     xstart = ((xlen_spc - int(xlen_spc) + 1)) * spacing / 2
     ystart = ((ylen_spc - int(ylen_spc) + 1)) * spacing / 2
-    x0 = [x + xstart for x in util.frange_inc(imin, imax, spacing)]
-    y0 = [x + ystart for x in util.frange_inc(jmin, jmax, spacing)]
-    grid_dir = polygon.normal().reverse()
-    grid_hgt = radgeom.Vector(0, 0, plane_height) + grid_dir.scale(height)
-    raw_pts = [radgeom.Vector(round(i, 3), round(j, 3), round(grid_hgt.z, 3))
-               for i in x0 for j in y0]
-    scale_factor = 1 - 0.3/(imax - imin)  # scale boundary down .3 meter
-    _polygon = polygon.scale(radgeom.Vector(
-        scale_factor, scale_factor, 0), polygon.centroid())
+    x0 = [x + xstart for x in frange_inc(imin, imax, spacing)]
+    y0 = [x + ystart for x in frange_inc(jmin, jmax, spacing)]
+    grid_dir = polygon.normal.reverse()
+    grid_hgt = geom.Vector(0, 0, plane_height) + grid_dir.scale(height)
+    raw_pts = [
+        geom.Vector(round(i, 3), round(j, 3), round(grid_hgt.z, 3))
+        for i in x0
+        for j in y0
+    ]
+    scale_factor = 1 - 0.3 / (imax - imin)  # scale boundary down .3 meter
+    _polygon = polygon.scale(
+        geom.Vector(scale_factor, scale_factor, 0), polygon.centroid
+    )
     _vertices = _polygon.vertices
-    if polygon.normal() == radgeom.Vector(0, 0, 1):
-        pt_incls = pt_inclusion(_vertices)
+    if polygon.normal == geom.Vector(0, 0, 1):
+        # pt_incls = pt_inclusion(_vertices)
+        _grid = [p for p in raw_pts if pt_inclusion(p, _vertices) > 0]
     else:
-        pt_incls = pt_inclusion(_vertices[::-1])
-    _grid = [p for p in raw_pts if pt_incls.test_inside(p) > 0]
+        # pt_incls = pt_inclusion(_vertices[::-1])
+        _grid = [p for p in raw_pts if pt_inclusion(p, _vertices[::-1]) > 0]
+    # _grid = [p for p in raw_pts if pt_incls.test_inside(p) > 0]
     grid = [p.to_list() + grid_dir.to_list() for p in _grid]
     return grid
 
 
-def gengrid():
-    """Commandline program for generating a grid of sensor points."""
-    parser = argparse.ArgumentParser(
-        prog='gengrid',
-        description='Generate an equal-spaced sensor grid based on a surface.')
-    parser.add_argument('surface', help='surface file path')
-    parser.add_argument('spacing', type=float)
-    parser.add_argument('height', type=float)
-    parser.add_argument('-op', action='store_const', const='', default=True)
-    args = parser.parse_args()
-    prims = unpack_primitives(args.surface)
-    polygon_prims = [prim for prim in prims if prim.ptype == 'polygon']
-    polygon = parse_polygon(polygon_prims[0].real_arg)
-    if args.op:
-        polygon = polygon.flip()
-    grid_list = gen_grid(polygon, args.height, args.spacing)
-    grid_str = '\n'.join([' '.join(map(str, row)) for row in grid_list])
-    print(grid_str)
-
-
-def material_lib():
-    mlib = []
-    # carpet .2
-    mlib.append(neutral_plastic_prim('void', 'carpet_20', .2, 0, 0))
-    # Paint .5
-    mlib.append(neutral_plastic_prim('void', 'white_paint_50', .5, 0, 0))
-    # Paint .7
-    mlib.append(neutral_plastic_prim('void', 'white_paint_70', .7, 0, 0))
-    # Glass .6
-    tmis = util.tmit2tmis(.6)
-    mlib.append(glass_prim('void', 'glass_60', tmis, tmis, tmis))
-    return mlib
+def material_lib() -> Dict[str, Any]:
+    """Generate a list of generic material primitives."""
+    tmis = tmit2tmis(0.6)
+    return {
+        "neutral_lambertian_0.2": neutral_plastic_prim(
+            "void", "neutral_lambertian_0.2", 0.2, 0, 0
+        ),
+        "neutral_lambertian_0.5": neutral_plastic_prim(
+            "void", "neutral_lambertian_0.5", 0.5, 0, 0
+        ),
+        "neutral_lambertian_0.7": neutral_plastic_prim(
+            "void", "neutral_lambertian_0.7", 0.7, 0, 0
+        ),
+        "glass_60": glass_prim("void", "glass_60", tmis, tmis, tmis),
+    }
 
 
-def gen_blinds(depth, width, height, spacing, angle, curve, movedown):
+def gen_blinds(depth, width, height, spacing, angle, curve, movedown) -> str:
     """Generate genblinds command for genBSDF."""
     nslats = int(round(height / spacing, 0))
     slat_cmd = "!genblinds blindmaterial blinds "
-    slat_cmd += "{} {} {} {} {} {}".format(
-        depth, width, height, nslats, angle, curve)
+    slat_cmd += f"{depth} {width} {height} {nslats} {angle} {curve}"
     slat_cmd += "| xform -rz -90 -rx -90 -t "
     slat_cmd += f"{-width/2} {-height/2} {-movedown}\n"
     return slat_cmd
 
 
-def analyze_vert_polygon(window_polygon, movedown):
-    """Parse window primitive and prepare for genBSDF.
-    Window has to be verticle.
-    """
-    window_normal = window_polygon.normal()
-    if round(window_normal.z, 1) != 0:
-        raise Exception("Can only analyze vertical polygons")
-    vertices = window_polygon.vertices
-    if len(vertices) != 4:
-        raise Exception("4-sided polygon only")
-    window_center = window_polygon.centroid()
-    dim1 = vertices[0] - vertices[1]
-    dim2 = vertices[1] - vertices[2]
-    if dim1.normalize() in (radgeom.Vector(0, 0, 1), radgeom.Vector(0, 0, -1)):
-        height = dim1.length()
-        width = dim2.length()
-    else:
-        height = dim2.length()
-        width = dim1.length()
-    _south = radgeom.Vector(0, -1, 0)
-    angle2negY = window_normal.angle_from(_south)
-    rotate_window = window_center.rotate_3d(
-        radgeom.Vector(0, 0, 1), angle2negY).rotate_3d(
-            radgeom.Vector(1, 0, 0), math.pi / 2)
-    translate = radgeom.Vector(0, 0, -movedown) - rotate_window
-    return height, width, angle2negY, translate
-
-
-def varays():
-    """Commandline utility program for generating circular fisheye rays."""
-    aparser = argparse.ArgumentParser(
-        prog='varays',
-        description='Generate a fisheye view rays with blackedout corners')
-    aparser.add_argument(
-        '-x', required=True, help='square image resolution')
-    aparser.add_argument('-c', default='1', help='Ray count')
-    aparser.add_argument('-vf', required=True, help='View file path')
-    args = aparser.parse_args()
-    cmd = "vwrays -ff -x {0} -y {0} ".format(args.x)
-    if args.c != '1':
-        cmd += '-c {} -pj 0.7 '.format(args.c)
-    cmd += f"-vf {args.vf} | "
-    cmd += radmtx.Sender.crop2circle(args.c, args.x)
-    sp.run(cmd, shell=True)
-
-
-def get_glazing_primitive(panes: List[util.PaneRGB]) -> Primitive:
+def get_glazing_primitive(panes: List[PaneRGB]) -> Primitive:
     """Generate a BRTDfunc to represent a glazing system."""
     if len(panes) > 2:
         raise ValueError("Only double pane supported")
     name = "+".join([pane.measured_data.name for pane in panes])
     if len(panes) == 1:
-        str_arg = "10 sr_clear_r sr_clear_g sr_clear_b "
-        str_arg += "st_clear_r st_clear_g st_clear_b 0 0 0 glaze1.cal"
-        coated_real = "1" if panes[0].measured_data.coated_side == 'front' else "-1"
-        real_arg = f"19 0 0 0 0 0 0 0 0 0 {coated_real} "
-        real_arg += " ".join(map(str, panes[0].glass_rgb)) + " "
-        real_arg += " ".join(map(str, panes[0].coated_rgb)) + " "
-        real_arg += " ".join(map(str, panes[0].trans_rgb))
+        str_arg = [
+            "10",
+            "sr_clear_r",
+            "sr_clear_g",
+            "sr_clear_b",
+            "st_clear_r",
+            "st_clear_g",
+            "st_clear_b",
+            "0",
+            "0",
+            "0",
+            "glaze1.cal",
+        ]
+        coated_real = 1 if panes[0].measured_data.coated_side == "front" else -1
+        real_arg = [
+            19,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            coated_real,
+            *[round(i, 3) for i in panes[0].glass_rgb],
+            *[round(i, 3) for i in panes[0].coated_rgb],
+            *[round(i, 3) for i in panes[0].trans_rgb],
+        ]
     else:
-        s12t_rgb = panes[0].trans_rgb
-        s34t_rgb = panes[1].trans_rgb
-        if panes[0].measured_data.coated_side == 'back':
-            s2r_rgb = panes[0].coated_rgb
-            s1r_rgb = panes[0].glass_rgb
+        s12t_r, s12t_g, s12t_b = panes[0].trans_rgb
+        s34t_r, s34t_g, s34t_b = panes[1].trans_rgb
+        if panes[0].measured_data.coated_side == "back":
+            s2r_r, s2r_g, s2r_b = panes[0].coated_rgb
+            s1r_r, s1r_g, s1r_b = panes[0].glass_rgb
         else:  # front or neither side coated
-            s2r_rgb = panes[0].glass_rgb
-            s1r_rgb = panes[0].coated_rgb
-        if panes[1].measured_data.coated_side == 'back':
-            s4r_rgb = panes[1].coated_rgb
-            s3r_rgb = panes[1].glass_rgb
+            s2r_r, s2r_g, s2r_b = panes[0].glass_rgb
+            s1r_r, s1r_g, s1r_b = panes[0].coated_rgb
+        if panes[1].measured_data.coated_side == "back":
+            s4r_r, s4r_g, s4r_b = panes[1].coated_rgb
+            s3r_r, s3r_g, s3r_b = panes[1].glass_rgb
         else:  # front or neither side coated
-            s4r_rgb = panes[1].glass_rgb
-            s3r_rgb = panes[1].coated_rgb
-        str_arg = "10\nif(Rdot,"
-        str_arg += f"cr(fr({s4r_rgb[0]}),ft({s34t_rgb[0]}),fr({s2r_rgb[0]})),"
-        str_arg += f"cr(fr({s1r_rgb[0]}),ft({s12t_rgb[0]}),ft({s3r_rgb[0]})))\n"
-        str_arg += "if(Rdot,"
-        str_arg += f"cr(fr({s4r_rgb[1]}),ft({s34t_rgb[1]}),fr({s2r_rgb[1]})),"
-        str_arg += f"cr(fr({s1r_rgb[1]}),ft({s12t_rgb[1]}),fr({s3r_rgb[1]})))\n"
-        str_arg += "if(Rdot,"
-        str_arg += f"cr(fr({s4r_rgb[2]}),ft({s34t_rgb[2]}),fr({s2r_rgb[2]})),"
-        str_arg += f"cr(fr({s1r_rgb[2]}),ft({s12t_rgb[2]}),fr({s3r_rgb[2]})))\n"
-        str_arg += f"ft({s34t_rgb[0]})*ft({s12t_rgb[0]})\n"
-        str_arg += f"ft({s34t_rgb[1]})*ft({s12t_rgb[1]})\n"
-        str_arg += f"ft({s34t_rgb[2]})*ft({s12t_rgb[2]})\n"
-        str_arg += "0 0 0 glaze2.cal"
-        real_arg = "9 0 0 0 0 0 0 0 0 0"
+            s4r_r, s4r_g, s4r_b = panes[1].glass_rgb
+            s3r_r, s3r_g, s3r_b = panes[1].coated_rgb
+        str_arg = [
+            "10",
+            (
+                f"if(Rdot,cr(fr({s4r_r:.3f}),ft({s34t_r:.3f}),fr({s2r_r:.3f})),"
+                f"cr(fr({s1r_r:.3f}),ft({s12t_r:.3f}),fr({s3r_r:.3f})))"
+            ),
+            (
+                f"if(Rdot,cr(fr({s4r_g:.3f}),ft({s34t_g:.3f}),fr({s2r_g:.3f})),"
+                f"cr(fr({s1r_g:.3f}),ft({s12t_g:.3f}),fr({s3r_g:.3f})))"
+            ),
+            (
+                f"if(Rdot,cr(fr({s4r_b:.3f}),ft({s34t_b:.3f}),fr({s2r_b:.3f})),"
+                f"cr(fr({s1r_b:.3f}),ft({s12t_b:.3f}),fr({s3r_b:.3f})))"
+            ),
+            f"ft({s34t_r:.3f})*ft({s12t_r:.3f})",
+            f"ft({s34t_g:.3f})*ft({s12t_g:.3f})",
+            f"ft({s34t_b:.3f})*ft({s12t_b:.3f})",
+            "0",
+            "0",
+            "0",
+            "glaze2.cal",
+        ]
+        real_arg = [9, 0, 0, 0, 0, 0, 0, 0, 0, 0]
     return Primitive("void", "BRTDfunc", name, str_arg, real_arg)
 
 
-def glaze():
-    """Command-line program for generating BRTDfunc for glazing system."""
-    aparser = argparse.ArgumentParser(
-        prog='glaze',
-        description='Generate BRTDfunc for a glazing system')
-    aparser.add_argument('-X', '--optics', nargs='+', help='Optics file path')
-    aparser.add_argument('-C', '--cspace', default='radiance',
-                         help='Color space to determine primaries')
-    aparser.add_argument('-D', '--igsdb', nargs="+",
-                         help='IGSDB json file path or ID')
-    aparser.add_argument('-T', '--token', help='IGSDB token')
-    args = aparser.parse_args()
-    if args.optics is not None:
-        panes = [util.parse_optics(fpath) for fpath in args.optics]
-    elif args.igsdb is not None:
-        panes = []
-        for item in args.igsdb:
-            if os.path.isfile(item):
-                with open(item, 'r') as rdr:
-                    json_obj = json.load(rdr)
-            elif item[0].isdigit():
-                if args.token is None:
-                    raise ValueError("Missing IGSDB token")
-                json_string = util.get_igsdb_json(item, args.token)
-                json_obj = json.loads(json_string)
-            else:
-                raise ValueError("Unknown IGSDB entry format")
-            panes.append(util.parse_igsdb_json(json_obj))
+def get_flush_corner_rays_command(ray_cnt: int, xres: int) -> list:
+    """Flush the corner rays from a fisheye view.
+
+    Args:
+        ray_cnt: ray count;
+        xres: resolution of the square image;
+
+    Returns:
+        Command to generate cropped rays
+
+    """
+    cmd = [
+        "rcalc",
+        "-if6",
+        "-of",
+        "-e",
+        f"DIM:{xres};CNT:{ray_cnt}",
+        "-e",
+        "pn=(recno-1)/CNT+.5",
+        "-e",
+        "frac(x):x-floor(x)",
+        "-e",
+        "xpos=frac(pn/DIM);ypos=pn/(DIM*DIM)",
+        "-e",
+        "incir=if(.25-(xpos-.5)*(xpos-.5)-(ypos-.5)*(ypos-.5),1,0)",
+        "-e",
+        "$1=$1;$2=$2;$3=$3;$4=$4*incir;$5=$5*incir;$6=$6*incir",
+    ]
+    return cmd
+
+
+def batch_process(
+    commands: List[List[str]],
+    inputs: Optional[List[bytes]] = None,
+    opaths: Optional[List[Path]] = None,
+    nproc: Optional[int] = None,
+) -> None:
+    """Run commands in batches.
+
+    Use subprocess.Popen to run commands.
+
+    Args:
+        commands: commands as a list of strings.
+        inputs: list of standard input to the commands.
+        opaths: list of paths to write standard output to.
+        nproc: number of commands to run in parallel at a time.
+    Returns:
+        None
+    """
+    nproc = 1 if nproc is None else nproc
+    command_groups = [commands[i : i + nproc] for i in range(0, len(commands), nproc)]
+    stdin_groups: List[List[Any]] = [[None] * len(ele) for ele in command_groups]
+    if inputs:
+        if len(inputs) != len(commands):
+            raise ValueError("Number of stdins not equal number of commands.")
+        stdin_groups = [inputs[i : i + nproc] for i in range(0, len(inputs), nproc)]
+    if opaths:
+        if len(opaths) != len(commands):
+            raise ValueError("Number of opaths not equal number of commands.")
+        opath_groups = [opaths[i : i + nproc] for i in range(0, len(opaths), nproc)]
+        for igrp, cgrp, ogrp in zip(stdin_groups, command_groups, opath_groups):
+            processes = []
+            fds = []
+            for command, opath in zip(cgrp, ogrp):
+                fd = open(opath, "wb")
+                processes.append(sp.Popen(command, stdin=sp.PIPE, stdout=fd))
+                fds.append(fd)
+            for proc, sin in zip(processes, igrp):
+                if (proc.stdin is not None) and (sin is not None):
+                    proc.stdin.write(sin)
+            for p, f in zip(processes, fds):
+                p.wait()
+                f.close()
     else:
-        raise ValueError("Need to specify either optics or igsdb file")
-    pane_rgb = []
-    for pane in panes:
-        tf_rgb = util.spec2rgb(pane.get_tf_str(), args.cspace)
-        rf_rgb = util.spec2rgb(pane.get_rf_str(), args.cspace)
-        rb_rgb = util.spec2rgb(pane.get_rb_str(), args.cspace)
-        if pane.coated_side == 'front':
-            coated_rgb = rf_rgb
-            glass_rgb = rb_rgb
-        else:
-            coated_rgb = rb_rgb
-            glass_rgb = rf_rgb
-        pane_rgb.append(util.PaneRGB(pane, coated_rgb, glass_rgb, tf_rgb))
-    print(get_glazing_primitive(pane_rgb))
+        for igrp, cgrp in zip(stdin_groups, command_groups):
+            processes = [sp.Popen(command, stdin=sp.PIPE) for command in cgrp]
+            for proc, sin in zip(processes, igrp):
+                if (proc.stdin is not None) and (sin is not None):
+                    proc.stdin.write(sin)
+            for proc in processes:
+                proc.wait()
+
+
+def run_write(command, out, stdin=None) -> None:
+    """Run command and write stdout to file."""
+    with open(out, "wb") as wtr:
+        sp.run(command, check=True, input=stdin, stdout=wtr)
```

