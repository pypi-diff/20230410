# Comparing `tmp/SimPEG-0.9.3.tar.gz` & `tmp/SimPEG-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SimPEG-0.9.3.tar", last modified: Mon Nov 19 17:07:44 2018, max compression
+gzip compressed data, was "dist/SimPEG-0.9.4.tar", last modified: Sun Dec  9 21:41:37 2018, max compression
```

## Comparing `SimPEG-0.9.3.tar` & `SimPEG-0.9.4.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6232 2018-11-19 17:07:44.000000 SimPEG-0.9.3/PKG-INFO
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG.egg-info/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6232 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG.egg-info/PKG-INFO
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4724 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG.egg-info/SOURCES.txt
--rw-r--r--   0 lindseyjh   (501) staff       (20)      136 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG.egg-info/requires.txt
--rw-r--r--   0 lindseyjh   (501) staff       (20)       13 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG.egg-info/top_level.txt
--rw-r--r--   0 lindseyjh   (501) staff       (20)        1 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG.egg-info/dependency_links.txt
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1089 2017-12-18 20:30:26.000000 SimPEG-0.9.3/LICENSE
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2758 2018-08-10 21:29:34.000000 SimPEG-0.9.3/CONTRIBUTING.rst
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/tests/
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/tests/seis/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1082 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/seis/test_tomo.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/seis/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/__init__.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/tests/utils/
--rw-r--r--   0 lindseyjh   (501) staff       (20)        0 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/utils/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2804 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/utils/test_printinfo.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/tests/pf/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1525 2018-08-13 22:29:38.000000 SimPEG-0.9.3/tests/pf/test_magnetics_IO.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1578 2018-08-13 22:29:38.000000 SimPEG-0.9.3/tests/pf/test_gravity_IO.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     5206 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/pf/test_mag_inversion_linear.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2000 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/pf/test_magnetics_analytics.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     3050 2018-08-13 22:29:38.000000 SimPEG-0.9.3/tests/pf/test_forward_Grav_Linear.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     3403 2018-08-13 22:29:38.000000 SimPEG-0.9.3/tests/pf/test_forward_Mag_Linear.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/pf/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1697 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/pf/test_forward_PFproblem.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     5192 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/pf/test_grav_inversion_linear.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    11447 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/pf/test_sensitivity_PFproblem.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/tests/base/
--rw-r--r--   0 lindseyjh   (501) staff       (20)    11642 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/base/test_utils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1828 2018-04-02 22:21:17.000000 SimPEG-0.9.3/tests/base/test_DataMisfit.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    13068 2018-11-19 01:28:05.000000 SimPEG-0.9.3/tests/base/test_maps.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    13632 2018-09-14 16:25:54.000000 SimPEG-0.9.3/tests/base/test_regularization.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2935 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/base/test_joint.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2863 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/base/test_SurveyAndData.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     7810 2017-12-18 23:17:14.000000 SimPEG-0.9.3/tests/base/test_Props.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     3906 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/base/test_directives.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2324 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/base/test_optimizers.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/base/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     9419 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/base/test_Objectivefct.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1751 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/base/test_Solver.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1727 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/base/test_coordutils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    16097 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/base/test_Fields.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1159 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/base/test_problem.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/tests/flow/
--rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.3/tests/flow/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6750 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/flow/test_Richards_empirical.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     8601 2018-08-10 21:29:34.000000 SimPEG-0.9.3/tests/flow/test_Richards.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)       22 2014-12-04 07:53:52.000000 SimPEG-0.9.3/MANIFEST.in
--rw-r--r--   0 lindseyjh   (501) staff       (20)      813 2016-02-11 00:13:44.000000 SimPEG-0.9.3/CITATION.rst
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1745 2018-11-19 17:07:29.000000 SimPEG-0.9.3/setup.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      848 2017-12-18 20:30:26.000000 SimPEG-0.9.3/AUTHORS.rst
--rw-r--r--   0 lindseyjh   (501) staff       (20)       38 2018-11-19 17:07:44.000000 SimPEG-0.9.3/setup.cfg
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4232 2018-11-03 02:23:34.000000 SimPEG-0.9.3/README.rst
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/NSEM/
--rw-r--r--   0 lindseyjh   (501) staff       (20)       28 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/NSEM/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2301 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/Inversion.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    14479 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/Survey.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/SEIS/
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/SEIS/StraightRay/
--rw-r--r--   0 lindseyjh   (501) staff       (20)      238 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/SEIS/StraightRay/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     3084 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/SEIS/StraightRay/StraightRayProblem.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      856 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/SEIS/StraightRay/StraightRaySurvey.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)       26 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/SEIS/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    99497 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/Maps.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    14027 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/ObjectiveFunction.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/VRM/
--rw-r--r--   0 lindseyjh   (501) staff       (20)    17385 2018-11-06 00:55:18.000000 SimPEG-0.9.3/SimPEG/VRM/WaveformVRM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2126 2018-11-06 00:55:18.000000 SimPEG-0.9.3/SimPEG/VRM/SurveyVRM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    36864 2018-11-06 00:55:18.000000 SimPEG-0.9.3/SimPEG/VRM/ProblemVRM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      222 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/VRM/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    13213 2018-11-06 00:55:18.000000 SimPEG-0.9.3/SimPEG/VRM/SrcVRM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     3076 2018-11-06 00:55:18.000000 SimPEG-0.9.3/SimPEG/VRM/RxVRM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1210 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/Models.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     9735 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/Fields.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6979 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/InvProblem.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     9251 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/SurveyNSEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    21456 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/FieldsNSEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    16323 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/ProblemNSEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      410 2018-03-02 18:15:07.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/__init__.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1364 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/MT1Dsolutions.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    18906 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/plotDataTypes.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4919 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/MT1Danalytic.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6614 2018-03-02 18:15:07.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/testUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      847 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     7680 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/sourceUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6927 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/ediFilesUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    16498 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/dataUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4746 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/data_viewer.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    29008 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/plotUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     9306 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/SrcNSEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    26166 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/NSEM/RxNSEM.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/TDEM/
--rw-r--r--   0 lindseyjh   (501) staff       (20)    19368 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/EM/TDEM/SrcTDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      281 2018-05-01 17:37:09.000000 SimPEG-0.9.3/SimPEG/EM/TDEM/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     7121 2018-05-01 17:37:09.000000 SimPEG-0.9.3/SimPEG/EM/TDEM/RxTDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1021 2018-05-01 17:37:09.000000 SimPEG-0.9.3/SimPEG/EM/TDEM/SurveyTDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    24101 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/EM/TDEM/FieldsTDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    36983 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/EM/TDEM/ProblemTDEM.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/FDEM/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1794 2018-05-01 17:37:09.000000 SimPEG-0.9.3/SimPEG/EM/FDEM/SurveyFDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    55216 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/FDEM/FieldsFDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    26247 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/FDEM/ProblemFDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      234 2018-05-01 17:37:09.000000 SimPEG-0.9.3/SimPEG/EM/FDEM/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    27542 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/FDEM/SrcFDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     5432 2018-08-15 23:24:37.000000 SimPEG-0.9.3/SimPEG/EM/FDEM/RxFDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      226 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/__init__.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/Utils/
--rw-r--r--   0 lindseyjh   (501) staff       (20)      304 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Utils/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     5799 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Utils/CurrentUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4489 2018-05-01 17:37:09.000000 SimPEG-0.9.3/SimPEG/EM/Utils/testingUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    12049 2018-06-26 22:23:41.000000 SimPEG-0.9.3/SimPEG/EM/Utils/AnalyticUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1772 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Utils/EMUtils.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/Static/
--rw-r--r--   0 lindseyjh   (501) staff       (20)       72 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Static/__init__.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/Static/Utils/
--rw-r--r--   0 lindseyjh   (501) staff       (20)    49374 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/Utils/StaticUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)       27 2017-12-19 05:06:13.000000 SimPEG-0.9.3/SimPEG/EM/Static/Utils/__init__.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/
--rw-r--r--   0 lindseyjh   (501) staff       (20)    15118 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/ProblemDC.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     5794 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/FieldsDC_2D.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2052 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/Run.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6947 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/BoundaryUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    13345 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/SurveyDC.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      461 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    20646 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/ProblemDC_2D.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    21738 2018-11-19 17:07:29.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/IODC.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1391 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/Utils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6928 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/FieldsDC.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6360 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/RxDC.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2298 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/DC/SrcDC.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/Static/SIP/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4829 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/SIP/Run.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    16462 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/SIP/ProblemSIP.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4640 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/SIP/SurveySIP.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      269 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/SIP/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     3466 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/SIP/RxSIP.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2142 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/SIP/SrcSIP.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    14200 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/SIP/ProblemSIP_2D.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/Static/IP/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2042 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/IP/Run.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     8506 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/IP/ProblemIP_2D.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      201 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/IP/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    10195 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/IP/ProblemIP.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1898 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Static/IP/SurveyIP.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    18936 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/EM/Base.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/EM/Analytics/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6656 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Analytics/DC.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      204 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Analytics/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    10268 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Analytics/FDEMDipolarfields.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      593 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Analytics/TDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4048 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Analytics/FDEMcasing.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4698 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Analytics/FDEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     5344 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/EM/Analytics/NSEM.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    36214 2018-08-13 22:29:38.000000 SimPEG-0.9.3/SimPEG/Optimization.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      740 2018-11-19 17:07:29.000000 SimPEG-0.9.3/SimPEG/__init__.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/Utils/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     7037 2018-08-12 04:48:05.000000 SimPEG-0.9.3/SimPEG/Utils/modelutils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     7794 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/Utils/printinfo.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     3207 2018-05-01 17:37:09.000000 SimPEG-0.9.3/SimPEG/Utils/CounterUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)       96 2017-12-18 23:17:14.000000 SimPEG-0.9.3/SimPEG/Utils/meshutils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)       59 2017-12-18 23:17:14.000000 SimPEG-0.9.3/SimPEG/Utils/curvutils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2379 2018-08-13 22:29:38.000000 SimPEG-0.9.3/SimPEG/Utils/matutils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    10959 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/Utils/ModelBuilder.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1027 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/Utils/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)       80 2017-12-18 23:17:14.000000 SimPEG-0.9.3/SimPEG/Utils/coordutils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6810 2018-10-24 20:10:13.000000 SimPEG-0.9.3/SimPEG/Utils/io_utils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     5303 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/Utils/SolverUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     6831 2018-11-19 17:07:29.000000 SimPEG-0.9.3/SimPEG/Utils/PlotUtils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     7341 2017-12-18 23:17:14.000000 SimPEG-0.9.3/SimPEG/Utils/codeutils.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    33407 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/Directives.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     8457 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/Problem.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/PF/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     5070 2018-08-13 22:29:38.000000 SimPEG-0.9.3/SimPEG/PF/BaseMag.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     1060 2018-08-13 22:29:38.000000 SimPEG-0.9.3/SimPEG/PF/GravAnalytics.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     9054 2018-08-13 22:29:38.000000 SimPEG-0.9.3/SimPEG/PF/GravityDriver.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      204 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/PF/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    14829 2018-08-13 22:29:38.000000 SimPEG-0.9.3/SimPEG/PF/Gravity.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    33553 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/PF/Magnetics.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    11448 2018-08-13 22:29:38.000000 SimPEG-0.9.3/SimPEG/PF/MagneticsDriver.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     2723 2018-08-13 22:29:38.000000 SimPEG-0.9.3/SimPEG/PF/BaseGrav.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     7637 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/PF/MagAnalytics.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/DC/
--rw-r--r--   0 lindseyjh   (501) staff       (20)       90 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/DC/__init__.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/SIP/
--rw-r--r--   0 lindseyjh   (501) staff       (20)       35 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/SIP/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    15924 2018-08-15 23:24:37.000000 SimPEG-0.9.3/SimPEG/Props.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)     4582 2018-11-19 01:28:05.000000 SimPEG-0.9.3/SimPEG/DataMisfit.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/IP/
--rw-r--r--   0 lindseyjh   (501) staff       (20)       34 2018-08-10 21:29:34.000000 SimPEG-0.9.3/SimPEG/IP/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    57743 2018-09-14 16:25:54.000000 SimPEG-0.9.3/SimPEG/Regularization.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/FLOW/
--rw-r--r--   0 lindseyjh   (501) staff       (20)       33 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/FLOW/__init__.py
-drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-11-19 17:07:44.000000 SimPEG-0.9.3/SimPEG/FLOW/Richards/
--rw-r--r--   0 lindseyjh   (501) staff       (20)     3985 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/FLOW/Richards/RichardsSurvey.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)      144 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/FLOW/Richards/__init__.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    11130 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/FLOW/Richards/RichardsProblem.py
--rw-r--r--   0 lindseyjh   (501) staff       (20)    27201 2017-12-18 20:30:26.000000 SimPEG-0.9.3/SimPEG/FLOW/Richards/Empirical.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6232 2018-12-09 21:41:37.000000 SimPEG-0.9.4/PKG-INFO
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG.egg-info/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6232 2018-12-09 21:41:36.000000 SimPEG-0.9.4/SimPEG.egg-info/PKG-INFO
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4724 2018-12-09 21:41:36.000000 SimPEG-0.9.4/SimPEG.egg-info/SOURCES.txt
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      136 2018-12-09 21:41:36.000000 SimPEG-0.9.4/SimPEG.egg-info/requires.txt
+-rw-r--r--   0 lindseyjh   (501) staff       (20)        7 2018-12-09 21:41:36.000000 SimPEG-0.9.4/SimPEG.egg-info/top_level.txt
+-rw-r--r--   0 lindseyjh   (501) staff       (20)        1 2018-12-09 21:41:36.000000 SimPEG-0.9.4/SimPEG.egg-info/dependency_links.txt
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1089 2017-12-18 20:30:26.000000 SimPEG-0.9.4/LICENSE
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2758 2018-08-10 21:29:34.000000 SimPEG-0.9.4/CONTRIBUTING.rst
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/tests/
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/tests/seis/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1082 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/seis/test_tomo.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/seis/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/__init__.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/tests/utils/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)        0 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/utils/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2804 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/utils/test_printinfo.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/tests/pf/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1525 2018-08-13 22:29:38.000000 SimPEG-0.9.4/tests/pf/test_magnetics_IO.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1578 2018-08-13 22:29:38.000000 SimPEG-0.9.4/tests/pf/test_gravity_IO.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     5206 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/pf/test_mag_inversion_linear.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2000 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/pf/test_magnetics_analytics.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     3050 2018-08-13 22:29:38.000000 SimPEG-0.9.4/tests/pf/test_forward_Grav_Linear.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     3403 2018-08-13 22:29:38.000000 SimPEG-0.9.4/tests/pf/test_forward_Mag_Linear.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/pf/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1697 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/pf/test_forward_PFproblem.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     5192 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/pf/test_grav_inversion_linear.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    11447 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/pf/test_sensitivity_PFproblem.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/tests/base/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    11642 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/base/test_utils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1828 2018-04-02 22:21:17.000000 SimPEG-0.9.4/tests/base/test_DataMisfit.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    13068 2018-11-19 01:28:05.000000 SimPEG-0.9.4/tests/base/test_maps.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    13632 2018-09-14 16:25:54.000000 SimPEG-0.9.4/tests/base/test_regularization.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2935 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/base/test_joint.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2863 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/base/test_SurveyAndData.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     7810 2017-12-18 23:17:14.000000 SimPEG-0.9.4/tests/base/test_Props.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     3906 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/base/test_directives.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2324 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/base/test_optimizers.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/base/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     9419 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/base/test_Objectivefct.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1751 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/base/test_Solver.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1727 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/base/test_coordutils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    16097 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/base/test_Fields.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1159 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/base/test_problem.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/tests/flow/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      385 2017-12-18 20:30:26.000000 SimPEG-0.9.4/tests/flow/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6750 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/flow/test_Richards_empirical.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     8601 2018-08-10 21:29:34.000000 SimPEG-0.9.4/tests/flow/test_Richards.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       22 2014-12-04 07:53:52.000000 SimPEG-0.9.4/MANIFEST.in
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      813 2016-02-11 00:13:44.000000 SimPEG-0.9.4/CITATION.rst
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1763 2018-12-09 17:13:05.000000 SimPEG-0.9.4/setup.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      848 2017-12-18 20:30:26.000000 SimPEG-0.9.4/AUTHORS.rst
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       38 2018-12-09 21:41:37.000000 SimPEG-0.9.4/setup.cfg
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4232 2018-11-03 02:23:34.000000 SimPEG-0.9.4/README.rst
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/NSEM/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       28 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/NSEM/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2301 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/Inversion.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    14479 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/Survey.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/SEIS/
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/SEIS/StraightRay/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      238 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/SEIS/StraightRay/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     3084 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/SEIS/StraightRay/StraightRayProblem.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      856 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/SEIS/StraightRay/StraightRaySurvey.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       26 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/SEIS/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    99497 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/Maps.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    14027 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/ObjectiveFunction.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/VRM/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    17385 2018-11-06 00:55:18.000000 SimPEG-0.9.4/SimPEG/VRM/WaveformVRM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2126 2018-11-06 00:55:18.000000 SimPEG-0.9.4/SimPEG/VRM/SurveyVRM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    36864 2018-11-06 00:55:18.000000 SimPEG-0.9.4/SimPEG/VRM/ProblemVRM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      222 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/VRM/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    13213 2018-11-06 00:55:18.000000 SimPEG-0.9.4/SimPEG/VRM/SrcVRM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     3076 2018-11-06 00:55:18.000000 SimPEG-0.9.4/SimPEG/VRM/RxVRM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1210 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/Models.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     9735 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/Fields.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6979 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/InvProblem.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     9251 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/SurveyNSEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    21456 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/FieldsNSEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    16323 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/ProblemNSEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      410 2018-03-02 18:15:07.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/__init__.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1364 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/MT1Dsolutions.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    18906 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/plotDataTypes.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4919 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/MT1Danalytic.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6614 2018-03-02 18:15:07.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/testUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      847 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     7680 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/sourceUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6927 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/ediFilesUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    16498 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/dataUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4746 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/data_viewer.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    29008 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/plotUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     9306 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/SrcNSEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    26166 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/NSEM/RxNSEM.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/TDEM/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    19368 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/EM/TDEM/SrcTDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      281 2018-05-01 17:37:09.000000 SimPEG-0.9.4/SimPEG/EM/TDEM/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     7121 2018-05-01 17:37:09.000000 SimPEG-0.9.4/SimPEG/EM/TDEM/RxTDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1021 2018-05-01 17:37:09.000000 SimPEG-0.9.4/SimPEG/EM/TDEM/SurveyTDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    24101 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/EM/TDEM/FieldsTDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    36983 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/EM/TDEM/ProblemTDEM.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/FDEM/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1794 2018-05-01 17:37:09.000000 SimPEG-0.9.4/SimPEG/EM/FDEM/SurveyFDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    55216 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/FDEM/FieldsFDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    26247 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/FDEM/ProblemFDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      234 2018-05-01 17:37:09.000000 SimPEG-0.9.4/SimPEG/EM/FDEM/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    27542 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/FDEM/SrcFDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     5432 2018-08-15 23:24:37.000000 SimPEG-0.9.4/SimPEG/EM/FDEM/RxFDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      226 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/__init__.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/Utils/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      304 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Utils/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     5799 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Utils/CurrentUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4489 2018-05-01 17:37:09.000000 SimPEG-0.9.4/SimPEG/EM/Utils/testingUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    12049 2018-06-26 22:23:41.000000 SimPEG-0.9.4/SimPEG/EM/Utils/AnalyticUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1772 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Utils/EMUtils.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/Static/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       72 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Static/__init__.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/Static/Utils/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    49374 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/Utils/StaticUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       27 2017-12-19 05:06:13.000000 SimPEG-0.9.4/SimPEG/EM/Static/Utils/__init__.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    15118 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/ProblemDC.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     5794 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/FieldsDC_2D.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2052 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/Run.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6947 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/BoundaryUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    13345 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/SurveyDC.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      461 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    20646 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/ProblemDC_2D.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    21738 2018-11-19 17:07:29.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/IODC.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1391 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/Utils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6928 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/FieldsDC.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6360 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/RxDC.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2298 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/DC/SrcDC.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/Static/SIP/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4829 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/SIP/Run.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    16462 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/SIP/ProblemSIP.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4640 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/SIP/SurveySIP.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      269 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/SIP/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     3466 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/SIP/RxSIP.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2142 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/SIP/SrcSIP.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    14200 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/SIP/ProblemSIP_2D.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/Static/IP/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2042 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/IP/Run.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     8506 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/IP/ProblemIP_2D.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      201 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/IP/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    10195 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/IP/ProblemIP.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1898 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Static/IP/SurveyIP.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    18936 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/EM/Base.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/EM/Analytics/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6656 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Analytics/DC.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      204 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Analytics/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    10268 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Analytics/FDEMDipolarfields.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      593 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Analytics/TDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4048 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Analytics/FDEMcasing.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4698 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Analytics/FDEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     5344 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/EM/Analytics/NSEM.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    36214 2018-08-13 22:29:38.000000 SimPEG-0.9.4/SimPEG/Optimization.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      740 2018-12-09 17:13:05.000000 SimPEG-0.9.4/SimPEG/__init__.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/Utils/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     7037 2018-08-12 04:48:05.000000 SimPEG-0.9.4/SimPEG/Utils/modelutils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     7794 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/Utils/printinfo.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     3207 2018-05-01 17:37:09.000000 SimPEG-0.9.4/SimPEG/Utils/CounterUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       96 2017-12-18 23:17:14.000000 SimPEG-0.9.4/SimPEG/Utils/meshutils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       59 2017-12-18 23:17:14.000000 SimPEG-0.9.4/SimPEG/Utils/curvutils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2379 2018-08-13 22:29:38.000000 SimPEG-0.9.4/SimPEG/Utils/matutils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    10959 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/Utils/ModelBuilder.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1027 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/Utils/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       80 2017-12-18 23:17:14.000000 SimPEG-0.9.4/SimPEG/Utils/coordutils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     6810 2018-10-24 20:10:13.000000 SimPEG-0.9.4/SimPEG/Utils/io_utils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     5303 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/Utils/SolverUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     8044 2018-12-09 17:12:25.000000 SimPEG-0.9.4/SimPEG/Utils/PlotUtils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     7341 2017-12-18 23:17:14.000000 SimPEG-0.9.4/SimPEG/Utils/codeutils.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    33407 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/Directives.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     8457 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/Problem.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/PF/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     5070 2018-08-13 22:29:38.000000 SimPEG-0.9.4/SimPEG/PF/BaseMag.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     1060 2018-08-13 22:29:38.000000 SimPEG-0.9.4/SimPEG/PF/GravAnalytics.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     9054 2018-08-13 22:29:38.000000 SimPEG-0.9.4/SimPEG/PF/GravityDriver.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      204 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/PF/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    14829 2018-08-13 22:29:38.000000 SimPEG-0.9.4/SimPEG/PF/Gravity.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    33553 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/PF/Magnetics.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    11448 2018-08-13 22:29:38.000000 SimPEG-0.9.4/SimPEG/PF/MagneticsDriver.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     2723 2018-08-13 22:29:38.000000 SimPEG-0.9.4/SimPEG/PF/BaseGrav.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     7637 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/PF/MagAnalytics.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/DC/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       90 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/DC/__init__.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/SIP/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       35 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/SIP/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    15924 2018-08-15 23:24:37.000000 SimPEG-0.9.4/SimPEG/Props.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     4582 2018-11-19 01:28:05.000000 SimPEG-0.9.4/SimPEG/DataMisfit.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/IP/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       34 2018-08-10 21:29:34.000000 SimPEG-0.9.4/SimPEG/IP/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    57743 2018-09-14 16:25:54.000000 SimPEG-0.9.4/SimPEG/Regularization.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/FLOW/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)       33 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/FLOW/__init__.py
+drwxr-xr-x   0 lindseyjh   (501) staff       (20)        0 2018-12-09 21:41:37.000000 SimPEG-0.9.4/SimPEG/FLOW/Richards/
+-rw-r--r--   0 lindseyjh   (501) staff       (20)     3985 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/FLOW/Richards/RichardsSurvey.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)      144 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/FLOW/Richards/__init__.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    11130 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/FLOW/Richards/RichardsProblem.py
+-rw-r--r--   0 lindseyjh   (501) staff       (20)    27201 2017-12-18 20:30:26.000000 SimPEG-0.9.4/SimPEG/FLOW/Richards/Empirical.py
```

### Comparing `SimPEG-0.9.3/PKG-INFO` & `SimPEG-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SimPEG
-Version: 0.9.3
+Version: 0.9.4
 Summary: SimPEG: Simulation and Parameter Estimation in Geophysics
 Home-page: http://simpeg.xyz/
 Author: Rowan Cockett
 Author-email: rowanc1@gmail.com
 License: MIT
 Download-URL: http://github.com/simpeg/simpeg
 Description: .. image:: https://raw.github.com/simpeg/simpeg/master/docs/images/simpeg-logo.png
