# Comparing `tmp/PyAstronomy-0.8.1.tar.gz` & `tmp/PyAstronomy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyAstronomy-0.8.1.tar", last modified: Sun Mar  1 17:24:47 2015, max compression
+gzip compressed data, was "dist/PyAstronomy-0.9.0.tar", last modified: Wed Nov  4 11:28:32 2015, max compression
```

## Comparing `PyAstronomy-0.8.1.tar` & `PyAstronomy-0.9.0.tar`

### file list

```diff
@@ -1,355 +1,370 @@
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/
--rw-r--r--   0 steh312   (5677) st         (750)      313 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/PKG-INFO
--rw-r--r--   0 steh312   (5677) st         (750)     6852 2014-10-06 12:40:45.000000 PyAstronomy-0.8.1/setup.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyasl/
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyasl/phoenixUtils/
--rw-r--r--   0 steh312   (5677) st         (750)     3824 2015-02-25 10:55:52.000000 PyAstronomy-0.8.1/src/pyasl/phoenixUtils/read.py
--rw-r--r--   0 steh312   (5677) st         (750)       18 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/phoenixUtils/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)      258 2013-11-25 11:39:15.000000 PyAstronomy-0.8.1/src/pyasl/__init__.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyasl/resBased/
--rw-r--r--   0 steh312   (5677) st         (750)     3575 2014-04-29 12:44:10.000000 PyAstronomy-0.8.1/src/pyasl/resBased/fip.py
--rw-r--r--   0 steh312   (5677) st         (750)    10663 2014-01-21 11:36:37.000000 PyAstronomy-0.8.1/src/pyasl/resBased/exoplanetsOrg.py
--rw-r--r--   0 steh312   (5677) st         (750)     4445 2014-04-29 12:44:10.000000 PyAstronomy-0.8.1/src/pyasl/resBased/exampleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)     5116 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/resBased/baraffe98tracks.py
--rw-r--r--   0 steh312   (5677) st         (750)    22573 2014-04-29 12:44:10.000000 PyAstronomy-0.8.1/src/pyasl/resBased/fip.dat
--rw-r--r--   0 steh312   (5677) st         (750)      163 2014-04-29 12:44:10.000000 PyAstronomy-0.8.1/src/pyasl/resBased/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)     7576 2013-03-08 13:54:07.000000 PyAstronomy-0.8.1/src/pyasl/resBased/nasaExoplanetArchive.py
--rw-r--r--   0 steh312   (5677) st         (750)     8107 2014-01-22 11:12:11.000000 PyAstronomy-0.8.1/src/pyasl/resBased/exoplanetEU.py
--rw-r--r--   0 steh312   (5677) st         (750)    11828 2014-04-02 12:05:55.000000 PyAstronomy-0.8.1/src/pyasl/resBased/kuruczModels.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyasl/asl/
--rw-r--r--   0 steh312   (5677) st         (750)      448 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/idlMod.py
--rw-r--r--   0 steh312   (5677) st         (750)      611 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/idlCirrange.py
--rw-r--r--   0 steh312   (5677) st         (750)     1276 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/planetPhase.py
--rw-r--r--   0 steh312   (5677) st         (750)     9208 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/sunpos.py
--rw-r--r--   0 steh312   (5677) st         (750)     2078 2015-01-08 14:00:41.000000 PyAstronomy-0.8.1/src/pyasl/asl/planck.py
--rw-r--r--   0 steh312   (5677) st         (750)     4109 2013-12-09 17:48:08.000000 PyAstronomy-0.8.1/src/pyasl/asl/estimateSNR.py
--rw-r--r--   0 steh312   (5677) st         (750)     2815 2013-11-25 11:50:12.000000 PyAstronomy-0.8.1/src/pyasl/asl/readFitsSpec.py
--rw-r--r--   0 steh312   (5677) st         (750)     6352 2014-03-25 08:48:39.000000 PyAstronomy-0.8.1/src/pyasl/asl/observatory.cfg
--rw-r--r--   0 steh312   (5677) st         (750)     7095 2014-11-20 10:06:56.000000 PyAstronomy-0.8.1/src/pyasl/asl/writeFitsSpec.py
--rw-r--r--   0 steh312   (5677) st         (750)     1540 2013-03-08 13:43:29.000000 PyAstronomy-0.8.1/src/pyasl/asl/localtime.py
--rw-r--r--   0 steh312   (5677) st         (750)    62043 2015-01-14 13:16:57.000000 PyAstronomy-0.8.1/src/pyasl/asl/sanityTest.py
--rw-r--r--   0 steh312   (5677) st         (750)    14275 2014-12-19 18:30:00.000000 PyAstronomy-0.8.1/src/pyasl/asl/test.py
--rw-r--r--   0 steh312   (5677) st         (750)     1187 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/pyasl/asl/cardinalPoint.py
--rw-r--r--   0 steh312   (5677) st         (750)     1628 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/planet_Teq.py
--rw-r--r--   0 steh312   (5677) st         (750)     6547 2014-11-07 09:35:24.000000 PyAstronomy-0.8.1/src/pyasl/asl/binning.py
--rw-r--r--   0 steh312   (5677) st         (750)     5277 2014-03-19 16:03:47.000000 PyAstronomy-0.8.1/src/pyasl/asl/broad.py
--rw-r--r--   0 steh312   (5677) st         (750)    21219 2014-03-21 10:48:24.000000 PyAstronomy-0.8.1/src/pyasl/asl/baryvel.py
--rw-r--r--   0 steh312   (5677) st         (750)     1156 2014-11-20 10:06:56.000000 PyAstronomy-0.8.1/src/pyasl/asl/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)    10914 2013-03-08 13:43:29.000000 PyAstronomy-0.8.1/src/pyasl/asl/moonpos.py
--rw-r--r--   0 steh312   (5677) st         (750)     2416 2014-04-02 12:05:55.000000 PyAstronomy-0.8.1/src/pyasl/asl/atomicNo.py
--rw-r--r--   0 steh312   (5677) st         (750)     3224 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/dopplerShift.py
--rw-r--r--   0 steh312   (5677) st         (750)     6544 2014-12-02 10:54:17.000000 PyAstronomy-0.8.1/src/pyasl/asl/crosscorr.py
--rw-r--r--   0 steh312   (5677) st         (750)     1601 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/lineOfSight.py
--rw-r--r--   0 steh312   (5677) st         (750)     1015 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/pyasl/asl/twilight.py
--rw-r--r--   0 steh312   (5677) st         (750)     1853 2013-03-08 13:43:29.000000 PyAstronomy-0.8.1/src/pyasl/asl/moonphase.py
--rw-r--r--   0 steh312   (5677) st         (750)    54107 2013-03-08 13:43:29.000000 PyAstronomy-0.8.1/src/pyasl/asl/eq2hor.py
--rw-r--r--   0 steh312   (5677) st         (750)     7447 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/rotBroad.py
--rw-r--r--   0 steh312   (5677) st         (750)     4412 2014-01-21 17:35:30.000000 PyAstronomy-0.8.1/src/pyasl/asl/posAngle.py
--rw-r--r--   0 steh312   (5677) st         (750)     1915 2014-04-02 12:05:55.000000 PyAstronomy-0.8.1/src/pyasl/asl/atomicNo.dat
--rw-r--r--   0 steh312   (5677) st         (750)     1834 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/pyasl/asl/airmass.py
--rw-r--r--   0 steh312   (5677) st         (750)     1395 2013-03-29 14:35:38.000000 PyAstronomy-0.8.1/src/pyasl/asl/lineWidth.py
--rw-r--r--   0 steh312   (5677) st         (750)     6996 2014-11-07 09:32:05.000000 PyAstronomy-0.8.1/src/pyasl/asl/outlier.py
--rw-r--r--   0 steh312   (5677) st         (750)    38887 2014-03-21 10:15:57.000000 PyAstronomy-0.8.1/src/pyasl/asl/astroTimeLegacy.py
--rw-r--r--   0 steh312   (5677) st         (750)     6484 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/unred.py
--rw-r--r--   0 steh312   (5677) st         (750)     2981 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/smooth.py
--rw-r--r--   0 steh312   (5677) st         (750)     7155 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/pyasl/asl/statTest.py
--rw-r--r--   0 steh312   (5677) st         (750)    15309 2014-12-22 10:36:22.000000 PyAstronomy-0.8.1/src/pyasl/asl/airtovac.py
--rw-r--r--   0 steh312   (5677) st         (750)    38111 2013-08-12 09:31:59.000000 PyAstronomy-0.8.1/src/pyasl/asl/inTransit.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyasl/asl/testPro/
--rw-r--r--   0 steh312   (5677) st         (750)     2154 2014-12-19 18:11:21.000000 PyAstronomy-0.8.1/src/pyasl/asl/testPro/airtovac.pro
--rw-r--r--   0 steh312   (5677) st         (750)     1785 2014-12-19 18:10:57.000000 PyAstronomy-0.8.1/src/pyasl/asl/testPro/vactoair.pro
--rw-r--r--   0 steh312   (5677) st         (750)    12217 2014-12-19 18:20:19.000000 PyAstronomy-0.8.1/src/pyasl/asl/testPro/test.pro
--rw-r--r--   0 steh312   (5677) st         (750)     3872 2015-01-14 09:13:03.000000 PyAstronomy-0.8.1/src/pyasl/asl/intep.py
--rw-r--r--   0 steh312   (5677) st         (750)     1219 2014-04-02 12:05:50.000000 PyAstronomy-0.8.1/src/pyasl/asl/magnitudes.py
--rw-r--r--   0 steh312   (5677) st         (750)     1033 2014-04-29 12:44:10.000000 PyAstronomy-0.8.1/src/pyasl/asl/folding.py
--rw-r--r--   0 steh312   (5677) st         (750)     1081 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/fluxConversion.py
--rw-r--r--   0 steh312   (5677) st         (750)     3192 2013-02-20 17:16:19.000000 PyAstronomy-0.8.1/src/pyasl/asl/observatory.py
--rw-r--r--   0 steh312   (5677) st         (750)     3610 2014-07-30 09:17:36.000000 PyAstronomy-0.8.1/src/pyasl/asl/quadextreme.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/
--rw-r--r--   0 steh312   (5677) st         (750)     2406 2015-01-08 11:02:58.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/expCorrRN.py
--rw-r--r--   0 steh312   (5677) st         (750)     7516 2015-02-25 09:33:17.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/sanityExt1Test.py
--rw-r--r--   0 steh312   (5677) st         (750)      132 2015-02-25 09:33:17.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)     1647 2015-02-25 09:33:17.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/ballesterosBV_T.py
--rw-r--r--   0 steh312   (5677) st         (750)     1800 2014-10-06 12:40:45.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/pizzolato2003tables.dat
--rw-r--r--   0 steh312   (5677) st         (750)     2408 2015-02-19 08:50:40.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/stellarAge.py
--rw-r--r--   0 steh312   (5677) st         (750)     4940 2014-10-06 12:40:45.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/pizzolato2003.py
--rw-r--r--   0 steh312   (5677) st         (750)    12905 2015-02-11 11:40:22.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/ramirez2005tables.dat
--rw-r--r--   0 steh312   (5677) st         (750)    13206 2015-02-12 10:59:07.000000 PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/ramirez2005.py
--rw-r--r--   0 steh312   (5677) st         (750)    18249 2015-02-14 15:16:08.000000 PyAstronomy-0.8.1/src/pyasl/asl/keplerOrbit.py
--rw-r--r--   0 steh312   (5677) st         (750)     3759 2015-01-14 13:02:14.000000 PyAstronomy-0.8.1/src/pyasl/asl/decimalYear.py
--rw-r--r--   0 steh312   (5677) st         (750)     6031 2014-10-06 17:33:06.000000 PyAstronomy-0.8.1/src/pyasl/asl/coordinates.py
--rw-r--r--   0 steh312   (5677) st         (750)      877 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/pyasl/asl/angularDistance.py
--rw-r--r--   0 steh312   (5677) st         (750)    11836 2015-03-01 17:00:33.000000 PyAstronomy-0.8.1/src/pyasl/asl/sindex.py
--rw-r--r--   0 steh312   (5677) st         (750)     6615 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/pyasl/asl/svd.py
--rw-r--r--   0 steh312   (5677) st         (750)     4061 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyasl/asl/aitoffLegacy.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/constants/
--rw-r--r--   0 steh312   (5677) st         (750)     1548 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/constants/exampleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)     6779 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/constants/itc.py
--rw-r--r--   0 steh312   (5677) st         (750)     3398 2014-03-19 15:26:05.000000 PyAstronomy-0.8.1/src/constants/cdat.dat
--rw-r--r--   0 steh312   (5677) st         (750)     5508 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/constants/__init__.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyaGui/
--rw-r--r--   0 steh312   (5677) st         (750)    23712 2015-02-14 13:11:02.000000 PyAstronomy-0.8.1/src/pyaGui/interactiveGV.py
--rw-r--r--   0 steh312   (5677) st         (750)     6343 2015-02-14 13:11:02.000000 PyAstronomy-0.8.1/src/pyaGui/exampleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)     7553 2014-07-30 09:17:36.000000 PyAstronomy-0.8.1/src/pyaGui/pyaPicker.py
--rw-r--r--   0 steh312   (5677) st         (750)      332 2015-02-14 13:11:02.000000 PyAstronomy-0.8.1/src/pyaGui/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)    28329 2014-08-05 16:34:41.000000 PyAstronomy-0.8.1/src/pyaGui/ffmodelExplorer.py
--rw-r--r--   0 steh312   (5677) st         (750)    19232 2014-11-04 14:54:21.000000 PyAstronomy-0.8.1/src/pyaGui/continuumFinder.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/funcFit/
--rw-r--r--   0 steh312   (5677) st         (750)    44324 2014-03-18 16:42:32.000000 PyAstronomy-0.8.1/src/funcFit/TutorialExampleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)    67804 2014-11-03 15:46:48.000000 PyAstronomy-0.8.1/src/funcFit/onedfit.py
--rw-r--r--   0 steh312   (5677) st         (750)     1750 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/funcFit/polyModel.py
--rw-r--r--   0 steh312   (5677) st         (750)     1487 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/funcFit/sinexp1d.py
--rw-r--r--   0 steh312   (5677) st         (750)      792 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/funcFit/cauchyLorentz1d.py
--rw-r--r--   0 steh312   (5677) st         (750)     5668 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/funcFit/nameIdentBase.py
--rw-r--r--   0 steh312   (5677) st         (750)     1703 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/funcFit/coordinateGrid.py
--rw-r--r--   0 steh312   (5677) st         (750)     7816 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/funcFit/extFitter.py
--rw-r--r--   0 steh312   (5677) st         (750)    28630 2015-01-14 09:13:14.000000 PyAstronomy-0.8.1/src/funcFit/params.py
--rw-r--r--   0 steh312   (5677) st         (750)     2304 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/funcFit/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)     3219 2014-07-29 14:50:06.000000 PyAstronomy-0.8.1/src/funcFit/gauss1d.py
--rw-r--r--   0 steh312   (5677) st         (750)     6346 2014-03-10 12:52:42.000000 PyAstronomy-0.8.1/src/funcFit/gauss2d.py
--rw-r--r--   0 steh312   (5677) st         (750)     2951 2014-03-18 16:48:37.000000 PyAstronomy-0.8.1/src/funcFit/funcFitSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)    17958 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/funcFit/syncFit.py
--rw-r--r--   0 steh312   (5677) st         (750)      963 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/funcFit/circle2d.py
--rw-r--r--   0 steh312   (5677) st         (750)     1384 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/funcFit/moduleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)    17475 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/funcFit/anneal.py
--rw-r--r--   0 steh312   (5677) st         (750)     1116 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/funcFit/fufDS.py
--rw-r--r--   0 steh312   (5677) st         (750)     5082 2013-11-08 17:13:02.000000 PyAstronomy-0.8.1/src/funcFit/voigt1d.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/funcFit/utils/
--rw-r--r--   0 steh312   (5677) st         (750)     1016 2013-11-18 16:21:12.000000 PyAstronomy-0.8.1/src/funcFit/utils/bayesFactors.py
--rw-r--r--   0 steh312   (5677) st         (750)    26791 2013-08-19 17:01:29.000000 PyAstronomy-0.8.1/src/funcFit/utils/anaMCMCTraces.py
--rw-r--r--   0 steh312   (5677) st         (750)      384 2014-03-11 16:08:17.000000 PyAstronomy-0.8.1/src/funcFit/utils/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)     4682 2013-08-14 09:22:08.000000 PyAstronomy-0.8.1/src/funcFit/modelRebin.py
--rw-r--r--   0 steh312   (5677) st         (750)       36 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/setup.cfg
--rw-r--r--   0 steh312   (5677) st         (750)     1196 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/__init__.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyTiming/
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyTiming/pyPeriod/
--rw-r--r--   0 steh312   (5677) st         (750)     4168 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyTiming/pyPeriod/lombScargle.py
--rw-r--r--   0 steh312   (5677) st         (750)     2275 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyTiming/pyPeriod/exampleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)     2443 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyTiming/pyPeriod/fourier.py
--rw-r--r--   0 steh312   (5677) st         (750)      488 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyTiming/pyPeriod/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)    10706 2013-11-08 17:42:17.000000 PyAstronomy-0.8.1/src/pyTiming/pyPeriod/gls.py
--rw-r--r--   0 steh312   (5677) st         (750)     5444 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyTiming/pyPeriod/periodBase.py
--rw-r--r--   0 steh312   (5677) st         (750)       29 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyTiming/__init__.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyTiming/pyPDM/
--rw-r--r--   0 steh312   (5677) st         (750)     1674 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyTiming/pyPDM/exampleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)      104 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyTiming/pyPDM/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)    10322 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyTiming/pyPDM/pdm.py
--rw-r--r--   0 steh312   (5677) st         (750)       37 2015-03-01 17:15:22.000000 PyAstronomy-0.8.1/src/PyA_Version.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyaC/
--rw-r--r--   0 steh312   (5677) st         (750)     2758 2013-04-17 10:42:26.000000 PyAstronomy-0.8.1/src/pyaC/numericalDerivatives.py
--rw-r--r--   0 steh312   (5677) st         (750)      560 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/pyaC/conversions.py
--rw-r--r--   0 steh312   (5677) st         (750)     4105 2013-08-07 12:14:33.000000 PyAstronomy-0.8.1/src/pyaC/output.py
--rw-r--r--   0 steh312   (5677) st         (750)      367 2013-08-15 12:56:07.000000 PyAstronomy-0.8.1/src/pyaC/__init__.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyaC/pyaErrors/
--rw-r--r--   0 steh312   (5677) st         (750)     2209 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyaC/pyaErrors/pyaErrTemplate.py
--rw-r--r--   0 steh312   (5677) st         (750)      827 2013-08-15 13:45:58.000000 PyAstronomy-0.8.1/src/pyaC/pyaErrors/pyaValErrs.py
--rw-r--r--   0 steh312   (5677) st         (750)     3317 2014-08-05 16:32:25.000000 PyAstronomy-0.8.1/src/pyaC/pyaErrors/pyaOtherErrors.py
--rw-r--r--   0 steh312   (5677) st         (750)       72 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyaC/pyaErrors/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)      463 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyaC/pyaErrors/warn.py
--rw-r--r--   0 steh312   (5677) st         (750)     2995 2013-08-15 13:15:55.000000 PyAstronomy-0.8.1/src/pyaC/simiof.py
--rw-r--r--   0 steh312   (5677) st         (750)      917 2013-04-17 08:59:26.000000 PyAstronomy-0.8.1/src/pyaC/centralFiniteDiff.dat
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/pyaC/pyaPermanent/
--rw-r--r--   0 steh312   (5677) st         (750)     6840 2013-03-08 13:43:29.000000 PyAstronomy-0.8.1/src/pyaC/pyaPermanent/pyaFS.py
--rw-r--r--   0 steh312   (5677) st         (750)     8966 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyaC/pyaPermanent/pyaConfig.py
--rw-r--r--   0 steh312   (5677) st         (750)     4586 2013-03-08 13:54:07.000000 PyAstronomy-0.8.1/src/pyaC/pyaPermanent/updateCycler.py
--rw-r--r--   0 steh312   (5677) st         (750)       83 2013-03-08 13:54:07.000000 PyAstronomy-0.8.1/src/pyaC/pyaPermanent/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)     1272 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyaC/importCheck.py
--rw-r--r--   0 steh312   (5677) st         (750)     1449 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyaC/invertIndexSelection.py
--rw-r--r--   0 steh312   (5677) st         (750)      230 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyaC/sanity.py
--rw-r--r--   0 steh312   (5677) st         (750)     2433 2013-03-08 13:43:29.000000 PyAstronomy-0.8.1/src/pyaC/fuzzyMatch.py
--rw-r--r--   0 steh312   (5677) st         (750)     2659 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/pyaC/nestedLoop.py
--rw-r--r--   0 steh312   (5677) st         (750)     5595 2013-08-15 13:05:58.000000 PyAstronomy-0.8.1/src/pyaC/sanityNeedfThings.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/modelSuite/
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/
--rw-r--r--   0 steh312   (5677) st         (750)     1214 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palMandelSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)    10946 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/rmcl_ohta.py
--rw-r--r--   0 steh312   (5677) st         (750)     4843 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/limBrightTrans.py
--rw-r--r--   0 steh312   (5677) st         (750)      146 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)     3690 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/circKepZList.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/
--rw-r--r--   0 steh312   (5677) st         (750)     3562 2013-04-19 11:05:25.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/mandelAgol.py
--rw-r--r--   0 steh312   (5677) st         (750)     2448 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/exampleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)     5038 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/occultnl.f
--rw-r--r--   0 steh312   (5677) st         (750)     1630 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/occultquad.pyf
--rw-r--r--   0 steh312   (5677) st         (750)       51 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)     1117 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/occultnl.pyf
--rw-r--r--   0 steh312   (5677) st         (750)    10336 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/occultquad.f
--rw-r--r--   0 steh312   (5677) st         (750)     3531 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/mandelAgolNL.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/
--rw-r--r--   0 steh312   (5677) st         (750)     4660 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/exampleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)     2591 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/seconPal.py
--rw-r--r--   0 steh312   (5677) st         (750)       40 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/__init__.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/ellint/
--rw-r--r--   0 steh312   (5677) st         (750)      810 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/ellint/ell.cpp
--rw-r--r--   0 steh312   (5677) st         (750)      611 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/ellint/makefile_template
--rw-r--r--   0 steh312   (5677) st         (750)    15519 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/pal.py
--rw-r--r--   0 steh312   (5677) st         (750)     1812 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/palSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)    11708 2014-02-26 16:27:34.000000 PyAstronomy-0.8.1/src/modelSuite/exampleSanity.py
--rw-r--r--   0 steh312   (5677) st         (750)      548 2014-02-26 14:39:59.000000 PyAstronomy-0.8.1/src/modelSuite/__init__.py
--rw-r--r--   0 steh312   (5677) st         (750)     1063 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/radVel.py
--rw-r--r--   0 steh312   (5677) st         (750)     2303 2013-03-29 14:35:38.000000 PyAstronomy-0.8.1/src/modelSuite/voigtAstro.py
--rw-r--r--   0 steh312   (5677) st         (750)     2818 2014-05-20 09:38:03.000000 PyAstronomy-0.8.1/src/modelSuite/keplerEllipseModel.py
--rw-r--r--   0 steh312   (5677) st         (750)     2391 2013-03-29 14:35:38.000000 PyAstronomy-0.8.1/src/modelSuite/LyAProfile.py
--rw-r--r--   0 steh312   (5677) st         (750)     9743 2014-07-30 09:17:36.000000 PyAstronomy-0.8.1/src/modelSuite/lineListGaussModel.py
--rw-r--r--   0 steh312   (5677) st         (750)     2826 2014-03-20 09:42:28.000000 PyAstronomy-0.8.1/src/modelSuite/rotBroadProfile.py
--rw-r--r--   0 steh312   (5677) st         (750)      498 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/planetBrightnessPhases.py
--rw-r--r--   0 steh312   (5677) st         (750)     5584 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/modelSuite/atanProfile.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/
--rw-r--r--   0 steh312   (5677) st         (750)     1238 2014-09-30 15:17:11.000000 PyAstronomy-0.8.1/src/doc/index.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1265 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/license.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/
--rw-r--r--   0 steh312   (5677) st         (750)      281 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/index.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPeriodDoc/
--rw-r--r--   0 steh312   (5677) st         (750)      424 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPeriodDoc/pyPeriod.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2269 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPeriodDoc/examples.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1613 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPeriodDoc/periodograms.rst
--rw-r--r--   0 steh312   (5677) st         (750)      722 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPeriodDoc/baseClasses.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPDMDoc/
--rw-r--r--   0 steh312   (5677) st         (750)     1761 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPDMDoc/examples.rst
--rw-r--r--   0 steh312   (5677) st         (750)      516 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPDMDoc/pdm.rst
--rw-r--r--   0 steh312   (5677) st         (750)      361 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPDMDoc/classes.rst
--rw-r--r--   0 steh312   (5677) st         (750)     7890 2015-02-18 09:39:02.000000 PyAstronomy-0.8.1/src/doc/conf.py
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/
--rw-r--r--   0 steh312   (5677) st         (750)     2202 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/installingPyA.rst
--rw-r--r--   0 steh312   (5677) st         (750)      434 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/index.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaPermanentDoc/
--rw-r--r--   0 steh312   (5677) st         (750)     1532 2013-03-08 13:54:07.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaPermanentDoc/index.rst
--rw-r--r--   0 steh312   (5677) st         (750)      224 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaPermanentDoc/pyaFS.rst
--rw-r--r--   0 steh312   (5677) st         (750)      812 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaPermanentDoc/pyaConfig.rst
--rw-r--r--   0 steh312   (5677) st         (750)      145 2013-03-08 13:54:07.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaPermanentDoc/updateCycler.rst
--rw-r--r--   0 steh312   (5677) st         (750)     3724 2013-08-15 13:01:38.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/needfulThings.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaErrorsDoc/
--rw-r--r--   0 steh312   (5677) st         (750)      712 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaErrorsDoc/index.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2349 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaErrorsDoc/pyaExTemplate.rst
--rw-r--r--   0 steh312   (5677) st         (750)      201 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaErrorsDoc/showWarning.rst
--rw-r--r--   0 steh312   (5677) st         (750)      452 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaErrorsDoc/pyaExceptions.rst
--rw-r--r--   0 steh312   (5677) st         (750)      778 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/whatIsIt.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1115 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/versioning.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1505 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/IDLPorting.rst
--rw-r--r--   0 steh312   (5677) st         (750)      375 2014-09-30 15:17:11.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/acknowledgement.rst
--rw-r--r--   0 steh312   (5677) st         (750)      382 2014-02-10 16:58:55.000000 PyAstronomy-0.8.1/src/doc/pyaCDoc/cont.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/changeLog/
--rw-r--r--   0 steh312   (5677) st         (750)      478 2014-03-13 10:39:13.000000 PyAstronomy-0.8.1/src/doc/changeLog/index.rst
--rw-r--r--   0 steh312   (5677) st         (750)      952 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/changeLog/from020to030.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1284 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/changeLog/from040to050.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1343 2014-03-11 13:30:42.000000 PyAstronomy-0.8.1/src/doc/changeLog/from060to070.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1636 2013-04-02 12:57:30.000000 PyAstronomy-0.8.1/src/doc/changeLog/from050to060.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1029 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/changeLog/from030to040.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1434 2015-02-19 08:50:40.000000 PyAstronomy-0.8.1/src/doc/changeLog/from070to080.rst
--rw-r--r--   0 steh312   (5677) st         (750)     4826 2015-02-26 17:06:21.000000 PyAstronomy-0.8.1/src/doc/Makefile
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/phoenixUtils/
--rw-r--r--   0 steh312   (5677) st         (750)      480 2015-02-25 09:56:54.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/phoenixUtils/phoenixUtils.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/
--rw-r--r--   0 steh312   (5677) st         (750)     1033 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aberration.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1411 2013-08-15 08:58:52.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/crosscorr.rst
--rw-r--r--   0 steh312   (5677) st         (750)      855 2014-03-19 09:52:43.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/broad.rst
--rw-r--r--   0 steh312   (5677) st         (750)      453 2013-03-29 14:35:38.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/lineWidth.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1183 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/estimateSNR.rst
--rw-r--r--   0 steh312   (5677) st         (750)      855 2013-09-26 11:32:28.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/magnitudes.rst
--rw-r--r--   0 steh312   (5677) st         (750)   196510 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/transVis-WASP-7b.png
--rw-r--r--   0 steh312   (5677) st         (750)      441 2014-04-02 12:05:55.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/atomicNo.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1891 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/coorTimeDate.rst
--rw-r--r--   0 steh312   (5677) st         (750)      718 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/unredDoc.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/
--rw-r--r--   0 steh312   (5677) st         (750)      770 2015-02-19 08:50:40.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/stellarAge.rst
--rw-r--r--   0 steh312   (5677) st         (750)      930 2014-10-06 12:40:45.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/pizzolato2003Doc.rst
--rw-r--r--   0 steh312   (5677) st         (750)     4127 2015-02-25 09:33:17.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/ramirez2005.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1665 2015-01-08 11:02:58.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/expCorrRN.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1040 2014-09-30 15:17:11.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/coordinates.rst
--rw-r--r--   0 steh312   (5677) st         (750)     3313 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/transitVisibility.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1862 2014-03-20 17:40:28.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/baryvel.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1904 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/nutate.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2619 2015-02-14 13:11:02.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/dopplerShift.rst
--rw-r--r--   0 steh312   (5677) st         (750)      508 2013-02-20 17:16:19.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/observatory.rst
--rw-r--r--   0 steh312   (5677) st         (750)      538 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/cardinalPoint.rst
--rw-r--r--   0 steh312   (5677) st         (750)      741 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/transitDuration.rst
--rw-r--r--   0 steh312   (5677) st         (750)      197 2014-03-19 16:11:37.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/broadening.rst
--rw-r--r--   0 steh312   (5677) st         (750)      905 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/airmass.rst
--rw-r--r--   0 steh312   (5677) st         (750)      365 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/twilight.rst
--rw-r--r--   0 steh312   (5677) st         (750)      631 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/fluxConversion.rst
--rw-r--r--   0 steh312   (5677) st         (750)      373 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/keplerOrbitAPI.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1001 2014-11-20 10:06:56.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/readFitsSpec.rst
--rw-r--r--   0 steh312   (5677) st         (750)     4893 2014-12-22 10:42:09.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/pyasl_wvlconv.rst
--rw-r--r--   0 steh312   (5677) st         (750)      618 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/pyaslAitoff.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1362 2013-03-08 13:43:29.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/moon.rst
--rw-r--r--   0 steh312   (5677) st         (750)       91 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/statTest.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2772 2013-07-19 15:14:02.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/binning.rst
--rw-r--r--   0 steh312   (5677) st         (750)     4096 2014-11-07 09:32:05.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/outlier.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1217 2014-03-18 15:36:55.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/sindex.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2651 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/svd.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1599 2013-08-15 09:18:13.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/quadextreme.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1273 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/inTran.rst
--rw-r--r--   0 steh312   (5677) st         (750)      537 2014-01-22 10:35:15.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/posAngle.rst
--rw-r--r--   0 steh312   (5677) st         (750)      187 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/planetPhase.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2985 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/rotBroad.rst
--rw-r--r--   0 steh312   (5677) st         (750)      986 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/sunpos.rst
--rw-r--r--   0 steh312   (5677) st         (750)      832 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/folding.rst
--rw-r--r--   0 steh312   (5677) st         (750)      675 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/intep.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2448 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/keplerOrbit.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2292 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/eq2hor.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1737 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/altitude.rst
--rw-r--r--   0 steh312   (5677) st         (750)      110 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/planck.rst
--rw-r--r--   0 steh312   (5677) st         (750)      118 2014-03-19 16:09:23.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/thermalBroad.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1026 2015-01-14 13:13:00.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/decimalYear.rst
--rw-r--r--   0 steh312   (5677) st         (750)      444 2013-04-02 12:55:35.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/angularDistance.rst
--rw-r--r--   0 steh312   (5677) st         (750)      720 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/smooth.rst
--rw-r--r--   0 steh312   (5677) st         (750)     3626 2015-02-25 11:18:21.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/pyasl.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:47.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/
--rw-r--r--   0 steh312   (5677) st         (750)      739 2014-04-29 12:44:10.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/fip.rst
--rw-r--r--   0 steh312   (5677) st         (750)      618 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/exoplanetsOrg.rst
--rw-r--r--   0 steh312   (5677) st         (750)      626 2013-03-08 13:54:07.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/exoplanetEU.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1108 2014-03-26 12:32:30.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/kuruczModels.rst
--rw-r--r--   0 steh312   (5677) st         (750)      706 2013-03-08 13:54:07.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/nasaExoplanetArchive.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1167 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/baraffe98tracks.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/logo/
--rw-r--r--   0 steh312   (5677) st         (750)     7040 2015-02-18 09:39:02.000000 PyAstronomy-0.8.1/src/doc/logo/pyalogo.png
--rw-r--r--   0 steh312   (5677) st         (750)    13790 2015-02-18 09:39:02.000000 PyAstronomy-0.8.1/src/doc/logo/pyafavicon.ico
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/pyaGuiDoc/
--rw-r--r--   0 steh312   (5677) st         (750)      137 2015-02-14 13:11:02.000000 PyAstronomy-0.8.1/src/doc/pyaGuiDoc/index.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1851 2014-08-05 16:44:06.000000 PyAstronomy-0.8.1/src/doc/pyaGuiDoc/modelExplorer.rst
--rw-r--r--   0 steh312   (5677) st         (750)      714 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/pyaGuiDoc/pyapicker.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1912 2014-07-31 15:55:35.000000 PyAstronomy-0.8.1/src/doc/pyaGuiDoc/continuumFinder.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2459 2015-02-14 13:11:02.000000 PyAstronomy-0.8.1/src/doc/pyaGuiDoc/interactiveGV.rst
--rw-r--r--   0 steh312   (5677) st         (750)      156 2014-02-10 15:17:28.000000 PyAstronomy-0.8.1/src/doc/PyAGroup.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/constantsDoc/
--rw-r--r--   0 steh312   (5677) st         (750)     6277 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/constantsDoc/index.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/
--rw-r--r--   0 steh312   (5677) st         (750)     1495 2014-03-10 12:52:42.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/index.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1623 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/nelderMead.rst
--rw-r--r--   0 steh312   (5677) st         (750)     9713 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/tutorial2.rst
--rw-r--r--   0 steh312   (5677) st         (750)     3836 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/onedfit.rst
--rw-r--r--   0 steh312   (5677) st         (750)    47317 2014-03-18 16:41:57.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/tutorial.rst
--rw-r--r--   0 steh312   (5677) st         (750)      118 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/params.rst
--rw-r--r--   0 steh312   (5677) st         (750)      271 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/coordinateGrid.rst
--rw-r--r--   0 steh312   (5677) st         (750)      167 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/fufDS.rst
--rw-r--r--   0 steh312   (5677) st         (750)      808 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/modelRebin.rst
--rw-r--r--   0 steh312   (5677) st         (750)      449 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/extFitters.rst
--rw-r--r--   0 steh312   (5677) st         (750)     7313 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/traceAnalysisTutorial.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2215 2014-03-10 12:52:42.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/simplemodels.rst
--rw-r--r--   0 steh312   (5677) st         (750)      446 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/syncFit.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1634 2013-02-05 14:13:18.000000 PyAstronomy-0.8.1/src/doc/funcFitDoc/traceAnalysis.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/
--rw-r--r--   0 steh312   (5677) st         (750)      684 2014-02-26 14:43:12.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/index.rst
--rw-r--r--   0 steh312   (5677) st         (750)      965 2014-02-26 15:21:12.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/rotBroadProfile.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/
--rw-r--r--   0 steh312   (5677) st         (750)      737 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/palRebin.rst
--rw-r--r--   0 steh312   (5677) st         (750)      529 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/pal.rst
--rw-r--r--   0 steh312   (5677) st         (750)     5005 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/exams.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1586 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/boostsupport.rst
--rw-r--r--   0 steh312   (5677) st         (750)      510 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/palTrans.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/radVelDoc/
--rw-r--r--   0 steh312   (5677) st         (750)     1792 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/radVelDoc/radVel.rst
--rw-r--r--   0 steh312   (5677) st         (750)     3401 2015-02-18 09:38:06.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/forTrans.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2612 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/keplerEllipseModelDoc.rst
--rw-r--r--   0 steh312   (5677) st         (750)      683 2013-03-29 14:35:38.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/astroVoigt.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1965 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/lineListGaussModelDoc.rst
--rw-r--r--   0 steh312   (5677) st         (750)      574 2013-03-29 14:35:38.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/LyAProfile.rst
-drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-03-01 17:24:46.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/RmcLOhtaDoc/
--rw-r--r--   0 steh312   (5677) st         (750)      728 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/RmcLOhtaDoc/index.rst
--rw-r--r--   0 steh312   (5677) st         (750)      229 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/RmcLOhtaDoc/rmcl.rst
--rw-r--r--   0 steh312   (5677) st         (750)     2376 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/RmcLOhtaDoc/rmclExamples.rst
--rw-r--r--   0 steh312   (5677) st         (750)      573 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/xtranDoc.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1367 2013-02-06 13:17:26.000000 PyAstronomy-0.8.1/src/doc/modelSuiteDoc/limBrightTrans.rst
--rw-r--r--   0 steh312   (5677) st         (750)     1600 2013-09-25 16:08:06.000000 PyAstronomy-0.8.1/README
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/
+-rw-r--r--   0 steh312   (5677) st         (750)      313 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/PKG-INFO
+-rw-r--r--   0 steh312   (5677) st         (750)     6893 2015-03-05 09:32:12.000000 PyAstronomy-0.9.0/setup.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyasl/
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyasl/phoenixUtils/
+-rw-r--r--   0 steh312   (5677) st         (750)     3824 2015-02-25 10:55:52.000000 PyAstronomy-0.9.0/src/pyasl/phoenixUtils/read.py
+-rw-r--r--   0 steh312   (5677) st         (750)       18 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/phoenixUtils/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)      277 2015-10-30 16:28:18.000000 PyAstronomy-0.9.0/src/pyasl/__init__.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyasl/resBased/
+-rw-r--r--   0 steh312   (5677) st         (750)     3575 2014-04-29 12:44:10.000000 PyAstronomy-0.9.0/src/pyasl/resBased/fip.py
+-rw-r--r--   0 steh312   (5677) st         (750)    10663 2015-06-02 12:55:47.000000 PyAstronomy-0.9.0/src/pyasl/resBased/exoplanetsOrg.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4455 2015-05-22 08:42:22.000000 PyAstronomy-0.9.0/src/pyasl/resBased/exampleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)     5116 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/resBased/baraffe98tracks.py
+-rw-r--r--   0 steh312   (5677) st         (750)    22573 2014-04-29 12:44:10.000000 PyAstronomy-0.9.0/src/pyasl/resBased/fip.dat
+-rw-r--r--   0 steh312   (5677) st         (750)      187 2015-05-22 08:42:22.000000 PyAstronomy-0.9.0/src/pyasl/resBased/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)     7576 2013-03-08 13:54:07.000000 PyAstronomy-0.9.0/src/pyasl/resBased/nasaExoplanetArchive.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4898 2015-06-02 12:55:50.000000 PyAstronomy-0.9.0/src/pyasl/resBased/sweet_cat.py
+-rw-r--r--   0 steh312   (5677) st         (750)     8753 2015-06-02 12:55:47.000000 PyAstronomy-0.9.0/src/pyasl/resBased/exoplanetEU.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1091 2015-05-22 08:42:22.000000 PyAstronomy-0.9.0/src/pyasl/resBased/exampleSanity_future.py
+-rw-r--r--   0 steh312   (5677) st         (750)    11828 2014-04-02 12:05:55.000000 PyAstronomy-0.9.0/src/pyasl/resBased/kuruczModels.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyasl/asl/
+-rw-r--r--   0 steh312   (5677) st         (750)      448 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/idlMod.py
+-rw-r--r--   0 steh312   (5677) st         (750)      611 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/idlCirrange.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1276 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/planetPhase.py
+-rw-r--r--   0 steh312   (5677) st         (750)     9208 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/sunpos.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2078 2015-01-08 14:00:41.000000 PyAstronomy-0.9.0/src/pyasl/asl/planck.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4109 2013-12-09 17:48:08.000000 PyAstronomy-0.9.0/src/pyasl/asl/estimateSNR.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2815 2013-11-25 11:50:12.000000 PyAstronomy-0.9.0/src/pyasl/asl/readFitsSpec.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6532 2015-08-28 13:02:03.000000 PyAstronomy-0.9.0/src/pyasl/asl/observatory.cfg
+-rw-r--r--   0 steh312   (5677) st         (750)     7095 2014-11-20 10:06:56.000000 PyAstronomy-0.9.0/src/pyasl/asl/writeFitsSpec.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1540 2013-03-08 13:43:29.000000 PyAstronomy-0.9.0/src/pyasl/asl/localtime.py
+-rw-r--r--   0 steh312   (5677) st         (750)    67865 2015-08-17 09:10:59.000000 PyAstronomy-0.9.0/src/pyasl/asl/sanityTest.py
+-rw-r--r--   0 steh312   (5677) st         (750)    14275 2014-12-19 18:30:00.000000 PyAstronomy-0.9.0/src/pyasl/asl/test.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1187 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/pyasl/asl/cardinalPoint.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1628 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/planet_Teq.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6547 2014-11-07 09:35:24.000000 PyAstronomy-0.9.0/src/pyasl/asl/binning.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6077 2015-08-17 08:40:29.000000 PyAstronomy-0.9.0/src/pyasl/asl/broad.py
+-rw-r--r--   0 steh312   (5677) st         (750)    21219 2014-03-21 10:48:24.000000 PyAstronomy-0.9.0/src/pyasl/asl/baryvel.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1156 2015-05-19 13:20:48.000000 PyAstronomy-0.9.0/src/pyasl/asl/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)    10914 2013-03-08 13:43:29.000000 PyAstronomy-0.9.0/src/pyasl/asl/moonpos.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2416 2014-04-02 12:05:55.000000 PyAstronomy-0.9.0/src/pyasl/asl/atomicNo.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3224 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/dopplerShift.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6724 2015-10-27 14:53:34.000000 PyAstronomy-0.9.0/src/pyasl/asl/crosscorr.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1601 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/lineOfSight.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1015 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/pyasl/asl/twilight.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1853 2013-03-08 13:43:29.000000 PyAstronomy-0.9.0/src/pyasl/asl/moonphase.py
+-rw-r--r--   0 steh312   (5677) st         (750)    54107 2013-03-08 13:43:29.000000 PyAstronomy-0.9.0/src/pyasl/asl/eq2hor.py
+-rw-r--r--   0 steh312   (5677) st         (750)     7447 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/rotBroad.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4412 2014-01-21 17:35:30.000000 PyAstronomy-0.9.0/src/pyasl/asl/posAngle.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1915 2014-04-02 12:05:55.000000 PyAstronomy-0.9.0/src/pyasl/asl/atomicNo.dat
+-rw-r--r--   0 steh312   (5677) st         (750)     1834 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/pyasl/asl/airmass.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1395 2013-03-29 14:35:38.000000 PyAstronomy-0.9.0/src/pyasl/asl/lineWidth.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6996 2014-11-07 09:32:05.000000 PyAstronomy-0.9.0/src/pyasl/asl/outlier.py
+-rw-r--r--   0 steh312   (5677) st         (750)    38887 2014-03-21 10:15:57.000000 PyAstronomy-0.9.0/src/pyasl/asl/astroTimeLegacy.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6484 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/unred.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2981 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/smooth.py
+-rw-r--r--   0 steh312   (5677) st         (750)     7155 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/pyasl/asl/statTest.py
+-rw-r--r--   0 steh312   (5677) st         (750)    16728 2015-05-18 15:26:54.000000 PyAstronomy-0.9.0/src/pyasl/asl/airtovac.py
+-rw-r--r--   0 steh312   (5677) st         (750)    38111 2013-08-12 09:31:59.000000 PyAstronomy-0.9.0/src/pyasl/asl/inTransit.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyasl/asl/testPro/
+-rw-r--r--   0 steh312   (5677) st         (750)     2154 2014-12-19 18:11:21.000000 PyAstronomy-0.9.0/src/pyasl/asl/testPro/airtovac.pro
+-rw-r--r--   0 steh312   (5677) st         (750)     1785 2014-12-19 18:10:57.000000 PyAstronomy-0.9.0/src/pyasl/asl/testPro/vactoair.pro
+-rw-r--r--   0 steh312   (5677) st         (750)    12217 2014-12-19 18:20:19.000000 PyAstronomy-0.9.0/src/pyasl/asl/testPro/test.pro
+-rw-r--r--   0 steh312   (5677) st         (750)     3872 2015-01-14 09:13:03.000000 PyAstronomy-0.9.0/src/pyasl/asl/intep.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1219 2014-04-02 12:05:50.000000 PyAstronomy-0.9.0/src/pyasl/asl/magnitudes.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1033 2014-04-29 12:44:10.000000 PyAstronomy-0.9.0/src/pyasl/asl/folding.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1081 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/fluxConversion.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3192 2013-02-20 17:16:19.000000 PyAstronomy-0.9.0/src/pyasl/asl/observatory.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3610 2014-07-30 09:17:36.000000 PyAstronomy-0.9.0/src/pyasl/asl/quadextreme.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/
+-rw-r--r--   0 steh312   (5677) st         (750)     2406 2015-01-08 11:02:58.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/expCorrRN.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2538 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/abundances.dat
+-rw-r--r--   0 steh312   (5677) st         (750)     8647 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/sanityExt1Test.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4424 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/abundances.py
+-rw-r--r--   0 steh312   (5677) st         (750)      157 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1647 2015-02-25 09:33:17.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/ballesterosBV_T.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1800 2014-10-06 12:40:45.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/pizzolato2003tables.dat
+-rw-r--r--   0 steh312   (5677) st         (750)     2408 2015-02-19 08:50:40.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/stellarAge.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4940 2014-10-06 12:40:45.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/pizzolato2003.py
+-rw-r--r--   0 steh312   (5677) st         (750)    12905 2015-02-11 11:40:22.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/ramirez2005tables.dat
+-rw-r--r--   0 steh312   (5677) st         (750)    13206 2015-02-12 10:59:07.000000 PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/ramirez2005.py
+-rw-r--r--   0 steh312   (5677) st         (750)    23127 2015-05-20 14:12:02.000000 PyAstronomy-0.9.0/src/pyasl/asl/keplerOrbit.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3759 2015-01-14 13:02:14.000000 PyAstronomy-0.9.0/src/pyasl/asl/decimalYear.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6031 2014-10-06 17:33:06.000000 PyAstronomy-0.9.0/src/pyasl/asl/coordinates.py
+-rw-r--r--   0 steh312   (5677) st         (750)      877 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/pyasl/asl/angularDistance.py
+-rw-r--r--   0 steh312   (5677) st         (750)    11836 2015-03-01 17:00:33.000000 PyAstronomy-0.9.0/src/pyasl/asl/sindex.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6615 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/pyasl/asl/svd.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4061 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyasl/asl/aitoffLegacy.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/constants/
+-rw-r--r--   0 steh312   (5677) st         (750)     1548 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/constants/exampleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6779 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/constants/itc.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3398 2014-03-19 15:26:05.000000 PyAstronomy-0.9.0/src/constants/cdat.dat
+-rw-r--r--   0 steh312   (5677) st         (750)     5508 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/constants/__init__.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyaGui/
+-rw-r--r--   0 steh312   (5677) st         (750)    23712 2015-02-14 13:11:02.000000 PyAstronomy-0.9.0/src/pyaGui/interactiveGV.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6343 2015-02-14 13:11:02.000000 PyAstronomy-0.9.0/src/pyaGui/exampleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)     7553 2014-07-30 09:17:36.000000 PyAstronomy-0.9.0/src/pyaGui/pyaPicker.py
+-rw-r--r--   0 steh312   (5677) st         (750)      332 2015-02-14 13:11:02.000000 PyAstronomy-0.9.0/src/pyaGui/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)    29114 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/pyaGui/ffmodelExplorer.py
+-rw-r--r--   0 steh312   (5677) st         (750)    19232 2014-11-04 14:54:21.000000 PyAstronomy-0.9.0/src/pyaGui/continuumFinder.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/funcFit/
+-rw-r--r--   0 steh312   (5677) st         (750)    49803 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/funcFit/TutorialExampleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)    86004 2015-08-25 13:15:55.000000 PyAstronomy-0.9.0/src/funcFit/onedfit.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1750 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/funcFit/polyModel.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1487 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/funcFit/sinexp1d.py
+-rw-r--r--   0 steh312   (5677) st         (750)      792 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/funcFit/cauchyLorentz1d.py
+-rw-r--r--   0 steh312   (5677) st         (750)     5668 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/funcFit/nameIdentBase.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1703 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/funcFit/coordinateGrid.py
+-rw-r--r--   0 steh312   (5677) st         (750)     7972 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/funcFit/extFitter.py
+-rw-r--r--   0 steh312   (5677) st         (750)    28748 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/funcFit/params.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2905 2015-11-04 10:09:34.000000 PyAstronomy-0.9.0/src/funcFit/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3227 2015-03-25 13:46:56.000000 PyAstronomy-0.9.0/src/funcFit/gauss1d.py
+-rw-r--r--   0 steh312   (5677) st         (750)     6346 2014-03-10 12:52:42.000000 PyAstronomy-0.9.0/src/funcFit/gauss2d.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2951 2014-03-18 16:48:37.000000 PyAstronomy-0.9.0/src/funcFit/funcFitSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)    17958 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/funcFit/syncFit.py
+-rw-r--r--   0 steh312   (5677) st         (750)      963 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/funcFit/circle2d.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1384 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/funcFit/moduleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)    17475 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/funcFit/anneal.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1661 2015-08-25 12:52:50.000000 PyAstronomy-0.9.0/src/funcFit/fufDS.py
+-rw-r--r--   0 steh312   (5677) st         (750)     5097 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/funcFit/voigt1d.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/funcFit/utils/
+-rw-r--r--   0 steh312   (5677) st         (750)     1302 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/funcFit/utils/bayesFactors.py
+-rw-r--r--   0 steh312   (5677) st         (750)    30057 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/funcFit/utils/anaMCMCTraces.py
+-rw-r--r--   0 steh312   (5677) st         (750)      303 2015-11-04 10:09:58.000000 PyAstronomy-0.9.0/src/funcFit/utils/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4682 2013-08-14 09:22:08.000000 PyAstronomy-0.9.0/src/funcFit/modelRebin.py
+-rw-r--r--   0 steh312   (5677) st         (750)       36 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/setup.cfg
+-rw-r--r--   0 steh312   (5677) st         (750)     1196 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/__init__.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyTiming/
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyTiming/pyPeriod/
+-rw-r--r--   0 steh312   (5677) st         (750)     4168 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyTiming/pyPeriod/lombScargle.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2275 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyTiming/pyPeriod/exampleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2443 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyTiming/pyPeriod/fourier.py
+-rw-r--r--   0 steh312   (5677) st         (750)      488 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyTiming/pyPeriod/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)    10706 2013-11-08 17:42:17.000000 PyAstronomy-0.9.0/src/pyTiming/pyPeriod/gls.py
+-rw-r--r--   0 steh312   (5677) st         (750)     5444 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyTiming/pyPeriod/periodBase.py
+-rw-r--r--   0 steh312   (5677) st         (750)       29 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyTiming/__init__.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyTiming/pyPDM/
+-rw-r--r--   0 steh312   (5677) st         (750)     1674 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyTiming/pyPDM/exampleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)      104 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyTiming/pyPDM/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)    10322 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyTiming/pyPDM/pdm.py
+-rw-r--r--   0 steh312   (5677) st         (750)       37 2015-10-30 13:42:20.000000 PyAstronomy-0.9.0/src/PyA_Version.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyaC/
+-rw-r--r--   0 steh312   (5677) st         (750)      560 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/pyaC/conversions.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4105 2013-08-07 12:14:33.000000 PyAstronomy-0.9.0/src/pyaC/output.py
+-rw-r--r--   0 steh312   (5677) st         (750)      363 2015-03-05 10:09:01.000000 PyAstronomy-0.9.0/src/pyaC/__init__.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyaC/pyaErrors/
+-rw-r--r--   0 steh312   (5677) st         (750)     2246 2015-08-25 14:23:42.000000 PyAstronomy-0.9.0/src/pyaC/pyaErrors/pyaErrTemplate.py
+-rw-r--r--   0 steh312   (5677) st         (750)      827 2013-08-15 13:45:58.000000 PyAstronomy-0.9.0/src/pyaC/pyaErrors/pyaValErrs.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3317 2014-08-05 16:32:25.000000 PyAstronomy-0.9.0/src/pyaC/pyaErrors/pyaOtherErrors.py
+-rw-r--r--   0 steh312   (5677) st         (750)       72 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyaC/pyaErrors/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)      463 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyaC/pyaErrors/warn.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2995 2013-08-15 13:15:55.000000 PyAstronomy-0.9.0/src/pyaC/simiof.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyaC/pyaPermanent/
+-rw-r--r--   0 steh312   (5677) st         (750)     6840 2013-03-08 13:43:29.000000 PyAstronomy-0.9.0/src/pyaC/pyaPermanent/pyaFS.py
+-rw-r--r--   0 steh312   (5677) st         (750)     8966 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyaC/pyaPermanent/pyaConfig.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4586 2013-03-08 13:54:07.000000 PyAstronomy-0.9.0/src/pyaC/pyaPermanent/updateCycler.py
+-rw-r--r--   0 steh312   (5677) st         (750)       83 2013-03-08 13:54:07.000000 PyAstronomy-0.9.0/src/pyaC/pyaPermanent/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1272 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyaC/importCheck.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1449 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyaC/invertIndexSelection.py
+-rw-r--r--   0 steh312   (5677) st         (750)      230 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyaC/sanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2433 2013-03-08 13:43:29.000000 PyAstronomy-0.9.0/src/pyaC/fuzzyMatch.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/pyaC/mtools/
+-rw-r--r--   0 steh312   (5677) st         (750)     2385 2015-03-05 10:16:55.000000 PyAstronomy-0.9.0/src/pyaC/mtools/integrat.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2758 2013-04-17 10:42:26.000000 PyAstronomy-0.9.0/src/pyaC/mtools/numericalDerivatives.py
+-rw-r--r--   0 steh312   (5677) st         (750)       69 2015-03-05 10:05:14.000000 PyAstronomy-0.9.0/src/pyaC/mtools/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3345 2015-03-05 10:30:40.000000 PyAstronomy-0.9.0/src/pyaC/mtools/sanityOfmtools.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2659 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/pyaC/nestedLoop.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3614 2015-03-05 09:38:13.000000 PyAstronomy-0.9.0/src/pyaC/sanityNeedfThings.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/modelSuite/
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/
+-rw-r--r--   0 steh312   (5677) st         (750)     2173 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palMandelSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)    10946 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/rmcl_ohta.py
+-rw-r--r--   0 steh312   (5677) st         (750)     4843 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/limBrightTrans.py
+-rw-r--r--   0 steh312   (5677) st         (750)      146 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3913 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/circKepZList.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/
+-rw-r--r--   0 steh312   (5677) st         (750)     7291 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/mandelAgol.py
+-rw-r--r--   0 steh312   (5677) st         (750)     3300 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/exampleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)     5038 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/occultnl.f
+-rw-r--r--   0 steh312   (5677) st         (750)     1630 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/occultquad.pyf
+-rw-r--r--   0 steh312   (5677) st         (750)       51 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1117 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/occultnl.pyf
+-rw-r--r--   0 steh312   (5677) st         (750)    10336 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/occultquad.f
+-rw-r--r--   0 steh312   (5677) st         (750)     3535 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/mandelAgolNL.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/
+-rw-r--r--   0 steh312   (5677) st         (750)     4652 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/exampleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2591 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/seconPal.py
+-rw-r--r--   0 steh312   (5677) st         (750)       40 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/__init__.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/ellint/
+-rw-r--r--   0 steh312   (5677) st         (750)      810 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/ellint/ell.cpp
+-rw-r--r--   0 steh312   (5677) st         (750)      611 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/ellint/makefile_template
+-rw-r--r--   0 steh312   (5677) st         (750)    15838 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/pal.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1404 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/palSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)    11708 2014-02-26 16:27:34.000000 PyAstronomy-0.9.0/src/modelSuite/exampleSanity.py
+-rw-r--r--   0 steh312   (5677) st         (750)      548 2014-02-26 14:39:59.000000 PyAstronomy-0.9.0/src/modelSuite/__init__.py
+-rw-r--r--   0 steh312   (5677) st         (750)     1063 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/radVel.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2303 2013-03-29 14:35:38.000000 PyAstronomy-0.9.0/src/modelSuite/voigtAstro.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2818 2014-05-20 09:38:03.000000 PyAstronomy-0.9.0/src/modelSuite/keplerEllipseModel.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2391 2013-03-29 14:35:38.000000 PyAstronomy-0.9.0/src/modelSuite/LyAProfile.py
+-rw-r--r--   0 steh312   (5677) st         (750)     9736 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/modelSuite/lineListGaussModel.py
+-rw-r--r--   0 steh312   (5677) st         (750)     2826 2014-03-20 09:42:28.000000 PyAstronomy-0.9.0/src/modelSuite/rotBroadProfile.py
+-rw-r--r--   0 steh312   (5677) st         (750)      498 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/planetBrightnessPhases.py
+-rw-r--r--   0 steh312   (5677) st         (750)     5584 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/modelSuite/atanProfile.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/
+-rw-r--r--   0 steh312   (5677) st         (750)     1238 2014-09-30 15:17:11.000000 PyAstronomy-0.9.0/src/doc/index.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1265 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/license.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)      281 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/index.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPeriodDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)      424 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPeriodDoc/pyPeriod.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2269 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPeriodDoc/examples.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1613 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPeriodDoc/periodograms.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      722 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPeriodDoc/baseClasses.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPDMDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)     1761 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPDMDoc/examples.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      516 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPDMDoc/pdm.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      361 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPDMDoc/classes.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     7890 2015-02-18 09:39:02.000000 PyAstronomy-0.9.0/src/doc/conf.py
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)     2202 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/installingPyA.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      555 2015-03-05 09:42:19.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/index.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaPermanentDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)     1532 2013-03-08 13:54:07.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaPermanentDoc/index.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      224 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaPermanentDoc/pyaFS.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      812 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaPermanentDoc/pyaConfig.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      145 2013-03-08 13:54:07.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaPermanentDoc/updateCycler.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     3045 2015-03-05 09:25:59.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/needfulThings.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaErrorsDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)      712 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaErrorsDoc/index.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2349 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaErrorsDoc/pyaExTemplate.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      201 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaErrorsDoc/showWarning.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      452 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaErrorsDoc/pyaExceptions.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      778 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/whatIsIt.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/mtoolsDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)      244 2015-03-05 10:20:00.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/mtoolsDoc/mtools.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      543 2015-03-05 10:19:41.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/mtoolsDoc/integratDoc.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      715 2015-03-05 09:43:06.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/mtoolsDoc/numericalDerivativesDoc.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1115 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/versioning.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1505 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/IDLPorting.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      375 2014-09-30 15:17:11.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/acknowledgement.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      382 2014-02-10 16:58:55.000000 PyAstronomy-0.9.0/src/doc/pyaCDoc/cont.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/changeLog/
+-rw-r--r--   0 steh312   (5677) st         (750)      498 2015-03-05 10:33:35.000000 PyAstronomy-0.9.0/src/doc/changeLog/index.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      952 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/changeLog/from020to030.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1284 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/changeLog/from040to050.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      800 2015-08-24 10:16:38.000000 PyAstronomy-0.9.0/src/doc/changeLog/from081to090.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1343 2014-03-11 13:30:42.000000 PyAstronomy-0.9.0/src/doc/changeLog/from060to070.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1636 2013-04-02 12:57:30.000000 PyAstronomy-0.9.0/src/doc/changeLog/from050to060.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1029 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/changeLog/from030to040.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1434 2015-02-19 08:50:40.000000 PyAstronomy-0.9.0/src/doc/changeLog/from070to080.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     4826 2015-02-26 17:06:21.000000 PyAstronomy-0.9.0/src/doc/Makefile
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/phoenixUtils/
+-rw-r--r--   0 steh312   (5677) st         (750)      480 2015-02-25 09:56:54.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/phoenixUtils/phoenixUtils.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)     1033 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aberration.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1411 2013-08-15 08:58:52.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/crosscorr.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1340 2015-08-17 09:10:19.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/broad.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      453 2013-03-29 14:35:38.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/lineWidth.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1183 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/estimateSNR.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      855 2013-09-26 11:32:28.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/magnitudes.rst
+-rw-r--r--   0 steh312   (5677) st         (750)   196510 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/transVis-WASP-7b.png
+-rw-r--r--   0 steh312   (5677) st         (750)      441 2014-04-02 12:05:55.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/atomicNo.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1891 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/coorTimeDate.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      718 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/unredDoc.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/
+-rw-r--r--   0 steh312   (5677) st         (750)      770 2015-02-19 08:50:40.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/stellarAge.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      930 2014-10-06 12:40:45.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/pizzolato2003Doc.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      728 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/abundances.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     4127 2015-02-25 09:33:17.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/ramirez2005.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1665 2015-01-08 11:02:58.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/expCorrRN.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1040 2014-09-30 15:17:11.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/coordinates.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     3313 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/transitVisibility.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1862 2014-03-20 17:40:28.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/baryvel.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1904 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/nutate.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2619 2015-02-14 13:11:02.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/dopplerShift.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      508 2013-02-20 17:16:19.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/observatory.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      538 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/cardinalPoint.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      741 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/transitDuration.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      197 2014-03-19 16:11:37.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/broadening.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      905 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/airmass.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      365 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/twilight.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      631 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/fluxConversion.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      373 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/keplerOrbitAPI.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1001 2014-11-20 10:06:56.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/readFitsSpec.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     4893 2014-12-22 10:42:09.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/pyasl_wvlconv.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      618 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/pyaslAitoff.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1362 2013-03-08 13:43:29.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/moon.rst
+-rw-r--r--   0 steh312   (5677) st         (750)       91 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/statTest.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2772 2013-07-19 15:14:02.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/binning.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     4096 2014-11-07 09:32:05.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/outlier.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1217 2014-03-18 15:36:55.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/sindex.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2651 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/svd.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1599 2013-08-15 09:18:13.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/quadextreme.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1273 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/inTran.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      537 2014-01-22 10:35:15.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/posAngle.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      187 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/planetPhase.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2985 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/rotBroad.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      986 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/sunpos.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      832 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/folding.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      675 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/intep.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     6064 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/keplerOrbit.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2292 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/eq2hor.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1737 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/altitude.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      110 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/planck.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      118 2014-03-19 16:09:23.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/thermalBroad.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1026 2015-01-14 13:13:00.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/decimalYear.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      444 2013-04-02 12:55:35.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/angularDistance.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      720 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/smooth.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     3692 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/pyasl.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)     1026 2015-05-22 08:42:22.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/sweet_cat.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      739 2014-04-29 12:44:10.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/fip.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      618 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/exoplanetsOrg.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      626 2013-03-08 13:54:07.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/exoplanetEU.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1108 2014-03-26 12:32:30.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/kuruczModels.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      706 2013-03-08 13:54:07.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/nasaExoplanetArchive.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1167 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/baraffe98tracks.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/logo/
+-rw-r--r--   0 steh312   (5677) st         (750)     7040 2015-02-18 09:39:02.000000 PyAstronomy-0.9.0/src/doc/logo/pyalogo.png
+-rw-r--r--   0 steh312   (5677) st         (750)    13790 2015-02-18 09:39:02.000000 PyAstronomy-0.9.0/src/doc/logo/pyafavicon.ico
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/pyaGuiDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)      137 2015-02-14 13:11:02.000000 PyAstronomy-0.9.0/src/doc/pyaGuiDoc/index.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1851 2014-08-05 16:44:06.000000 PyAstronomy-0.9.0/src/doc/pyaGuiDoc/modelExplorer.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      714 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/pyaGuiDoc/pyapicker.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1912 2014-07-31 15:55:35.000000 PyAstronomy-0.9.0/src/doc/pyaGuiDoc/continuumFinder.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2459 2015-02-14 13:11:02.000000 PyAstronomy-0.9.0/src/doc/pyaGuiDoc/interactiveGV.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      451 2015-05-22 08:42:22.000000 PyAstronomy-0.9.0/src/doc/PyAGroup.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/constantsDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)     6277 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/constantsDoc/index.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)     1560 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/index.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1623 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/nelderMead.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     9713 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/tutorial2.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     3836 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/onedfit.rst
+-rw-r--r--   0 steh312   (5677) st         (750)    37914 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/tutorial.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      118 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/params.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      271 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/coordinateGrid.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      167 2013-09-25 16:08:06.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/fufDS.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      808 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/modelRebin.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1433 2015-03-12 10:25:58.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/extFitters.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     8273 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/traceAnalysisTutorial.rst
+-rw-r--r--   0 steh312   (5677) st         (750)    17936 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/tutorialMCMC.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2215 2014-03-10 12:52:42.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/simplemodels.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      446 2013-02-05 14:13:18.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/syncFit.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      446 2015-08-24 10:14:44.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/traceAnalysis.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      532 2015-03-12 10:25:58.000000 PyAstronomy-0.9.0/src/doc/funcFitDoc/fitters.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)      684 2014-02-26 14:43:12.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/index.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      965 2014-02-26 15:21:12.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/rotBroadProfile.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)      737 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/palRebin.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      529 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/pal.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     5005 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/exams.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1586 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/boostsupport.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      510 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/palTrans.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/radVelDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)     1792 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/radVelDoc/radVel.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     4653 2015-08-13 09:04:18.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/forTrans.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2612 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/keplerEllipseModelDoc.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      683 2013-03-29 14:35:38.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/astroVoigt.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1965 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/lineListGaussModelDoc.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      574 2013-03-29 14:35:38.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/LyAProfile.rst
+drwxr-xr-x   0 steh312   (5677) st         (750)        0 2015-11-04 11:28:32.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/RmcLOhtaDoc/
+-rw-r--r--   0 steh312   (5677) st         (750)      728 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/RmcLOhtaDoc/index.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      229 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/RmcLOhtaDoc/rmcl.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     2376 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/RmcLOhtaDoc/rmclExamples.rst
+-rw-r--r--   0 steh312   (5677) st         (750)      573 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/xtranDoc.rst
+-rw-r--r--   0 steh312   (5677) st         (750)     1367 2013-02-06 13:17:26.000000 PyAstronomy-0.9.0/src/doc/modelSuiteDoc/limBrightTrans.rst
```

### Comparing `PyAstronomy-0.8.1/setup.py` & `PyAstronomy-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
             'PyAstronomy.modelSuite.XTran.forTrans', \
             'PyAstronomy.pyTiming', \
             'PyAstronomy.pyTiming.pyPDM', \
             'PyAstronomy.pyTiming.pyPeriod', \
             'PyAstronomy.pyaC', \
             'PyAstronomy.pyaC.pyaErrors', \
             'PyAstronomy.pyaC.pyaPermanent', \
+            'PyAstronomy.pyaC.mtools', \
             'PyAstronomy.constants', \
             'PyAstronomy.pyaGui']
 
 # "doc/*/*.rst", "doc/*/*.png"],
 package_data = {"PyAstronomy":["setup.cfg"],
                 "PyAstronomy.modelSuite.XTran.palTrans":["ellint/makefile_template", "ellint/ell.cpp"], \
                 "PyAstronomy.modelSuite.XTran.forTrans":["*.f", "*.pyf"], \
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/phoenixUtils/read.py` & `PyAstronomy-0.9.0/src/pyasl/phoenixUtils/read.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/resBased/fip.py` & `PyAstronomy-0.9.0/src/pyasl/resBased/fip.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/resBased/exoplanetsOrg.py` & `PyAstronomy-0.9.0/src/pyasl/resBased/exoplanetsOrg.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/resBased/exampleSanity.py` & `PyAstronomy-0.9.0/src/pyasl/resBased/exampleSanity.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,8 +161,10 @@
     from PyAstronomy import pyasl
   
     fip = pyasl.FirstIonizationPot()
     self.assertAlmostEqual(10.451260, fip.getFIP(53)[0], 6, msg="FIP for iodine does not match (an).")
     self.assertAlmostEqual(10.451260, fip.getFIP("I")[0], 6, msg="FIP for iodine does not match (sym).")
     
     self.assertAlmostEqual(25e-6, fip.getFIP(53)[1], 6, msg="FIP for iodine does not match (an).")
-    self.assertAlmostEqual(25e-6, fip.getFIP("I")[1], 6, msg="FIP for iodine does not match (sym).")
+    self.assertAlmostEqual(25e-6, fip.getFIP("I")[1], 6, msg="FIP for iodine does not match (sym).")
+    
+
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/resBased/baraffe98tracks.py` & `PyAstronomy-0.9.0/src/pyasl/resBased/baraffe98tracks.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/resBased/fip.dat` & `PyAstronomy-0.9.0/src/pyasl/resBased/fip.dat`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/resBased/nasaExoplanetArchive.py` & `PyAstronomy-0.9.0/src/pyasl/resBased/nasaExoplanetArchive.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/resBased/exoplanetEU.py` & `PyAstronomy-0.9.0/src/pyasl/resBased/exoplanetEU.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,48 +13,48 @@
     This class downloads the data base as a csv
     file and converts it into a numpy recarray.
     By default, the data are re-downloaded
     every 7 days.
     
     The available columns are:
     
-    ============  ==============================  =====
-     Column Name                     Description   Unit
+    ============  ==============================  ======
+     Column Name                     Description    Unit
 
           plName                  Name of planet       
-          plMass                  Mass of planet     MJ
-        plRadius                Radius of planet     RJ
-          period                  Orbital period      d
-             sma                 Semi-major axis     AU
+          plMass                  Mass of planet      MJ
+        plRadius                Radius of planet      RJ
+          period                  Orbital period       d
+             sma                 Semi-major axis      AU
     eccentricity            Orbital eccentricity       
-     inclination             Orbital inclination    deg
-     angDistance                Angular Distance arcsec
+     inclination             Orbital inclination     deg
+     angDistance                Angular Distance  arcsec
        pubStatus              Publication status       
-      discovered               Year of discovery     yr
+      discovered               Year of discovery      yr
          updated             Date of data update       
-           omega          Argument of Periastron    deg
-           tperi             Epoch of Periastron      d
+           omega          Argument of Periastron     deg
+           tperi             Epoch of Periastron       d
          detType                  Detection type       
        molecules      List of detected molecules       
           stName                    Name of star       
-              ra         Right ascension (J2000)    hms
-             dec             Declination (J2000)    dms
-           mag_v      V magnitude of a host star    mag
-           mag_i      I magnitude of a host star    mag
-           mag_j      J magnitude of a host star    mag
-           mag_h      H magnitude of a host star    mag
-           mag_k      K magnitude of a host star    mag
-            dist           Distance to host star     pc
-              mh        Metallicity of host star    dex
-          stMass                    Stellar mass  solar
-        stRadius                  Radius of star  solar
+              ra         Right ascension (J2000)     hms
+             dec             Declination (J2000)     dms
+           mag_v      V magnitude of a host star     mag
+           mag_i      I magnitude of a host star     mag
+           mag_j      J magnitude of a host star     mag
+           mag_h      H magnitude of a host star     mag
+           mag_k      K magnitude of a host star     mag
+            dist           Distance to host star      pc
+              mh        Metallicity of host star     dex
+          stMass                    Stellar mass   solar
+        stRadius                  Radius of star   solar
              SpT      Spectral type of host star       
-           stAge                     Stellar age     Ga
-          stTeff   Stellar effective temperature      K
-    ============  ==============================  =====
+           stAge                     Stellar age      Ga
+          stTeff   Stellar effective temperature       K
+    ============  ==============================  ======
     
     Parameters
     ----------
     skipUpdate : boolean, optional
         If True, no re-download of the data
         will be initiated no matter how old
         they are.
@@ -78,14 +78,15 @@
       pass
     # Reinitialize csv file
     r = csv.DictReader(self._fs.requestFile(self.dataFileName, 'r', gzip.open), delimiter=',')
     # Determine data types for numpy recarray from columns
     # and initialize array
     dtype = map(lambda x: (self._columns[x][0], self._columns[x][3]), range(len(self._columns)))
     self.data = np.recarray((nplanets+1,), dtype=dtype)
+    colnotfilled = map(lambda x:self._columns[x][0], self._columns.keys())
     for i, x in enumerate(r):
       for k, v in x.iteritems():
         # Remove hash and white spaces from column names
         k = k.strip('#')
         k = k.strip()
         # Translate csv column name into internal column name
         if k in self._ident:
@@ -93,15 +94,24 @@
         else:
           key = k
         if len(v) == 0:
           v = None
         # Accept only expected fields 
         if not key in self.data.dtype.names:
           continue
+        try:
+          colnotfilled.remove(key)
+        except ValueError:
+          # Ignoring already removed value
+          pass
         self.data[key][i] = v
+    if len(colnotfilled) > 0:
+      PE.warn(PE.PyAAlgorithmFailure("Not all columns could be filled with data. The following columns must not be used: " + ", ".join(colnotfilled), \
+                                     where="ExoplanetEU", \
+                                     solution="The format of the data base must be checked. Please consider issuing a bug report via github."))
 
   def availableColumns(self):
     """
       Show a summary of the available columns.
       
       Returns
       -------
@@ -185,10 +195,10 @@
     # Identify exoplanet.eu csv column names with internal column names
     self._ident = {"name":"plName", "mass":"plMass", "radius":"plRadius", \
                    "semi_major_axis":"sma", "angular_distance":"angDistance", "publication_status":"pubStatus", \
                    "detection_type":"detType", "star_name":"stName", "mag_v":"mag_v", \
                    "mag_i":"mag_i", "mag_j":"mag_j", "mag_h":"mag_h", \
                    "mag_k":"mag_k", "star_distance":"dist", "star_metallicity":"mh", \
                    "star_mass":"stMass", "star_radius":"stRadius", "star_sp_type":"SpT", \
-                   "star_age":"stAge", "star_teff":"stTeff"}
+                   "star_age":"stAge", "star_teff":"stTeff", "orbital_period":"period"}
     
     self._readData()
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/resBased/kuruczModels.py` & `PyAstronomy-0.9.0/src/pyasl/resBased/kuruczModels.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/idlCirrange.py` & `PyAstronomy-0.9.0/src/pyasl/asl/idlCirrange.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/planetPhase.py` & `PyAstronomy-0.9.0/src/pyasl/asl/planetPhase.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/sunpos.py` & `PyAstronomy-0.9.0/src/pyasl/asl/sunpos.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/planck.py` & `PyAstronomy-0.9.0/src/pyasl/asl/planck.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/estimateSNR.py` & `PyAstronomy-0.9.0/src/pyasl/asl/estimateSNR.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/readFitsSpec.py` & `PyAstronomy-0.9.0/src/pyasl/asl/readFitsSpec.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/observatory.cfg` & `PyAstronomy-0.9.0/src/pyasl/asl/observatory.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -316,7 +316,14 @@
 [PTST]
 name = Planetary Transit Search Telescope (Hamburger Sternwarte), Mallorca
 longitude = 2.95
 latitude = 39.64
 altitude = 162.0
 tz = -1.0
 
+[SUBARU]
+# http://www.naoj.org/Observing/Telescope/Parameters/
+name = SUBARU (NAOJ, Mauna-Kea-Observatorium)
+longitude = 204.523888
+latitude = 19.82555
+altitude = 4163.
+tz = -10.0
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/writeFitsSpec.py` & `PyAstronomy-0.9.0/src/pyasl/asl/writeFitsSpec.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/localtime.py` & `PyAstronomy-0.9.0/src/pyasl/asl/localtime.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/sanityTest.py` & `PyAstronomy-0.9.0/src/pyasl/asl/sanityTest.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,82 @@
     time = numpy.linspace(0, 6.78, 200)
     ke = KeplerEllipse(4.5, 3.14159, 0.314)
     pos = ke.xyzPos(time)
     for i in xrange(len(time)):
       pos1 = ke.xyzPos(time[i])
       self.assertEqual( numpy.sum(numpy.abs((pos[i,::]-pos1))), 0.0)
   
+  def sanity_keplerAngMom(self):
+    """
+      Checking Kepler orbit: Angular momentum
+    """
+    import numpy as np
+    ke = KeplerEllipse(1 , 2.0*np.pi, e=0.0, i=90.0, Omega=0., w=0.0, tau=0.0)
+    am1 = ke.orbAngMomentum()
+    am2 = ke.orbAngMomentum(t=101.7)
+    d = np.max(np.abs(am1 - am2))
+    self.assertAlmostEqual(d, 0.0, delta=1e-12, msg="Angular momentum is not constant in time")
+    
+    d = np.max(np.abs(am1 - np.array([0,-1,0])))
+    self.assertAlmostEqual(d, 0.0, delta=1e-12, msg="Angular momentum wrong for i=90 deg")
+    
+    ke = KeplerEllipse(1 , 2.0*np.pi, e=0.0, i=0.0, Omega=0., w=0.0, tau=0.0)
+    am1 = ke.orbAngMomentum()
+    d = np.max(np.abs(am1 - np.array([0,0,1])))
+    self.assertAlmostEqual(d, 0.0, delta=1e-12, msg="Angular momentum wrong for i=0 deg")
+    
+    for w in [10.0, 87.0, 277.8]:
+      ke = KeplerEllipse(1 , 2.0*np.pi, e=0.0, i=0.0, Omega=0., w=w, tau=0.0)
+      ame = ke.orbAngMomentum()
+      d = np.max(np.abs(ame - am1))
+      self.assertAlmostEqual(d, 0.0, delta=1e-12, msg="Angular momentum changes with argument of periapsis")
+  
+  def sanity_keplerOrbitNodes(self):
+    """
+      Checking node position of Kepler ellipse.
+    """
+    import numpy as np
+    ke = KeplerEllipse(1 ,1, e=0.0, i=90.0, Omega=0., w=0.0, tau=0.0)
+  
+    n1 = ke.xyzNodes_LOSZ(los='+z')
+    self.assertAlmostEqual(max(np.abs(n1[0] - np.array([1.0,0.0,0.0]))), 0.0, delta=1e-15, \
+                           msg="Location of ascending node does not match.")
+    self.assertAlmostEqual(max(np.abs(n1[1] - np.array([-1.0,0.0,0.0]))), 0.0, delta=1e-15, \
+                           msg="Location of descending node does not match.")
+    
+    n2 = ke.xyzNodes_LOSZ(los='-z')
+    for i in range(2):
+      md = np.max(np.abs(n1[i] - n2[(i+1)%2]))
+      self.assertAlmostEqual(md, 0.0, delta=1e-15, msg="Nodes are not exchanged when LOS is reversed.")
+    
+    # None of this should have an impact on the node
+    for w in xrange(0, 360, 80):
+      for tau in xrange(0, 100, 25):
+        for i in xrange(5, 85, 20):
+          ke2 = KeplerEllipse(1 , 1, e=0.0, i=i, Omega=0., w=w, tau=tau)
+          n3 = ke2.xyzNodes_LOSZ(los='+z')
+          for j in xrange(2):
+            md = np.max(np.abs(n1[j]-n3[j]))
+            self.assertAlmostEqual(md, 0.0, delta=1e-12, \
+                                   msg="Unexpected impact on position of node.")
+    
+    # Check node rotation
+    ke3 = KeplerEllipse(1 , 1, e=0.0, i=90., Omega=90., w=0.0, tau=0.0)
+    n4 = ke3.xyzNodes_LOSZ(los='+z')
+    self.assertAlmostEqual(np.max(np.abs(n4[0] - np.array([0.,1.,0.]))), 0.0, delta=1e-12, \
+                           msg="Wrong ascending node for Omega = 90")
+    ke3 = KeplerEllipse(1 , 1, e=0.0, i=90., Omega=180., w=0.0, tau=0.0)
+    n4 = ke3.xyzNodes_LOSZ(los='+z')
+    self.assertAlmostEqual(np.max(np.abs(n4[0] - np.array([-1.,0.,0.]))), 0.0, delta=1e-12, \
+                           msg="Wrong ascending node for Omega = 180")
+    ke3 = KeplerEllipse(1 , 1, e=0.0, i=90., Omega=270., w=0.0, tau=0.0)
+    n4 = ke3.xyzNodes_LOSZ(los='+z')
+    self.assertAlmostEqual(np.max(np.abs(n4[0] - np.array([0.,-1.,0.]))), 0.0, delta=1e-12, \
+                           msg="Wrong ascending node for Omega = 270") 
+  
   def sanity_MarkleyKESolver_precision(self):
     """
       Checking precision of Markley solver for Kepler's equation.
     """
     ks = MarkleyKESolver()
     p = ks.precisionTest()
     self.assertLess(p, 1e-14)
@@ -264,45 +332,64 @@
     e = 0.3
     print "Eccentric anomaly: ", ks.getE(M, e)
   
   def sanity_example2(self):
     """
       Checking Kepler orbit calculation example.
     """
-    import numpy
+    import numpy as np
     from PyAstronomy import pyasl
     import matplotlib.pylab as plt
     
     # Instantiate a Keplerian elliptical orbit with
     # semi-major axis of 1.3 length units,
-    # period of 2 time units, eccentricity of 0.5, and
-    # longitude of ascending node of 70 degrees.
-    ke = pyasl.KeplerEllipse(1.3, 2., e=0.5, Omega=70.)
+    # a period of 2 time units, eccentricity of 0.5,
+    # longitude of ascending node of 70 degrees, an inclination
+    # of 10 deg, and a periapsis argument of 110 deg.
+    ke = pyasl.KeplerEllipse(1.3, 2., e=0.5, Omega=70., i=10.0, w=110.0)
     
     # Get a time axis
-    t = numpy.linspace(0, 6.5, 200)
+    t = np.linspace(0, 1.9, 200)
     
     # Calculate the orbit position at the given points
     # in a Cartesian coordinate system.
     pos = ke.xyzPos(t)
     print "Shape of output array: ", pos.shape
     
     # x, y, and z coordinates for 50th time point
     print "x, y, z for 50th point: ", pos[50, ::]
     
     # Calculate orbit radius as a function of the
     radius = ke.radius(t)
     
+    # Calculate velocity on orbit
+    vel = ke.xyzVel(t)
+    
+    # Find the nodes of the orbit (Observer at -z)
+    ascn, descn = ke.xyzNodes_LOSZ()
+    
     # Plot x and y coordinates of the orbit
     plt.subplot(2,1,1)
-    plt.plot(pos[::,0], pos[::,1], 'bp')
-    # Plot orbit radius as a function of time
+    plt.title("Periapsis (red diamond), Asc. node (green circle), desc. node (red circle)")
+    plt.xlabel("East ->")
+    plt.ylabel("North ->")
+    plt.plot([0], [0], 'k+', markersize=9)
+    plt.plot(pos[::,1], pos[::,0], 'bp')
+    # Point of periapsis
+    plt.plot([pos[0,1]], [pos[0,0]], 'rd')
+    # Nodes of the orbit
+    plt.plot([ascn[1]], [ascn[0]], 'go', markersize=10)
+    plt.plot([descn[1]], [descn[0]], 'ro', markersize=10)
+    # Plot RV
     plt.subplot(2,1,2)
-    plt.plot(t, radius, 'bp')
-    # plt.show()
+    plt.xlabel("Time")
+    plt.ylabel("Radial velocity [length/time]")
+    plt.plot(t, vel[::,2], 'r.-')
+#    plt.show()
+
 
 
 class SanityOfBinnin(unittest.TestCase, SaniBase):
   
   def setUp(self):
     pass
   
@@ -1673,22 +1760,30 @@
     y[187] = 0.3
     y[505] = 0.1
     y[610] = 0.1
     y[615] = 0.7
     
     # Apply Gaussian instrumental broadening, setting the resolution to 10000.
     r, fwhm = pyasl.instrBroadGaussFast(x, y, 10000,
-                                        edgeHandling="firstlast", fullout=True)
+              edgeHandling="firstlast", fullout=True)
     
+    # Apply Gaussian instrumental broadening, setting the resolution to 10000.
+    # Limit the extent of the Gaussian broadening kernel to five standard
+    # deviations.
+    r2, fwhm = pyasl.instrBroadGaussFast(x, y, 10000,
+              edgeHandling="firstlast", fullout=True, maxsig=5.0)
+              
     print "FWHM used for the Gaussian kernel: ", fwhm, " A"
     
     # Plot the output
-    plt.plot(x,r, 'r--p')
-    plt.plot(x,y, 'b-')
-#    plt.show()
+    plt.plot(x,r, 'r--p', label="Broadened curve (full)")
+    plt.plot(x, r2, 'k:', label="Broadened curve (5 stds)")
+    plt.plot(x,y, 'b-', label="Input")
+    plt.legend(loc=4)
+#     plt.show()
 
   def sanity_tests(self):
     """
       Checking sanity of 'instrBroadGaussFast'
     """
     from PyAstronomy import pyasl
     import numpy as np
@@ -1732,14 +1827,48 @@
     
     print np.mean(x*y)/np.sum(y), np.mean(x*y2)/np.sum(y2)
     print np.sqrt(np.sum( x**2*y)/np.sum(y))
     print np.sqrt(np.sum( x**2*y2)/np.sum(y2))
     print np.sum(y), np.sum(y2)
     
     mean2 = np.mean(x*y2)/np.sum(y2)
+    self.assertAlmostEqual(mean2, 0.0, delta=1e-9, \
+                           msg="Barycenter of convoluted Gaussian (" + str(mean2) + ") deviates from 0.0.")
+    std2 = np.sqrt(np.sum( x**2*y2)/np.sum(y2))
+    std2_nom = np.sqrt(gf["sig"]**2 + (1.5-gf["sig"])**2)
+    self.assertAlmostEqual(std2, std2_nom, delta=1e-5, \
+                           msg="Std of convoluted Gaussian (" + str(std2) +") deviates from nominal value.")
+    self.assertAlmostEqual(np.sum(y), np.sum(y2), delta=1e-4,
+                           msg="Normalization of convoluted Gaussian (" + str(np.sum(y2)) +") is incorrect.")
+
+  def sanity_convolutionGaussianMaxsig(self):
+    """
+      Check the sanity of broadGaussFast including maxsig
+    """
+    import numpy as np
+    from PyAstronomy import pyasl
+    from PyAstronomy import funcFit as fuf
+    
+    x = np.arange(-10.0, 10.0, 0.001)
+    gf = fuf.GaussFit1d()
+    gf["A"] = 0.8
+    gf["sig"] = 0.471
+    y = gf.evaluate(x)
+    
+    y3 = pyasl.broadGaussFast(x, y, 1.5-gf["sig"], edgeHandling="firstlast", maxsig=5.0)
+    y2 = pyasl.broadGaussFast(x, y, 1.5-gf["sig"], edgeHandling="firstlast", maxsig=None)
+    
+    self.assertAlmostEqual(np.max(np.abs(y2-y3)), 0.0, delta=2e-7, msg="Deviation in profiles using maxsig (broadGaussFast)")
+    
+    print np.mean(x*y)/np.sum(y), np.mean(x*y2)/np.sum(y2)
+    print np.sqrt(np.sum( x**2*y)/np.sum(y))
+    print np.sqrt(np.sum( x**2*y2)/np.sum(y2))
+    print np.sum(y), np.sum(y2)
+    
+    mean2 = np.mean(x*y2)/np.sum(y2)
     self.assertAlmostEqual(mean2, 0.0, delta=1e-9, \
                            msg="Barycenter of convoluted Gaussian (" + str(mean2) + ") deviates from 0.0.")
     std2 = np.sqrt(np.sum( x**2*y2)/np.sum(y2))
     std2_nom = np.sqrt(gf["sig"]**2 + (1.5-gf["sig"])**2)
     self.assertAlmostEqual(std2, std2_nom, delta=1e-5, \
                            msg="Std of convoluted Gaussian (" + str(std2) +") deviates from nominal value.")
     self.assertAlmostEqual(np.sum(y), np.sum(y2), delta=1e-4,
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/test.py` & `PyAstronomy-0.9.0/src/pyasl/asl/test.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/cardinalPoint.py` & `PyAstronomy-0.9.0/src/pyasl/asl/cardinalPoint.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/planet_Teq.py` & `PyAstronomy-0.9.0/src/pyasl/asl/planet_Teq.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/binning.py` & `PyAstronomy-0.9.0/src/pyasl/asl/binning.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/broad.py` & `PyAstronomy-0.9.0/src/pyasl/asl/broad.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from PyAstronomy.pyaC import pyaErrors as PE
 from PyAstronomy import funcFit as fuf
 
 
-def broadGaussFast(x, y, sigma, edgeHandling=None):
+def broadGaussFast(x, y, sigma, edgeHandling=None, maxsig=None):
   """
     Apply Gaussian broadening. 
     
     This function broadens the given data using a Gaussian
     kernel.
     
     Parameters
@@ -19,30 +19,40 @@
         profile used in the convolution.
     edgeHandling : string, {None, "firstlast"}, optional
         Determines the way edges will be handled. If None,
         nothing will be done about it. If set to "firstlast",
         the spectrum will be extended by using the first and
         last value at the start or end. Note that this is
         not necessarily appropriate. The default is None.
+    maxsig : float, optional
+        The extent of the broadening kernel in terms of
+        standrad deviations. By default, the Gaussian broadening
+        kernel will be extended over the entire given spectrum,
+        which can cause slow evaluation in the case of large spectra.
+        A reasonable choice could, e.g., be five.  
     
     Returns
     -------
     Broadened data : array
         The input data convolved with the Gaussian
         kernel.
   """
   # Check whether x-axis is linear
   dxs = x[1:] - x[0:-1]
   if abs(max(dxs) - min(dxs)) > np.mean(dxs)*1e-6:
     raise(PE.PyAValError("The x-axis is not equidistant, which is required.", \
                          where="broadGaussFast"))
   
+  if maxsig is None:
+    lx = len(x)
+  else:
+    lx = int(((sigma*maxsig) / dxs[0]) * 2.0) + 1
   # To preserve the position of spectral lines, the broadening function
   # must be centered at N//2 - (1-N%2) = N//2 + N%2 - 1
-  nx = (np.arange(len(x), dtype=np.int) - sum(divmod(len(x),2)) + 1) * dxs[0]
+  nx = (np.arange(lx, dtype=np.int) - sum(divmod(lx,2)) + 1) * dxs[0]
   gf = fuf.GaussFit1d()
   gf["A"] = 1.0
   gf["sig"] = sigma
   e = gf.evaluate(nx)
   # This step ensured that the 
   e /= np.sum(e)
   
@@ -55,15 +65,15 @@
   else:
     raise(PE.PyAValError("Invalid value for `edgeHandling`: " + str(edgeHandling), \
                          where="broadGaussFast", \
                          solution="Choose either 'firstlast' or None"))
   return result
   
 
-def instrBroadGaussFast(wvl, flux, resolution, edgeHandling=None, fullout=False):
+def instrBroadGaussFast(wvl, flux, resolution, edgeHandling=None, fullout=False, maxsig=None):
   """
     Apply Gaussian instrumental broadening. 
     
     This function broadens a spectrum assuming a Gaussian
     kernel. The width of the kernel is determined by the
     resolution. In particular, the function will determine
     the mean wavelength and set the Full Width at Half
@@ -82,14 +92,20 @@
         Determines the way edges will be handled. If None,
         nothing will be done about it. If set to "firstlast",
         the spectrum will be extended by using the first and
         last value at the start or end. Note that this is
         not necessarily appropriate. The default is None.
     fullout : boolean, optional
         If True, also the FWHM of the Gaussian will be returned.
+    maxsig : float, optional
+        The extent of the broadening kernel in terms of
+        standrad deviations. By default, the Gaussian broadening
+        kernel will be extended over the entire given spectrum,
+        which can cause slow evaluation in the case of large spectra.
+        A reasonable choice could, e.g., be five.  
     
     Returns
     -------
     Broadened spectrum : array
         The input spectrum convolved with a Gaussian
         kernel.
     FWHM : float, optional
@@ -101,15 +117,15 @@
   if abs(max(dwls) - min(dwls)) > np.mean(dwls)*1e-6:
     raise(PE.PyAValError("The wavelength axis is not equidistant, which is required.", \
                          where="instrBroadGaussFast"))
   meanWvl = np.mean(wvl)
   fwhm = 1.0/float(resolution) * meanWvl
   sigma = fwhm/(2.0*np.sqrt(2.*np.log(2.)))
   
-  result = broadGaussFast(wvl, flux, sigma, edgeHandling=edgeHandling)
+  result = broadGaussFast(wvl, flux, sigma, edgeHandling=edgeHandling, maxsig=maxsig)
   
   if not fullout:
     return result
   else:
     return (result, fwhm)
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/baryvel.py` & `PyAstronomy-0.9.0/src/pyasl/asl/baryvel.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/__init__.py` & `PyAstronomy-0.9.0/src/pyasl/asl/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/moonpos.py` & `PyAstronomy-0.9.0/src/pyasl/asl/moonpos.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/atomicNo.py` & `PyAstronomy-0.9.0/src/pyasl/asl/atomicNo.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/dopplerShift.py` & `PyAstronomy-0.9.0/src/pyasl/asl/dopplerShift.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/crosscorr.py` & `PyAstronomy-0.9.0/src/pyasl/asl/crosscorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,31 +104,32 @@
                          where="crosscorrRV", \
                          solution="Change the order of the parameters."))
   # Check whether template is large enough
   if mode == "lin":
     meanWl = np.mean(w)
     dwlmax = meanWl * (rvmax/c)
     dwlmin = meanWl * (rvmin/c)
-    if (w.min() + dwlmin) < tw[0]:
-      raise(PE.PyAValError("The minimum wavelength is not covered by the template.", \
+    if (tw[0] + dwlmax) > w[0]:
+      raise(PE.PyAValError("The minimum wavelength is not covered by the template for all indicated RV shifts.", \
                            where="crosscorrRV", \
                            solution=["Provide a larger template", "Try to use skipedge"]))
-    if (w.max() + dwlmax) > tw[-1]:
-      raise(PE.PyAValError("The maximum wavelength is not covered by the template.", \
+    if (tw[-1] + dwlmin) < w[-1]:
+      raise(PE.PyAValError("he maximum wavelength is not covered by the template for all indicated RV shifts.", \
                            where="crosscorrRV", \
                            solution=["Provide a larger template", "Try to use skipedge"]))
   elif mode == "doppler":
-    maxwl = w[-1] * (1.0+rvmax/c)
-    minwl = w[0] * (1.0+rvmin/c)
-    if minwl < tw[0]:
-      raise(PE.PyAValError("The minimum wavelength is not covered by the template.", \
+    # Ensure that the template covers the entire observaion for all shifts
+    maxwl = tw[-1] * (1.0+rvmin/c)
+    minwl = tw[0] * (1.0+rvmax/c)
+    if minwl > w[0]:
+      raise(PE.PyAValError("he minimum wavelength is not covered by the template for all indicated RV shifts.", \
                            where="crosscorrRV", \
                            solution=["Provide a larger template", "Try to use skipedge"]))
-    if maxwl > tw[-1]:
-      raise(PE.PyAValError("The maximum wavelength is not covered by the template.", \
+    if maxwl < w[-1]:
+      raise(PE.PyAValError("The maximum wavelength is not covered by the template for all indicated RV shifts.", \
                            where="crosscorrRV", \
                            solution=["Provide a larger template", "Try to use skipedge"]))
   else:
     raise(PE.PyAValError("Unknown mode: " + str(mode), \
                          where="crosscorrRV", \
                          solution="See documentation for available modes."))
   # Calculate the cross correlation
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/lineOfSight.py` & `PyAstronomy-0.9.0/src/pyasl/asl/lineOfSight.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/twilight.py` & `PyAstronomy-0.9.0/src/pyasl/asl/twilight.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/moonphase.py` & `PyAstronomy-0.9.0/src/pyasl/asl/moonphase.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/eq2hor.py` & `PyAstronomy-0.9.0/src/pyasl/asl/eq2hor.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/rotBroad.py` & `PyAstronomy-0.9.0/src/pyasl/asl/rotBroad.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/posAngle.py` & `PyAstronomy-0.9.0/src/pyasl/asl/posAngle.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/atomicNo.dat` & `PyAstronomy-0.9.0/src/pyasl/asl/atomicNo.dat`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/airmass.py` & `PyAstronomy-0.9.0/src/pyasl/asl/airmass.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/lineWidth.py` & `PyAstronomy-0.9.0/src/pyasl/asl/lineWidth.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/outlier.py` & `PyAstronomy-0.9.0/src/pyasl/asl/outlier.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/astroTimeLegacy.py` & `PyAstronomy-0.9.0/src/pyasl/asl/astroTimeLegacy.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/unred.py` & `PyAstronomy-0.9.0/src/pyasl/asl/unred.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/smooth.py` & `PyAstronomy-0.9.0/src/pyasl/asl/smooth.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/statTest.py` & `PyAstronomy-0.9.0/src/pyasl/asl/statTest.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/airtovac.py` & `PyAstronomy-0.9.0/src/pyasl/asl/airtovac.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,14 +232,58 @@
   sflux = shiftSpec(wvl)
   # Determine 'valid' indices
   vind = np.where(np.bitwise_not(np.isnan(sflux)))[0]
   
   return sflux, vind
   
   
+
+
+def _iocon(inp):
+  """
+    Convert input into np float array and create function to convert back.
+    
+    Parameters
+    ----------
+    inp : some numeric type
+        Input
+    
+    Returns
+    -------
+    output : float array
+        The input converted into a numpy float array
+    recovery function : callable
+        Function that converts the output back into a float
+        number unless the input was an numpy array. In the latter
+        case, it remains an array.
+  """
+  
+  try:
+    # Using ravel to avoid generating object with zero length
+    out = np.ravel(np.array(inp, dtype=np.float))
+  except Exception, e:
+    raise(PE.PyAValError("Could not convert input of type: " + str(type(inp)) + " into float array. Error: " + str(e), \
+          where="_IOCON", \
+          solution="Use an input which can be converted into a numpy float array."))
+  
+  if isinstance(inp, np.ndarray) or len(out) > 1:
+    return out, lambda x:x
+  else:
+    def recover(x):
+      try:
+        result = float(x)
+      except Exception, e:
+        raise(PE.PyAValError("Could not convert result into a float. Error: " + str(e), \
+                             where="_iocon", \
+                             solution="Use a float or numpy array as input. Are you maybe using a list?"))
+      return result
+    return out, recover
+    
+
+
   
 class RefractiveIndexAV:
   """
     Refractive index for conversion between air- and vacuum wavelengths.
     
     The conversion is based on the formulae provided either by:
       - Edlen 1953, J. Opt. Soc. Am 43 no. 5
@@ -368,15 +412,17 @@
           specified 'mode').
       
       Returns
       -------
       wvl : float or array
           Wavelength in air.
     """
-    return wvl/self.refractiveIndex(wvl, **kwargs)
+    wvl, rec = _iocon(wvl)
+    result = wvl/self.refractiveIndex(wvl, **kwargs)
+    return rec(result)
   
   def airtovac(self, wvl, precision=1e-12, maxiter=30, **kwargs):
     """
       Convert air wavelength into wavelength in vacuum.
       
       An iterative scheme is applied to invert the formula.
       
@@ -397,34 +443,35 @@
       
       Returns
       -------
       wvl : float or array
           Wavelength in air.
     """
     # First guess for vacuum wavelength is wavelength in air
+    wvl, rec = _iocon(wvl)
     lvac = wvl.copy()
     counter = 0
     while True:
       counter += 1
       dl = lvac/self.refractiveIndex(lvac) - wvl
       lvac -= dl
       # Obtain difference between air wavelength resulting from
       # current estimate of vacuum wavelength 
       dlair = self.vactoair(lvac) - wvl
       if np.abs(np.max(dlair)) < precision:
-        return lvac 
+        return rec(lvac) 
       if counter > maxiter:
         p = np.max(dlair)
         raise(PE.PyAValError("Maximum of iterations reached. Current precision is " + str(p) + " A.", \
                              where="RefractiveIndexAV::airtovac", \
                              solution=["Try to increase 'maxiter'", \
                                        "Try to use subrange of wavelengths", \
                                        "Try to adapt 'precision' to necessary value"]))
       
-    return lvac
+    return rec(lvac)
   
   def __init__(self, mode="ciddor"):
     
     if mode == "edlen53":
       self.refractiveIndex = self._edlen53
     elif mode == "peckReeder":
       self.refractiveIndex = self._peckReeder
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/inTransit.py` & `PyAstronomy-0.9.0/src/pyasl/asl/inTransit.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/testPro/airtovac.pro` & `PyAstronomy-0.9.0/src/pyasl/asl/testPro/airtovac.pro`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/testPro/vactoair.pro` & `PyAstronomy-0.9.0/src/pyasl/asl/testPro/vactoair.pro`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/testPro/test.pro` & `PyAstronomy-0.9.0/src/pyasl/asl/testPro/test.pro`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/intep.py` & `PyAstronomy-0.9.0/src/pyasl/asl/intep.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/magnitudes.py` & `PyAstronomy-0.9.0/src/pyasl/asl/magnitudes.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/folding.py` & `PyAstronomy-0.9.0/src/pyasl/asl/folding.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/fluxConversion.py` & `PyAstronomy-0.9.0/src/pyasl/asl/fluxConversion.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/observatory.py` & `PyAstronomy-0.9.0/src/pyasl/asl/observatory.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/quadextreme.py` & `PyAstronomy-0.9.0/src/pyasl/asl/quadextreme.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/expCorrRN.py` & `PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/expCorrRN.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/sanityExt1Test.py` & `PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/sanityExt1Test.py`

 * *Files 9% similar despite different names*

```diff
@@ -232,8 +232,44 @@
     """
       Example chromospheric age (Donahue)
     """
     from PyAstronomy import pyasl
   
     # Approximate chromospheric age of the Sun
     print "Solar age: {0:4.2f} Ga".format(pyasl.chromoAgeRHK(-4.95))
-  
+  
+  def sanity_abundancepatternsExample(self):
+    """
+      Checking example of AbundancePatterns
+    """
+    from PyAstronomy import pyasl
+
+    ap = pyasl.AbundancePatterns()
+
+    print "Names of the available abundance patterns:"
+    print ap.availablePatterns()
+
+    print
+    print "Get the Asplund et al. pattern (aspl) as a dictionary using"
+    print "atomic number as a key:"
+    print ap.pattern("aspl", form="dict", key="number")
+
+    print
+    print "Get (relative) number abundance of oxygen using elemental symbol:"
+    print ap.abundance("O", pat="wilm")
+    print "or atomic number"
+    print ap.abundance(8, pat="wilm")
+  
+  def sanity_abundancePatterns(self):
+    """
+      Checking abundance pattern
+    """
+    from PyAstronomy import pyasl
+
+    ap = pyasl.AbundancePatterns()
+    
+    self.assertAlmostEqual(2.82e-07, ap.abundance("P", pat="feld"), delta=1e-12, \
+                           msg="Abundance of P (feld) incorrect.")
+    p = ap.pattern("wilm", form="dict", key="symbol")
+    self.assertAlmostEqual(p["Ti"], 6.46e-08, delta=1e-12, \
+                           msg="Ti abundance broken (wilm)")
+
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/ballesterosBV_T.py` & `PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/ballesterosBV_T.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/pizzolato2003tables.dat` & `PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/pizzolato2003tables.dat`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/stellarAge.py` & `PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/stellarAge.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/pizzolato2003.py` & `PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/pizzolato2003.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/ramirez2005tables.dat` & `PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/ramirez2005tables.dat`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/aslExt_1/ramirez2005.py` & `PyAstronomy-0.9.0/src/pyasl/asl/aslExt_1/ramirez2005.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/keplerOrbit.py` & `PyAstronomy-0.9.0/src/pyasl/asl/keplerOrbit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy
 from numpy import pi, abs, sqrt, cos, sin, arccos, arctan, tan
-
+from PyAstronomy.pyaC import pyaErrors as PE
 
 class MarkleyKESolver:
   """
     Solve Kepler's Equation.
     
     This class implements a solver for Kepler's Equation:
     .. math::
@@ -159,64 +159,105 @@
 class KeplerEllipse(object):
   """
     Calculate a Kepler orbit.
     
     The definitions and most of the formulae used in this class
     derive from the book "Orbital Motion" by A.E. Roy.
     
-    The orientation of the ellipse:
+    :Orientation of the ellipse in the coordinate system:
         For zero inclination the ellipse is located in the x-y plane.
         If the eccentricity is increased, the periastron will lie
         in +x direction. If the inclination is increased, the ellipse
         will be rotating around the x-axis, so that +y is rotated
-        toward +z. In increase in Omega corresponds to a rotation
+        toward +z. An increase in Omega corresponds to a rotation
         around the z-axis so that +x is rotated toward +y.
-        Changing `w`, i.e., the longitude of the periastron, will
+        Changing `w`, i.e., the argument of the periastron, will
         not change the plane of the orbit, but rather represent a
-        rotation of the orbit in the plane.
+        rotation of the orbit in the plane. In particular, the
+        periapsis is shifted in the direction of motion.
+        
+    :Orbital angular momentum:
+        For all parameters but semi-major axis and orbital period set to zero,
+        the (orbital) angular momentum points into the +z direction. For an
+        inclination of 90 deg (the remaining parameters remaining zero),
+        it points in the -y direction.
+    
+    :Orientation of the ellipse in the sky:
+        To project the ellipse onto the sky, the coordinate system
+        should be oriented so that the +x direction points North and
+        the +y direction points East (direction of increasing right
+        ascension). The +z axis must be chosen so that the coordinate
+        system becomes right handed. If the line of sight (LOS) points
+        in the +z direction, i.e., the observer is located on the
+        negative z axis, the parameters assume their conventional
+        meaning.
     
+    :The ascending and descending nodes:
+        For systems outside the Solar System, the ascending node is the
+        point where the body "crosses" the plane of the sky away from the
+        observer. Likewise, the descending node is the point where the
+        plane is crossed with the body approaching the observer. For the
+        coordinate system described above and a value of zero for the longitude
+        of the ascending node, the latter is in the North and rotates
+        toward East (i.e., +y) when the longitude of the ascending node
+        is increased.  
+        
+    :The argument and longitude of periapsis:
+        The argument of periapsis is the angle between the ascending node
+        and the periapsis of the body measured in the direction of motion.
+        For exoplanets with circular orbits, for which no well-defined periapsis
+        exists, the argument of periapsis is often chosen so that time
+        of periapsis and central transit time coincide. For the planet, this
+        is the case if the argument of periapsis is -90 deg. However, in the exoplanet
+        literature, the argument of periapsis often refers to the *stellar* orbit
+        (see, e.g., Pollacco et al. 2008, MNRAS 385, 1576-1584, Sect. 3.2.1). In
+        this case, the corresponding value is +90 deg.
+        The so-called longitude of the periapsis is given by the sum of the
+        longitude of the ascending node and the argument of periapsis.
+        
     Parameters
     ----------
     a : float
         Semi-major axis
     per : float
         Orbital period
     e : float, optional
         Orbital eccentricity (0-1).
     tau : float, optional
-        Time of perihelion passage.
+        Time of periapsis passage.
     Omega : float, optional
         Longitude of the ascending node [deg].
     w : float, optional
-        Longitude of perihelion [deg]
+        Argument of periapsis [deg]. Note that the longitude
+        if periapsis is given by Omega+w.
     i : float, optional
         Orbit inclination [deg].
     ks : Class object, optional
         The solver for Kepler's Equation. Default is the
         `MarkleyKESolver`. Each solver must have a `getE`
         method, which takes either a float or array of float
         of mean anomalies and the eccentricity, and returns
         the associated eccentric anomalies.
     
     Attributes
     ----------
     i : float
         Orbit inclination [deg].
     w : float
-        Longitude of perihelion [deg]
+        Argument of periapsis [deg]
     Omega : float
         Longitude of the ascending node [deg]
     e : float
         Eccentricity
     a : float
         Semi-major axis
     per : float
         Orbital period
     tau : float
-        Time of perihelion passage
+        Time of periapsis passage
     ks : Class object
         Solver for Kepler's equation
     _n : float
         Circular frequency.
   """
   
   def _getEccentricAnomaly(self, t):
@@ -435,40 +476,110 @@
     peri = self.xyzPeriastron()
     apas = self.xyzApastron()
     center = (peri + apas) / 2.0
     direc = (peri - apas) / numpy.sqrt( ((peri - apas)**2).sum() )
     ae = self.a * self.e
     return (center + ae*direc, center - ae*direc)
     
-  def xyzNodes(self):
+  def xyzNodes_LOSZ(self, los="+z"):
     """
-      Calculate the nodes of the orbit.
+      Calculate the nodes of the orbit for LOS in +/-z direction.
       
       The nodes of the orbit are the points at which
-      the orbit cuts the observing plane. In this case,
+      the orbit cuts the plane of the sky. In this case,
       these are the points at which the z-coordinate
       vanishes, i.e., the x-y plane is regarded the plane
-      of observation.
+      of the sky.
+      
+      Parameters
+      ----------
+      los : string, {+z,-z}, optional
+          Line of sight points either in +z direction (observer
+          at -z) or vice versa. Changing the direction
+          interchanges the ascending and descending node.
       
       Returns
       -------
       Nodes : Tuple of two coordinate arrays
-          Returns the xyz coordinates of both nodes. 
+          Returns the xyz coordinates of both nodes. The first is the
+          ascending node and the second is the descending node.
     """
-    # f = -w
+    # f = -w (z-component vanishes there)
     E = arctan( tan(-self._w/2.0) * sqrt((1.-self.e)/(1.+self.e)) ) * 2.
     M = E - self.e * sin(E)
     t = M/self._n + self.tau
     node1 = self.xyzPos(t)
+    # Velocity is used to distinguish nodes
+    v1 = self.xyzVel(t)
     # f = -w + pi
     E = arctan( tan((-self._w + pi)/2.0) * sqrt((1.-self.e)/(1.+self.e)) ) * 2.
     M = E - self.e * sin(E)
     t = M/self._n + self.tau
     node2 = self.xyzPos(t)
-    return (node1, node2)
+    # Find the ascending and descending node
+    from PyAstronomy.pyasl import LineOfSight
+    l = LineOfSight(los).los
+    if abs(l[2]) != 1.0:
+      raise(PE.PyAValError("Invalid line of sight (LOS): " + str(los), \
+                           where="xyzNodes_LOSZ", \
+                           solution="Use '-z' or '+z'."))
+
+    if l[2] == 1.0:
+      # Looking in +z direction
+      if v1[2] > 0.0:
+        # First node is ascending
+        return (node1, node2)
+      else:
+        return (node2, node1)
+    else:
+      # Looking in -z direction
+      if v1[2] < 0.0:
+        # First node is ascending
+        return (node1, node2)
+      else:
+        return (node2, node1)
+    
+  def xyzNodes(self):
+    """
+      Calculate the nodes of the orbit.
+      
+      The nodes of the orbit are the points at which
+      the orbit cuts the observing plane. In this case,
+      these are the points at which the z-coordinate
+      vanishes, i.e., the x-y plane is regarded the plane
+      of observation.
+      
+      Returns
+      -------
+      Nodes : Tuple of two coordinate arrays
+          Returns the xyz coordinates of both nodes. 
+    """
+    raise(PE.PyADeprecationError("xyzNodes is deprecated.", \
+                                 solution="Please use 'xyzNodes_LOSZ' instead."))
+
+  def orbAngMomentum(self, t=0.0):
+    """
+      The specific orbital angular momentum of a body in the current orbit.
+      
+      Parameters
+      ----------
+      t : float, optional
+          The time used to calculate the angular momentum. As
+          is it constant for a Kepler orbit, this parameter is
+          of no relevance.
+      
+      Results
+      -------
+      Specific angular momentum : array with three elements
+          The specific angular momentum (i.e., per unit mass)
+          of a body on the current orbit.
+    """
+    r = self.xyzPos(t)
+    v = self.xyzVel(t)
+    return numpy.cross(r, v)
   
   def projPlaStDist(self, t):
     """
       Calculate the sky-projected planet-star separation.
       
       Parameters
       ----------
```

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/decimalYear.py` & `PyAstronomy-0.9.0/src/pyasl/asl/decimalYear.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/coordinates.py` & `PyAstronomy-0.9.0/src/pyasl/asl/coordinates.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/angularDistance.py` & `PyAstronomy-0.9.0/src/pyasl/asl/angularDistance.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/sindex.py` & `PyAstronomy-0.9.0/src/pyasl/asl/sindex.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/svd.py` & `PyAstronomy-0.9.0/src/pyasl/asl/svd.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyasl/asl/aitoffLegacy.py` & `PyAstronomy-0.9.0/src/pyasl/asl/aitoffLegacy.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/constants/exampleSanity.py` & `PyAstronomy-0.9.0/src/constants/exampleSanity.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/constants/itc.py` & `PyAstronomy-0.9.0/src/constants/itc.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/constants/cdat.dat` & `PyAstronomy-0.9.0/src/constants/cdat.dat`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/constants/__init__.py` & `PyAstronomy-0.9.0/src/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaGui/interactiveGV.py` & `PyAstronomy-0.9.0/src/pyaGui/interactiveGV.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaGui/exampleSanity.py` & `PyAstronomy-0.9.0/src/pyaGui/exampleSanity.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaGui/pyaPicker.py` & `PyAstronomy-0.9.0/src/pyaGui/pyaPicker.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaGui/ffmodelExplorer.py` & `PyAstronomy-0.9.0/src/pyaGui/ffmodelExplorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,30 +133,32 @@
     
     if lims:
         if False: # if old fit ranges -> use old indices... lims == self.fitLims and self.fitIdx:
             odf.fit(self.x[self.fitIdx], self.y[self.fitIdx], yerr=self.yerr[self.fitIdx])
         else:
             self.fitLims = lims
             self.fitIdx = numpy.where(numpy.logical_and(self.x >= self.fitLims[0], self.x <= self.fitLims[1]))[0]
-	    if verbose>1:
-	      print "fit index: ",self.fitIdx
-	      print "         x ",self.x[self.fitIdx]
-	      print "         y ", self.y[self.fitIdx]
-	      if self.yerr: print "    yerr ",self.yerr[self.fitIdx]
-	      print "     model ",odf.evaluate(self.x[self.fitIdx])
-            if self.yerr  is not None:
-	       odf.fit(self.x[self.fitIdx], self.y[self.fitIdx], yerr=self.yerr[self.fitIdx])
-	    else:
-	       odf.fit(self.x[self.fitIdx], self.y[self.fitIdx])
+            if verbose > 1:
+              print "fit index: ",self.fitIdx
+              print "         x ",self.x[self.fitIdx]
+              print "         y ", self.y[self.fitIdx]
+              if self.yerr: print "    yerr ",self.yerr[self.fitIdx]
+              print "     model ",odf.evaluate(self.x[self.fitIdx])
+            if self.yerr is not None:
+              odf.fit(self.x[self.fitIdx], self.y[self.fitIdx], yerr=self.yerr[self.fitIdx])
+            else:
+              odf.fit(self.x[self.fitIdx], self.y[self.fitIdx])
     else:
         if self.yerr is not None:
-	    odf.fit(self.x, self.y, yerr=self.yerr)
+          odf.fit(self.x, self.y, yerr=self.yerr)
         else:
-	    odf.fit(self.x, self.y)
+          odf.fit(self.x, self.y)
+
 
+    
 class SetToDialog(tk.Toplevel):
   
   def __init__(self, parent, oldVal, pname):
     tk.Toplevel.__init__(self, parent)
     self.transient(parent)
     self.parent = parent
     self.newVal = None
@@ -265,16 +267,19 @@
     self.modelEntry.bind('<Return>', self._updateModelName)
     self.modelEntry.grid(row=0,column=1)
     
     self.showText = tk.Text(self.showFrame)
     self.showText.config(background='white')
     self.showText.grid(row=1,column=0,columnspan=2) #.pack(expand=True)
     
+    self.clipboardButton = tk.Button(self.showFrame, text="Copy to Clipboard", command=self._copyToClipboard)
+    self.clipboardButton.grid(row=2, column=0, columnspan=2)
+    
     self.helpLabel = tk.Label(self.showFrame, text="You may use the above code for pasting...")
-    self.helpLabel.grid(row=2, column=0, columnspan=2)
+    self.helpLabel.grid(row=3, column=0, columnspan=2)
     
     self.showFrame.pack()
     
     self.protocol("WM_DELETE_WINDOW", self._windowClosed)
 
   def _updateModelName(self, *args):
       self.updateInfo(self.odf)
@@ -296,14 +301,18 @@
     
     self.showText.config(width=max(map(lambda x: len(x), lines)), \
                          height=len(lines)+1)
     t = "".join(map(lambda x: x + "\n", lines))
     self.showText.insert(tk.END, t)
     self.showText.config(state=tk.DISABLED)
 
+  def _copyToClipboard(self):
+    self.clipboard_clear()
+    text = self.showText.get("1.0",tk.END)
+    self.clipboard_append(text)
   def _windowClosed(self):
     """
       The window is closed.
     """
     # Tell the parent that the window does no longer exist
     self.parent.parSumWin = None
     self.destroy()
@@ -388,29 +397,37 @@
     def hitReturn(k):
       def change(*args):
         self.selectedPar.set(k)
         self.odf[k] = float(self.singleParameterVar[k].get())
         self._parameterValueChanged()
       return change  
     
-    # defines what heppens when a parameter's value is changed, but not set yet, i.e., not current (closures)
+    # defines what happens when a parameter's value is changed, but not set yet, i.e., not current (closures)
     def parameterValueChanged(k):
         def valueChanged(*args):
             pp,ll = str(self.singleParameterVar[k].get()).find("."), len(str(self.singleParameterVar[k].get()))
             if round(self.odf[k],ll-pp-1) != round(self.singleParameterVar[k].get(), ll-pp-1):
                 self.singleParameterEntry[k].configure(bg = "red")
             else:
                 self.singleParameterEntry[k].configure(bg = "white")
         return valueChanged    
     
+    
     # Create an entry for each parameter
+      ## Create a scrollable region
+      ## Check maximum number of characters for parameter names:
+    maxParamLen = 0
+    for k in sorted(self.odf.parameters().keys()):
+      if len(k) > maxParamLen:
+        maxParamLen = len(k)
+      ## Create an entry for each parameter	
     for k in sorted(self.odf.parameters().keys()):
       x = tk.Frame(self.parameterFrame, height=2, bd=2, relief=tk.SUNKEN,pady=2)
       self.singleParameterFrames[k] = x 
-      y0 = tk.Radiobutton(x, text=k,variable=self.selectedPar,value=k, width=3)
+      y0 = tk.Radiobutton(x, text=k,variable=self.selectedPar,value=k, width=maxParamLen+1, indicatoron=0)
       y0.pack(side=tk.LEFT)
       #y1 = tk.StringVar()
       y1 = tk.DoubleVar()
       y1.set(self.odf[k])
       y2 = tk.Entry(x, textvariable=y1, width=8)
       y2.bind('<Return>', hitReturn(k))
       self.singleParameterVar[k] = y1
@@ -608,18 +625,21 @@
       #print self.chi2value.get(), self.fit_lo.get(), self.fit_hi.get()
       self.f.canvas.draw()    
 
   def _updateDof(self):
       self.dofValue.set(len(self.plotter.fitIdx)- len(self.odf.freeParameters())-1)
       
   def _updateChi2(self):
-      if self.plotter.chi2 > 1e-3 and self.plotter.chi2 < 1e4:
+      try:
+        if self.plotter.chi2 > 1e-3 and self.plotter.chi2 < 1e4:
           self.chi2value.set("%8.3f" % self.plotter.chi2)
-      else:
+        else:
           self.chi2value.set("%8.3e" % self.plotter.chi2)
+      except:
+        self.chi2value.set("N/A")
   
   def _parameterSummaryClicked(self, *args):
     """
     """
     if self.root.parSumWin is None:
       self.root.parSumWin = ShowParameterSummary(self.root, self.odf)
     self.root.parSumWin.updateInfo(self.odf)
@@ -707,16 +727,16 @@
       newText = "% g" % (self.odf[self.selectedPar.get()])
       #self.valLabel.config(text=newText)
       #print self.selectedPar.get()
       #print "selected Par: ",self.selectedPar.get()," value: ",self.odf[self.selectedPar.get()]
       self.singleParameterVar[self.selectedPar.get()].set(newText)
     else:
       for p in self.odf.freeParamNames():
-	newText = "% g" % (self.odf[p])
-	self.singleParameterVar[p].set(newText)
+        newText = "% g" % (self.odf[p])
+        self.singleParameterVar[p].set(newText)
 
     self.plotter.plot(self.f, self.odf)
     #print self.plotter.chi2
     self._updateChi2()
     self.f.canvas.draw()
 
   def _onWheel(self, event):
@@ -730,16 +750,16 @@
     except ValueError:
       tkMessageBox.showwarning("Invalid float", "Cannot convert " + self.modEntry.get() + " to float." + \
                                " Make it a valid value to proceed.")
       return
     if self.modModus.get() == "mul":
         if event.delta>0:
           self.odf[pname] = val * mf
-	else:
-	  self.odf[pname] = val / mf
+        else:
+          self.odf[pname] = val / mf
     else:
         self.odf[pname] = val + mf * event.delta/2.
     self._parameterValueChanged()
 
   def _mouseWheel(self, event):
     """
       Mouse wheel moved
@@ -808,8 +828,8 @@
     PE.warn(PE.PyADeprecationError("Please note that the dropdown version is no longer supported. " + \
                                    "The list version will be called instead."))
     ffmod = FFModelExplorerList(odf, plotter)
     return ffmod
   else:
     raise(PE.PyAValError("Unknown version: '" + str(version) + "'", \
                          where="ffmodelExplorer", \
-                         solution="Choose between 'list' and 'dropdown'."))
+                         solution="Choose between 'list' and 'dropdown'."))
```

### Comparing `PyAstronomy-0.8.1/src/pyaGui/continuumFinder.py` & `PyAstronomy-0.9.0/src/pyaGui/continuumFinder.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/TutorialExampleSanity.py` & `PyAstronomy-0.9.0/src/funcFit/TutorialExampleSanity.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,22 @@
 
 class ExampleSanity(unittest.TestCase):
   
   def setUp(self):
     pass
   
   def tearDown(self):
-    try:
-      os.remove("mcmcExample.tmp")
-    except:
-      print "Could not remove file: mcmcExample.tmp"
-    try:
-      os.remove("mcmcTA.tmp")
-    except:
-      print "Could not remove file: mcmcTA.tmp"
-    try:
-      os.remove("mcmcSample.tmp")
-    except:
-      print "Could not remove file: mcmcSample.tmp"
+    pass
 
   
   def sanity_firstExample(self):
     # Import numpy and matplotlib
     from numpy import arange, sqrt, exp, pi, random, ones
-    import matplotlib.pylab as mpl
-    # ... and now the funcFit module
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
     from PyAstronomy import funcFit as fuf
     
     # Before we can start fitting, we need something to fit.
     # So let us create some data...
     
     # Creating a Gaussian with some noise
     # Choose some parameters...
@@ -37,20 +26,20 @@
     # Calculate profile
     x = arange(100) - 50.0
     y = gPar["off"] + gPar["A"] / sqrt(2*pi*gPar["sig"]**2) \
         * exp(-(x-gPar["mu"])**2/(2*gPar["sig"]**2))
     # Add some noise
     y += random.normal(0.0, 0.01, x.size)
     # Let us see what we have done...
-    mpl.plot(x, y, 'bp') 
-  
+    plt.plot(x, y, 'bp')
+    
     # Now we can start exploiting the funcFit functionality to
     # fit a Gaussian to our data. In the following lines, we
     # create a fitting object representing a Gaussian and set guess parameters.
-  
+    
     # Now let us come to the fitting
     # First, we create the Gauss1d fit object
     gf = fuf.GaussFit1d()
     # See what parameters are available
     print "List of available parameters: ", gf.availableParameters()
     # Set guess values for the parameters
     gf["A"] = -10.0
@@ -60,45 +49,45 @@
     # Let us see whether the assignment worked
     print "Parameters and guess values: "
     print "  A   : ", gf["A"]
     print "  sig : ", gf["sig"]
     print "  off : ", gf["off"]
     print "  mu  : ", gf["mu"]
     print ""
-  
+    
     # Now some of the strengths of funcFit are demonstrated; namely, the
     # ability to consider some parameters as free and others as fixed.
     # By default, all parameters of the GaussFit1d are frozen.
     
     # Show values and names of frozen parameters
-    print "Names and values if FROZEN parameters: ", gf.frozenParameters()
-  
+    print "Names and values of FROZEN parameters: ", gf.frozenParameters()
+    
     # Which parameters shall be variable during the fit?
     # 'Thaw' those (the order is irrelevant)
     gf.thaw(["A", "sig", "off", "mu"])
     
     # Let us assume that we know that the amplitude is negative, i.e.,
     # no lower boundary (None) and 0.0 as upper limit.
     gf.setRestriction({"A":[None,0.0]})
     
     # Now start the fit
     gf.fit(x, y, yerr=ones(x.size)*0.01)
     
     # Write the result to the screen and plot the best fit model
     gf.parameterSummary()
-    mpl.plot(x, gf.model, 'r--')
+    plt.plot(x, gf.model, 'r--')
     
     # Show the data and the best fit model
-    # mpl.show()
+#     plt.show()
 
   def sanity_CustomModel(self):
     # Import numpy and matplotlib
     from numpy import arange, random
-    import matplotlib.pylab as mpl
-    # ... and now the funcFit module
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
     from PyAstronomy import funcFit as fuf
     
     class StraightLine(fuf.OneDFit):
       """
         Implements a straight line of the form y = "off" + x * "lin".
       """
     
@@ -112,15 +101,15 @@
     
           Parameters:
             - `x` - Array specifying the positions at \
                     which to evaluate the model.
         """
         y = self["off"] + (self["lin"] * x)
         return y
-    
+      
     # Generate some data and add noise
     x = arange(100)
     y = 10.0 + 2.0 * x + random.normal(0.0, 5.0, 100)
     
     # Create fitting class instance and set initial guess
     # Note that all parameters are frozen by default
     lf = StraightLine()
@@ -130,23 +119,23 @@
     lf.thaw(["off", "lin"])
     
     # Start fitting
     lf.fit(x, y)
     
     # Investigate the result
     lf.parameterSummary()
-    mpl.plot(x, y, 'bp')
-    mpl.plot(x, lf.model, 'r--')
-    #  mpl.show()
-
+    plt.plot(x, y, 'bp')
+    plt.plot(x, lf.model, 'r--')
+#     plt.show()
+    
   def sanity_Relations(self):
     # import numpy and matplotlib
     from numpy import arange, random
-    import matplotlib.pylab as mpl
-    # ... and now the funcFit module
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
     from PyAstronomy import funcFit as fuf
     
     class StraightLine(fuf.OneDFit):
       """
         Implements a straight line of the form y = "off" + x * "lin".
       """
     
@@ -168,52 +157,53 @@
     
     def getLinearRelation(factor):
       def linOffRel(off):
         """
           Function used to relate parameters "lin" and "off".
         """
         return factor * off
+      return linOffRel
     
     # Note, above we used a nested function (a closure) to define
     # the relation. This approach is very flexible. If we were already
     # sure about the value of ``factor'' (e.g., 10.0), we could
     # simply have used:
     #
     # def linOffRel(off):
     #   return 10.0 * off
     
     # Generate some data with noise
     x = arange(100)
-    y = 10.0 + 2.0 * x + random.normal(0.0, 5.0, 100)
+    y = 100.0 + 2.0 * x + random.normal(0.0, 5.0, 100)
     
     # Create fitting class instance and set initial guess
     lf = StraightLine()
     lf["off"] = 20.0
     lf["lin"] = 1.0
     # Thaw parameters
     lf.thaw(["off", "lin"])
     
     # Assume we know about a relation between 'lin' and 'off'
     # In particular, lin = 9.0 * off. We use the function getLinearRelation
     # to obtain a function object defining the relation.
-    lf.relate("lin", ["off"], getLinearRelation(9.0))
+    lf.relate("lin", ["off"], getLinearRelation(9))
     
     # Start fitting
     lf.fit(x, y)
     
     # Investigate the result
     lf.parameterSummary()
-    mpl.plot(x, y, 'bp')
-    mpl.plot(x, lf.model, 'r--')
-    # mpl.show()
-
+    plt.plot(x, y, 'bp')
+    plt.plot(x, lf.model, 'r--')
+#     plt.show()
+  
   def sanity_CombiningModels(self):
     # Import numpy and matplotlib
     from numpy import arange, sqrt, exp, pi, random, ones
-    import matplotlib.pylab as mpl
+    import matplotlib.pylab as plt
     # ... and now the funcFit package
     from PyAstronomy import funcFit as fuf
     
     # Creating Gaussians with some noise
     # Choose some parameters...
     gPar1 = {"A":-5.0, "sig":10.0, "mu":20.0, "off":1.0, "lin":0.0}
     gPar2 = {"A":+10.0, "sig":10.0, "mu":-20.0, "off":0.0, "lin":0.0}
@@ -222,15 +212,15 @@
     y = gPar1["off"] + gPar1["A"] / sqrt(2*pi*gPar1["sig"]**2) \
         * exp(-(x-gPar1["mu"])**2/(2*gPar1["sig"]**2))
     y -= gPar2["off"] + gPar2["A"] / sqrt(2*pi*gPar2["sig"]**2) \
         * exp(-(x-gPar2["mu"])**2/(2*gPar2["sig"]**2))
     # Add some noise
     y += random.normal(0.0, 0.01, x.size)
     # Let us see what we have done...
-    mpl.plot(x, y, 'bp')
+    plt.plot(x, y, 'bp')
     
     # Now let us come to the fitting
     # First, we create two Gauss1d fit objects
     gf1 = fuf.GaussFit1d()
     gf2 = fuf.GaussFit1d()
     
     # Assign guess values for the parameters
@@ -284,21 +274,21 @@
     print
     print "--------------------------------"
     print "Parameters for the combined fit:"
     print "--------------------------------"
     twoG.parameterSummary()
     
     # Show the data and the best fit model
-    mpl.plot(x, twoG.model, 'r--')
-    # mpl.show()
+    plt.plot(x, twoG.model, 'r--')
+#     plt.show()
 
   def sanity_CustomObjectiveFunctions(self):
     # Import numpy and matplotlib
     from numpy import arange, exp, random, ones, sum, abs
-    import matplotlib.pylab as mpl
+    import matplotlib.pylab as plt
     # Import funcFit
     from PyAstronomy import funcFit as fuf
     
     # Define parameters of faked data
     A = 1.0
     tau = 10.
     off = 0.2
@@ -319,127 +309,50 @@
     edf.setRestriction({"A":[0.0,None]})
     # Define initial guess
     edf.assignValue({"A":1.0, "tau": 15., "off":0.2, "t0":50.})
     
     # Do not use chi square, but the linear deviation from model
     # to evaluate quality of fit.
     # Use the "MiniFunc" decorator to define your custom objective
-    # function. This decorator takes the fitting objexct as an
+    # function. This decorator takes the fitting object as an
     # argument. The function has to accept two arguments: the
     # fitting object and the list of free parameters.
     @fuf.MiniFunc(edf)
     def mini(edf, P):
       m = sum(abs(edf.model - edf.y)/edf.yerr)
       print "mini - current parameters: ", P, ", value is: ", m
       return m
     
     # Carry out fit WITH SELF-DEFINED OBJECTIVE FUNCTION
     edf.fit(x, y, yerr=yerr, miniFunc=mini)
     
     # Show parameter values and plot best-fit model.
     edf.parameterSummary()
-    mpl.errorbar(x,y,yerr)
-    mpl.plot(x, edf.model, 'r-')
-    # mpl.show()
-
-  def sanity_MCMCSampler(self):
-    # Import some required modules
-    from numpy import arange, sqrt, exp, pi, random, ones
-    import matplotlib.pylab as mpl
-    import pymc
-    # ... and now the funcFit module
-    from PyAstronomy import funcFit as fuf
-    
-    # Creating a Gaussian with some noise
-    # Choose some parameters...
-    gPar = {"A":-5.0, "sig":10.0, "mu":10.0, "off":1.0, "lin":0.0}
-    # Calculate profile
-    x = arange(100) - 50.0
-    y = gPar["off"] + gPar["A"] / sqrt(2*pi*gPar["sig"]**2) \
-    * exp(-(x-gPar["mu"])**2/(2*gPar["sig"]**2))
-    # Add some noise
-    y += random.normal(0.0, 0.01, x.size)
-    
-    # Now let us come to the fitting
-    # First, we create the Gauss1d fit object
-    gf = fuf.GaussFit1d()
-    # See what parameters are available
-    print "List of available parameters: ", gf.availableParameters()
-    # Set guess values for the parameters
-    gf["A"] = -10.0
-    gf["sig"] = 15.77
-    gf["off"] = 0.87
-    gf["mu"] = 7.5
-    # Let us see whether the assignment worked
-    print "Parameters and guess values: ", gf.parameters()
-    
-    # Which parameters shall be variable during the fit?
-    # 'Thaw' those (the order is irrelevant)
-    gf.thaw(["A", "sig", "off", "mu"])
-    
-    # Let us assume that we know that the amplitude is negative, i.e.,
-    # no lower boundary (None) and 0.0 as upper limit.
-    gf.setRestriction({"A":[None,0.0]})
-    
-    # Now start a simplex fit
-    gf.fit(x,y,yerr=ones(x.size)*0.01)
-    
-    # Obtain the best-fit values derived by the simplex fit.
-    # They are to be used as start values for the MCMC sampling.
-    # Note that 'A' is missing - we will introduce this later.
-    X0 = {"sig":gf["sig"], "off":gf["off"], "mu":gf["mu"]}
-    
-    # Now we specify the limits within which the individual parameters
-    # can be varied (for those parameters listed in the 'X0' dictionary).
-    Lims = {"sig":[-20.,20.], "off":[0.,2.], "mu":[5.,15.]}
-    
-    # For the parameters contained in 'X0', define the step widths, which
-    # are to be used by the MCMC sampler. The steps are specified using
-    # the same scale/units as the actual parameters.
-    steps = {"A":0.01, "sig":0.1, "off":0.1, "mu":0.1}
-    
-    # In this example, we wish to define our ``own'' PyMC variable for the parameter
-    # 'A'. This can be useful, if nonstandard behavior is desired. Note that this
-    # is an optional parameter and you could simply include the parameter 'A' into
-    # The framework of X0, Lims, and steps.
-    ppa = {}
-    ppa["A"] = pymc.Uniform("A", value=gf["A"], lower=-20., \
-                            upper=10.0, doc="Amplitude")
-    
-    # Start the sampling. The resulting Marchov-Chain will be written
-    # to the file 'mcmcExample.tmp'.
-    gf.fitMCMC(x, y, X0, Lims, steps, yerr=ones(x.size)*0.01, \
-               pymcPars=ppa, iter=2500, burn=0, thin=1, \
-               dbfile="mcmcExample.tmp")
-    
-    # Reload the database (here, this is actually not required, but it is
-    # if the Marchov chain is to be analyzed later).
-    db = pymc.database.pickle.load('mcmcExample.tmp')
-    # Plot the trace of the amplitude, 'A'.
-    mpl.hist(db.trace("A", 0)[:])
-    # mpl.show()
+    plt.errorbar(x,y,yerr)
+    plt.plot(x, edf.model, 'r-')
+#     plt.show()
 
   def sanity_Overbinning(self):
     # Import numpy and matplotlib
     from numpy import arange, sqrt, exp, pi, random, ones
-    import matplotlib.pylab as mpl
-    # ... and now the funcFit module
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
     from PyAstronomy import funcFit as fuf
     
     # Creating a Gaussian with some noise
     # Choose some parameters...
     gPar = {"A":-5.0, "sig":10.0, "mu":10.0, "off":1.0, "lin":0.0}
     # Calculate profile
     x = arange(20)/20.0 * 100.0 - 50.0
     y = gPar["off"] + gPar["A"] / sqrt(2*pi*gPar["sig"]**2) \
         * exp(-(x-gPar["mu"])**2/(2*gPar["sig"]**2))
     # Add some noise
     y += random.normal(0.0, 0.01, x.size)
     # Let us see what we have done...
-    mpl.plot(x, y, 'bp')
+    plt.plot(x, y, 'bp')
     
     # First, we create a "GaussFit1d_Rebin" class object (note that the
     # class object has still to be instantiated, the name is arbitrary).
     GaussFit1d_Rebin = fuf.turnIntoRebin(fuf.GaussFit1d)
     # Do the instantiation and specify how the overbinning should be
     # carried out.
     gf = GaussFit1d_Rebin()
@@ -476,27 +389,27 @@
     
     # Now start the fit
     gf.fit(x, y, yerr=ones(x.size)*0.01)
     
     # Write the result to the screen and plot the best fit model
     gf.parameterSummary()
     # Plot the final best-fit model
-    mpl.plot(x, gf.model, 'rp--')
+    plt.plot(x, gf.model, 'rp--')
     # Show the overbinned (=unbinned) model, indicate by color
     # which point are averaged to obtain a point in the binned
     # model.
     for k, v in gf.rebinIdent.iteritems():
       c = "y"
       if k % 2 == 0: c = "k"
-      mpl.plot(gf.rebinTimes[v], gf.unbinnedModel[v], c+'.')
-    
+      plt.plot(gf.rebinTimes[v], gf.unbinnedModel[v], c+'.')   
+
   def sanity_simultaneousFit(self):
     from PyAstronomy import funcFit as fuf
     import numpy
-    import matplotlib.pylab as mpl
+    import matplotlib.pylab as plt
     
     # Set up two different x axes.
     x1 = numpy.arange(100.)/100. - 0.5
     x2 = numpy.arange(150.)/150. - 0.25
     
     # Getting the models ...
     gauss = fuf.GaussFit1d()
@@ -506,18 +419,18 @@
     calor.assignValue({"A":0.07, "g":0.1, "mu":0.2, "off":1.0, "lin":0.0})
     
     # Create noisy data.
     y1 = gauss.evaluate(x1) + numpy.random.normal(0., 0.01, 100)
     y2 = calor.evaluate(x2) + numpy.random.normal(0., 0.01, 150)
     
     # Plot the noisy data.
-    mpl.subplot(2,1,1)
-    mpl.errorbar(x1, y1, yerr=numpy.ones(100)*0.01)
-    mpl.subplot(2,1,2)
-    mpl.errorbar(x2, y2, yerr=numpy.ones(150)*0.01)
+    plt.subplot(2,1,1)
+    plt.errorbar(x1, y1, yerr=numpy.ones(100)*0.01)
+    plt.subplot(2,1,2)
+    plt.errorbar(x2, y2, yerr=numpy.ones(150)*0.01)
     
     # Now, get ready two fit the data sets simultaneously.
     sf = fuf.SyncFitContainer()
     # Tell the class about the two components and save the
     # component numbers assigned to them:
     gaussCno = sf.addComponent(gauss)
     calorCno = sf.addComponent(calor)
@@ -562,165 +475,20 @@
     
     # Show the best-fit values.
     print
     print "Best-fit parameters:"
     sf.parameterSummary()
     
     # Plot the best-fit model(s).
-    mpl.subplot(2,1,1)
-    mpl.plot(x1, sf.models[gaussCno], 'r--')
-    mpl.subplot(2,1,2)
-    mpl.plot(x2, sf.models[calorCno], 'r--')
-    
-    # mpl.show()
-
-
-  def sanity_MCMCPriorExample(self):
-    from PyAstronomy import funcFit as fuf
-    import numpy as np
-    import matplotlib.pylab as plt
-    import pymc
-    
-    # Create a Gauss-fit object
-    gf = fuf.GaussFit1d()
-    
-    # Choose some parameters
-    gf["A"] = -0.65
-    gf["mu"] = 1.0
-    gf["lin"] = 0.0
-    gf["off"] = 1.1
-    gf["sig"] = 0.2
-    
-    # Simulate data with noise
-    x = np.linspace(0., 2., 100)
-    y = gf.evaluate(x)
-    y += np.random.normal(0, 0.05, len(x))
-    
-    gf.thaw(["A", "off", "mu", "sig"])
-    
-    # Set up a normal prior for the offset parameter
-    # Note!---The name (first parameter) must correspond to that
-    #         of the parameter.
-    # The expectation value us set to 0.9 while the width is given
-    # as 0.01 (tau = 1/sigma**2). The starting value is specified
-    # as 1.0.
-    offPar = pymc.Normal("off", mu=0.9, tau=(1./0.01)**2, value=1.0)
-    # Use a uniform prior for mu.
-    muPar = pymc.Uniform("mu", lower=0.95, upper=0.97, value=0.96)
-    
-    # Collect the "extra"-variables in a dictionary using
-    # their names as keys
-    pymcPars = {"mu":muPar, "off":offPar}
-    
-    # Specify starting values, X0, and limits, lims, for
-    # those parameter distributions not given specifically.
-    X0 = {"A":gf["A"], "sig":gf["sig"]}
-    lims = {"A":[-1.0,0.0], "sig":[0., 1.0]}
-    # Still, the steps dictionary has to contain all
-    # parameter distributions.
-    steps = {"A":0.02, "sig":0.02, "mu":0.01, "off":0.01}
-    
-    # Carry out the MCMC sampling
-    gf.fitMCMC(x, y, X0, lims, steps, yerr=np.ones(len(x))*0.05, \
-               pymcPars=pymcPars, burn=1000, iter=3000)
-    
-    # Setting parameters to mean values
-    for p in gf.freeParameters():
-      gf[p] = gf.MCMC.trace(p)[:].mean()
-    
-    # Show the "data" and model in the upper panel
     plt.subplot(2,1,1)
-    plt.title("Data and model")
-    plt.errorbar(x, y, yerr=np.ones(len(x))*0.05, fmt="bp")
-    # Plot lowest deviance solution
-    plt.plot(x, gf.evaluate(x), 'r--')
-    
-    # Show the residuals in the lower panel
+    plt.plot(x1, sf.models[gaussCno], 'r--')
     plt.subplot(2,1,2)
-    plt.title("Residuals")
-    plt.errorbar(x, y-gf.evaluate(x), yerr=np.ones(len(x))*0.05, fmt="bp")
-    plt.plot([min(x), max(x)], [0.0,0.0], 'r-')
-    
-    #plt.show()
-    
-  def sanity_autoMCMCExample1(self):
-    from PyAstronomy import funcFit as fuf
-    import numpy as np
-    import matplotlib.pylab as plt
-    
-    x = np.linspace(0,30,1000)
-    gauss = fuf.GaussFit1d()
-    gauss["A"] = 1
-    gauss["mu"] = 23.
-    gauss["sig"] = 0.5
-    # Generate some "data" to fit
-    yerr = np.random.normal(0., 0.05, len(x))
-    y = gauss.evaluate(x) + yerr
-    # Thaw the parameters A, mu, and sig
-    gauss.thaw(["A","mu","sig"])
-    
-    # Define the ranges, which are used to construct the
-    # uniform priors and step sizes.
-    # Note that for "sig", we give only a single value.
-    # In this case, the limits for the uniform prior will
-    # be constructed as [m0-1.5, m0+1.5], where m0 is the
-    # starting value interpreted as the current value of
-    # mu (23. in this case).
-    ranges = {"A":[0,10],"mu":3, "sig":[0.1,1.0]}
-    # Generate default input for X0, lims, and steps
-    X0, lims, steps = gauss.MCMCautoParameters(ranges)
-    
-    # Show what happened...
-    print
-    print "Auto-generated input parameters:"
-    print "X0: ", X0
-    print "lims: ", lims
-    print "steps: ", steps
-    print
-    # Call the usual sampler
-    gauss.fitMCMC(x, y, X0, lims, steps, yerr=yerr, iter=1000)
-    
-    # and plot the results
-    plt.plot(x, y, 'k+')
-    plt.plot(x, gauss.evaluate(x), 'r--')
-#    plt.show() 
-
-  def sanity_autoMCMCExample2(self):
-    from PyAstronomy import funcFit as fuf
-    import numpy as np
-    import matplotlib.pylab as plt
+    plt.plot(x2, sf.models[calorCno], 'r--')
     
-    x = np.linspace(0,30,1000)
-    gauss = fuf.GaussFit1d()
-    gauss["A"] = 1
-    gauss["mu"] = 23.
-    gauss["sig"] = 0.5
-    # Generate some "data" to fit
-    yerr = np.random.normal(0., 0.05, len(x))
-    y = gauss.evaluate(x) + yerr
-    
-    # Define the ranges, which are used to construct the
-    # uniform priors and step sizes.
-    # Note that for "sig", we give only a single value.
-    # In this case, the limits for the uniform prior will
-    # be constructed as [m0-1.5, m0+1.5], where m0 is the
-    # starting value interpreted as the current value of
-    # mu (23. in this case).
-    ranges = {"A":[0,10],"mu":3, "sig":[0.1,1.0]}
-    
-    # Call the auto-sampler
-    # Note that we set picky to False here. In this case, the
-    # parameters specified in ranges will be thawed automatically.
-    # All parameters not mentioned there, will be frozen.
-    gauss.autoFitMCMC(x, y, ranges, yerr=yerr, picky=False, iter=1000)
-    
-    # and plot the results
-    plt.plot(x, y, 'k+')
-    plt.plot(x, gauss.evaluate(x), 'r--')
-#    plt.show()
+#     plt.show()
 
   def sanity_2dCircularFit(self):
     import numpy as np
     import matplotlib.pylab as plt
     from PyAstronomy import funcFit as fuf
     
     # Get the circular model and assign
@@ -1061,14 +829,330 @@
     plt.plot([cfi90["limits"][0]]*2, [min(chis), max(chis)], 'k--')
     plt.plot([cfi90["limits"][1]]*2, [min(chis), max(chis)], 'k--')
     plt.plot([cfi68["limits"][0]]*2, [min(chis), max(chis)], 'b--')
     plt.plot([cfi68["limits"][1]]*2, [min(chis), max(chis)], 'b--')
     
 #    plt.show()
 
+
+  def sanity_conditionalRestrictions(self):
+    """
+      Check the conditional restriction example.
+    """
+    import numpy as np
+    import matplotlib.pylab as plt
+    from PyAstronomy import funcFit as fuf
+    
+    # Get fitting object for a Gaussian ...
+    g = fuf.GaussFit1d()
+    # .. and define the parameters
+    g["A"] = 0.97
+    g["mu"] = 0.1
+    g["sig"] = 0.06
+    
+    # Generate some "data" with noise included
+    x = np.linspace(-1.0,1.0,200)
+    y = g.evaluate(x) + np.random.normal(0.0, 0.1, len(x))
+    yerr = np.ones(len(x)) * 0.1
+    
+    
+    def myRestriction(A, sig):
+      """
+        A conditional restriction.
+    
+        Returns
+        -------
+        Penalty : float
+            A large value if condition is violated
+            and zero otherwise.
+      """
+      if A > 10.0*sig:
+        return np.abs(A-10.0*sig + 1.0)*1e20
+      return 0.0
+    
+    
+    # Add the conditional restriction to the model and save
+    # the unique ID, which can be used to refer to that
+    # restriction.
+    uid = g.addConditionalRestriction(["A", "sig"], myRestriction)
+    print "Conditional restriction has been assigned the ID: ", uid
+    print
+    
+    # Now see whether the restriction is really in place
+    g.showConditionalRestrictions()
+    
+    # Define free parameters ...
+    g.thaw(["A", "mu", "sig"])
+    # ... and fit the model (restriction included)
+    g.fit(x, y, yerr=yerr)
+    
+    # Save the resulting best-fit model
+    restrictedModel = g.model.copy()
+    
+    # Remove the conditional restriction and re-fit
+    g.removeConditionalRestriction(uid)
+    g.fit(x, y, yerr=yerr)
+    
+    # Save new model
+    unrestrictedModel = g.model.copy()
+    
+    # Plot the result
+#    plt.errorbar(x, y, yerr=yerr, fmt='b.')
+#    plt.plot(x, restrictedModel, 'r--', label="Restricted")
+#    plt.plot(x, unrestrictedModel, 'g--', label="Unresctricted")
+#    plt.legend()
+#    plt.show()
+
+
+class MCMCExampleSanity(unittest.TestCase):
+  
+  def setUp(self):
+    pass
+  
+  def tearDown(self):
+    try:
+      os.remove("mcmcExample.tmp")
+    except:
+      print "Could not remove file: mcmcExample.tmp"
+    try:
+      os.remove("mcmcTA.tmp")
+    except:
+      print "Could not remove file: mcmcTA.tmp"
+    try:
+      os.remove("mcmcSample.tmp")
+    except:
+      print "Could not remove file: mcmcSample.tmp"
+    try:
+      os.remove("chain.emcee")
+    except:
+      pass
+
+  def sanity_MCMCSampler(self):
+    # Import some required modules
+    from numpy import arange, sqrt, exp, pi, random, ones
+    import matplotlib.pylab as mpl
+    import pymc
+    # ... and now the funcFit module
+    from PyAstronomy import funcFit as fuf
+    
+    # Creating a Gaussian with some noise
+    # Choose some parameters...
+    gPar = {"A":-5.0, "sig":10.0, "mu":10.0, "off":1.0, "lin":0.0}
+    # Calculate profile
+    x = arange(100) - 50.0
+    y = gPar["off"] + gPar["A"] / sqrt(2*pi*gPar["sig"]**2) \
+    * exp(-(x-gPar["mu"])**2/(2*gPar["sig"]**2))
+    # Add some noise
+    y += random.normal(0.0, 0.01, x.size)
+    
+    # Now let us come to the fitting
+    # First, we create the Gauss1d fit object
+    gf = fuf.GaussFit1d()
+    # See what parameters are available
+    print "List of available parameters: ", gf.availableParameters()
+    # Set guess values for the parameters
+    gf["A"] = -10.0
+    gf["sig"] = 15.77
+    gf["off"] = 0.87
+    gf["mu"] = 7.5
+    # Let us see whether the assignment worked
+    print "Parameters and guess values: ", gf.parameters()
+    
+    # Which parameters shall be variable during the fit?
+    # 'Thaw' those (the order is irrelevant)
+    gf.thaw(["A", "sig", "off", "mu"])
+    
+    # Let us assume that we know that the amplitude is negative, i.e.,
+    # no lower boundary (None) and 0.0 as upper limit.
+    gf.setRestriction({"A":[None,0.0]})
+    
+    # Now start a simplex fit
+    gf.fit(x,y,yerr=ones(x.size)*0.01)
+    
+    # Obtain the best-fit values derived by the simplex fit.
+    # They are to be used as start values for the MCMC sampling.
+    # Note that 'A' is missing - we will introduce this later.
+    X0 = {"sig":gf["sig"], "off":gf["off"], "mu":gf["mu"]}
+    
+    # Now we specify the limits within which the individual parameters
+    # can be varied (for those parameters listed in the 'X0' dictionary).
+    Lims = {"sig":[-20.,20.], "off":[0.,2.], "mu":[5.,15.]}
+    
+    # For the parameters contained in 'X0', define the step widths, which
+    # are to be used by the MCMC sampler. The steps are specified using
+    # the same scale/units as the actual parameters.
+    steps = {"A":0.01, "sig":0.1, "off":0.1, "mu":0.1}
+    
+    # In this example, we wish to define our ``own'' PyMC variable for the parameter
+    # 'A'. This can be useful, if nonstandard behavior is desired. Note that this
+    # is an optional parameter and you could simply include the parameter 'A' into
+    # The framework of X0, Lims, and steps.
+    ppa = {}
+    ppa["A"] = pymc.Uniform("A", value=gf["A"], lower=-20., \
+                            upper=10.0, doc="Amplitude")
+    
+    # Start the sampling. The resulting Marchov-Chain will be written
+    # to the file 'mcmcExample.tmp'.
+    gf.fitMCMC(x, y, X0, Lims, steps, yerr=ones(x.size)*0.01, \
+               pymcPars=ppa, iter=2500, burn=0, thin=1, \
+               dbfile="mcmcExample.tmp")
+    
+    # Reload the database (here, this is actually not required, but it is
+    # if the Marchov chain is to be analyzed later).
+    db = pymc.database.pickle.load('mcmcExample.tmp')
+    # Plot the trace of the amplitude, 'A'.
+    mpl.hist(db.trace("A", 0)[:])
+    # mpl.show()
+
+
+  def sanity_MCMCPriorExample(self):
+    from PyAstronomy import funcFit as fuf
+    import numpy as np
+    import matplotlib.pylab as plt
+    import pymc
+    
+    # Create a Gauss-fit object
+    gf = fuf.GaussFit1d()
+    
+    # Choose some parameters
+    gf["A"] = -0.65
+    gf["mu"] = 1.0
+    gf["lin"] = 0.0
+    gf["off"] = 1.1
+    gf["sig"] = 0.2
+    
+    # Simulate data with noise
+    x = np.linspace(0., 2., 100)
+    y = gf.evaluate(x)
+    y += np.random.normal(0, 0.05, len(x))
+    
+    gf.thaw(["A", "off", "mu", "sig"])
+    
+    # Set up a normal prior for the offset parameter
+    # Note!---The name (first parameter) must correspond to that
+    #         of the parameter.
+    # The expectation value us set to 0.9 while the width is given
+    # as 0.01 (tau = 1/sigma**2). The starting value is specified
+    # as 1.0.
+    offPar = pymc.Normal("off", mu=0.9, tau=(1./0.01)**2, value=1.0)
+    # Use a uniform prior for mu.
+    muPar = pymc.Uniform("mu", lower=0.95, upper=0.97, value=0.96)
+    
+    # Collect the "extra"-variables in a dictionary using
+    # their names as keys
+    pymcPars = {"mu":muPar, "off":offPar}
+    
+    # Specify starting values, X0, and limits, lims, for
+    # those parameter distributions not given specifically.
+    X0 = {"A":gf["A"], "sig":gf["sig"]}
+    lims = {"A":[-1.0,0.0], "sig":[0., 1.0]}
+    # Still, the steps dictionary has to contain all
+    # parameter distributions.
+    steps = {"A":0.02, "sig":0.02, "mu":0.01, "off":0.01}
+    
+    # Carry out the MCMC sampling
+    gf.fitMCMC(x, y, X0, lims, steps, yerr=np.ones(len(x))*0.05, \
+               pymcPars=pymcPars, burn=1000, iter=3000)
+    
+    # Setting parameters to mean values
+    for p in gf.freeParameters():
+      gf[p] = gf.MCMC.trace(p)[:].mean()
+    
+    # Show the "data" and model in the upper panel
+    plt.subplot(2,1,1)
+    plt.title("Data and model")
+    plt.errorbar(x, y, yerr=np.ones(len(x))*0.05, fmt="bp")
+    # Plot lowest deviance solution
+    plt.plot(x, gf.evaluate(x), 'r--')
+    
+    # Show the residuals in the lower panel
+    plt.subplot(2,1,2)
+    plt.title("Residuals")
+    plt.errorbar(x, y-gf.evaluate(x), yerr=np.ones(len(x))*0.05, fmt="bp")
+    plt.plot([min(x), max(x)], [0.0,0.0], 'r-')
+    
+    #plt.show()
+    
+  def sanity_autoMCMCExample1(self):
+    from PyAstronomy import funcFit as fuf
+    import numpy as np
+    import matplotlib.pylab as plt
+    
+    x = np.linspace(0,30,1000)
+    gauss = fuf.GaussFit1d()
+    gauss["A"] = 1
+    gauss["mu"] = 23.
+    gauss["sig"] = 0.5
+    # Generate some "data" to fit
+    yerr = np.random.normal(0., 0.05, len(x))
+    y = gauss.evaluate(x) + yerr
+    # Thaw the parameters A, mu, and sig
+    gauss.thaw(["A","mu","sig"])
+    
+    # Define the ranges, which are used to construct the
+    # uniform priors and step sizes.
+    # Note that for "sig", we give only a single value.
+    # In this case, the limits for the uniform prior will
+    # be constructed as [m0-1.5, m0+1.5], where m0 is the
+    # starting value interpreted as the current value of
+    # mu (23. in this case).
+    ranges = {"A":[0,10],"mu":3, "sig":[0.1,1.0]}
+    # Generate default input for X0, lims, and steps
+    X0, lims, steps = gauss.MCMCautoParameters(ranges)
+    
+    # Show what happened...
+    print
+    print "Auto-generated input parameters:"
+    print "X0: ", X0
+    print "lims: ", lims
+    print "steps: ", steps
+    print
+    # Call the usual sampler
+    gauss.fitMCMC(x, y, X0, lims, steps, yerr=yerr, iter=1000)
+    
+    # and plot the results
+    plt.plot(x, y, 'k+')
+    plt.plot(x, gauss.evaluate(x), 'r--')
+#    plt.show() 
+
+  def sanity_autoMCMCExample2(self):
+    from PyAstronomy import funcFit as fuf
+    import numpy as np
+    import matplotlib.pylab as plt
+    
+    x = np.linspace(0,30,1000)
+    gauss = fuf.GaussFit1d()
+    gauss["A"] = 1
+    gauss["mu"] = 23.
+    gauss["sig"] = 0.5
+    # Generate some "data" to fit
+    yerr = np.random.normal(0., 0.05, len(x))
+    y = gauss.evaluate(x) + yerr
+    
+    # Define the ranges, which are used to construct the
+    # uniform priors and step sizes.
+    # Note that for "sig", we give only a single value.
+    # In this case, the limits for the uniform prior will
+    # be constructed as [m0-1.5, m0+1.5], where m0 is the
+    # starting value interpreted as the current value of
+    # mu (23. in this case).
+    ranges = {"A":[0,10],"mu":3, "sig":[0.1,1.0]}
+    
+    # Call the auto-sampler
+    # Note that we set picky to False here. In this case, the
+    # parameters specified in ranges will be thawed automatically.
+    # All parameters not mentioned there, will be frozen.
+    gauss.autoFitMCMC(x, y, ranges, yerr=yerr, picky=False, iter=1000)
+    
+    # and plot the results
+    plt.plot(x, y, 'k+')
+    plt.plot(x, gauss.evaluate(x), 'r--')
+#    plt.show()
+
+
   def sanity_TAtut_createTrace(self):
     """
       TA tutorial, all examples
     """
     import numpy as np
     import matplotlib.pylab as plt
     # ... and now the funcFit package
@@ -1288,74 +1372,157 @@
     X0, lims, steps = gauss.MCMCautoParameters({"A":[0,10],"mu":3, "sig":[0.1,1.0]})
     gauss.fitMCMC(x, y, X0, lims, steps, yerr=yerr, iter=1000)
     
 #     plt.plot(x, y, 'k+')
 #     plt.plot(x, gauss.evaluate(x), 'r--')
 #     plt.show()
 
-  def sanity_conditionalRestrictions(self):
-    """
-      Check the conditional restriction example.
-    """
-    import numpy as np
+  def sanity_EMCEEfirstexample(self):
+
+    # Import numpy and matplotlib
+    from numpy import arange, sqrt, exp, pi, random, ones
     import matplotlib.pylab as plt
+    # ... and now the funcFit package
     from PyAstronomy import funcFit as fuf
     
-    # Get fitting object for a Gaussian ...
-    g = fuf.GaussFit1d()
-    # .. and define the parameters
-    g["A"] = 0.97
-    g["mu"] = 0.1
-    g["sig"] = 0.06
+    # Before we can start fitting, we need something to fit.
+    # So let us create some data...
     
-    # Generate some "data" with noise included
-    x = np.linspace(-1.0,1.0,200)
-    y = g.evaluate(x) + np.random.normal(0.0, 0.1, len(x))
-    yerr = np.ones(len(x)) * 0.1
+    # Choose some signal-to-noise ratio
+    snr = 25.0
     
+    # Creating a Gaussian with some noise
+    # Choose some parameters...
+    gf = fuf.GaussFit1d()
+    gf.assignValues({"A":-5.0, "sig":2.5, "mu":10.0, "off":1.0, "lin":0.0})
+    # Calculate profile
+    x = arange(100) - 50.0
+    y = gf.evaluate(x)
+    # Add some noise
+    y += random.normal(0.0, 1.0/snr, x.size)
     
-    def myRestriction(A, sig):
-      """
-        A conditional restriction.
+    # Define the free parameters
+    gf.thaw(["A", "sig", "mu", "off"])
     
-        Returns
-        -------
-        Penalty : float
-            A large value if condition is violated
-            and zero otherwise.
-      """
-      if A > 10.0*sig:
-        return np.abs(A-10.0*sig + 1.0)*1e20
-      return 0.0
+    # Start a fit (quite dispensable here)
+    gf.fit(x, y, yerr=ones(x.size)/snr)
     
+    # Say, we want 200 burn-in iterations and, thereafter,
+    # 1000 further iterations (per walker).
+    sampleArgs = {"iters":1000, "burn":200}
+    
+    # Start the sampling (ps could be used to continueb the sampling)
+    ps = gf.fitEMCEE(x, y, yerr=ones(x.size)/snr, sampleArgs=sampleArgs)
+    
+    # Plot the distributions of the chains
+    # NOTE: the order of the parameters in the chain object is the same
+    #       as the order of the parameters returned by freeParamNames()
+    for i, p in enumerate(gf.freeParamNames()):
+      plt.subplot(len(gf.freeParamNames()), 1, i+1)
+      plt.hist(gf.emceeSampler.flatchain[::,i], label=p)
+      plt.legend()
+#     plt.show()
+
+
+  def sanity_EMCEEpriorexample(self):
+    # Import numpy and matplotlib
+    from numpy import arange, sqrt, exp, pi, random, ones
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
+    from PyAstronomy import funcFit as fuf
+    import numpy as np
     
-    # Add the conditional restriction to the model and save
-    # the unique ID, which can be used to refer to that
-    # restriction.
-    uid = g.addConditionalRestriction(["A", "sig"], myRestriction)
-    print "Conditional restriction has been assigned the ID: ", uid
+    # Before we can start fitting, we need something to fit.
+    # So let us create some data...
+    
+    # Choose some signal-to-noise ratio
+    snr = 25.0
+    
+    # Choosing an arbitrary constant and ...
+    c = 10.0
+    # ... an equally arbitrary number of data points
+    npoint = 10
+    
+    # Define 'data'
+    x = arange(npoint)
+    y = np.ones(len(x)) * c
+    # Add some noise
+    y += random.normal(0.0, 1.0/snr, x.size)
+    
+    # A funcFit object representing a constant
+    pf = fuf.PolyFit1d(0)
+    pf["c0"] = c
+    
+    # The only parameter shall be free
+    pf.thaw("c0")
+    
+    # Say, we want 200 burn-in iterations and, thereafter,
+    # 2500 further iterations (per walker).
+    sampleArgs = {"iters":2500, "burn":200}
+    
+    # Start the sampling (ps could be used to continueb the sampling)
+    ps = pf.fitEMCEE(x, y, yerr=ones(x.size)/snr, sampleArgs=sampleArgs)
     print
     
-    # Now see whether the restriction is really in place
-    g.showConditionalRestrictions()
+    # Plot the distributions of the chains
+    # NOTE: the order of the parameters in the chain object is the same
+    #       as the order of the parameters returned by freeParamNames()
+    h = plt.hist(pf.emceeSampler.flatchain[::,0], label="c0", normed=True)
+    # Construct "data points" in the middle of the bins
+    xhist = (h[1][1:] + h[1][0:-1]) / 2.0
+    yhist = h[0]
     
-    # Define free parameters ...
-    g.thaw(["A", "mu", "sig"])
-    # ... and fit the model (restriction included)
-    g.fit(x, y, yerr=yerr)
+    # Fit the histogram using a Gaussian
+    gf = fuf.GaussFit1d()
+    gf.assignValues({"A":1.0, "mu":c, "sig":1.0/snr/np.sqrt(npoint)})
+    # First fitting only "mu" is simply quite stable
+    gf.thaw("mu")
+    gf.fit(xhist, yhist)
+    gf.thaw(["A", "sig"])
+    gf.fit(xhist, yhist)
     
-    # Save the resulting best-fit model
-    restrictedModel = g.model.copy()
+    print
+    print "  --- Sampling results ---"
+    print "Posterior estimate of constant: ", np.mean(pf.emceeSampler.flatchain[::,0])
+    print "Nominal error of the mean: ", 1.0/snr/np.sqrt(npoint)
+    print "Estimate from Markov chain: ", np.std(pf.emceeSampler.flatchain[::,0]),
+    print " and from Gaussian fit to distribution: ", gf["sig"]
+    
+    # Evaluate best-fit model ...
+    xmodel = np.linspace(c - 10.0/snr, c + 10.0/snr, 250)
+    ymodel = gf.evaluate(xmodel)
+    # ... and plot
+#     plt.plot(xhist, yhist, 'rp')
+#     plt.plot(xmodel, ymodel, 'r--')
+#     plt.legend()
+#     plt.show()
     
-    # Remove the conditional restriction and re-fit
-    g.removeConditionalRestriction(uid)
-    g.fit(x, y, yerr=yerr)
     
-    # Save new model
-    unrestrictedModel = g.model.copy()
+    # Defining a prior on c0. Prior knowledge tells us that its value
+    # is around 7. Let us choose the standard deviation of the prior so
+    # that the estimate will lie in the middle between 7 and 10. Here we
+    # exploit symmetry and make the prior information as strong as the
+    # information contained in the likelihood function.
+    priors = {"c0":fuf.FuFPrior("gaussian", sig=1.0/snr/np.sqrt(npoint), mu=7.0)}
     
-    # Plot the result
-#    plt.errorbar(x, y, yerr=yerr, fmt='b.')
-#    plt.plot(x, restrictedModel, 'r--', label="Restricted")
-#    plt.plot(x, unrestrictedModel, 'g--', label="Unresctricted")
-#    plt.legend()
-#    plt.show()
+    # Start the sampling (ps could be used to continueb the sampling)
+    ps = pf.fitEMCEE(x, y, yerr=ones(x.size)/snr, sampleArgs=sampleArgs, priors=priors)
+    
+    print
+    print "  --- Sampling results with strong prior information ---"
+    print "Posterior estimate of constant: ", np.mean(pf.emceeSampler.flatchain[::,0]),
+    print " +/-", np.std(pf.emceeSampler.flatchain[::,0])
+    
+    plt.hist(pf.emceeSampler.flatchain[::,0], label="c0", normed=True)
+#     plt.show()
+
+  def sanity_InstatiatePrior(self):
+    from PyAstronomy import funcFit as fuf
+    
+    # Instantiate prior
+    gp = fuf.FuFPrior("gaussian", sig=0.1, mu=1.0)
+    
+    # Current values (arbitrary)
+    cvals = {"a":1.4, "b":0.86, "c":1.1}
+    
+    # Get log(prior) for parameter "b"
+    print gp(cvals, "b")
```

### Comparing `PyAstronomy-0.8.1/src/funcFit/onedfit.py` & `PyAstronomy-0.9.0/src/funcFit/onedfit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # -*- coding: utf-8 -*-
-import numpy
+import numpy as np
 from params import Params
 import re
 import copy
 from new import instancemethod
 from PyAstronomy.pyaC import pyaErrors as PE
 from nameIdentBase import ModelNameIdentBase
 from anneal import PyAAnneal
 from PyAstronomy import pyaC 
 from time import time as timestamp
 from fufDS import FufDS
+from extFitter import NelderMead
 
-from PyAstronomy.funcFit import _pymcImport, _scoImport
+from PyAstronomy.funcFit import _pymcImport, _scoImport, ic
 if _pymcImport:
   import pymc
 if _scoImport:
   import scipy.optimize as sco
+if ic.check["emcee"]:
+  import emcee
+if ic.check["progressbar"]:
+  import progressbar
 
 def addEval(self, x):
   return (self.leftCompo.evaluate(x) + self.rightCompo.evaluate(x))
 
 def subEval(self, x):
   return (self.leftCompo.evaluate(x) - self.rightCompo.evaluate(x))
 
@@ -556,14 +561,194 @@
   removeConditionalRestriction.__doc__ = Params.removeConditionalRestriction.__doc__
   
   def showConditionalRestrictions(self, **kwargs):
     return self.pars.showConditionalRestrictions(**kwargs)
   showConditionalRestrictions.__doc__ = Params.showConditionalRestrictions.__doc__
 
 
+
+class IFitterBase:
+  """
+    Base class for internal fitter.
+  """
+  
+  def __init__(self):
+    self._objfval = None
+  
+  def fit(self, minifunc, x0):
+    """
+      Carry out the minimization.
+      
+      Parameters
+      ----------
+      minifunc : callable
+          Objective function.
+      x0 : list
+          Starting values
+      
+      Returns
+      -------
+      Result : list or tuple
+          First item is a list of the best-fit values and second
+          item is the value of the objective function.
+    """
+    raise(PE.PyANotImplemented("IFitterBase: fit method needs to be implemented"))
+  
+  def _digestkwargs(self, kwargs):
+    """
+      Check validity of keywords.
+      
+      Tests whether all given keywords are included in the list
+      of "allowed" keywords (attribute _allowedKWs).
+      
+      Parameters
+      ----------
+      kwargs : dictionary
+          Keyword arguments handed to the minimizer.
+    """
+    if not hasattr(self, "_allowedKWs"):
+      raise(PE.PyANotImplemented("No _allowedKWs attribute. Must be set to use '_digestkwargs'.", \
+                                 solution="Specify _allowedKWs, e.g., in constructor."))
+    for k in kwargs.keys():
+      if not k in self._allowedKWs:
+        raise(PE.PyAValError("Keyword " + k + " not allowed in algorithm: " + self.name,
+                             solution="Allowed keywords: " + ', '.join(self._allowedKWs), \
+                             where=self.name))
+  
+  def getObjFuncValue(self):
+    """
+      Access value of objective function.
+      
+      Returns
+      -------
+      value : float
+          Value of objective function.
+    """
+    return self._objfval
+  
+  def __call__(self, *args, **kwargs):
+    """
+      Wrapper around the actual fit method.
+    """
+    return self.fit(*args, **kwargs)
+
+
+class ScipyFMIN(IFitterBase):
+  """
+    Wrapper around scipy.optimize.fmin.
+  """
+  
+  def __init__(self, *args, **kwargs):
+    IFitterBase.__init__(self)
+    self._allowedKWs = ["xtol", "ftol", "maxiter", "maxfun", "disp", "retall", "callback"]
+    self.name = "scipy.optimize.fmin"
+    
+  def fit(self, miniFunc, x0, *fminpars, **fminargs):
+    """
+      Wrapper around scipy.optimize.fmin.
+    """
+    self._digestkwargs(fminargs)
+    self._result = sco.fmin(miniFunc, x0, *fminpars, full_output=True, **fminargs)
+    self._objfval = self._result[1]
+    return self._result[0], self._result[1]
+  
+
+class FuFNM(IFitterBase):
+
+  def __init__(self, *args, **kwargs):
+    IFitterBase.__init__(self)
+    self._allowedKWs = ["initDelta", "maxIter", "callback"]
+    self.name = "funcFit NM65"
+    self._obj = args[0]
+    self._nm = NelderMead(**kwargs)
+  
+  def fit(self, miniFunc, x0, *fminpars, **fminargs):
+    """
+      Wrapper around funcFit's NelderMead implementation.
+    """
+    self._digestkwargs(fminargs)
+    self._bestFit = self._nm.fit(self._obj, self._obj._fufDS, self._obj.miniFunc, **fminargs)
+    self._bestFitVals = self._obj.pars.getFreeParams()
+    self._objfval = self._obj.miniFunc(self._bestFitVals)
+    return self._bestFitVals, self._objfval
+
+FuFNM.__doc__ = NelderMead.__doc__
+
+
+class FuFPrior:
+  """
+    A number of priors.
+    
+    Properly initialized, an object of type "FuFPrior"
+    is callable. On call, it expects a dictionary with
+    the names and values of the parameters as first
+    argument and the name of the parameter under consideration
+    as second argument. The return value should be the
+    (natural) logarithm of the associated prior probability
+    distribution.
+    
+    Parameters
+    ----------
+    lnp : string, {uniform, jeffreyPS, gaussian, limuniform}
+        uniform : improper uniform prior. limuniform: proper
+        uniform prior. 'lower' and 'upper' define the lower and
+        upper bounds of the interval.
+        jeffreyPS: Jeffreys
+        prior for a Poisson scaling parameter. gaussian: A
+        Gaussian prior. The keyswords 'mu' and 'sig' must be
+        specified to define the mean and standard deviation of
+        the Gaussian.
+  """
+  
+  def _uniform(self, **kwargs):
+    def uniform(ps, n, **rest):
+      return 0.0
+    return uniform
+  
+  def _uniformLimit(self, **kwargs):
+    if kwargs["upper"] < kwargs["lower"]:
+      raise(PE.PyAValError("upper needs to be larger than lower", \
+                           where="FuFPrior (limited uniform distribution)", \
+                           solution="Adapt upper and lower."))
+    p = np.log(1.0/(kwargs["upper"] - kwargs["lower"]))
+    def unilimit(ps, n, **rest):
+      if (ps[n] >= kwargs["lower"]) and (ps[n] <= kwargs["upper"]):
+        return p
+      else:
+        return -np.Inf
+    return unilimit
+  
+  def _jeffreyPoissonScale(self, **kwargs):
+    def jps(ps, n, **rest):
+      return -0.5 * np.log(ps[n])
+    return jps
+  
+  def _gaussian(self, **kwargs):
+    r = -0.5*np.log(2.0*np.pi*kwargs["sig"]**2)
+    def gaussianPrior(ps, n, **rest):
+      return r - (ps[n] - kwargs["mu"])**2 / (2.0*kwargs["sig"]**2)
+    return gaussianPrior
+  
+  def __init__(self, lnp, **kwargs):
+    if isinstance(lnp, basestring):
+      if lnp == "uniform":
+        self.__call__ = self._uniform(**kwargs)
+      elif lnp == "limuniform":
+        self.__call__ = self._uniformLimit(**kwargs)
+      elif lnp == "jeffreyPS":
+        self.__call__ = self._jeffreyPoissonScale(**kwargs)
+      elif lnp == "gaussian":
+        self.__call__ = self._gaussian(**kwargs)
+      else:
+        raise(PE.PyAValError("No prior defined for " + str(lnp), \
+                             where="FuFPrior", \
+                             solution="Use either of {uniform, jeffreyPS, gaussian}"))
+        
+
+
 class OneDFit(_OndeDFitParBase, _PyMCSampler):
   """
     The base class for fitting objects.
     
     Parameters
     ----------
     parList : list of strings
@@ -776,35 +961,35 @@
     for k in coDat.iterkeys():
       # Loop over all available root names
       if len(coDat[k]) == 1:
         # Only a single component with that root, no problem, no renaming
         continue
       elif len(coDat[k]) >= 2:
         # Get all component counters pertaining to that root
-        cs = numpy.array([c.naming.getComponentCounter() for c in coDat[k]])
+        cs = np.array([c.naming.getComponentCounter() for c in coDat[k]])
         # What is the current maximum
-        highest = numpy.max(cs)
+        highest = np.max(cs)
         # Check whether one or more counters are zero;
         # if so, increase the number and set it to "highest + 1".
         for c in coDat[k]:
           if c.naming.getComponentCounter() == 0:
             c.naming.setComponentCounter(highest + 1)
             highest += 1
         # Now re-check whether counters are unique 
         while True:
-          cs = numpy.array([c.naming.getComponentCounter() for c in coDat[k]])
-          u = numpy.unique(cs)
+          cs = np.array([c.naming.getComponentCounter() for c in coDat[k]])
+          u = np.unique(cs)
           if len(u) == len(cs):
             # All counters are unique, work is finished
             break
           # Set lowest counter
           again = False
           for c in coDat[k]:
             # Loop over components
-            if len(numpy.where(cs == c.naming.getComponentCounter())[0]) > 1:
+            if len(np.where(cs == c.naming.getComponentCounter())[0]) > 1:
               # If there are nonunique counters, make them unique and retry
               c.naming.setComponentCounter(highest + 1)
               highest += 1
               again = True
               break
           if not again:
             break
@@ -907,31 +1092,31 @@
     result._operator = '**'
     return result
   
   def __sqrDiff(self):
     @MiniFunc(self)
     def miniSqrDiff(odf, P):
       # Calculate squared difference
-      chi = numpy.sum((self._fufDS.y - self.model)**2)
+      chi = np.sum((self._fufDS.y - self.model)**2)
       return chi
     return miniSqrDiff   
   
   def __chiSqr(self):
     @MiniFunc(self)
     def miniChiSqr(odf, P):
       # Calculate chi^2 and apply penalty if boundaries are violated.
-      chi = numpy.sum(((self._fufDS.y - self.model)/self._fufDS.yerr)**2)
+      chi = np.sum(((self._fufDS.y - self.model)/self._fufDS.yerr)**2)
       return chi
     return miniChiSqr
 
   def __cash79(self):
     @MiniFunc(self)
     def miniCash79(odf, P):
       # Calculate Cash statistics according to Cash 1979 (ApJ 228, 939)
-      c = -2.0 * numpy.sum(self._fufDS.y * numpy.log(self.model) - self.model)
+      c = -2.0 * np.sum(self._fufDS.y * np.log(self.model) - self.model)
       return c
     return miniCash79
 
   def setRootName(self, root, rename=False):
     """
       Define the root name of the model.
       
@@ -1318,112 +1503,401 @@
 
     if not quiet: self.MCMC.isample(**sampleArgs)
     else: self.MCMC.sample(**sampleArgs)
     self.basicStats = self.MCMC.stats()
     if not quiet: self._basicStatMCMCOutput(self.basicStats)
     
     # Setting values to ``best fit values'' (lowest deviance)
-    mindex = numpy.argmin(self.MCMC.trace("deviance")[:])
+    mindex = np.argmin(self.MCMC.trace("deviance")[:])
     if not quiet:
       print "Searching for lowest-deviance solution."
       print "  Index of lowest-deviance solution: ", mindex
     for par in pymcPars.iterkeys():
       # Weird way of accessing element with index "mindex";
       # prevents slicing/indexing problem in pymc-Trace
       self[par] = (self.MCMC.trace(par)[mindex:mindex+1])[0]
       if not quiet:
         print "  Parameter: ", par, ", value: ", self[par]
     self.updateModel() 
     self.MCMC.db.close()
     
-  def fit(self, x, y, yerr=None, X0=None, minAlgo=None, miniFunc=None, printTime=False, *fminPars, **fminArgs):
+  def fitEMCEE(self, x=None, y=None, yerr=None, nwalker=None, priors=None, pots=None, scales=None, \
+               sampleArgs=None, dbfile="chain.emcee", ps=None, emcp=None, toMD=True):
+    """
+      MCMC samplign using emcee package.
+      
+      Sample from the posterior probability distribution using the emcee
+      package. By default the likelihood is calculated as -0.5 times the
+      model chi-square value.
+      
+      The emcee sampler can be accessed via the `emceeSampler` attribute,
+      which may be used to continue or manipulate sampling.
+      
+      Parameters
+      ----------
+      nwalker : int, optional
+          The number of walker to be used. By default, two times the
+          number of free parameters is used.
+      scales : dictionary, optional
+          The scales argument can be used to control the initial distribution
+          of the walkers. By default, all walkers are distributed around the
+          location given by the current state of the object, i.e., the current
+          parameter values. In each direction, the walker are randomly distributed
+          with a Gaussian distribution, whose default standard deviation is one.
+          The scales argument can be used to control the width of Gaussians used
+          to distribute the walkers.
+      sampleArgs : dictionary, optional
+          Number controling the sampling process. Use 'burn' (int) to specify
+          the number of burn-in iterations (default is 0). Via 'iters' (int)
+          the numbers of iterations after the burn-in can be specified (default 1000).
+          The 'process' (int) key can be used to control the number of iterations after
+          which the progress bar is updated (default is iters/100). Note that the
+          'progressbar' package must be installed to get a progress bar. Otherwise
+          more mundane print statements will be used.  
+      priors : dictionary, optional
+          For each parameter, a primary can be specified. In particular, a
+          prior is a callable, which is called with two arguments: first, a
+          dictionary mapping the names of the free parameters to their
+          current values, and second, a string specifying the name of the
+          parameter for which the prior is to apply. The return value must be
+          the logarithmic prior probability (natural logarithm). A number of default
+          priors are available in the form of the `FuFPrior` class. By
+          default, a uniform (improper) prior is used for all parameter, for
+          which no other prior was specified.
+      pots : list, optional
+          A list of 'potentials'. A potential is a function, which is called using
+          a dictionary holding the current value for all parameters and returns
+          the logarithm of the associated probability. Potentials may, e.g., be
+          used to implement certain relations between parameter values not otherwise
+          accounted for. 
+      dbfile : string, optional
+          The result of the sampling, i.e., the chain(s), the corresponding
+          values of the posterior, and the names of the free parameters are
+          saved to the specified file (by default 'chain.emcee' is used).
+          The traces stored there can be analyzed using the 'TraceAnalysis'
+          class. Set this parameter to 'None' to avoid saving the results.
+      ps : tuple, optional
+          A tuple holding the current position and state of the sampler. This
+          tuple is returned by this method. The `ps` argument can be used
+          to continue sampling from the last state. Note that no burn-in will
+          ne carried out and the other arguments should be given as previously
+          to continue sampling successfully. 
+      emcp : dictionary, optional
+          Extra arguemnts handed to `EnsembleSampler` object.
+      toMD : boolean, optional
+          If True (default), the object is set to the lowest-deviance solution
+          after sampling. Otherwise, it remains in a random state.
+    """
+  
+    if not ic.check["emcee"]:
+      raise(PE.PyARequiredImport("Could not import the 'emcee' package.", \
+                                 solution="Please install 'emcee'."))
+
+    if (not x is None) and (not y is None) and (not yerr is None):
+      # Assign attributes and check x, y, and yerr.
+      self._fufDS = FufDS(x, y, yerr)
+    elif (not x is None) and (not y is None) and (yerr is None):
+      raise(PE.PyAValError("An error on the y values is required.", \
+                           where="fitEMCEE", \
+                           solution="Please specify 'yerr'"))
+    if self._fufDS is None:
+      raise(PE.PyAValError("Please specify the data completely.", \
+                           where="fitEMCEE", \
+                           solution="Specify x, y, and yerr."))
+    
+    if not self._fufDS.xyyerrDefined():
+      raise(PE.PyAValError("Please specify the data completely. Either of x, y, and/or yerr are missing.", \
+                           where="fitEMCEE", \
+                           solution="Specify x, y, and yerr.")) 
+
+
+    # Names and values of free parameters
+    fps = self.freeParameters()
+    # Names of the free parameters in specific order
+    fpns = self.freeParamNames()
+    # Number of dimensions 
+    ndims = len(fps)
+    
+    if ndims == 0:
+      raise(PE.PyAValError("At least one free parameter is required for sampling.", \
+                           where="fitEMCEE", \
+                           solution="Use 'thaw' to free same parameters."))
+    
+    if not dbfile is None:
+      if re.match(".*\.emcee$", dbfile) is None:
+        PE.warn(PE.PyAValError("The db filename (" + str(dbfile) + ") does not end in .emcee. TraceAnalysis will not recognize it as an emcee trace file.", \
+                               solution="Use a filename of the form *.emcee"))
+    
+    # Number of walkers
+    if nwalker is None:
+      self.nwalker = ndims * 2
+    else:
+      self.nwalker = nwalker
+      
+    if self.nwalker < ndims * 2:
+      raise(PE.PyAValError("The number of walkers must be at least twice the number of free parameters.", \
+                           where="fitEMCEE", \
+                           solution="Increase the number of walkers."))
+    if self.nwalker % 2 == 1:
+      raise(PE.PyAValError("The number of walkers must be even.", \
+                           where="fitEMCEE", \
+                           solution="Use an even number of walkers."))
+      
+    # Use default prior for those parameters not listed
+    if priors is None:
+      priors = {}
+    for n in fpns:
+      if not n in priors:
+        priors[n] = FuFPrior("uniform")
+    
+    # Ensure that potentials is at least an empty list
+    if pots is None:
+      pots = []
+    
+    # Chi square calucaltor
+    chisqr = self.__chiSqr()
+    
+    def likeli(names, vals):
+      # The likelihood function
+      likeli = -0.5 * chisqr(vals)
+      return likeli
+    
+    def lnpostdf(values):
+      # Parameter-Value dictionary
+      ps = dict(zip(fpns, values))
+      # Likelihood
+      pdf = likeli(fpns, values)
+      # Add prior information
+      for name in fpns:
+        pdf += priors[name](ps, name)
+      # Add information from potentials
+      for p in pots:
+        pdf += p(ps)
+      return pdf
+    
+    # Set default values for sampleArgs
+    if sampleArgs is None:
+      sampleArgs = {}
+    if not "burn" in sampleArgs:
+      sampleArgs["burn"] = 0
+    if not "iters" in sampleArgs:
+      sampleArgs["iters"] = 1000
+    if not "progress" in sampleArgs:
+      sampleArgs["progress"] = sampleArgs["iters"] / 100
+    
+    if ps is None:
+      
+      if emcp is None:
+        emcp = {}
+    
+      # Generate the sampler
+      self.emceeSampler = emcee.EnsembleSampler(self.nwalker, ndims, lnpostdf, **emcp)
+    
+      if scales is None:
+        scales = {}
+      
+      # Generate starting values
+      pos = []
+      for _ in xrange(self.nwalker):
+        pos.append(np.zeros(ndims))
+        for i, n in enumerate(fpns):
+          if not n in scales:
+            s = 1.0
+          else:
+            s = scales[n]
+          pos[-1][i] = np.random.normal(fps[n], s)
+      
+      # Default value for state
+      state = None
+      
+      if sampleArgs["burn"] > 0:
+        # Run burn-in
+        pos, prob, state = self.emceeSampler.run_mcmc(pos, sampleArgs["burn"])
+        # Reset the chain to remove the burn-in samples.
+        self.emceeSampler.reset()
+    
+    else:
+      # Assign position and state from previous run
+      pos, state = ps
+
+    if (not sampleArgs["progress"] is None) and ic.check["progressbar"]:
+      widgets = ['EMCEE progress: ', progressbar.Percentage(), ' ', progressbar.Bar(marker=progressbar.RotatingMarker()),
+           ' ', progressbar.ETA()]
+      pbar = progressbar.ProgressBar(widgets=widgets, maxval=sampleArgs["iters"]).start()
+    
+    n = 0
+    for pos, prob, state in self.emceeSampler.sample(pos, rstate0=state, iterations=sampleArgs["iters"], thin=1, storechain=True):
+      n += 1
+      if (not sampleArgs["progress"] is None) and (n % sampleArgs["progress"] == 0):
+        if ic.check["progressbar"]:
+          pbar.update(n)
+        else:
+          print "EMCEE: Reached iteration ", n, " of ", sampleArgs["iters"]
+    
+    # Save the chain to a file
+    if not dbfile is None:
+      np.savez_compressed(open(dbfile, 'w'), chain=self.emceeSampler.chain, lnp=self.emceeSampler.lnprobability, \
+                             pnames=np.array(fpns, dtype=np.string_))
+    
+    if toMD:
+      # Set to lowest-deviance solution
+      indimin = np.argmin(self.emceeSampler.lnprobability)
+      for i, p in enumerate(self.freeParamNames()):
+        self[p] = self.emceeSampler.flatchain[indimin, i] 
+    
+    return pos, state
+    
+    
+  def _resolveMinAlgo(self, minAlgo, default=None, mAA=None):
+    """
+      Resolve minimization algorithm (minAlgo).
+      
+      Parameters
+      ----------
+      minAlgo : callable, string, or None
+          If None, the default will be used. If it is
+          a callable, it will be assumed to be a valid
+          implementation of a minimization algorithm. If
+          it is a string, the function will try to resolve
+          it.
+      default : callable, string, or None
+          The algorithm used, if minAlgo itself is None.
+      mAA : dictionary, optional
+          Keyword arguments given to constructor of minAlgo.
+      
+      Returns
+      -------
+      minAlgo : callable
+          An instance of the minimization algorithm.
+    """
+    if minAlgo is None:
+      # If not specified use default.
+      minAlgo = default
+    
+    if minAlgo is None:
+      # This should not happen. Default must be specified.
+      raise(PE.PyAValError("No minimization algorithm specified.",\
+                           solution="Use, e.g., minAlgo='spfmin' or minAlgo='fufnm'"))
+    
+    if hasattr(minAlgo, '__call__'):
+      # It is a callable. Just assume that it can be used
+      return minAlgo
+    
+    # Check keyword arguments to be handed to constructor
+    # of the fitter 
+    if mAA is None:
+      maa = {}
+    else:
+      maa = mAA
+    
+    if isinstance(minAlgo, basestring):
+      if minAlgo == "fufnm":
+        return FuFNM(self, **maa)
+      elif minAlgo == "spfmin":
+        # scipy.optimize.fmin
+        global _scoImport
+        if not _scoImport:
+          raise(PE.PyARequiredImport("SciPy.optimize could not be imported.", \
+                                     solution=["Install SciPy (see www.scipy.org/).",
+                                               "Use funcFit's Nelder-Mead simplex implementation (minAlgo='fufnm')"]))
+        return ScipyFMIN(**maa)
+      else:
+        raise(PE.PyAValError("Unknown string identifier for minimization algorithm: " + minAlgo, \
+                             solution="Use, e.g., minAlgo='spfmin' or minAlgo='fufnm'"))
+    
+    else:
+      raise(PE.PyAValError("Could not resolve 'minAlgo'.", \
+                           where="funcFit::OneDFit", \
+                           solution="Use, e.g., minAlgo='spfmin' or minAlgo='fufnm'"))
+  
+  def fit(self, x, y, yerr=None, X0=None, minAlgo=None, mAA=None, miniFunc=None, printTime=False, *fminPars, **fminArgs):
     """
       Carries out a fit.
       
-      In principle, any fit algorithm can be used. If none is specified,
-      the default is scipy.optimize.fmin (Nelder-Mead Simplex).
-      Another choice could, for instance, be scipy.optimize.fmin_powell.
-      After the fit, the return value of the fitting method
-      is stored in the class property `fitResult` and the `model`
-      property is set to the best fit.
+      Uses an internal optimizer to find the best-fit parameters.
+      By default, the method uses the scipy.optimize.fmin algorithm
+      (Nelder-Mead Simplex) to find the best-fit parameters. After the
+      fit, the parameter values are set to the best-fit values.
       
       Parameters
       ----------
       x,y : arrays
           Specify the abscissa and ordinate values of the data points.
       yerr : array, optional
           Error of data values.
       X0 : list, optional
           The initial guess. If not provided, it will be assumed
           that the current parameter values already contains
           the initial guess.
-      minAlgo : callable,
-          The minimization algorithm. Default is scipy.optimize.fmin;
-          other algorithms from scipy may be chosen. Alternatively,
-          any callable object taking the function to minimize as
-          the first, the vector of starting
-          values as the second, and a full_output flag as
-          arguments can be used.
+      minAlgo : callable or string, optional
+          The minimization algorithm. If not specified, scipy's 'fmin'
+          implementation will be used. If a callable is given, it
+          must adhere to funcFit's internal optimizer model.
+          Valid strings are:
+            - 'spfmin' : scipy.optimize.fmin
+            - 'fufnm' : funcFit's implementation of the Nelder-Mead simplex algorithm.
+      mAA : dictionary, optional
+          Keyword arguments handed to the constructor of minAlgo, i.e.,
+          minAlgo Arguments (mAA). Valid keywords depend on the choice
+          of the fit algorithm.
       fminArgs : dict 
           Keywords passed to the minimization method
-          (e.g., `xtol` or `ftol` for scipy.optimize.fmin).
-      printTime: boolean, optional
-          If True, the number of seconds needed to carry out the fit
-          is printed. Default is False.     
+          (e.g., `xtol` or `ftol` for scipy.optimize.fmin).  
       fminPars :
           Non-keyword arguments passed to the  minimization method
           (e.g., fprime in scipy.optimize.fmin_ncg).
       miniFunc : None, string {"chisqr", "cash79"}, or function
           Function to be minimized. If None or "chisqr" is given,
           chi-square will be minimized. If "cash79" is given, the
           Cash statistics (Cash 1979, ApJ 228, 939, Eq. 5) will
           be minimized. If a function is specified, that, potentially
           user defined, function will be used to calculated the
           statistics, which will be minimized.
+      printTime: boolean, optional
+          If True, the number of seconds needed to carry out the fit
+          is printed. Default is False. At any rate, the time in seconds
+          is stored in the "requiredTime" attribute.
     """
     # Assign attributes and check x, y, and yerr.
     if (x is not None) and (y is not None):
       # This is a not-so-beautiful way to allow
       # calls from within without redefining the
       # data object. This way, the API can remain
       # unchanged.
       self._fufDS = FufDS(x, y, yerr)
     # Choose minimization algorithm
-    if minAlgo is None:
-      # If not specified use default.
-      # Check whether it is available...
-      global _scoImport
-      if not _scoImport:
-        raise(PE.PyARequiredImport("SciPy.optimize could not be imported.", solution="Install SciPy (see www.scipy.org/)."))
-      self.minAlgo = sco.fmin
-    else:
-      self.minAlgo = minAlgo
+    self.mAA = copy.copy(mAA)
+    self.minAlgo = self._resolveMinAlgo(minAlgo, default="spfmin", mAA=mAA)
+    
     # Determine function to be minimized
     if (miniFunc is None) and (yerr is not None):
       miniFunc = "chisqr"
     elif (miniFunc is None) and (yerr is None):
       miniFunc = "sqrdiff"
     self.setObjectiveFunction(miniFunc)
     # Assign initial guess if necessary
     if X0 is not None:
       self.pars.setFreeParams(X0)
     # Save fminPars and fminArgs to internal variables
-    self.fminArgs = fminArgs
-    self.fminPars = fminPars
+    self.fminArgs, self.fminPars = fminArgs, fminPars
     # Carry out fit
-    if printTime:
-      fitStartTime = timestamp()
+    fitStartTime = timestamp()
+    # For "historical" reasons, the fitResult must hold a list of the
+    # best-fit parameter values as its first item and the final value of
+    # the objective function as its second item.
     self.fitResult = self.minAlgo(self.miniFunc, self.pars.getFreeParams(), *self.fminPars, \
-                             full_output=True, **self.fminArgs)
+                             **self.fminArgs)
+    # Set parameters and model to best-fit values 
     self.pars.setFreeParams(self.fitResult[0])
     self.updateModel()
     self._stepparEnabled = True
     
+    self.requiredTime = timestamp() - fitStartTime
     if printTime:
-      print "The fit took " + str(timestamp() - fitStartTime) + " seconds."
+      print "The fit took " + str(self.requiredTime) + " seconds."
   
   def __extractFunctionValue(self, fr):
     """
       Returns the function value (e.g., chi-square).
       
       Parameters
       ----------
@@ -1519,19 +1993,19 @@
         mode = 'lin'
       else:
         if not isinstance(r[3], basestring):
           raise(PE.PyAValError("If the range has 4 entries, the fourth must be a string specifying the mode.", \
                                solution="Use either 'lin' or 'log' as the fourth entry."))
         mode = r[3]
       if mode == 'lin':
-        rs.append(numpy.linspace(r[0], r[1], r[2]))
+        rs.append(np.linspace(r[0], r[1], r[2]))
       elif mode == 'log':
         # Calculate factor
-        s = numpy.power((r[1]/r[0]), 1.0/r[2])
-        rs.append( r[0] * numpy.power(s, numpy.arange(r[2])) )
+        s = np.power((r[1]/r[0]), 1.0/r[2])
+        rs.append( r[0] * np.power(s, np.arange(r[2])) )
       else:
         raise(PE.PyAValError("Unknown mode: " + str(mode), \
                              solution="Use either 'lin' or 'log'."))
     # Save state of object
     saveObj = self.saveState()
     saveFitResult = self.fitResult
     saveModel = self.model.copy()
@@ -1541,14 +2015,15 @@
     result = []
     # Loop over the axes
     nli = pyaC.NestedLoop(map(len, rs))
     for index in nli:
       for i, p in enumerate(pars):
         self[p] = rs[i][index[i]]
       # Fit using previous setting
+      # Note that mAA is dispensable, because self.minAlgo will be a callable.
       self.fit(None, None, yerr=None, minAlgo=self.minAlgo, miniFunc=self.miniFunc, \
                *self.fminPars, **self.fminArgs)
       # Build up result
       ppr = []
       for par in pars:
         ppr.append(self[par])
       try:
@@ -1656,14 +2131,15 @@
     iters = 2
     self.freeze(par)
     # Find lower limit
     # Calculate first step
     x0 = parmin
     y0 = cvalmin
     self[par] = parmin - scale
+    # Note that mAA is dispensable, because self.minAlgo will be a callable.
     self.fit(None, None, yerr=None, minAlgo=self.minAlgo, miniFunc=self.miniFunc)
     x1 = self[par]
     y1 = self.__extractFunctionValue(self.fitResult)
     while True:
       if y1 < cvalmin:
         PE.warn(PE.PyAParameterConflict("Found a new minimum for the objective function during error search."))
       iters += 1
@@ -1704,15 +2180,16 @@
     lowerLimit = self[par]
     lowerOF = y1
     
     # Find upper limit
     x0 = parmin
     y0 = cvalmin
     self[par] = parmin + scale
-    self.fit(None, None, yerr=None, minAlgo=self.minAlgo, miniFunc=self.miniFunc)
+    self.fit(None, None, yerr=None, minAlgo=self.minAlgo, miniFunc=self.miniFunc, \
+            *self.fminPars, **self.fminArgs)
     x1 = self[par]
     y1 = self.__extractFunctionValue(self.fitResult)
     while True:
       iters += 1
       if iters > maxiter:
         PE.warn(PE.PyAValError("Maximum number if iterations (" + str(maxiter) + ") exceeded. Returning None.", \
                 solution=["Increase maximum number of iterations via `maxiter` flag.", \
```

### Comparing `PyAstronomy-0.8.1/src/funcFit/polyModel.py` & `PyAstronomy-0.9.0/src/funcFit/polyModel.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/sinexp1d.py` & `PyAstronomy-0.9.0/src/funcFit/sinexp1d.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/cauchyLorentz1d.py` & `PyAstronomy-0.9.0/src/funcFit/cauchyLorentz1d.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/nameIdentBase.py` & `PyAstronomy-0.9.0/src/funcFit/nameIdentBase.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/coordinateGrid.py` & `PyAstronomy-0.9.0/src/funcFit/coordinateGrid.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/extFitter.py` & `PyAstronomy-0.9.0/src/funcFit/extFitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,23 @@
     The default stop criterion is the one used by NM 1965. In
     particular, the value
     
     .. math:: \\sqrt{\\sum (\\bar{y}-y_i) / n}
     
     is calculated. If it falls below the limit defined by the
     attribute `nmCritLim`, the iteration stops.
-   
+    
+    Parameters
+    ----------
+    abg : tuple of three floats, optional
+        Values for alpha, beta, and gamma.
+    isw : float, optional
+        Initial step width for simplex.
+    critlim : float, optional
+        Critical limit for stopping criterion.
     
     Attributes
     ----------
     alpha, beta, gamma : float
         The reflection-, expansion-, and contraction-coefficients.
         The default values (after NM 1965) are 1.0, 0.5, and 2.0.
         These coefficients control the modification of the simplex.
@@ -31,21 +39,21 @@
         the starting value. The default is 0.05.
     nmCritLim : float
         Critical value for the NM 1965 stopping criterion. The
         default is 1e-8.
         
   """
   
-  def __init__(self):
+  def __init__(self, abg=(1.0, 0.5, 2.0), isw=0.05, critlim=1e-8):
     # Best guesses after NM 1965
-    self.alpha, self.beta, self.gamma = (1.0, 0.5, 2.0)
+    self.alpha, self.beta, self.gamma = abg
     # Step-width factor for initial simplex (if not specified otherwise)
-    self.initialStepWidthFac = 0.05
+    self.initialStepWidthFac = isw
     # Critical limit for the NM 1965 stopping criterion
-    self.nmCritLim = 1e-8
+    self.nmCritLim = critlim
     # Stopping criterion
     self._stopCrit = self._stopNM1965
   
   def _initSimplex(self, m, initDelta):
     """
       Define the initial simplex.
       
@@ -66,19 +74,19 @@
     self._yi[0] = m.miniFunc(self._simplex[0,::])
     for i, p in enumerate(self._fpns):
       self._simplex[i+1,::] = self._simplex[0,::].copy()
       if (initDelta is not None) and (p in initDelta):
         self._simplex[i+1, i] += initDelta[p]
       else:
         if self._simplex[0,i] == 0.0:
-          raise(PE.PyAValError("The start value of the parameter '" + p + "' is 0.0. This will lead" + \
-                         " to an appropriate simplex.", \
-                          solution="Specify an initial step via the `initDelta` parameter.\n" + \
-                          "The size of the step should reflect the 'scale' of the problem."))
-        self._simplex[i+1, i] += self._simplex[0,i] * self.initialStepWidthFac
+          # Construct simplex by adding initial step width
+          self._simplex[i+1, i] = self._simplex[0,i] + self.initialStepWidthFac
+        else:
+          # Construct simplex by adding fraction of the value
+          self._simplex[i+1, i] += self._simplex[0,i] * self.initialStepWidthFac
       self._yi[i+1] = m.miniFunc(self._simplex[i+1,::])
     
   def _step(self, m):
     """
       Proceed one step of the simplex algorithm.
     """
     # Indices with lowest and highest objective function value
```

### Comparing `PyAstronomy-0.8.1/src/funcFit/params.py` & `PyAstronomy-0.9.0/src/funcFit/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,15 +649,16 @@
       raise(PE.PyAValError("The dependent variable ("+parName1+") cannot be in the list of independent variables."))
     # Use equal function if None is specified.
     if func is None: func = equal
     # Append to 'relations' list
     for p in pars:
       # If parameter 'p' is set, redefine 'parName1' using function 'func' with parameters 'pars'
       self.relations[p].append( [parName1, func, pars] )
-    # Update parameter values
+    # Update parameter values (on re-assigned the values of the independent
+    # parameters, the value of the dependent parameter will be updated)
     for p in pars:
       self.assignValue({p:self.__params[p]})
     self.isFree[parName1] = False
 
   def getPenalty(self, penaltyFact=1e20):
     """
       Get applied penalty for current parameter set.
```

### Comparing `PyAstronomy-0.8.1/src/funcFit/__init__.py` & `PyAstronomy-0.9.0/src/funcFit/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 import sys
 
 # Check Python version
 _majV, _minV = sys.version_info[0:2]
 if _minV < 7:
   PE.warn("funcFit needs 2.7.x or greater (but not Python 3.x). See documentation (Prerequisites) for explanation.")
   
-ic = ImportCheck(["numpy", "scipy", "pymc", "matplotlib", "pyfits"])
+ic = ImportCheck(["numpy", "scipy", "pymc", "matplotlib", "matplotlib.pylab", "pyfits", "emcee", "progressbar"])
 
 # Get out if numpy not present
 if not ic.check["numpy"]:
   raise(PE.PyARequiredImport("Numpy cannot be imported.", solution="Install numpy (see http://numpy.scipy.org/, you probably should also install SciPy).", \
                              addInfo="The numpy package provides array support for Python and is indispensable in many scientific applications."))
 
 # Check whether fitting modules can be imported
 _scoImport = ic.check["scipy"]
 _pymcImport = ic.check["pymc"]
 _mplImport = ic.check["matplotlib"]
 
-if _pymcImport: from PyAstronomy.funcFit.utils import *
+from PyAstronomy.funcFit.utils import *
 from modelRebin import turnIntoRebin, _ModelRebinDocu
 from onedfit import *
 from gauss1d import *
 from gauss2d import *
 from params import *
 from sinexp1d import *
 from polyModel import *
@@ -53,11 +53,24 @@
   if not _scoImport:
     print "  The minimization algorithms from SciPy cannot be used."
     print "  Install SciPy to make them available (see http://www.scipy.org/)."
   print "Is pymc available? ", __question(_pymcImport)
   if not _pymcImport:
     print "  No Markov-Chain Monte-Carlo sampling via pymc will be possible."
     print "  Install pymc to enable it (see http://code.google.com/p/pymc/)."
+  else:
+    import pymc
+    print "  pymc is available in version: ", pymc.__version__
+    try:
+      majorversion = int(pymc.__version__.split('.')[0])
+      if majorversion > 2:
+        print "  NOTE: Sampling is only supported with pymc 2.x (not 3.x)!"
+    except:
+      print "  Could not parse pymc version string..."
+  print "Is emcee available? ", __question(ic.check["emcee"])
+  if not ic.check["emcee"]:
+    print "  No Markov-Chain Monte-Carlo sampling via emcee will be possible."
+    print "  Install emcee to enable it (see http://dan.iel.fm/emcee/current/)."
 
 __all__ = ["cauchyLorentz1d", "gauss1d", "modelRebin", "onedfit", "params", "voigt1d", "sinexp1d", "polyModel",
            "BoltzmannSAS", "PyAAnneal"]
```

### Comparing `PyAstronomy-0.8.1/src/funcFit/gauss1d.py` & `PyAstronomy-0.9.0/src/funcFit/gauss1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class GaussFit1d(OneDFit):
   """
     Implements a one dimensional Gaussian.
     
     The functional form is:
     
-    .. math:: \\frac{A}{2\\pi\\sigma^2}e^{-(x-\\mu)^2/(2\\sigma^2)} + x \\times lin + off
+    .. math:: \\frac{A}{\\sqrt{2\\pi\\sigma^2}}e^{-(x-\\mu)^2/(2\\sigma^2)} + x \\times lin + off
     
     Here, `lin` and `off` denote the linear and the offset term.
     
     *Fit parameters*:
      - `A` - Amplitude (the area of the Gaussian)
      - `mu` - Center of the Gaussian
      - `sig` - Standard deviation
```

### Comparing `PyAstronomy-0.8.1/src/funcFit/gauss2d.py` & `PyAstronomy-0.9.0/src/funcFit/gauss2d.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/funcFitSanity.py` & `PyAstronomy-0.9.0/src/funcFit/funcFitSanity.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/syncFit.py` & `PyAstronomy-0.9.0/src/funcFit/syncFit.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/circle2d.py` & `PyAstronomy-0.9.0/src/funcFit/circle2d.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/moduleSanity.py` & `PyAstronomy-0.9.0/src/funcFit/moduleSanity.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/anneal.py` & `PyAstronomy-0.9.0/src/funcFit/anneal.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/funcFit/voigt1d.py` & `PyAstronomy-0.9.0/src/funcFit/voigt1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,17 @@
       ----------
       x : array
           Specifies the points at which to evaluate the model.
     """
     try:
         
         
-      z = ((x-self["mu"]) + (1.j)*self["al"])/(numpy.sqrt(2.0) * self["ad"])
+      z = ((x-self["mu"]) + (1.j)*abs(self["al"]))/(numpy.sqrt(2.0) * abs(self["ad"]))
       y = self["A"] * numpy.real(sps.wofz(z)) 
-      y /= (self["ad"] * numpy.sqrt(2.0*numpy.pi))
+      y /= (abs(self["ad"]) * numpy.sqrt(2.0*numpy.pi))
       y += x * self["lin"] + self["off"]
   
       y[numpy.where(numpy.isnan(y))] = 0.0
     except FloatingPointError, fpe:
       raise(PE.PyAFloatingPointError("The following floating point error occurred:\n  " + str(fpe) + "\n" +
                                      "Current Parameter values:\n"+str(self.parameters()),
                                      solution=["Try to rescale/shift your abscissa. For instance, put" +
```

### Comparing `PyAstronomy-0.8.1/src/funcFit/utils/bayesFactors.py` & `PyAstronomy-0.9.0/src/funcFit/utils/bayesFactors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 import numpy
+from PyAstronomy.funcFit.utils import ic
+from PyAstronomy.pyaC import pyaErrors as PE
 
+try:
+  import pymc
+except ImportError:
+  pass
+  
 def bayesFactors(model1, model2):
   """
     Computes the Bayes factor for two competing models.
     
     The computation is based on Newton & Raftery 1994 (Eq. 13).
     
     Parameters
@@ -17,15 +24,17 @@
     -------
     BF : float
         The Bayes factor BF (neither log10(BF) nor ln(BF)).
         Note that a small value means that the first model
         is favored, i.e., BF=p(M2)/p(M1).
     
   """
-  import pymc
+  if not ic.check["pymc"]:
+    raise(PE.PyARequiredImport("pymc is required to evaluate the bayesFactor", \
+                               solution="Install pymc"))
   
   logp1 = model1["deviance"]/(-2.)
   logp2 = model2["deviance"]/(-2.)
 
   # Given a number of numbers x1, x2, ... whose logarithms are given by l_i=ln(x_i) etc.,
   # logsum calculates: ln(sum_i exp(l_i)) = ln(sum_i x_i)
   bf = numpy.exp(  pymc.flib.logsum(-logp1) - numpy.log(len(logp1))
```

### Comparing `PyAstronomy-0.8.1/src/funcFit/utils/anaMCMCTraces.py` & `PyAstronomy-0.9.0/src/funcFit/utils/anaMCMCTraces.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,127 @@
 # -*- coding: utf-8 -*-
-import pymc
-import matplotlib.pylab as mpl
 from numpy import mean, median, std
-import numpy
+import numpy as np
 import re
 import os
 from scipy.stats import spearmanr, pearsonr
 from PyAstronomy.pyaC import pyaErrors as PE
 from PyAstronomy.funcFit.utils import ic
 import itertools
 from PyAstronomy import pyaC as PC
 
+try:
+  import pymc
+except ImportError:
+  pass
+
+try:
+  import matplotlib.pylab as plt
+except ImportError:
+  pass
+
+
+
+def hpd(trace, cred):
+  """
+    Estimate the highest probability density interval.
+    
+    This function determines the shortest, continous interval
+    containing the specified fraction (cred) of steps of
+    the Markov chain. Note that multi-modal distribution
+    may require further scrutiny.
+    
+    Parameters
+    ----------
+    trace : array
+        The steps of the Markov chain.
+    cred : float
+        The probability mass to be included in the
+        interval (between 0 and 1).
+    
+    Returns
+    -------
+    start, end : float
+        The start and end points of the interval.
+  """
+  # Sort the trace steps in ascending order
+  st = np.sort(trace)
+  
+  # Number of steps in the chain
+  n = len(st)
+  # Number of steps to be included in the interval
+  nin = int(n * cred)
+  
+  # All potential intervals must be 1) continous and 2) cover
+  # the given number of trace steps. Potential start and end
+  # points of the HPD are given by
+  starts = st[0:-nin]
+  ends = st[nin:]
+  # All possible widths are
+  widths = ends - starts
+  # The density is highest in the shortest one
+  imin = np.argmin(widths)
+  return starts[imin], ends[imin]
+  
+
+def quantiles(trace, qs):
+  """
+    Get quantiles for trace.
+    
+    Parameters
+    ----------
+    trace : array
+        The steps of the Markov chain.
+    qs : list or array
+        The quantiles in *percent*.
+    
+    Returns
+    -------
+    Quantiles : dictionary
+        For each quantile, the corresponding value.
+  """
+  # Sort the trace steps in ascending order
+  st = np.sort(trace)
+  n = len(st)
+  # Convert percent into fractions 
+  qfrac = np.array(qs) / 100.0
+  # Evaluate quantiles
+  result = {}
+  for i in xrange(len(qfrac)):
+    result[qs[i]] = st[int(n*qfrac[i])]
+  return result
+
+
 class TraceAnalysis:
   """
-    This class provides a wrapper around PyMC's own
-    plotting and statistics engine.
+    Support to analyze MCMC chains.
+
+    This class provides a number of plotting methods. Note that
+    **you still need to call *show()* from pylab** to see the
+    result.
 
     Parameters
     ----------
     resource : string or pymc database object
         If string, it assumed to be the filename of the
         Markov Chain file. Otherwise, it is supposed
-        to be a pymc database object already. 
+        to be a pymc database object. If the filename is
+        of the form "*.emcee", it is assumed to be
+        a trace produced by emcee. 
     
     Attributes
     ----------
     burn : int
         Applies a burn-in. All iterations
         earlier than `burn` will be neglected.
     
     thin : int
         Applies thinning to each chain.
         Retains every `k` th sample,
-        where `k` is an integer value.
-        
-    
-    Notes
-    -----
-    The class provides a number of plotting methods, which
-    either use PyMC's capabilities or refer to matplotlib
-    directly. Note that to see the plots
-    **you still need to call *show()* from pylab**.
-    
+        where `k` is an integer value.  
   """
 
   def _parmCheck(self, parm):
     """
       Checks whether a trace is available for the given parameter.
       If not, it throws an exception.
       
@@ -63,62 +139,116 @@
       Helps to define the optimum plot size for large big-picture plots.
     """
     c=1; r=1
     while c*r<size:
       c+=1
       if c*r>=size: break
       else: r+=1
-    return [c,r]
+    return c, r
 
+  def _loadEMCEEChain(self, fn=None, burn=0):
+    """
+    """
+    if not fn is None: 
+      self._emceedat = np.load(fn)
+    self.emceepnames = list(self._emceedat["pnames"]) + ["deviance"]
+    # Dummy tracesDic
+    self.tracesDic = dict(zip( self.emceepnames, [None]*len(self.emceepnames)))
+    # Build stateDic
+    self.stateDic = {"stochastics":dict(zip( list(self._emceedat["pnames"]), [None]*len(list(self._emceedat["pnames"])))), "sampler":{}}
+    
+    # Flatten the chain
+    s = self._emceedat["chain"].shape
+    self.emceechain = np.zeros((s[0] * (s[1]-burn), s[2]+1))
+    self.emceechain[::,0:-1] = self._emceedat["chain"][::,burn:,::].reshape(s[0] * (s[1]-burn), s[2])
+    self.emceelnp = self._emceedat["lnp"][::,burn:]
+    self.emceelnp = self.emceelnp.reshape(s[0] * (s[1]-burn))
+    
+    # Incorporate "deviance" into the usual chain
+    self.emceechain[::,-1] = -2.0 * self.emceelnp
+    
+    self.stateDic["sampler"]["_iter"] = self.emceechain.shape[0]
+    self.stateDic["sampler"]["_burn"] = None
+    self.stateDic["sampler"]["_thin"] = None
+    
+    
+  def _checkPackage(self, p):
+    """
+      Check whether package is availabel and raise exception otherwise.
+      
+      Parameters
+      ----------
+      p : string
+          Name of package
+    """
+    if not ic.check[p]:
+      raise(PE.PyARequiredImport("The package '" + str(p) + "' is not currently installed.", \
+                                 solution="Please install " + str(p)))
+  
   def __init__(self, resource, db="pickle"):
     if isinstance(resource, basestring):
+      # Resource is a filename
       if not os.path.isfile(resource):
         raise(PE.PyAFileError(resource, "ne"))
       self.file = resource
+      
       if not (re.match(".*\.hdf5", resource) is None):
         db = "hdf5"
       if not (re.match(".*\.zlib", resource) is None):
         db = "hdf5"
+      if not (re.match(".*\.emcee", resource) is None):
+        db = "emcee"
+        
       if db == "pickle":
+        self.dbtype = "pymc"
+        self._checkPackage("pymc")
         self.db = pymc.database.pickle.load(resource)
+        self.stateDic = self.db.getstate()
+        self.tracesDic = self.db._traces
       elif db == "hdf5":
+        self.dbtype = "pymc"
+        self._checkPackage("pymc")
         self.db = pymc.database.hdf5.load(resource)
+        self.stateDic = self.db.getstate()
+        self.tracesDic = self.db._traces
+      elif db == "emcee":
+        self.dbtype = "emcee"
+        self._loadEMCEEChain(resource)
       else:
         raise(PE.PyAValError("Database type '"+db+"' is currently not supported."))
+      
     elif isinstance(resource, pymc.database.base.Database):
       self.db = resource
     else:
       raise(PE.PyAValError("'resource' must be a filename or a pymc database object.", where="TraceAnalysis::__init__"))
-    self.stateDic = self.db.getstate()
-    self.tracesDic = self.db._traces           # dictionary of available traces
-    self.noc = self.db.chains                  # number of chains
-    self.burn = 0                              # Use this as "post burn-in"
-    self.thin = 1                              # Use this as "post-thinner"
+    
+    # Set default burn-in and thinning 
+    self.burn = 0                             
+    self.thin = 1                         
 
   def __getitem__(self, parm):
     """
       Returns the trace for parameter `parm`.
       
       Parameters
       ----------
       parm : string
-          Variable name.
+          Name of the parameter.
       
       Returns
       -------
       trace : array
-          The trace for the parameters.
-      
-      Notes
-      -----
-      The returned trace comprises all chains possibly present in the
-      data base.
+          The trace for the parameter.
     """
     self._parmCheck(parm)
-    return self.tracesDic[parm].gettrace()[self.burn::self.thin]
+    if self.dbtype == "pymc":
+      return self.tracesDic[parm].gettrace()[self.burn::self.thin]
+    elif self.dbtype == "emcee":
+      index = self.emceepnames.index(parm)
+      return self.emceechain[self.burn::self.thin,index]
 
   def __str__(self):
     """
       Prints basic information on the current MCMC sample file.
     """
     info =  "MCMC database - Basic information:\n"
     info += "----------------------------------\n\n"
@@ -146,62 +276,60 @@
   def state(self):
     """
       Returns dictionary containing basic information
       on the sampling process.
     """
     return self.stateDic
 
-  def plotTrace(self, parm, **traceArgs):
+  def plotTrace(self, parm):
     """
       Plots the trace.
       
       Parameters
       ----------
       parm : string
           The variable name.
-      traceArgs : dict
-          Keyword arguments handed to `pymc.Matplot.trace`.
     """
     if not ic.check["matplotlib"]:
       PE.warn(PE.PyARequiredImport("To use 'plotTrace', matplotlib has to be installed.", \
                                    solution="Install matplotlib."))
       return
     self._parmCheck(parm)
-    pymc.Matplot.trace(self[parm],parm,fontmap={0.5: 10, 1:10, 2:8, 3:6, 4:5, 5:4},**traceArgs)
+    plt.plot(self[parm], 'b-', label=parm + " trace")
+    plt.legend()
 
-  def plotTraceHist(self, parm, **plotArgs):
+  def plotTraceHist(self, parm):
     """
       Plots trace and histogram (distribution).
 
       Parameters
       ----------
       parm : string
           The variable name.
-      plotArgs : dict
-          Keyword arguments handed to `pymc.Matplot.plot`.
     """
     if not ic.check["matplotlib"]:
       PE.warn(PE.PyARequiredImport("To use 'plotTraceHist', matplotlib has to be installed.", \
                                    solution="Install matplotlib."))
       return
     self._parmCheck(parm)
-    pymc.Matplot.plot(self[parm], parm, **plotArgs)
+    
+    plt.subplot(1,2,1)
+    self.plotTrace(parm)
+    plt.subplot(1,2,2)
+    self.plotHist(parm)
 
-  def plotHist(self, parsList=None, **histArgs):
+  def plotHist(self, parsList=None):
     """
       Plots distributions for a number of traces.
 
       Parameters
       ----------
       parsList : string or list of strings, optional,
           Refers to a parameter name or a list of parameter names.
           If None, all available parameters are plotted.
-      histArgs : dict, optional
-          Keyword arguments (e.g., `nbins`) passed to the
-          histogram plotter (`pymc.Matplot.histogram`).
     """
     if not ic.check["matplotlib"]:
       PE.warn(PE.PyARequiredImport("To use 'plotHists', matplotlib has to be installed.", \
                                    solution="Install matplotlib."))
       return
     if isinstance(parsList, basestring):
       parsList = [parsList]
@@ -211,19 +339,21 @@
         self._parmCheck(parm)
         tracesDic[parm] = self[parm]
     else:
       # Use all available traces
       for parm in self.availableParameters():
         tracesDic[parm] = self[parm]
 
-    ps = self.__plotsizeHelper(len(tracesDic))
+    cols, rows = self.__plotsizeHelper(len(tracesDic))
 
     for i,[pars,trace] in enumerate(tracesDic.items()):
-      pymc.Matplot.histogram(trace,pars,columns=ps[0],rows=ps[1],num=i+1,**histArgs)
-
+      if len(parsList) > 1:
+        plt.subplot(rows, cols, i+1)
+      plt.hist(trace, label=pars + " hist")
+      plt.legend()
 
   def plotDeviance(self, parsList=None):
     """
       Plots value of deviance over parameter values encountered during sampling.
 
       Parameters
       ----------
@@ -246,31 +376,28 @@
       # Use all available traces
       for parm in self.availableParameters():
         tracesDic[parm] = self[parm]
 
     ps = self.__plotsizeHelper(len(tracesDic))
 
     for i,[pars,trace] in enumerate(tracesDic.items()):
-      mpl.subplot(ps[0],ps[1],i)
-      mpl.xlabel(pars)
-      mpl.ylabel("Deviance")
-      mpl.plot(self[pars],self["deviance"],'.')
+      plt.subplot(ps[0],ps[1],i)
+      plt.xlabel(pars)
+      plt.ylabel("Deviance")
+      plt.plot(self[pars],self["deviance"],'.')
 
 
   def plotHists(self, parsList=None, **histArgs):
     print "TraceAnalysis::plotHists() - Warning! This function is deprecated. Use plotHist() instead."
     self.plotHist(parsList, **histArgs)
 
 
   def hpd(self, parm, trace=None, cred=0.95):
     """
-      Calculates highest probability density (HPD, minimum width BCI).
-      
-      interval for
-      parameter `parm` given a certain probability level 'cred'.
+      Calculates highest probability density interval (HPD, minimum width BCI).
       
       Parameters
       ----------
       parm : string
           Name of parameter
       cred : float, optional
           Credibility level. Defaults to 0.95, i.e., the 95\% HPD will
@@ -278,43 +405,43 @@
       trace : array, optional
           If a trace is given, it will be used in the calculation instead of the
           trace for `parm` stored in the class. Note that the parm will be
           ignored in this case!
       
       Returns
       -------
-        HPD : array
-            The lower and upper bound of the credibility
-            interval.
+      HPD : tuple
+          The lower and upper bound of the credibility interval.
     """
     if trace is None:
       self._parmCheck(parm)
-      return pymc.utils.hpd(self[parm], 1.-cred)
+      return hpd(self[parm], cred)
     else:
-      return pymc.utils.hpd(trace, 1.-cred)
+      return hpd(trace, cred)
 
   def quantiles(self, parm, qlist=None):
     """
-      Returns a dictionary of requested quantiles for given
-      parameter name.
+      Quantiles for given trace.
       
       Parameters
       ----------
       parm : string
           Name of parameter
       qlist : list of floats (0-100), optional
-          Specifies which quantiles shall be calculated.
+          Specifies which quantiles shall be calculated. The default is
+          2.5, 25, 50, 75, and 97.5 percent.
       
       Returns
       -------
-      Quantiles : list of quantiles
+      Quantiles : dictionary
+          For each quantile (in percent) the corresponding value.
     """
     if qlist is None:
       qlist = [2.5, 25, 50, 75, 97.5]
-    return pymc.utils.quantiles(self[parm],qlist)
+    return quantiles(self[parm],qlist)
 
   def plotCorr(self, parsList=None, **plotArgs):
     """
       Produces correlation plots.
       
       Parameters
       ----------
@@ -350,40 +477,40 @@
     if not len(tracesDic)-1 in fontmap:
       fontmap[len(tracesDic)-1] = 3
 
     k = 1
     for j in range(len(tracesDic)):
       for i in range(len(tracesDic)):
         if i>j:
-          mpl.subplot(len(tracesDic)-1,len(tracesDic)-1,k)
-          mpl.title("Pearson's R: %1.5f" % self.pearsonr(pars[j],pars[i])[0], fontsize='x-small')
-          mpl.xlabel(pars[j], fontsize='x-small')
-          mpl.ylabel(pars[i], fontsize='x-small')
-          tlabels = mpl.gca().get_xticklabels()
-          mpl.setp(tlabels, 'fontsize', fontmap[len(tracesDic)-1])
-          tlabels = mpl.gca().get_yticklabels()
-          mpl.setp(tlabels, 'fontsize', fontmap[len(tracesDic)-1])
-          mpl.plot(traces[j],traces[i],'.',**plotArgs)
+          plt.subplot(len(tracesDic)-1,len(tracesDic)-1,k)
+          plt.title("Pearson's R: %1.5f" % self.pearsonr(pars[j],pars[i])[0], fontsize='x-small')
+          plt.xlabel(pars[j], fontsize='x-small')
+          plt.ylabel(pars[i], fontsize='x-small')
+          tlabels = plt.gca().get_xticklabels()
+          plt.setp(tlabels, 'fontsize', fontmap[len(tracesDic)-1])
+          tlabels = plt.gca().get_yticklabels()
+          plt.setp(tlabels, 'fontsize', fontmap[len(tracesDic)-1])
+          plt.plot(traces[j],traces[i],'.',**plotArgs)
         if i!=j:
           k+=1
 
   def __hist2d(self,x,y,contour=False,bins=(200,200),cmap="Purples",interpolation='nearest',origin="lower", colors="k"):
     """
       Parameters
       ----------
       bins : tuple of two ints
     """
-    H, xedges, yedges = numpy.histogram2d(x, y, bins)
+    H, xedges, yedges = np.histogram2d(x, y, bins)
     extent = [xedges.min(), xedges.max(), yedges.min(), yedges.max()]
     if not contour:
-      mpl.imshow(H, extent=extent, interpolation=interpolation,origin=origin, cmap=cmap, aspect="auto")
-#      mpl.colorbar(fontsize=4)
+      plt.imshow(H, extent=extent, interpolation=interpolation,origin=origin, cmap=cmap, aspect="auto")
+#      plt.colorbar(fontsize=4)
     else:
-      CS = mpl.contour(H, extent=extent,origin=origin,colors=colors)
-      mpl.clabel(CS, inline=1, fontsize=10)
+      CS = plt.contour(H, extent=extent,origin=origin,colors=colors)
+      plt.clabel(CS, inline=1, fontsize=10)
 
   def correlationTable(self, parsList=None, coeff="pearson", noPrint=False):
     """
       Calculate and show parameter correlations
       
       Parameters
       ----------
@@ -485,23 +612,23 @@
     if not len(tracesDic)-1 in fontmap:
       fontmap[len(tracesDic)-1] = 8
 
     k = 1
     for j in range(len(tracesDic)):
       for i in range(len(tracesDic)):
         if i>j:
-          mpl.subplot(len(tracesDic)-1,len(tracesDic)-1,k)
-#          mpl.title("Pearson's R: %1.5f" % self.pearsonr(pars[j],pars[i])[0], fontsize='x-small')
-          mpl.xlabel(pars[j], fontsize=fontmap[len(tracesDic)-1])
-          mpl.ylabel(pars[i], fontsize=fontmap[len(tracesDic)-1])
-          tlabels = mpl.gca().get_xticklabels()
-          mpl.setp(tlabels, 'fontsize', fontmap[len(tracesDic)-1])
-          tlabels = mpl.gca().get_yticklabels()
-          mpl.setp(tlabels, 'fontsize', fontmap[len(tracesDic)-1])
-#          mpl.plot(traces[j],traces[i],'.',**plotArgs)
+          plt.subplot(len(tracesDic)-1,len(tracesDic)-1,k)
+#          plt.title("Pearson's R: %1.5f" % self.pearsonr(pars[j],pars[i])[0], fontsize='x-small')
+          plt.xlabel(pars[j], fontsize=fontmap[len(tracesDic)-1])
+          plt.ylabel(pars[i], fontsize=fontmap[len(tracesDic)-1])
+          tlabels = plt.gca().get_xticklabels()
+          plt.setp(tlabels, 'fontsize', fontmap[len(tracesDic)-1])
+          tlabels = plt.gca().get_yticklabels()
+          plt.setp(tlabels, 'fontsize', fontmap[len(tracesDic)-1])
+#          plt.plot(traces[j],traces[i],'.',**plotArgs)
           self.__hist2d(traces[j],traces[i],**plotArgs)
         if i!=j:
           k+=1
 
 
   def correlationMatrix(self, toScreen=True, method="pearson", parList=None, covariance=False):
     """
@@ -546,15 +673,15 @@
       # correlation coefficient has to be multiplied by the
       # standard deviation(s).
       stds = {}
       for p in parList:
         stds[p] = self.std(p)
     # Calculate the matrix
     n = len(parList)
-    matrix = numpy.zeros( (n, n) )
+    matrix = np.zeros( (n, n) )
     for i in xrange(n):
       for j in xrange(n):
         matrix[i, j] = corFunc(parList[i], parList[j])[0]
         if covariance:
           matrix[i, j] *= (stds[parList[i]] * stds[parList[j]])
 
     # Format the output
@@ -596,15 +723,15 @@
         system producing data sets that have a Pearson correlation at
         least as extreme as the one computed from these data sets.
         The p-values are not entirely reliable but are probably reasonable
         for data sets larger than 500 or so.
     """
     self._parmCheck(parm1)
     self._parmCheck(parm2)
-    return pearsonr(self.tracesDic[parm1].gettrace(), self.tracesDic[parm2].gettrace())
+    return pearsonr(self[parm1], self[parm2])
 
   def spearmanr(self, parm1, parm2):
     """
       Calculates a Spearman rank-order correlation coefficient
       and the p-value to test for non-correlation.
       
       Parameters
@@ -636,15 +763,15 @@
         an uncorrelated system producing data sets that have a Spearman
         correlation at least as extreme as the one computed from these
         data sets. The p-values are not entirely reliable but are
         probably reasonable for data sets larger than 500 or so.
     """
     self._parmCheck(parm1)
     self._parmCheck(parm2)
-    return spearmanr(self.tracesDic[parm1].gettrace(), self.tracesDic[parm2].gettrace())
+    return spearmanr(self[parm1], self[parm2])
 
   def mean(self, parm):
     """
       Calculate mean.
       
       Parameters
       ----------
@@ -691,34 +818,35 @@
     return std(self[parm])
 
   def show(self):
     """
       Call *show()* from matplotlib to bring graphs to screen.
     """
     try:
-      mpl.show()
+      plt.show()
     except Exception, e:
       PE.warn(PE.PyAUnclassifiedError("Plot could not be shown. The following exception occurred:\n" \
                                       + str(e)))
 
   def setBurn(self, burn):
     """
       Change value of "post burn-in".
       
+      In the case of an emcee trace, the "post burn-in" is
+      applied to the trace of all walkers.
+      
       Parameters
       ----------
       burn : int
           The number of samples to be neglected.
-      
-      Notes
-      -----
-      Use the "post burn-in" to neglect all sampling points before
-      the specified iteration.
     """
     self.burn = burn
+    if self.dbtype == "emcee":
+      # Apply burn-in to individual walkers
+      self._loadEMCEEChain(burn=self.burn)
   
   def setThin(self, thin):
     """
       Change value of "post thinning".
       
       Parameters
       ----------
@@ -753,15 +881,15 @@
           derived using the specified prescription.
       Lowest deviance index : int
           The index of the lowest deviance solution. Only
           returned if the prescription is 'lowestDev'
     """
     if prescription == "lowestDev":
       result = {}
-      indi = numpy.argmin(self["deviance"])
+      indi = np.argmin(self["deviance"])
       for par in self.availableParameters():
         result[par] = self[par][indi]
       return result, indi
     elif prescription == "mean":
       result = {}
       for par in self.availableParameters():
         result[par] = self.mean(par)
@@ -792,25 +920,25 @@
           If False, no output about what is done will be generated
           (default is True).
     """
     if verbose:
       print "Setting model to state: ", state
     if state == "best":
       # Setting to best state as measured by deviance
-      indi = numpy.argmin(self["deviance"])
+      indi = np.argmin(self["deviance"])
       if verbose:
         print "Lowest deviance of ", self["deviance"][indi], " at index ", indi
       for par in self.availableParameters():
         if not par in model.parameters().keys():
           continue
         model[par] = self[par][indi]
         if verbose:
           print "Setting parameter: ", par, " to value: ", model[par]
     if state == "mean":
       # Setting to "mean" state
       for par in self.availableParameters():
         if not par in model.parameters().keys():
           continue
-        model[par] = numpy.mean(self[par])
+        model[par] = np.mean(self[par])
         if verbose:
           print "Setting parameter: ", par, " to mean value: ", model[par]
```

### Comparing `PyAstronomy-0.8.1/src/funcFit/modelRebin.py` & `PyAstronomy-0.9.0/src/funcFit/modelRebin.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/__init__.py` & `PyAstronomy-0.9.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyTiming/pyPeriod/lombScargle.py` & `PyAstronomy-0.9.0/src/pyTiming/pyPeriod/lombScargle.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyTiming/pyPeriod/exampleSanity.py` & `PyAstronomy-0.9.0/src/pyTiming/pyPeriod/exampleSanity.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyTiming/pyPeriod/fourier.py` & `PyAstronomy-0.9.0/src/pyTiming/pyPeriod/fourier.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyTiming/pyPeriod/gls.py` & `PyAstronomy-0.9.0/src/pyTiming/pyPeriod/gls.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyTiming/pyPeriod/periodBase.py` & `PyAstronomy-0.9.0/src/pyTiming/pyPeriod/periodBase.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyTiming/pyPDM/exampleSanity.py` & `PyAstronomy-0.9.0/src/pyTiming/pyPDM/exampleSanity.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyTiming/pyPDM/pdm.py` & `PyAstronomy-0.9.0/src/pyTiming/pyPDM/pdm.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/numericalDerivatives.py` & `PyAstronomy-0.9.0/src/pyaC/mtools/numericalDerivatives.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/conversions.py` & `PyAstronomy-0.9.0/src/pyaC/conversions.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/output.py` & `PyAstronomy-0.9.0/src/pyaC/output.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/pyaErrors/pyaErrTemplate.py` & `PyAstronomy-0.9.0/src/pyaC/pyaErrors/pyaErrTemplate.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,22 @@
     if head:
       e = "\n"
       e += "---------------------\n"
       e += "A PyA error occurred:\n"
       e += "---------------------\n"
       e += "Type of error: " + self.errorType + "\n"
     e += "What happened?\n"
-    e += self.what + "\n"
+    e += "    " + self.what + "\n"
     if not self.where is None:
       e += "Where did it happen?\n"
-      e += self.where + "\n"
+      e += "    " + self.where + "\n"
     if not self.why is None:
       e += "Why did it happen?\n"
-      e += self.why + "\n"
+      e += "    " + self.why + "\n"
     if not self.solution is None:
       e += "What are possible solutions?\n"
       for s in self.solution:
-        e += " - " + s + "\n"
+        e += "  - " + s + "\n"
     if not self.addInfo is None:
       e += "Additional information:\n"
-      e += self.addInfo + "\n"
+      e += "    " + self.addInfo + "\n"
     return e
```

### Comparing `PyAstronomy-0.8.1/src/pyaC/pyaErrors/pyaValErrs.py` & `PyAstronomy-0.9.0/src/pyaC/pyaErrors/pyaValErrs.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/pyaErrors/pyaOtherErrors.py` & `PyAstronomy-0.9.0/src/pyaC/pyaErrors/pyaOtherErrors.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/simiof.py` & `PyAstronomy-0.9.0/src/pyaC/simiof.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/pyaPermanent/pyaFS.py` & `PyAstronomy-0.9.0/src/pyaC/pyaPermanent/pyaFS.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/pyaPermanent/pyaConfig.py` & `PyAstronomy-0.9.0/src/pyaC/pyaPermanent/pyaConfig.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/pyaPermanent/updateCycler.py` & `PyAstronomy-0.9.0/src/pyaC/pyaPermanent/updateCycler.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/importCheck.py` & `PyAstronomy-0.9.0/src/pyaC/importCheck.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/invertIndexSelection.py` & `PyAstronomy-0.9.0/src/pyaC/invertIndexSelection.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/fuzzyMatch.py` & `PyAstronomy-0.9.0/src/pyaC/fuzzyMatch.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/nestedLoop.py` & `PyAstronomy-0.9.0/src/pyaC/nestedLoop.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/pyaC/sanityNeedfThings.py` & `PyAstronomy-0.9.0/src/pyaC/sanityNeedfThings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import os
 
-class SanityOfPyasl(unittest.TestCase):
+class SanityOfNeedfulThings(unittest.TestCase):
   
   def setUp(self):
     pass
   
   def tearDown(self):
     if os.path.isfile("test.tmp"):
       os.remove("test.tmp")
@@ -70,78 +70,15 @@
     print "Exact match: {em:}, close match(es): {cm:}".format(**r)
     
     r = pyaC.fuzzyMatch("One", wordList, cutoff=0.4)
     print "Exact match: {em:}, close match(es): {cm:}".format(**r)
     
     r = pyaC.fuzzyMatch("One", wordList, caseSensitive=False)
     print "Exact match: {em:}, close match(es): {cm:}".format(**r)
-
-  def sanity_numericalDerivative(self):
-    """
-      Checking accuracy of numerical derivatives.
-    """
-    # Check polynomial
-    from numericalDerivatives import diffCFD
-    import numpy as np
-    
-    # Analytical derivatives
-    x = np.linspace(-10,10,1000)
-    y = [np.poly1d((0.03, -0.31, 0.4, 0.35, 1.4))]
-    for i in range(4):
-      y.append(y[-1].deriv())
-    
-    for erro in [2,4,6]:
-      for i in range(1,5):
-        indi, der = diffCFD(x, np.polyval(y[0], x), i, erro)
-        self.assertLess(np.max(np.abs(der/np.polyval(y[i], x[indi]) - 1.0)), 2e-2*pow(10.0,erro-2))
-    
-    # Check trigonometric
-    y = [np.sin(x/10.0*2*np.pi+3)]
-    y.append(2*np.pi/10.0 * np.cos(x/10.0*2*np.pi+3))
-    y.append(-(2*np.pi/10.0)**2 * np.sin(x/10.0*2*np.pi+3))
-    y.append(-(2*np.pi/10.0)**3 * np.cos(x/10.0*2*np.pi+3))
-    y.append((2*np.pi/10.0)**4 * np.sin(x/10.0*2*np.pi+3))
-    for erro in [2,4,6]:
-      for i in range(1,5):
-        indi, der = diffCFD(x, y[0], i, erro)
-        self.assertLess(np.max(np.abs(der/y[i][indi] - 1.0)), 1e-3*pow(10.0,erro-2))
-    
-    # Check exponential
-    y = np.exp(x)
-    for erro in [2,4,6]:
-      for i in range(1,5):
-        print i, erro
-        indi, der = diffCFD(x, y, i, erro)
-        self.assertLess(np.max(np.abs(der/y[indi] - 1.0)), 1e-3*pow(10.0,erro-2))
-
-  def sanity_diffCFDExample(self):
-    """
-      diffCFD example
-    """
-    from PyAstronomy import pyaC
-    import matplotlib.pylab as plt
-    import numpy as np
-    
-    x = np.linspace(-10,10,1000)
     
-    # Computer polynomial and its derivatives
-    # (quasi analytically)
-    y = [np.poly1d((0.03, -0.31, 0.4, 0.35, 1.4))]
-    for i in range(4):
-      y.append(y[-1].deriv())
-    
-    # Compute derivates numerically and compare to
-    # analytic solution
-    erro = 2
-    for i in range(1,5):
-      indi, der = pyaC.diffCFD(x, np.polyval(y[0], x), i, erro)
-      plt.plot(x[indi], np.polyval(y[i], x[indi]), 'b.')
-      plt.plot(x[indi], der, 'r--')
-#      plt.show()
-
   def sanity_matrix2doutputExample(self):
     """
       Sanity of matrix2doutput.
     """
     from PyAstronomy import pyaC as PC
     import numpy as np
```

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/rmcl_ohta.py` & `PyAstronomy-0.9.0/src/modelSuite/XTran/rmcl_ohta.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/limBrightTrans.py` & `PyAstronomy-0.9.0/src/modelSuite/XTran/limBrightTrans.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/circKepZList.py` & `PyAstronomy-0.9.0/src/modelSuite/XTran/circKepZList.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy
 from PyAstronomy.pyaC import pyaErrors as PE
+from PyAstronomy import pyasl
 
 class _ZList:
   """
     Calculate the projected distance between the centers of star and planet.
     
     The resulting values will be stored in the `_zlist` attribute. Additionally,
     the indices belonging to in-transit points will be saved in the `_intrans`
@@ -56,45 +57,53 @@
       Parameters
       ----------
       time : array
           The time points (unit has to be consistent throughout all
           parameters used for calculation).
     """
     # Assign values to KeplerEllipse
-    self.ke.a = self["a"]
-    self.ke.e = self["e"]
-    self.ke.i = self["i"]
-    self.ke.Omega = self["Omega"]
-    self.ke.per = self["per"]
-    self.ke.tau = self["T0pa"]
-    self.ke.w = self["w"]
+    self._ke.a = self["a"]
+    self._ke.e = self["e"]
+    self._ke.i = self["i"]
+    self._ke.Omega = self["Omega"]
+    self._ke.per = self["per"]
+    self._ke.tau = self["tau"]
+    self._ke.w = self["w"]
     
     # Initialize the z-list (NaN values will be neglected)
     self._zlist = numpy.empty(len(time))
     self._zlist[:] = numpy.NAN
     # Get position of body from Keplerian orbit
-    pos = self.ke.xyzPos(time)
+    pos = self._ke.xyzPos(time)
+    
+    # Default line of sight is in +z direction (i.e., observer
+    # located at -z)
+    
+    # Calculate projected distance between centers of star and
+    # planet sqrt(x**2 + y**2)
+    z = numpy.sqrt(pos[::,0]**2 + pos[::,1]**2)
     
     # If enabled, check for body collisions
-    if self.collisionCheck:
+    if self._collisionCheck:
       r = numpy.sqrt(pos[::,0]**2+pos[::,1]**2+pos[::,2]**2)
       indi = numpy.where(r < 1.+self["p"])[0]
       if len(indi) > 0:
         raise(PE.PyAValError("There is a body collision on this orbit.", \
                              where="_ZList"))
     
-    # Calculate projected distance between centers of star and planet sqrt(x**2 + y**2)
-    z = numpy.sqrt(pos[::,0]**2 + pos[::,1]**2)
+
     # Determine which values are relevant. In particular, these are those
     # for which the planet is in front of the star (z > 0) and the distance
     # between stellar and planetary distance is lower than 1+p.
-    self._intrans = numpy.where(numpy.logical_and(z <= (1.+self["p"]), pos[::,2] > 0.0))[0]
+    self._intrans = numpy.where(numpy.logical_and(z <= (1.+self["p"]), pos[::,2] < 0.0))[0]
     
-    # Calculate the 'orbit' and store z-values in __zlist
+    # Calculate the 'orbit' and store z-values in _zlist
     self._zlist[self._intrans] = z[self._intrans]
   
   
-  def __init__(self, orbit):
+  def __init__(self, orbit, cc=True):
     if orbit == "circular":
       self._calcZList = self._zlistCirc
     elif orbit == "keplerian":
+      self._collisionCheck = cc
+      self._ke = pyasl.KeplerEllipse(1.,1.)
       self._calcZList = self._zlistKep
```

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/mandelAgol.py` & `PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/mandelAgolNL.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 # -*- coding: utf-8 -*-
 import numpy
 import PyAstronomy.funcFit as fuf
 from PyAstronomy.pyaC import pyaErrors as PE
 from PyAstronomy.modelSuite.XTran import _ZList
 
 try:
-  import occultquad
-  _importOccultquad = True
+  import occultnl
+  _importOccultnl = True
 except ImportError:
-  _importOccultquad = False
+  _importOccultnl = False
   
     
-class MandelAgolLC(_ZList, fuf.OneDFit):
+class MandelAgolNLLC(_ZList, fuf.OneDFit):
   """
     Calculate and fit analytical transit light-curves using the formulae
-    provided by Mandel & Agol 2002.
+    provided by Mandel & Agol 2002. This model uses the non-linear
+    limb-darkening prescription by Claret 2011:
+    
+    .. math :: \\frac{I(\mu)}{I(1)}= 1 - \\sum_{n=1}^{4}{a_n(1-\mu^{n/2})}
     
     .. note :: The computation of transit light curves
-               is done using the external *occultquad* FORTRAN library.
+               is done using the external *occultnl* FORTRAN library.
                This library must be compiled manually using SciPy's f2py
                wrapper (http://www.scipy.org/F2py). Simply go to the
                *forTrans* directory of the source distribution of PyAstronomy,
                then invoke
                
-               f2py -c occultquad.pyf occultquad.f
+               f2py -c occultnl.pyf occultnl.f
+               
                
-               That's it. 
     
     *Model parameters*:
       - `p` - Radius ratio between planet and star.
       - `a` - Semi-major axis of planetary orbit [stellar radii].
       - `i` - Inclination of orbit in degrees (90 deg is *edge on* view).
-      - `linLib` - Linear limb-darkening coefficient.
-      - `quadLimb` - Quadratic limb-darkening coefficient.
+      - `a1` - Non-Linear limb-darkening coefficient.
+      - `a2` - Non-Linear limb-darkening coefficient.
+      - `a3` - Non-Linear limb-darkening coefficient.
+      - `a4` - Non-Linear limb-darkening coefficient.
       - `T0` - Time offset of transit center.
       - `per` - Period of planetary orbit.
       - `b` - Describes the flux ratio between a stellar companion and the main star (default is 0).
-
-    This class inherits the functionality of funcFit's OneDFit object.
-    You can, therefore, set and get the parameter using the brackets:
-      e.g., pallc["p"] = 0.12345
-
-    .. warning::
-        Time units have to be consistent.
+    
   """
   
   def __init__(self):
     _ZList.__init__(self, "circular")
-    if not _importOccultquad:
+    if not _importOccultnl:
         raise(PE.PyARequiredImport("Could not import required shared object library 'occultquad.so'",\
                                    solution=["Invoke PyA's install script (setup.py) with the --with-ext option.",
-                                             "Go to 'forTrans' directory of PyAstronomy and invoke\n    f2py -c occultquad.pyf occultquad.f"]
+                                             "Go to 'forTrans' directory of PyAstronomy and invoke\n    f2py -c occultnl.pyf occultnl.f"]
                                    ))
 
-    fuf.OneDFit.__init__(self, ["p", "a", "i", "linLimb", "quadLimb", "T0", "per", "b"])
-    self.freeze(["p", "a", "i", "linLimb", "quadLimb", "T0", "per", "b"])
-    self.setRootName("Occultquad")
+    fuf.OneDFit.__init__(self, ["p", "a", "i", "a1", "a2", "a3", "a4", "T0", "per", "b"])
+    self.freeze(["p", "a", "i", "a1", "a2", "a3", "a4", "T0", "per", "b"])
+    self.setRootName("MandelAgolNL")
     
     self.__zlist=None
     
   def evaluate(self, time):
     """ 
      Calculate a light curve according to the analytical models
-     given by Pal 2008.
+     given by Mandel & Agol 2002.
         
      Parameters
      ----------
      time : array
          An array of time points at which the light curve
          shall be calculated.
         
@@ -79,18 +78,19 @@
     """
 
     # Translate the given parameters into an orbit and, finally,
     # into a projected, normalized distance (z-parameter)
     self._calcZList(time - self["T0"])
 
     # Use occultquad Fortran library to compute flux decrease
-    df = numpy.zeros(len(time))
-    if len(self._intrans) > 0:
-      result = occultquad.occultquad(self._zlist[self._intrans],self["linLimb"],self["quadLimb"], \
-                                     self["p"],len(self._intrans))
-      df[self._intrans] = (1.0 - result[0])
+    result = occultnl.occultnl(self["p"],self["a1"],self["a2"],self["a3"], \
+                               self["a4"],self._zlist[self._intrans])
     
+    df = numpy.zeros(len(time))
+    df[self._intrans] = (1.0 - result[0])
+ 
     self.lightcurve = (1.-df)*1./(1.+self["b"]) + self["b"]/(1.0+self["b"])
     
     return self.lightcurve
 
-MandelAgolLC_Rebin = fuf.turnIntoRebin(MandelAgolLC)
+
+MandelAgolNLLC_Rebin = fuf.turnIntoRebin(MandelAgolNLLC)
```

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/exampleSanity.py` & `PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/exampleSanity.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,100 +4,130 @@
   
   def setUp(self):
     pass
   
   def tearDown(self):
     pass
   
-  def sanity_calcModel(self):
+  def sanity_calcModel_1(self):
     # Import some unrelated modules
-    import numpy
-    import matplotlib.pylab as mpl
-    
+    import numpy as np
+    import matplotlib.pylab as plt
     # ... and now the forTrans module
     from PyAstronomy.modelSuite import forTrans as ft
     
-    # Load a simple timer for demonstration purposes
-    import time as timerMod
     
-    # Create MandelAgolLC object
-    ma = ft.MandelAgolLC()
+    # Create MandelAgolLC object with
+    # circular orbit and quadratic limb darkening
+    ma = ft.MandelAgolLC(orbit="circular", ld="quad")
+    
+    # See the available parameters and their current values
+    ma.parameterSummary()
     
     # Set parameters
     ma["per"] = 0.2
     ma["i"] = 90.0
     ma["a"] = 6.5
-    ma["T0"] = 0.5
+    ma["T0"] = 0.0
     ma["p"] = 0.16
     ma["linLimb"] = 0.47
     ma["quadLimb"] = 0.24
     ma["b"] = 0.
     
-    # Choose some (large) time axis
-    time = numpy.linspace(0,5,100000)
-    
-    # Start the clock
-    tstart = timerMod.time()
+    # Choose some time axis
+    time = np.linspace(0, 0.5, 1000)
     
     # ... and calculate model
     y = ma.evaluate(time)
     
-    # Stop the clock
-    tstop = timerMod.time()
-    print "Elapsed time [sec]:", tstop -tstart
+    # Let's see what happened ...
+    plt.plot(time, y, 'b.')
+    #plt.show()
+
+  def sanity_calcModel_2(self):
+    # Import some unrelated modules
+    import numpy as np
+    import matplotlib.pylab as plt
+    # ... and now the forTrans module
+    from PyAstronomy.modelSuite import forTrans as ft
+    
+    
+    # Create MandelAgolLC object with
+    # keplerian orbit and quadratic limb darkening
+    ma = ft.MandelAgolLC(orbit="keplerian", ld="quad")
+    
+    # See the available parameters and their current values
+    ma.parameterSummary()
+    
+    # Set parameters
+    ma["per"] = 0.2
+    ma["i"] = 88.76
+    ma["a"] = 6.5
+    ma["p"] = 0.16
+    ma["linLimb"] = 0.47
+    ma["quadLimb"] = 0.24
+    ma["b"] = 0.
+    ma["e"] = 0.75
+    ma["w"] = 127.
+    ma["Omega"] = 3.9
+    
+    # Choose some time axis
+    time = np.linspace(0, 0.5, 1000)
+    
+    # ... and calculate model
+    y = ma.evaluate(time)
     
     # Let's see what happened ...
-    mpl.plot(time, y,'.')
-#    mpl.show()
+    plt.plot(time, y, 'b.')
+    #plt.show()
 
   def sanity_CompareLDLaws(self):
     # Import some modules
-    import numpy
-    import matplotlib.pylab as mpl
-    
+    import numpy as np
+    import matplotlib.pylab as plt
     # ... and now the forTrans module
     from PyAstronomy.modelSuite import forTrans as ft
     
     # First, let's compute a transit model using
     # quadratic limb-darkening prescription.
-    ma = ft.MandelAgolLC()
+    ma = ft.MandelAgolLC(ld="quad")
     
     # Set parameters. The LD coefficients are taken
     # from Claret 2011 for a solar-metallicity star
     # with Teff=6000 K and logg=4.5.
     ma["per"] = 0.2
     ma["i"] = 90.0
     ma["a"] = 6.5
     ma["T0"] = 0.5
     ma["p"] = 0.16
     ma["linLimb"] = 0.0479
     ma["quadLimb"] = 0.2716
     ma["b"] = 0.
     
     # Choose some time axis
-    time = numpy.linspace(0,0.2,1000)
+    time = np.linspace(0,0.2,1000)
     
     # ... and calculate model
     yQLD = ma.evaluate(time)
     
     # Now, let's compute a transit model with
     # non-linear limb-darkening prescription
     # for the same stellar parameters.
-    maNL = ft.MandelAgolNLLC()
+    maNL = ft.MandelAgolLC(ld="nl")
     maNL["per"] = 0.2
     maNL["i"] = 90.0
     maNL["a"] = 6.5
     maNL["T0"] = 0.5
     maNL["p"] = 0.16
     maNL["a1"] = 0.5335
     maNL["a2"] = 0.0793
     maNL["a3"] = -0.3466
     maNL["a4"] = 0.1609
     maNL["b"] = 0.
     
     yNLLD = maNL.evaluate(time)
     
     # Let's compare both models...
-    mpl.plot(time, yQLD,'-',label="Quadratic LD")
-    mpl.plot(time, yNLLD,'d',label="Non-linear LD")
-    mpl.legend()
-#    mpl.show()
+    plt.plot(time, yQLD,'-',label="Quadratic LD")
+    plt.plot(time, yNLLD,'d',label="Non-linear LD")
+    plt.legend()
+    #plt.show()
```

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/occultnl.f` & `PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/occultnl.f`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/occultquad.pyf` & `PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/occultquad.pyf`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/occultnl.pyf` & `PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/occultnl.pyf`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/forTrans/occultquad.f` & `PyAstronomy-0.9.0/src/modelSuite/XTran/forTrans/occultquad.f`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/exampleSanity.py` & `PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/exampleSanity.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     pass
   
   def sanity_calcModel(self):
     """
       Calculate a Pal transit model.
     """
     from PyAstronomy.modelSuite import palTrans
-    import matplotlib.pylab as mpl
-    import numpy
-  
+    import matplotlib.pylab as plt
+    import numpy as np
+    
     # Create a PalLC instance
     plc = palTrans.PalLC()
     
     # Set parameter values
     plc["p"] = 0.1    # Planet radius / Stellar radius
     plc["per"] = 1.0  # Orbital period
     plc["a"] = 2.0    # Large semi major axis [R_S]
@@ -33,31 +33,31 @@
     # Specify binary contribution
     plc["b"] = 0.0
     
     # Check the parameters
     plc.parameterSummary()
     
     # Create a time axis
-    time = numpy.arange(1000)/1000.0 - 0.5
+    time = np.arange(1000)/1000.0 - 0.5
     
     # Calculate the light curve using above set
     # model parameters
     lightcurve = plc.evaluate(time)
     
     # Plot the result
-    mpl.plot(time, lightcurve, 'bp')
-    # mpl.show()
+    plt.plot(time, lightcurve, 'bp')
+    #plt.show()
 
   def sanity_FitModel(self):
     """
       Trying to fit a Pal transit model. 
     """
     from PyAstronomy.modelSuite import palTrans
-    import matplotlib.pylab as mpl
-    import numpy
+    import matplotlib.pylab as plt
+    import numpy as np
     
     # Create a PalLC instance
     plc = palTrans.PalLC()
     
     # Set parameter values
     plc["p"] = 0.1    # Planet radius / Stellar radius
     plc["per"] = 1.0  # Orbital period
@@ -73,63 +73,63 @@
     plc["b"] = 0.0
     
     # Check the parameters
     print "Input parameters: "
     plc.parameterSummary()
     
     # Create a time axis
-    time = numpy.arange(100)/100.0 * 0.2 - 0.2
+    time = np.arange(100)/100.0 * 0.2 - 0.2
     
     # Calculate the light curve using above set
     # model parameters
     lc = plc.evaluate(time)
     
     # Save the result and add some noise
-    flux = lc + numpy.random.normal(0.0, 0.002, time.size)
+    flux = lc + np.random.normal(0.0, 0.002, time.size)
     
     # Now lets try to recover what we put in
     # Choose some "guess" parameters
-    plc["p"] = 0.12    # Planet radius / Stellar radius
+    plc["p"] = 0.1     # Planet radius / Stellar radius
     plc["per"] = 1.0   # Orbital period
-    plc["a"] = 7.0     # Large semi major axis [R_S]
+    plc["a"] = 7.5     # Large semi major axis [R_S]
     plc["i"] = 90.0    # Orbital inclination [deg]
     # Specify limb darkening
     # (quadratic limb-darkening law)
     plc["linLimb"] = 0.4
     plc["quadLimb"] = 0.2
     # Specify T0 (central time of transit)
     plc["T0"] = -0.08
     # Specify binary contribution
     plc["b"] = 0.0
     
     # Assume we want to fit "p", "a", "i", and "T0"
-    plc.thaw(["p", "a", "T0", "i"])
+    plc.thaw(["T0", "i"])
     
     # Before we start fitting, check how the elliptical integrals
     # are evaluated (mpmath or Boost)
     print "Which elliptical integrals are used?: ", plc.whichEllInts()
     
     # Carry out the fit
-    plc.fit(time, flux, yerr=numpy.ones(time.size)*0.002)
+    plc.fit(time, flux, yerr=np.ones(time.size)*0.002)
     
     print "Fit parameters: "
     plc.parameterSummary()
     
     # Plot the result
-    mpl.plot(time, flux, 'bp')
-    mpl.plot(time, plc.model, 'r-')
-    # mpl.show()
+    plt.plot(time, flux, 'bp')
+    plt.plot(time, plc.model, 'r-')
+    #plt.show()
   
   def sanity_RebinModel(self):
     """
       Evaluating a rebinned Pal transit model.
     """
     from PyAstronomy.modelSuite import palTrans
-    import matplotlib.pylab as mpl
-    import numpy
+    import matplotlib.pylab as plt
+    import numpy as np
     
     # Create a PalLC_Rebin instance
     plc = palTrans.PalLC_Rebin()
     
     # Set parameter values
     plc["p"] = 0.1    # Planet radius / Stellar radius
     plc["per"] = 1.0  # Orbital period
@@ -144,23 +144,23 @@
     # Specify binary contribution
     plc["b"] = 0.0
     
     # Check the parameters
     plc.parameterSummary()
     
     # Create a time axis
-    time = numpy.arange(50)/50.0 - 0.51
+    time = np.arange(50)/50.0 - 0.51
     
     # Specify oversampling parameters.
     # Here use 10 points per observed bin.
     plc.setRebinArray_Ndt(time, 10, time[1]-time[0])
     
     # Calculate the light curve using above set
     # model parameters
     lc = plc.evaluate(time)
     
     # Plot the result (both the overbinned and final
     # model light-curves)
-    mpl.plot(plc.rebinTimes, plc.unbinnedModel, 'b.-')
-    mpl.plot(time, plc.binnedModel, 'rd--')
-    mpl.legend(["Overbinned LC", "Averaged LC"])
-    # mpl.show()
+    plt.plot(plc.rebinTimes, plc.unbinnedModel, 'b.-')
+    plt.plot(time, plc.binnedModel, 'rd--')
+    plt.legend(["Overbinned LC", "Averaged LC"])
+    #plt.show()
```

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/seconPal.py` & `PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/seconPal.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/ellint/ell.cpp` & `PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/ellint/ell.cpp`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/ellint/makefile_template` & `PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/ellint/makefile_template`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/pal.py` & `PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/pal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 import numpy
 import PyAstronomy.funcFit as fuf
-from PyAstronomy.pyasl import KeplerEllipse
 from PyAstronomy.pyaC import pyaErrors as PE
 from PyAstronomy.modelSuite.XTran import _ZList
 
 
 # Check whether mpmath and/or the elliptical integrals from the boost library
 # can be imported.
 
@@ -349,24 +348,17 @@
 
 
 
 
     
 class PalLCKep(PalLC):
   """
-    Calculate and fit analytical transit light-curves using the formulae
-    provided by Pal 2008.
-    
-    In the **special case of the circular orbit** with e=0, w=0, and Omega=0,
-    the time of periastron passage, `T0pa`, will be related to the central
-    time of the transit, `T0` as
-      
-      T0 = T0pa + period/4 .
+    Analytical transit light-curves using the formulae provided by Pal 2008.
     
-    In general, however, this will not be the case.
+    More information on the Keplerian orbit can be found here: :ref:`keplerorbitpyasl`
     
     .. note :: The **evaluation of elliptical integrals** is essential
                in calculating the transit model. While both
                the *mpmath* module and the *Boost* libraries implement
                those integrals, it is the Boost library, which
                evaluates them by far more quickly. Yet, the support
                for Boost has to be added manually. 
@@ -376,15 +368,15 @@
       - `a` - Semi-major axis of planetary orbit [stellar radii].
       - `w` - Longitude of periastron [deg].
       - `Omega` - Longitude of the ascending node [deg].
       - `e` - Orbital eccentricity.
       - `i` - Inclination of orbit in degrees (90 deg is *edge on* view).
       - `linLib` - Linear limb-darkening coefficient.
       - `quadLimb` - Quadratic limb-darkening coefficient.
-      - `T0pa` - Time of periastron passage.
+      - `tau` - Time of periastron passage.
       - `per` - Period of planetary orbit.
       - `b` - Describes the flux ratio between a stellar companion and the main star (default is 0).
 
     This class inherits the functionality of funcFit's OneDFit object.
     You can, therefore, set and get the parameter using the brackets:
       e.g., pallc["p"] = 0.12345
 
@@ -394,34 +386,50 @@
     Parameters
     ----------
     collisionCheck : boolean
         If set True, it will be checked whether the two bodies collide on the current orbit.
   """
   
   def __init__(self, collisionCheck=False):
-    _ZList.__init__(self, "keplerian")
-    fuf.OneDFit.__init__(self, ["p", "a", "i", "linLimb", "quadLimb", "T0pa", "per", "b", \
+    _ZList.__init__(self, "keplerian", collisionCheck)
+    fuf.OneDFit.__init__(self, ["p", "a", "i", "linLimb", "quadLimb", "tau", "per", "b", \
                                 "w", "Omega", "e"])
-    self.freeze(["p", "a", "i", "linLimb", "quadLimb", "T0pa", "per", "b", \
+    self.freeze(["p", "a", "i", "linLimb", "quadLimb", "tau", "per", "b", \
                  "w", "Omega", "e"])
     self.setRootName("Pal08")
     self["per"] = 1.0
+    self["w"] = -90
     
     self._zlist=None
     
     if (not mpmath_imported) and (not boostEll_imported):
       raise(PE.PyARequiredImport("Neither mpmath nor the elliptical integrals from the boost library could be found!", \
                                  where="PalLC::__init__", solution="Install mpmath or make Boost library available (more complicated - see documentation)"))
     self.useBoost = False
     if boostEll_imported:
       self.useBoost = True
       self.ell = ell.ell()
-    
-    self.ke = KeplerEllipse(self["a"], self["per"])
+
     self.collisionCheck = collisionCheck
+    
+    # Wrap get/setitem to inform about change in parameter name
+    T0paE = PE.PyADeprecationError("The parameter 'T0pa' in PalLCKep had to be renamed 'tau'.", \
+                                   solution="Use 'tau' instead of 'T0pa'.")
+    
+    def getitem(specifier, **kwargs):
+      if specifier == "T0pa":
+        PE.warn(T0paE)
+      return PalLC.__getitem__(self, specifier, **kwargs)
+    self.__getitem__ = getitem
+    
+    def setitem(specifier, value):
+      if specifier == "T0pa":
+        PE.warn(T0paE)
+      PalLC.__setitem__(self, specifier, value)
+    self.__setitem__ = setitem
 
   def evaluate(self, time):
     """ 
       Calculate a light curve according to the analytical models
       given by Pal 2008.
          
       Parameters
```

### Comparing `PyAstronomy-0.8.1/src/modelSuite/XTran/palTrans/palSanity.py` & `PyAstronomy-0.9.0/src/modelSuite/XTran/palTrans/palSanity.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,44 +16,32 @@
   def sanity_CircVsKep(self):
     """
       Check that Keplerian and circular solutions do not differ in case of circular orbit.
     """
     from PyAstronomy.modelSuite.XTran import palTrans as pt
     c = pt.PalLC()
     k = pt.PalLCKep()
-    # Ensure that `k` has a properly defined circular orbit
-    k["w"] = 0.0; k["Omega"] = 0.0; k["e"] = 0.0
+
     # A time axis
-    x = np.linspace(-5., 5., 3000)
+    x = np.linspace(-5., 5., 300)
     for counter in xrange(5):
       # Get some random parameters
       # p, a, i, linLimb, quadLimb, T0, per, b
       linLimb = self._rr(0.,1.)
-      T0 = self._rr(-8., 3.)
       pars = {"p":self._rr(0.02, 0.2),
               "a":self._rr(2., 10),
               "i":self._rr(86., 94.),
               "linLimb":linLimb,
               "quadLimb":self._rr(0,1.-linLimb),
               "per":self._rr(1.,4.),
               "b":self._rr(0., 0.1)
               }
       c.assignValue(pars)
       k.assignValue(pars)
-      c["T0"] = T0
-      k["T0pa"] = c["T0"] - k["per"]/4.
+      c["T0"] = 0.0
+      k["tau"] = 0.0 
       yc = c.evaluate(x)
       yk = k.evaluate(x)
-#      import matplotlib.pylab as plt
-#      plt.cla()
-#      
-##      plt.plot(x, c._zlist, 'b--')
-##      plt.plot(x, k._zlist, 'r--')
-##      plt.show()
-#      
-#      plt.plot(x, yc)
-#      plt.plot(x, yk)
-#      plt.plot(x, yc/yk)
-#      plt.show()
+
       np.testing.assert_almost_equal(yc, yk, \
                                      err_msg="Circular and Keplerian Pal models differ.\n"+"\n".join(k.parameterSummary(toScreen=False))+"\n\n"+ \
                                      "\n".join(c.parameterSummary(toScreen=False)) , decimal=10, verbose=True)
```

### Comparing `PyAstronomy-0.8.1/src/modelSuite/exampleSanity.py` & `PyAstronomy-0.9.0/src/modelSuite/exampleSanity.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/__init__.py` & `PyAstronomy-0.9.0/src/modelSuite/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/radVel.py` & `PyAstronomy-0.9.0/src/modelSuite/radVel.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/voigtAstro.py` & `PyAstronomy-0.9.0/src/modelSuite/voigtAstro.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/keplerEllipseModel.py` & `PyAstronomy-0.9.0/src/modelSuite/keplerEllipseModel.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/LyAProfile.py` & `PyAstronomy-0.9.0/src/modelSuite/LyAProfile.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/lineListGaussModel.py` & `PyAstronomy-0.9.0/src/modelSuite/lineListGaussModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
     # Set parameters of multiGauss
     for i in xrange(self._nl):
       p = str(i+1)
       # Apply global scaling of amplitudes
       self._mg["A"+p] = -self["A"+p] * self["lineScale"]
       self._mg["sig"+p] = self["sig"+p]
       # Apply doppler shift of lines
-      self._mg["mu"+p] = (1.0 + self["vrad"]/299792.458) * self._lineList[i,0]
+      self._mg["mu"+p] = (1.0 + self["vrad"]/299792.458) * self["mu"+p]
     mflux += self._mg.evaluate(mwvl)
     
     if abs(self["vsini"]) > 0.0:
       if self._usefastRB:
         mflux = pyasl.fastRotBroad(mwvl, mflux, self["eps"], np.abs(self["vsini"]))
       else:
         mflux = pyasl.rotBroad(mwvl, mflux, self["eps"], np.abs(self["vsini"]))
```

### Comparing `PyAstronomy-0.8.1/src/modelSuite/rotBroadProfile.py` & `PyAstronomy-0.9.0/src/modelSuite/rotBroadProfile.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/modelSuite/atanProfile.py` & `PyAstronomy-0.9.0/src/modelSuite/atanProfile.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/index.rst` & `PyAstronomy-0.9.0/src/doc/index.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/license.rst` & `PyAstronomy-0.9.0/src/doc/license.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPeriodDoc/examples.rst` & `PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPeriodDoc/examples.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPeriodDoc/periodograms.rst` & `PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPeriodDoc/periodograms.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPeriodDoc/baseClasses.rst` & `PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPeriodDoc/baseClasses.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPDMDoc/examples.rst` & `PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPDMDoc/examples.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyTimingDoc/pyPDMDoc/pdm.rst` & `PyAstronomy-0.9.0/src/doc/pyTimingDoc/pyPDMDoc/pdm.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/conf.py` & `PyAstronomy-0.9.0/src/doc/conf.py`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaCDoc/installingPyA.rst` & `PyAstronomy-0.9.0/src/doc/pyaCDoc/installingPyA.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaPermanentDoc/index.rst` & `PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaPermanentDoc/index.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaPermanentDoc/pyaConfig.rst` & `PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaPermanentDoc/pyaConfig.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaCDoc/needfulThings.rst` & `PyAstronomy-0.9.0/src/doc/pyaCDoc/needfulThings.rst`

 * *Files 15% similar despite different names*

```diff
@@ -87,46 +87,14 @@
   
 Convert degree into rad and vice versa
 ---------------------------------------
 
 .. autofunction:: degtorad
 .. autofunction:: radtodeg
 
-
-Computer numerical derivatives
---------------------------------
-
-.. autofunction:: diffCFD
-
-Example
-~~~~~~~~
-
-::
-
-  from PyAstronomy import pyaC
-  import matplotlib.pylab as plt
-  import numpy as np
-  
-  x = np.linspace(-10,10,1000)
-  
-  # Computer polynomial and its derivatives
-  # (quasi analytically)
-  y = [np.poly1d((0.03, -0.31, 0.4, 0.35, 1.4))]
-  for i in range(4):
-    y.append(y[-1].deriv())
-  
-  # Compute derivates numerically and compare to
-  # analytic solution
-  erro = 2
-  for i in range(1,5):
-    indi, der = pyaC.diffCFD(x, np.polyval(y[0], x), i, erro)
-    plt.plot(x[indi], np.polyval(y[i], x[indi]), 'b.')
-    plt.plot(x[indi], der, 'r--')
-    plt.show()
-
     
 Matrix (2d) output
 -------------------
 
 .. autofunction:: matrix2doutput
 
 Example
```

### Comparing `PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaErrorsDoc/index.rst` & `PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaErrorsDoc/index.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaCDoc/pyaErrorsDoc/pyaExTemplate.rst` & `PyAstronomy-0.9.0/src/doc/pyaCDoc/pyaErrorsDoc/pyaExTemplate.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaCDoc/whatIsIt.rst` & `PyAstronomy-0.9.0/src/doc/pyaCDoc/whatIsIt.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaCDoc/versioning.rst` & `PyAstronomy-0.9.0/src/doc/pyaCDoc/versioning.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaCDoc/IDLPorting.rst` & `PyAstronomy-0.9.0/src/doc/pyaCDoc/IDLPorting.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/changeLog/from020to030.rst` & `PyAstronomy-0.9.0/src/doc/changeLog/from020to030.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/changeLog/from040to050.rst` & `PyAstronomy-0.9.0/src/doc/changeLog/from040to050.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/changeLog/from060to070.rst` & `PyAstronomy-0.9.0/src/doc/changeLog/from060to070.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/changeLog/from050to060.rst` & `PyAstronomy-0.9.0/src/doc/changeLog/from050to060.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/changeLog/from030to040.rst` & `PyAstronomy-0.9.0/src/doc/changeLog/from030to040.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/changeLog/from070to080.rst` & `PyAstronomy-0.9.0/src/doc/changeLog/from070to080.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/Makefile` & `PyAstronomy-0.9.0/src/doc/Makefile`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aberration.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aberration.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/crosscorr.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/crosscorr.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/broad.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/broad.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,32 +6,40 @@
 .. autofunction:: instrBroadGaussFast
 
 Example of usage
 -----------------
 
 ::
 
-  from PyAstronomy import pyasl
-  import matplotlib.pylab as plt
-  import numpy as np
-  
-  # Set up an input spectrum
-  x = np.linspace(5000.0,5100.0,1000)
-  y = np.ones(x.size)
-  
-  # Introduce some delta-peaked lines
-  y[165] = 0.7
-  y[187] = 0.3
-  y[505] = 0.1
-  y[610] = 0.1
-  y[615] = 0.7
-  
-  # Apply Gaussian instrumental broadening, setting the resolution to 10000.
-  r, fwhm = pyasl.instrBroadGaussFast(x, y, 10000,
-            edgeHandling="firstlast", fullout=True)
-  
-  print "FWHM used for the Gaussian kernel: ", fwhm, " A"
-  
-  # Plot the output
-  plt.plot(x,r, 'r--p')
-  plt.plot(x,y, 'b-')
-  plt.show()
+    from PyAstronomy import pyasl
+    import matplotlib.pylab as plt
+    import numpy as np
+    
+    # Set up an input spectrum
+    x = np.linspace(5000.0,5100.0,1000)
+    y = np.ones(x.size)
+    
+    # Introduce some delta-peaked lines
+    y[165] = 0.7
+    y[187] = 0.3
+    y[505] = 0.1
+    y[610] = 0.1
+    y[615] = 0.7
+    
+    # Apply Gaussian instrumental broadening, setting the resolution to 10000.
+    r, fwhm = pyasl.instrBroadGaussFast(x, y, 10000,
+              edgeHandling="firstlast", fullout=True)
+    
+    # Apply Gaussian instrumental broadening, setting the resolution to 10000.
+    # Limit the extent of the Gaussian broadening kernel to five standard
+    # deviations.
+    r2, fwhm = pyasl.instrBroadGaussFast(x, y, 10000,
+              edgeHandling="firstlast", fullout=True, maxsig=5.0)
+              
+    print "FWHM used for the Gaussian kernel: ", fwhm, " A"
+    
+    # Plot the output
+    plt.plot(x,r, 'r--p', label="Broadened curve (full)")
+    plt.plot(x, r2, 'k:', label="Broadened curve (5 stds)")
+    plt.plot(x,y, 'b-', label="Input")
+    plt.legend(loc=4)
+    plt.show()
```

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/estimateSNR.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/estimateSNR.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/magnitudes.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/magnitudes.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/transVis-WASP-7b.png` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/transVis-WASP-7b.png`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/coorTimeDate.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/coorTimeDate.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/unredDoc.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/unredDoc.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/stellarAge.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/stellarAge.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/pizzolato2003Doc.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/pizzolato2003Doc.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/ramirez2005.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/ramirez2005.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/expCorrRN.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/aslExt_1Doc/expCorrRN.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/coordinates.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/coordinates.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/transitVisibility.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/transitVisibility.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/baryvel.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/baryvel.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/nutate.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/nutate.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/dopplerShift.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/dopplerShift.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/cardinalPoint.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/cardinalPoint.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/transitDuration.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/transitDuration.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/airmass.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/airmass.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/fluxConversion.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/fluxConversion.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/readFitsSpec.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/readFitsSpec.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/pyasl_wvlconv.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/pyasl_wvlconv.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/pyaslAitoff.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/pyaslAitoff.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/moon.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/moon.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/binning.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/binning.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/outlier.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/outlier.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/sindex.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/sindex.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/svd.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/svd.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/quadextreme.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/quadextreme.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/inTran.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/inTran.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/posAngle.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/posAngle.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/rotBroad.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/rotBroad.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/sunpos.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/sunpos.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/folding.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/folding.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/intep.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/intep.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/eq2hor.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/eq2hor.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/altitude.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/altitude.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/decimalYear.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/decimalYear.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/aslDoc/smooth.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/aslDoc/smooth.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/pyasl.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/pyasl.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 .. toctree::
    :maxdepth: 1
    
    aslDoc/keplerOrbit.rst
    aslDoc/magnitudes.rst
    aslDoc/sindex.rst
    aslDoc/atomicNo.rst
+   aslDoc/aslExt_1Doc/abundances.rst
    aslDoc/aslExt_1Doc/pizzolato2003Doc.rst
    aslDoc/aslExt_1Doc/ramirez2005.rst
    aslDoc/aslExt_1Doc/stellarAge.rst
 
 General data analysis
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -117,14 +118,15 @@
 .. toctree::
    :maxdepth: 1
    
    resBasedDoc/baraffe98tracks.rst
    resBasedDoc/nasaExoplanetArchive.rst
    resBasedDoc/exoplanetEU.rst
    resBasedDoc/exoplanetsOrg.rst
+   resBasedDoc/sweet_cat.rst
    resBasedDoc/kuruczModels.rst
    resBasedDoc/fip.rst
    
 
    
 License note
 ----------------
```

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/fip.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/fip.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/exoplanetsOrg.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/exoplanetsOrg.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/exoplanetEU.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/exoplanetEU.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/kuruczModels.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/kuruczModels.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/nasaExoplanetArchive.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/nasaExoplanetArchive.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaslDoc/resBasedDoc/baraffe98tracks.rst` & `PyAstronomy-0.9.0/src/doc/pyaslDoc/resBasedDoc/baraffe98tracks.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/logo/pyalogo.png` & `PyAstronomy-0.9.0/src/doc/logo/pyalogo.png`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/logo/pyafavicon.ico` & `PyAstronomy-0.9.0/src/doc/logo/pyafavicon.ico`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaGuiDoc/modelExplorer.rst` & `PyAstronomy-0.9.0/src/doc/pyaGuiDoc/modelExplorer.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaGuiDoc/pyapicker.rst` & `PyAstronomy-0.9.0/src/doc/pyaGuiDoc/pyapicker.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaGuiDoc/continuumFinder.rst` & `PyAstronomy-0.9.0/src/doc/pyaGuiDoc/continuumFinder.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/pyaGuiDoc/interactiveGV.rst` & `PyAstronomy-0.9.0/src/doc/pyaGuiDoc/interactiveGV.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/constantsDoc/index.rst` & `PyAstronomy-0.9.0/src/doc/constantsDoc/index.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/funcFitDoc/index.rst` & `PyAstronomy-0.9.0/src/doc/funcFitDoc/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -20,26 +20,27 @@
 package. The most important aspects are demonstrated by example. 
 
 .. toctree::
     :maxdepth: 2
 
     tutorial.rst
     tutorial2.rst
+    tutorialMCMC.rst
     traceAnalysisTutorial.rst
 
 Basic models
 ----------------
 
 .. toctree::
     :maxdepth: 2
 
     simplemodels.rst
 
-External fitters
----------------------
+Internal and external fitters
+--------------------------------
 
 .. toctree::
     :maxdepth: 2
 
     extFitters.rst
 
 Parameters and further functionality
@@ -48,12 +49,13 @@
 .. toctree::
     :maxdepth: 2
     
     params.rst
     onedfit.rst
     modelRebin.rst
     syncFit.rst
+    emceePriors.rst
     traceAnalysis.rst
     coordinateGrid.rst
```

### Comparing `PyAstronomy-0.8.1/src/doc/funcFitDoc/nelderMead.rst` & `PyAstronomy-0.9.0/src/doc/funcFitDoc/nelderMead.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/funcFitDoc/tutorial2.rst` & `PyAstronomy-0.9.0/src/doc/funcFitDoc/tutorial2.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/funcFitDoc/onedfit.rst` & `PyAstronomy-0.9.0/src/doc/funcFitDoc/onedfit.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/funcFitDoc/tutorial.rst` & `PyAstronomy-0.9.0/src/doc/funcFitDoc/tutorial.rst`

 * *Files 16% similar despite different names*

```diff
@@ -11,22 +11,27 @@
 .. contents:: Sections of this tutorial
 
 .. _matplotlib: http://matplotlib.sourceforge.net/
 .. _pymc: https://github.com/pymc-devs/pymc
 .. _SciPy: www.scipy.org/
 .. _numpy: numpy.scipy.org/
 .. _XSPEC: http://heasarc.nasa.gov/xanadu/xspec/
+.. _emcee: http://dan.iel.fm/emcee/current/
 
 Prerequisites
 -------------------
 To run the example in this tutorial you need to have installed the following packages:
  * numpy_
  * SciPy_
  * matplotlib_
- * pymc_ (only MCMC example).
+ 
+For MCMC sampling, at least one of the following packages should be installed
+ 
+ * pymc_ (in version *2.x*, unfortunately, version 3.x is not supported)
+ * emcee_
 
 We also assume that you have a basic knowledge of Python and these packages (except for
 pymc).
 
 .. warning:: funcFit relies on **Python 2.7.x**. The 2.6.x series (and prior) has a bug affecting the copying of
              dynamically created class methods, which has not been (and will not be) corrected. This interferes with many of
              funcFit's algorithms.
@@ -53,314 +58,321 @@
 .. note:: In this tutorial, it is assumed that you also have matplotlib installed,
           which provides a neat interface for plotting under Python.
           If you did not already install it, have a look at their we page (matplotlib_).
 
 Diving into the first example
 -------------------------------
 
-After you have installed PyAstronomy (PyA), the funcFit package \
-is ready for being used. As a very first step, let us import the \
-package and see whether we will be able to actually fit something. \
-Therefore, execute the following lines as a script or from the \
+After you have installed PyAstronomy (PyA), the funcFit package
+is ready for being used. As a very first step, let us import the
+package and see whether we will be able to actually fit something.
+Therefore, execute the following lines as a script or from the
 Python interactive command shell: 
 
 ::
 
   from PyAstronomy import funcFit as fuf
   
   fuf.status()
 
 Depending on your installation the output should look like:
 
-
 ::
 
-  Status of funcFit:
-  --------------------------
-  Is scipy.optimize available?  yes
-  Is pymc available?  yes
-
-.. note:: At the moment, you do not need to be concerned about pymc support, but SciPy is indispensable.
-
+    Status of funcFit:
+    --------------------------
+    Is scipy.optimize available?  yes
+    Is pymc available?  yes
+      pymc is available in version:  2.3.4
+    Is emcee available?  yes
+    
 
 Now let us dive into the business of fitting. The first example shown below demonstrates how to \
 exploit the functionality of funcFit to fit a Gaussian to artificially created data. \
 It shows how free parameters can be specified and restrictions can be applied.
 
 ::
 
-  # Import numpy and matplotlib
-  from numpy import arange, sqrt, exp, pi, random, ones
-  import matplotlib.pylab as mpl
-  # ... and now the funcFit package
-  from PyAstronomy import funcFit as fuf
-  
-  # Before we can start fitting, we need something to fit.
-  # So let us create some data...
-  
-  # Creating a Gaussian with some noise
-  # Choose some parameters...
-  gPar = {"A":-5.0, "sig":10.0, "mu":10.0, "off":1.0, "lin":0.0}
-  # Calculate profile
-  x = arange(100) - 50.0
-  y = gPar["off"] + gPar["A"] / sqrt(2*pi*gPar["sig"]**2) \
-      * exp(-(x-gPar["mu"])**2/(2*gPar["sig"]**2))
-  # Add some noise
-  y += random.normal(0.0, 0.01, x.size)
-  # Let us see what we have done...
-  mpl.plot(x, y, 'bp') 
-
-  # Now we can start exploiting the funcFit functionality to
-  # fit a Gaussian to our data. In the following lines, we
-  # create a fitting object representing a Gaussian and set guess parameters.
-
-  # Now let us come to the fitting
-  # First, we create the Gauss1d fit object
-  gf = fuf.GaussFit1d()
-  # See what parameters are available
-  print "List of available parameters: ", gf.availableParameters()
-  # Set guess values for the parameters
-  gf["A"] = -10.0
-  gf["sig"] = 15.77
-  gf["off"] = 0.87
-  gf["mu"] = 7.5
-  # Let us see whether the assignment worked
-  print "Parameters and guess values: "
-  print "  A   : ", gf["A"]
-  print "  sig : ", gf["sig"]
-  print "  off : ", gf["off"]
-  print "  mu  : ", gf["mu"]
-  print ""
-
-  # Now some of the strengths of funcFit are demonstrated; namely, the
-  # ability to consider some parameters as free and others as fixed.
-  # By default, all parameters of the GaussFit1d are frozen.
-  
-  # Show values and names of frozen parameters
-  print "Names and values if FROZEN parameters: ", gf.frozenParameters()
-
-  # Which parameters shall be variable during the fit?
-  # 'Thaw' those (the order is irrelevant)
-  gf.thaw(["A", "sig", "off", "mu"])
-  
-  # Let us assume that we know that the amplitude is negative, i.e.,
-  # no lower boundary (None) and 0.0 as upper limit.
-  gf.setRestriction({"A":[None,0.0]})
-  
-  # Now start the fit
-  gf.fit(x, y, yerr=ones(x.size)*0.01)
-  
-  # Write the result to the screen and plot the best fit model
-  gf.parameterSummary()
-  mpl.plot(x, gf.model, 'r--')
-  
-  # Show the data and the best fit model
-  mpl.show()
+    # Import numpy and matplotlib
+    from numpy import arange, sqrt, exp, pi, random, ones
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
+    from PyAstronomy import funcFit as fuf
+    
+    # Before we can start fitting, we need something to fit.
+    # So let us create some data...
+    
+    # Creating a Gaussian with some noise
+    # Choose some parameters...
+    gPar = {"A":-5.0, "sig":10.0, "mu":10.0, "off":1.0, "lin":0.0}
+    # Calculate profile
+    x = arange(100) - 50.0
+    y = gPar["off"] + gPar["A"] / sqrt(2*pi*gPar["sig"]**2) \
+        * exp(-(x-gPar["mu"])**2/(2*gPar["sig"]**2))
+    # Add some noise
+    y += random.normal(0.0, 0.01, x.size)
+    # Let us see what we have done...
+    plt.plot(x, y, 'bp')
+    
+    # Now we can start exploiting the funcFit functionality to
+    # fit a Gaussian to our data. In the following lines, we
+    # create a fitting object representing a Gaussian and set guess parameters.
+    
+    # Now let us come to the fitting
+    # First, we create the Gauss1d fit object
+    gf = fuf.GaussFit1d()
+    # See what parameters are available
+    print "List of available parameters: ", gf.availableParameters()
+    # Set guess values for the parameters
+    gf["A"] = -10.0
+    gf["sig"] = 15.77
+    gf["off"] = 0.87
+    gf["mu"] = 7.5
+    # Let us see whether the assignment worked
+    print "Parameters and guess values: "
+    print "  A   : ", gf["A"]
+    print "  sig : ", gf["sig"]
+    print "  off : ", gf["off"]
+    print "  mu  : ", gf["mu"]
+    print ""
+    
+    # Now some of the strengths of funcFit are demonstrated; namely, the
+    # ability to consider some parameters as free and others as fixed.
+    # By default, all parameters of the GaussFit1d are frozen.
+    
+    # Show values and names of frozen parameters
+    print "Names and values of FROZEN parameters: ", gf.frozenParameters()
+    
+    # Which parameters shall be variable during the fit?
+    # 'Thaw' those (the order is irrelevant)
+    gf.thaw(["A", "sig", "off", "mu"])
+    
+    # Let us assume that we know that the amplitude is negative, i.e.,
+    # no lower boundary (None) and 0.0 as upper limit.
+    gf.setRestriction({"A":[None,0.0]})
+    
+    # Now start the fit
+    gf.fit(x, y, yerr=ones(x.size)*0.01)
+    
+    # Write the result to the screen and plot the best fit model
+    gf.parameterSummary()
+    plt.plot(x, gf.model, 'r--')
+    
+    # Show the data and the best fit model
+    plt.show()
 
 
 Running the above script yields the following output (numbers may slightly differ):
 
 ::
 
-  List of available parameters:  ['A', 'mu', 'lin', 'sig', 'off']
-  Parameters and guess values: 
-    A   :  -10.0
-    sig :  15.77
-    off :  0.87
-    mu  :  7.5
-  
-  Names and values if FROZEN parameters: \
-    {'A': -10.0, 'mu': 7.5, 'lin': 0.0, 'sig': 15.77, 'off': 0.87}
-  Optimization terminated successfully.
-           Current function value: 89.047028
-           Iterations: 182
-           Function evaluations: 317
-  Parameter:   A, value:     -4.932741, free: True, restricted: True, \
-    lower bound: None, upper bound:     0.000000
-  Parameter: lin, value:      0.000000, free: False, restricted: False
-  Parameter:  mu, value:      9.942224, free: True, restricted: False
-  Parameter: off, value:      1.000320, free: True, restricted: False
-  Parameter: sig, value:      9.877148, free: True, restricted: False
+    List of available parameters:  ['A', 'mu', 'lin', 'sig', 'off']
+    Parameters and guess values: 
+      A   :  -10.0
+      sig :  15.77
+      off :  0.87
+      mu  :  7.5
+    
+    Names and values of FROZEN parameters:  {'A': -10.0, 'mu': 7.5, 'lin': 0.0, 'sig': 15.77, 'off': 0.87}
+    Optimization terminated successfully.
+             Current function value: 111.455503
+             Iterations: 176
+             Function evaluations: 310
+    ----------------------------------
+    Parameters for Component: Gaussian
+    ----------------------------------
+    Parameter:   A  Gaussian, [  A], value:     -4.92037, free:  True, restricted:  True, related: False
+        Restriction: [None,  0]
+    Parameter:  mu  Gaussian, [ mu], value:      9.83938, free:  True, restricted: False, related: False
+    Parameter: lin  Gaussian, [lin], value:            0, free: False, restricted: False, related: False
+    Parameter: sig  Gaussian, [sig], value:      9.97104, free:  True, restricted: False, related: False
+    Parameter: off  Gaussian, [off], value:     0.999786, free:  True, restricted: False, related: False
 
 
 Some points in the example shall be emphasized:
   * The names of the parameters are defined by the fitting object (in this case GaussFit1d),
   * Parameter values can be set and obtained using brackets,
   * Individual parameters can be thawed or frozen depending on the needs of the user,
   * Restrictions on the parameter ranges can be applied either on both or just on side of the range,
-  * After the fit, the best fit values become the current parameters, i.e., they can be obtained using the bracket operator,
-  * After the fit, the best fit model can be accessed through the `model` property. 
+  * After the fit, the best-fit values become the current parameters, i.e., they can be obtained using the bracket operator,
+  * After the fit, the best-fit model can be accessed through the `model` property. 
 
-The central step of the script is the call to *fit*. The method takes at least two arguments: the \
-x-axis and corresponding y-axis values; errors on the y-axis values can be given optionally \
-via the *yerr* keyword as shown in the example. In default configuration, the *fit* method \
-uses the *fmin* routine provided by SciPy.optimize to minimize :math:`\chi^2` if errors (yerr) \
-are given. If no errors are provided, it will simply minimize the quadratic deviation between \
-model and data.
+The central step of the script is the call to *fit*. The method takes at least two arguments: the
+x-axis and corresponding y-axis values; errors on the y-axis values can be given optionally
+via the *yerr* keyword as shown in the example. In default configuration, the *fit* method
+uses the *fmin* routine provided by SciPy.optimize to minimize either the sum of quadratic residuals
+of no error is provided, or :math:`\chi^2` if errors (yerr)
+are given.
 
-.. note:: Restrictions are implemented using a penalty function. The steepness of the penalty
+.. note:: Restrictions are implemented using a **penalty function**. The steepness of the penalty
           may be changed by the *setPenaltyFactor* method or by accessing the `penaltyFactor`
           property directly.
 
 
 Introducing a custom model
 -------------------------------
 
-The funcFit package comes with some fitting models, but in many cases it will be necessary \
-to use custom models. Introducing a new model is easy in funcFit and will be demonstrated \
+The funcFit package comes with some fitting models, but in many cases it will be necessary
+to use custom models. Introducing a new model is easy in funcFit and will be demonstrated
 in the next example. Here we implement a straight line and fit it to some artificial data.
 
 ::
 
-  # Import numpy and matplotlib
-  from numpy import arange, random
-  import matplotlib.pylab as mpl
-  # ... and now the funcFit package
-  from PyAstronomy import funcFit as fuf
-  
-  class StraightLine(fuf.OneDFit):
-    """
-      Implements a straight line of the form y = "off" + x * "lin".
-    """
-  
-    def __init__(self):
-      fuf.OneDFit.__init__(self, ["off", "lin"])
-  
-    def evaluate(self, x):
+    # Import numpy and matplotlib
+    from numpy import arange, random
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
+    from PyAstronomy import funcFit as fuf
+    
+    class StraightLine(fuf.OneDFit):
       """
-        Calculates and returns model according to the \
-        current parameter values.
-  
-        Parameters:
-          - `x` - Array specifying the positions at \
-                  which to evaluate the model.
+        Implements a straight line of the form y = "off" + x * "lin".
       """
-      y = self["off"] + (self["lin"] * x)
-      return y
     
-  # Generate some data and add noise
-  x = arange(100)
-  y = 10.0 + 2.0 * x + random.normal(0.0, 5.0, 100)
-  
-  # Create fitting class instance and set initial guess
-  # Note that all parameters are frozen by default
-  lf = StraightLine()
-  lf["off"] = 20.0
-  lf["lin"] = 1.0
-  # Thaw parameters
-  lf.thaw(["off", "lin"])
-  
-  # Start fitting
-  lf.fit(x, y)
-  
-  # Investigate the result
-  lf.parameterSummary()
-  mpl.plot(x, y, 'bp')
-  mpl.plot(x, lf.model, 'r--')
-  mpl.show()
+      def __init__(self):
+        fuf.OneDFit.__init__(self, ["off", "lin"])
+    
+      def evaluate(self, x):
+        """
+          Calculates and returns model according to the \
+          current parameter values.
+    
+          Parameters:
+            - `x` - Array specifying the positions at \
+                    which to evaluate the model.
+        """
+        y = self["off"] + (self["lin"] * x)
+        return y
+      
+    # Generate some data and add noise
+    x = arange(100)
+    y = 10.0 + 2.0 * x + random.normal(0.0, 5.0, 100)
+    
+    # Create fitting class instance and set initial guess
+    # Note that all parameters are frozen by default
+    lf = StraightLine()
+    lf["off"] = 20.0
+    lf["lin"] = 1.0
+    # Thaw parameters
+    lf.thaw(["off", "lin"])
+    
+    # Start fitting
+    lf.fit(x, y)
+    
+    # Investigate the result
+    lf.parameterSummary()
+    plt.plot(x, y, 'bp')
+    plt.plot(x, lf.model, 'r--')
+    plt.show()
 
-This example resembles the first one. The new thing is that we defined a custom fitting \
-model at the top instead of using the *GaussFit1d* class seen in the first example.
+This example resembles the first one, but here we defined a custom fitting
+model at the top instead of using the *GaussFit1d* class as in the first example.
 
-A new fitting model is a class, which inherits from the *OneDFit* class. Additionally, two \
+A new fitting model is a class, which inherits from the *OneDFit* class. Additionally, two
 methods (*__init__* and *evaluate*) must be implemented.
-In the example, we \
-provide a minimal constructor (__init__ method), which only consists of a call to the \
-base class (OneDFit) constructor. The argument is a list of strings with the names of the \
-variables characterizing the model. The *evaluate* method takes a single argument, which is \
-an array of values at which to evaluate the model. It returns the function values at the \
-given position. Note how, e.g., *self["off"]*, is used to get the current value if the offset \
+In the example, we
+provide a minimal constructor (__init__ method), which only consists of a call to the
+base class (OneDFit) constructor. The argument is a list of strings with the names of the
+variables characterizing the model. The *evaluate* method takes a single argument, which is
+an array of values at which to evaluate the model. It returns the function values at the
+given position. Note how, e.g., *self["off"]*, is used to get the current value if the offset
 variable in *evaluate*.
 
 Applying *relations*
 ----------------------
 In funcFit *relations* refer to a functional dependence between two or more model parameters.
 To demonstrate the application of such a relation, we slightly extend the previous example.
 In particular, we will assume that the gradient of our line is a multiple of the offset.
 
 ::
   
-  # import numpy and matplotlib
-  from numpy import arange, random
-  import matplotlib.pylab as mpl
-  # ... and now the funcFit package
-  from PyAstronomy import funcFit as fuf
-  
-  class StraightLine(fuf.OneDFit):
-    """
-      Implements a straight line of the form y = "off" + x * "lin".
-    """
-  
-    def __init__(self):
-      fuf.OneDFit.__init__(self, ["off", "lin"])
-  
-    def evaluate(self, x):
-      """
-        Calculates and returns model according to the current parameter values.
-  
-        Parameters:
-          - x - Array specifying the positions at which to evaluate the model.
-      """
-      y = self["off"] + (self["lin"] * x)
-      return y
-  
-  
-  # Create a function, which defines the relation.
-  
-  def getLinearRelation(factor):
-    def linOffRel(off):
+    # import numpy and matplotlib
+    from numpy import arange, random
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
+    from PyAstronomy import funcFit as fuf
+    
+    class StraightLine(fuf.OneDFit):
       """
-        Function used to relate parameters "lin" and "off".
+        Implements a straight line of the form y = "off" + x * "lin".
       """
-      return factor * off
+    
+      def __init__(self):
+        fuf.OneDFit.__init__(self, ["off", "lin"])
+    
+      def evaluate(self, x):
+        """
+          Calculates and returns model according to the current parameter values.
+    
+          Parameters:
+            - x - Array specifying the positions at which to evaluate the model.
+        """
+        y = self["off"] + (self["lin"] * x)
+        return y
+    
+    
+    # Create a function, which defines the relation.
+    
+    def getLinearRelation(factor):
+      def linOffRel(off):
+        """
+          Function used to relate parameters "lin" and "off".
+        """
+        return factor * off
+      return linOffRel
+    
+    # Note, above we used a nested function (a closure) to define
+    # the relation. This approach is very flexible. If we were already
+    # sure about the value of ``factor'' (e.g., 10.0), we could
+    # simply have used:
+    #
+    # def linOffRel(off):
+    #   return 10.0 * off
+    
+    # Generate some data with noise
+    x = arange(100)
+    y = 100.0 + 2.0 * x + random.normal(0.0, 5.0, 100)
+    
+    # Create fitting class instance and set initial guess
+    lf = StraightLine()
+    lf["off"] = 20.0
+    lf["lin"] = 1.0
+    # Thaw parameters
+    lf.thaw(["off", "lin"])
+    
+    # Assume we know about a relation between 'lin' and 'off'
+    # In particular, lin = 9.0 * off. We use the function getLinearRelation
+    # to obtain a function object defining the relation.
+    lf.relate("lin", ["off"], getLinearRelation(9))
+    
+    # Start fitting
+    lf.fit(x, y)
+    
+    # Investigate the result
+    lf.parameterSummary()
+    plt.plot(x, y, 'bp')
+    plt.plot(x, lf.model, 'r--')
+    plt.show()
   
-  # Note, above we used a nested function (a closure) to define
-  # the relation. This approach is very flexible. If we were already
-  # sure about the value of ``factor'' (e.g., 10.0), we could
-  # simply have used:
-  #
-  # def linOffRel(off):
-  #   return 10.0 * off
-  
-  # Generate some data with noise
-  x = arange(100)
-  y = 10.0 + 2.0 * x + random.normal(0.0, 5.0, 100)
-  
-  # Create fitting class instance and set initial guess
-  lf = StraightLine()
-  lf["off"] = 20.0
-  lf["lin"] = 1.0
-  # Thaw parameters
-  lf.thaw(["off", "lin"])
-  
-  # Assume we know about a relation between 'lin' and 'off'
-  # In particular, lin = 9.0 * off. We use the function getLinearRelation
-  # to obtain a function object defining the relation.
-  lf.relate("lin", ["off"], getLinearRelation(9.0))
-  
-  # Start fitting
-  lf.fit(x, y)
-  
-  # Investigate the result
-  lf.parameterSummary()
-  mpl.plot(x, y, 'bp')
-  mpl.plot(x, lf.model, 'r--')
-  mpl.show()
 
 The output of the script reads (numbers may differ):
 
 ::
 
-  Optimization terminated successfully.
-           Current function value: 4684.711018
-           Iterations: 23
-           Function evaluations: 46
-  Parameter: lin, value:      2.120667, free: False, restricted: False,  \
-    Relation: lin = f(off)
-  Parameter: off, value:      2.120667, free: True, restricted: False
+    Optimization terminated successfully.
+             Current function value: 251539.530679
+             Iterations: 27
+             Function evaluations: 54
+    ---------------------------------
+    Parameters for Component: unnamed
+    ---------------------------------
+    Parameter: lin  , [lin], value:       3.5004, free: False, restricted: False, related:  True
+         Relation: lin = f(off)
+    Parameter: off  , [off], value:     0.388933, free:  True, restricted: False, related: False
+
 
 .. note:: The `lin` parameter is no longer free, as it depends on `off`.
 
 The *relate* method takes three arguments. The first is the name of
 the dependent variable (in this case "lin"). The second is a list
 containing the names of the independent variables (in this case
 only "off"). The third argument is a callable object, which provides
@@ -374,111 +386,112 @@
 The funcFit package allows to combine two models. That means that models (then becoming model components) can
 be added, subtracted, divided, multiplied, and even used as exponents. This can be very useful in creating
 more complex models and requires only little effort. The following example shows how two Gaussians models
 can be summed.
 
 ::
 
-  # Import numpy and matplotlib
-  from numpy import arange, sqrt, exp, pi, random, ones
-  import matplotlib.pylab as mpl
-  # ... and now the funcFit package
-  from PyAstronomy import funcFit as fuf
-  
-  # Creating Gaussians with some noise
-  # Choose some parameters...
-  gPar1 = {"A":-5.0, "sig":10.0, "mu":20.0, "off":1.0, "lin":0.0}
-  gPar2 = {"A":+10.0, "sig":10.0, "mu":-20.0, "off":0.0, "lin":0.0}
-  # Calculate profile
-  x = arange(100) - 50.0
-  y = gPar1["off"] + gPar1["A"] / sqrt(2*pi*gPar1["sig"]**2) \
-      * exp(-(x-gPar1["mu"])**2/(2*gPar1["sig"]**2))
-  y -= gPar2["off"] + gPar2["A"] / sqrt(2*pi*gPar2["sig"]**2) \
-      * exp(-(x-gPar2["mu"])**2/(2*gPar2["sig"]**2))
-  # Add some noise
-  y += random.normal(0.0, 0.01, x.size)
-  # Let us see what we have done...
-  mpl.plot(x, y, 'bp')
-  
-  # Now let us come to the fitting
-  # First, we create two Gauss1d fit objects
-  gf1 = fuf.GaussFit1d()
-  gf2 = fuf.GaussFit1d()
-  
-  # Assign guess values for the parameters
-  gf1["A"] = -0.3
-  gf1["sig"] = 3.0
-  gf1["off"] = 0.0
-  gf1["mu"] = +5.0
-  
-  gf2["A"] = 3.0
-  gf2["sig"] = 15.0
-  gf2["off"] = 1.0
-  gf2["mu"] = -10.0
-  
-  # Which parameters shall be variable during the fit?
-  # 'Thaw' those (the order is irrelevant)
-  gf1.thaw(["A", "sig", "mu"])
-  gf2.thaw(["sig", "mu", "off"])
-  
-  # Our actual model is the sum of both Gaussians
-  twoG = gf1 + gf2
-  
-  # Show a description of the model depending on the
-  # names of the individual components
-  print
-  print "Description of the model: ", twoG.description()
-  print
-  
-  # Note that now the parameter names changed!
-  # Each parameter is now named using the "property"
-  # (e.g., 'A' or 'sig') as the first part, the component
-  # "root name" (in this case 'Gaussian') and a component
-  # number in paranthesis.
-  print "New parameter names and values: "
-  twoG.parameterSummary()
-  
-  # We forgot to thaw the amplitude of the second Gaussian, but
-  # we can still do it, but we have to refer to the correct name:
-  # either by using the (new) variable name:
-  twoG.thaw("A_Gaussian(2)")
-  # or by specifying property name, root name, and component number
-  # separately (note that a tuple is used to encapsulate them):
-  twoG.thaw(("A", "Gaussian", 2))
-  # We decide to rather freeze the offset of the second
-  # Gaussian (we could have used a tuple here, too).
-  twoG.freeze("off_Gaussian(2)")
-  
-  # Start fit as usual
-  twoG.fit(x,y,yerr=ones(x.size)*0.01)
-  
-  # Write the result to the screen and plot the best fit model
-  print
-  print "--------------------------------"
-  print "Parameters for the combined fit:"
-  print "--------------------------------"
-  twoG.parameterSummary()
-  
-  # Show the data and the best fit model
-  mpl.plot(x, twoG.model, 'r--')
-  mpl.show()
+    # Import numpy and matplotlib
+    from numpy import arange, sqrt, exp, pi, random, ones
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
+    from PyAstronomy import funcFit as fuf
+    
+    # Creating Gaussians with some noise
+    # Choose some parameters...
+    gPar1 = {"A":-5.0, "sig":10.0, "mu":20.0, "off":1.0, "lin":0.0}
+    gPar2 = {"A":+10.0, "sig":10.0, "mu":-20.0, "off":0.0, "lin":0.0}
+    # Calculate profile
+    x = arange(100) - 50.0
+    y = gPar1["off"] + gPar1["A"] / sqrt(2*pi*gPar1["sig"]**2) \
+        * exp(-(x-gPar1["mu"])**2/(2*gPar1["sig"]**2))
+    y -= gPar2["off"] + gPar2["A"] / sqrt(2*pi*gPar2["sig"]**2) \
+        * exp(-(x-gPar2["mu"])**2/(2*gPar2["sig"]**2))
+    # Add some noise
+    y += random.normal(0.0, 0.01, x.size)
+    # Let us see what we have done...
+    plt.plot(x, y, 'bp')
+    
+    # Now let us come to the fitting
+    # First, we create two Gauss1d fit objects
+    gf1 = fuf.GaussFit1d()
+    gf2 = fuf.GaussFit1d()
+    
+    # Assign guess values for the parameters
+    gf1["A"] = -0.3
+    gf1["sig"] = 3.0
+    gf1["off"] = 0.0
+    gf1["mu"] = +5.0
+    
+    gf2["A"] = 3.0
+    gf2["sig"] = 15.0
+    gf2["off"] = 1.0
+    gf2["mu"] = -10.0
+    
+    # Which parameters shall be variable during the fit?
+    # 'Thaw' those (the order is irrelevant)
+    gf1.thaw(["A", "sig", "mu"])
+    gf2.thaw(["sig", "mu", "off"])
+    
+    # Our actual model is the sum of both Gaussians
+    twoG = gf1 + gf2
+    
+    # Show a description of the model depending on the
+    # names of the individual components
+    print
+    print "Description of the model: ", twoG.description()
+    print
+    
+    # Note that now the parameter names changed!
+    # Each parameter is now named using the "property"
+    # (e.g., 'A' or 'sig') as the first part, the component
+    # "root name" (in this case 'Gaussian') and a component
+    # number in paranthesis.
+    print "New parameter names and values: "
+    twoG.parameterSummary()
+    
+    # We forgot to thaw the amplitude of the second Gaussian, but
+    # we can still do it, but we have to refer to the correct name:
+    # either by using the (new) variable name:
+    twoG.thaw("A_Gaussian(2)")
+    # or by specifying property name, root name, and component number
+    # separately (note that a tuple is used to encapsulate them):
+    twoG.thaw(("A", "Gaussian", 2))
+    # We decide to rather freeze the offset of the second
+    # Gaussian (we could have used a tuple here, too).
+    twoG.freeze("off_Gaussian(2)")
+    
+    # Start fit as usual
+    twoG.fit(x,y,yerr=ones(x.size)*0.01)
+    
+    # Write the result to the screen and plot the best fit model
+    print
+    print "--------------------------------"
+    print "Parameters for the combined fit:"
+    print "--------------------------------"
+    twoG.parameterSummary()
+    
+    # Show the data and the best fit model
+    plt.plot(x, twoG.model, 'r--')
+    plt.show()
 
 .. note:: `twoG` contains copies (not references) two its "ancestors" (`gf1` and `gf2`). You can, thus, continue using those as usual.
 
 When the models are combined (added in this case), funcFit adds "component identifiers" to the variable names to ensure that they
-remain unique. A component identifier is simply an appendix to the variable name consisting of an underscore and a number. The combined
+remain unique. A component identifier is simply an appendix to the variable name consisting of an underscore, the model name,
+and a number. The combined
 model behaves exactly like the individual ones. It should also be noted that model characteristics such as relations, restrictions, etc.,
 are preserved in the combined model.
 
 
 Applying conditional restrictions
 --------------------------------------
 
 Via `conditional restrictions` complex penalty (or reward) functions can be
-defined, which keep the fit out or force into a specific subspace of the
+defined, which keep the fit out or force it into a specific subspace of the
 parameter space. Conditional restrictions are self-defined callables such
 as function, which take a number of parameters and return a float, which
 specifies the penalty. The latter is added to the objective function.
 
 Conditional restrictions are referred to by a unique ID, which is generated
 as soon as it is added to the model. Note that this ID does not change, when
 models are combined.    
@@ -809,452 +822,157 @@
 By default, funcFit minimizes :math:`\chi^2` when an error is given and the quadratic model deviation otherwise. It may, however,
 be necessary to minimize something else such as the likelihood for instance. The following example shows
 how to apply a custom objective function, in this case, we simply use the linear deviation between
 model and data (weighted by the error) to define the fit quality. 
 
 ::
 
-  # Import numpy and matplotlib
-  from numpy import arange, exp, random, ones, sum, abs
-  import matplotlib.pylab as mpl
-  # Import funcFit
-  from PyAstronomy import funcFit as fuf
-  
-  # Define parameters of faked data
-  A = 1.0
-  tau = 10.
-  off = 0.2
-  t0 = 40.
-  
-  # Caculate fake data set
-  x = arange(100)
-  y = A*exp(-(x-t0)/tau) * (x>t0) + off
-  y += random.normal(0., 0.1, 100)
-  yerr = ones(100)*0.01
-  
-  # Exponential decay model
-  edf = fuf.ExpDecayFit1d()
-  
-  # Define free quantities
-  edf.thaw(["A", "tau", "off", "t0"])
-  # Let the amplitude be positive
-  edf.setRestriction({"A":[0.0,None]})
-  # Define initial guess
-  edf.assignValue({"A":1.0, "tau": 15., "off":0.2, "t0":50.})
-  
-  # Do not use chi square, but the linear deviation from model
-  # to evaluate quality of fit.
-  # Use the "MiniFunc" decorator to define your custom objective
-  # function. This decorator takes the fitting object as an
-  # argument. The function has to accept two arguments: the
-  # fitting object and the list of free parameters.
-  @fuf.MiniFunc(edf)
-  def mini(edf, P):
-    m = sum(abs(edf.model - edf.y)/edf.yerr)
-    print "mini - current parameters: ", P, ", value is: ", m
-    return m
-  
-  # Carry out fit WITH SELF-DEFINED OBJECTIVE FUNCTION
-  edf.fit(x, y, yerr=yerr, miniFunc=mini)
-  
-  # Show parameter values and plot best-fit model.
-  edf.parameterSummary()
-  mpl.errorbar(x,y,yerr)
-  mpl.plot(x, edf.model, 'r-')
-  mpl.show()
+    # Import numpy and matplotlib
+    from numpy import arange, exp, random, ones, sum, abs
+    import matplotlib.pylab as plt
+    # Import funcFit
+    from PyAstronomy import funcFit as fuf
+    
+    # Define parameters of faked data
+    A = 1.0
+    tau = 10.
+    off = 0.2
+    t0 = 40.
+    
+    # Caculate fake data set
+    x = arange(100)
+    y = A*exp(-(x-t0)/tau) * (x>t0) + off
+    y += random.normal(0., 0.1, 100)
+    yerr = ones(100)*0.01
+    
+    # Exponential decay model
+    edf = fuf.ExpDecayFit1d()
+    
+    # Define free quantities
+    edf.thaw(["A", "tau", "off", "t0"])
+    # Let the amplitude be positive
+    edf.setRestriction({"A":[0.0,None]})
+    # Define initial guess
+    edf.assignValue({"A":1.0, "tau": 15., "off":0.2, "t0":50.})
+    
+    # Do not use chi square, but the linear deviation from model
+    # to evaluate quality of fit.
+    # Use the "MiniFunc" decorator to define your custom objective
+    # function. This decorator takes the fitting object as an
+    # argument. The function has to accept two arguments: the
+    # fitting object and the list of free parameters.
+    @fuf.MiniFunc(edf)
+    def mini(edf, P):
+      m = sum(abs(edf.model - edf.y)/edf.yerr)
+      print "mini - current parameters: ", P, ", value is: ", m
+      return m
+    
+    # Carry out fit WITH SELF-DEFINED OBJECTIVE FUNCTION
+    edf.fit(x, y, yerr=yerr, miniFunc=mini)
+    
+    # Show parameter values and plot best-fit model.
+    edf.parameterSummary()
+    plt.errorbar(x,y,yerr)
+    plt.plot(x, edf.model, 'r-')
+    plt.show()
 
 Some points may be highlighted in this example:
   * You may have noticed that although the parameter `P` is given to the *mini* function, it is not
     used there. You cannot leave it out, however, because the decorator, in fact, creates a more complex
     object, which needs this information.
   * The penalty assignment (for restricted parameters) is done automatically. You do not have
     to include it in your objective function.
   * The custom objective function has to be specified on call to the fit routine (*miniFunc* keyword).
 
-.. _tutMCMCSampler:
-
-Using the Markov-Chain Monte-Carlo (MCMC) sampler
-----------------------------------------------------
-
-The *fitMCMC* method provided by funcFit is not an MCMC sampler itself, but, similar to
-the *fit* method, it is a wrapper around functionality provided by a third party package,
-namely, PyMC_.
-
-pymc is a powerful Python package providing a wealth of functionality concerning Bayesian
-analysis. *fitMCMC* provides an easy to use interface to pymc sampling, which
-allows to carry out a basic Bayesian data analysis quickly. We note that despite the
-method name *fitMCMC* fitting is not the exact purpose of the analysis
-carried out here, but sampling from the posterior.
-
-The following example demonstrates
-how the funcFit interface can be used to carry out a Bayesian analysis using pymc.
-For a deeper understanding of the working, adaptability, and logic implemented by
-pymc, we refer the reader to their web page (PyMC_).
-
-.. note:: To run this example, pymc must be installed (check the output of funcFit.status() shown at the beginning
-          of this tutorial to see whether this is the case on your system).
-
-::
-
-  # Import some required modules
-  from numpy import arange, sqrt, exp, pi, random, ones
-  import matplotlib.pylab as mpl
-  import pymc
-  # ... and now the funcFit package
-  from PyAstronomy import funcFit as fuf
-  
-  # Creating a Gaussian with some noise
-  # Choose some parameters...
-  gPar = {"A":-5.0, "sig":10.0, "mu":10.0, "off":1.0, "lin":0.0}
-  # Calculate profile
-  x = arange(100) - 50.0
-  y = gPar["off"] + gPar["A"] / sqrt(2*pi*gPar["sig"]**2) \
-  * exp(-(x-gPar["mu"])**2/(2*gPar["sig"]**2))
-  # Add some noise
-  y += random.normal(0.0, 0.01, x.size)
-  
-  # Now let us come to the fitting
-  # First, we create the Gauss1d fit object
-  gf = fuf.GaussFit1d()
-  # See what parameters are available
-  print "List of available parameters: ", gf.availableParameters()
-  # Set guess values for the parameters
-  gf["A"] = -10.0
-  gf["sig"] = 15.77
-  gf["off"] = 0.87
-  gf["mu"] = 7.5
-  # Let us see whether the assignment worked
-  print "Parameters and guess values: ", gf.parameters()
-  
-  # Which parameters shall be variable during the fit?
-  # 'Thaw' those (the order is irrelevant)
-  gf.thaw(["A", "sig", "off", "mu"])
-  
-  # Let us assume that we know that the amplitude is negative, i.e.,
-  # no lower boundary (None) and 0.0 as upper limit.
-  gf.setRestriction({"A":[None,0.0]})
-  
-  # Now start a simplex fit
-  gf.fit(x,y,yerr=ones(x.size)*0.01)
-  
-  # Obtain the best-fit values derived by the simplex fit.
-  # They are to be used as start values for the MCMC sampling.
-  # Note that 'A' is missing - we will introduce this later.
-  X0 = {"sig":gf["sig"], "off":gf["off"], "mu":gf["mu"]}
-  
-  # Now we specify the limits within which the individual parameters
-  # can be varied (for those parameters listed in the 'X0' dictionary).
-  Lims = {"sig":[-20.,20.], "off":[0.,2.], "mu":[5.,15.]}
-  
-  # For the parameters contained in 'X0', define the step widths, which
-  # are to be used by the MCMC sampler. The steps are specified using
-  # the same scale/units as the actual parameters.
-  steps = {"A":0.01, "sig":0.1, "off":0.1, "mu":0.1}
-  
-  # In this example, we wish to define our ``own'' PyMC variable for the parameter
-  # 'A'. This can be useful, if nonstandard behavior is desired. Note that this
-  # is an optional parameter and you could simply include the parameter 'A' into
-  # The framework of X0, Lims, and steps.
-  ppa = {}
-  ppa["A"] = pymc.Uniform("A", value=gf["A"], lower=-20., \
-                          upper=10.0, doc="Amplitude")
-  
-  # Start the sampling. The resulting Marchov-Chain will be written
-  # to the file 'mcmcExample.tmp'. In default configuration, pickle
-  # is used to write that file.
-  # To save the chain to a compressed 'hdf5'
-  # file, you have to specify the dbArgs keyword; e.g., use:
-  #   dbArgs = {"db":"hdf5", "dbname":"mcmcExample.hdf5"}
-  gf.fitMCMC(x, y, X0, Lims, steps, yerr=ones(x.size)*0.01, \
-             pymcPars=ppa, iter=2500, burn=0, thin=1, \
-             dbfile="mcmcExample.tmp")
-  
-  # Reload the database (here, this is actually not required, but it is
-  # if the Marchov chain is to be analyzed later).
-  db = pymc.database.pickle.load('mcmcExample.tmp')
-  # Plot the trace of the amplitude, 'A'.
-  mpl.hist(db.trace("A", 0)[:])
-  mpl.show()
-
-Some points shall be emphasized in this example:
- * For MCMC sampling the exact same fit object is used as for "normal" fitting.
- * If the *yerr* keyword is specified in the call to fitMCMC, a Gaussian distribution is
-   assumed for the data points. Otherwise a Poisson distribution is assumed.
- * We used the normal simplex fit to obtain starting values for the Markov chain. You may also
-   use, e.g., burn-in.
- * In the example, we demonstrated how a uniformly distributed PyMC variable is created. Normally,
-   the fitMCMC method does this for you.
- * The result, i.e., the Markov chain, is saved to the file mcmcExample.tmp and is reloaded to
-   obtain the trace of the amplitude.
-
-.. note:: A convenient analysis of the resulting traces can be carried out using the *TraceAnalysis*
-          class (see :ref:`traceAnalysisClass`)
-
-We emphasize that PyMC is a powerful and highly adaptable package, which can do a lot more. A more
-detailed introduction is, however, beyond the scope of this tutorial.
-
------------------------------
-
-Occasionally, it can become cumbersome to define the starting values, steps,
-and ranges for uniform priors as done in the above example.
-Using the "auto" methods defined in the fitting class, you can take a short
-cut. Be, however, warned:
-
-.. warning:: There is NO guarantee that the auto functions produce reasonable
-             results. You need to check that.
-             
-::
-
-  from PyAstronomy import funcFit as fuf
-  import numpy as np
-  import matplotlib.pylab as plt
-  
-  x = np.linspace(0,30,1000)
-  gauss = fuf.GaussFit1d()
-  gauss["A"] = 1
-  gauss["mu"] = 23.
-  gauss["sig"] = 0.5
-  # Generate some "data" to fit
-  yerr = np.random.normal(0., 0.05, len(x))
-  y = gauss.evaluate(x) + yerr
-  # Thaw the parameters A, mu, and sig
-  gauss.thaw(["A","mu","sig"])
-  
-  # Define the ranges, which are used to construct the
-  # uniform priors and step sizes.
-  # Note that for "sig", we give only a single value.
-  # In this case, the limits for the uniform prior will
-  # be constructed as [m0-1.5, m0+1.5], where m0 is the
-  # starting value interpreted as the current value of
-  # mu (23. in this case).
-  ranges = {"A":[0,10],"mu":3, "sig":[0.1,1.0]}
-  # Generate default input for X0, lims, and steps
-  X0, lims, steps = gauss.MCMCautoParameters(ranges)
-  
-  # Show what happened...
-  print
-  print "Auto-generated input parameters:"
-  print "X0: ", X0
-  print "lims: ", lims
-  print "steps: ", steps
-  print
-  # Call the usual sampler
-  gauss.fitMCMC(x, y, X0, lims, steps, yerr=yerr, iter=1000)
-  
-  # and plot the results
-  plt.plot(x, y, 'k+')
-  plt.plot(x, gauss.evaluate(x), 'r--')
-  plt.show()
-
-
-You may even shorten the short-cut by using the `autoFitMCMC` method.
-**However, note that the same warning remains valid here.**
-
-::
-
-  from PyAstronomy import funcFit as fuf
-  import numpy as np
-  import matplotlib.pylab as plt
-  
-  x = np.linspace(0,30,1000)
-  gauss = fuf.GaussFit1d()
-  gauss["A"] = 1
-  gauss["mu"] = 23.
-  gauss["sig"] = 0.5
-  # Generate some "data" to fit
-  yerr = np.random.normal(0., 0.05, len(x))
-  y = gauss.evaluate(x) + yerr
-  
-  # Define the ranges, which are used to construct the
-  # uniform priors and step sizes.
-  # Note that for "sig", we give only a single value.
-  # In this case, the limits for the uniform prior will
-  # be constructed as [m0-1.5, m0+1.5], where m0 is the
-  # starting value interpreted as the current value of
-  # mu (23. in this case).
-  ranges = {"A":[0,10],"mu":3, "sig":[0.1,1.0]}
-  
-  # Call the auto-sampler
-  # Note that we set picky to False here. In this case, the
-  # parameters specified in ranges will be thawed automatically.
-  # All parameters not mentioned there, will be frozen.
-  gauss.autoFitMCMC(x, y, ranges, yerr=yerr, picky=False, iter=1000)
-  
-  # and plot the results
-  plt.plot(x, y, 'k+')
-  plt.plot(x, gauss.evaluate(x), 'r--')
-  plt.show()
-
-
-MCMC sampling with Gaussian and uniform priors
-----------------------------------------------
-
-The use of prior information is inherent in Bayesian analyses. The
-following example demonstrates how prior information can explicitly
-be included in the sampling. We note, however, that some kind of prior
-is implicitly assumed for all parameters; in this case, a uniform one.
-
-::
-
-  from PyAstronomy import funcFit as fuf
-  import numpy as np
-  import matplotlib.pylab as plt
-  import pymc
-  
-  # Create a Gauss-fit object
-  gf = fuf.GaussFit1d()
-  
-  # Choose some parameters
-  gf["A"] = -0.65
-  gf["mu"] = 1.0
-  gf["lin"] = 0.0
-  gf["off"] = 1.1
-  gf["sig"] = 0.2
-  
-  # Simulate data with noise
-  x = np.linspace(0., 2., 100)
-  y = gf.evaluate(x)
-  y += np.random.normal(0, 0.05, len(x))
-  
-  gf.thaw(["A", "off", "mu", "sig"])
-  
-  # Set up a normal prior for the offset parameter
-  # Note!---The name (first parameter) must correspond to that
-  #         of the parameter.
-  # The expectation value us set to 0.9 while the width is given
-  # as 0.01 (tau = 1/sigma**2). The starting value is specified
-  # as 1.0.
-  offPar = pymc.Normal("off", mu=0.9, tau=(1./0.01)**2, value=1.0)
-  # Use a uniform prior for mu.
-  muPar = pymc.Uniform("mu", lower=0.95, upper=0.97, value=0.96)
-  
-  # Collect the "extra"-variables in a dictionary using
-  # their names as keys
-  pymcPars = {"mu":muPar, "off":offPar}
-  
-  # Specify starting values, X0, and limits, lims, for
-  # those parameter distributions not given specifically.
-  X0 = {"A":gf["A"], "sig":gf["sig"]}
-  lims = {"A":[-1.0,0.0], "sig":[0., 1.0]}
-  # Still, the steps dictionary has to contain all
-  # parameter distributions.
-  steps = {"A":0.02, "sig":0.02, "mu":0.01, "off":0.01}
-  
-  # Carry out the MCMC sampling
-  gf.fitMCMC(x, y, X0, lims, steps, yerr=np.ones(len(x))*0.05, \
-             pymcPars=pymcPars, burn=1000, iter=3000)
-  
-  # Setting parameters to mean values
-  for p in gf.freeParameters():
-    gf[p] = gf.MCMC.trace(p)[:].mean()
-  
-  # Show the "data" and model in the upper panel
-  plt.subplot(2,1,1)
-  plt.title("Data and model")
-  plt.errorbar(x, y, yerr=np.ones(len(x))*0.05, fmt="bp")
-  # Plot lowest deviance solution
-  plt.plot(x, gf.evaluate(x), 'r--')
-  
-  # Show the residuals in the lower panel
-  plt.subplot(2,1,2)
-  plt.title("Residuals")
-  plt.errorbar(x, y-gf.evaluate(x), yerr=np.ones(len(x))*0.05, fmt="bp")
-  plt.plot([min(x), max(x)], [0.0,0.0], 'r-')
-  
-  plt.show()
-
-Clearly, the plot shows that the solution fits not very well, because the prior
-information has a significant influence on the outcome. Whether this remains
-reasonable or not is not a question for the sampler, however. 
 
 Using an overbinned model 
 -----------------------------
 
 In some cases it may be necessary to evaluate a model at more points than actually required by, e.g.,
 an observation. The final model is than obtained by averaging a number of points. This may be
 necessary to take finite integration times of your instrument into account as can be the case
 in planetary transit modeling.
 
 The *turnIntoRebin* method of funcFit provides a convenient way to work with
 such "overbinned" models; a demonstration is given in the example below.
 
 ::
 
-  # Import numpy and matplotlib
-  from numpy import arange, sqrt, exp, pi, random, ones
-  import matplotlib.pylab as mpl
-  # ... and now the funcFit package
-  from PyAstronomy import funcFit as fuf
-  
-  # Creating a Gaussian with some noise
-  # Choose some parameters...
-  gPar = {"A":-5.0, "sig":10.0, "mu":10.0, "off":1.0, "lin":0.0}
-  # Calculate profile
-  x = arange(20)/20.0 * 100.0 - 50.0
-  y = gPar["off"] + gPar["A"] / sqrt(2*pi*gPar["sig"]**2) \
-      * exp(-(x-gPar["mu"])**2/(2*gPar["sig"]**2))
-  # Add some noise
-  y += random.normal(0.0, 0.01, x.size)
-  # Let us see what we have done...
-  mpl.plot(x, y, 'bp')
-  
-  # First, we create a "GaussFit1d_Rebin" class object (note that the
-  # class object has still to be instantiated, the name is arbitrary).
-  GaussFit1d_Rebin = fuf.turnIntoRebin(fuf.GaussFit1d)
-  # Do the instantiation and specify how the overbinning should be
-  # carried out.
-  gf = GaussFit1d_Rebin()
-  gf.setRebinArray_Ndt(x, 10, x[1]-x[0])
-  # See what parameters are available
-  print "List of available parameters: ", gf.availableParameters()
-  # Set guess values for the parameters
-  gf["A"] = -10.0
-  gf["sig"] = 15.77
-  gf["off"] = 0.87
-  gf["mu"] = 7.5
-  # Let us see whether the assignment worked
-  print "Parameters and guess values: "
-  print "  A   : ", gf["A"]
-  print "  sig : ", gf["sig"]
-  print "  off : ", gf["off"]
-  print "  mu  : ", gf["mu"]
-  print ""
-  
-  # Now some of the strengths of funcFit are demonstrated; namely, the
-  # ability to consider some parameters as free and others as fixed.
-  # By default, all parameters of the GaussFit1d are frozen.
-  
-  # Show values and names of frozen parameters
-  print "Names and values if FROZEN parameters: ", gf.frozenParameters()
-  
-  # Which parameters shall be variable during the fit?
-  # 'Thaw' those (the order is irrelevant)
-  gf.thaw(["A", "sig", "off", "mu"])
-  
-  # Let us assume that we know that the amplitude is negative, i.e.,
-  # no lower boundary (None) and 0.0 as upper limit.
-  gf.setRestriction({"A":[None,0.0]})
-  
-  # Now start the fit
-  gf.fit(x, y, yerr=ones(x.size)*0.01)
-  
-  # Write the result to the screen and plot the best fit model
-  gf.parameterSummary()
-  # Plot the final best-fit model
-  mpl.plot(x, gf.model, 'rp--')
-  # Show the overbinned (=unbinned) model, indicate by color
-  # which point are averaged to obtain a point in the binned
-  # model.
-  for k, v in gf.rebinIdent.iteritems():
-    c = "y"
-    if k % 2 == 0: c = "k"
-    mpl.plot(gf.rebinTimes[v], gf.unbinnedModel[v], c+'.')
-  
-  # Show the data and the best fit model
-  mpl.show()
+    # Import numpy and matplotlib
+    from numpy import arange, sqrt, exp, pi, random, ones
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
+    from PyAstronomy import funcFit as fuf
+    
+    # Creating a Gaussian with some noise
+    # Choose some parameters...
+    gPar = {"A":-5.0, "sig":10.0, "mu":10.0, "off":1.0, "lin":0.0}
+    # Calculate profile
+    x = arange(20)/20.0 * 100.0 - 50.0
+    y = gPar["off"] + gPar["A"] / sqrt(2*pi*gPar["sig"]**2) \
+        * exp(-(x-gPar["mu"])**2/(2*gPar["sig"]**2))
+    # Add some noise
+    y += random.normal(0.0, 0.01, x.size)
+    # Let us see what we have done...
+    plt.plot(x, y, 'bp')
+    
+    # First, we create a "GaussFit1d_Rebin" class object (note that the
+    # class object has still to be instantiated, the name is arbitrary).
+    GaussFit1d_Rebin = fuf.turnIntoRebin(fuf.GaussFit1d)
+    # Do the instantiation and specify how the overbinning should be
+    # carried out.
+    gf = GaussFit1d_Rebin()
+    gf.setRebinArray_Ndt(x, 10, x[1]-x[0])
+    # See what parameters are available
+    print "List of available parameters: ", gf.availableParameters()
+    # Set guess values for the parameters
+    gf["A"] = -10.0
+    gf["sig"] = 15.77
+    gf["off"] = 0.87
+    gf["mu"] = 7.5
+    # Let us see whether the assignment worked
+    print "Parameters and guess values: "
+    print "  A   : ", gf["A"]
+    print "  sig : ", gf["sig"]
+    print "  off : ", gf["off"]
+    print "  mu  : ", gf["mu"]
+    print ""
+    
+    # Now some of the strengths of funcFit are demonstrated; namely, the
+    # ability to consider some parameters as free and others as fixed.
+    # By default, all parameters of the GaussFit1d are frozen.
+    
+    # Show values and names of frozen parameters
+    print "Names and values if FROZEN parameters: ", gf.frozenParameters()
+    
+    # Which parameters shall be variable during the fit?
+    # 'Thaw' those (the order is irrelevant)
+    gf.thaw(["A", "sig", "off", "mu"])
+    
+    # Let us assume that we know that the amplitude is negative, i.e.,
+    # no lower boundary (None) and 0.0 as upper limit.
+    gf.setRestriction({"A":[None,0.0]})
+    
+    # Now start the fit
+    gf.fit(x, y, yerr=ones(x.size)*0.01)
+    
+    # Write the result to the screen and plot the best fit model
+    gf.parameterSummary()
+    # Plot the final best-fit model
+    plt.plot(x, gf.model, 'rp--')
+    # Show the overbinned (=unbinned) model, indicate by color
+    # which point are averaged to obtain a point in the binned
+    # model.
+    for k, v in gf.rebinIdent.iteritems():
+      c = "y"
+      if k % 2 == 0: c = "k"
+      plt.plot(gf.rebinTimes[v], gf.unbinnedModel[v], c+'.')
+    
+    # Show the data and the best fit model
+    plt.show()
 
 This example is very similar to the very first one. Some differences shall, however, be
 emphasized:
   * Obtaining the model:
     In this example, we used a model that we called *GaussFit1d_Rebin*. 
     We created the model by calling the *turnIntoRebin* method giving
     GaussFit1d (by name NOT instance, i.e., we use the class object) as the parameter. The return value of this function is another class object,
@@ -1270,89 +988,91 @@
 
 The following example demonstrates how the *SyncFitContainer* class can be used
 to fit two different models with a partly overlapping parameter set, but differing
 x-axes simultaneously.
  
 ::
  
-  from PyAstronomy import funcFit as fuf
-  import numpy
-  import matplotlib.pylab as mpl
-  
-  # Set up two different x axes.
-  x1 = numpy.arange(100.)/100. - 0.5
-  x2 = numpy.arange(150.)/150. - 0.25
-  
-  # Getting the models ...
-  gauss = fuf.GaussFit1d()
-  calor = fuf.CauchyLorentz1d()
-  # and assign parameters.
-  gauss.assignValue({"A":0.02, "sig":0.1, "mu":0.0, "off":1.0, "lin":0.0})
-  calor.assignValue({"A":0.07, "g":0.1, "mu":0.2, "off":1.0, "lin":0.0})
-  
-  # Create noisy data.
-  y1 = gauss.evaluate(x1) + numpy.random.normal(0., 0.01, 100)
-  y2 = calor.evaluate(x2) + numpy.random.normal(0., 0.01, 150)
-  
-  # Plot the noisy data.
-  mpl.subplot(2,1,1)
-  mpl.errorbar(x1, y1, yerr=numpy.ones(100)*0.01)
-  mpl.subplot(2,1,2)
-  mpl.errorbar(x2, y2, yerr=numpy.ones(150)*0.01)
-  
-  # Now, get ready two fit the data sets simultaneously.
-  sf = fuf.SyncFitContainer()
-  # Tell the class about the two components and save the
-  # component numbers assigned to them:
-  gaussCno = sf.addComponent(gauss)
-  calorCno = sf.addComponent(calor)
-  
-  print "Component numbers in the syncFit container:"
-  print "  Gauss: ", gaussCno, ",  Cauchy-Lorentz: ", calorCno
-  print
-  
-  # See what happened to the parameters in the
-  # simultaneous fitting class.
-  # The variable names have changed.
-  sf.parameterSummary()
-  
-  # Thaw all parameters (for later fit) ...
-  sf.thaw(sf.parameters().keys())
-  # but not the linear term.
-  sf.freeze(["lin_Gaussian[s1]", "lin_CauLor[s2]"])
-  
-  # Tell the class about the identity of parameters,
-  # either by using the "property name" of the parameter:
-  sf.treatAsEqual("off")
-  # or by specifying the names explicitly.
-  sf.treatAsEqual(["g_CauLor[s2]", "sig_Gaussian[s1]"])
-  
-  # See what happened to the parameters in the
-  # simultaneous fitting class.
-  print
-  print "Parameters after 'treatAsEqual' has been applied:"
-  sf.parameterSummary()
-  
-  # Randomize starting values.
-  for fp in sf.freeParamNames():
-    sf[fp] = sf[fp] + numpy.random.normal(0., 0.05)
-  
-  # Set up the data appropriately.
-  data = {gaussCno:[x1, y1], calorCno:[x2, y2]}
-  yerr = {gaussCno: numpy.ones(100)*0.01, \
-          calorCno: numpy.ones(150)*0.01}
-  
-  # Start the fit.
-  sf.fit(data, yerr=yerr)
-  
-  # Show the best-fit values.
-  print
-  print "Best-fit parameters:"
-  sf.parameterSummary()
-  
-  # Plot the best-fit model(s).
-  mpl.subplot(2,1,1)
-  mpl.plot(x1, sf.models[gaussCno], 'r--')
-  mpl.subplot(2,1,2)
-  mpl.plot(x2, sf.models[calorCno], 'r--')
-  
-  mpl.show()
+    from PyAstronomy import funcFit as fuf
+    import numpy
+    import matplotlib.pylab as plt
+    
+    # Set up two different x axes.
+    x1 = numpy.arange(100.)/100. - 0.5
+    x2 = numpy.arange(150.)/150. - 0.25
+    
+    # Getting the models ...
+    gauss = fuf.GaussFit1d()
+    calor = fuf.CauchyLorentz1d()
+    # and assign parameters.
+    gauss.assignValue({"A":0.02, "sig":0.1, "mu":0.0, "off":1.0, "lin":0.0})
+    calor.assignValue({"A":0.07, "g":0.1, "mu":0.2, "off":1.0, "lin":0.0})
+    
+    # Create noisy data.
+    y1 = gauss.evaluate(x1) + numpy.random.normal(0., 0.01, 100)
+    y2 = calor.evaluate(x2) + numpy.random.normal(0., 0.01, 150)
+    
+    # Plot the noisy data.
+    plt.subplot(2,1,1)
+    plt.errorbar(x1, y1, yerr=numpy.ones(100)*0.01)
+    plt.subplot(2,1,2)
+    plt.errorbar(x2, y2, yerr=numpy.ones(150)*0.01)
+    
+    # Now, get ready two fit the data sets simultaneously.
+    sf = fuf.SyncFitContainer()
+    # Tell the class about the two components and save the
+    # component numbers assigned to them:
+    gaussCno = sf.addComponent(gauss)
+    calorCno = sf.addComponent(calor)
+    
+    print "Component numbers in the syncFit container:"
+    print "  Gauss: ", gaussCno, ",  Cauchy-Lorentz: ", calorCno
+    print
+    
+    # See what happened to the parameters in the
+    # simultaneous fitting class.
+    # The variable names have changed.
+    sf.parameterSummary()
+    
+    # Thaw all parameters (for later fit) ...
+    sf.thaw(sf.parameters().keys())
+    # but not the linear term.
+    sf.freeze(["lin_Gaussian[s1]", "lin_CauLor[s2]"])
+    
+    # Tell the class about the identity of parameters,
+    # either by using the "property name" of the parameter:
+    sf.treatAsEqual("off")
+    # or by specifying the names explicitly.
+    sf.treatAsEqual(["g_CauLor[s2]", "sig_Gaussian[s1]"])
+    
+    # See what happened to the parameters in the
+    # simultaneous fitting class.
+    print
+    print "Parameters after 'treatAsEqual' has been applied:"
+    sf.parameterSummary()
+    
+    # Randomize starting values.
+    for fp in sf.freeParamNames():
+      sf[fp] = sf[fp] + numpy.random.normal(0., 0.05)
+    
+    # Set up the data appropriately.
+    data = {gaussCno:[x1, y1], calorCno:[x2, y2]}
+    yerr = {gaussCno: numpy.ones(100)*0.01, \
+            calorCno: numpy.ones(150)*0.01}
+    
+    # Start the fit.
+    sf.fit(data, yerr=yerr)
+    
+    # Show the best-fit values.
+    print
+    print "Best-fit parameters:"
+    sf.parameterSummary()
+    
+    # Plot the best-fit model(s).
+    plt.subplot(2,1,1)
+    plt.plot(x1, sf.models[gaussCno], 'r--')
+    plt.subplot(2,1,2)
+    plt.plot(x2, sf.models[calorCno], 'r--')
+    
+    plt.show()
+
+
```

### Comparing `PyAstronomy-0.8.1/src/doc/funcFitDoc/modelRebin.rst` & `PyAstronomy-0.9.0/src/doc/funcFitDoc/modelRebin.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/funcFitDoc/traceAnalysisTutorial.rst` & `PyAstronomy-0.9.0/src/doc/funcFitDoc/traceAnalysisTutorial.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _traceAnalysisTut:
+
 Analyze Markov-Chains using `TraceAnalysis`
 =============================================
 
 .. currentmodule:: PyAstronomy.funcFit
 
 After having using `pymc`, e.g., via PyAstronomy's
 wrapper `fitMCMC` and having created a Markov Chain,
@@ -16,74 +18,91 @@
 -------------------------------------
 
 The following example demonstrates how to **create
 the Markov-Chain**, which will later be analyzed. 
 
 ::
 
-  import numpy as np
-  import matplotlib.pylab as plt
-  # ... and now the funcFit package
-  from PyAstronomy import funcFit as fuf
-  
-  # Starting from with Voigt profile
-  vp = fuf.Voigt1d()
-  # Set some values to create a model
-  vp["A"] = -0.4
-  vp["al"] = 0.7
-  vp["mu"] = 5500.
-  vp["ad"] = 0.3
-  vp["off"] = 1.0
-  
-  x = np.linspace(5490., 5510., 200)
-  # Create our data with some noise
-  yerr = np.ones(len(x))*0.01
-  y = vp.evaluate(x) + np.random.normal(0.0, 0.01, len(x))
-  
-  # Say, we have a guess of the parameters, which is, however,
-  # not entirely correct
-  vp["A"] = -0.376
-  vp["al"] = 0.9
-  vp["mu"] = 5499.7
-  vp["ad"] = 0.4
-  vp["off"] = 1.0
-  
-  # Plot the data and our guess
-  plt.errorbar(x, y, yerr=yerr, fmt='b.-')
-  plt.plot(x, vp.evaluate(x), 'r--')
-  plt.show()
-  
-  # Thaw the parameters, which we wish to vary
-  # during the sampling
-  vp.thaw(["A", "al", "mu", "ad"])
-  
-  # Use current parameters as starting point for the sampling
-  X0 = vp.freeParameters()
-  print "Starting point for sampling: ", X0
-  
-  # Now we specify the limits within which the individual parameters
-  # can be varied. Actually, you specify the limits of uniform priors
-  # here.
-  lims = {"A":[-1.0,0.0], "al":[0.0,3.], "ad":[0.0,3.0], "mu":[5495., 5505.]}
-  
-  # Provide a guess for the proposal step widths.
-  # Try to guess the scale of the problem in the individual
-  # parameters.
-  steps = {"A":0.02, "al":0.01, "ad":0.01, "mu":0.05}
-  
-  # Start the sampling. The resulting Marchov-Chain will be written
-  # to the file 'mcmcTA.tmp'. In default configuration, pickle
-  # is used to write that file.
-  # To save the chain to a compressed 'hdf5'
-  # file, you have to specify the dbArgs keyword; e.g., use:
-  #   dbArgs = {"db":"hdf5", "dbname":"mcmcExample.hdf5"}
-  vp.fitMCMC(x, y, X0, lims, steps, yerr=yerr, \
-             iter=2500, burn=0, thin=1, \
-             dbfile="mcmcTA.tmp")
-
+    # Import some required modules
+    import numpy as np
+    import matplotlib.pylab as plt
+    # ... and now the funcFit package
+    from PyAstronomy import funcFit as fuf
+    
+    # Starting from with Voigt profile
+    vp = fuf.Voigt1d()
+    # Set some values to create a model
+    vp["A"] = -0.4
+    vp["al"] = 0.7
+    vp["mu"] = 5500.
+    vp["ad"] = 0.3
+    vp["off"] = 1.0
+    
+    x = np.linspace(5490., 5510., 200)
+    # Create our data with some noise
+    yerr = np.ones(len(x))*0.01
+    y = vp.evaluate(x) + np.random.normal(0.0, 0.01, len(x))
+    
+    # Say, we have a guess of the parameters, which is, however,
+    # not entirely correct
+    vp["A"] = -0.376
+    vp["al"] = 0.9
+    vp["mu"] = 5499.7
+    vp["ad"] = 0.4
+    vp["off"] = 1.0
+    
+    # Plot the data and our guess
+    plt.errorbar(x, y, yerr=yerr, fmt='b.-')
+    plt.plot(x, vp.evaluate(x), 'r--')
+    plt.show()
+    
+    # Thaw the parameters, which we wish to vary
+    # during the sampling
+    vp.thaw(["A", "al", "mu", "ad"])
+    
+    # Use current parameters as starting point for the sampling
+    X0 = vp.freeParameters()
+    print "Starting point for sampling: ", X0
+    
+    
+    ##############################################################
+    ### Using pymc for sampling, for emcee see below
+    ##############################################################
+    
+    # Now we specify the limits within which the individual parameters
+    # can be varied. Actually, you specify the limits of uniform priors
+    # here.
+    lims = {"A":[-1.0,0.0], "al":[0.0,3.], "ad":[0.0,3.0], "mu":[5495., 5505.]}
+    
+    # Provide a guess for the proposal step widths.
+    # Try to guess the scale of the problem in the individual
+    # parameters.
+    steps = {"A":0.02, "al":0.01, "ad":0.01, "mu":0.05}
+    
+    # Start the sampling. The resulting Marchov-Chain will be written
+    # to the file 'mcmcTA.tmp'. In default configuration, pickle
+    # is used to write that file.
+    # To save the chain to a compressed 'hdf5'
+    # file, you have to specify the dbArgs keyword; e.g., use:
+    #   dbArgs = {"db":"hdf5", "dbname":"mcmcExample.hdf5"}
+    vp.fitMCMC(x, y, X0, lims, steps, yerr=yerr, \
+               iter=2500, burn=0, thin=1, \
+               dbfile="mcmcTA.tmp")
+    
+    ##############################################################
+    ### Uncomment to use emcee for sampling
+    ##############################################################           
+               
+    #priors = {"al":fuf.FuFPrior("limuniform", lower=0.0, upper=100.), \
+              #"ad":fuf.FuFPrior("limuniform", lower=0.0, upper=100.)}
+    
+    ## Note that the filename should end in .emcee. Substitute this filename
+    ## in the following examples.
+    #vp.fitEMCEE(x, y, yerr=yerr, sampleArgs={"iters":2500}, \
+                #dbfile="mcmcTA.emcee", priors=priors)
 
 Investigate convergence behavior using the "deviance"
 ------------------------------------------------------
 
 This example demonstrates how to investigate whether the
 chain has converged using the **deviance** and setting
 an appropriate **burn-in**.
```

### Comparing `PyAstronomy-0.8.1/src/doc/funcFitDoc/simplemodels.rst` & `PyAstronomy-0.9.0/src/doc/funcFitDoc/simplemodels.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/index.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/index.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/rotBroadProfile.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/rotBroadProfile.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/palRebin.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/palRebin.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/pal.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/pal.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/exams.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/exams.rst`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 -----------------------
 
 In this first example, we demonstrate how to calculate a model transit light-curve. 
 
 ::
 
   from PyAstronomy.modelSuite import palTrans
-  import matplotlib.pylab as mpl
-  import numpy
-
+  import matplotlib.pylab as plt
+  import numpy as np
+  
   # Create a PalLC instance
   plc = palTrans.PalLC()
   
   # Set parameter values
   plc["p"] = 0.1    # Planet radius / Stellar radius
   plc["per"] = 1.0  # Orbital period
   plc["a"] = 2.0    # Large semi major axis [R_S]
@@ -32,41 +32,41 @@
   # Specify binary contribution
   plc["b"] = 0.0
   
   # Check the parameters
   plc.parameterSummary()
   
   # Create a time axis
-  time = numpy.arange(1000)/1000.0 - 0.5
+  time = np.arange(1000)/1000.0 - 0.5
   
   # Calculate the light curve using above set
   # model parameters
   lightcurve = plc.evaluate(time)
   
   # Plot the result
-  mpl.plot(time, lightcurve, 'bp')
-  mpl.show()
+  plt.plot(time, lightcurve, 'bp')
+  plt.show()
 
 
 Fitting a transit
 ---------------------
 
 The leading half of this example is very similar to the first one; we only
 use a smaller number of point for the time axis. The second half demonstrates
 how the fitting interface is invoked (more examples using simpler models
 can are shown in the *funcFit tutorial*). 
 
 .. warning:: If you are using *mpmath* for evaluation of the elliptical integrals, the
              calculations will be quite slow.
 
 ::
-  
+   
   from PyAstronomy.modelSuite import palTrans
-  import matplotlib.pylab as mpl
-  import numpy
+  import matplotlib.pylab as plt
+  import numpy as np
   
   # Create a PalLC instance
   plc = palTrans.PalLC()
   
   # Set parameter values
   plc["p"] = 0.1    # Planet radius / Stellar radius
   plc["per"] = 1.0  # Orbital period
@@ -82,68 +82,69 @@
   plc["b"] = 0.0
   
   # Check the parameters
   print "Input parameters: "
   plc.parameterSummary()
   
   # Create a time axis
-  time = numpy.arange(100)/100.0 * 0.2 - 0.2
+  time = np.arange(100)/100.0 * 0.2 - 0.2
   
   # Calculate the light curve using above set
   # model parameters
   lc = plc.evaluate(time)
   
   # Save the result and add some noise
-  flux = lc + numpy.random.normal(0.0, 0.002, time.size)
+  flux = lc + np.random.normal(0.0, 0.002, time.size)
   
   # Now lets try to recover what we put in
   # Choose some "guess" parameters
-  plc["p"] = 0.12    # Planet radius / Stellar radius
+  plc["p"] = 0.1     # Planet radius / Stellar radius
   plc["per"] = 1.0   # Orbital period
-  plc["a"] = 7.0     # Large semi major axis [R_S]
+  plc["a"] = 7.5     # Large semi major axis [R_S]
   plc["i"] = 90.0    # Orbital inclination [deg]
   # Specify limb darkening
   # (quadratic limb-darkening law)
   plc["linLimb"] = 0.4
   plc["quadLimb"] = 0.2
   # Specify T0 (central time of transit)
   plc["T0"] = -0.08
   # Specify binary contribution
   plc["b"] = 0.0
   
   # Assume we want to fit "p", "a", "i", and "T0"
-  plc.thaw(["p", "a", "T0", "i"])
+  plc.thaw(["T0", "i"])
   
   # Before we start fitting, check how the elliptical integrals
   # are evaluated (mpmath or Boost)
   print "Which elliptical integrals are used?: ", plc.whichEllInts()
   
   # Carry out the fit
-  plc.fit(time, flux, yerr=numpy.ones(time.size)*0.002)
+  plc.fit(time, flux, yerr=np.ones(time.size)*0.002)
   
   print "Fit parameters: "
   plc.parameterSummary()
   
   # Plot the result
-  mpl.plot(time, flux, 'bp')
-  mpl.plot(time, plc.model, 'r-')
-  mpl.show()
+  plt.plot(time, flux, 'bp')
+  plt.plot(time, plc.model, 'r-')
+  plt.show()
 
+ 
 Obtain a model taking finite integration time into account
 -------------------------------------------------------------
 
 This example shows how to use the *PalLC_Rebin* class to take finite
 integration times and the resulting light-curve distortion into account.
 This example is very similar to the first one.
 
 ::
   
   from PyAstronomy.modelSuite import palTrans
-  import matplotlib.pylab as mpl
-  import numpy
+  import matplotlib.pylab as plt
+  import numpy as np
   
   # Create a PalLC_Rebin instance
   plc = palTrans.PalLC_Rebin()
   
   # Set parameter values
   plc["p"] = 0.1    # Planet radius / Stellar radius
   plc["per"] = 1.0  # Orbital period
@@ -158,23 +159,24 @@
   # Specify binary contribution
   plc["b"] = 0.0
   
   # Check the parameters
   plc.parameterSummary()
   
   # Create a time axis
-  time = numpy.arange(50)/50.0 - 0.51
+  time = np.arange(50)/50.0 - 0.51
   
   # Specify oversampling parameters.
   # Here use 10 points per observed bin.
   plc.setRebinArray_Ndt(time, 10, time[1]-time[0])
   
   # Calculate the light curve using above set
   # model parameters
   lc = plc.evaluate(time)
   
   # Plot the result (both the overbinned and final
   # model light-curves)
-  mpl.plot(plc.rebinTimes, plc.unbinnedModel, 'b.-')
-  mpl.plot(time, plc.binnedModel, 'rd--')
-  mpl.legend(["Overbinned LC", "Averaged LC"])
-  mpl.show()
+  plt.plot(plc.rebinTimes, plc.unbinnedModel, 'b.-')
+  plt.plot(time, plc.binnedModel, 'rd--')
+  plt.legend(["Overbinned LC", "Averaged LC"])
+  plt.show()
+
```

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/palTransDoc/boostsupport.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/palTransDoc/boostsupport.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/radVelDoc/radVel.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/radVelDoc/radVel.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/keplerEllipseModelDoc.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/keplerEllipseModelDoc.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/astroVoigt.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/astroVoigt.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/lineListGaussModelDoc.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/lineListGaussModelDoc.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/LyAProfile.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/LyAProfile.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/RmcLOhtaDoc/index.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/RmcLOhtaDoc/index.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/RmcLOhtaDoc/rmclExamples.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/RmcLOhtaDoc/rmclExamples.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/xtranDoc.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/xtranDoc.rst`

 * *Files identical despite different names*

### Comparing `PyAstronomy-0.8.1/src/doc/modelSuiteDoc/limBrightTrans.rst` & `PyAstronomy-0.9.0/src/doc/modelSuiteDoc/limBrightTrans.rst`

 * *Files identical despite different names*