```

### Comparing `SimPEG-0.9.3/SimPEG.egg-info/PKG-INFO` & `SimPEG-0.9.4/SimPEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SimPEG
-Version: 0.9.3
+Version: 0.9.4
 Summary: SimPEG: Simulation and Parameter Estimation in Geophysics
 Home-page: http://simpeg.xyz/
 Author: Rowan Cockett
 Author-email: rowanc1@gmail.com
 License: MIT
 Download-URL: http://github.com/simpeg/simpeg
 Description: .. image:: https://raw.github.com/simpeg/simpeg/master/docs/images/simpeg-logo.png
```

### Comparing `SimPEG-0.9.3/SimPEG.egg-info/SOURCES.txt` & `SimPEG-0.9.4/SimPEG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/LICENSE` & `SimPEG-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/CONTRIBUTING.rst` & `SimPEG-0.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/seis/test_tomo.py` & `SimPEG-0.9.4/tests/seis/test_tomo.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/utils/test_printinfo.py` & `SimPEG-0.9.4/tests/utils/test_printinfo.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/pf/test_magnetics_IO.py` & `SimPEG-0.9.4/tests/pf/test_magnetics_IO.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/pf/test_gravity_IO.py` & `SimPEG-0.9.4/tests/pf/test_gravity_IO.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/pf/test_mag_inversion_linear.py` & `SimPEG-0.9.4/tests/pf/test_mag_inversion_linear.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/pf/test_magnetics_analytics.py` & `SimPEG-0.9.4/tests/pf/test_magnetics_analytics.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/pf/test_forward_Grav_Linear.py` & `SimPEG-0.9.4/tests/pf/test_forward_Grav_Linear.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/pf/test_forward_Mag_Linear.py` & `SimPEG-0.9.4/tests/pf/test_forward_Mag_Linear.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/pf/test_forward_PFproblem.py` & `SimPEG-0.9.4/tests/pf/test_forward_PFproblem.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/pf/test_grav_inversion_linear.py` & `SimPEG-0.9.4/tests/pf/test_grav_inversion_linear.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/pf/test_sensitivity_PFproblem.py` & `SimPEG-0.9.4/tests/pf/test_sensitivity_PFproblem.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_utils.py` & `SimPEG-0.9.4/tests/base/test_utils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_DataMisfit.py` & `SimPEG-0.9.4/tests/base/test_DataMisfit.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_maps.py` & `SimPEG-0.9.4/tests/base/test_maps.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_regularization.py` & `SimPEG-0.9.4/tests/base/test_regularization.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_joint.py` & `SimPEG-0.9.4/tests/base/test_joint.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_SurveyAndData.py` & `SimPEG-0.9.4/tests/base/test_SurveyAndData.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_Props.py` & `SimPEG-0.9.4/tests/base/test_Props.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_directives.py` & `SimPEG-0.9.4/tests/base/test_directives.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_optimizers.py` & `SimPEG-0.9.4/tests/base/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_Objectivefct.py` & `SimPEG-0.9.4/tests/base/test_Objectivefct.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_Solver.py` & `SimPEG-0.9.4/tests/base/test_Solver.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_coordutils.py` & `SimPEG-0.9.4/tests/base/test_coordutils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_Fields.py` & `SimPEG-0.9.4/tests/base/test_Fields.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/base/test_problem.py` & `SimPEG-0.9.4/tests/base/test_problem.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/flow/test_Richards_empirical.py` & `SimPEG-0.9.4/tests/flow/test_Richards_empirical.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/tests/flow/test_Richards.py` & `SimPEG-0.9.4/tests/flow/test_Richards.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/CITATION.rst` & `SimPEG-0.9.4/CITATION.rst`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/setup.py` & `SimPEG-0.9.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 ]
 
 with open("README.rst") as f:
     LONG_DESCRIPTION = ''.join(f.readlines())
 
 setup(
     name="SimPEG",
-    version="0.9.3",
-    packages=find_packages(),
+    version="0.9.4",
+    packages=find_packages(exclude=['tests*']),
     install_requires=[
         'numpy>=1.7',
         'scipy>=0.13',
         'cython',
         'pymatsolver>=0.1.1',
         'ipython',
         'matplotlib',
```

### Comparing `SimPEG-0.9.3/AUTHORS.rst` & `SimPEG-0.9.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/README.rst` & `SimPEG-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Inversion.py` & `SimPEG-0.9.4/SimPEG/Inversion.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Survey.py` & `SimPEG-0.9.4/SimPEG/Survey.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/SEIS/StraightRay/StraightRayProblem.py` & `SimPEG-0.9.4/SimPEG/SEIS/StraightRay/StraightRayProblem.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/SEIS/StraightRay/StraightRaySurvey.py` & `SimPEG-0.9.4/SimPEG/SEIS/StraightRay/StraightRaySurvey.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Maps.py` & `SimPEG-0.9.4/SimPEG/Maps.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/ObjectiveFunction.py` & `SimPEG-0.9.4/SimPEG/ObjectiveFunction.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/VRM/WaveformVRM.py` & `SimPEG-0.9.4/SimPEG/VRM/WaveformVRM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/VRM/SurveyVRM.py` & `SimPEG-0.9.4/SimPEG/VRM/SurveyVRM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/VRM/ProblemVRM.py` & `SimPEG-0.9.4/SimPEG/VRM/ProblemVRM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/VRM/SrcVRM.py` & `SimPEG-0.9.4/SimPEG/VRM/SrcVRM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/VRM/RxVRM.py` & `SimPEG-0.9.4/SimPEG/VRM/RxVRM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Models.py` & `SimPEG-0.9.4/SimPEG/Models.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Fields.py` & `SimPEG-0.9.4/SimPEG/Fields.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/InvProblem.py` & `SimPEG-0.9.4/SimPEG/InvProblem.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/SurveyNSEM.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/SurveyNSEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/FieldsNSEM.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/FieldsNSEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/ProblemNSEM.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/ProblemNSEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/MT1Dsolutions.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/MT1Dsolutions.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/plotDataTypes.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/plotDataTypes.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/MT1Danalytic.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/MT1Danalytic.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/testUtils.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/testUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/__init__.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/sourceUtils.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/sourceUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/ediFilesUtils.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/ediFilesUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/dataUtils.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/dataUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/data_viewer.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/data_viewer.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/Utils/plotUtils.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/Utils/plotUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/SrcNSEM.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/SrcNSEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/NSEM/RxNSEM.py` & `SimPEG-0.9.4/SimPEG/EM/NSEM/RxNSEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/TDEM/SrcTDEM.py` & `SimPEG-0.9.4/SimPEG/EM/TDEM/SrcTDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/TDEM/RxTDEM.py` & `SimPEG-0.9.4/SimPEG/EM/TDEM/RxTDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/TDEM/SurveyTDEM.py` & `SimPEG-0.9.4/SimPEG/EM/TDEM/SurveyTDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/TDEM/FieldsTDEM.py` & `SimPEG-0.9.4/SimPEG/EM/TDEM/FieldsTDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/TDEM/ProblemTDEM.py` & `SimPEG-0.9.4/SimPEG/EM/TDEM/ProblemTDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/FDEM/SurveyFDEM.py` & `SimPEG-0.9.4/SimPEG/EM/FDEM/SurveyFDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/FDEM/FieldsFDEM.py` & `SimPEG-0.9.4/SimPEG/EM/FDEM/FieldsFDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/FDEM/ProblemFDEM.py` & `SimPEG-0.9.4/SimPEG/EM/FDEM/ProblemFDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/FDEM/SrcFDEM.py` & `SimPEG-0.9.4/SimPEG/EM/FDEM/SrcFDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/FDEM/RxFDEM.py` & `SimPEG-0.9.4/SimPEG/EM/FDEM/RxFDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Utils/CurrentUtils.py` & `SimPEG-0.9.4/SimPEG/EM/Utils/CurrentUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Utils/testingUtils.py` & `SimPEG-0.9.4/SimPEG/EM/Utils/testingUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Utils/AnalyticUtils.py` & `SimPEG-0.9.4/SimPEG/EM/Utils/AnalyticUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Utils/EMUtils.py` & `SimPEG-0.9.4/SimPEG/EM/Utils/EMUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/Utils/StaticUtils.py` & `SimPEG-0.9.4/SimPEG/EM/Static/Utils/StaticUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/ProblemDC.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/ProblemDC.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/FieldsDC_2D.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/FieldsDC_2D.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/Run.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/Run.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/BoundaryUtils.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/BoundaryUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/SurveyDC.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/SurveyDC.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/ProblemDC_2D.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/ProblemDC_2D.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/IODC.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/IODC.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/Utils.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/Utils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/FieldsDC.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/FieldsDC.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/RxDC.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/RxDC.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/DC/SrcDC.py` & `SimPEG-0.9.4/SimPEG/EM/Static/DC/SrcDC.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/SIP/Run.py` & `SimPEG-0.9.4/SimPEG/EM/Static/SIP/Run.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/SIP/ProblemSIP.py` & `SimPEG-0.9.4/SimPEG/EM/Static/SIP/ProblemSIP.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/SIP/SurveySIP.py` & `SimPEG-0.9.4/SimPEG/EM/Static/SIP/SurveySIP.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/SIP/RxSIP.py` & `SimPEG-0.9.4/SimPEG/EM/Static/SIP/RxSIP.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/SIP/SrcSIP.py` & `SimPEG-0.9.4/SimPEG/EM/Static/SIP/SrcSIP.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/SIP/ProblemSIP_2D.py` & `SimPEG-0.9.4/SimPEG/EM/Static/SIP/ProblemSIP_2D.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/IP/Run.py` & `SimPEG-0.9.4/SimPEG/EM/Static/IP/Run.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/IP/ProblemIP_2D.py` & `SimPEG-0.9.4/SimPEG/EM/Static/IP/ProblemIP_2D.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/IP/ProblemIP.py` & `SimPEG-0.9.4/SimPEG/EM/Static/IP/ProblemIP.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Static/IP/SurveyIP.py` & `SimPEG-0.9.4/SimPEG/EM/Static/IP/SurveyIP.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Base.py` & `SimPEG-0.9.4/SimPEG/EM/Base.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Analytics/DC.py` & `SimPEG-0.9.4/SimPEG/EM/Analytics/DC.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Analytics/FDEMDipolarfields.py` & `SimPEG-0.9.4/SimPEG/EM/Analytics/FDEMDipolarfields.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Analytics/TDEM.py` & `SimPEG-0.9.4/SimPEG/EM/Analytics/TDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Analytics/FDEMcasing.py` & `SimPEG-0.9.4/SimPEG/EM/Analytics/FDEMcasing.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Analytics/FDEM.py` & `SimPEG-0.9.4/SimPEG/EM/Analytics/FDEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/EM/Analytics/NSEM.py` & `SimPEG-0.9.4/SimPEG/EM/Analytics/NSEM.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Optimization.py` & `SimPEG-0.9.4/SimPEG/Optimization.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/__init__.py` & `SimPEG-0.9.4/SimPEG/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 from . import Utils
 from .Utils import mkvc
 from .Utils import versions
 from .Utils.SolverUtils import (
     _checkAccuracy, SolverWrapD, SolverWrapI,
     Solver, SolverCG, SolverDiag, SolverLU, SolverBiCG,
 )
-__version__   = '0.9.3'
+__version__   = '0.9.4'
 __author__    = 'SimPEG Team'
 __license__   = 'MIT'
 __copyright__ = '2013 - 2018, SimPEG Team, http://simpeg.xyz'
```

### Comparing `SimPEG-0.9.3/SimPEG/Utils/modelutils.py` & `SimPEG-0.9.4/SimPEG/Utils/modelutils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Utils/printinfo.py` & `SimPEG-0.9.4/SimPEG/Utils/printinfo.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Utils/CounterUtils.py` & `SimPEG-0.9.4/SimPEG/Utils/CounterUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Utils/matutils.py` & `SimPEG-0.9.4/SimPEG/Utils/matutils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Utils/ModelBuilder.py` & `SimPEG-0.9.4/SimPEG/Utils/ModelBuilder.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Utils/__init__.py` & `SimPEG-0.9.4/SimPEG/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Utils/io_utils.py` & `SimPEG-0.9.4/SimPEG/Utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Utils/SolverUtils.py` & `SimPEG-0.9.4/SimPEG/Utils/SolverUtils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Utils/PlotUtils.py` & `SimPEG-0.9.4/SimPEG/Utils/PlotUtils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 import numpy as np
-from scipy.interpolate import LinearNDInterpolator
+from scipy.interpolate import LinearNDInterpolator, NearestNDInterpolator
 import matplotlib.pyplot as plt
 
 
-def plot2Ddata(xyz, data, vec=False, nx=100, ny=100,
-               ax=None, mask=None, level=None, figname=None,
-               ncontour=10, dataloc=False, contourOpts={},
-               scale="linear", clim=None):
+def plot2Ddata(
+    xyz, data, vec=False, nx=100, ny=100,
+    ax=None, mask=None, level=False, figname=None,
+    ncontour=10, dataloc=False, contourOpts={},
+    levelOpts={}, scale="linear", clim=None,
+    method='linear'
+):
     """
 
         Take unstructured xy points, interpolate, then plot in 2D
 
         :param numpy.array xyz: data locations
         :param numpy.array data: data values
         :param bool vec: plot streamplot?
         :param float nx: number of x grid locations
         :param float ny: number of y grid locations
         :param matplotlib.axes ax: axes
-        :param numpy.array mask: mask for the array
-        :param float level: level at which to draw a contour
+        :param boolean numpy.array mask: mask for the array
+        :param boolean level: boolean to plot (or not)
+                                :meth:`matplotlib.pyplot.contour`
         :param string figname: figure name
         :param float ncontour: number of :meth:`matplotlib.pyplot.contourf`
-                               contours
+                                contours
         :param bool dataloc: plot the data locations
         :param dict controuOpts: :meth:`matplotlib.pyplot.contourf` options
+        :param dict levelOpts: :meth:`matplotlib.pyplot.contour` options
         :param numpy.array clim: colorbar limits
+        :param str method: interpolation method, either 'linear' or 'nearest'
 
     """
     if ax is None:
         fig = plt.figure()
         ax = plt.subplot(111)
 
     xmin, xmax = xyz[:, 0].min(), xyz[:, 0].max()
     ymin, ymax = xyz[:, 1].min(), xyz[:, 1].max()
     x = np.linspace(xmin, xmax, nx)
     y = np.linspace(ymin, ymax, ny)
     X, Y = np.meshgrid(x, y)
     xy = np.c_[X.flatten(), Y.flatten()]
     if vec is False:
-        F = LinearNDInterpolator(xyz[:, :2], data)
+        if method == 'nearest':
+            F = NearestNDInterpolator(xyz[:, :2], data)
+        else:
+            F = LinearNDInterpolator(xyz[:, :2], data)
         DATA = F(xy)
         DATA = DATA.reshape(X.shape)
         if scale == "log":
             DATA = np.log10(abs(DATA))
 
         # Levels definitions
         dataselection = np.logical_and(
             ~np.isnan(DATA),
             np.abs(DATA) != np.inf
             )
         if clim is None:
             vmin = DATA[dataselection].min()
             vmax = DATA[dataselection].max()
+        elif np.logical_and(
+            'vmin' in contourOpts.keys(),
+            'vmax' in contourOpts.keys()
+        ):
+            vmin = contourOpts['vmin']
+            vmax = contourOpts['vmax']
         else:
             vmin = np.min(clim)
             vmax = np.max(clim)
             if scale == "log":
                 vmin = np.log10(vmin)
                 vmax = np.log10(vmax)
         if np.logical_or(
@@ -69,35 +84,47 @@
             )
         ):
             raise Exception(
                 """clim must be sctrictly positive in log scale"""
             )
         vstep = np.abs((vmin-vmax)/(ncontour+1))
         levels = np.arange(vmin, vmax+vstep, vstep)
-        if DATA[dataselection].min() < vmin:
+        if DATA[dataselection].min() < levels.min():
                 levels = np.r_[DATA[dataselection].min(), levels]
-        if DATA[dataselection].max() > vmax:
+        if DATA[dataselection].max() > levels.max():
                 levels = np.r_[levels, DATA[dataselection].max()]
 
+        if mask is not None:
+            Fmask = NearestNDInterpolator(xyz[:, :2], mask)
+            MASK = Fmask(xy)
+            MASK = MASK.reshape(X.shape)
+            DATA = np.ma.masked_array(DATA, mask=MASK)
+
+        if 'vmin' not in contourOpts.keys():
+            contourOpts['vmin'] = vmin
+        if 'vmax' not in contourOpts.keys():
+            contourOpts['vmax'] = vmax
+
         cont = ax.contourf(
             X, Y, DATA, levels=levels,
-            vmin=vmin, vmax=vmax,
             **contourOpts
         )
-        if level is not None:
-            if scale == "log":
-                level = np.log10(level)
-            CS = ax.contour(X, Y, DATA, level, colors="k", linewidths=2)
+        if level:
+            CS = ax.contour(X, Y, DATA, levels=levels, **levelOpts)
 
     else:
         # Assume size of data is (N,2)
         datax = data[:, 0]
         datay = data[:, 1]
-        Fx = LinearNDInterpolator(xyz[:, :2], datax)
-        Fy = LinearNDInterpolator(xyz[:, :2], datay)
+        if method == 'nearest':
+            Fx = NearestNDInterpolator(xyz[:, :2], datax)
+            Fy = NearestNDInterpolator(xyz[:, :2], datay)
+        else:
+            Fx = LinearNDInterpolator(xyz[:, :2], datax)
+            Fy = LinearNDInterpolator(xyz[:, :2], datay)
         DATAx = Fx(xy)
         DATAy = Fy(xy)
         DATA = np.sqrt(DATAx**2+DATAy**2).reshape(X.shape)
         DATAx = DATAx.reshape(X.shape)
         DATAy = DATAy.reshape(X.shape)
         if scale == "log":
             DATA = np.log10(abs(DATA))
@@ -127,38 +154,44 @@
             )
         ):
             raise Exception(
                 """clim must be sctrictly positive in log scale"""
             )
         vstep = np.abs((vmin-vmax)/(ncontour+1))
         levels = np.arange(vmin, vmax+vstep, vstep)
-        if DATA[dataselection].min() < vmin:
+        if DATA[dataselection].min() < levels.min():
                 levels = np.r_[DATA[dataselection].min(), levels]
-        if DATA[dataselection].max() > vmax:
+        if DATA[dataselection].max() > levels.max():
                 levels = np.r_[levels, DATA[dataselection].max()]
 
+        if mask is not None:
+            Fmask = NearestNDInterpolator(xyz[:, :2], mask)
+            MASK = Fmask(xy)
+            MASK = MASK.reshape(X.shape)
+            DATA = np.ma.masked_array(DATA, mask=MASK)
+
         cont = ax.contourf(
             X, Y, DATA, levels=levels,
             vmin=vmin, vmax=vmax,
             **contourOpts
         )
         ax.streamplot(X, Y, DATAx, DATAy, color="w")
-        if level is not None:
-            CS = ax.contour(X, Y, DATA, level, colors="k", linewidths=2)
+        if level:
+            CS = ax.contour(X, Y, DATA, levels=levels, **levelOpts)
 
     if dataloc:
         ax.plot(xyz[:, 0], xyz[:, 1], 'k.', ms=2)
     plt.gca().set_aspect('equal', adjustable='box')
     if figname:
         plt.axis("off")
         fig.savefig(figname, dpi=200)
-    if level is None:
-        return cont, ax
-    else:
+    if level:
         return cont, ax, CS
+    else:
+        return cont, ax
 
 
 def plotLayer(sig, LocSigZ, xscale='log', ax=None,
               showlayers=False, xlim=None, **kwargs):
     """Plot a layered earth model"""
     sigma = np.repeat(sig, 2, axis=0)
     z = np.repeat(LocSigZ[1:], 2, axis=0)
```

### Comparing `SimPEG-0.9.3/SimPEG/Utils/codeutils.py` & `SimPEG-0.9.4/SimPEG/Utils/codeutils.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Directives.py` & `SimPEG-0.9.4/SimPEG/Directives.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Problem.py` & `SimPEG-0.9.4/SimPEG/Problem.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/PF/BaseMag.py` & `SimPEG-0.9.4/SimPEG/PF/BaseMag.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/PF/GravAnalytics.py` & `SimPEG-0.9.4/SimPEG/PF/GravAnalytics.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/PF/GravityDriver.py` & `SimPEG-0.9.4/SimPEG/PF/GravityDriver.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/PF/Gravity.py` & `SimPEG-0.9.4/SimPEG/PF/Gravity.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/PF/Magnetics.py` & `SimPEG-0.9.4/SimPEG/PF/Magnetics.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/PF/MagneticsDriver.py` & `SimPEG-0.9.4/SimPEG/PF/MagneticsDriver.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/PF/BaseGrav.py` & `SimPEG-0.9.4/SimPEG/PF/BaseGrav.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/PF/MagAnalytics.py` & `SimPEG-0.9.4/SimPEG/PF/MagAnalytics.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Props.py` & `SimPEG-0.9.4/SimPEG/Props.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/DataMisfit.py` & `SimPEG-0.9.4/SimPEG/DataMisfit.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/Regularization.py` & `SimPEG-0.9.4/SimPEG/Regularization.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/FLOW/Richards/RichardsSurvey.py` & `SimPEG-0.9.4/SimPEG/FLOW/Richards/RichardsSurvey.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/FLOW/Richards/RichardsProblem.py` & `SimPEG-0.9.4/SimPEG/FLOW/Richards/RichardsProblem.py`

 * *Files identical despite different names*

### Comparing `SimPEG-0.9.3/SimPEG/FLOW/Richards/Empirical.py` & `SimPEG-0.9.4/SimPEG/FLOW/Richards/Empirical.py`

 * *Files identical despite different names*

